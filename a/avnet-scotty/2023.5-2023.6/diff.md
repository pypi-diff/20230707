# Comparing `tmp/avnet-scotty-2023.5.tar.gz` & `tmp/avnet-scotty-2023.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avnet-scotty-2023.5.tar", last modified: Thu Jun  1 13:07:20 2023, max compression
+gzip compressed data, was "avnet-scotty-2023.6.tar", last modified: Fri Jul  7 06:38:04 2023, max compression
```

## Comparing `avnet-scotty-2023.5.tar` & `avnet-scotty-2023.6.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:07:20.484009 avnet-scotty-2023.5/
--rw-r--r--   0 root         (0) root         (0)    32879 2023-06-01 13:07:12.000000 avnet-scotty-2023.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)    19899 2023-06-01 13:07:20.484009 avnet-scotty-2023.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    19601 2023-06-01 13:07:12.000000 avnet-scotty-2023.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:07:20.484009 avnet-scotty-2023.5/avnet_scotty.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19899 2023-06-01 13:07:20.000000 avnet-scotty-2023.5/avnet_scotty.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      356 2023-06-01 13:07:20.000000 avnet-scotty-2023.5/avnet_scotty.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 13:07:20.000000 avnet-scotty-2023.5/avnet_scotty.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-01 13:07:20.000000 avnet-scotty-2023.5/avnet_scotty.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-06-01 13:07:20.000000 avnet-scotty-2023.5/avnet_scotty.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-01 13:07:20.000000 avnet-scotty-2023.5/avnet_scotty.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:07:20.484009 avnet-scotty-2023.5/bumper/
--rw-r--r--   0 root         (0) root         (0)      110 2023-06-01 13:07:12.000000 avnet-scotty-2023.5/bumper/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4006 2023-06-01 13:07:12.000000 avnet-scotty-2023.5/bumper/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     6713 2023-06-01 13:07:12.000000 avnet-scotty-2023.5/scotty
--rwxr-xr-x   0 root         (0) root         (0)     1637 2023-06-01 13:07:12.000000 avnet-scotty-2023.5/scotty-runqemu
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:07:20.484009 avnet-scotty-2023.5/scripts/
--rwxr-xr-x   0 root         (0) root         (0)      811 2023-06-01 13:07:12.000000 avnet-scotty-2023.5/scripts/vm_bundle.sh
--rw-r--r--   0 root         (0) root         (0)     1137 2023-06-01 13:07:12.000000 avnet-scotty-2023.5/scripts/vm_create.sh.template
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 13:07:20.484009 avnet-scotty-2023.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1144 2023-06-01 13:07:12.000000 avnet-scotty-2023.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:38:04.233218 avnet-scotty-2023.6/
+-rw-r--r--   0 root         (0) root         (0)    32879 2023-07-07 06:37:53.000000 avnet-scotty-2023.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    20288 2023-07-07 06:38:04.233218 avnet-scotty-2023.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    19990 2023-07-07 06:37:53.000000 avnet-scotty-2023.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:38:04.229218 avnet-scotty-2023.6/avnet_scotty.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    20288 2023-07-07 06:38:04.000000 avnet-scotty-2023.6/avnet_scotty.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      380 2023-07-07 06:38:04.000000 avnet-scotty-2023.6/avnet_scotty.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 06:38:04.000000 avnet-scotty-2023.6/avnet_scotty.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-07 06:38:04.000000 avnet-scotty-2023.6/avnet_scotty.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-07 06:38:04.000000 avnet-scotty-2023.6/avnet_scotty.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-07 06:38:04.000000 avnet-scotty-2023.6/avnet_scotty.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:38:04.229218 avnet-scotty-2023.6/bumper/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-07 06:37:53.000000 avnet-scotty-2023.6/bumper/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4006 2023-07-07 06:37:53.000000 avnet-scotty-2023.6/bumper/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6719 2023-07-07 06:37:53.000000 avnet-scotty-2023.6/scotty
+-rwxr-xr-x   0 root         (0) root         (0)     1637 2023-07-07 06:37:53.000000 avnet-scotty-2023.6/scotty-runqemu
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:38:04.229218 avnet-scotty-2023.6/scotty_test/
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-07-07 06:37:53.000000 avnet-scotty-2023.6/scotty_test/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:38:04.233218 avnet-scotty-2023.6/scripts/
+-rwxr-xr-x   0 root         (0) root         (0)      811 2023-07-07 06:37:53.000000 avnet-scotty-2023.6/scripts/vm_bundle.sh
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-07-07 06:37:53.000000 avnet-scotty-2023.6/scripts/vm_create.sh.template
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 06:38:04.233218 avnet-scotty-2023.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-07-07 06:37:53.000000 avnet-scotty-2023.6/setup.py
```

### Comparing `avnet-scotty-2023.5/LICENSE` & `avnet-scotty-2023.6/LICENSE`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.5/PKG-INFO` & `avnet-scotty-2023.6/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: avnet-scotty
-Version: 2023.5
-Summary: scotty: S(imple)C(ore) O(pen) T(echnology) T(ool for) Y(ou)
-Home-page: https://github.com/avnet-embedded/simplecore-tools
-Author: Avnet Embedded GmbH
-License: GPL-3.0-only
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 ***************
 The Scotty tool
 ***************
 
 Scotty
 ======
 
@@ -467,15 +457,18 @@
 | Key               | Type   | Description                                    | Example                                         |
 +===================+========+================================================+=================================================+
 | description       | string | Human readable description                     | description: "My feature"                       |
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
 | menu_priority     | int    | Defines the order in the menu                  | menu_priority: 100                              |
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
 | layers            | list   | Paths to layers to be used                     | layers:                                         |
-|                   |        |                                                |    ? "meta-myfeature"                           | 
+|                   |        |                                                |    ? "meta-myfeature"                           |
++-------------------+--------+------------------------------------------------+-------------------------------------------------+
+| extraconf         | list   | Extra configuration variables for local.conf   | extraconf:                                      |
+|                   |        |                                                |    ? "INHERIT += 'myclass'"                     |
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
 | supported_distros | dict   | key/value table of DISTRO name and description | supported_distros: &distros_myfeature           |
 |                   |        |                                                |    <<: [\*distros_poky]                         |
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
 | add-overlays      | object | Additional selectable overlays of the feature  | add-overlays:                                   |
 |                   |        |   see `overlays section` for details           |    overlays:                                    |
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
```

### Comparing `avnet-scotty-2023.5/README.rst` & `avnet-scotty-2023.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: avnet-scotty
+Version: 2023.6
+Summary: scotty: S(imple)C(ore) O(pen) T(echnology) T(ool for) Y(ou)
+Home-page: https://github.com/avnet-embedded/simplecore-tools
+Author: Avnet Embedded GmbH
+License: GPL-3.0-only
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 ***************
 The Scotty tool
 ***************
 
 Scotty
 ======
 
@@ -457,15 +467,18 @@
 | Key               | Type   | Description                                    | Example                                         |
 +===================+========+================================================+=================================================+
 | description       | string | Human readable description                     | description: "My feature"                       |
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
 | menu_priority     | int    | Defines the order in the menu                  | menu_priority: 100                              |
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
 | layers            | list   | Paths to layers to be used                     | layers:                                         |
-|                   |        |                                                |    ? "meta-myfeature"                           | 
+|                   |        |                                                |    ? "meta-myfeature"                           |
++-------------------+--------+------------------------------------------------+-------------------------------------------------+
+| extraconf         | list   | Extra configuration variables for local.conf   | extraconf:                                      |
+|                   |        |                                                |    ? "INHERIT += 'myclass'"                     |
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
 | supported_distros | dict   | key/value table of DISTRO name and description | supported_distros: &distros_myfeature           |
 |                   |        |                                                |    <<: [\*distros_poky]                         |
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
 | add-overlays      | object | Additional selectable overlays of the feature  | add-overlays:                                   |
 |                   |        |   see `overlays section` for details           |    overlays:                                    |
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
```

### Comparing `avnet-scotty-2023.5/avnet_scotty.egg-info/PKG-INFO` & `avnet-scotty-2023.6/avnet_scotty.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avnet-scotty
-Version: 2023.5
+Version: 2023.6
 Summary: scotty: S(imple)C(ore) O(pen) T(echnology) T(ool for) Y(ou)
 Home-page: https://github.com/avnet-embedded/simplecore-tools
 Author: Avnet Embedded GmbH
 License: GPL-3.0-only
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -467,15 +467,18 @@
 | Key               | Type   | Description                                    | Example                                         |
 +===================+========+================================================+=================================================+
 | description       | string | Human readable description                     | description: "My feature"                       |
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
 | menu_priority     | int    | Defines the order in the menu                  | menu_priority: 100                              |
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
 | layers            | list   | Paths to layers to be used                     | layers:                                         |
-|                   |        |                                                |    ? "meta-myfeature"                           | 
+|                   |        |                                                |    ? "meta-myfeature"                           |
++-------------------+--------+------------------------------------------------+-------------------------------------------------+
+| extraconf         | list   | Extra configuration variables for local.conf   | extraconf:                                      |
+|                   |        |                                                |    ? "INHERIT += 'myclass'"                     |
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
 | supported_distros | dict   | key/value table of DISTRO name and description | supported_distros: &distros_myfeature           |
 |                   |        |                                                |    <<: [\*distros_poky]                         |
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
 | add-overlays      | object | Additional selectable overlays of the feature  | add-overlays:                                   |
 |                   |        |   see `overlays section` for details           |    overlays:                                    |
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
```

### Comparing `avnet-scotty-2023.5/bumper/__main__.py` & `avnet-scotty-2023.6/bumper/__main__.py`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.5/scotty` & `avnet-scotty-2023.6/scotty`

 * *Files 2% similar despite different names*

```diff
@@ -29,20 +29,20 @@
 	TERM \
 	UBOOT_ENV_VARS \
 	"
 # SCOTTY_FEATURES_LAYERS REPO_URL SCOTTY_MACHINE_DIR BUILDDIR
 declare -r scotty_whitelist=${SCOTTY_WHITELIST:-${scotty_whitelist_default}}
 
 if [ "${SCOTTY_DOCKER_IMAGE:-1}" == "1" ]; then
-    declare -r docker_default_image="ghcr.io/avnet-embedded/scotty:2023.5"
+    declare -r docker_default_image="ghcr.io/avnet-embedded/scotty:2023.6"
 else
     declare -r docker_default_image="${SCOTTY_DOCKER_IMAGE}"
 fi
 
-export SCOTTY_DEFAULT_MANIFEST_BRANCH="refs/tags/2023.5"
+export SCOTTY_DEFAULT_MANIFEST_BRANCH="refs/tags/2023.6"
 export SCOTTY_DEFAULT_MANIFEST_NAME="default-release.xml"
 
 debug() {
 	if [ "${SCOTTY_DEBUG:-0}" == "1" ]; then
 		echo -e "\033[1;38m${*}\033[0m"
 	fi
 }
@@ -84,19 +84,19 @@
 	touch "${SCOTTY_HOME}/bash_history"
 
 	# Set docker parameters
 	read -ra docker_args <<< "${DOCKER_EXTRA_ARGS:-}"
 	docker_args+=(--env "uid=$(id --user)")
 	docker_args+=(--env "gid=$(id --group)")
 	docker_args+=(--env "kvm_gid=$(getent group kvm | cut -d: -f3)")
-	if [ -n "${SIMPLESWITCH_REGISTRY_USERNAME:-}" ]; then
-		docker_args+=(--env "SIMPLESWITCH_REGISTRY_USERNAME=${SIMPLESWITCH_REGISTRY_USERNAME}")
+	if [ -n "${_SIMPLESWITCH_REGISTRY_USERNAME:-}" ]; then
+		docker_args+=(--env "_SIMPLESWITCH_REGISTRY_USERNAME=${_SIMPLESWITCH_REGISTRY_USERNAME}")
 	fi
-	if [ -n "${SIMPLESWITCH_REGISTRY_PAT:-}" ]; then
-		docker_args+=(--env "SIMPLESWITCH_REGISTRY_PAT=${SIMPLESWITCH_REGISTRY_PAT}")
+	if [ -n "${_SIMPLESWITCH_REGISTRY_PAT:-}" ]; then
+		docker_args+=(--env "_SIMPLESWITCH_REGISTRY_PAT=${_SIMPLESWITCH_REGISTRY_PAT}")
 	fi
 	docker_args+=(--volume "${outdir}:${outdir}")
 	if [ -n "${SCOTTY_DOCKER_EXTRA_VOLUME:-}" ]; then
     while read -r -d ',' volume
       do
         docker_args+=(--volume "${volume}:${volume}")
       done <<< "${SCOTTY_DOCKER_EXTRA_VOLUME},"
```

### Comparing `avnet-scotty-2023.5/scotty-runqemu` & `avnet-scotty-2023.6/scotty-runqemu`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.5/scripts/vm_bundle.sh` & `avnet-scotty-2023.6/scripts/vm_bundle.sh`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.5/scripts/vm_create.sh.template` & `avnet-scotty-2023.6/scripts/vm_create.sh.template`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.5/setup.py` & `avnet-scotty-2023.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,31 +3,33 @@
 # noqa: D100
 
 import setuptools
 import os
 
 _version = os.environ.get('SCOTTY_VERSION', '0.0.1')
 
+requirements = []
+with open('requirements.txt') as f:
+    requirements = f.read().splitlines()
+
 setuptools.setup(
     author='Avnet Embedded GmbH',
     description='scotty: S(imple)C(ore) O(pen) T(echnology) T(ool for) Y(ou)',
     long_description=open('README.rst', 'r').read(),
     long_description_content_type='text/x-rst',
     license='GPL-3.0-only',
     license_files=('LICENSE',),
     entry_points={
         'console_scripts': [
             'bumper = bumper.__main__:main',
             'scotty-test = scotty_test.__main__:main',
         ],
     },
-    packages=['bumper'],
-    install_requires=['GitPython ~= 3.1',
-                      'azure-storage-blob ~= 12.16',
-                      'inquirer ~= 3.0'],
+    packages=['bumper', 'scotty_test'],
+    install_requires=requirements,
     # As scotty is already in use on PyPi our package is called
     # avnet-scotty
     name='avnet-scotty',
     scripts=[
         'scotty',
         'scotty-runqemu',
         'scripts/vm_bundle.sh',
```

