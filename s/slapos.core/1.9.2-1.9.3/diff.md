# Comparing `tmp/slapos.core-1.9.2.tar.gz` & `tmp/slapos.core-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slapos.core-1.9.2.tar", last modified: Fri Mar 24 17:13:19 2023, max compression
+gzip compressed data, was "slapos.core-1.9.3.tar", last modified: Wed Apr 26 07:52:45 2023, max compression
```

## Comparing `slapos.core-1.9.2.tar` & `slapos.core-1.9.3.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-03-24 17:13:19.789591 slapos.core-1.9.2/
--rw-r--r--   0 tomo      (1000) tomo      (1000)    44668 2023-03-24 17:13:12.000000 slapos.core-1.9.2/CHANGES.rst
--rw-r--r--   0 tomo      (1000) tomo      (1000)      215 2019-01-24 13:19:05.000000 slapos.core-1.9.2/MANIFEST.in
--rw-r--r--   0 tomo      (1000) tomo      (1000)    67441 2023-03-24 17:13:19.789591 slapos.core-1.9.2/PKG-INFO
--rw-r--r--   0 tomo      (1000) tomo      (1000)      162 2019-01-24 13:19:05.000000 slapos.core-1.9.2/README.rst
--rw-r--r--   0 tomo      (1000) tomo      (1000)      189 2023-03-24 17:13:19.793591 slapos.core-1.9.2/setup.cfg
--rw-r--r--   0 tomo      (1000) tomo      (1000)     5714 2023-01-25 16:39:11.000000 slapos.core-1.9.2/setup.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-03-24 17:13:19.729590 slapos.core-1.9.2/slapos/
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2887 2022-12-14 14:59:28.000000 slapos.core-1.9.2/slapos/README.console.rst
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1121 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/README.format.rst
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2852 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/README.grid.rst
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1103 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/README.manager.rst
--rw-r--r--   0 tomo      (1000) tomo      (1000)      491 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/README.proxy.rst
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1252 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/README.slap.rst
--rw-r--r--   0 tomo      (1000) tomo      (1000)      244 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/__init__.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2042 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/bang.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-03-24 17:13:19.741590 slapos.core-1.9.2/slapos/cli/
--rw-r--r--   0 tomo      (1000) tomo      (1000)        0 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/cli/__init__.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2147 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/cli/bang.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     9149 2022-10-12 09:38:50.000000 slapos.core-1.9.2/slapos/cli/boot.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     4360 2022-05-13 09:28:15.000000 slapos.core-1.9.2/slapos/cli/cache_binarysr.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     3859 2022-05-13 09:28:15.000000 slapos.core-1.9.2/slapos/cli/cache_pypi.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     3714 2022-05-13 09:28:15.000000 slapos.core-1.9.2/slapos/cli/cache_url.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1915 2021-07-29 16:59:57.000000 slapos.core-1.9.2/slapos/cli/collect.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-03-24 17:13:19.745590 slapos.core-1.9.2/slapos/cli/coloredlogs/
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1056 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/cli/coloredlogs/LICENSE.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)     5680 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/cli/coloredlogs/README.rst
--rw-r--r--   0 tomo      (1000) tomo      (1000)     9204 2021-12-15 17:10:09.000000 slapos.core-1.9.2/slapos/cli/coloredlogs/__init__.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     4103 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/cli/coloredlogs/converter.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1220 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/cli/coloredlogs/demo.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2314 2021-06-01 08:31:24.000000 slapos.core-1.9.2/slapos/cli/command.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     8279 2022-03-10 14:28:56.000000 slapos.core-1.9.2/slapos/cli/complete.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2653 2021-06-01 08:31:24.000000 slapos.core-1.9.2/slapos/cli/computer_info.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2303 2021-06-01 08:31:24.000000 slapos.core-1.9.2/slapos/cli/computer_list.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2458 2021-06-01 08:31:24.000000 slapos.core-1.9.2/slapos/cli/computer_token.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     3408 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/cli/config.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     5936 2021-03-29 08:31:02.000000 slapos.core-1.9.2/slapos/cli/configure_client.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-03-24 17:13:19.745590 slapos.core-1.9.2/slapos/cli/configure_local/
--rw-r--r--   0 tomo      (1000) tomo      (1000)    10706 2022-03-10 14:28:56.000000 slapos.core-1.9.2/slapos/cli/configure_local/__init__.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     5155 2023-03-24 17:13:12.000000 slapos.core-1.9.2/slapos/cli/console.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    12312 2022-12-14 14:59:28.000000 slapos.core-1.9.2/slapos/cli/entry.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     6133 2023-03-09 05:36:51.000000 slapos.core-1.9.2/slapos/cli/format.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     4714 2023-03-22 20:27:16.000000 slapos.core-1.9.2/slapos/cli/info.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2297 2022-10-26 10:02:13.000000 slapos.core-1.9.2/slapos/cli/list.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     8937 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/cli/proxy_show.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2707 2021-06-01 08:31:24.000000 slapos.core-1.9.2/slapos/cli/proxy_start.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     8430 2021-12-15 17:10:09.000000 slapos.core-1.9.2/slapos/cli/prune.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    14657 2022-07-21 08:28:35.000000 slapos.core-1.9.2/slapos/cli/register.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2558 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/cli/remove.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     7005 2022-10-26 10:02:13.000000 slapos.core-1.9.2/slapos/cli/request.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     8795 2023-03-22 20:27:16.000000 slapos.core-1.9.2/slapos/cli/slapgrid.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     4226 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/cli/supervisorctl.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2438 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/cli/supervisord.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2644 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/cli/supply.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     5445 2023-03-24 16:05:18.000000 slapos.core-1.9.2/slapos/client.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-03-24 17:13:19.745590 slapos.core-1.9.2/slapos/collect/
--rw-r--r--   0 tomo      (1000) tomo      (1000)     7869 2020-05-12 14:37:38.000000 slapos.core-1.9.2/slapos/collect/README.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)     7294 2021-07-29 16:59:57.000000 slapos.core-1.9.2/slapos/collect/__init__.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    19241 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/collect/db.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     9850 2021-07-29 16:59:57.000000 slapos.core-1.9.2/slapos/collect/entity.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    20012 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/collect/reporter.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     9026 2021-07-29 16:59:57.000000 slapos.core-1.9.2/slapos/collect/snapshot.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-03-24 17:13:19.745590 slapos.core-1.9.2/slapos/collect/temperature/
--rw-r--r--   0 tomo      (1000) tomo      (1000)     4282 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/collect/temperature/__init__.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)      467 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/collect/temperature/heating.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    67578 2023-03-24 17:13:12.000000 slapos.core-1.9.2/slapos/format.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-03-24 17:13:19.761590 slapos.core-1.9.2/slapos/grid/
--rw-r--r--   0 tomo      (1000) tomo      (1000)    42579 2023-03-02 14:19:08.000000 slapos.core-1.9.2/slapos/grid/SlapObject.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1322 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/grid/__init__.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2609 2022-03-22 20:09:35.000000 slapos.core-1.9.2/slapos/grid/distribution.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1540 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/grid/exception.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     6825 2022-07-21 08:28:35.000000 slapos.core-1.9.2/slapos/grid/networkcache.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-03-24 17:13:19.761590 slapos.core-1.9.2/slapos/grid/promise/
--rw-r--r--   0 tomo      (1000) tomo      (1000)    33429 2021-12-15 17:10:09.000000 slapos.core-1.9.2/slapos/grid/promise/__init__.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    17418 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/grid/promise/generic.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)      601 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/grid/promise/interface.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2450 2022-03-16 16:40:25.000000 slapos.core-1.9.2/slapos/grid/promise/runpromises.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     3058 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/grid/promise/wrapper.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    77515 2023-03-02 14:19:08.000000 slapos.core-1.9.2/slapos/grid/slapgrid.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     9970 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/grid/svcbackend.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-03-24 17:13:19.761590 slapos.core-1.9.2/slapos/grid/templates/
--rw-r--r--   0 tomo      (1000) tomo      (1000)      919 2023-03-02 14:19:08.000000 slapos.core-1.9.2/slapos/grid/templates/buildout-tail.cfg.in
--rw-r--r--   0 tomo      (1000) tomo      (1000)       50 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/grid/templates/group_partition_supervisord.conf.in
--rw-r--r--   0 tomo      (1000) tomo      (1000)        0 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/grid/templates/iptables-ipv4-firewall-add.in
--rw-r--r--   0 tomo      (1000) tomo      (1000)      605 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/grid/templates/program_partition_supervisord.conf.in
--rw-r--r--   0 tomo      (1000) tomo      (1000)      749 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/grid/templates/supervisord.conf.in
--rw-r--r--   0 tomo      (1000) tomo      (1000)    16825 2023-03-02 14:19:08.000000 slapos.core-1.9.2/slapos/grid/utils.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     7381 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/grid/watchdog.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    10516 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/grid/zc.buildout-bootstrap.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     3598 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/human.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-03-24 17:13:19.765590 slapos.core-1.9.2/slapos/manager/
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1289 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/manager/__init__.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     8871 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/manager/cpuset.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     4738 2022-12-14 14:59:28.000000 slapos.core-1.9.2/slapos/manager/devperm.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1538 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/manager/interface.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     6024 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/manager/portredir.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     3128 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/manager/prerm.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     8497 2021-03-29 08:31:02.000000 slapos.core-1.9.2/slapos/manager/whitelistfirewall.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-03-24 17:13:19.765590 slapos.core-1.9.2/slapos/proxy/
--rw-r--r--   0 tomo      (1000) tomo      (1000)     4315 2021-06-01 08:31:24.000000 slapos.core-1.9.2/slapos/proxy/__init__.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)      199 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/proxy/db_version.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2018 2022-10-06 08:28:57.000000 slapos.core-1.9.2/slapos/proxy/schema.sql
--rw-r--r--   0 tomo      (1000) tomo      (1000)    47291 2023-03-22 20:27:16.000000 slapos.core-1.9.2/slapos/proxy/views.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-03-24 17:13:19.765590 slapos.core-1.9.2/slapos/slap/
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1573 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/slap/__init__.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-03-24 17:13:19.769590 slapos.core-1.9.2/slapos/slap/doc/
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2192 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/slap/doc/computer_consumption.xsd
--rw-r--r--   0 tomo      (1000) tomo      (1000)      974 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/slap/doc/partition_consumption.xsd
--rw-r--r--   0 tomo      (1000) tomo      (1000)      667 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/slap/doc/software_instance.xsd
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1864 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/slap/exception.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    17165 2022-04-12 20:02:08.000000 slapos.core-1.9.2/slapos/slap/hateoas.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-03-24 17:13:19.769590 slapos.core-1.9.2/slapos/slap/interface/
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1344 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/slap/interface/__init__.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    15731 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/slap/interface/slap.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    33167 2023-03-02 14:19:08.000000 slapos.core-1.9.2/slapos/slap/slap.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    35321 2022-05-13 09:28:20.000000 slapos.core-1.9.2/slapos/slap/standalone.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)      479 2023-03-24 17:13:19.000000 slapos.core-1.9.2/slapos/slapos-client.cfg.example
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2658 2023-03-24 17:13:19.000000 slapos.core-1.9.2/slapos/slapos-proxy.cfg.example
--rw-r--r--   0 tomo      (1000) tomo      (1000)     8783 2023-03-24 17:13:19.000000 slapos.core-1.9.2/slapos/slapos.cfg.example
--rw-r--r--   0 tomo      (1000) tomo      (1000)      953 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/slapos.xsd
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-03-24 17:13:19.773590 slapos.core-1.9.2/slapos/testing/
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1338 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/testing/__init__.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    11928 2022-12-14 14:59:28.000000 slapos.core-1.9.2/slapos/testing/check_software.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    24217 2022-03-10 14:28:56.000000 slapos.core-1.9.2/slapos/testing/testcase.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     8344 2021-12-15 17:10:09.000000 slapos.core-1.9.2/slapos/testing/utils.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-03-24 17:13:19.789591 slapos.core-1.9.2/slapos/tests/
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1628 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/tests/__init__.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-03-24 17:13:19.789591 slapos.core-1.9.2/slapos/tests/data/
--rw-r--r--   0 tomo      (1000) tomo      (1000)        0 2019-10-29 10:28:38.000000 slapos.core-1.9.2/slapos/tests/data/__init__.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-03-24 17:13:19.789591 slapos.core-1.9.2/slapos/tests/slapmock/
--rw-r--r--   0 tomo      (1000) tomo      (1000)        0 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/tests/slapmock/__init__.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)      142 2019-01-24 13:19:06.000000 slapos.core-1.9.2/slapos/tests/slapmock/requests.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     7512 2022-05-13 09:28:23.000000 slapos.core-1.9.2/slapos/tests/test_check_software.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    47967 2023-03-24 17:13:12.000000 slapos.core-1.9.2/slapos/tests/test_cli.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     3864 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/tests/test_client.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    46102 2022-03-22 09:17:21.000000 slapos.core-1.9.2/slapos/tests/test_collect.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     5696 2022-03-22 09:17:21.000000 slapos.core-1.9.2/slapos/tests/test_configure_local.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     3828 2022-03-22 20:09:35.000000 slapos.core-1.9.2/slapos/tests/test_distribution.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    14662 2023-01-25 16:39:11.000000 slapos.core-1.9.2/slapos/tests/test_grid_utils.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     4058 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/tests/test_interface.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    23962 2023-03-02 14:19:08.000000 slapos.core-1.9.2/slapos/tests/test_object.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    76488 2023-01-25 16:39:11.000000 slapos.core-1.9.2/slapos/tests/test_promise.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    13240 2021-09-28 09:41:08.000000 slapos.core-1.9.2/slapos/tests/test_prune.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-03-24 17:13:19.789591 slapos.core-1.9.2/slapos/tests/test_pyflakes/
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2210 2021-02-25 15:19:39.000000 slapos.core-1.9.2/slapos/tests/test_pyflakes/__init__.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     5226 2022-09-01 19:49:21.000000 slapos.core-1.9.2/slapos/tests/test_register.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    63442 2022-03-10 14:28:56.000000 slapos.core-1.9.2/slapos/tests/test_slap.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    33038 2023-03-22 20:27:16.000000 slapos.core-1.9.2/slapos/tests/test_slapformat.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)   188701 2023-03-02 14:19:08.000000 slapos.core-1.9.2/slapos/tests/test_slapgrid.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-03-24 17:13:19.789591 slapos.core-1.9.2/slapos/tests/test_slapproxy/
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1733 2021-06-01 08:31:24.000000 slapos.core-1.9.2/slapos/tests/test_slapproxy/slapos_multimaster.cfg.in
--rw-r--r--   0 tomo      (1000) tomo      (1000)   104385 2023-03-22 20:27:16.000000 slapos.core-1.9.2/slapos/tests/test_slapproxy.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    22430 2022-03-30 15:40:46.000000 slapos.core-1.9.2/slapos/tests/test_standalone.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    16945 2022-07-06 09:01:19.000000 slapos.core-1.9.2/slapos/tests/test_util.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)    17593 2023-03-22 20:27:16.000000 slapos.core-1.9.2/slapos/util.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1356 2023-03-24 17:13:12.000000 slapos.core-1.9.2/slapos/version.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-03-24 17:13:19.733590 slapos.core-1.9.2/slapos.core.egg-info/
--rw-r--r--   0 tomo      (1000) tomo      (1000)    67441 2023-03-24 17:13:19.000000 slapos.core-1.9.2/slapos.core.egg-info/PKG-INFO
--rw-r--r--   0 tomo      (1000) tomo      (1000)     3980 2023-03-24 17:13:19.000000 slapos.core-1.9.2/slapos.core.egg-info/SOURCES.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)        1 2023-03-24 17:13:19.000000 slapos.core-1.9.2/slapos.core.egg-info/dependency_links.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1996 2023-03-24 17:13:19.000000 slapos.core-1.9.2/slapos.core.egg-info/entry_points.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)        7 2023-03-24 17:13:19.000000 slapos.core-1.9.2/slapos.core.egg-info/namespace_packages.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)        1 2022-07-21 08:31:10.000000 slapos.core-1.9.2/slapos.core.egg-info/not-zip-safe
--rw-r--r--   0 tomo      (1000) tomo      (1000)      435 2023-03-24 17:13:19.000000 slapos.core-1.9.2/slapos.core.egg-info/requires.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)        7 2023-03-24 17:13:19.000000 slapos.core-1.9.2/slapos.core.egg-info/top_level.txt
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-04-26 07:52:45.186559 slapos.core-1.9.3/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    45042 2023-04-26 07:51:51.000000 slapos.core-1.9.3/CHANGES.rst
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      215 2019-01-24 13:19:05.000000 slapos.core-1.9.3/MANIFEST.in
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    67895 2023-04-26 07:52:45.186559 slapos.core-1.9.3/PKG-INFO
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      162 2019-01-24 13:19:05.000000 slapos.core-1.9.3/README.rst
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      189 2023-04-26 07:52:45.190559 slapos.core-1.9.3/setup.cfg
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     5714 2023-01-25 16:39:11.000000 slapos.core-1.9.3/setup.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-04-26 07:52:45.070557 slapos.core-1.9.3/slapos/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2887 2022-12-14 14:59:28.000000 slapos.core-1.9.3/slapos/README.console.rst
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     1121 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/README.format.rst
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2852 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/README.grid.rst
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     1103 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/README.manager.rst
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      491 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/README.proxy.rst
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     1252 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/README.slap.rst
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      244 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/__init__.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2042 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/bang.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-04-26 07:52:45.098557 slapos.core-1.9.3/slapos/cli/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)        0 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/cli/__init__.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2147 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/cli/bang.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     9149 2022-10-12 09:38:50.000000 slapos.core-1.9.3/slapos/cli/boot.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     4360 2022-05-13 09:28:15.000000 slapos.core-1.9.3/slapos/cli/cache_binarysr.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     3859 2022-05-13 09:28:15.000000 slapos.core-1.9.3/slapos/cli/cache_pypi.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     3714 2022-05-13 09:28:15.000000 slapos.core-1.9.3/slapos/cli/cache_url.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     1915 2021-07-29 16:59:57.000000 slapos.core-1.9.3/slapos/cli/collect.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-04-26 07:52:45.102557 slapos.core-1.9.3/slapos/cli/coloredlogs/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     1056 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/cli/coloredlogs/LICENSE.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     5680 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/cli/coloredlogs/README.rst
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     9204 2021-12-15 17:10:09.000000 slapos.core-1.9.3/slapos/cli/coloredlogs/__init__.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     4103 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/cli/coloredlogs/converter.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     1220 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/cli/coloredlogs/demo.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2314 2021-06-01 08:31:24.000000 slapos.core-1.9.3/slapos/cli/command.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     8279 2022-03-10 14:28:56.000000 slapos.core-1.9.3/slapos/cli/complete.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2653 2021-06-01 08:31:24.000000 slapos.core-1.9.3/slapos/cli/computer_info.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2303 2021-06-01 08:31:24.000000 slapos.core-1.9.3/slapos/cli/computer_list.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2458 2021-06-01 08:31:24.000000 slapos.core-1.9.3/slapos/cli/computer_token.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     3408 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/cli/config.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     5936 2021-03-29 08:31:02.000000 slapos.core-1.9.3/slapos/cli/configure_client.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-04-26 07:52:45.106557 slapos.core-1.9.3/slapos/cli/configure_local/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    10706 2022-03-10 14:28:56.000000 slapos.core-1.9.3/slapos/cli/configure_local/__init__.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     5155 2023-03-24 17:13:12.000000 slapos.core-1.9.3/slapos/cli/console.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    12312 2022-12-14 14:59:28.000000 slapos.core-1.9.3/slapos/cli/entry.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     6133 2023-03-09 05:36:51.000000 slapos.core-1.9.3/slapos/cli/format.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     4813 2023-04-26 07:51:51.000000 slapos.core-1.9.3/slapos/cli/info.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2297 2022-10-26 10:02:13.000000 slapos.core-1.9.3/slapos/cli/list.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     8937 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/cli/proxy_show.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2707 2021-06-01 08:31:24.000000 slapos.core-1.9.3/slapos/cli/proxy_start.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     8430 2021-12-15 17:10:09.000000 slapos.core-1.9.3/slapos/cli/prune.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    14657 2022-07-21 08:28:35.000000 slapos.core-1.9.3/slapos/cli/register.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2558 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/cli/remove.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     7005 2022-10-26 10:02:13.000000 slapos.core-1.9.3/slapos/cli/request.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     8795 2023-03-22 20:27:16.000000 slapos.core-1.9.3/slapos/cli/slapgrid.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     4226 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/cli/supervisorctl.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2438 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/cli/supervisord.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2644 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/cli/supply.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     5445 2023-03-24 16:05:18.000000 slapos.core-1.9.3/slapos/client.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-04-26 07:52:45.110557 slapos.core-1.9.3/slapos/collect/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     7869 2020-05-12 14:37:38.000000 slapos.core-1.9.3/slapos/collect/README.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     7294 2021-07-29 16:59:57.000000 slapos.core-1.9.3/slapos/collect/__init__.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    19241 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/collect/db.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     9850 2021-07-29 16:59:57.000000 slapos.core-1.9.3/slapos/collect/entity.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    20012 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/collect/reporter.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     9026 2021-07-29 16:59:57.000000 slapos.core-1.9.3/slapos/collect/snapshot.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-04-26 07:52:45.110557 slapos.core-1.9.3/slapos/collect/temperature/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     4282 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/collect/temperature/__init__.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      467 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/collect/temperature/heating.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    67535 2023-04-26 07:51:51.000000 slapos.core-1.9.3/slapos/format.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-04-26 07:52:45.122558 slapos.core-1.9.3/slapos/grid/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    42579 2023-03-02 14:19:08.000000 slapos.core-1.9.3/slapos/grid/SlapObject.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     1322 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/grid/__init__.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2609 2022-03-22 20:09:35.000000 slapos.core-1.9.3/slapos/grid/distribution.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     1540 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/grid/exception.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     6825 2022-07-21 08:28:35.000000 slapos.core-1.9.3/slapos/grid/networkcache.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-04-26 07:52:45.126558 slapos.core-1.9.3/slapos/grid/promise/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    33429 2021-12-15 17:10:09.000000 slapos.core-1.9.3/slapos/grid/promise/__init__.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    17418 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/grid/promise/generic.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      601 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/grid/promise/interface.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2450 2022-03-16 16:40:25.000000 slapos.core-1.9.3/slapos/grid/promise/runpromises.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     3058 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/grid/promise/wrapper.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    77773 2023-04-26 07:51:51.000000 slapos.core-1.9.3/slapos/grid/slapgrid.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     9970 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/grid/svcbackend.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-04-26 07:52:45.134558 slapos.core-1.9.3/slapos/grid/templates/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      919 2023-03-02 14:19:08.000000 slapos.core-1.9.3/slapos/grid/templates/buildout-tail.cfg.in
+-rw-r--r--   0 tomo      (1000) tomo      (1000)       50 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/grid/templates/group_partition_supervisord.conf.in
+-rw-r--r--   0 tomo      (1000) tomo      (1000)        0 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/grid/templates/iptables-ipv4-firewall-add.in
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      605 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/grid/templates/program_partition_supervisord.conf.in
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      749 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/grid/templates/supervisord.conf.in
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    16825 2023-03-02 14:19:08.000000 slapos.core-1.9.3/slapos/grid/utils.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     7381 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/grid/watchdog.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    10516 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/grid/zc.buildout-bootstrap.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     3598 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/human.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-04-26 07:52:45.142558 slapos.core-1.9.3/slapos/manager/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     1289 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/manager/__init__.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     8871 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/manager/cpuset.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     4738 2022-12-14 14:59:28.000000 slapos.core-1.9.3/slapos/manager/devperm.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     1538 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/manager/interface.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     6024 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/manager/portredir.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     3128 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/manager/prerm.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     8497 2021-03-29 08:31:02.000000 slapos.core-1.9.3/slapos/manager/whitelistfirewall.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-04-26 07:52:45.146558 slapos.core-1.9.3/slapos/proxy/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     4315 2021-06-01 08:31:24.000000 slapos.core-1.9.3/slapos/proxy/__init__.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      199 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/proxy/db_version.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2018 2022-10-06 08:28:57.000000 slapos.core-1.9.3/slapos/proxy/schema.sql
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    49770 2023-04-26 07:51:51.000000 slapos.core-1.9.3/slapos/proxy/views.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-04-26 07:52:45.150558 slapos.core-1.9.3/slapos/slap/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     1573 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/slap/__init__.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-04-26 07:52:45.154558 slapos.core-1.9.3/slapos/slap/doc/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2192 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/slap/doc/computer_consumption.xsd
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      974 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/slap/doc/partition_consumption.xsd
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      667 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/slap/doc/software_instance.xsd
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     1864 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/slap/exception.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    17165 2022-04-12 20:02:08.000000 slapos.core-1.9.3/slapos/slap/hateoas.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-04-26 07:52:45.154558 slapos.core-1.9.3/slapos/slap/interface/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     1344 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/slap/interface/__init__.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    15731 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/slap/interface/slap.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    33167 2023-03-02 14:19:08.000000 slapos.core-1.9.3/slapos/slap/slap.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    35321 2022-05-13 09:28:20.000000 slapos.core-1.9.3/slapos/slap/standalone.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      479 2023-04-26 07:52:44.000000 slapos.core-1.9.3/slapos/slapos-client.cfg.example
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2658 2023-04-26 07:52:44.000000 slapos.core-1.9.3/slapos/slapos-proxy.cfg.example
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     8912 2023-04-26 07:52:44.000000 slapos.core-1.9.3/slapos/slapos.cfg.example
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      953 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/slapos.xsd
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-04-26 07:52:45.158558 slapos.core-1.9.3/slapos/testing/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     1338 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/testing/__init__.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    11928 2022-12-14 14:59:28.000000 slapos.core-1.9.3/slapos/testing/check_software.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    24217 2022-03-10 14:28:56.000000 slapos.core-1.9.3/slapos/testing/testcase.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     8344 2021-12-15 17:10:09.000000 slapos.core-1.9.3/slapos/testing/utils.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-04-26 07:52:45.182559 slapos.core-1.9.3/slapos/tests/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     1628 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/tests/__init__.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-04-26 07:52:45.182559 slapos.core-1.9.3/slapos/tests/data/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)        0 2019-10-29 10:28:38.000000 slapos.core-1.9.3/slapos/tests/data/__init__.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-04-26 07:52:45.182559 slapos.core-1.9.3/slapos/tests/slapmock/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)        0 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/tests/slapmock/__init__.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      142 2019-01-24 13:19:06.000000 slapos.core-1.9.3/slapos/tests/slapmock/requests.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     7512 2022-05-13 09:28:23.000000 slapos.core-1.9.3/slapos/tests/test_check_software.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    48119 2023-04-26 07:51:51.000000 slapos.core-1.9.3/slapos/tests/test_cli.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     3864 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/tests/test_client.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    46102 2022-03-22 09:17:21.000000 slapos.core-1.9.3/slapos/tests/test_collect.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     5696 2022-03-22 09:17:21.000000 slapos.core-1.9.3/slapos/tests/test_configure_local.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     3828 2022-03-22 20:09:35.000000 slapos.core-1.9.3/slapos/tests/test_distribution.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    14662 2023-01-25 16:39:11.000000 slapos.core-1.9.3/slapos/tests/test_grid_utils.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     4058 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/tests/test_interface.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    23962 2023-03-02 14:19:08.000000 slapos.core-1.9.3/slapos/tests/test_object.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    76488 2023-01-25 16:39:11.000000 slapos.core-1.9.3/slapos/tests/test_promise.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    13240 2021-09-28 09:41:08.000000 slapos.core-1.9.3/slapos/tests/test_prune.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-04-26 07:52:45.182559 slapos.core-1.9.3/slapos/tests/test_pyflakes/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2210 2021-02-25 15:19:39.000000 slapos.core-1.9.3/slapos/tests/test_pyflakes/__init__.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     5226 2022-09-01 19:49:21.000000 slapos.core-1.9.3/slapos/tests/test_register.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    63442 2022-03-10 14:28:56.000000 slapos.core-1.9.3/slapos/tests/test_slap.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    33038 2023-03-22 20:27:16.000000 slapos.core-1.9.3/slapos/tests/test_slapformat.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)   188701 2023-03-02 14:19:08.000000 slapos.core-1.9.3/slapos/tests/test_slapgrid.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-04-26 07:52:45.186559 slapos.core-1.9.3/slapos/tests/test_slapproxy/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     1733 2021-06-01 08:31:24.000000 slapos.core-1.9.3/slapos/tests/test_slapproxy/slapos_multimaster.cfg.in
+-rw-r--r--   0 tomo      (1000) tomo      (1000)   106428 2023-04-26 07:51:51.000000 slapos.core-1.9.3/slapos/tests/test_slapproxy.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    22430 2022-03-30 15:40:46.000000 slapos.core-1.9.3/slapos/tests/test_standalone.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    16945 2022-07-06 09:01:19.000000 slapos.core-1.9.3/slapos/tests/test_util.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    17593 2023-03-22 20:27:16.000000 slapos.core-1.9.3/slapos/util.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     1356 2023-04-26 07:51:51.000000 slapos.core-1.9.3/slapos/version.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2023-04-26 07:52:45.074557 slapos.core-1.9.3/slapos.core.egg-info/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    67895 2023-04-26 07:52:44.000000 slapos.core-1.9.3/slapos.core.egg-info/PKG-INFO
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     3980 2023-04-26 07:52:44.000000 slapos.core-1.9.3/slapos.core.egg-info/SOURCES.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)        1 2023-04-26 07:52:44.000000 slapos.core-1.9.3/slapos.core.egg-info/dependency_links.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     1996 2023-04-26 07:52:44.000000 slapos.core-1.9.3/slapos.core.egg-info/entry_points.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)        7 2023-04-26 07:52:44.000000 slapos.core-1.9.3/slapos.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)        1 2023-04-26 07:52:44.000000 slapos.core-1.9.3/slapos.core.egg-info/not-zip-safe
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      435 2023-04-26 07:52:44.000000 slapos.core-1.9.3/slapos.core.egg-info/requires.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)        7 2023-04-26 07:52:44.000000 slapos.core-1.9.3/slapos.core.egg-info/top_level.txt
```

### Comparing `slapos.core-1.9.2/CHANGES.rst` & `slapos.core-1.9.3/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changes
 =======
 
+1.9.3 (2023-04-26)
+------------------
+ * slapgrid: run promise with clean environment
+ * slapproxy: Fix Python2 syntax incompatibility
+ * slapproxy: Show shared in slapos service list/info
+ * cli/info: Report whether the instance is shared
+ * slapformat: Fix crash in specific code path
+ * cli/info: Include software-type in output
+ * slapformat: Fix ipv6_prefixshift typo
+
 1.9.2 (2023-03-24)
 ------------------
  * console: support args when passing a script file
  * format: fix sapos node format at boot time
  * client: add getInformation shorthand method
 
 1.9.1 (2023-03-22)
```

### Comparing `slapos.core-1.9.2/PKG-INFO` & `slapos.core-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 Metadata-Version: 2.1
 Name: slapos.core
-Version: 1.9.2
+Version: 1.9.3
 Summary: SlapOS core.
 Home-page: https://slapos.nexedi.com/
 Author: VIFIB
 License: GPLv3
 Description: slapos.core
         ===========
         
         The core of SlapOS.
         Contains the SLAP library, and the slapos command line tools.
         For more information, see https://slapos.nexedi.com/ .
         
         Changes
         =======
         
+        1.9.3 (2023-04-26)
+        ------------------
+         * slapgrid: run promise with clean environment
+         * slapproxy: Fix Python2 syntax incompatibility
+         * slapproxy: Show shared in slapos service list/info
+         * cli/info: Report whether the instance is shared
+         * slapformat: Fix crash in specific code path
+         * cli/info: Include software-type in output
+         * slapformat: Fix ipv6_prefixshift typo
+        
         1.9.2 (2023-03-24)
         ------------------
          * console: support args when passing a script file
          * format: fix sapos node format at boot time
          * client: add getInformation shorthand method
         
         1.9.1 (2023-03-22)
```

### Comparing `slapos.core-1.9.2/setup.py` & `slapos.core-1.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/README.console.rst` & `slapos.core-1.9.3/slapos/README.console.rst`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/README.format.rst` & `slapos.core-1.9.3/slapos/README.format.rst`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/README.grid.rst` & `slapos.core-1.9.3/slapos/README.grid.rst`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/README.manager.rst` & `slapos.core-1.9.3/slapos/README.manager.rst`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/README.slap.rst` & `slapos.core-1.9.3/slapos/README.slap.rst`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/bang.py` & `slapos.core-1.9.3/slapos/bang.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/bang.py` & `slapos.core-1.9.3/slapos/cli/bang.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/boot.py` & `slapos.core-1.9.3/slapos/cli/boot.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/cache_binarysr.py` & `slapos.core-1.9.3/slapos/cli/cache_binarysr.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/cache_pypi.py` & `slapos.core-1.9.3/slapos/cli/cache_pypi.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/cache_url.py` & `slapos.core-1.9.3/slapos/cli/cache_url.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/collect.py` & `slapos.core-1.9.3/slapos/cli/collect.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/coloredlogs/LICENSE.txt` & `slapos.core-1.9.3/slapos/cli/coloredlogs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/coloredlogs/README.rst` & `slapos.core-1.9.3/slapos/cli/coloredlogs/README.rst`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/coloredlogs/__init__.py` & `slapos.core-1.9.3/slapos/cli/coloredlogs/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/coloredlogs/converter.py` & `slapos.core-1.9.3/slapos/cli/coloredlogs/converter.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/coloredlogs/demo.py` & `slapos.core-1.9.3/slapos/cli/coloredlogs/demo.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/command.py` & `slapos.core-1.9.3/slapos/cli/command.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/complete.py` & `slapos.core-1.9.3/slapos/cli/complete.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/computer_info.py` & `slapos.core-1.9.3/slapos/cli/computer_info.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/computer_list.py` & `slapos.core-1.9.3/slapos/cli/computer_list.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/computer_token.py` & `slapos.core-1.9.3/slapos/cli/computer_token.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/config.py` & `slapos.core-1.9.3/slapos/cli/config.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/configure_client.py` & `slapos.core-1.9.3/slapos/cli/configure_client.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/configure_local/__init__.py` & `slapos.core-1.9.3/slapos/cli/configure_local/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/console.py` & `slapos.core-1.9.3/slapos/cli/console.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/entry.py` & `slapos.core-1.9.3/slapos/cli/entry.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/format.py` & `slapos.core-1.9.3/slapos/cli/format.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/info.py` & `slapos.core-1.9.3/slapos/cli/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,16 @@
     if software_serialisation == SoftwareReleaseSerialisation.JsonInXml:
         if '_' in connection_parameter_dict:
             connection_parameter_dict = json.loads(connection_parameter_dict['_'])
 
 
     info = {
         'software-url': instance._software_release_url,
+        'software-type': instance._source_reference,
+        'shared': bool(instance._root_slave),
         'requested-state': instance._requested_state,
         'instance-parameters': instance._parameter_dict,
         'connection-parameters': connection_parameter_dict,
     }
 
     try:
         news = instance._news['instance']
```

### Comparing `slapos.core-1.9.2/slapos/cli/list.py` & `slapos.core-1.9.3/slapos/cli/list.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/proxy_show.py` & `slapos.core-1.9.3/slapos/cli/proxy_show.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/proxy_start.py` & `slapos.core-1.9.3/slapos/cli/proxy_start.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/prune.py` & `slapos.core-1.9.3/slapos/cli/prune.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/register.py` & `slapos.core-1.9.3/slapos/cli/register.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/remove.py` & `slapos.core-1.9.3/slapos/cli/remove.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/request.py` & `slapos.core-1.9.3/slapos/cli/request.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/slapgrid.py` & `slapos.core-1.9.3/slapos/cli/slapgrid.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/supervisorctl.py` & `slapos.core-1.9.3/slapos/cli/supervisorctl.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/supervisord.py` & `slapos.core-1.9.3/slapos/cli/supervisord.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/cli/supply.py` & `slapos.core-1.9.3/slapos/cli/supply.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/client.py` & `slapos.core-1.9.3/slapos/client.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/collect/README.txt` & `slapos.core-1.9.3/slapos/collect/README.txt`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/collect/__init__.py` & `slapos.core-1.9.3/slapos/collect/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/collect/db.py` & `slapos.core-1.9.3/slapos/collect/db.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/collect/entity.py` & `slapos.core-1.9.3/slapos/collect/entity.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/collect/reporter.py` & `slapos.core-1.9.3/slapos/collect/reporter.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/collect/snapshot.py` & `slapos.core-1.9.3/slapos/collect/snapshot.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/collect/temperature/__init__.py` & `slapos.core-1.9.3/slapos/collect/temperature/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/format.py` & `slapos.core-1.9.3/slapos/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -686,15 +686,15 @@
           #  * global IPv6
           if not partition.address_list:
             # generate new addresses
             partition.address_list.append(self.interface.addIPv4LocalAddress())
             partition_ipv6_dict = self.interface.addIPv6Address(partition_index)
             # Avoid leaking prefixlen in dumped data because it is not loaded
             # otherwise format dumps a different result after the first run
-            del partition_ipv6_dict['prefixlen']
+            partition_ipv6_dict.pop('prefixlen', None)
             partition.address_list.append(partition_ipv6_dict)
           else:
             # regenerate list of addresses
             old_partition_address_list = partition.address_list
             partition.address_list = []
             if len(old_partition_address_list) != 2:
               raise ValueError(
@@ -1210,18 +1210,17 @@
     if self._checkIpv6Range(address, prefixlen):
       self._reserveIpv6Range(address, prefixlen)
       return True
     return False
 
   def _generateRandomIPv6Addr(self, address_dict):
     netmask = address_dict['netmask']
-    netmask_len = lenNetmaskIpv6(netmask)
     r = random.randint(1, 65000)
     addr = ':'.join(address_dict['addr'].split(':')[:-1] + ['%x' % r])
-    socket.inet_pton(socket.AF_INET6, address)
+    socket.inet_pton(socket.AF_INET6, addr)
     return dict(addr=addr, netmask=netmask)
 
   def _generateRandomIPv6Range(self, address_dict, suffix):
     prefixlen = lenNetmaskIpv6(address_dict['netmask'])
     prefix = binFromIpv6(address_dict['addr'])[:prefixlen]
     prefixlen += 16
     if prefixlen >= 128:
@@ -1308,22 +1307,22 @@
     result_addr['netmask'] = netmaskFromLenIPv6(result_addr['prefixlen'])
     if not tap or self._checkIpv6Range(result_addr['addr'], result_addr['prefixlen']):
       if self._addSystemAddress(result_addr['addr'], result_addr['netmask'], tap=tap):
         if tap:
           self._reserveIpv6Range(result_addr['addr'], result_addr['prefixlen'])
         return result_addr
 
-    if self._ipv6_prefixshift != 16:
+    if self.ipv6_prefixshift != 16:
       self._logger.error(
         "Address %s/%s for partition %s is already taken;"
         " aborting because IPv6 prefixshift is %s != 16" % (
           result_addr['addr'],
           result_addr['prefixlen'],
           '%s tap' % partition_index if tap else partition_index,
-          self._ipv6_prefixshift,
+          self.ipv6_prefixshift,
       ))
       raise AddressGenerationError(addr)
 
     self._logger.warning(
       "Falling back to random address selection for partition %s"
       " because %s/%s is already taken" % (
         '%s tap' % partition_index if tap else partition_index,
@@ -1371,21 +1370,21 @@
     else:
       ipv6_range = getPartitionIpv6Range(address_dict, i, self.ipv6_prefixshift)
     ipv6_range['netmask'] = netmaskFromLenIPv6(ipv6_range['prefixlen'])
     ipv6_range['network'] = '%(addr)s/%(prefixlen)d' % ipv6_range
     if self._tryReserveIpv6Range(ipv6_range['addr'], ipv6_range['prefixlen']):
       return ipv6_range
 
-    if self._ipv6_prefixshift != 16:
+    if self.ipv6_prefixshift != 16:
       self._logger.error(
         "Address % for partition %s is already taken;"
         " aborting because IPv6 prefixshift is %s != 16" % (
           ipv6_range['network'],
           '%s tun' % i if tun else i,
-          self._ipv6_prefixshift,
+          self.ipv6_prefixshift,
       ))
       raise AddressGenerationError(ipv6_range['addr'])
 
     self._logger.warning(
       "Falling back to random IPv6 range selection for partition %s"
       " because %s is already taken" % (
         '%s tun' % i if tun else i,
```

### Comparing `slapos.core-1.9.2/slapos/grid/SlapObject.py` & `slapos.core-1.9.3/slapos/grid/SlapObject.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/grid/__init__.py` & `slapos.core-1.9.3/slapos/grid/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/grid/distribution.py` & `slapos.core-1.9.3/slapos/grid/distribution.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/grid/exception.py` & `slapos.core-1.9.3/slapos/grid/exception.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/grid/networkcache.py` & `slapos.core-1.9.3/slapos/grid/networkcache.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/grid/promise/__init__.py` & `slapos.core-1.9.3/slapos/grid/promise/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/grid/promise/generic.py` & `slapos.core-1.9.3/slapos/grid/promise/generic.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/grid/promise/interface.py` & `slapos.core-1.9.3/slapos/grid/promise/interface.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/grid/promise/runpromises.py` & `slapos.core-1.9.3/slapos/grid/promise/runpromises.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/grid/promise/wrapper.py` & `slapos.core-1.9.3/slapos/grid/promise/wrapper.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/grid/slapgrid.py` & `slapos.core-1.9.3/slapos/grid/slapgrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 import traceback
 import warnings
 import logging
 import json
 import shutil
 import six
 import errno
+import pwd
 
 if six.PY3:
   import subprocess
 else:
   import subprocess32 as subprocess
 
 if sys.version_info < (2, 6):
@@ -69,15 +70,16 @@
 from slapos.grid.svcbackend import (launchSupervisord,
                                     createSupervisordConfiguration,
                                     _getSupervisordConfigurationDirectory,
                                     _getSupervisordSocketPath)
 from slapos.grid.utils import (md5digest,
                               dropPrivileges,
                               SlapPopen,
-                              updateFile)
+                              updateFile,
+                              getCleanEnvironment)
 from slapos.grid.promise import PromiseLauncher, PromiseError
 from slapos.grid.promise.generic import PROMISE_LOG_FOLDER_NAME
 from slapos.human import human2bytes
 import slapos.slap
 from netaddr import valid_ipv4, valid_ipv6
 
 
@@ -750,14 +752,16 @@
         os.dup2(1, 2)
         dropPrivileges(uid, gid, logger=self.logger)
         os.dup2(err, 2)
       process = SlapPopen(
         command,
         preexec_fn=preexec_fn,
         cwd=instance_path,
+        env=getCleanEnvironment(self.logger,
+          home_path=pwd.getpwuid(uid).pw_dir),
         universal_newlines=True,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         logger=self.logger,
         timeout=timeout,
       )
       if process.returncode == 2:
@@ -1690,15 +1694,16 @@
           # Dropping privileges
           stat_info = os.stat(instance_path)
           uid = stat_info.st_uid
           gid = stat_info.st_gid
           process_handler = SlapPopen(invocation_list,
                                       preexec_fn=lambda: dropPrivileges(uid, gid, logger=self.logger),
                                       cwd=os.path.join(instance_path, 'etc', 'report'),
-                                      env=None,
+                                      env=getCleanEnvironment(self.logger,
+                                        home_path=pwd.getpwuid(uid).pw_dir),
                                       stdout=subprocess.PIPE,
                                       stderr=subprocess.STDOUT,
                                       logger=self.logger)
           if process_handler.returncode is None:
             process_handler.kill()
           if process_handler.returncode != 0:
             clean_run = False
```

### Comparing `slapos.core-1.9.2/slapos/grid/svcbackend.py` & `slapos.core-1.9.3/slapos/grid/svcbackend.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/grid/templates/buildout-tail.cfg.in` & `slapos.core-1.9.3/slapos/grid/templates/buildout-tail.cfg.in`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/grid/templates/program_partition_supervisord.conf.in` & `slapos.core-1.9.3/slapos/grid/templates/program_partition_supervisord.conf.in`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/grid/templates/supervisord.conf.in` & `slapos.core-1.9.3/slapos/grid/templates/supervisord.conf.in`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/grid/utils.py` & `slapos.core-1.9.3/slapos/grid/utils.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/grid/watchdog.py` & `slapos.core-1.9.3/slapos/grid/watchdog.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/grid/zc.buildout-bootstrap.py` & `slapos.core-1.9.3/slapos/grid/zc.buildout-bootstrap.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/human.py` & `slapos.core-1.9.3/slapos/human.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/manager/__init__.py` & `slapos.core-1.9.3/slapos/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/manager/cpuset.py` & `slapos.core-1.9.3/slapos/manager/cpuset.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/manager/devperm.py` & `slapos.core-1.9.3/slapos/manager/devperm.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/manager/interface.py` & `slapos.core-1.9.3/slapos/manager/interface.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/manager/portredir.py` & `slapos.core-1.9.3/slapos/manager/portredir.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/manager/prerm.py` & `slapos.core-1.9.3/slapos/manager/prerm.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/manager/whitelistfirewall.py` & `slapos.core-1.9.3/slapos/manager/whitelistfirewall.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/proxy/__init__.py` & `slapos.core-1.9.3/slapos/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/proxy/schema.sql` & `slapos.core-1.9.3/slapos/proxy/schema.sql`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/proxy/views.py` & `slapos.core-1.9.3/slapos/proxy/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1033,14 +1033,37 @@
     p = dict(row)
     p['url_string'] = p['software_release']
     p['title'] = p['partition_reference']
     p['relative_url'] = url_for('hateoas_partitions', partition_reference=p['partition_reference'])
     partitions.append(p)
   return partitions
 
+def busy_root_shared_list(title=None):
+  shared = []
+  query = 'SELECT * FROM %s WHERE asked_by==""'
+  args = []
+  if title:
+    query += ' AND reference=?'
+    args.append('_' + title)
+  for row in execute_db('slave', query, args):
+    host = execute_db('partition', 'SELECT * FROM %s WHERE reference=?', [row['hosted_by']], one=True)
+    if not host:
+      continue
+    for slave_dict in loads(host['slave_instance_list'].encode('utf-8')):
+      if slave_dict['slave_reference'] == row['reference']:
+        break
+    else:
+      continue
+    s = {}
+    s['url_string'] = host['software_release']
+    s['title'] = row['reference'][1:] # root shared are prefixed with _
+    s['relative_url'] = url_for('hateoas_shared', shared_reference=s['title'])
+    shared.append(s)
+  return shared
+
 def computers_list(reference=None):
   computers = []
   query = 'SELECT * FROM %s'
   args = []
   if reference:
     query += ' WHERE reference=?'
     args.append(reference)
@@ -1062,65 +1085,111 @@
 p_service_list = 'portal_type:"Instance Tree" AND validation_state:validated'
 p_service_info = p_service_list + ' AND title:='
 p_computer_list = 'portal_type:"Computer" AND validation_state:validated'
 p_computer_info = p_computer_list + ' AND reference:='
 
 def parse_query(query):
   if query == p_service_list:
-    return busy_root_partitions_list()
+    return busy_root_partitions_list() + busy_root_shared_list()
   elif query.startswith(p_service_info):
     title = query[len(p_service_info):]
     if is_valid(title):
-      return busy_root_partitions_list(title.strip('"'))
+      partition = busy_root_partitions_list(title.strip('"'))
+      if partition:
+        return partition
+      return busy_root_shared_list(title.strip('"'))
   elif query == p_computer_list:
     return computers_list()
   elif query.startswith(p_computer_info):
     reference = query[len(p_computer_info):]
     if is_valid(reference):
       return computers_list(reference.strip('"'))
   return None
 
 @app.route('/hateoas/partitions/<partition_reference>', methods=['GET'])
 def hateoas_partitions(partition_reference):
   partition = execute_db('partition', 'SELECT * FROM %s WHERE partition_reference=?', [partition_reference], one=True)
   if partition is None:
     abort(404)
+  partition['reference'] = partition['partition_reference']
+  partition['shared'] = 0
+  return hateoas_service_document(**partition)
+
+@app.route('/hateoas/shared/<shared_reference>', methods=['GET'])
+def hateoas_shared(shared_reference):
+  slave_reference = '_' + shared_reference # root shared are prefixed with _ in db
+  shared = execute_db('slave', 'SELECT * FROM %s WHERE reference=?', [slave_reference], one=True)
+  if shared is None:
+    abort(404)
+  partition = execute_db('partition', 'SELECT * FROM %s WHERE reference=?', [shared['hosted_by']], one=True)
+  if partition is None:
+    abort(404)
+  slave_list = loads(partition['slave_instance_list'].encode('utf-8'))
+  for slave_dict in slave_list:
+    if slave_dict['slave_reference'] == slave_reference:
+      break
+  else:
+    abort(404)
+  del slave_dict['slave_title'], slave_dict['slave_reference']
+  software_type = slave_dict.pop('slap_software_type')
+  xml = dict2xml(slave_dict)
+  return hateoas_service_document(
+    reference = shared_reference,
+    requested_state='unused',
+    xml=xml,
+    connection_xml=shared['connection_xml'],
+    software_release=partition['software_release'],
+    software_type=software_type,
+    shared=1,
+  )
+
+def hateoas_service_document(**kw):
   # my_slap_state corresponds to requested_state, not slap_state.
   return {
     '_embedded': {
       '_view': {
         'form_id': {
           'type': 'StringField',
-          'key': 'partition',
-          'default': partition['reference'],
+          'key': 'form_id',
+          'default': 'InstanceTree_viewAsHateoas',
         },
         'my_reference': {
           'type': 'StringField',
-          'key': 'partition_reference',
-          'default': partition['partition_reference'],
+          'key': 'field_my_reference',
+          'default': kw['reference'],
         },
         'my_slap_state': {
           'type': 'StringField',
-          'key': 'slap_state',
-          'default': partition['requested_state'],
+          'key': 'field_my_slap_state',
+          'default': kw['requested_state'],
         },
         'my_text_content': {
           'type': 'StringField',
-          'key': 'xml',
-          'default': partition['xml'],
+          'key': 'field_my_text_content',
+          'default': kw['xml'],
         },
         'my_connection_parameter_list': {
           'type': 'StringField',
-          'key': 'connection_xml',
-          'default': partition['connection_xml'],
+          'key': 'field_my_connection_parameter_list',
+          'default': kw['connection_xml'],
         },
         'my_url_string': {
           'type': 'StringField',
-          'key': 'software_release',
-          'default': partition['software_release'],
+          'key': 'field_my_url_string',
+          'default': kw['software_release'],
+        },
+        'my_source_reference': {
+          'type': 'StringField',
+          'key': 'field_my_source_reference',
+          'default': kw['software_type'],
+        },
+        'my_root_slave': {
+          'type': 'IntegerField',
+          'key': 'field_my_root_slave',
+          'default': kw['shared'],
         },
       },
     },
     '_links': {
       'type': {
         'name': 'Instance Tree',
       },
```

### Comparing `slapos.core-1.9.2/slapos/slap/__init__.py` & `slapos.core-1.9.3/slapos/slap/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/slap/doc/computer_consumption.xsd` & `slapos.core-1.9.3/slapos/slap/doc/computer_consumption.xsd`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/slap/doc/partition_consumption.xsd` & `slapos.core-1.9.3/slapos/slap/doc/partition_consumption.xsd`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/slap/doc/software_instance.xsd` & `slapos.core-1.9.3/slapos/slap/doc/software_instance.xsd`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/slap/exception.py` & `slapos.core-1.9.3/slapos/slap/exception.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/slap/hateoas.py` & `slapos.core-1.9.3/slapos/slap/hateoas.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/slap/interface/__init__.py` & `slapos.core-1.9.3/slapos/slap/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/slap/interface/slap.py` & `slapos.core-1.9.3/slapos/slap/interface/slap.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/slap/slap.py` & `slapos.core-1.9.3/slapos/slap/slap.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/slap/standalone.py` & `slapos.core-1.9.3/slapos/slap/standalone.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/slapos-proxy.cfg.example` & `slapos.core-1.9.3/slapos/slapos-proxy.cfg.example`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/slapos.cfg.example` & `slapos.core-1.9.3/slapos/slapos.cfg.example`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 tap_base_name = slaptap
 # Change "tap_ipv6" into "false" if you don't want the tap to have IPv6 addresses (tap will have only IPv4)
 # This option has no effect if create_tap is false
 tap_ipv6 = true
 # You can choose any other local network which does not conflict with your
 # current machine configuration
 ipv4_local_network = 10.0.0.0/16
+# Use this option to set the prefixlength of IPv6 subranges compared to the top-level range (default 16)
+# ipv6_prefixshift = 16
 
 # to enable, change to [firewall]
 [disabled-firewall]
 dbus_executable = /opt/slapos/parts/dbus/bin/dbus-daemon --nofork --nopidfile --system --nosyslog
 firewall_executable = /opt/slapos/parts/firewalld/sbin/firewalld --nofork --nopid --log-file /opt/slapos/log/firewalld-process.log
 firewall_cmd = /opt/slapos/parts/firewalld/bin/firewall-cmd
 reload_config_cmd = /opt/slapos/parts/firewalld/bin/firewall-cmd --reload
```

### Comparing `slapos.core-1.9.2/slapos/slapos.xsd` & `slapos.core-1.9.3/slapos/slapos.xsd`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/testing/__init__.py` & `slapos.core-1.9.3/slapos/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/testing/check_software.py` & `slapos.core-1.9.3/slapos/testing/check_software.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/testing/testcase.py` & `slapos.core-1.9.3/slapos/testing/testcase.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/testing/utils.py` & `slapos.core-1.9.3/slapos/testing/utils.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/tests/__init__.py` & `slapos.core-1.9.3/slapos/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/tests/test_check_software.py` & `slapos.core-1.9.3/slapos/tests/test_check_software.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/tests/test_cli.py` & `slapos.core-1.9.3/slapos/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -658,14 +658,16 @@
     conn = {'myconnectionparameter': 'value1'}
     if xml:
       conn_params = dict2xml(conn)
     else:
       conn_params = '<instance>\n  <parameter id="_">%s</parameter>\n</instance>' % json.dumps(conn)
     instance = slapos.slap.SoftwareInstance(
       _software_release_url='SR1',
+      _source_reference='mytype',
+      _root_slave=False,
       _requested_state='mystate',
       _connection_dict=conn_params,
       _parameter_dict={'myinstanceparameter': 'value2'})
     if news:
       instance._news = {'instance': news}
     return instance
 
@@ -678,14 +680,16 @@
     with patch.object(slapos.slap.OpenOrder, 'getInformation',
                       return_value=instance):
       slapos.cli.info.do_info(self.logger, self.conf, self.local)
 
     if six.PY3:
       expected = {
         "software-url": instance._software_release_url,
+        "software-type": instance._source_reference,
+        'shared': instance._root_slave,
         "requested-state": instance._requested_state,
         "instance-parameters": instance._parameter_dict,
         "connection-parameters": {
           "myconnectionparameter": "value1"
         },
         "status": status
       }
```

### Comparing `slapos.core-1.9.2/slapos/tests/test_client.py` & `slapos.core-1.9.3/slapos/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/tests/test_collect.py` & `slapos.core-1.9.3/slapos/tests/test_collect.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/tests/test_configure_local.py` & `slapos.core-1.9.3/slapos/tests/test_configure_local.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/tests/test_distribution.py` & `slapos.core-1.9.3/slapos/tests/test_distribution.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/tests/test_grid_utils.py` & `slapos.core-1.9.3/slapos/tests/test_grid_utils.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/tests/test_interface.py` & `slapos.core-1.9.3/slapos/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/tests/test_object.py` & `slapos.core-1.9.3/slapos/tests/test_object.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/tests/test_promise.py` & `slapos.core-1.9.3/slapos/tests/test_promise.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/tests/test_prune.py` & `slapos.core-1.9.3/slapos/tests/test_prune.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/tests/test_pyflakes/__init__.py` & `slapos.core-1.9.3/slapos/tests/test_pyflakes/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/tests/test_register.py` & `slapos.core-1.9.3/slapos/tests/test_register.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/tests/test_slap.py` & `slapos.core-1.9.3/slapos/tests/test_slap.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/tests/test_slapformat.py` & `slapos.core-1.9.3/slapos/tests/test_slapformat.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/tests/test_slapgrid.py` & `slapos.core-1.9.3/slapos/tests/test_slapgrid.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/tests/test_slapproxy/slapos_multimaster.cfg.in` & `slapos.core-1.9.3/slapos/tests/test_slapproxy/slapos_multimaster.cfg.in`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/tests/test_slapproxy.py` & `slapos.core-1.9.3/slapos/tests/test_slapproxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -447,15 +447,15 @@
     if not kw.get('shared'):
       self.assertLessEqual(
         float(computer_partition._parameter_dict['timestamp']), requested_at)
 
     app = self.app
     class TestConnectionHelper:
       def GET(self, path, params=None, headers=None):
-        return app.get(path, query_string=params, data=data).data
+        return app.get(path, query_string=params, headers=headers).data
 
       def POST(self, path, params=None, data=None,
               content_type='application/x-www-form-urlencoded'):
         return app.post(path, query_string=params, data=data).data
     computer_partition._connection_helper = TestConnectionHelper()
     return computer_partition
 
@@ -1213,16 +1213,17 @@
       env={"PYTHONPATH": ':'.join(sys.path)},
       cwd=os.chdir(os.path.join(os.path.dirname(slapos.proxy.__file__), os.pardir, os.pardir)),
       universal_newlines=True,
       **kwargs
     )
 
   def startProxy(self):
+    logfile = os.path.join(self._rootdir, 'proxy.log')
     self.proxy_process = self.cliDoSlapos(
-      ('proxy', 'start'),
+      ('proxy', 'start', '--log-file', logfile),
       method=subprocess.Popen,
       stdout=subprocess.DEVNULL,
       stderr=subprocess.DEVNULL,
     )
     self.app = TestAppSession(self.proxyaddr)
     # Wait a bit for proxy to be started
     for attempts in range(1, 20):
@@ -1284,47 +1285,93 @@
     self.request('http://sr2//', None, 'MyInstance2', None)
     self.request('http://sr3//', None, 'MyInstance3', 'slappart0')
     output = self.cliDoSlapos(('service', 'list'), stderr=subprocess.DEVNULL)
     self.assertEqual(
       json.loads(output),
       {'MyInstance0': 'http://sr0//', 'MyInstance1': 'http://sr1//', 'MyInstance2': 'http://sr2//'})
 
+  def test_service_list_with_shared(self):
+    self.format_for_number_of_partitions(1)
+    self.request('http://sr0//', None, 'MyHostInstance0', None)
+    self.request('http://sr0//', None, 'MySharedInstance1', None, shared=True)
+    self.request('http://sr0//', None, 'MySharedInstance2', None, shared=True)
+    output = self.cliDoSlapos(('service', 'list'), stderr=subprocess.DEVNULL)
+    self.assertEqual(
+      json.loads(output),
+      {'MyHostInstance0': 'http://sr0//', 'MySharedInstance1': 'http://sr0//', 'MySharedInstance2': 'http://sr0//'})
+
   def test_service_info(self):
     self.format_for_number_of_partitions(3)
     self.request('http://sr0//', None, 'MyInstance0', None)
-    self.request('http://sr1//', None, 'MyInstance1', None, partition_parameter_kw={'couscous': 'hello'})
+    self.request('http://sr1//', "MyType1", 'MyInstance1', None, partition_parameter_kw={'couscous': 'hello'})
     self.request('http://sr2//', None, 'MyInstance2', 'slappart0')
     output0 = self.cliDoSlapos(('service', 'info', 'MyInstance0'), stderr=subprocess.DEVNULL)
     self.assertEqual(
       json.loads(output0),
       {
         "software-url": "http://sr0//",
+        "software-type": "default",
+        "shared": False,
         "requested-state": "started",
         "instance-parameters": {},
         "connection-parameters": {},
         "status": "unsupported",
       },
     )
     output1 = self.cliDoSlapos(('service', 'info', 'MyInstance1'), stderr=subprocess.DEVNULL)
     self.assertEqual(
       json.loads(output1),
       {
         "software-url": "http://sr1//",
+        "software-type": "MyType1",
+        "shared": False,
         "requested-state": "started",
         "instance-parameters": {"couscous": "hello"},
         "connection-parameters": {},
         "status": "unsupported",
       },
     )
     try:
       self.cliDoSlapos(('service', 'info', 'MyInstance2'), stderr=subprocess.STDOUT)
       self.fail()
     except subprocess.CalledProcessError as e:
       self.assertIn('Instance MyInstance2 does not exist.', e.output)
 
+  def test_service_info_with_shared(self):
+    self.format_for_number_of_partitions(1)
+    self.request('http://sr0//', 'MyType1', 'MyHostInstance0', None)
+    self.request('http://sr0//', 'MyType1', 'MySharedInstance1', None, shared=True, partition_parameter_kw={'couscous': 'hello'})
+    self.request('http://sr0//', 'MyType1', 'MySharedInstance2', None, shared=True, partition_parameter_kw={'couscous': 'bye'})
+    output0 = self.cliDoSlapos(('service', 'info', 'MySharedInstance1'), stderr=subprocess.DEVNULL)
+    self.assertEqual(
+      json.loads(output0),
+      {
+        "software-url": "http://sr0//",
+        "software-type": "MyType1",
+        "shared": True,
+        "requested-state": "unused",
+        "instance-parameters": {"couscous": "hello"},
+        "connection-parameters": {},
+        "status": "unsupported",
+      },
+    )
+    output1 = self.cliDoSlapos(('service', 'info', 'MySharedInstance2'), stderr=subprocess.DEVNULL)
+    self.assertEqual(
+      json.loads(output1),
+      {
+        "software-url": "http://sr0//",
+        "software-type": "MyType1",
+        "shared": True,
+        "requested-state": "unused",
+        "instance-parameters": {"couscous": "bye"},
+        "connection-parameters": {},
+        "status": "unsupported",
+      },
+    )
+
   def test_invalid_service_names(self):
     invalid_names = ('"MyInstance0', 'MyInstance1"', 'My"Instance2', 'title:="MyInstance3"', 'reference:="MyInstance4"')
     self.format_for_number_of_partitions(len(invalid_names))
     for i, name in enumerate(invalid_names):
       self.request('http://sr%d//' % i, None, name)
     for i, name in enumerate(invalid_names):
       try:
```

### Comparing `slapos.core-1.9.2/slapos/tests/test_standalone.py` & `slapos.core-1.9.3/slapos/tests/test_standalone.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/tests/test_util.py` & `slapos.core-1.9.3/slapos/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/util.py` & `slapos.core-1.9.3/slapos/util.py`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos/version.py` & `slapos.core-1.9.3/slapos/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
 
-version = '1.9.2'
+version = '1.9.3'
```

### Comparing `slapos.core-1.9.2/slapos.core.egg-info/PKG-INFO` & `slapos.core-1.9.3/slapos.core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 Metadata-Version: 2.1
 Name: slapos.core
-Version: 1.9.2
+Version: 1.9.3
 Summary: SlapOS core.
 Home-page: https://slapos.nexedi.com/
 Author: VIFIB
 License: GPLv3
 Description: slapos.core
         ===========
         
         The core of SlapOS.
         Contains the SLAP library, and the slapos command line tools.
         For more information, see https://slapos.nexedi.com/ .
         
         Changes
         =======
         
+        1.9.3 (2023-04-26)
+        ------------------
+         * slapgrid: run promise with clean environment
+         * slapproxy: Fix Python2 syntax incompatibility
+         * slapproxy: Show shared in slapos service list/info
+         * cli/info: Report whether the instance is shared
+         * slapformat: Fix crash in specific code path
+         * cli/info: Include software-type in output
+         * slapformat: Fix ipv6_prefixshift typo
+        
         1.9.2 (2023-03-24)
         ------------------
          * console: support args when passing a script file
          * format: fix sapos node format at boot time
          * client: add getInformation shorthand method
         
         1.9.1 (2023-03-22)
```

### Comparing `slapos.core-1.9.2/slapos.core.egg-info/SOURCES.txt` & `slapos.core-1.9.3/slapos.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slapos.core-1.9.2/slapos.core.egg-info/entry_points.txt` & `slapos.core-1.9.3/slapos.core.egg-info/entry_points.txt`

 * *Files identical despite different names*

