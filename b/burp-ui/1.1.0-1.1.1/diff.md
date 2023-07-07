# Comparing `tmp/burp-ui-1.1.0.tar.gz` & `tmp/burp-ui-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burp-ui-1.1.0.tar", last modified: Mon May  1 19:13:30 2023, max compression
+gzip compressed data, was "burp-ui-1.1.1.tar", last modified: Fri Jul  7 18:24:28 2023, max compression
```

## Comparing `burp-ui-1.1.0.tar` & `burp-ui-1.1.1.tar`

### file list

```diff
@@ -1,517 +1,517 @@
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.148662 burp-ui-1.1.0/
--rw-r--r--   0 master    (1000) master    (1000)    22785 2023-05-01 19:11:44.000000 burp-ui-1.1.0/CHANGELOG.rst
--rw-r--r--   0 master    (1000) master    (1000)      368 2022-11-06 21:20:42.000000 burp-ui-1.1.0/CONTRIBUTORS
--rw-r--r--   0 master    (1000) master    (1000)     1575 2018-05-14 12:28:48.000000 burp-ui-1.1.0/LICENSE
--rw-r--r--   0 master    (1000) master    (1000)      342 2022-11-06 21:20:42.000000 burp-ui-1.1.0/MANIFEST.in
--rw-r--r--   0 master    (1000) master    (1000)     5873 2023-05-01 19:13:30.148662 burp-ui-1.1.0/PKG-INFO
--rw-r--r--   0 master    (1000) master    (1000)     5025 2022-11-06 21:20:42.000000 burp-ui-1.1.0/README.rst
--rw-r--r--   0 master    (1000) master    (1000)      229 2017-04-28 13:40:18.000000 burp-ui-1.1.0/babel.cfg
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.096661 burp-ui-1.1.0/burp_ui.egg-info/
--rw-r--r--   0 master    (1000) master    (1000)     5873 2023-05-01 19:13:30.000000 burp-ui-1.1.0/burp_ui.egg-info/PKG-INFO
--rw-r--r--   0 master    (1000) master    (1000)    15086 2023-05-01 19:13:30.000000 burp-ui-1.1.0/burp_ui.egg-info/SOURCES.txt
--rw-r--r--   0 master    (1000) master    (1000)        1 2023-05-01 19:13:30.000000 burp-ui-1.1.0/burp_ui.egg-info/dependency_links.txt
--rw-r--r--   0 master    (1000) master    (1000)      243 2023-05-01 19:13:30.000000 burp-ui-1.1.0/burp_ui.egg-info/entry_points.txt
--rw-r--r--   0 master    (1000) master    (1000)      755 2023-05-01 19:13:30.000000 burp-ui-1.1.0/burp_ui.egg-info/requires.txt
--rw-r--r--   0 master    (1000) master    (1000)        7 2023-05-01 19:13:30.000000 burp-ui-1.1.0/burp_ui.egg-info/top_level.txt
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.100661 burp-ui-1.1.0/burpui/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.100661 burp-ui-1.1.0/burpui/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4829 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)    12191 2019-10-03 09:41:02.000000 burp-ui-1.1.0/burpui/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2018-06-05 15:54:46.000000 burp-ui-1.1.0/burpui/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)      779 2019-10-03 09:41:02.000000 burp-ui-1.1.0/burpui/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.000000 burp-ui-1.1.0/burpui/RELEASE
--rw-r--r--   0 master    (1000) master    (1000)        6 2023-05-01 19:11:44.000000 burp-ui-1.1.0/burpui/VERSION
--rw-r--r--   0 master    (1000) master    (1000)      382 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)     9535 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/__main__.py
--rw-r--r--   0 master    (1000) master    (1000)      249 2021-05-12 15:45:53.000000 burp-ui-1.1.0/burpui/_cli.py
--rw-r--r--   0 master    (1000) master    (1000)     2058 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/_compat.py
--rw-r--r--   0 master    (1000) master    (1000)     1202 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/_json.py
--rw-r--r--   0 master    (1000) master    (1000)      397 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/_rtfd.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.104661 burp-ui-1.1.0/burpui/api/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.104661 burp-ui-1.1.0/burpui/api/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4794 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/api/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)     2643 2018-09-14 14:17:22.000000 burp-ui-1.1.0/burpui/api/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2018-07-23 14:42:15.000000 burp-ui-1.1.0/burpui/api/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)        6 2018-09-14 14:17:22.000000 burp-ui-1.1.0/burpui/api/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)     8428 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)    60894 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/admin.py
--rw-r--r--   0 master    (1000) master    (1000)     4961 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/backup.py
--rw-r--r--   0 master    (1000) master    (1000)    36404 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/client.py
--rw-r--r--   0 master    (1000) master    (1000)    25725 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/clients.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.104661 burp-ui-1.1.0/burpui/api/custom/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.104661 burp-ui-1.1.0/burpui/api/custom/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4794 2019-10-01 14:25:10.000000 burp-ui-1.1.0/burpui/api/custom/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)      291 2019-10-01 14:25:10.000000 burp-ui-1.1.0/burpui/api/custom/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2019-10-01 14:25:10.000000 burp-ui-1.1.0/burpui/api/custom/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)        6 2019-10-01 14:25:10.000000 burp-ui-1.1.0/burpui/api/custom/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)      213 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/api/custom/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)      585 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/custom/fields.py
--rw-r--r--   0 master    (1000) master    (1000)     2860 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/custom/my_fields.py
--rw-r--r--   0 master    (1000) master    (1000)     1430 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/api/custom/resource.py
--rw-r--r--   0 master    (1000) master    (1000)    35378 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/misc.py
--rw-r--r--   0 master    (1000) master    (1000)     8585 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/prefs.py
--rw-r--r--   0 master    (1000) master    (1000)    17608 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/restore.py
--rw-r--r--   0 master    (1000) master    (1000)     8028 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/servers.py
--rw-r--r--   0 master    (1000) master    (1000)    35800 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/settings.py
--rw-r--r--   0 master    (1000) master    (1000)    32795 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/tasks.py
--rw-r--r--   0 master    (1000) master    (1000)    15706 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/app.py
--rw-r--r--   0 master    (1000) master    (1000)    16384 2017-07-26 14:40:04.000000 burp-ui-1.1.0/burpui/celerybeat-schedule
--rw-r--r--   0 master    (1000) master    (1000)    45118 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/cli.py
--rw-r--r--   0 master    (1000) master    (1000)    10045 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/config.py
--rw-r--r--   0 master    (1000) master    (1000)    23767 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/datastructures.py
--rw-r--r--   0 master    (1000) master    (1000)     2768 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/decorators.py
--rw-r--r--   0 master    (1000) master    (1000)      964 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/desc.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.104661 burp-ui-1.1.0/burpui/engines/
--rw-r--r--   0 master    (1000) master    (1000)        0 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/engines/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)    14171 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/engines/agent.py
--rw-r--r--   0 master    (1000) master    (1000)    11302 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/engines/monitor.py
--rw-r--r--   0 master    (1000) master    (1000)    17914 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/engines/server.py
--rw-r--r--   0 master    (1000) master    (1000)      943 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/engines/worker.py
--rw-r--r--   0 master    (1000) master    (1000)      871 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/exceptions.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.104661 burp-ui-1.1.0/burpui/ext/
--rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/ext/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)      371 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/ext/cache.py
--rw-r--r--   0 master    (1000) master    (1000)      926 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/ext/i18n.py
--rw-r--r--   0 master    (1000) master    (1000)      309 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/ext/limit.py
--rw-r--r--   0 master    (1000) master    (1000)      233 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/ext/session.py
--rw-r--r--   0 master    (1000) master    (1000)      232 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/ext/sql.py
--rw-r--r--   0 master    (1000) master    (1000)      230 2019-04-02 19:43:50.000000 burp-ui-1.1.0/burpui/ext/tasks.py
--rw-r--r--   0 master    (1000) master    (1000)      545 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/ext/ws.py
--rw-r--r--   0 master    (1000) master    (1000)    11897 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/extensions.py
--rw-r--r--   0 master    (1000) master    (1000)     3524 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/filter.py
--rw-r--r--   0 master    (1000) master    (1000)      728 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/forms.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.104661 burp-ui-1.1.0/burpui/misc/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.108661 burp-ui-1.1.0/burpui/misc/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4794 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/misc/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)     2452 2018-07-23 07:59:35.000000 burp-ui-1.1.0/burpui/misc/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2018-07-20 15:54:46.000000 burp-ui-1.1.0/burpui/misc/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)        6 2018-07-23 07:59:35.000000 burp-ui-1.1.0/burpui/misc/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/misc/__init__.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.108661 burp-ui-1.1.0/burpui/misc/acl/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.108661 burp-ui-1.1.0/burpui/misc/acl/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4794 2019-09-24 13:37:49.000000 burp-ui-1.1.0/burpui/misc/acl/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)      346 2019-09-27 12:40:13.000000 burp-ui-1.1.0/burpui/misc/acl/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2019-09-25 20:15:11.000000 burp-ui-1.1.0/burpui/misc/acl/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)        6 2019-09-27 12:40:13.000000 burp-ui-1.1.0/burpui/misc/acl/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/misc/acl/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)    14445 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/acl/basic.py
--rw-r--r--   0 master    (1000) master    (1000)     5655 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/acl/handler.py
--rw-r--r--   0 master    (1000) master    (1000)     5389 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/acl/interface.py
--rw-r--r--   0 master    (1000) master    (1000)    28562 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/acl/meta.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.108661 burp-ui-1.1.0/burpui/misc/audit/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.108661 burp-ui-1.1.0/burpui/misc/audit/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4829 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/misc/audit/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)      138 2018-08-03 09:24:44.000000 burp-ui-1.1.0/burpui/misc/audit/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2018-06-05 13:59:15.000000 burp-ui-1.1.0/burpui/misc/audit/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)       27 2018-08-03 09:24:44.000000 burp-ui-1.1.0/burpui/misc/audit/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)        0 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/misc/audit/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)     2804 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/audit/basic.py
--rw-r--r--   0 master    (1000) master    (1000)     3591 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/audit/handler.py
--rw-r--r--   0 master    (1000) master    (1000)     1854 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/audit/interface.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.108661 burp-ui-1.1.0/burpui/misc/auth/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.108661 burp-ui-1.1.0/burpui/misc/auth/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4829 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/misc/auth/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)      763 2019-01-29 14:01:08.000000 burp-ui-1.1.0/burpui/misc/auth/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2018-06-07 15:21:13.000000 burp-ui-1.1.0/burpui/misc/auth/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)     2077 2019-01-29 14:01:08.000000 burp-ui-1.1.0/burpui/misc/auth/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/misc/auth/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)     9656 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/auth/basic.py
--rw-r--r--   0 master    (1000) master    (1000)    10821 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/auth/handler.py
--rw-r--r--   0 master    (1000) master    (1000)     3489 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/auth/interface.py
--rw-r--r--   0 master    (1000) master    (1000)    11181 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/auth/ldap.py
--rw-r--r--   0 master    (1000) master    (1000)     4675 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/auth/local.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.112661 burp-ui-1.1.0/burpui/misc/backend/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.112661 burp-ui-1.1.0/burpui/misc/backend/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4829 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/misc/backend/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)     1168 2020-05-08 22:06:12.000000 burp-ui-1.1.0/burpui/misc/backend/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2018-07-18 09:19:37.000000 burp-ui-1.1.0/burpui/misc/backend/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)        6 2020-05-08 22:06:12.000000 burp-ui-1.1.0/burpui/misc/backend/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/misc/backend/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)    47346 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/backend/burp1.py
--rw-r--r--   0 master    (1000) master    (1000)    30620 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/backend/burp2.py
--rw-r--r--   0 master    (1000) master    (1000)    41267 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/backend/interface.py
--rw-r--r--   0 master    (1000) master    (1000)    23472 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/backend/multi.py
--rw-r--r--   0 master    (1000) master    (1000)    38354 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/backend/parallel.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.112661 burp-ui-1.1.0/burpui/misc/backend/utils/
--rw-r--r--   0 master    (1000) master    (1000)        0 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/misc/backend/utils/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)    12735 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/backend/utils/burp2.py
--rw-r--r--   0 master    (1000) master    (1000)      398 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/misc/backend/utils/constant.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.112661 burp-ui-1.1.0/burpui/misc/parser/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.112661 burp-ui-1.1.0/burpui/misc/parser/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4794 2019-10-01 12:38:25.000000 burp-ui-1.1.0/burpui/misc/parser/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)      431 2021-10-04 08:39:12.000000 burp-ui-1.1.0/burpui/misc/parser/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2019-10-03 09:34:38.000000 burp-ui-1.1.0/burpui/misc/parser/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)        6 2021-10-04 08:39:12.000000 burp-ui-1.1.0/burpui/misc/parser/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/misc/parser/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)    37464 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/parser/burp1.py
--rw-r--r--   0 master    (1000) master    (1000)    13883 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/parser/burp2.py
--rw-r--r--   0 master    (1000) master    (1000)    43592 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/misc/parser/doc.py
--rw-r--r--   0 master    (1000) master    (1000)    17679 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/misc/parser/interface.py
--rw-r--r--   0 master    (1000) master    (1000)     8075 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/parser/openssl.py
--rw-r--r--   0 master    (1000) master    (1000)    57165 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/parser/utils.py
--rw-r--r--   0 master    (1000) master    (1000)     3399 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/models.py
--rw-r--r--   0 master    (1000) master    (1000)     2642 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/plugins.py
--rw-r--r--   0 master    (1000) master    (1000)    17427 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/routes.py
--rw-r--r--   0 master    (1000) master    (1000)     2913 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/security.py
--rw-r--r--   0 master    (1000) master    (1000)    11088 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/sessions.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.112661 burp-ui-1.1.0/burpui/static/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.088661 burp-ui-1.1.0/burpui/static/3rdparty/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.112661 burp-ui-1.1.0/burpui/static/3rdparty/highlightjs/
--rw-r--r--   0 master    (1000) master    (1000)     8711 2018-05-14 12:28:49.000000 burp-ui-1.1.0/burpui/static/3rdparty/highlightjs/highlight.pack.js
--rw-r--r--   0 master    (1000) master    (1000)     1211 2018-05-14 12:28:49.000000 burp-ui-1.1.0/burpui/static/3rdparty/highlightjs/style.css
--rw-r--r--   0 master    (1000) master    (1000)     7298 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/static/dashboard.css
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.088661 burp-ui-1.1.0/burpui/static/extra/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.112661 burp-ui-1.1.0/burpui/static/extra/i18n/
--rw-r--r--   0 master    (1000) master    (1000)      885 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/static/extra/i18n/datatable-es.json
--rw-r--r--   0 master    (1000) master    (1000)      990 2017-04-28 13:40:18.000000 burp-ui-1.1.0/burpui/static/extra/i18n/datatable-fr.json
--rw-r--r--   0 master    (1000) master    (1000)      818 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/static/extra/i18n/datatable-it.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/images/
--rw-r--r--   0 master    (1000) master    (1000)     1150 2017-04-28 13:40:18.000000 burp-ui-1.1.0/burpui/static/images/favicon.ico
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/vendor/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/vendor/ace-builds/
--rw-r--r--   0 master    (1000) master    (1000)      517 2021-09-17 08:35:27.000000 burp-ui-1.1.0/burpui/static/vendor/ace-builds/bower.json
--rw-r--r--   0 master    (1000) master    (1000)      545 2021-09-17 08:35:27.000000 burp-ui-1.1.0/burpui/static/vendor/ace-builds/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/vendor/ace-builds/src-min-noconflict/
--rw-r--r--   0 master    (1000) master    (1000)   358296 2021-09-17 08:35:27.000000 burp-ui-1.1.0/burpui/static/vendor/ace-builds/src-min-noconflict/ace.js
--rw-r--r--   0 master    (1000) master    (1000)     5505 2021-09-17 08:35:27.000000 burp-ui-1.1.0/burpui/static/vendor/ace-builds/src-min-noconflict/mode-json.js
--rw-r--r--   0 master    (1000) master    (1000)    27789 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/ace-builds/src-min-noconflict/theme-ambiance.js
--rw-r--r--   0 master    (1000) master    (1000)    32966 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/ace-builds/src-min-noconflict/worker-json.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/vendor/angular/
--rw-r--r--   0 master    (1000) master    (1000)   169920 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular/angular.min.js
--rw-r--r--   0 master    (1000) master    (1000)      133 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular/bower.json
--rw-r--r--   0 master    (1000) master    (1000)      572 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/vendor/angular-animate/
--rw-r--r--   0 master    (1000) master    (1000)    25733 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-animate/angular-animate.min.js
--rw-r--r--   0 master    (1000) master    (1000)      172 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-animate/bower.json
--rw-r--r--   0 master    (1000) master    (1000)      702 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-animate/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap/
--rw-r--r--   0 master    (1000) master    (1000)      460 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap/bower.json
--rw-r--r--   0 master    (1000) master    (1000)      569 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap/package.json
--rw-r--r--   0 master    (1000) master    (1000)   125728 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap/ui-bootstrap-tpls.min.js
--rw-r--r--   0 master    (1000) master    (1000)   103577 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap/ui-bootstrap.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap-switch/
--rw-r--r--   0 master    (1000) master    (1000)      799 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap-switch/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap-switch/dist/
--rw-r--r--   0 master    (1000) master    (1000)     3139 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap-switch/dist/angular-bootstrap-switch.min.js
--rw-r--r--   0 master    (1000) master    (1000)     1228 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap-switch/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/vendor/angular-datatables-0.6.2/
--rw-r--r--   0 master    (1000) master    (1000)     1720 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-datatables-0.6.2/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/vendor/angular-datatables-0.6.2/dist/
--rw-r--r--   0 master    (1000) master    (1000)    14421 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-datatables-0.6.2/dist/angular-datatables.min.js
--rw-r--r--   0 master    (1000) master    (1000)     1846 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-datatables-0.6.2/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/vendor/angular-highlightjs/
--rw-r--r--   0 master    (1000) master    (1000)      457 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-highlightjs/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-highlightjs/build/
--rw-r--r--   0 master    (1000) master    (1000)     4707 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-highlightjs/build/angular-highlightjs.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-onbeforeunload/
--rw-r--r--   0 master    (1000) master    (1000)      678 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-onbeforeunload/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-onbeforeunload/build/
--rw-r--r--   0 master    (1000) master    (1000)      906 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-onbeforeunload/build/angular-onbeforeunload.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-resource/
--rw-r--r--   0 master    (1000) master    (1000)     4508 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-resource/angular-resource.min.js
--rw-r--r--   0 master    (1000) master    (1000)      174 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-resource/bower.json
--rw-r--r--   0 master    (1000) master    (1000)      738 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-resource/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-route/
--rw-r--r--   0 master    (1000) master    (1000)     5611 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-route/angular-route.min.js
--rw-r--r--   0 master    (1000) master    (1000)      168 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-route/bower.json
--rw-r--r--   0 master    (1000) master    (1000)      687 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-route/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-sanitize/
--rw-r--r--   0 master    (1000) master    (1000)     6612 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-sanitize/angular-sanitize.min.js
--rw-r--r--   0 master    (1000) master    (1000)      174 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-sanitize/bower.json
--rw-r--r--   0 master    (1000) master    (1000)      704 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-sanitize/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-strap/
--rw-r--r--   0 master    (1000) master    (1000)     1268 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-strap/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-strap/dist/
--rw-r--r--   0 master    (1000) master    (1000)    83061 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-strap/dist/angular-strap.min.js
--rw-r--r--   0 master    (1000) master    (1000)     9858 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-strap/dist/angular-strap.tpl.min.js
--rw-r--r--   0 master    (1000) master    (1000)     1756 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-strap/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-ui-calendar/
--rw-r--r--   0 master    (1000) master    (1000)      739 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-ui-calendar/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-ui-calendar/src/
--rw-r--r--   0 master    (1000) master    (1000)    16233 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-ui-calendar/src/calendar.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-ui-select/
--rw-r--r--   0 master    (1000) master    (1000)      574 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-ui-select/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-ui-select/dist/
--rw-r--r--   0 master    (1000) master    (1000)     6092 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-ui-select/dist/select.min.css
--rw-r--r--   0 master    (1000) master    (1000)    45235 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-ui-select/dist/select.min.js
--rw-r--r--   0 master    (1000) master    (1000)     1738 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-ui-select/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-ui-select3/
--rw-r--r--   0 master    (1000) master    (1000)      374 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-ui-select3/bower.json
--rw-r--r--   0 master    (1000) master    (1000)      640 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-ui-select3/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/bootstrap/
--rw-r--r--   0 master    (1000) master    (1000)      641 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootstrap/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.088661 burp-ui-1.1.0/burpui/static/vendor/bootstrap/dist/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/bootstrap/dist/js/
--rw-r--r--   0 master    (1000) master    (1000)    37045 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootstrap/dist/js/bootstrap.min.js
--rw-r--r--   0 master    (1000) master    (1000)     2200 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootstrap/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/bootstrap-switch/
--rw-r--r--   0 master    (1000) master    (1000)      452 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootstrap-switch/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.088661 burp-ui-1.1.0/burpui/static/vendor/bootstrap-switch/dist/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.088661 burp-ui-1.1.0/burpui/static/vendor/bootstrap-switch/dist/css/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/bootstrap-switch/dist/css/bootstrap3/
--rw-r--r--   0 master    (1000) master    (1000)     5612 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootstrap-switch/dist/css/bootstrap3/bootstrap-switch.min.css
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/bootstrap-switch/dist/js/
--rw-r--r--   0 master    (1000) master    (1000)    14920 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootstrap-switch/dist/js/bootstrap-switch.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/bootswatch/
--rw-r--r--   0 master    (1000) master    (1000)      830 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootswatch/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.124662 burp-ui-1.1.0/burpui/static/vendor/bootswatch/fonts/
--rw-r--r--   0 master    (1000) master    (1000)    20127 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 master    (1000) master    (1000)   108738 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 master    (1000) master    (1000)    45404 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 master    (1000) master    (1000)    23424 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 master    (1000) master    (1000)    18028 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.124662 burp-ui-1.1.0/burpui/static/vendor/bootswatch/slate/
--rw-r--r--   0 master    (1000) master    (1000)   142322 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootswatch/slate/bootstrap.min.css
--rw-r--r--   0 master    (1000) master    (1000)     1686 2021-09-17 08:36:04.000000 burp-ui-1.1.0/burpui/static/vendor/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.124662 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/
--rw-r--r--   0 master    (1000) master    (1000)      399 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.124662 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/css/
--rw-r--r--   0 master    (1000) master    (1000)    31000 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/css/font-awesome.min.css
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.124662 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/
--rw-r--r--   0 master    (1000) master    (1000)   134808 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/FontAwesome.otf
--rw-r--r--   0 master    (1000) master    (1000)   165742 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0 master    (1000) master    (1000)   444379 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0 master    (1000) master    (1000)   165548 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 master    (1000) master    (1000)    98024 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0 master    (1000) master    (1000)    77160 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 master    (1000) master    (1000)      332 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.124662 burp-ui-1.1.0/burpui/static/vendor/d3/
--rw-r--r--   0 master    (1000) master    (1000)      156 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/d3/bower.json
--rw-r--r--   0 master    (1000) master    (1000)   151725 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/d3/d3.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.124662 burp-ui-1.1.0/burpui/static/vendor/datatables.net/
--rw-r--r--   0 master    (1000) master    (1000)      692 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net/js/
--rw-r--r--   0 master    (1000) master    (1000)    81906 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net/js/jquery.dataTables.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-bs/
--rw-r--r--   0 master    (1000) master    (1000)      829 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-bs/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-bs/css/
--rw-r--r--   0 master    (1000) master    (1000)     4188 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-bs/css/dataTables.bootstrap.min.css
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-bs/js/
--rw-r--r--   0 master    (1000) master    (1000)     1966 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-bs/js/dataTables.bootstrap.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons/
--rw-r--r--   0 master    (1000) master    (1000)      943 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons/js/
--rw-r--r--   0 master    (1000) master    (1000)    17553 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons/js/dataTables.buttons.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons-bs/
--rw-r--r--   0 master    (1000) master    (1000)      960 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons-bs/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons-bs/css/
--rw-r--r--   0 master    (1000) master    (1000)     2867 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons-bs/css/buttons.bootstrap.min.css
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons-bs/js/
--rw-r--r--   0 master    (1000) master    (1000)      975 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons-bs/js/buttons.bootstrap.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-fixedheader/
--rw-r--r--   0 master    (1000) master    (1000)      761 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-fixedheader/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-fixedheader/js/
--rw-r--r--   0 master    (1000) master    (1000)     6730 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-fixedheader/js/dataTables.fixedHeader.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-fixedheader-bs/
--rw-r--r--   0 master    (1000) master    (1000)      872 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-fixedheader-bs/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-fixedheader-bs/css/
--rw-r--r--   0 master    (1000) master    (1000)      328 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-fixedheader-bs/css/fixedHeader.bootstrap.min.css
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive/
--rw-r--r--   0 master    (1000) master    (1000)      737 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive/js/
--rw-r--r--   0 master    (1000) master    (1000)    12400 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive/js/dataTables.responsive.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive-bs/
--rw-r--r--   0 master    (1000) master    (1000)      885 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive-bs/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive-bs/css/
--rw-r--r--   0 master    (1000) master    (1000)     3992 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive-bs/css/responsive.bootstrap.min.css
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive-bs/js/
--rw-r--r--   0 master    (1000) master    (1000)     1246 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive-bs/js/responsive.bootstrap.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-select/
--rw-r--r--   0 master    (1000) master    (1000)      742 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-select/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-select/js/
--rw-r--r--   0 master    (1000) master    (1000)    11472 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-select/js/dataTables.select.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-select-bs/
--rw-r--r--   0 master    (1000) master    (1000)      848 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-select-bs/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-select-bs/css/
--rw-r--r--   0 master    (1000) master    (1000)     4154 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-select-bs/css/select.bootstrap.min.css
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/fullcalendar/
--rw-r--r--   0 master    (1000) master    (1000)      853 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/fullcalendar/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/
--rw-r--r--   0 master    (1000) master    (1000)    16066 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/fullcalendar.min.css
--rw-r--r--   0 master    (1000) master    (1000)   213774 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/fullcalendar.min.js
--rw-r--r--   0 master    (1000) master    (1000)     1997 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/fullcalendar.print.min.css
--rw-r--r--   0 master    (1000) master    (1000)     4626 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/gcal.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/locale/
--rw-r--r--   0 master    (1000) master    (1000)     3816 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/locale/es.js
--rw-r--r--   0 master    (1000) master    (1000)     3073 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/locale/fr.js
--rw-r--r--   0 master    (1000) master    (1000)     2987 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/locale/it.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/jquery/
--rw-r--r--   0 master    (1000) master    (1000)      190 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/jquery/dist/
--rw-r--r--   0 master    (1000) master    (1000)    86927 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery/dist/jquery.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/jquery-file-download/
--rw-r--r--   0 master    (1000) master    (1000)      694 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery-file-download/bower.json
--rw-r--r--   0 master    (1000) master    (1000)      264 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery-file-download/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.092661 burp-ui-1.1.0/burpui/static/vendor/jquery-file-download/src/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/jquery-file-download/src/Scripts/
--rw-r--r--   0 master    (1000) master    (1000)    19606 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery-file-download/src/Scripts/jquery.fileDownload.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/jquery-ui/
--rw-r--r--   0 master    (1000) master    (1000)      171 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery-ui/bower.json
--rw-r--r--   0 master    (1000) master    (1000)   253669 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery-ui/jquery-ui.min.js
--rw-r--r--   0 master    (1000) master    (1000)      564 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery-ui/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/jquery.fancytree/
--rw-r--r--   0 master    (1000) master    (1000)     1009 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery.fancytree/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/jquery.fancytree/dist/
--rw-r--r--   0 master    (1000) master    (1000)   114799 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery.fancytree/dist/jquery.fancytree-all.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/jquery.fancytree/dist/skin-bootstrap/
--rw-r--r--   0 master    (1000) master    (1000)    13769 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery.fancytree/dist/skin-bootstrap/ui.fancytree.min.css
--rw-r--r--   0 master    (1000) master    (1000)     1881 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery.fancytree/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/jquery.floatThead/
--rw-r--r--   0 master    (1000) master    (1000)      698 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery.floatThead/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/jquery.floatThead/dist/
--rw-r--r--   0 master    (1000) master    (1000)    13515 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery.floatThead/dist/jquery.floatThead.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/js-cookie/
--rw-r--r--   0 master    (1000) master    (1000)      270 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/js-cookie/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/js-cookie/src/
--rw-r--r--   0 master    (1000) master    (1000)     3886 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/js-cookie/src/js.cookie.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/lodash/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/lodash/dist/
--rw-r--r--   0 master    (1000) master    (1000)    73121 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/lodash/dist/lodash.min.js
--rw-r--r--   0 master    (1000) master    (1000)     2044 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/lodash/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/moment/
--rw-r--r--   0 master    (1000) master    (1000)      442 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/moment/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/moment/locale/
--rw-r--r--   0 master    (1000) master    (1000)     3449 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/moment/locale/es.js
--rw-r--r--   0 master    (1000) master    (1000)     2703 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/moment/locale/fr.js
--rw-r--r--   0 master    (1000) master    (1000)     2157 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/moment/locale/it.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/moment/min/
--rw-r--r--   0 master    (1000) master    (1000)    51654 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/moment/min/moment.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/moment-timezone/
--rw-r--r--   0 master    (1000) master    (1000)      395 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/moment-timezone/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/moment-timezone/builds/
--rw-r--r--   0 master    (1000) master    (1000)    42530 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/moment-timezone/builds/moment-timezone-with-data-10-year-range.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.136662 burp-ui-1.1.0/burpui/static/vendor/nvd3/
--rw-r--r--   0 master    (1000) master    (1000)      643 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/nvd3/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.136662 burp-ui-1.1.0/burpui/static/vendor/nvd3/build/
--rw-r--r--   0 master    (1000) master    (1000)     8419 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/nvd3/build/nv.d3.min.css
--rw-r--r--   0 master    (1000) master    (1000)   253352 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/nvd3/build/nv.d3.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.136662 burp-ui-1.1.0/burpui/static/vendor/select2/
--rw-r--r--   0 master    (1000) master    (1000)      206 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/select2/bower.json
--rw-r--r--   0 master    (1000) master    (1000)      678 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/select2/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.136662 burp-ui-1.1.0/burpui/static/vendor/socket.io-client/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.136662 burp-ui-1.1.0/burpui/static/vendor/socket.io-client/dist/
--rw-r--r--   0 master    (1000) master    (1000)    61701 2021-09-17 08:36:04.000000 burp-ui-1.1.0/burpui/static/vendor/socket.io-client/dist/socket.io.min.js
--rw-r--r--   0 master    (1000) master    (1000)     3098 2021-09-17 08:36:04.000000 burp-ui-1.1.0/burpui/static/vendor/socket.io-client/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.136662 burp-ui-1.1.0/burpui/static/vendor/typeahead.js/
--rw-r--r--   0 master    (1000) master    (1000)      247 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/typeahead.js/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.136662 burp-ui-1.1.0/burpui/static/vendor/typeahead.js/dist/
--rw-r--r--   0 master    (1000) master    (1000)    26900 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/typeahead.js/dist/typeahead.jquery.min.js
--rw-r--r--   0 master    (1000) master    (1000)     1801 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/typeahead.js/package.json
--rw-r--r--   0 master    (1000) master    (1000)    12285 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/tasks.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.140662 burp-ui-1.1.0/burpui/templates/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.140662 burp-ui-1.1.0/burpui/templates/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4794 2019-10-02 15:12:13.000000 burp-ui-1.1.0/burpui/templates/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)        6 2019-10-02 15:12:13.000000 burp-ui-1.1.0/burpui/templates/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2019-10-02 15:12:13.000000 burp-ui-1.1.0/burpui/templates/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)        6 2019-10-02 15:12:13.000000 burp-ui-1.1.0/burpui/templates/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)     1162 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/about.html
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.140662 burp-ui-1.1.0/burpui/templates/admin/
--rw-r--r--   0 master    (1000) master    (1000)     1780 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/admin/authentication.html
--rw-r--r--   0 master    (1000) master    (1000)     3045 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/admin/grant-authorization.html
--rw-r--r--   0 master    (1000) master    (1000)     3989 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/admin/group-authorization.html
--rw-r--r--   0 master    (1000) master    (1000)     2722 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/admin/sessions.html
--rw-r--r--   0 master    (1000) master    (1000)     7776 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/admin-authentications.html
--rw-r--r--   0 master    (1000) master    (1000)    13642 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/admin-authorizations.html
--rw-r--r--   0 master    (1000) master    (1000)     1846 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/admin-backends.html
--rw-r--r--   0 master    (1000) master    (1000)     4195 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/backup-report.html
--rw-r--r--   0 master    (1000) master    (1000)     1158 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/calendar.html
--rw-r--r--   0 master    (1000) master    (1000)    11932 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/client-browse.html
--rw-r--r--   0 master    (1000) master    (1000)     3121 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/client-report.html
--rw-r--r--   0 master    (1000) master    (1000)     4686 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/client.html
--rw-r--r--   0 master    (1000) master    (1000)     3588 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/clients-report.html
--rw-r--r--   0 master    (1000) master    (1000)     1402 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/clients.html
--rw-r--r--   0 master    (1000) master    (1000)    14377 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/gerard.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.140662 burp-ui-1.1.0/burpui/templates/js/
--rw-r--r--   0 master    (1000) master    (1000)      743 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/about.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.140662 burp-ui-1.1.0/burpui/templates/js/admin/
--rw-r--r--   0 master    (1000) master    (1000)     1116 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/admin/authentication.js
--rw-r--r--   0 master    (1000) master    (1000)     3860 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/admin/grant-authorization.js
--rw-r--r--   0 master    (1000) master    (1000)     7738 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/admin/group-authorization.js
--rw-r--r--   0 master    (1000) master    (1000)     8347 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/js/admin/sessions.js
--rw-r--r--   0 master    (1000) master    (1000)     9009 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/admin-authentications.js
--rw-r--r--   0 master    (1000) master    (1000)    30828 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/admin-authorizations.js
--rw-r--r--   0 master    (1000) master    (1000)     3896 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/admin-backends.js
--rw-r--r--   0 master    (1000) master    (1000)     2926 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/backup-report.js
--rw-r--r--   0 master    (1000) master    (1000)     1680 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/js/calendar.js
--rw-r--r--   0 master    (1000) master    (1000)    13073 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/js/client-browse.js
--rw-r--r--   0 master    (1000) master    (1000)     5127 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/js/client-report.js
--rw-r--r--   0 master    (1000) master    (1000)    10240 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/js/client.js
--rw-r--r--   0 master    (1000) master    (1000)     2643 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/js/clients-report.js
--rw-r--r--   0 master    (1000) master    (1000)     7921 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/js/clients.js
--rw-r--r--   0 master    (1000) master    (1000)     2470 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/live-monitor.js
--rw-r--r--   0 master    (1000) master    (1000)     2084 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/servers-report.js
--rw-r--r--   0 master    (1000) master    (1000)     1782 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/servers.js
--rw-r--r--   0 master    (1000) master    (1000)    27017 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/js/settings.js
--rw-r--r--   0 master    (1000) master    (1000)    20380 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/js/user.js
--rw-r--r--   0 master    (1000) master    (1000)      347 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/websocket.js
--rw-r--r--   0 master    (1000) master    (1000)     9972 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/layout.html
--rw-r--r--   0 master    (1000) master    (1000)     4937 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/live-monitor.html
--rw-r--r--   0 master    (1000) master    (1000)      735 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/login.html
--rw-r--r--   0 master    (1000) master    (1000)    16144 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/macros.html
--rw-r--r--   0 master    (1000) master    (1000)     1346 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/notifications.html
--rw-r--r--   0 master    (1000) master    (1000)     1776 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/servers-report.html
--rw-r--r--   0 master    (1000) master    (1000)      923 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/servers.html
--rw-r--r--   0 master    (1000) master    (1000)    40891 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/settings.html
--rw-r--r--   0 master    (1000) master    (1000)      861 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/sideadmin.html
--rw-r--r--   0 master    (1000) master    (1000)     2870 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/sidebar.html
--rw-r--r--   0 master    (1000) master    (1000)     1490 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/sideconfig.html
--rw-r--r--   0 master    (1000) master    (1000)      830 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/sideuser.html
--rw-r--r--   0 master    (1000) master    (1000)     3767 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/small_topbar.html
--rw-r--r--   0 master    (1000) master    (1000)     4572 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/topbar.html
--rw-r--r--   0 master    (1000) master    (1000)    10122 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/user.html
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/burpui/thirdparty/
--rw-r--r--   0 master    (1000) master    (1000)    24832 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/thirdparty/flask_bower.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/burpui/tools/
--rw-r--r--   0 master    (1000) master    (1000)     3289 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/tools/logging.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.096661 burp-ui-1.1.0/burpui/translations/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.096661 burp-ui-1.1.0/burpui/translations/es/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/burpui/translations/es/LC_MESSAGES/
--rw-r--r--   0 master    (1000) master    (1000)    60903 2023-05-01 19:13:29.000000 burp-ui-1.1.0/burpui/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 master    (1000) master    (1000)   102166 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.096661 burp-ui-1.1.0/burpui/translations/fr/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/burpui/translations/fr/LC_MESSAGES/
--rw-r--r--   0 master    (1000) master    (1000)    24327 2023-05-01 19:13:29.000000 burp-ui-1.1.0/burpui/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 master    (1000) master    (1000)    80323 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.096661 burp-ui-1.1.0/burpui/translations/it/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/burpui/translations/it/LC_MESSAGES/
--rw-r--r--   0 master    (1000) master    (1000)    56806 2023-05-01 19:13:29.000000 burp-ui-1.1.0/burpui/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 master    (1000) master    (1000)    97706 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/translations/it/LC_MESSAGES/messages.po
--rw-r--r--   0 master    (1000) master    (1000)     8182 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/utils.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/burpui/ws/
--rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/ws/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)      927 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/ws/namespace.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.096661 burp-ui-1.1.0/contrib/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/contrib/centos/
--rwxr-xr-x   0 master    (1000) master    (1000)     1595 2017-04-28 13:40:18.000000 burp-ui-1.1.0/contrib/centos/init.sh
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/contrib/freebsd/
--rw-r--r--   0 master    (1000) master    (1000)      602 2018-05-14 12:28:49.000000 burp-ui-1.1.0/contrib/freebsd/gunicorn.rc
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/contrib/gunicorn/
--rw-r--r--   0 master    (1000) master    (1000)     6080 2022-11-06 21:20:42.000000 burp-ui-1.1.0/contrib/gunicorn/burpui_gunicorn.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/contrib/systemd/
--rw-r--r--   0 master    (1000) master    (1000)      171 2017-05-09 16:54:39.000000 burp-ui-1.1.0/contrib/systemd/bui-agent.service
--rw-r--r--   0 master    (1000) master    (1000)      337 2022-11-06 21:20:42.000000 burp-ui-1.1.0/contrib/systemd/bui-celery-beat.service
--rw-r--r--   0 master    (1000) master    (1000)      191 2022-11-06 21:20:42.000000 burp-ui-1.1.0/contrib/systemd/bui-celery.service
--rw-r--r--   0 master    (1000) master    (1000)      299 2017-05-09 16:54:39.000000 burp-ui-1.1.0/contrib/systemd/bui-gunicorn.service
--rw-r--r--   0 master    (1000) master    (1000)      253 2022-11-06 21:20:42.000000 burp-ui-1.1.0/contrib/systemd/bui-monitor.service
--rw-r--r--   0 master    (1000) master    (1000)      188 2018-05-14 12:28:49.000000 burp-ui-1.1.0/contrib/systemd/bui-websocket.service
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/migrations/
--rwxr-xr-x   0 master    (1000) master    (1000)       39 2022-11-06 21:20:42.000000 burp-ui-1.1.0/migrations/README
--rw-r--r--   0 master    (1000) master    (1000)      770 2017-04-28 13:40:18.000000 burp-ui-1.1.0/migrations/alembic.ini
--rwxr-xr-x   0 master    (1000) master    (1000)     2919 2023-05-01 18:42:40.000000 burp-ui-1.1.0/migrations/env.py
--rwxr-xr-x   0 master    (1000) master    (1000)      412 2017-04-28 13:40:18.000000 burp-ui-1.1.0/migrations/script.py.mako
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/migrations/versions/
--rw-r--r--   0 master    (1000) master    (1000)      980 2023-05-01 18:42:40.000000 burp-ui-1.1.0/migrations/versions/225d9b2f0fb1_initial.py
--rw-r--r--   0 master    (1000) master    (1000)      875 2023-05-01 18:42:40.000000 burp-ui-1.1.0/migrations/versions/4445080944ee_hidden_hosts_management.py
--rw-r--r--   0 master    (1000) master    (1000)      844 2023-05-01 18:42:40.000000 burp-ui-1.1.0/migrations/versions/56de018f4d88_user_prefs.py
--rw-r--r--   0 master    (1000) master    (1000)      983 2023-05-01 18:42:40.000000 burp-ui-1.1.0/migrations/versions/695dcbd29d4f_increase_pref_value_size.py
--rw-r--r--   0 master    (1000) master    (1000)     1190 2023-05-01 18:42:40.000000 burp-ui-1.1.0/migrations/versions/7f317474332d_handle_sessions.py
--rw-r--r--   0 master    (1000) master    (1000)     3244 2023-05-01 18:42:40.000000 burp-ui-1.1.0/migrations/versions/fc07e3fa0086_sql_compatibility.py
--rw-r--r--   0 master    (1000) master    (1000)      224 2022-11-06 21:20:42.000000 burp-ui-1.1.0/pyproject.toml
--rw-r--r--   0 master    (1000) master    (1000)      290 2023-05-01 18:42:40.000000 burp-ui-1.1.0/requirements.txt
--rw-r--r--   0 master    (1000) master    (1000)      503 2023-05-01 19:13:30.148662 burp-ui-1.1.0/setup.cfg
--rwxr-xr-x   0 master    (1000) master    (1000)    14194 2023-05-01 18:42:40.000000 burp-ui-1.1.0/setup.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.096661 burp-ui-1.1.0/share/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.096661 burp-ui-1.1.0/share/burpui/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/share/burpui/etc/
--rw-r--r--   0 master    (1000) master    (1000)      772 2022-11-06 21:20:42.000000 burp-ui-1.1.0/share/burpui/etc/buimonitor.sample.cfg
--rw-r--r--   0 master    (1000) master    (1000)    15828 2022-11-06 21:20:42.000000 burp-ui-1.1.0/share/burpui/etc/burpui.sample.cfg
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.851496 burp-ui-1.1.1/
+-rw-r--r--   0 master    (1000) master    (1000)    22942 2023-07-07 18:23:10.000000 burp-ui-1.1.1/CHANGELOG.rst
+-rw-r--r--   0 master    (1000) master    (1000)      368 2022-11-06 21:20:42.000000 burp-ui-1.1.1/CONTRIBUTORS
+-rw-r--r--   0 master    (1000) master    (1000)     1575 2018-05-14 12:28:48.000000 burp-ui-1.1.1/LICENSE
+-rw-r--r--   0 master    (1000) master    (1000)      342 2022-11-06 21:20:42.000000 burp-ui-1.1.1/MANIFEST.in
+-rw-r--r--   0 master    (1000) master    (1000)     5873 2023-07-07 18:24:28.851496 burp-ui-1.1.1/PKG-INFO
+-rw-r--r--   0 master    (1000) master    (1000)     5025 2022-11-06 21:20:42.000000 burp-ui-1.1.1/README.rst
+-rw-r--r--   0 master    (1000) master    (1000)      229 2017-04-28 13:40:18.000000 burp-ui-1.1.1/babel.cfg
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.111459 burp-ui-1.1.1/burp_ui.egg-info/
+-rw-r--r--   0 master    (1000) master    (1000)     5873 2023-07-07 18:24:26.000000 burp-ui-1.1.1/burp_ui.egg-info/PKG-INFO
+-rw-r--r--   0 master    (1000) master    (1000)    15086 2023-07-07 18:24:26.000000 burp-ui-1.1.1/burp_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 master    (1000) master    (1000)        1 2023-07-07 18:24:26.000000 burp-ui-1.1.1/burp_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 master    (1000) master    (1000)      243 2023-07-07 18:24:26.000000 burp-ui-1.1.1/burp_ui.egg-info/entry_points.txt
+-rw-r--r--   0 master    (1000) master    (1000)      755 2023-07-07 18:24:26.000000 burp-ui-1.1.1/burp_ui.egg-info/requires.txt
+-rw-r--r--   0 master    (1000) master    (1000)        7 2023-07-07 18:24:26.000000 burp-ui-1.1.1/burp_ui.egg-info/top_level.txt
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.135459 burp-ui-1.1.1/burpui/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.151460 burp-ui-1.1.1/burpui/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4829 2018-07-24 09:36:18.000000 burp-ui-1.1.1/burpui/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)    12191 2019-10-03 09:41:02.000000 burp-ui-1.1.1/burpui/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2018-06-05 15:54:46.000000 burp-ui-1.1.1/burpui/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)      779 2019-10-03 09:41:02.000000 burp-ui-1.1.1/burpui/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)        0 2023-07-07 18:24:25.000000 burp-ui-1.1.1/burpui/RELEASE
+-rw-r--r--   0 master    (1000) master    (1000)        6 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/VERSION
+-rw-r--r--   0 master    (1000) master    (1000)      382 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)     9535 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/__main__.py
+-rw-r--r--   0 master    (1000) master    (1000)      249 2021-05-12 15:45:53.000000 burp-ui-1.1.1/burpui/_cli.py
+-rw-r--r--   0 master    (1000) master    (1000)     2058 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/_compat.py
+-rw-r--r--   0 master    (1000) master    (1000)     1202 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/_json.py
+-rw-r--r--   0 master    (1000) master    (1000)      397 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/_rtfd.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.155460 burp-ui-1.1.1/burpui/api/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.159460 burp-ui-1.1.1/burpui/api/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4794 2018-07-24 09:36:18.000000 burp-ui-1.1.1/burpui/api/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)     2643 2018-09-14 14:17:22.000000 burp-ui-1.1.1/burpui/api/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2018-07-23 14:42:15.000000 burp-ui-1.1.1/burpui/api/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)        6 2018-09-14 14:17:22.000000 burp-ui-1.1.1/burpui/api/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)     8428 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/api/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)    60894 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/api/admin.py
+-rw-r--r--   0 master    (1000) master    (1000)     4961 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/api/backup.py
+-rw-r--r--   0 master    (1000) master    (1000)    36404 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/api/client.py
+-rw-r--r--   0 master    (1000) master    (1000)    25725 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/api/clients.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.159460 burp-ui-1.1.1/burpui/api/custom/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.171460 burp-ui-1.1.1/burpui/api/custom/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4794 2019-10-01 14:25:10.000000 burp-ui-1.1.1/burpui/api/custom/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)      291 2019-10-01 14:25:10.000000 burp-ui-1.1.1/burpui/api/custom/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2019-10-01 14:25:10.000000 burp-ui-1.1.1/burpui/api/custom/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)        6 2019-10-01 14:25:10.000000 burp-ui-1.1.1/burpui/api/custom/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)      213 2018-07-24 09:36:18.000000 burp-ui-1.1.1/burpui/api/custom/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)      585 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/api/custom/fields.py
+-rw-r--r--   0 master    (1000) master    (1000)     2860 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/api/custom/my_fields.py
+-rw-r--r--   0 master    (1000) master    (1000)     1430 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/api/custom/resource.py
+-rw-r--r--   0 master    (1000) master    (1000)    35378 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/api/misc.py
+-rw-r--r--   0 master    (1000) master    (1000)     8585 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/api/prefs.py
+-rw-r--r--   0 master    (1000) master    (1000)    17608 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/api/restore.py
+-rw-r--r--   0 master    (1000) master    (1000)     8028 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/api/servers.py
+-rw-r--r--   0 master    (1000) master    (1000)    35800 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/api/settings.py
+-rw-r--r--   0 master    (1000) master    (1000)    32795 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/api/tasks.py
+-rw-r--r--   0 master    (1000) master    (1000)    15706 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/app.py
+-rw-r--r--   0 master    (1000) master    (1000)    16384 2017-07-26 14:40:04.000000 burp-ui-1.1.1/burpui/celerybeat-schedule
+-rw-r--r--   0 master    (1000) master    (1000)    45118 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/cli.py
+-rw-r--r--   0 master    (1000) master    (1000)    10045 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/config.py
+-rw-r--r--   0 master    (1000) master    (1000)    23767 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/datastructures.py
+-rw-r--r--   0 master    (1000) master    (1000)     2768 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/decorators.py
+-rw-r--r--   0 master    (1000) master    (1000)      964 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/desc.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.171460 burp-ui-1.1.1/burpui/engines/
+-rw-r--r--   0 master    (1000) master    (1000)        0 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/engines/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)    14171 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/engines/agent.py
+-rw-r--r--   0 master    (1000) master    (1000)    11302 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/engines/monitor.py
+-rw-r--r--   0 master    (1000) master    (1000)    17914 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/engines/server.py
+-rw-r--r--   0 master    (1000) master    (1000)      943 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/engines/worker.py
+-rw-r--r--   0 master    (1000) master    (1000)      871 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/exceptions.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.195460 burp-ui-1.1.1/burpui/ext/
+-rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.1.1/burpui/ext/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)      371 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/ext/cache.py
+-rw-r--r--   0 master    (1000) master    (1000)      926 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/ext/i18n.py
+-rw-r--r--   0 master    (1000) master    (1000)      309 2018-07-24 09:36:18.000000 burp-ui-1.1.1/burpui/ext/limit.py
+-rw-r--r--   0 master    (1000) master    (1000)      233 2018-07-24 09:36:18.000000 burp-ui-1.1.1/burpui/ext/session.py
+-rw-r--r--   0 master    (1000) master    (1000)      232 2018-07-24 09:36:18.000000 burp-ui-1.1.1/burpui/ext/sql.py
+-rw-r--r--   0 master    (1000) master    (1000)      230 2019-04-02 19:43:50.000000 burp-ui-1.1.1/burpui/ext/tasks.py
+-rw-r--r--   0 master    (1000) master    (1000)      545 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/ext/ws.py
+-rw-r--r--   0 master    (1000) master    (1000)    11954 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/extensions.py
+-rw-r--r--   0 master    (1000) master    (1000)     3524 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/filter.py
+-rw-r--r--   0 master    (1000) master    (1000)      728 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/forms.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.195460 burp-ui-1.1.1/burpui/misc/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.195460 burp-ui-1.1.1/burpui/misc/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4794 2018-07-24 09:36:18.000000 burp-ui-1.1.1/burpui/misc/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)     2452 2018-07-23 07:59:35.000000 burp-ui-1.1.1/burpui/misc/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2018-07-20 15:54:46.000000 burp-ui-1.1.1/burpui/misc/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)        6 2018-07-23 07:59:35.000000 burp-ui-1.1.1/burpui/misc/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.1.1/burpui/misc/__init__.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.199461 burp-ui-1.1.1/burpui/misc/acl/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.215461 burp-ui-1.1.1/burpui/misc/acl/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4794 2019-09-24 13:37:49.000000 burp-ui-1.1.1/burpui/misc/acl/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)      346 2019-09-27 12:40:13.000000 burp-ui-1.1.1/burpui/misc/acl/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2019-09-25 20:15:11.000000 burp-ui-1.1.1/burpui/misc/acl/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)        6 2019-09-27 12:40:13.000000 burp-ui-1.1.1/burpui/misc/acl/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.1.1/burpui/misc/acl/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)    14445 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/misc/acl/basic.py
+-rw-r--r--   0 master    (1000) master    (1000)     5655 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/misc/acl/handler.py
+-rw-r--r--   0 master    (1000) master    (1000)     5389 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/misc/acl/interface.py
+-rw-r--r--   0 master    (1000) master    (1000)    28562 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/misc/acl/meta.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.215461 burp-ui-1.1.1/burpui/misc/audit/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.323463 burp-ui-1.1.1/burpui/misc/audit/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4829 2018-07-24 09:36:18.000000 burp-ui-1.1.1/burpui/misc/audit/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)      138 2018-08-03 09:24:44.000000 burp-ui-1.1.1/burpui/misc/audit/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2018-06-05 13:59:15.000000 burp-ui-1.1.1/burpui/misc/audit/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)       27 2018-08-03 09:24:44.000000 burp-ui-1.1.1/burpui/misc/audit/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)        0 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/misc/audit/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)     2804 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/misc/audit/basic.py
+-rw-r--r--   0 master    (1000) master    (1000)     3591 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/misc/audit/handler.py
+-rw-r--r--   0 master    (1000) master    (1000)     1854 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/misc/audit/interface.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.343464 burp-ui-1.1.1/burpui/misc/auth/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.379464 burp-ui-1.1.1/burpui/misc/auth/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4829 2018-07-24 09:36:18.000000 burp-ui-1.1.1/burpui/misc/auth/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)      763 2019-01-29 14:01:08.000000 burp-ui-1.1.1/burpui/misc/auth/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2018-06-07 15:21:13.000000 burp-ui-1.1.1/burpui/misc/auth/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)     2077 2019-01-29 14:01:08.000000 burp-ui-1.1.1/burpui/misc/auth/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.1.1/burpui/misc/auth/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)     9656 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/misc/auth/basic.py
+-rw-r--r--   0 master    (1000) master    (1000)    10821 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/misc/auth/handler.py
+-rw-r--r--   0 master    (1000) master    (1000)     3489 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/misc/auth/interface.py
+-rw-r--r--   0 master    (1000) master    (1000)    11181 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/misc/auth/ldap.py
+-rw-r--r--   0 master    (1000) master    (1000)     4675 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/misc/auth/local.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.383465 burp-ui-1.1.1/burpui/misc/backend/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.407465 burp-ui-1.1.1/burpui/misc/backend/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4829 2018-07-24 09:36:18.000000 burp-ui-1.1.1/burpui/misc/backend/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)     1168 2020-05-08 22:06:12.000000 burp-ui-1.1.1/burpui/misc/backend/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2018-07-18 09:19:37.000000 burp-ui-1.1.1/burpui/misc/backend/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)        6 2020-05-08 22:06:12.000000 burp-ui-1.1.1/burpui/misc/backend/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.1.1/burpui/misc/backend/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)    47346 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/misc/backend/burp1.py
+-rw-r--r--   0 master    (1000) master    (1000)    30620 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/misc/backend/burp2.py
+-rw-r--r--   0 master    (1000) master    (1000)    41267 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/misc/backend/interface.py
+-rw-r--r--   0 master    (1000) master    (1000)    23472 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/misc/backend/multi.py
+-rw-r--r--   0 master    (1000) master    (1000)    38354 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/misc/backend/parallel.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.407465 burp-ui-1.1.1/burpui/misc/backend/utils/
+-rw-r--r--   0 master    (1000) master    (1000)        0 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/misc/backend/utils/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)    12735 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/misc/backend/utils/burp2.py
+-rw-r--r--   0 master    (1000) master    (1000)      398 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/misc/backend/utils/constant.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.431465 burp-ui-1.1.1/burpui/misc/parser/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.443466 burp-ui-1.1.1/burpui/misc/parser/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4794 2019-10-01 12:38:25.000000 burp-ui-1.1.1/burpui/misc/parser/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)      431 2021-10-04 08:39:12.000000 burp-ui-1.1.1/burpui/misc/parser/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2019-10-03 09:34:38.000000 burp-ui-1.1.1/burpui/misc/parser/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)        6 2021-10-04 08:39:12.000000 burp-ui-1.1.1/burpui/misc/parser/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.1.1/burpui/misc/parser/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)    37464 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/misc/parser/burp1.py
+-rw-r--r--   0 master    (1000) master    (1000)    13883 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/misc/parser/burp2.py
+-rw-r--r--   0 master    (1000) master    (1000)    43592 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/misc/parser/doc.py
+-rw-r--r--   0 master    (1000) master    (1000)    17679 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/misc/parser/interface.py
+-rw-r--r--   0 master    (1000) master    (1000)     8075 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/misc/parser/openssl.py
+-rw-r--r--   0 master    (1000) master    (1000)    57165 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/misc/parser/utils.py
+-rw-r--r--   0 master    (1000) master    (1000)     3399 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/models.py
+-rw-r--r--   0 master    (1000) master    (1000)     2642 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/plugins.py
+-rw-r--r--   0 master    (1000) master    (1000)    17427 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/routes.py
+-rw-r--r--   0 master    (1000) master    (1000)     2913 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/security.py
+-rw-r--r--   0 master    (1000) master    (1000)    11088 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/sessions.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.451466 burp-ui-1.1.1/burpui/static/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.059458 burp-ui-1.1.1/burpui/static/3rdparty/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.479467 burp-ui-1.1.1/burpui/static/3rdparty/highlightjs/
+-rw-r--r--   0 master    (1000) master    (1000)     8711 2018-05-14 12:28:49.000000 burp-ui-1.1.1/burpui/static/3rdparty/highlightjs/highlight.pack.js
+-rw-r--r--   0 master    (1000) master    (1000)     1211 2018-05-14 12:28:49.000000 burp-ui-1.1.1/burpui/static/3rdparty/highlightjs/style.css
+-rw-r--r--   0 master    (1000) master    (1000)     7298 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/static/dashboard.css
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.059458 burp-ui-1.1.1/burpui/static/extra/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.499467 burp-ui-1.1.1/burpui/static/extra/i18n/
+-rw-r--r--   0 master    (1000) master    (1000)      885 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/static/extra/i18n/datatable-es.json
+-rw-r--r--   0 master    (1000) master    (1000)      990 2017-04-28 13:40:18.000000 burp-ui-1.1.1/burpui/static/extra/i18n/datatable-fr.json
+-rw-r--r--   0 master    (1000) master    (1000)      818 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/static/extra/i18n/datatable-it.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.503467 burp-ui-1.1.1/burpui/static/images/
+-rw-r--r--   0 master    (1000) master    (1000)     1150 2017-04-28 13:40:18.000000 burp-ui-1.1.1/burpui/static/images/favicon.ico
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.507467 burp-ui-1.1.1/burpui/static/vendor/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.531468 burp-ui-1.1.1/burpui/static/vendor/ace-builds/
+-rw-r--r--   0 master    (1000) master    (1000)      517 2021-09-17 08:35:27.000000 burp-ui-1.1.1/burpui/static/vendor/ace-builds/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)      545 2021-09-17 08:35:27.000000 burp-ui-1.1.1/burpui/static/vendor/ace-builds/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.575469 burp-ui-1.1.1/burpui/static/vendor/ace-builds/src-min-noconflict/
+-rw-r--r--   0 master    (1000) master    (1000)   358296 2021-09-17 08:35:27.000000 burp-ui-1.1.1/burpui/static/vendor/ace-builds/src-min-noconflict/ace.js
+-rw-r--r--   0 master    (1000) master    (1000)     5505 2021-09-17 08:35:27.000000 burp-ui-1.1.1/burpui/static/vendor/ace-builds/src-min-noconflict/mode-json.js
+-rw-r--r--   0 master    (1000) master    (1000)    27789 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/ace-builds/src-min-noconflict/theme-ambiance.js
+-rw-r--r--   0 master    (1000) master    (1000)    32966 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/ace-builds/src-min-noconflict/worker-json.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.603469 burp-ui-1.1.1/burpui/static/vendor/angular/
+-rw-r--r--   0 master    (1000) master    (1000)   169920 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular/angular.min.js
+-rw-r--r--   0 master    (1000) master    (1000)      133 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)      572 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.667471 burp-ui-1.1.1/burpui/static/vendor/angular-animate/
+-rw-r--r--   0 master    (1000) master    (1000)    25733 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-animate/angular-animate.min.js
+-rw-r--r--   0 master    (1000) master    (1000)      172 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-animate/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)      702 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-animate/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.703472 burp-ui-1.1.1/burpui/static/vendor/angular-bootstrap/
+-rw-r--r--   0 master    (1000) master    (1000)      460 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-bootstrap/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)      569 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-bootstrap/package.json
+-rw-r--r--   0 master    (1000) master    (1000)   125728 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-bootstrap/ui-bootstrap-tpls.min.js
+-rw-r--r--   0 master    (1000) master    (1000)   103577 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-bootstrap/ui-bootstrap.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.707471 burp-ui-1.1.1/burpui/static/vendor/angular-bootstrap-switch/
+-rw-r--r--   0 master    (1000) master    (1000)      799 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-bootstrap-switch/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.743472 burp-ui-1.1.1/burpui/static/vendor/angular-bootstrap-switch/dist/
+-rw-r--r--   0 master    (1000) master    (1000)     3139 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-bootstrap-switch/dist/angular-bootstrap-switch.min.js
+-rw-r--r--   0 master    (1000) master    (1000)     1228 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-bootstrap-switch/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.799473 burp-ui-1.1.1/burpui/static/vendor/angular-datatables-0.6.2/
+-rw-r--r--   0 master    (1000) master    (1000)     1720 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-datatables-0.6.2/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.799473 burp-ui-1.1.1/burpui/static/vendor/angular-datatables-0.6.2/dist/
+-rw-r--r--   0 master    (1000) master    (1000)    14421 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-datatables-0.6.2/dist/angular-datatables.min.js
+-rw-r--r--   0 master    (1000) master    (1000)     1846 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-datatables-0.6.2/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.799473 burp-ui-1.1.1/burpui/static/vendor/angular-highlightjs/
+-rw-r--r--   0 master    (1000) master    (1000)      457 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-highlightjs/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.819474 burp-ui-1.1.1/burpui/static/vendor/angular-highlightjs/build/
+-rw-r--r--   0 master    (1000) master    (1000)     4707 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-highlightjs/build/angular-highlightjs.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.819474 burp-ui-1.1.1/burpui/static/vendor/angular-onbeforeunload/
+-rw-r--r--   0 master    (1000) master    (1000)      678 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-onbeforeunload/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.819474 burp-ui-1.1.1/burpui/static/vendor/angular-onbeforeunload/build/
+-rw-r--r--   0 master    (1000) master    (1000)      906 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-onbeforeunload/build/angular-onbeforeunload.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.823474 burp-ui-1.1.1/burpui/static/vendor/angular-resource/
+-rw-r--r--   0 master    (1000) master    (1000)     4508 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-resource/angular-resource.min.js
+-rw-r--r--   0 master    (1000) master    (1000)      174 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-resource/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)      738 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-resource/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.835474 burp-ui-1.1.1/burpui/static/vendor/angular-route/
+-rw-r--r--   0 master    (1000) master    (1000)     5611 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-route/angular-route.min.js
+-rw-r--r--   0 master    (1000) master    (1000)      168 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-route/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)      687 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-route/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.843474 burp-ui-1.1.1/burpui/static/vendor/angular-sanitize/
+-rw-r--r--   0 master    (1000) master    (1000)     6612 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-sanitize/angular-sanitize.min.js
+-rw-r--r--   0 master    (1000) master    (1000)      174 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-sanitize/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)      704 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-sanitize/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.843474 burp-ui-1.1.1/burpui/static/vendor/angular-strap/
+-rw-r--r--   0 master    (1000) master    (1000)     1268 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-strap/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.855475 burp-ui-1.1.1/burpui/static/vendor/angular-strap/dist/
+-rw-r--r--   0 master    (1000) master    (1000)    83061 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-strap/dist/angular-strap.min.js
+-rw-r--r--   0 master    (1000) master    (1000)     9858 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-strap/dist/angular-strap.tpl.min.js
+-rw-r--r--   0 master    (1000) master    (1000)     1756 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-strap/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.855475 burp-ui-1.1.1/burpui/static/vendor/angular-ui-calendar/
+-rw-r--r--   0 master    (1000) master    (1000)      739 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-ui-calendar/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.863475 burp-ui-1.1.1/burpui/static/vendor/angular-ui-calendar/src/
+-rw-r--r--   0 master    (1000) master    (1000)    16233 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-ui-calendar/src/calendar.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.867475 burp-ui-1.1.1/burpui/static/vendor/angular-ui-select/
+-rw-r--r--   0 master    (1000) master    (1000)      574 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-ui-select/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.879475 burp-ui-1.1.1/burpui/static/vendor/angular-ui-select/dist/
+-rw-r--r--   0 master    (1000) master    (1000)     6092 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-ui-select/dist/select.min.css
+-rw-r--r--   0 master    (1000) master    (1000)    45235 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-ui-select/dist/select.min.js
+-rw-r--r--   0 master    (1000) master    (1000)     1738 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-ui-select/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.887475 burp-ui-1.1.1/burpui/static/vendor/angular-ui-select3/
+-rw-r--r--   0 master    (1000) master    (1000)      374 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-ui-select3/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)      640 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/angular-ui-select3/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.887475 burp-ui-1.1.1/burpui/static/vendor/bootstrap/
+-rw-r--r--   0 master    (1000) master    (1000)      641 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/bootstrap/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.063458 burp-ui-1.1.1/burpui/static/vendor/bootstrap/dist/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.903476 burp-ui-1.1.1/burpui/static/vendor/bootstrap/dist/js/
+-rw-r--r--   0 master    (1000) master    (1000)    37045 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/bootstrap/dist/js/bootstrap.min.js
+-rw-r--r--   0 master    (1000) master    (1000)     2200 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/bootstrap/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.887475 burp-ui-1.1.1/burpui/static/vendor/bootstrap-switch/
+-rw-r--r--   0 master    (1000) master    (1000)      452 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/bootstrap-switch/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.063458 burp-ui-1.1.1/burpui/static/vendor/bootstrap-switch/dist/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.063458 burp-ui-1.1.1/burpui/static/vendor/bootstrap-switch/dist/css/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.887475 burp-ui-1.1.1/burpui/static/vendor/bootstrap-switch/dist/css/bootstrap3/
+-rw-r--r--   0 master    (1000) master    (1000)     5612 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/bootstrap-switch/dist/css/bootstrap3/bootstrap-switch.min.css
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.891476 burp-ui-1.1.1/burpui/static/vendor/bootstrap-switch/dist/js/
+-rw-r--r--   0 master    (1000) master    (1000)    14920 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/bootstrap-switch/dist/js/bootstrap-switch.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.911476 burp-ui-1.1.1/burpui/static/vendor/bootswatch/
+-rw-r--r--   0 master    (1000) master    (1000)      830 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/bootswatch/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.015478 burp-ui-1.1.1/burpui/static/vendor/bootswatch/fonts/
+-rw-r--r--   0 master    (1000) master    (1000)    20127 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 master    (1000) master    (1000)   108738 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 master    (1000) master    (1000)    45404 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 master    (1000) master    (1000)    23424 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 master    (1000) master    (1000)    18028 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.039479 burp-ui-1.1.1/burpui/static/vendor/bootswatch/slate/
+-rw-r--r--   0 master    (1000) master    (1000)   142322 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/bootswatch/slate/bootstrap.min.css
+-rw-r--r--   0 master    (1000) master    (1000)     1686 2021-09-17 08:36:04.000000 burp-ui-1.1.1/burpui/static/vendor/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.063479 burp-ui-1.1.1/burpui/static/vendor/components-font-awesome/
+-rw-r--r--   0 master    (1000) master    (1000)      399 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/components-font-awesome/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.063479 burp-ui-1.1.1/burpui/static/vendor/components-font-awesome/css/
+-rw-r--r--   0 master    (1000) master    (1000)    31000 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/components-font-awesome/css/font-awesome.min.css
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.111480 burp-ui-1.1.1/burpui/static/vendor/components-font-awesome/fonts/
+-rw-r--r--   0 master    (1000) master    (1000)   134808 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/components-font-awesome/fonts/FontAwesome.otf
+-rw-r--r--   0 master    (1000) master    (1000)   165742 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 master    (1000) master    (1000)   444379 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 master    (1000) master    (1000)   165548 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 master    (1000) master    (1000)    98024 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 master    (1000) master    (1000)    77160 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 master    (1000) master    (1000)      332 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/components-font-awesome/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.119480 burp-ui-1.1.1/burpui/static/vendor/d3/
+-rw-r--r--   0 master    (1000) master    (1000)      156 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/d3/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)   151725 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/d3/d3.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.131481 burp-ui-1.1.1/burpui/static/vendor/datatables.net/
+-rw-r--r--   0 master    (1000) master    (1000)      692 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.175482 burp-ui-1.1.1/burpui/static/vendor/datatables.net/js/
+-rw-r--r--   0 master    (1000) master    (1000)    81906 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net/js/jquery.dataTables.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.131481 burp-ui-1.1.1/burpui/static/vendor/datatables.net-bs/
+-rw-r--r--   0 master    (1000) master    (1000)      829 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net-bs/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.131481 burp-ui-1.1.1/burpui/static/vendor/datatables.net-bs/css/
+-rw-r--r--   0 master    (1000) master    (1000)     4188 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net-bs/css/dataTables.bootstrap.min.css
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.135481 burp-ui-1.1.1/burpui/static/vendor/datatables.net-bs/js/
+-rw-r--r--   0 master    (1000) master    (1000)     1966 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net-bs/js/dataTables.bootstrap.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.135481 burp-ui-1.1.1/burpui/static/vendor/datatables.net-buttons/
+-rw-r--r--   0 master    (1000) master    (1000)      943 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net-buttons/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.139481 burp-ui-1.1.1/burpui/static/vendor/datatables.net-buttons/js/
+-rw-r--r--   0 master    (1000) master    (1000)    17553 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net-buttons/js/dataTables.buttons.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.135481 burp-ui-1.1.1/burpui/static/vendor/datatables.net-buttons-bs/
+-rw-r--r--   0 master    (1000) master    (1000)      960 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net-buttons-bs/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.135481 burp-ui-1.1.1/burpui/static/vendor/datatables.net-buttons-bs/css/
+-rw-r--r--   0 master    (1000) master    (1000)     2867 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net-buttons-bs/css/buttons.bootstrap.min.css
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.139481 burp-ui-1.1.1/burpui/static/vendor/datatables.net-buttons-bs/js/
+-rw-r--r--   0 master    (1000) master    (1000)      975 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net-buttons-bs/js/buttons.bootstrap.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.139481 burp-ui-1.1.1/burpui/static/vendor/datatables.net-fixedheader/
+-rw-r--r--   0 master    (1000) master    (1000)      761 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net-fixedheader/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.151481 burp-ui-1.1.1/burpui/static/vendor/datatables.net-fixedheader/js/
+-rw-r--r--   0 master    (1000) master    (1000)     6730 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net-fixedheader/js/dataTables.fixedHeader.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.147481 burp-ui-1.1.1/burpui/static/vendor/datatables.net-fixedheader-bs/
+-rw-r--r--   0 master    (1000) master    (1000)      872 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net-fixedheader-bs/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.147481 burp-ui-1.1.1/burpui/static/vendor/datatables.net-fixedheader-bs/css/
+-rw-r--r--   0 master    (1000) master    (1000)      328 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net-fixedheader-bs/css/fixedHeader.bootstrap.min.css
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.151481 burp-ui-1.1.1/burpui/static/vendor/datatables.net-responsive/
+-rw-r--r--   0 master    (1000) master    (1000)      737 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net-responsive/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.155481 burp-ui-1.1.1/burpui/static/vendor/datatables.net-responsive/js/
+-rw-r--r--   0 master    (1000) master    (1000)    12400 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net-responsive/js/dataTables.responsive.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.151481 burp-ui-1.1.1/burpui/static/vendor/datatables.net-responsive-bs/
+-rw-r--r--   0 master    (1000) master    (1000)      885 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net-responsive-bs/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.155481 burp-ui-1.1.1/burpui/static/vendor/datatables.net-responsive-bs/css/
+-rw-r--r--   0 master    (1000) master    (1000)     3992 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net-responsive-bs/css/responsive.bootstrap.min.css
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.155481 burp-ui-1.1.1/burpui/static/vendor/datatables.net-responsive-bs/js/
+-rw-r--r--   0 master    (1000) master    (1000)     1246 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net-responsive-bs/js/responsive.bootstrap.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.171481 burp-ui-1.1.1/burpui/static/vendor/datatables.net-select/
+-rw-r--r--   0 master    (1000) master    (1000)      742 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net-select/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.171481 burp-ui-1.1.1/burpui/static/vendor/datatables.net-select/js/
+-rw-r--r--   0 master    (1000) master    (1000)    11472 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net-select/js/dataTables.select.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.171481 burp-ui-1.1.1/burpui/static/vendor/datatables.net-select-bs/
+-rw-r--r--   0 master    (1000) master    (1000)      848 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net-select-bs/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.171481 burp-ui-1.1.1/burpui/static/vendor/datatables.net-select-bs/css/
+-rw-r--r--   0 master    (1000) master    (1000)     4154 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/datatables.net-select-bs/css/select.bootstrap.min.css
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.183482 burp-ui-1.1.1/burpui/static/vendor/fullcalendar/
+-rw-r--r--   0 master    (1000) master    (1000)      853 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/fullcalendar/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.187482 burp-ui-1.1.1/burpui/static/vendor/fullcalendar/dist/
+-rw-r--r--   0 master    (1000) master    (1000)    16066 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/fullcalendar/dist/fullcalendar.min.css
+-rw-r--r--   0 master    (1000) master    (1000)   213774 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/fullcalendar/dist/fullcalendar.min.js
+-rw-r--r--   0 master    (1000) master    (1000)     1997 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/fullcalendar/dist/fullcalendar.print.min.css
+-rw-r--r--   0 master    (1000) master    (1000)     4626 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/fullcalendar/dist/gcal.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.219483 burp-ui-1.1.1/burpui/static/vendor/fullcalendar/dist/locale/
+-rw-r--r--   0 master    (1000) master    (1000)     3816 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/fullcalendar/dist/locale/es.js
+-rw-r--r--   0 master    (1000) master    (1000)     3073 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/fullcalendar/dist/locale/fr.js
+-rw-r--r--   0 master    (1000) master    (1000)     2987 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/fullcalendar/dist/locale/it.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.219483 burp-ui-1.1.1/burpui/static/vendor/jquery/
+-rw-r--r--   0 master    (1000) master    (1000)      190 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/jquery/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.415487 burp-ui-1.1.1/burpui/static/vendor/jquery/dist/
+-rw-r--r--   0 master    (1000) master    (1000)    86927 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/jquery/dist/jquery.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.235483 burp-ui-1.1.1/burpui/static/vendor/jquery-file-download/
+-rw-r--r--   0 master    (1000) master    (1000)      694 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/jquery-file-download/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)      264 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/jquery-file-download/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.067458 burp-ui-1.1.1/burpui/static/vendor/jquery-file-download/src/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.235483 burp-ui-1.1.1/burpui/static/vendor/jquery-file-download/src/Scripts/
+-rw-r--r--   0 master    (1000) master    (1000)    19606 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/jquery-file-download/src/Scripts/jquery.fileDownload.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.351485 burp-ui-1.1.1/burpui/static/vendor/jquery-ui/
+-rw-r--r--   0 master    (1000) master    (1000)      171 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/jquery-ui/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)   253669 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/jquery-ui/jquery-ui.min.js
+-rw-r--r--   0 master    (1000) master    (1000)      564 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/jquery-ui/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.371486 burp-ui-1.1.1/burpui/static/vendor/jquery.fancytree/
+-rw-r--r--   0 master    (1000) master    (1000)     1009 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/jquery.fancytree/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.383486 burp-ui-1.1.1/burpui/static/vendor/jquery.fancytree/dist/
+-rw-r--r--   0 master    (1000) master    (1000)   114799 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/jquery.fancytree/dist/jquery.fancytree-all.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.395486 burp-ui-1.1.1/burpui/static/vendor/jquery.fancytree/dist/skin-bootstrap/
+-rw-r--r--   0 master    (1000) master    (1000)    13769 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/jquery.fancytree/dist/skin-bootstrap/ui.fancytree.min.css
+-rw-r--r--   0 master    (1000) master    (1000)     1881 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/jquery.fancytree/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.399486 burp-ui-1.1.1/burpui/static/vendor/jquery.floatThead/
+-rw-r--r--   0 master    (1000) master    (1000)      698 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/jquery.floatThead/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.407487 burp-ui-1.1.1/burpui/static/vendor/jquery.floatThead/dist/
+-rw-r--r--   0 master    (1000) master    (1000)    13515 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/jquery.floatThead/dist/jquery.floatThead.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.435487 burp-ui-1.1.1/burpui/static/vendor/js-cookie/
+-rw-r--r--   0 master    (1000) master    (1000)      270 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/js-cookie/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.443487 burp-ui-1.1.1/burpui/static/vendor/js-cookie/src/
+-rw-r--r--   0 master    (1000) master    (1000)     3886 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/js-cookie/src/js.cookie.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.447487 burp-ui-1.1.1/burpui/static/vendor/lodash/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.459488 burp-ui-1.1.1/burpui/static/vendor/lodash/dist/
+-rw-r--r--   0 master    (1000) master    (1000)    73121 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/lodash/dist/lodash.min.js
+-rw-r--r--   0 master    (1000) master    (1000)     2044 2021-09-17 08:35:28.000000 burp-ui-1.1.1/burpui/static/vendor/lodash/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.463488 burp-ui-1.1.1/burpui/static/vendor/moment/
+-rw-r--r--   0 master    (1000) master    (1000)      442 2021-09-17 08:35:29.000000 burp-ui-1.1.1/burpui/static/vendor/moment/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.499488 burp-ui-1.1.1/burpui/static/vendor/moment/locale/
+-rw-r--r--   0 master    (1000) master    (1000)     3449 2021-09-17 08:35:29.000000 burp-ui-1.1.1/burpui/static/vendor/moment/locale/es.js
+-rw-r--r--   0 master    (1000) master    (1000)     2703 2021-09-17 08:35:29.000000 burp-ui-1.1.1/burpui/static/vendor/moment/locale/fr.js
+-rw-r--r--   0 master    (1000) master    (1000)     2157 2021-09-17 08:35:29.000000 burp-ui-1.1.1/burpui/static/vendor/moment/locale/it.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.507489 burp-ui-1.1.1/burpui/static/vendor/moment/min/
+-rw-r--r--   0 master    (1000) master    (1000)    51654 2021-09-17 08:35:29.000000 burp-ui-1.1.1/burpui/static/vendor/moment/min/moment.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.467488 burp-ui-1.1.1/burpui/static/vendor/moment-timezone/
+-rw-r--r--   0 master    (1000) master    (1000)      395 2021-09-17 08:35:29.000000 burp-ui-1.1.1/burpui/static/vendor/moment-timezone/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.467488 burp-ui-1.1.1/burpui/static/vendor/moment-timezone/builds/
+-rw-r--r--   0 master    (1000) master    (1000)    42530 2021-09-17 08:35:29.000000 burp-ui-1.1.1/burpui/static/vendor/moment-timezone/builds/moment-timezone-with-data-10-year-range.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.519489 burp-ui-1.1.1/burpui/static/vendor/nvd3/
+-rw-r--r--   0 master    (1000) master    (1000)      643 2021-09-17 08:35:29.000000 burp-ui-1.1.1/burpui/static/vendor/nvd3/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.539489 burp-ui-1.1.1/burpui/static/vendor/nvd3/build/
+-rw-r--r--   0 master    (1000) master    (1000)     8419 2021-09-17 08:35:29.000000 burp-ui-1.1.1/burpui/static/vendor/nvd3/build/nv.d3.min.css
+-rw-r--r--   0 master    (1000) master    (1000)   253352 2021-09-17 08:35:29.000000 burp-ui-1.1.1/burpui/static/vendor/nvd3/build/nv.d3.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.559490 burp-ui-1.1.1/burpui/static/vendor/select2/
+-rw-r--r--   0 master    (1000) master    (1000)      206 2021-09-17 08:35:29.000000 burp-ui-1.1.1/burpui/static/vendor/select2/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)      678 2021-09-17 08:35:29.000000 burp-ui-1.1.1/burpui/static/vendor/select2/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.567490 burp-ui-1.1.1/burpui/static/vendor/socket.io-client/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.575490 burp-ui-1.1.1/burpui/static/vendor/socket.io-client/dist/
+-rw-r--r--   0 master    (1000) master    (1000)    61701 2021-09-17 08:36:04.000000 burp-ui-1.1.1/burpui/static/vendor/socket.io-client/dist/socket.io.min.js
+-rw-r--r--   0 master    (1000) master    (1000)     3098 2021-09-17 08:36:04.000000 burp-ui-1.1.1/burpui/static/vendor/socket.io-client/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.595491 burp-ui-1.1.1/burpui/static/vendor/typeahead.js/
+-rw-r--r--   0 master    (1000) master    (1000)      247 2021-09-17 08:35:29.000000 burp-ui-1.1.1/burpui/static/vendor/typeahead.js/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.599491 burp-ui-1.1.1/burpui/static/vendor/typeahead.js/dist/
+-rw-r--r--   0 master    (1000) master    (1000)    26900 2021-09-17 08:35:29.000000 burp-ui-1.1.1/burpui/static/vendor/typeahead.js/dist/typeahead.jquery.min.js
+-rw-r--r--   0 master    (1000) master    (1000)     1801 2021-09-17 08:35:29.000000 burp-ui-1.1.1/burpui/static/vendor/typeahead.js/package.json
+-rw-r--r--   0 master    (1000) master    (1000)    12285 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/tasks.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.735494 burp-ui-1.1.1/burpui/templates/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.759494 burp-ui-1.1.1/burpui/templates/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4794 2019-10-02 15:12:13.000000 burp-ui-1.1.1/burpui/templates/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)        6 2019-10-02 15:12:13.000000 burp-ui-1.1.1/burpui/templates/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2019-10-02 15:12:13.000000 burp-ui-1.1.1/burpui/templates/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)        6 2019-10-02 15:12:13.000000 burp-ui-1.1.1/burpui/templates/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)     1162 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/about.html
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.767494 burp-ui-1.1.1/burpui/templates/admin/
+-rw-r--r--   0 master    (1000) master    (1000)     1780 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/admin/authentication.html
+-rw-r--r--   0 master    (1000) master    (1000)     3045 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/admin/grant-authorization.html
+-rw-r--r--   0 master    (1000) master    (1000)     3989 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/admin/group-authorization.html
+-rw-r--r--   0 master    (1000) master    (1000)     2722 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/admin/sessions.html
+-rw-r--r--   0 master    (1000) master    (1000)     7776 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/admin-authentications.html
+-rw-r--r--   0 master    (1000) master    (1000)    13642 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/admin-authorizations.html
+-rw-r--r--   0 master    (1000) master    (1000)     1846 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/admin-backends.html
+-rw-r--r--   0 master    (1000) master    (1000)     4195 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/backup-report.html
+-rw-r--r--   0 master    (1000) master    (1000)     1158 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/calendar.html
+-rw-r--r--   0 master    (1000) master    (1000)    11932 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/templates/client-browse.html
+-rw-r--r--   0 master    (1000) master    (1000)     3121 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/client-report.html
+-rw-r--r--   0 master    (1000) master    (1000)     4686 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/templates/client.html
+-rw-r--r--   0 master    (1000) master    (1000)     3588 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/clients-report.html
+-rw-r--r--   0 master    (1000) master    (1000)     1402 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/templates/clients.html
+-rw-r--r--   0 master    (1000) master    (1000)    14377 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/templates/gerard.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.791495 burp-ui-1.1.1/burpui/templates/js/
+-rw-r--r--   0 master    (1000) master    (1000)      743 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/js/about.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.799495 burp-ui-1.1.1/burpui/templates/js/admin/
+-rw-r--r--   0 master    (1000) master    (1000)     1116 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/js/admin/authentication.js
+-rw-r--r--   0 master    (1000) master    (1000)     3860 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/js/admin/grant-authorization.js
+-rw-r--r--   0 master    (1000) master    (1000)     7738 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/js/admin/group-authorization.js
+-rw-r--r--   0 master    (1000) master    (1000)     8347 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/templates/js/admin/sessions.js
+-rw-r--r--   0 master    (1000) master    (1000)     9009 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/js/admin-authentications.js
+-rw-r--r--   0 master    (1000) master    (1000)    30828 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/js/admin-authorizations.js
+-rw-r--r--   0 master    (1000) master    (1000)     3896 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/js/admin-backends.js
+-rw-r--r--   0 master    (1000) master    (1000)     2926 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/js/backup-report.js
+-rw-r--r--   0 master    (1000) master    (1000)     1680 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/templates/js/calendar.js
+-rw-r--r--   0 master    (1000) master    (1000)    13073 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/templates/js/client-browse.js
+-rw-r--r--   0 master    (1000) master    (1000)     5127 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/templates/js/client-report.js
+-rw-r--r--   0 master    (1000) master    (1000)    10240 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/templates/js/client.js
+-rw-r--r--   0 master    (1000) master    (1000)     2643 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/templates/js/clients-report.js
+-rw-r--r--   0 master    (1000) master    (1000)     7921 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/templates/js/clients.js
+-rw-r--r--   0 master    (1000) master    (1000)     2470 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/js/live-monitor.js
+-rw-r--r--   0 master    (1000) master    (1000)     2084 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/js/servers-report.js
+-rw-r--r--   0 master    (1000) master    (1000)     1782 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/js/servers.js
+-rw-r--r--   0 master    (1000) master    (1000)    27017 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/templates/js/settings.js
+-rw-r--r--   0 master    (1000) master    (1000)    20380 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/templates/js/user.js
+-rw-r--r--   0 master    (1000) master    (1000)      347 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/js/websocket.js
+-rw-r--r--   0 master    (1000) master    (1000)     9972 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/templates/layout.html
+-rw-r--r--   0 master    (1000) master    (1000)     4937 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/templates/live-monitor.html
+-rw-r--r--   0 master    (1000) master    (1000)      735 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/login.html
+-rw-r--r--   0 master    (1000) master    (1000)    16144 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/templates/macros.html
+-rw-r--r--   0 master    (1000) master    (1000)     1346 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/notifications.html
+-rw-r--r--   0 master    (1000) master    (1000)     1776 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/servers-report.html
+-rw-r--r--   0 master    (1000) master    (1000)      923 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/templates/servers.html
+-rw-r--r--   0 master    (1000) master    (1000)    40891 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/templates/settings.html
+-rw-r--r--   0 master    (1000) master    (1000)      861 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/sideadmin.html
+-rw-r--r--   0 master    (1000) master    (1000)     2870 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/sidebar.html
+-rw-r--r--   0 master    (1000) master    (1000)     1490 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/templates/sideconfig.html
+-rw-r--r--   0 master    (1000) master    (1000)      830 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/templates/sideuser.html
+-rw-r--r--   0 master    (1000) master    (1000)     3767 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/small_topbar.html
+-rw-r--r--   0 master    (1000) master    (1000)     4572 2018-08-18 00:27:08.000000 burp-ui-1.1.1/burpui/templates/topbar.html
+-rw-r--r--   0 master    (1000) master    (1000)    10122 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/templates/user.html
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.799495 burp-ui-1.1.1/burpui/thirdparty/
+-rw-r--r--   0 master    (1000) master    (1000)    24832 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/thirdparty/flask_bower.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.799495 burp-ui-1.1.1/burpui/tools/
+-rw-r--r--   0 master    (1000) master    (1000)     3289 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/tools/logging.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.075458 burp-ui-1.1.1/burpui/translations/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.071458 burp-ui-1.1.1/burpui/translations/es/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.799495 burp-ui-1.1.1/burpui/translations/es/LC_MESSAGES/
+-rw-r--r--   0 master    (1000) master    (1000)    60903 2023-07-07 18:24:25.000000 burp-ui-1.1.1/burpui/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 master    (1000) master    (1000)   102166 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.075458 burp-ui-1.1.1/burpui/translations/fr/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.803495 burp-ui-1.1.1/burpui/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 master    (1000) master    (1000)    24327 2023-07-07 18:24:25.000000 burp-ui-1.1.1/burpui/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 master    (1000) master    (1000)    80323 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.075458 burp-ui-1.1.1/burpui/translations/it/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.803495 burp-ui-1.1.1/burpui/translations/it/LC_MESSAGES/
+-rw-r--r--   0 master    (1000) master    (1000)    56806 2023-07-07 18:24:25.000000 burp-ui-1.1.1/burpui/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 master    (1000) master    (1000)    97706 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/translations/it/LC_MESSAGES/messages.po
+-rw-r--r--   0 master    (1000) master    (1000)     8182 2023-07-07 18:23:10.000000 burp-ui-1.1.1/burpui/utils.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.803495 burp-ui-1.1.1/burpui/ws/
+-rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.1.1/burpui/ws/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)      927 2022-11-06 21:20:42.000000 burp-ui-1.1.1/burpui/ws/namespace.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.075458 burp-ui-1.1.1/contrib/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.815495 burp-ui-1.1.1/contrib/centos/
+-rwxr-xr-x   0 master    (1000) master    (1000)     1595 2017-04-28 13:40:18.000000 burp-ui-1.1.1/contrib/centos/init.sh
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.827495 burp-ui-1.1.1/contrib/freebsd/
+-rw-r--r--   0 master    (1000) master    (1000)      602 2018-05-14 12:28:49.000000 burp-ui-1.1.1/contrib/freebsd/gunicorn.rc
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.827495 burp-ui-1.1.1/contrib/gunicorn/
+-rw-r--r--   0 master    (1000) master    (1000)     6080 2022-11-06 21:20:42.000000 burp-ui-1.1.1/contrib/gunicorn/burpui_gunicorn.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.835496 burp-ui-1.1.1/contrib/systemd/
+-rw-r--r--   0 master    (1000) master    (1000)      171 2017-05-09 16:54:39.000000 burp-ui-1.1.1/contrib/systemd/bui-agent.service
+-rw-r--r--   0 master    (1000) master    (1000)      337 2022-11-06 21:20:42.000000 burp-ui-1.1.1/contrib/systemd/bui-celery-beat.service
+-rw-r--r--   0 master    (1000) master    (1000)      191 2022-11-06 21:20:42.000000 burp-ui-1.1.1/contrib/systemd/bui-celery.service
+-rw-r--r--   0 master    (1000) master    (1000)      299 2017-05-09 16:54:39.000000 burp-ui-1.1.1/contrib/systemd/bui-gunicorn.service
+-rw-r--r--   0 master    (1000) master    (1000)      253 2022-11-06 21:20:42.000000 burp-ui-1.1.1/contrib/systemd/bui-monitor.service
+-rw-r--r--   0 master    (1000) master    (1000)      188 2018-05-14 12:28:49.000000 burp-ui-1.1.1/contrib/systemd/bui-websocket.service
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.839496 burp-ui-1.1.1/migrations/
+-rwxr-xr-x   0 master    (1000) master    (1000)       39 2022-11-06 21:20:42.000000 burp-ui-1.1.1/migrations/README
+-rw-r--r--   0 master    (1000) master    (1000)      770 2017-04-28 13:40:18.000000 burp-ui-1.1.1/migrations/alembic.ini
+-rwxr-xr-x   0 master    (1000) master    (1000)     2892 2023-07-07 18:23:10.000000 burp-ui-1.1.1/migrations/env.py
+-rwxr-xr-x   0 master    (1000) master    (1000)      412 2017-04-28 13:40:18.000000 burp-ui-1.1.1/migrations/script.py.mako
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.839496 burp-ui-1.1.1/migrations/versions/
+-rw-r--r--   0 master    (1000) master    (1000)      980 2023-07-07 18:23:10.000000 burp-ui-1.1.1/migrations/versions/225d9b2f0fb1_initial.py
+-rw-r--r--   0 master    (1000) master    (1000)      875 2023-07-07 18:23:10.000000 burp-ui-1.1.1/migrations/versions/4445080944ee_hidden_hosts_management.py
+-rw-r--r--   0 master    (1000) master    (1000)      844 2023-07-07 18:23:10.000000 burp-ui-1.1.1/migrations/versions/56de018f4d88_user_prefs.py
+-rw-r--r--   0 master    (1000) master    (1000)      983 2023-07-07 18:23:10.000000 burp-ui-1.1.1/migrations/versions/695dcbd29d4f_increase_pref_value_size.py
+-rw-r--r--   0 master    (1000) master    (1000)     1190 2023-07-07 18:23:10.000000 burp-ui-1.1.1/migrations/versions/7f317474332d_handle_sessions.py
+-rw-r--r--   0 master    (1000) master    (1000)     3244 2023-07-07 18:23:10.000000 burp-ui-1.1.1/migrations/versions/fc07e3fa0086_sql_compatibility.py
+-rw-r--r--   0 master    (1000) master    (1000)      224 2022-11-06 21:20:42.000000 burp-ui-1.1.1/pyproject.toml
+-rw-r--r--   0 master    (1000) master    (1000)      290 2023-07-07 18:23:10.000000 burp-ui-1.1.1/requirements.txt
+-rw-r--r--   0 master    (1000) master    (1000)      503 2023-07-07 18:24:28.855496 burp-ui-1.1.1/setup.cfg
+-rwxr-xr-x   0 master    (1000) master    (1000)    14194 2023-07-07 18:23:10.000000 burp-ui-1.1.1/setup.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.075458 burp-ui-1.1.1/share/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:27.075458 burp-ui-1.1.1/share/burpui/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:24:28.851496 burp-ui-1.1.1/share/burpui/etc/
+-rw-r--r--   0 master    (1000) master    (1000)      772 2022-11-06 21:20:42.000000 burp-ui-1.1.1/share/burpui/etc/buimonitor.sample.cfg
+-rw-r--r--   0 master    (1000) master    (1000)    15828 2022-11-06 21:20:42.000000 burp-ui-1.1.1/share/burpui/etc/burpui.sample.cfg
```

### Comparing `burp-ui-1.1.0/CHANGELOG.rst` & `burp-ui-1.1.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+1.1.1 (07/07/2023)
+------------------
+
+- fix: remove duplicate compare_type from alembic config
+- fix: make sure we don't initialize the DB connector twice
+
 1.1.0 (05/01/2023)
 ------------------
 
 - fix: update dependencies and fix unit tests `#352 <https://git.ziirish.me/ziirish/burp-ui/issues/352>`_
 - fix: platform.dist is no longer part of the std lib
 - fix: adapt send_file usage
```

### Comparing `burp-ui-1.1.0/LICENSE` & `burp-ui-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/PKG-INFO` & `burp-ui-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burp-ui
-Version: 1.1.0
+Version: 1.1.1
 Summary: Burp-UI is a web-ui for burp backup written in python with Flask and jQuery/Bootstrap
 Home-page: https://git.ziirish.me/ziirish/burp-ui
 Author: Benjamin SANS (Ziirish)
 Author-email: hi+burpui@ziirish.me
 License: BSD 3-clause License
 Keywords: burp web ui backup monitoring
 Platform: UNKNOWN
```

### Comparing `burp-ui-1.1.0/README.rst` & `burp-ui-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burp_ui.egg-info/PKG-INFO` & `burp-ui-1.1.1/burp_ui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burp-ui
-Version: 1.1.0
+Version: 1.1.1
 Summary: Burp-UI is a web-ui for burp backup written in python with Flask and jQuery/Bootstrap
 Home-page: https://git.ziirish.me/ziirish/burp-ui
 Author: Benjamin SANS (Ziirish)
 Author-email: hi+burpui@ziirish.me
 License: BSD 3-clause License
 Keywords: burp web ui backup monitoring
 Platform: UNKNOWN
```

### Comparing `burp-ui-1.1.0/burp_ui.egg-info/SOURCES.txt` & `burp-ui-1.1.1/burp_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burp_ui.egg-info/requires.txt` & `burp-ui-1.1.1/burp_ui.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/.ropeproject/config.py` & `burp-ui-1.1.1/burpui/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/.ropeproject/globalnames` & `burp-ui-1.1.1/burpui/.ropeproject/globalnames`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/.ropeproject/objectdb` & `burp-ui-1.1.1/burpui/.ropeproject/objectdb`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/__main__.py` & `burp-ui-1.1.1/burpui/__main__.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/_compat.py` & `burp-ui-1.1.1/burpui/_compat.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/_json.py` & `burp-ui-1.1.1/burpui/_json.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/api/.ropeproject/config.py` & `burp-ui-1.1.1/burpui/api/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/api/.ropeproject/globalnames` & `burp-ui-1.1.1/burpui/api/.ropeproject/globalnames`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/api/__init__.py` & `burp-ui-1.1.1/burpui/api/__init__.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/api/admin.py` & `burp-ui-1.1.1/burpui/api/admin.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/api/backup.py` & `burp-ui-1.1.1/burpui/api/backup.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/api/client.py` & `burp-ui-1.1.1/burpui/api/client.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/api/clients.py` & `burp-ui-1.1.1/burpui/api/clients.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/api/custom/.ropeproject/config.py` & `burp-ui-1.1.1/burpui/api/custom/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/api/custom/fields.py` & `burp-ui-1.1.1/burpui/api/custom/fields.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/api/custom/my_fields.py` & `burp-ui-1.1.1/burpui/api/custom/my_fields.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/api/custom/resource.py` & `burp-ui-1.1.1/burpui/api/custom/resource.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/api/misc.py` & `burp-ui-1.1.1/burpui/api/misc.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/api/prefs.py` & `burp-ui-1.1.1/burpui/api/prefs.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/api/restore.py` & `burp-ui-1.1.1/burpui/api/restore.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/api/servers.py` & `burp-ui-1.1.1/burpui/api/servers.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/api/settings.py` & `burp-ui-1.1.1/burpui/api/settings.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/api/tasks.py` & `burp-ui-1.1.1/burpui/api/tasks.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/app.py` & `burp-ui-1.1.1/burpui/app.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/celerybeat-schedule` & `burp-ui-1.1.1/burpui/celerybeat-schedule`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/cli.py` & `burp-ui-1.1.1/burpui/cli.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/config.py` & `burp-ui-1.1.1/burpui/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/datastructures.py` & `burp-ui-1.1.1/burpui/datastructures.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/decorators.py` & `burp-ui-1.1.1/burpui/decorators.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/desc.py` & `burp-ui-1.1.1/burpui/desc.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/engines/agent.py` & `burp-ui-1.1.1/burpui/engines/agent.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/engines/monitor.py` & `burp-ui-1.1.1/burpui/engines/monitor.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/engines/server.py` & `burp-ui-1.1.1/burpui/engines/server.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/engines/worker.py` & `burp-ui-1.1.1/burpui/engines/worker.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/exceptions.py` & `burp-ui-1.1.1/burpui/exceptions.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/ext/i18n.py` & `burp-ui-1.1.1/burpui/ext/i18n.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/ext/ws.py` & `burp-ui-1.1.1/burpui/ext/ws.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/extensions.py` & `burp-ui-1.1.1/burpui/extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,16 @@
             back = parse_db_setting(myapp.config["SQLALCHEMY_DATABASE_URI"])[0]
 
             if "mysql" in back:  # pragma: no cover
                 # optimize SQL pools for MySQL driver
                 myapp.config["SQLALCHEMY_POOL_SIZE"] = 20
                 myapp.config["SQLALCHEMY_POOL_RECYCLE"] = 600
 
-            db.init_app(myapp)
+            if "sqlalchemy" not in myapp.extensions:
+                db.init_app(myapp)
             if not cli and not unittest and not celery_worker:  # pragma: no cover
                 with myapp.app_context():
                     try:
                         import subprocess
 
                         # get current head using alembic/FLask-Migrate
                         local = os.path.join(os.getcwd(), "tools", "bui-manage")
```

### Comparing `burp-ui-1.1.0/burpui/filter.py` & `burp-ui-1.1.1/burpui/filter.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/forms.py` & `burp-ui-1.1.1/burpui/forms.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/.ropeproject/config.py` & `burp-ui-1.1.1/burpui/misc/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/.ropeproject/globalnames` & `burp-ui-1.1.1/burpui/misc/.ropeproject/globalnames`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/acl/.ropeproject/config.py` & `burp-ui-1.1.1/burpui/misc/acl/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/acl/basic.py` & `burp-ui-1.1.1/burpui/misc/acl/basic.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/acl/handler.py` & `burp-ui-1.1.1/burpui/misc/acl/handler.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/acl/interface.py` & `burp-ui-1.1.1/burpui/misc/acl/interface.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/acl/meta.py` & `burp-ui-1.1.1/burpui/misc/acl/meta.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/audit/.ropeproject/config.py` & `burp-ui-1.1.1/burpui/misc/audit/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/audit/basic.py` & `burp-ui-1.1.1/burpui/misc/audit/basic.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/audit/handler.py` & `burp-ui-1.1.1/burpui/misc/audit/handler.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/audit/interface.py` & `burp-ui-1.1.1/burpui/misc/audit/interface.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/auth/.ropeproject/config.py` & `burp-ui-1.1.1/burpui/misc/auth/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/auth/.ropeproject/globalnames` & `burp-ui-1.1.1/burpui/misc/auth/.ropeproject/globalnames`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/auth/.ropeproject/objectdb` & `burp-ui-1.1.1/burpui/misc/auth/.ropeproject/objectdb`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/auth/basic.py` & `burp-ui-1.1.1/burpui/misc/auth/basic.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/auth/handler.py` & `burp-ui-1.1.1/burpui/misc/auth/handler.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/auth/interface.py` & `burp-ui-1.1.1/burpui/misc/auth/interface.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/auth/ldap.py` & `burp-ui-1.1.1/burpui/misc/auth/ldap.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/auth/local.py` & `burp-ui-1.1.1/burpui/misc/auth/local.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/backend/.ropeproject/config.py` & `burp-ui-1.1.1/burpui/misc/backend/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/backend/.ropeproject/globalnames` & `burp-ui-1.1.1/burpui/misc/backend/.ropeproject/globalnames`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/backend/burp1.py` & `burp-ui-1.1.1/burpui/misc/backend/burp1.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/backend/burp2.py` & `burp-ui-1.1.1/burpui/misc/backend/burp2.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/backend/interface.py` & `burp-ui-1.1.1/burpui/misc/backend/interface.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/backend/multi.py` & `burp-ui-1.1.1/burpui/misc/backend/multi.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/backend/parallel.py` & `burp-ui-1.1.1/burpui/misc/backend/parallel.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/backend/utils/burp2.py` & `burp-ui-1.1.1/burpui/misc/backend/utils/burp2.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/parser/.ropeproject/config.py` & `burp-ui-1.1.1/burpui/misc/parser/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/parser/burp1.py` & `burp-ui-1.1.1/burpui/misc/parser/burp1.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/parser/burp2.py` & `burp-ui-1.1.1/burpui/misc/parser/burp2.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/parser/doc.py` & `burp-ui-1.1.1/burpui/misc/parser/doc.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/parser/interface.py` & `burp-ui-1.1.1/burpui/misc/parser/interface.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/parser/openssl.py` & `burp-ui-1.1.1/burpui/misc/parser/openssl.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/misc/parser/utils.py` & `burp-ui-1.1.1/burpui/misc/parser/utils.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/models.py` & `burp-ui-1.1.1/burpui/models.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/plugins.py` & `burp-ui-1.1.1/burpui/plugins.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/routes.py` & `burp-ui-1.1.1/burpui/routes.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/security.py` & `burp-ui-1.1.1/burpui/security.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/sessions.py` & `burp-ui-1.1.1/burpui/sessions.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/3rdparty/highlightjs/highlight.pack.js` & `burp-ui-1.1.1/burpui/static/3rdparty/highlightjs/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/3rdparty/highlightjs/style.css` & `burp-ui-1.1.1/burpui/static/3rdparty/highlightjs/style.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/dashboard.css` & `burp-ui-1.1.1/burpui/static/dashboard.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/extra/i18n/datatable-es.json` & `burp-ui-1.1.1/burpui/static/extra/i18n/datatable-es.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/extra/i18n/datatable-fr.json` & `burp-ui-1.1.1/burpui/static/extra/i18n/datatable-fr.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/extra/i18n/datatable-it.json` & `burp-ui-1.1.1/burpui/static/extra/i18n/datatable-it.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/images/favicon.ico` & `burp-ui-1.1.1/burpui/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/ace-builds/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/ace-builds/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/ace-builds/package.json` & `burp-ui-1.1.1/burpui/static/vendor/ace-builds/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/ace-builds/src-min-noconflict/ace.js` & `burp-ui-1.1.1/burpui/static/vendor/ace-builds/src-min-noconflict/ace.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/ace-builds/src-min-noconflict/mode-json.js` & `burp-ui-1.1.1/burpui/static/vendor/ace-builds/src-min-noconflict/mode-json.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/ace-builds/src-min-noconflict/theme-ambiance.js` & `burp-ui-1.1.1/burpui/static/vendor/ace-builds/src-min-noconflict/theme-ambiance.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/ace-builds/src-min-noconflict/worker-json.js` & `burp-ui-1.1.1/burpui/static/vendor/ace-builds/src-min-noconflict/worker-json.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular/angular.min.js` & `burp-ui-1.1.1/burpui/static/vendor/angular/angular.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular/package.json` & `burp-ui-1.1.1/burpui/static/vendor/angular/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-animate/angular-animate.min.js` & `burp-ui-1.1.1/burpui/static/vendor/angular-animate/angular-animate.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-animate/package.json` & `burp-ui-1.1.1/burpui/static/vendor/angular-animate/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap/package.json` & `burp-ui-1.1.1/burpui/static/vendor/angular-bootstrap/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap/ui-bootstrap-tpls.min.js` & `burp-ui-1.1.1/burpui/static/vendor/angular-bootstrap/ui-bootstrap-tpls.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap/ui-bootstrap.min.js` & `burp-ui-1.1.1/burpui/static/vendor/angular-bootstrap/ui-bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap-switch/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/angular-bootstrap-switch/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap-switch/dist/angular-bootstrap-switch.min.js` & `burp-ui-1.1.1/burpui/static/vendor/angular-bootstrap-switch/dist/angular-bootstrap-switch.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap-switch/package.json` & `burp-ui-1.1.1/burpui/static/vendor/angular-bootstrap-switch/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-datatables-0.6.2/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/angular-datatables-0.6.2/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-datatables-0.6.2/dist/angular-datatables.min.js` & `burp-ui-1.1.1/burpui/static/vendor/angular-datatables-0.6.2/dist/angular-datatables.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-datatables-0.6.2/package.json` & `burp-ui-1.1.1/burpui/static/vendor/angular-datatables-0.6.2/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-highlightjs/build/angular-highlightjs.min.js` & `burp-ui-1.1.1/burpui/static/vendor/angular-highlightjs/build/angular-highlightjs.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-onbeforeunload/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/angular-onbeforeunload/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-onbeforeunload/build/angular-onbeforeunload.js` & `burp-ui-1.1.1/burpui/static/vendor/angular-onbeforeunload/build/angular-onbeforeunload.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-resource/angular-resource.min.js` & `burp-ui-1.1.1/burpui/static/vendor/angular-resource/angular-resource.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-resource/package.json` & `burp-ui-1.1.1/burpui/static/vendor/angular-resource/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-route/angular-route.min.js` & `burp-ui-1.1.1/burpui/static/vendor/angular-route/angular-route.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-route/package.json` & `burp-ui-1.1.1/burpui/static/vendor/angular-route/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-sanitize/angular-sanitize.min.js` & `burp-ui-1.1.1/burpui/static/vendor/angular-sanitize/angular-sanitize.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-sanitize/package.json` & `burp-ui-1.1.1/burpui/static/vendor/angular-sanitize/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-strap/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/angular-strap/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-strap/dist/angular-strap.min.js` & `burp-ui-1.1.1/burpui/static/vendor/angular-strap/dist/angular-strap.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-strap/dist/angular-strap.tpl.min.js` & `burp-ui-1.1.1/burpui/static/vendor/angular-strap/dist/angular-strap.tpl.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-strap/package.json` & `burp-ui-1.1.1/burpui/static/vendor/angular-strap/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-ui-calendar/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/angular-ui-calendar/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-ui-calendar/src/calendar.js` & `burp-ui-1.1.1/burpui/static/vendor/angular-ui-calendar/src/calendar.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-ui-select/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/angular-ui-select/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-ui-select/dist/select.min.css` & `burp-ui-1.1.1/burpui/static/vendor/angular-ui-select/dist/select.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-ui-select/dist/select.min.js` & `burp-ui-1.1.1/burpui/static/vendor/angular-ui-select/dist/select.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-ui-select/package.json` & `burp-ui-1.1.1/burpui/static/vendor/angular-ui-select/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/angular-ui-select3/package.json` & `burp-ui-1.1.1/burpui/static/vendor/angular-ui-select3/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/bootstrap/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/bootstrap/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/bootstrap/dist/js/bootstrap.min.js` & `burp-ui-1.1.1/burpui/static/vendor/bootstrap/dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/bootstrap/package.json` & `burp-ui-1.1.1/burpui/static/vendor/bootstrap/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/bootstrap-switch/dist/css/bootstrap3/bootstrap-switch.min.css` & `burp-ui-1.1.1/burpui/static/vendor/bootstrap-switch/dist/css/bootstrap3/bootstrap-switch.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/bootstrap-switch/dist/js/bootstrap-switch.min.js` & `burp-ui-1.1.1/burpui/static/vendor/bootstrap-switch/dist/js/bootstrap-switch.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/bootswatch/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/bootswatch/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.eot` & `burp-ui-1.1.1/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.svg` & `burp-ui-1.1.1/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.ttf` & `burp-ui-1.1.1/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.woff` & `burp-ui-1.1.1/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.woff2` & `burp-ui-1.1.1/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/bootswatch/slate/bootstrap.min.css` & `burp-ui-1.1.1/burpui/static/vendor/bootswatch/slate/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/css/font-awesome.min.css` & `burp-ui-1.1.1/burpui/static/vendor/components-font-awesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/FontAwesome.otf` & `burp-ui-1.1.1/burpui/static/vendor/components-font-awesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.eot` & `burp-ui-1.1.1/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.svg` & `burp-ui-1.1.1/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.ttf` & `burp-ui-1.1.1/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.woff` & `burp-ui-1.1.1/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.woff2` & `burp-ui-1.1.1/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/d3/d3.min.js` & `burp-ui-1.1.1/burpui/static/vendor/d3/d3.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/datatables.net/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/datatables.net/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/datatables.net/js/jquery.dataTables.min.js` & `burp-ui-1.1.1/burpui/static/vendor/datatables.net/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/datatables.net-bs/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/datatables.net-bs/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/datatables.net-bs/css/dataTables.bootstrap.min.css` & `burp-ui-1.1.1/burpui/static/vendor/datatables.net-bs/css/dataTables.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/datatables.net-bs/js/dataTables.bootstrap.min.js` & `burp-ui-1.1.1/burpui/static/vendor/datatables.net-bs/js/dataTables.bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/datatables.net-buttons/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons/js/dataTables.buttons.min.js` & `burp-ui-1.1.1/burpui/static/vendor/datatables.net-buttons/js/dataTables.buttons.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons-bs/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/datatables.net-buttons-bs/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons-bs/css/buttons.bootstrap.min.css` & `burp-ui-1.1.1/burpui/static/vendor/datatables.net-buttons-bs/css/buttons.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons-bs/js/buttons.bootstrap.min.js` & `burp-ui-1.1.1/burpui/static/vendor/datatables.net-buttons-bs/js/buttons.bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/datatables.net-fixedheader/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/datatables.net-fixedheader/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/datatables.net-fixedheader/js/dataTables.fixedHeader.min.js` & `burp-ui-1.1.1/burpui/static/vendor/datatables.net-fixedheader/js/dataTables.fixedHeader.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/datatables.net-fixedheader-bs/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/datatables.net-fixedheader-bs/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/datatables.net-responsive/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive/js/dataTables.responsive.min.js` & `burp-ui-1.1.1/burpui/static/vendor/datatables.net-responsive/js/dataTables.responsive.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive-bs/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/datatables.net-responsive-bs/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive-bs/css/responsive.bootstrap.min.css` & `burp-ui-1.1.1/burpui/static/vendor/datatables.net-responsive-bs/css/responsive.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive-bs/js/responsive.bootstrap.min.js` & `burp-ui-1.1.1/burpui/static/vendor/datatables.net-responsive-bs/js/responsive.bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/datatables.net-select/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/datatables.net-select/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/datatables.net-select/js/dataTables.select.min.js` & `burp-ui-1.1.1/burpui/static/vendor/datatables.net-select/js/dataTables.select.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/datatables.net-select-bs/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/datatables.net-select-bs/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/datatables.net-select-bs/css/select.bootstrap.min.css` & `burp-ui-1.1.1/burpui/static/vendor/datatables.net-select-bs/css/select.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/fullcalendar/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/fullcalendar/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/fullcalendar.min.css` & `burp-ui-1.1.1/burpui/static/vendor/fullcalendar/dist/fullcalendar.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/fullcalendar.min.js` & `burp-ui-1.1.1/burpui/static/vendor/fullcalendar/dist/fullcalendar.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/fullcalendar.print.min.css` & `burp-ui-1.1.1/burpui/static/vendor/fullcalendar/dist/fullcalendar.print.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/gcal.min.js` & `burp-ui-1.1.1/burpui/static/vendor/fullcalendar/dist/gcal.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/locale/es.js` & `burp-ui-1.1.1/burpui/static/vendor/fullcalendar/dist/locale/es.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/locale/fr.js` & `burp-ui-1.1.1/burpui/static/vendor/fullcalendar/dist/locale/fr.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/locale/it.js` & `burp-ui-1.1.1/burpui/static/vendor/fullcalendar/dist/locale/it.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/jquery/dist/jquery.min.js` & `burp-ui-1.1.1/burpui/static/vendor/jquery/dist/jquery.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/jquery-file-download/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/jquery-file-download/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/jquery-file-download/src/Scripts/jquery.fileDownload.js` & `burp-ui-1.1.1/burpui/static/vendor/jquery-file-download/src/Scripts/jquery.fileDownload.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/jquery-ui/jquery-ui.min.js` & `burp-ui-1.1.1/burpui/static/vendor/jquery-ui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/jquery-ui/package.json` & `burp-ui-1.1.1/burpui/static/vendor/jquery-ui/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/jquery.fancytree/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/jquery.fancytree/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/jquery.fancytree/dist/jquery.fancytree-all.min.js` & `burp-ui-1.1.1/burpui/static/vendor/jquery.fancytree/dist/jquery.fancytree-all.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/jquery.fancytree/dist/skin-bootstrap/ui.fancytree.min.css` & `burp-ui-1.1.1/burpui/static/vendor/jquery.fancytree/dist/skin-bootstrap/ui.fancytree.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/jquery.fancytree/package.json` & `burp-ui-1.1.1/burpui/static/vendor/jquery.fancytree/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/jquery.floatThead/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/jquery.floatThead/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/jquery.floatThead/dist/jquery.floatThead.min.js` & `burp-ui-1.1.1/burpui/static/vendor/jquery.floatThead/dist/jquery.floatThead.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/js-cookie/src/js.cookie.js` & `burp-ui-1.1.1/burpui/static/vendor/js-cookie/src/js.cookie.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/lodash/dist/lodash.min.js` & `burp-ui-1.1.1/burpui/static/vendor/lodash/dist/lodash.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/lodash/package.json` & `burp-ui-1.1.1/burpui/static/vendor/lodash/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/moment/locale/es.js` & `burp-ui-1.1.1/burpui/static/vendor/moment/locale/es.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/moment/locale/fr.js` & `burp-ui-1.1.1/burpui/static/vendor/moment/locale/fr.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/moment/locale/it.js` & `burp-ui-1.1.1/burpui/static/vendor/moment/locale/it.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/moment/min/moment.min.js` & `burp-ui-1.1.1/burpui/static/vendor/moment/min/moment.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/moment-timezone/builds/moment-timezone-with-data-10-year-range.min.js` & `burp-ui-1.1.1/burpui/static/vendor/moment-timezone/builds/moment-timezone-with-data-10-year-range.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/nvd3/bower.json` & `burp-ui-1.1.1/burpui/static/vendor/nvd3/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/nvd3/build/nv.d3.min.css` & `burp-ui-1.1.1/burpui/static/vendor/nvd3/build/nv.d3.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/nvd3/build/nv.d3.min.js` & `burp-ui-1.1.1/burpui/static/vendor/nvd3/build/nv.d3.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/select2/package.json` & `burp-ui-1.1.1/burpui/static/vendor/select2/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/socket.io-client/dist/socket.io.min.js` & `burp-ui-1.1.1/burpui/static/vendor/socket.io-client/dist/socket.io.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/socket.io-client/package.json` & `burp-ui-1.1.1/burpui/static/vendor/socket.io-client/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/typeahead.js/dist/typeahead.jquery.min.js` & `burp-ui-1.1.1/burpui/static/vendor/typeahead.js/dist/typeahead.jquery.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/static/vendor/typeahead.js/package.json` & `burp-ui-1.1.1/burpui/static/vendor/typeahead.js/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/tasks.py` & `burp-ui-1.1.1/burpui/tasks.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/.ropeproject/config.py` & `burp-ui-1.1.1/burpui/templates/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/about.html` & `burp-ui-1.1.1/burpui/templates/about.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/admin/authentication.html` & `burp-ui-1.1.1/burpui/templates/admin/authentication.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/admin/grant-authorization.html` & `burp-ui-1.1.1/burpui/templates/admin/grant-authorization.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/admin/group-authorization.html` & `burp-ui-1.1.1/burpui/templates/admin/group-authorization.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/admin/sessions.html` & `burp-ui-1.1.1/burpui/templates/admin/sessions.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/admin-authentications.html` & `burp-ui-1.1.1/burpui/templates/admin-authentications.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/admin-authorizations.html` & `burp-ui-1.1.1/burpui/templates/admin-authorizations.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/admin-backends.html` & `burp-ui-1.1.1/burpui/templates/admin-backends.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/backup-report.html` & `burp-ui-1.1.1/burpui/templates/backup-report.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/calendar.html` & `burp-ui-1.1.1/burpui/templates/calendar.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/client-browse.html` & `burp-ui-1.1.1/burpui/templates/client-browse.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/client-report.html` & `burp-ui-1.1.1/burpui/templates/client-report.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/client.html` & `burp-ui-1.1.1/burpui/templates/client.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/clients-report.html` & `burp-ui-1.1.1/burpui/templates/clients-report.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/clients.html` & `burp-ui-1.1.1/burpui/templates/clients.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/gerard.js` & `burp-ui-1.1.1/burpui/templates/gerard.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/js/about.js` & `burp-ui-1.1.1/burpui/templates/js/about.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/js/admin/authentication.js` & `burp-ui-1.1.1/burpui/templates/js/admin/authentication.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/js/admin/grant-authorization.js` & `burp-ui-1.1.1/burpui/templates/js/admin/grant-authorization.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/js/admin/group-authorization.js` & `burp-ui-1.1.1/burpui/templates/js/admin/group-authorization.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/js/admin/sessions.js` & `burp-ui-1.1.1/burpui/templates/js/admin/sessions.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/js/admin-authentications.js` & `burp-ui-1.1.1/burpui/templates/js/admin-authentications.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/js/admin-authorizations.js` & `burp-ui-1.1.1/burpui/templates/js/admin-authorizations.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/js/admin-backends.js` & `burp-ui-1.1.1/burpui/templates/js/admin-backends.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/js/backup-report.js` & `burp-ui-1.1.1/burpui/templates/js/backup-report.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/js/calendar.js` & `burp-ui-1.1.1/burpui/templates/js/calendar.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/js/client-browse.js` & `burp-ui-1.1.1/burpui/templates/js/client-browse.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/js/client-report.js` & `burp-ui-1.1.1/burpui/templates/js/client-report.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/js/client.js` & `burp-ui-1.1.1/burpui/templates/js/client.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/js/clients-report.js` & `burp-ui-1.1.1/burpui/templates/js/clients-report.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/js/clients.js` & `burp-ui-1.1.1/burpui/templates/js/clients.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/js/live-monitor.js` & `burp-ui-1.1.1/burpui/templates/js/live-monitor.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/js/servers-report.js` & `burp-ui-1.1.1/burpui/templates/js/servers-report.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/js/servers.js` & `burp-ui-1.1.1/burpui/templates/js/servers.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/js/settings.js` & `burp-ui-1.1.1/burpui/templates/js/settings.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/js/user.js` & `burp-ui-1.1.1/burpui/templates/js/user.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/layout.html` & `burp-ui-1.1.1/burpui/templates/layout.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/live-monitor.html` & `burp-ui-1.1.1/burpui/templates/live-monitor.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/login.html` & `burp-ui-1.1.1/burpui/templates/login.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/macros.html` & `burp-ui-1.1.1/burpui/templates/macros.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/notifications.html` & `burp-ui-1.1.1/burpui/templates/notifications.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/servers-report.html` & `burp-ui-1.1.1/burpui/templates/servers-report.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/servers.html` & `burp-ui-1.1.1/burpui/templates/servers.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/settings.html` & `burp-ui-1.1.1/burpui/templates/settings.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/sideadmin.html` & `burp-ui-1.1.1/burpui/templates/sideadmin.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/sidebar.html` & `burp-ui-1.1.1/burpui/templates/sidebar.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/sideconfig.html` & `burp-ui-1.1.1/burpui/templates/sideconfig.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/sideuser.html` & `burp-ui-1.1.1/burpui/templates/sideuser.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/small_topbar.html` & `burp-ui-1.1.1/burpui/templates/small_topbar.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/topbar.html` & `burp-ui-1.1.1/burpui/templates/topbar.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/templates/user.html` & `burp-ui-1.1.1/burpui/templates/user.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/thirdparty/flask_bower.py` & `burp-ui-1.1.1/burpui/thirdparty/flask_bower.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/tools/logging.py` & `burp-ui-1.1.1/burpui/tools/logging.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/translations/es/LC_MESSAGES/messages.mo` & `burp-ui-1.1.1/burpui/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/translations/es/LC_MESSAGES/messages.po` & `burp-ui-1.1.1/burpui/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/translations/fr/LC_MESSAGES/messages.mo` & `burp-ui-1.1.1/burpui/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/translations/fr/LC_MESSAGES/messages.po` & `burp-ui-1.1.1/burpui/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/translations/it/LC_MESSAGES/messages.mo` & `burp-ui-1.1.1/burpui/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/translations/it/LC_MESSAGES/messages.po` & `burp-ui-1.1.1/burpui/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/utils.py` & `burp-ui-1.1.1/burpui/utils.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/burpui/ws/namespace.py` & `burp-ui-1.1.1/burpui/ws/namespace.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/contrib/centos/init.sh` & `burp-ui-1.1.1/contrib/centos/init.sh`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/contrib/freebsd/gunicorn.rc` & `burp-ui-1.1.1/contrib/freebsd/gunicorn.rc`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/contrib/gunicorn/burpui_gunicorn.py` & `burp-ui-1.1.1/contrib/gunicorn/burpui_gunicorn.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/migrations/alembic.ini` & `burp-ui-1.1.1/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/migrations/env.py` & `burp-ui-1.1.1/migrations/env.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,15 +76,14 @@
     )
 
     connection = engine.connect()
     context.configure(
         connection=connection,
         target_metadata=target_metadata,
         process_revision_directives=process_revision_directives,
-        compare_type=True,
         **current_app.extensions["migrate"].configure_args
     )
     #                      render_as_batch=True,  ## use this when altering schema
 
     try:
         with context.begin_transaction():
             context.run_migrations()
```

### Comparing `burp-ui-1.1.0/migrations/versions/225d9b2f0fb1_initial.py` & `burp-ui-1.1.1/migrations/versions/225d9b2f0fb1_initial.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/migrations/versions/4445080944ee_hidden_hosts_management.py` & `burp-ui-1.1.1/migrations/versions/4445080944ee_hidden_hosts_management.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/migrations/versions/56de018f4d88_user_prefs.py` & `burp-ui-1.1.1/migrations/versions/56de018f4d88_user_prefs.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/migrations/versions/695dcbd29d4f_increase_pref_value_size.py` & `burp-ui-1.1.1/migrations/versions/695dcbd29d4f_increase_pref_value_size.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/migrations/versions/7f317474332d_handle_sessions.py` & `burp-ui-1.1.1/migrations/versions/7f317474332d_handle_sessions.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/migrations/versions/fc07e3fa0086_sql_compatibility.py` & `burp-ui-1.1.1/migrations/versions/fc07e3fa0086_sql_compatibility.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/setup.py` & `burp-ui-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/share/burpui/etc/buimonitor.sample.cfg` & `burp-ui-1.1.1/share/burpui/etc/buimonitor.sample.cfg`

 * *Files identical despite different names*

### Comparing `burp-ui-1.1.0/share/burpui/etc/burpui.sample.cfg` & `burp-ui-1.1.1/share/burpui/etc/burpui.sample.cfg`

 * *Files identical despite different names*

