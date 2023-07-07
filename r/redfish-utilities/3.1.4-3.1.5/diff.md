# Comparing `tmp/redfish_utilities-3.1.4.tar.gz` & `tmp/redfish_utilities-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfish_utilities-3.1.4.tar", last modified: Fri Jun 16 20:13:54 2023, max compression
+gzip compressed data, was "redfish_utilities-3.1.5.tar", last modified: Fri Jul  7 20:05:04 2023, max compression
```

## Comparing `redfish_utilities-3.1.4.tar` & `redfish_utilities-3.1.5.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:13:54.407136 redfish_utilities-3.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    37487 2023-06-16 20:13:54.407136 redfish_utilities-3.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36943 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:13:54.403136 redfish_utilities-3.1.4/redfish_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/event_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    17199 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17174 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/resets.py
--rw-r--r--   0 runner    (1001) docker     (123)    22012 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)    25527 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/systems.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:13:54.403136 redfish_utilities-3.1.4/redfish_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37487 2023-06-16 20:13:54.000000 redfish_utilities-3.1.4/redfish_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-16 20:13:54.000000 redfish_utilities-3.1.4/redfish_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:13:54.000000 redfish_utilities-3.1.4/redfish_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 20:13:54.000000 redfish_utilities-3.1.4/redfish_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-16 20:13:54.000000 redfish_utilities-3.1.4/redfish_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:13:54.407136 redfish_utilities-3.1.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_bios_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_boot_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_diagnostic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_discover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_event_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_manager_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_power_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_raw_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_sensor_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_sys_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_virtual_media.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 20:13:54.407136 redfish_utilities-3.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:05:04.359438 redfish_utilities-3.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    41821 2023-07-07 20:05:04.359438 redfish_utilities-3.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    41277 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:05:04.359438 redfish_utilities-3.1.5/redfish_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/event_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17199 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22420 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/resets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22012 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25527 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:05:04.359438 redfish_utilities-3.1.5/redfish_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41821 2023-07-07 20:05:03.000000 redfish_utilities-3.1.5/redfish_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-07 20:05:03.000000 redfish_utilities-3.1.5/redfish_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 20:05:03.000000 redfish_utilities-3.1.5/redfish_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-07 20:05:03.000000 redfish_utilities-3.1.5/redfish_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 20:05:03.000000 redfish_utilities-3.1.5/redfish_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:05:04.359438 redfish_utilities-3.1.5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_bios_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_boot_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_diagnostic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_event_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_power_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_raw_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_sensor_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_sys_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_virtual_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 20:05:04.359438 redfish_utilities-3.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/setup.py
```

### Comparing `redfish_utilities-3.1.4/LICENSE.md` & `redfish_utilities-3.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/PKG-INFO` & `redfish_utilities-3.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: redfish_utilities
-Version: 3.1.4
-Summary: Redfish Utilities
-Home-page: https://github.com/DMTF/Redfish-Tacklebox
-Author: DMTF, https://www.dmtf.org/standards/feedback
-License: BSD 3-clause "New" or "Revised License"
-Keywords: Redfish
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Communications
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-License-File: AUTHORS.md
-
 # Redfish Tacklebox
 
 Copyright 2019-2022 DMTF. All rights reserved.
 
 ## About
 
 Redfish Tacklebox contains a set of Python3 utilities to perform common management operations with a Redfish service.
@@ -264,19 +248,20 @@
 usage: rf_manager_config.py [-h] --user USER --password PASSWORD --rhost RHOST
                             [--manager MANAGER]
                             {info,reset,getnet,setnet} ...
 
 A tool to manage managers in a service
 
 positional arguments:
-  {info,reset,getnet,setnet}
+  {info,reset,getnet,setnet,resettodefaults}
     info                Displays information about a manager
     reset               Resets a manager
     getnet              Displays information about an Ethernet interface
     setnet              Configures an Ethernet interface
+    resettodefaults     Resets a manager to default setting
 
 required arguments:
   --user USER, -u USER  The user name for authentication
   --password PASSWORD, -p PASSWORD
                         The password for authentication
   --rhost RHOST, -r RHOST
                         The address of the Redfish service (with scheme)
@@ -313,15 +298,14 @@
                                   [--info]
 
 optional arguments:
   -h, --help            show this help message and exit
   --type {On,ForceOff,GracefulShutdown,GracefulRestart,ForceRestart,Nmi,ForceOn,PushPowerButton,PowerCycle}, -t {On,ForceOff,GracefulShutdown,GracefulRestart,ForceRestart,Nmi,ForceOn,PushPowerButton,PowerCycle}
                         The type of power/reset operation to perform
   --info, -info         Indicates if reset information should be reported
-
 ```
 
 Example: `rf_manager_config.py -u root -p root -r https://192.168.1.100 reset -t GracefulRestart`
 
 The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
 It then traverses the manager collection for the service to find the matching system specified by the *manager* argument.
 It will perform the `Reset` action with the specified reset type from the *type* argument.
@@ -352,15 +336,15 @@
 ```
 usage: rf_manager_config.py setnet [-h] [--id ID] [--ipv4address IPV4ADDRESS]
                                    [--ipv4netmask IPV4NETMASK]
                                    [--ipv4gateway IPV4GATEWAY]
                                    [--dhcpv4 {On,Off}]
                                    [--ipv6addresses IPV6ADDRESSES [IPV6ADDRESSES ...]]
                                    [--ipv6gateways IPV6GATEWAYS [IPV6GATEWAYS ...]]
-                                   [--dhcpv6 {Stateful,Stateless,Disabled}]
+                                   [--dhcpv6 {Stateful,Stateless,Disabled,Enabled}]
                                    [--vlan {On,Off}] [--vlanid VLANID]
                                    [--vlanpriority VLANPRIORITY]
 
 optional arguments:
   -h, --help            show this help message and exit
   --id ID, -i ID        The identifier of the Ethernet interface to configure
   --ipv4address IPV4ADDRESS, -ipv4address IPV4ADDRESS
@@ -372,15 +356,15 @@
   --dhcpv4 {On,Off}, -dhcpv4 {On,Off}
                         The DHCPv4 configuration to set
   --ipv6addresses IPV6ADDRESSES [IPV6ADDRESSES ...], -ipv6addresses IPV6ADDRESSES [IPV6ADDRESSES ...]
                         The static IPv6 addresses to set with prefix length
   --ipv6gateways IPV6GATEWAYS [IPV6GATEWAYS ...], -ipv6gateways IPV6GATEWAYS [IPV6GATEWAYS ...]
                         The static IPv6 default gateways to set with prefix
                         length
-  --dhcpv6 {Stateful,Stateless,Disabled}, -dhcpv6 {Stateful,Stateless,Disabled}
+  --dhcpv6 {Stateful,Stateless,Disabled,Enabled}, -dhcpv6 {Stateful,Stateless,Disabled,Enabled}
                         The DHCPv6 configuration to set
   --vlan {On,Off}, -vlan {On,Off}
                         The VLAN enabled configuration to set
   --vlanid VLANID, -vlanid VLANID
                         The VLAN ID to set
   --vlanpriority VLANPRIORITY, -vlanpriority VLANPRIORITY
                         The VLAN priority to set
@@ -390,14 +374,38 @@
 
 The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
 It will then locate the manager specified by the *manager* argument, locate the Ethernet interface specified by the *id* argument, and apply the requested settings to the interface.
 * If *manager* is not specified, and if the service has exactly one manager, it will perform the operation on the one manager.
 * If *id* is not specified, and if the manager has exactly one Ethernet interface, it will perform the operation on the one interface.
 
 
+#### Reset to Defaults
+
+```
+usage: rf_manager_config.py resettodefaults [-h]
+                                            [--type {ResetAll,PreserveNetworkAndUsers,PreserveNetwork}]
+                                            [--info]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --type {ResetAll,PreserveNetworkAndUsers,PreserveNetwork}, -t {ResetAll,PreserveNetworkAndUsers,PreserveNetwork}
+                        The type of reset-to-defaults operation to perform
+  --info, -info         Indicates if reset-to-defaults information should be
+                        reported
+```
+
+Example: `rf_manager_config.py -u root -p root -r https://192.168.1.100 resettodefaults -t ResetAll`
+
+The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
+It then traverses the manager collection for the service to find the matching system specified by the *manager* argument.
+It will perform the `ResetToDefaults` action with the specified reset type from the *type* argument.
+* If *manager* is not specified, and if the service has exactly one manager, it will perform the operation on the one manager.
+* If *type* is not specified, it will attempt to perform the action with `PreserveNetworkAndUsers`.
+
+
 ### BIOS Settings
 
 ```
 usage: rf_bios_settings.py [-h] --user USER --password PASSWORD --rhost RHOST
                            [--system SYSTEM] [--attribute name value]
 
 A tool to manager BIOS settings for a system
@@ -720,14 +728,103 @@
 Example: `rf_virtual_media.py -u root -p root -r https://192.168.1.100 eject --id 1`
 
 The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
 It will then locate the system specified by the *system* argument, find its virtual media collection.
 It will then locate the virtual media instance with matching `Id` property with the *id* argument, and then eject the media.
 
 
+### Licenses
+
+```
+usage: rf_licenses.py [-h] --user USER --password PASSWORD --rhost RHOST
+                      [--debug]
+                      {info,install,delete} ...
+
+A tool to manage licenses on a Redfish service
+
+positional arguments:
+  {info,install,delete}
+    info                Displays information about the licenses installed on
+                        the service
+    install             Installs a new license
+    delete              Deletes a license
+
+required arguments:
+  --user USER, -u USER  The user name for authentication
+  --password PASSWORD, -p PASSWORD
+                        The password for authentication
+  --rhost RHOST, -r RHOST
+                        The address of the Redfish service (with scheme)
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --debug               Creates debug file showing HTTP traces and exceptions
+```
+
+
+#### Info
+
+```
+usage: rf_licenses.py info [-h] [--details]
+
+options:
+  -h, --help           show this help message and exit
+  --details, -details  Indicates if the full details of each license should be
+                       shown
+```
+
+Example: `rf_licenses.py -u root -p root -r https://192.168.1.100 info`
+
+The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
+It will then locate the license service, find its license collection, and display the licenses.
+
+
+#### Install
+
+```
+usage: rf_licenses.py install [-h] --license LICENSE
+
+required arguments:
+  --license LICENSE, -l LICENSE
+                        The filepath or URI to the license to install
+
+optional arguments:
+  -h, --help            show this help message and exit
+``` 
+
+Example: `rf_licenses.py -u root -p root -r https://192.168.1.100 install --license /home/user/my_license.xml`
+
+The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
+It will then locate the license service.
+If the license referenced by the *license* argument is local file, it will insert the contents of the license file in the license collection.
+Otherwise, it will install the new license with the `Install` action found on the license service.
+
+
+#### Delete
+
+```
+usage: rf_licenses.py delete [-h] --license LICENSE
+
+options:
+
+required arguments:
+  --license LICENSE, -l LICENSE
+                        The identifier of the license to delete
+
+optional arguments:
+  -h, --help            show this help message and exit
+```
+
+Example: `rf_licenses.py -u root -p root -r https://192.168.1.100 delete --license 1`
+
+The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
+It will then locate the license service and find the license requested by the *license* argument.
+If the matching license is found, it will delete the license.
+
+
 ### Diagnostic Data
 
 ```
 usage: rf_diagnostic_data.py [-h] --user USER --password PASSWORD --rhost
                              RHOST [--manager [MANAGER]] [--system [SYSTEM]]
                              [--chassis [CHASSIS]] [--log LOG]
                              [--type {Manager,PreOS,OS,OEM}]
```

### Comparing `redfish_utilities-3.1.4/README.md` & `redfish_utilities-3.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: redfish_utilities
+Version: 3.1.5
+Summary: Redfish Utilities
+Home-page: https://github.com/DMTF/Redfish-Tacklebox
+Author: DMTF, https://www.dmtf.org/standards/feedback
+License: BSD 3-clause "New" or "Revised License"
+Keywords: Redfish
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Communications
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+License-File: AUTHORS.md
+
 # Redfish Tacklebox
 
 Copyright 2019-2022 DMTF. All rights reserved.
 
 ## About
 
 Redfish Tacklebox contains a set of Python3 utilities to perform common management operations with a Redfish service.
@@ -248,19 +264,20 @@
 usage: rf_manager_config.py [-h] --user USER --password PASSWORD --rhost RHOST
                             [--manager MANAGER]
                             {info,reset,getnet,setnet} ...
 
 A tool to manage managers in a service
 
 positional arguments:
-  {info,reset,getnet,setnet}
+  {info,reset,getnet,setnet,resettodefaults}
     info                Displays information about a manager
     reset               Resets a manager
     getnet              Displays information about an Ethernet interface
     setnet              Configures an Ethernet interface
+    resettodefaults     Resets a manager to default setting
 
 required arguments:
   --user USER, -u USER  The user name for authentication
   --password PASSWORD, -p PASSWORD
                         The password for authentication
   --rhost RHOST, -r RHOST
                         The address of the Redfish service (with scheme)
@@ -297,15 +314,14 @@
                                   [--info]
 
 optional arguments:
   -h, --help            show this help message and exit
   --type {On,ForceOff,GracefulShutdown,GracefulRestart,ForceRestart,Nmi,ForceOn,PushPowerButton,PowerCycle}, -t {On,ForceOff,GracefulShutdown,GracefulRestart,ForceRestart,Nmi,ForceOn,PushPowerButton,PowerCycle}
                         The type of power/reset operation to perform
   --info, -info         Indicates if reset information should be reported
-
 ```
 
 Example: `rf_manager_config.py -u root -p root -r https://192.168.1.100 reset -t GracefulRestart`
 
 The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
 It then traverses the manager collection for the service to find the matching system specified by the *manager* argument.
 It will perform the `Reset` action with the specified reset type from the *type* argument.
@@ -336,15 +352,15 @@
 ```
 usage: rf_manager_config.py setnet [-h] [--id ID] [--ipv4address IPV4ADDRESS]
                                    [--ipv4netmask IPV4NETMASK]
                                    [--ipv4gateway IPV4GATEWAY]
                                    [--dhcpv4 {On,Off}]
                                    [--ipv6addresses IPV6ADDRESSES [IPV6ADDRESSES ...]]
                                    [--ipv6gateways IPV6GATEWAYS [IPV6GATEWAYS ...]]
-                                   [--dhcpv6 {Stateful,Stateless,Disabled}]
+                                   [--dhcpv6 {Stateful,Stateless,Disabled,Enabled}]
                                    [--vlan {On,Off}] [--vlanid VLANID]
                                    [--vlanpriority VLANPRIORITY]
 
 optional arguments:
   -h, --help            show this help message and exit
   --id ID, -i ID        The identifier of the Ethernet interface to configure
   --ipv4address IPV4ADDRESS, -ipv4address IPV4ADDRESS
@@ -356,15 +372,15 @@
   --dhcpv4 {On,Off}, -dhcpv4 {On,Off}
                         The DHCPv4 configuration to set
   --ipv6addresses IPV6ADDRESSES [IPV6ADDRESSES ...], -ipv6addresses IPV6ADDRESSES [IPV6ADDRESSES ...]
                         The static IPv6 addresses to set with prefix length
   --ipv6gateways IPV6GATEWAYS [IPV6GATEWAYS ...], -ipv6gateways IPV6GATEWAYS [IPV6GATEWAYS ...]
                         The static IPv6 default gateways to set with prefix
                         length
-  --dhcpv6 {Stateful,Stateless,Disabled}, -dhcpv6 {Stateful,Stateless,Disabled}
+  --dhcpv6 {Stateful,Stateless,Disabled,Enabled}, -dhcpv6 {Stateful,Stateless,Disabled,Enabled}
                         The DHCPv6 configuration to set
   --vlan {On,Off}, -vlan {On,Off}
                         The VLAN enabled configuration to set
   --vlanid VLANID, -vlanid VLANID
                         The VLAN ID to set
   --vlanpriority VLANPRIORITY, -vlanpriority VLANPRIORITY
                         The VLAN priority to set
@@ -374,14 +390,38 @@
 
 The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
 It will then locate the manager specified by the *manager* argument, locate the Ethernet interface specified by the *id* argument, and apply the requested settings to the interface.
 * If *manager* is not specified, and if the service has exactly one manager, it will perform the operation on the one manager.
 * If *id* is not specified, and if the manager has exactly one Ethernet interface, it will perform the operation on the one interface.
 
 
+#### Reset to Defaults
+
+```
+usage: rf_manager_config.py resettodefaults [-h]
+                                            [--type {ResetAll,PreserveNetworkAndUsers,PreserveNetwork}]
+                                            [--info]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --type {ResetAll,PreserveNetworkAndUsers,PreserveNetwork}, -t {ResetAll,PreserveNetworkAndUsers,PreserveNetwork}
+                        The type of reset-to-defaults operation to perform
+  --info, -info         Indicates if reset-to-defaults information should be
+                        reported
+```
+
+Example: `rf_manager_config.py -u root -p root -r https://192.168.1.100 resettodefaults -t ResetAll`
+
+The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
+It then traverses the manager collection for the service to find the matching system specified by the *manager* argument.
+It will perform the `ResetToDefaults` action with the specified reset type from the *type* argument.
+* If *manager* is not specified, and if the service has exactly one manager, it will perform the operation on the one manager.
+* If *type* is not specified, it will attempt to perform the action with `PreserveNetworkAndUsers`.
+
+
 ### BIOS Settings
 
 ```
 usage: rf_bios_settings.py [-h] --user USER --password PASSWORD --rhost RHOST
                            [--system SYSTEM] [--attribute name value]
 
 A tool to manager BIOS settings for a system
@@ -704,14 +744,103 @@
 Example: `rf_virtual_media.py -u root -p root -r https://192.168.1.100 eject --id 1`
 
 The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
 It will then locate the system specified by the *system* argument, find its virtual media collection.
 It will then locate the virtual media instance with matching `Id` property with the *id* argument, and then eject the media.
 
 
+### Licenses
+
+```
+usage: rf_licenses.py [-h] --user USER --password PASSWORD --rhost RHOST
+                      [--debug]
+                      {info,install,delete} ...
+
+A tool to manage licenses on a Redfish service
+
+positional arguments:
+  {info,install,delete}
+    info                Displays information about the licenses installed on
+                        the service
+    install             Installs a new license
+    delete              Deletes a license
+
+required arguments:
+  --user USER, -u USER  The user name for authentication
+  --password PASSWORD, -p PASSWORD
+                        The password for authentication
+  --rhost RHOST, -r RHOST
+                        The address of the Redfish service (with scheme)
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --debug               Creates debug file showing HTTP traces and exceptions
+```
+
+
+#### Info
+
+```
+usage: rf_licenses.py info [-h] [--details]
+
+options:
+  -h, --help           show this help message and exit
+  --details, -details  Indicates if the full details of each license should be
+                       shown
+```
+
+Example: `rf_licenses.py -u root -p root -r https://192.168.1.100 info`
+
+The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
+It will then locate the license service, find its license collection, and display the licenses.
+
+
+#### Install
+
+```
+usage: rf_licenses.py install [-h] --license LICENSE
+
+required arguments:
+  --license LICENSE, -l LICENSE
+                        The filepath or URI to the license to install
+
+optional arguments:
+  -h, --help            show this help message and exit
+``` 
+
+Example: `rf_licenses.py -u root -p root -r https://192.168.1.100 install --license /home/user/my_license.xml`
+
+The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
+It will then locate the license service.
+If the license referenced by the *license* argument is local file, it will insert the contents of the license file in the license collection.
+Otherwise, it will install the new license with the `Install` action found on the license service.
+
+
+#### Delete
+
+```
+usage: rf_licenses.py delete [-h] --license LICENSE
+
+options:
+
+required arguments:
+  --license LICENSE, -l LICENSE
+                        The identifier of the license to delete
+
+optional arguments:
+  -h, --help            show this help message and exit
+```
+
+Example: `rf_licenses.py -u root -p root -r https://192.168.1.100 delete --license 1`
+
+The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
+It will then locate the license service and find the license requested by the *license* argument.
+If the matching license is found, it will delete the license.
+
+
 ### Diagnostic Data
 
 ```
 usage: rf_diagnostic_data.py [-h] --user USER --password PASSWORD --rhost
                              RHOST [--manager [MANAGER]] [--system [SYSTEM]]
                              [--chassis [CHASSIS]] [--log LOG]
                              [--type {Manager,PreOS,OS,OEM}]
```

### Comparing `redfish_utilities-3.1.4/redfish_utilities/__init__.py` & `redfish_utilities-3.1.5/redfish_utilities/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,33 +13,40 @@
 from .event_service import get_event_subscriptions
 from .event_service import print_event_subscriptions
 from .event_service import create_event_subscription
 from .event_service import delete_event_subscription
 from .inventory import get_system_inventory
 from .inventory import print_system_inventory
 from .inventory import write_system_inventory
+from .licenses import get_licenses
+from .licenses import print_licenses
+from .licenses import install_license
+from .licenses import delete_license
 from .logs import log_container
 from .logs import diagnostic_data_types
 from .logs import get_log_entries
 from .logs import print_log_entries
 from .logs import clear_log_entries
 from .logs import collect_diagnostic_data
 from .logs import download_diagnostic_data
 from .managers import get_manager_ids
 from .managers import get_manager
 from .managers import print_manager
 from .managers import get_manager_reset_info
 from .managers import manager_reset
+from .managers import get_manager_reset_to_defaults_info
+from .managers import manager_reset_to_defaults
 from .managers import get_manager_ethernet_interface_ids
 from .managers import get_manager_ethernet_interface
 from .managers import set_manager_ethernet_interface
 from .managers import print_manager_ethernet_interface
 from .messages import print_error_payload
 from .messages import verify_response
 from .resets import reset_types
+from .resets import reset_to_defaults_types
 from .sensors import get_sensors
 from .sensors import print_sensors
 from .systems import get_system_ids
 from .systems import get_system
 from .systems import get_system_boot
 from .systems import set_system_boot
 from .systems import print_system_boot
```

### Comparing `redfish_utilities-3.1.4/redfish_utilities/accounts.py` & `redfish_utilities-3.1.5/redfish_utilities/accounts.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/redfish_utilities/config.py` & `redfish_utilities-3.1.5/redfish_utilities/config.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/redfish_utilities/event_service.py` & `redfish_utilities-3.1.5/redfish_utilities/event_service.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/redfish_utilities/inventory.py` & `redfish_utilities-3.1.5/redfish_utilities/inventory.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/redfish_utilities/logs.py` & `redfish_utilities-3.1.5/redfish_utilities/logs.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/redfish_utilities/managers.py` & `redfish_utilities-3.1.5/redfish_utilities/managers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 #! /usr/bin/python
 # Copyright Notice:
-# Copyright 2019-2021 DMTF. All rights reserved.
+# Copyright 2019-2023 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Managers Module
 
 File : managers.py
 
 Brief : This file contains the definitions and functionalities for interacting
         with the managers collection for a given Redfish service
 """
 
+import sys
 from .collections import get_collection_ids
 from .messages import verify_response
 from .resets import reset_types
+from .resets import reset_to_defaults_types
 
 class RedfishManagerNotFoundError( Exception ):
     """
     Raised when a matching manager cannot be found
     """
     pass
 
@@ -30,14 +32,20 @@
 
 class RedfishManagerResetNotFoundError( Exception ):
     """
     Raised when the Reset action cannot be found
     """
     pass
 
+class RedfishManagerResetToDefaultsNotFoundError( Exception ):
+    """
+    Raised when the ResetToDefaults action cannot be found
+    """
+    pass
+
 def get_manager_ids( context ):
     """
     Finds the manager collection and returns all of the member's identifiers
 
     Args:
         context: The Redfish client object with an open session
 
@@ -45,15 +53,15 @@
         A list of identifiers of the members of the manager collection
     """
 
     # Get the service root to find the manager collection
     service_root = context.get( "/redfish/v1/" )
     if "Managers" not in service_root.dict:
         # No manager collection
-        raise RedfishManagerNotFoundError( "Service does not contain a manager collection" )
+        raise RedfishManagerNotFoundError( "The service does not contain a manager collection" )
 
     # Get the manager collection and iterate through its collection
     return get_collection_ids( context, service_root.dict["Managers"]["@odata.id"] )
 
 def get_manager( context, manager_id = None ):
     """
     Finds a manager matching the given identifier and returns its resource
@@ -74,21 +82,21 @@
         manager = context.get( manager_uri_pattern.format( manager_id ) )
     # No identifier given; see if there's exactly one member
     else:
         avail_managers = get_manager_ids( context )
         if len( avail_managers ) == 1:
             manager = context.get( manager_uri_pattern.format( avail_managers[0] ) )
         else:
-            raise RedfishManagerNotFoundError( "Service does not contain exactly one manager; a target manager needs to be specified: {}".format( ", ".join( avail_managers ) ) )
+            raise RedfishManagerNotFoundError( "The service does not contain exactly one manager; a target manager needs to be specified: {}".format( ", ".join( avail_managers ) ) )
 
     # Check the response and return the manager if the response is good
     if manager.status == 404:
         if avail_managers is None:
             avail_managers = get_manager_ids( context )
-        raise RedfishManagerNotFoundError( "Service does not contain a manager called {}; valid managers: {}".format( manager_id, ", ".join( avail_managers ) ) )
+        raise RedfishManagerNotFoundError( "The service does not contain a manager called {}; valid managers: {}".format( manager_id, ", ".join( avail_managers ) ) )
     verify_response( manager )
     return manager
 
 def print_manager( manager ):
     """
     Prints the manager info
 
@@ -117,32 +125,32 @@
     Args:
         context: The Redfish client object with an open session
         manager_id: The manager to locate; if None, perform on the only manager
         manager: Existing manager resource to inspect for reset info
 
     Returns:
         The URI of the Reset action
-        A list of parameter requirements from the Action Info
+        A list of parameter requirements from the action info
     """
 
     if manager is None:
         manager = get_manager( context, manager_id )
 
     # Check that there is a Reset action
     if "Actions" not in manager.dict:
-        raise RedfishManagerResetNotFoundError( "Manager does not support Reset" )
+        raise RedfishManagerResetNotFoundError( "Manager {} does not support the Reset action".format( manager["Id"] ) )
     if "#Manager.Reset" not in manager.dict["Actions"]:
-        raise RedfishManagerResetNotFoundError( "Manager does not support Reset" )
+        raise RedfishManagerResetNotFoundError( "Manager {} does not support the Reset action".format( manager["Id"] ) )
 
-    # Extract the info about the SimpleUpdate action
+    # Extract the info about the Reset action
     reset_action = manager.dict["Actions"]["#Manager.Reset"]
     reset_uri = reset_action["target"]
 
     if "@Redfish.ActionInfo" not in reset_action:
-        # No Action Info; need to build this manually based on other annotations
+        # No action info; need to build this manually based on other annotations
 
         # Default parameter requirements
         reset_parameters = [
             {
                 "Name": "ResetType",
                 "Required": False,
                 "DataType": "String",
@@ -151,15 +159,15 @@
         ]
 
         # Get the AllowableValues from annotations
         for param in reset_parameters:
             if param["Name"] + "@Redfish.AllowableValues" in reset_action:
                 param["AllowableValues"] = reset_action[param["Name"] + "@Redfish.AllowableValues"]
     else:
-        # Get the Action Info and its parameter listing
+        # Get the action info and its parameter listing
         action_info = context.get( reset_action["@Redfish.ActionInfo"] )
         reset_parameters = action_info.dict["Parameters"]
 
     return reset_uri, reset_parameters
 
 def manager_reset( context, manager_id = None, reset_type = None ):
     """
@@ -196,15 +204,128 @@
 
     payload = {}
     if reset_type is not None:
         payload["ResetType"] = reset_type
 
     # Reset the manager
     response = context.post( reset_uri, body = payload )
-    verify_response( response )
+    try:
+        verify_response( response )
+    except Exception as e:
+        additional_message = ""
+        if response.status == 400:
+            # Append the list of valid reset types to 400 Bad Request responses
+            additional_message = "\nNo supported reset types listed"
+            for param in reset_parameters:
+                if param["Name"] == "ResetType" and "AllowableValues" in param:
+                    additional_message = "\nSupported reset types: {}".format( ", ".join( param["AllowableValues"] ) )
+        raise type( e )( str( e ) + additional_message ).with_traceback( sys.exc_info()[2] )
+    return response
+
+def get_manager_reset_to_defaults_info( context, manager_id = None, manager = None ):
+    """
+    Finds a manager matching the given ID and returns its reset-to-defaults info
+
+    Args:
+        context: The Redfish client object with an open session
+        manager_id: The manager to locate; if None, perform on the only manager
+        manager: Existing manager resource to inspect for reset info
+
+    Returns:
+        The URI of the Reset action
+        A list of parameter requirements from the action info
+    """
+
+    if manager is None:
+        manager = get_manager( context, manager_id )
+
+    # Check that there is a Reset action
+    if "Actions" not in manager.dict:
+        raise RedfishManagerResetToDefaultsNotFoundError( "Manager {} does not support the ResetToDefaults action".format( manager["Id"] ) )
+    if "#Manager.ResetToDefaults" not in manager.dict["Actions"]:
+        raise RedfishManagerResetToDefaultsNotFoundError( "Manager {} does not support the ResetToDefaults action".format( manager["Id"] ) )
+
+    # Extract the info about the ResetToDefaults action
+    reset_action = manager.dict["Actions"]["#Manager.ResetToDefaults"]
+    reset_uri = reset_action["target"]
+
+    if "@Redfish.ActionInfo" not in reset_action:
+        # No action info; need to build this manually based on other annotations
+
+        # Default parameter requirements
+        reset_parameters = [
+            {
+                "Name": "ResetType",
+                "Required": True,
+                "DataType": "String",
+                "AllowableValues": reset_to_defaults_types
+            }
+        ]
+
+        # Get the AllowableValues from annotations
+        for param in reset_parameters:
+            if param["Name"] + "@Redfish.AllowableValues" in reset_action:
+                param["AllowableValues"] = reset_action[param["Name"] + "@Redfish.AllowableValues"]
+    else:
+        # Get the action info and its parameter listing
+        action_info = context.get( reset_action["@Redfish.ActionInfo"] )
+        reset_parameters = action_info.dict["Parameters"]
+
+    return reset_uri, reset_parameters
+
+def manager_reset_to_defaults( context, manager_id = None, reset_type = None ):
+    """
+    Finds a manager matching the given ID and performs a reset-to-defaults
+
+    Args:
+        context: The Redfish client object with an open session
+        manager_id: The manager to locate; if None, perform on the only manager
+        reset_type: The type of reset to perform; if None, perform one of the common resets
+
+    Returns:
+        The response of the action
+    """
+
+    # Check that the values themselves are supported by the schema
+    reset_to_default_type_values = reset_to_defaults_types
+    if reset_type is not None:
+        if reset_type not in reset_to_default_type_values:
+            raise ValueError( "{} is not an allowable reset type ({})".format( reset_type, ", ".join( reset_to_default_type_values ) ) )
+
+    # Locate the reset action
+    reset_uri, reset_parameters = get_manager_reset_to_defaults_info( context, manager_id )
+
+    # Build the payload
+    if reset_type is None:
+        for param in reset_parameters:
+            if param["Name"] == "ResetType":
+                if "PreserveNetworkAndUsers" in param["AllowableValues"]:
+                    reset_type = "PreserveNetworkAndUsers"
+                elif "PreserveNetwork" in param["AllowableValues"]:
+                    reset_type = "PreserveNetwork"
+                elif "ResetAll" in param["AllowableValues"]:
+                    reset_type = "ResetAll"
+
+    payload = {}
+    if reset_type is not None:
+        payload["ResetType"] = reset_type
+
+    # Reset the manager to defaults
+    response = context.post( reset_uri, body = payload )
+    try:
+        verify_response( response )
+    except Exception as e:
+        additional_message = ""
+        if response.status == 400:
+            # Append the list of valid reset types to 400 Bad Request responses
+            additional_message = "\nNo supported reset types listed"
+            for param in reset_parameters:
+                if param["Name"] == "ResetType" and "AllowableValues" in param:
+                    additional_message = "\nSupported reset types: {}".format( ", ".join( param["AllowableValues"] ) )
+        raise type( e )( str( e ) + additional_message ).with_traceback( sys.exc_info()[2] )
     return response
 
 def get_manager_ethernet_interface_ids( context, manager_id = None ):
     """
     Finds the Ethernet interface collection for a manager and returns all of the member's identifiers
 
     Args:
```

### Comparing `redfish_utilities-3.1.4/redfish_utilities/messages.py` & `redfish_utilities-3.1.5/redfish_utilities/messages.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/redfish_utilities/sensors.py` & `redfish_utilities-3.1.5/redfish_utilities/sensors.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/redfish_utilities/systems.py` & `redfish_utilities-3.1.5/redfish_utilities/systems.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/redfish_utilities/tasks.py` & `redfish_utilities-3.1.5/redfish_utilities/tasks.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/redfish_utilities/update.py` & `redfish_utilities-3.1.5/redfish_utilities/update.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/redfish_utilities.egg-info/PKG-INFO` & `redfish_utilities-3.1.5/redfish_utilities.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish-utilities
-Version: 3.1.4
+Version: 3.1.5
 Summary: Redfish Utilities
 Home-page: https://github.com/DMTF/Redfish-Tacklebox
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -264,19 +264,20 @@
 usage: rf_manager_config.py [-h] --user USER --password PASSWORD --rhost RHOST
                             [--manager MANAGER]
                             {info,reset,getnet,setnet} ...
 
 A tool to manage managers in a service
 
 positional arguments:
-  {info,reset,getnet,setnet}
+  {info,reset,getnet,setnet,resettodefaults}
     info                Displays information about a manager
     reset               Resets a manager
     getnet              Displays information about an Ethernet interface
     setnet              Configures an Ethernet interface
+    resettodefaults     Resets a manager to default setting
 
 required arguments:
   --user USER, -u USER  The user name for authentication
   --password PASSWORD, -p PASSWORD
                         The password for authentication
   --rhost RHOST, -r RHOST
                         The address of the Redfish service (with scheme)
@@ -313,15 +314,14 @@
                                   [--info]
 
 optional arguments:
   -h, --help            show this help message and exit
   --type {On,ForceOff,GracefulShutdown,GracefulRestart,ForceRestart,Nmi,ForceOn,PushPowerButton,PowerCycle}, -t {On,ForceOff,GracefulShutdown,GracefulRestart,ForceRestart,Nmi,ForceOn,PushPowerButton,PowerCycle}
                         The type of power/reset operation to perform
   --info, -info         Indicates if reset information should be reported
-
 ```
 
 Example: `rf_manager_config.py -u root -p root -r https://192.168.1.100 reset -t GracefulRestart`
 
 The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
 It then traverses the manager collection for the service to find the matching system specified by the *manager* argument.
 It will perform the `Reset` action with the specified reset type from the *type* argument.
@@ -352,15 +352,15 @@
 ```
 usage: rf_manager_config.py setnet [-h] [--id ID] [--ipv4address IPV4ADDRESS]
                                    [--ipv4netmask IPV4NETMASK]
                                    [--ipv4gateway IPV4GATEWAY]
                                    [--dhcpv4 {On,Off}]
                                    [--ipv6addresses IPV6ADDRESSES [IPV6ADDRESSES ...]]
                                    [--ipv6gateways IPV6GATEWAYS [IPV6GATEWAYS ...]]
-                                   [--dhcpv6 {Stateful,Stateless,Disabled}]
+                                   [--dhcpv6 {Stateful,Stateless,Disabled,Enabled}]
                                    [--vlan {On,Off}] [--vlanid VLANID]
                                    [--vlanpriority VLANPRIORITY]
 
 optional arguments:
   -h, --help            show this help message and exit
   --id ID, -i ID        The identifier of the Ethernet interface to configure
   --ipv4address IPV4ADDRESS, -ipv4address IPV4ADDRESS
@@ -372,15 +372,15 @@
   --dhcpv4 {On,Off}, -dhcpv4 {On,Off}
                         The DHCPv4 configuration to set
   --ipv6addresses IPV6ADDRESSES [IPV6ADDRESSES ...], -ipv6addresses IPV6ADDRESSES [IPV6ADDRESSES ...]
                         The static IPv6 addresses to set with prefix length
   --ipv6gateways IPV6GATEWAYS [IPV6GATEWAYS ...], -ipv6gateways IPV6GATEWAYS [IPV6GATEWAYS ...]
                         The static IPv6 default gateways to set with prefix
                         length
-  --dhcpv6 {Stateful,Stateless,Disabled}, -dhcpv6 {Stateful,Stateless,Disabled}
+  --dhcpv6 {Stateful,Stateless,Disabled,Enabled}, -dhcpv6 {Stateful,Stateless,Disabled,Enabled}
                         The DHCPv6 configuration to set
   --vlan {On,Off}, -vlan {On,Off}
                         The VLAN enabled configuration to set
   --vlanid VLANID, -vlanid VLANID
                         The VLAN ID to set
   --vlanpriority VLANPRIORITY, -vlanpriority VLANPRIORITY
                         The VLAN priority to set
@@ -390,14 +390,38 @@
 
 The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
 It will then locate the manager specified by the *manager* argument, locate the Ethernet interface specified by the *id* argument, and apply the requested settings to the interface.
 * If *manager* is not specified, and if the service has exactly one manager, it will perform the operation on the one manager.
 * If *id* is not specified, and if the manager has exactly one Ethernet interface, it will perform the operation on the one interface.
 
 
+#### Reset to Defaults
+
+```
+usage: rf_manager_config.py resettodefaults [-h]
+                                            [--type {ResetAll,PreserveNetworkAndUsers,PreserveNetwork}]
+                                            [--info]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --type {ResetAll,PreserveNetworkAndUsers,PreserveNetwork}, -t {ResetAll,PreserveNetworkAndUsers,PreserveNetwork}
+                        The type of reset-to-defaults operation to perform
+  --info, -info         Indicates if reset-to-defaults information should be
+                        reported
+```
+
+Example: `rf_manager_config.py -u root -p root -r https://192.168.1.100 resettodefaults -t ResetAll`
+
+The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
+It then traverses the manager collection for the service to find the matching system specified by the *manager* argument.
+It will perform the `ResetToDefaults` action with the specified reset type from the *type* argument.
+* If *manager* is not specified, and if the service has exactly one manager, it will perform the operation on the one manager.
+* If *type* is not specified, it will attempt to perform the action with `PreserveNetworkAndUsers`.
+
+
 ### BIOS Settings
 
 ```
 usage: rf_bios_settings.py [-h] --user USER --password PASSWORD --rhost RHOST
                            [--system SYSTEM] [--attribute name value]
 
 A tool to manager BIOS settings for a system
@@ -720,14 +744,103 @@
 Example: `rf_virtual_media.py -u root -p root -r https://192.168.1.100 eject --id 1`
 
 The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
 It will then locate the system specified by the *system* argument, find its virtual media collection.
 It will then locate the virtual media instance with matching `Id` property with the *id* argument, and then eject the media.
 
 
+### Licenses
+
+```
+usage: rf_licenses.py [-h] --user USER --password PASSWORD --rhost RHOST
+                      [--debug]
+                      {info,install,delete} ...
+
+A tool to manage licenses on a Redfish service
+
+positional arguments:
+  {info,install,delete}
+    info                Displays information about the licenses installed on
+                        the service
+    install             Installs a new license
+    delete              Deletes a license
+
+required arguments:
+  --user USER, -u USER  The user name for authentication
+  --password PASSWORD, -p PASSWORD
+                        The password for authentication
+  --rhost RHOST, -r RHOST
+                        The address of the Redfish service (with scheme)
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --debug               Creates debug file showing HTTP traces and exceptions
+```
+
+
+#### Info
+
+```
+usage: rf_licenses.py info [-h] [--details]
+
+options:
+  -h, --help           show this help message and exit
+  --details, -details  Indicates if the full details of each license should be
+                       shown
+```
+
+Example: `rf_licenses.py -u root -p root -r https://192.168.1.100 info`
+
+The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
+It will then locate the license service, find its license collection, and display the licenses.
+
+
+#### Install
+
+```
+usage: rf_licenses.py install [-h] --license LICENSE
+
+required arguments:
+  --license LICENSE, -l LICENSE
+                        The filepath or URI to the license to install
+
+optional arguments:
+  -h, --help            show this help message and exit
+``` 
+
+Example: `rf_licenses.py -u root -p root -r https://192.168.1.100 install --license /home/user/my_license.xml`
+
+The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
+It will then locate the license service.
+If the license referenced by the *license* argument is local file, it will insert the contents of the license file in the license collection.
+Otherwise, it will install the new license with the `Install` action found on the license service.
+
+
+#### Delete
+
+```
+usage: rf_licenses.py delete [-h] --license LICENSE
+
+options:
+
+required arguments:
+  --license LICENSE, -l LICENSE
+                        The identifier of the license to delete
+
+optional arguments:
+  -h, --help            show this help message and exit
+```
+
+Example: `rf_licenses.py -u root -p root -r https://192.168.1.100 delete --license 1`
+
+The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
+It will then locate the license service and find the license requested by the *license* argument.
+If the matching license is found, it will delete the license.
+
+
 ### Diagnostic Data
 
 ```
 usage: rf_diagnostic_data.py [-h] --user USER --password PASSWORD --rhost
                              RHOST [--manager [MANAGER]] [--system [SYSTEM]]
                              [--chassis [CHASSIS]] [--log LOG]
                              [--type {Manager,PreOS,OS,OEM}]
```

### Comparing `redfish_utilities-3.1.4/redfish_utilities.egg-info/SOURCES.txt` & `redfish_utilities-3.1.5/redfish_utilities.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 redfish_utilities/__init__.py
 redfish_utilities/accounts.py
 redfish_utilities/collections.py
 redfish_utilities/config.py
 redfish_utilities/event_service.py
 redfish_utilities/inventory.py
+redfish_utilities/licenses.py
 redfish_utilities/logs.py
 redfish_utilities/managers.py
 redfish_utilities/messages.py
 redfish_utilities/resets.py
 redfish_utilities/sensors.py
 redfish_utilities/systems.py
 redfish_utilities/tasks.py
@@ -23,14 +24,15 @@
 redfish_utilities.egg-info/top_level.txt
 scripts/rf_accounts.py
 scripts/rf_bios_settings.py
 scripts/rf_boot_override.py
 scripts/rf_diagnostic_data.py
 scripts/rf_discover.py
 scripts/rf_event_service.py
+scripts/rf_licenses.py
 scripts/rf_logs.py
 scripts/rf_manager_config.py
 scripts/rf_power_reset.py
 scripts/rf_raw_request.py
 scripts/rf_sensor_list.py
 scripts/rf_sys_inventory.py
 scripts/rf_update.py
```

### Comparing `redfish_utilities-3.1.4/scripts/rf_accounts.py` & `redfish_utilities-3.1.5/scripts/rf_accounts.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/scripts/rf_bios_settings.py` & `redfish_utilities-3.1.5/scripts/rf_bios_settings.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/scripts/rf_boot_override.py` & `redfish_utilities-3.1.5/scripts/rf_boot_override.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/scripts/rf_diagnostic_data.py` & `redfish_utilities-3.1.5/scripts/rf_diagnostic_data.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/scripts/rf_discover.py` & `redfish_utilities-3.1.5/scripts/rf_discover.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/scripts/rf_event_service.py` & `redfish_utilities-3.1.5/scripts/rf_event_service.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/scripts/rf_logs.py` & `redfish_utilities-3.1.5/scripts/rf_logs.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/scripts/rf_manager_config.py` & `redfish_utilities-3.1.5/scripts/rf_manager_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,18 +36,21 @@
 setnet_argget.add_argument( "--id", "-i", type = str, help = "The identifier of the Ethernet interface to configure" )
 setnet_argget.add_argument( "--ipv4address", "-ipv4address", type = str, help = "The static IPv4 address to set" )
 setnet_argget.add_argument( "--ipv4netmask", "-ipv4netmask", type = str, help = "The static IPv4 subnet mask to set" )
 setnet_argget.add_argument( "--ipv4gateway", "-ipv4gateway", type = str, help = "The static IPv4 gateway to set" )
 setnet_argget.add_argument( "--dhcpv4", "-dhcpv4", type = str, help = "The DHCPv4 configuration to set", choices = [ "On", "Off" ] )
 setnet_argget.add_argument( "--ipv6addresses", "-ipv6addresses", type = str, nargs = '+', help = "The static IPv6 addresses to set with prefix length" )
 setnet_argget.add_argument( "--ipv6gateways", "-ipv6gateways", type = str, nargs = '+', help = "The static IPv6 default gateways to set with prefix length" )
-setnet_argget.add_argument( "--dhcpv6", "-dhcpv6", type = str, help = "The DHCPv6 configuration to set", choices = [ "Stateful", "Stateless", "Disabled" ] )
+setnet_argget.add_argument( "--dhcpv6", "-dhcpv6", type = str, help = "The DHCPv6 configuration to set", choices = [ "Stateful", "Stateless", "Disabled", "Enabled" ] )
 setnet_argget.add_argument( "--vlan", "-vlan", type = str, help = "The VLAN enabled configuration to set", choices = [ "On", "Off" ] )
 setnet_argget.add_argument( "--vlanid", "-vlanid", type = int, help = "The VLAN ID to set" )
 setnet_argget.add_argument( "--vlanpriority", "-vlanpriority", type = int, help = "The VLAN priority to set" )
+reset_to_defaults_argget = subparsers.add_parser( "resettodefaults", help = "Resets a manager to default settings" )
+reset_to_defaults_argget.add_argument( "--type", "-t", type = str, help = "The type of reset-to-defaults operation to perform", choices = redfish_utilities.reset_to_defaults_types )
+reset_to_defaults_argget.add_argument( "--info", "-info", action = "store_true", help = "Indicates if reset-to-defaults information should be reported" )
 args = argget.parse_args()
 
 if args.debug:
     log_file = "rf_manager_config-{}.log".format( datetime.datetime.now().strftime( "%Y-%m-%d-%H%M%S" ) )
     log_format = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
     logger = redfish.redfish_logger( log_file, log_format, logging.DEBUG )
     logger.info( "rf_manager_config Trace" )
@@ -69,14 +72,29 @@
             if not printed_reset_types:
                 print( "No reset information found" )
         else:
             print( "Resetting the manager..." )
             response = redfish_utilities.manager_reset( redfish_obj, args.manager, args.type )
             response = redfish_utilities.poll_task_monitor( redfish_obj, response )
             redfish_utilities.verify_response( response )
+    elif args.command == "resettodefaults":
+        if args.info:
+            reset_uri, reset_parameters = redfish_utilities.get_manager_reset_to_defaults_info( redfish_obj, args.manager )
+            printed_reset_types = False
+            for param in reset_parameters:
+                if param["Name"] == "ResetType" and "AllowableValues" in param:
+                    print( "Supported reset types: {}".format( ", ".join( param["AllowableValues"] ) ) )
+                    printed_reset_types = True
+            if not printed_reset_types:
+                print( "No reset information found" )
+        else:
+            print( "Resetting the manager to defaults..." )
+            response = redfish_utilities.manager_reset_to_defaults( redfish_obj, args.manager, args.type )
+            response = redfish_utilities.poll_task_monitor( redfish_obj, response )
+            redfish_utilities.verify_response( response )
     elif args.command == "getnet":
         interface = redfish_utilities.get_manager_ethernet_interface( redfish_obj, args.manager, args.id )
         redfish_utilities.print_manager_ethernet_interface( interface )
     elif args.command == "setnet":
         vlan = {}
         if args.vlan == "On":
             vlan["VLANEnable"] = True
```

### Comparing `redfish_utilities-3.1.4/scripts/rf_power_reset.py` & `redfish_utilities-3.1.5/scripts/rf_power_reset.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/scripts/rf_raw_request.py` & `redfish_utilities-3.1.5/scripts/rf_raw_request.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/scripts/rf_sensor_list.py` & `redfish_utilities-3.1.5/scripts/rf_sensor_list.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/scripts/rf_sys_inventory.py` & `redfish_utilities-3.1.5/scripts/rf_sys_inventory.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/scripts/rf_update.py` & `redfish_utilities-3.1.5/scripts/rf_update.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/scripts/rf_virtual_media.py` & `redfish_utilities-3.1.5/scripts/rf_virtual_media.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.4/setup.py` & `redfish_utilities-3.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from codecs import open
 
 with open( "README.md", "r", "utf-8" ) as f:
     long_description = f.read()
 
 setup(
     name = "redfish_utilities",
-    version = "3.1.4",
+    version = "3.1.5",
     description = "Redfish Utilities",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     author = "DMTF, https://www.dmtf.org/standards/feedback",
     license = "BSD 3-clause \"New\" or \"Revised License\"",
     classifiers = [
         "Development Status :: 5 - Production/Stable",
@@ -29,14 +29,15 @@
     scripts = [
         "scripts/rf_accounts.py",
         "scripts/rf_bios_settings.py",
         "scripts/rf_boot_override.py",
         "scripts/rf_diagnostic_data.py",
         "scripts/rf_discover.py",
         "scripts/rf_event_service.py",
+        "scripts/rf_licenses.py",
         "scripts/rf_logs.py",
         "scripts/rf_manager_config.py",
         "scripts/rf_power_reset.py",
         "scripts/rf_raw_request.py",
         "scripts/rf_sensor_list.py",
         "scripts/rf_sys_inventory.py",
         "scripts/rf_update.py",
```

