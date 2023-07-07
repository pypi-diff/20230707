# Comparing `tmp/os_vif-3.1.1.tar.gz` & `tmp/os_vif-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os_vif-3.1.1.tar", last modified: Fri Feb 10 16:30:29 2023, max compression
+gzip compressed data, was "os_vif-3.2.0.tar", last modified: Fri Jul  7 14:34:40 2023, max compression
```

## Comparing `os_vif-3.1.1.tar` & `os_vif-3.2.0.tar`

### file list

```diff
@@ -1,219 +1,221 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.488906 os_vif-3.1.1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-02-10 16:29:59.000000 os_vif-3.1.1/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-02-10 16:29:59.000000 os_vif-3.1.1/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2023-02-10 16:29:59.000000 os_vif-3.1.1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5723 2023-02-10 16:29:59.000000 os_vif-3.1.1/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3132 2023-02-10 16:30:29.000000 os_vif-3.1.1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      599 2023-02-10 16:29:59.000000 os_vif-3.1.1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13231 2023-02-10 16:30:29.000000 os_vif-3.1.1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-10 16:29:59.000000 os_vif-3.1.1/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-02-10 16:29:59.000000 os_vif-3.1.1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2029 2023-02-10 16:30:29.488906 os_vif-3.1.1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      843 2023-02-10 16:29:59.000000 os_vif-3.1.1/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2023-02-10 16:29:59.000000 os_vif-3.1.1/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.452905 os_vif-3.1.1/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-02-10 16:29:59.000000 os_vif-3.1.1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.452905 os_vif-3.1.1/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1760 2023-02-10 16:29:59.000000 os_vif-3.1.1/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.452905 os_vif-3.1.1/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2100 2023-02-10 16:29:59.000000 os_vif-3.1.1/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2023-02-10 16:29:59.000000 os_vif-3.1.1/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.452905 os_vif-3.1.1/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7078 2023-02-10 16:29:59.000000 os_vif-3.1.1/doc/source/reference/glossary.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.456905 os_vif-3.1.1/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2803 2023-02-10 16:29:59.000000 os_vif-3.1.1/doc/source/user/host-info.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.456905 os_vif-3.1.1/doc/source/user/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2023-02-10 16:29:59.000000 os_vif-3.1.1/doc/source/user/plugins/linux-bridge.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2023-02-10 16:29:59.000000 os_vif-3.1.1/doc/source/user/plugins/noop.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1907 2023-02-10 16:29:59.000000 os_vif-3.1.1/doc/source/user/plugins/ovs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2352 2023-02-10 16:29:59.000000 os_vif-3.1.1/doc/source/user/usage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2164 2023-02-10 16:29:59.000000 os_vif-3.1.1/doc/source/user/vif-types.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.456905 os_vif-3.1.1/os_vif/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5484 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3340 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1040 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.456905 os_vif-3.1.1/os_vif/internal/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/internal/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.460905 os_vif-3.1.1/os_vif/internal/ip/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/internal/ip/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/internal/ip/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2787 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/internal/ip/ip_command.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.460905 os_vif-3.1.1/os_vif/internal/ip/linux/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/internal/ip/linux/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5511 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/internal/ip/linux/impl_pyroute2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.460905 os_vif-3.1.1/os_vif/internal/ip/windows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/internal/ip/windows/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1745 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/internal/ip/windows/impl_netifaces.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.460905 os_vif-3.1.1/os_vif/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1139 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/objects/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1761 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/objects/fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1282 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/objects/fixed_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6698 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/objects/host_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1226 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/objects/instance_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2134 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/objects/network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1352 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/objects/route.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/objects/subnet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21668 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/objects/vif.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3032 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.460905 os_vif-3.1.1/os_vif/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.460905 os_vif-3.1.1/os_vif/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5005 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/functional/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.464905 os_vif-3.1.1/os_vif/tests/functional/internal/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/functional/internal/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.464905 os_vif-3.1.1/os_vif/tests/functional/internal/command/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/functional/internal/command/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.464905 os_vif-3.1.1/os_vif/tests/functional/internal/command/ip/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/functional/internal/command/ip/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9758 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/functional/internal/command/ip/test_impl_pyroute2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      844 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/functional/privsep.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.464905 os_vif-3.1.1/os_vif/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      795 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/unit/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.464905 os_vif-3.1.1/os_vif/tests/unit/internal/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/unit/internal/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.464905 os_vif-3.1.1/os_vif/tests/unit/internal/ip/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/unit/internal/ip/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.464905 os_vif-3.1.1/os_vif/tests/unit/internal/ip/linux/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/unit/internal/ip/linux/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7364 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/unit/internal/ip/linux/test_impl_pyroute2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1415 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/unit/internal/ip/test_api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.464905 os_vif-3.1.1/os_vif/tests/unit/internal/ip/windows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/unit/internal/ip/windows/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1992 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/unit/internal/ip/windows/test_impl_netifaces.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3137 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/unit/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1335 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/unit/test_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7576 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/unit/test_host_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3709 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/unit/test_objects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6609 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/unit/test_os_vif.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18000 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/tests/unit/test_vif.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2023-02-10 16:29:59.000000 os_vif-3.1.1/os_vif/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.456905 os_vif-3.1.1/os_vif.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2029 2023-02-10 16:30:29.000000 os_vif-3.1.1/os_vif.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6559 2023-02-10 16:30:29.000000 os_vif-3.1.1/os_vif.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-10 16:30:29.000000 os_vif-3.1.1/os_vif.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2023-02-10 16:30:29.000000 os_vif-3.1.1/os_vif.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-10 16:30:29.000000 os_vif-3.1.1/os_vif.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-10 16:30:29.000000 os_vif-3.1.1/os_vif.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2023-02-10 16:30:29.000000 os_vif-3.1.1/os_vif.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2023-02-10 16:30:29.000000 os_vif-3.1.1/os_vif.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.448905 os_vif-3.1.1/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.468905 os_vif-3.1.1/playbooks/openstack-tox-functional-ovs-with-sudo/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-02-10 16:29:59.000000 os_vif-3.1.1/playbooks/openstack-tox-functional-ovs-with-sudo/Debian.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-02-10 16:29:59.000000 os_vif-3.1.1/playbooks/openstack-tox-functional-ovs-with-sudo/Gentoo.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-02-10 16:29:59.000000 os_vif-3.1.1/playbooks/openstack-tox-functional-ovs-with-sudo/RedHat.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-02-10 16:29:59.000000 os_vif-3.1.1/playbooks/openstack-tox-functional-ovs-with-sudo/Suse.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      566 2023-02-10 16:29:59.000000 os_vif-3.1.1/playbooks/openstack-tox-functional-ovs-with-sudo/pre.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.448905 os_vif-3.1.1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.472905 os_vif-3.1.1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/OVSVif-hybrid-unplug-f37bf57bc8e913de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/add-abstract-ovsdb-api-8f04df58d4ed5b73.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/add-fast-path-vhostuser-support-fe87e558326909b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/add-no-op-plugin-763a6703e7328a24.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/add-ovs-representor-portprofile-5f8290e5a40bf0a4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/add-ovs-vhostuser-support-2ba8de51c1f3a244.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/add-ovsdb-native-322fffb49c91503d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2079 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/always-plug-vifs-for-ovs-1d033fc49a9c6c4e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/brctl-removal-a5b0e69b865afa57.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/bug-1892132-812e6d5ce0588ebb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/contextlib-and-nested-with-statements-2747a9ebb9a5bfd7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      711 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/default-to-native-ovsdb-driver-112fb5adf6e19a30.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/do-not-force-mac-ageing-c6e8d750130c5740.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/drop-py36-support-0e9b07073f6ad73f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/drop-python2-support-7a4bc7d31253c1e5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/ensure-ovs-bridge-a0c1b51f469c92d0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/extend-vhostuser-object-fada14a1457d4e56.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/fix-ovs-plugin-describe-049750609559f1ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/fix-stevedore-entrypoints-8002ec7a5166c977.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/fix-vif-openvswitch-fa0d19be9dd668e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/generic-datapath-offloads-41cabb6842b41533.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/initial-release-2c71d6bbf55f763b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/oslo-config-opts-entrypoints-e83f907b686d774a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1659 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/per-port-bridge-c6a50179a0256de3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/port-profile-info-linux-bridge-4800f5a0b7328615.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/port-profile-info-ovs-63b46a3eafc11de2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/prevent-lb-reply-arp-6459133bfb056069.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/remove_iptools_implementation-2eb866573a680e61.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      981 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/revert-always-plug-port-for-ovs-hybrid-plug-false-dc015985cbc5443b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/vhost-user-mtu-support-cbc7d02a6665fab1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/notes/vhost-user-reconnect-fa4cbb731b787f71.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.476905 os_vif-3.1.1/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.476905 os_vif-3.1.1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.476905 os_vif-3.1.1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1843 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-10 16:29:59.000000 os_vif-3.1.1/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2023-02-10 16:29:59.000000 os_vif-3.1.1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1143 2023-02-10 16:30:29.488906 os_vif-3.1.1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-02-10 16:29:59.000000 os_vif-3.1.1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2023-02-10 16:29:59.000000 os_vif-3.1.1/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2437 2023-02-10 16:29:59.000000 os_vif-3.1.1/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.480905 os_vif-3.1.1/vif_plug_linux_bridge/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_linux_bridge/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_linux_bridge/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20641 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_linux_bridge/iptables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4949 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_linux_bridge/linux_bridge.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9481 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_linux_bridge/linux_net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_linux_bridge/privsep.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.480905 os_vif-3.1.1/vif_plug_linux_bridge/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_linux_bridge/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.480905 os_vif-3.1.1/vif_plug_linux_bridge/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_linux_bridge/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6740 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_linux_bridge/tests/unit/test_linux_net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4803 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_linux_bridge/tests/unit/test_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.480905 os_vif-3.1.1/vif_plug_noop/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_noop/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1629 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_noop/noop.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.480905 os_vif-3.1.1/vif_plug_noop/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_noop/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.480905 os_vif-3.1.1/vif_plug_noop/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_noop/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1236 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_noop/tests/unit/test_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.484906 os_vif-3.1.1/vif_plug_ovs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_ovs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_ovs/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1328 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_ovs/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14289 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_ovs/linux_net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21217 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_ovs/ovs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.484906 os_vif-3.1.1/vif_plug_ovs/ovsdb/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_ovs/ovsdb/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1293 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_ovs/ovsdb/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3020 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_ovs/ovsdb/impl_idl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14437 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_ovs/ovsdb/impl_vsctl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8565 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_ovs/ovsdb/ovsdb_lib.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1100 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_ovs/privsep.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.484906 os_vif-3.1.1/vif_plug_ovs/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_ovs/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.484906 os_vif-3.1.1/vif_plug_ovs/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_ovs/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1303 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_ovs/tests/functional/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.484906 os_vif-3.1.1/vif_plug_ovs/tests/functional/ovsdb/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_ovs/tests/functional/ovsdb/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7707 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_ovs/tests/functional/ovsdb/test_ovsdb_lib.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3550 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_ovs/tests/functional/test_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.484906 os_vif-3.1.1/vif_plug_ovs/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_ovs/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:29.488906 os_vif-3.1.1/vif_plug_ovs/tests/unit/ovsdb/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_ovs/tests/unit/ovsdb/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10705 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_ovs/tests/unit/ovsdb/test_ovsdb_lib.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17532 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_ovs/tests/unit/test_linux_net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31000 2023-02-10 16:29:59.000000 os_vif-3.1.1/vif_plug_ovs/tests/unit/test_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.174118 os_vif-3.2.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-07-07 14:33:59.000000 os_vif-3.2.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-07-07 14:33:59.000000 os_vif-3.2.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2023-07-07 14:33:59.000000 os_vif-3.2.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5253 2023-07-07 14:33:59.000000 os_vif-3.2.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3132 2023-07-07 14:34:39.000000 os_vif-3.2.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      599 2023-07-07 14:33:59.000000 os_vif-3.2.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13330 2023-07-07 14:34:39.000000 os_vif-3.2.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-07-07 14:33:59.000000 os_vif-3.2.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-07-07 14:33:59.000000 os_vif-3.2.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2029 2023-07-07 14:34:40.174118 os_vif-3.2.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      843 2023-07-07 14:33:59.000000 os_vif-3.2.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2023-07-07 14:33:59.000000 os_vif-3.2.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.142118 os_vif-3.2.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-07-07 14:33:59.000000 os_vif-3.2.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.142118 os_vif-3.2.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1760 2023-07-07 14:33:59.000000 os_vif-3.2.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.142118 os_vif-3.2.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2100 2023-07-07 14:33:59.000000 os_vif-3.2.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2023-07-07 14:33:59.000000 os_vif-3.2.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.142118 os_vif-3.2.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7078 2023-07-07 14:33:59.000000 os_vif-3.2.0/doc/source/reference/glossary.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.142118 os_vif-3.2.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2803 2023-07-07 14:33:59.000000 os_vif-3.2.0/doc/source/user/host-info.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.142118 os_vif-3.2.0/doc/source/user/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2023-07-07 14:33:59.000000 os_vif-3.2.0/doc/source/user/plugins/linux-bridge.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2023-07-07 14:33:59.000000 os_vif-3.2.0/doc/source/user/plugins/noop.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1907 2023-07-07 14:33:59.000000 os_vif-3.2.0/doc/source/user/plugins/ovs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2352 2023-07-07 14:33:59.000000 os_vif-3.2.0/doc/source/user/usage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2164 2023-07-07 14:33:59.000000 os_vif-3.2.0/doc/source/user/vif-types.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.142118 os_vif-3.2.0/os_vif/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5484 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3340 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1040 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.146118 os_vif-3.2.0/os_vif/internal/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/internal/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.146118 os_vif-3.2.0/os_vif/internal/ip/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/internal/ip/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/internal/ip/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2787 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/internal/ip/ip_command.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.146118 os_vif-3.2.0/os_vif/internal/ip/linux/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/internal/ip/linux/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5511 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/internal/ip/linux/impl_pyroute2.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.146118 os_vif-3.2.0/os_vif/internal/ip/windows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/internal/ip/windows/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1745 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/internal/ip/windows/impl_netifaces.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.150118 os_vif-3.2.0/os_vif/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1139 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/objects/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1761 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/objects/fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1282 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/objects/fixed_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6698 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/objects/host_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1226 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/objects/instance_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2134 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/objects/network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1352 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/objects/route.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/objects/subnet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21668 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/objects/vif.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3032 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.150118 os_vif-3.2.0/os_vif/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.150118 os_vif-3.2.0/os_vif/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5005 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/functional/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.150118 os_vif-3.2.0/os_vif/tests/functional/internal/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/functional/internal/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.150118 os_vif-3.2.0/os_vif/tests/functional/internal/command/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/functional/internal/command/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.150118 os_vif-3.2.0/os_vif/tests/functional/internal/command/ip/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/functional/internal/command/ip/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9982 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/functional/internal/command/ip/test_impl_pyroute2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      844 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/functional/privsep.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.150118 os_vif-3.2.0/os_vif/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      795 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/unit/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.150118 os_vif-3.2.0/os_vif/tests/unit/internal/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/unit/internal/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.154118 os_vif-3.2.0/os_vif/tests/unit/internal/ip/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/unit/internal/ip/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.154118 os_vif-3.2.0/os_vif/tests/unit/internal/ip/linux/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/unit/internal/ip/linux/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7364 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/unit/internal/ip/linux/test_impl_pyroute2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1415 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/unit/internal/ip/test_api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.154118 os_vif-3.2.0/os_vif/tests/unit/internal/ip/windows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/unit/internal/ip/windows/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1992 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/unit/internal/ip/windows/test_impl_netifaces.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3137 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/unit/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1335 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/unit/test_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7576 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/unit/test_host_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3709 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/unit/test_objects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6609 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/unit/test_os_vif.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18000 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/tests/unit/test_vif.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2023-07-07 14:33:59.000000 os_vif-3.2.0/os_vif/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.146118 os_vif-3.2.0/os_vif.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2029 2023-07-07 14:34:39.000000 os_vif-3.2.0/os_vif.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6658 2023-07-07 14:34:40.000000 os_vif-3.2.0/os_vif.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-07 14:34:39.000000 os_vif-3.2.0/os_vif.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2023-07-07 14:34:39.000000 os_vif-3.2.0/os_vif.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-07 14:34:39.000000 os_vif-3.2.0/os_vif.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-07-07 14:34:39.000000 os_vif-3.2.0/os_vif.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2023-07-07 14:34:39.000000 os_vif-3.2.0/os_vif.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2023-07-07 14:34:39.000000 os_vif-3.2.0/os_vif.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.138118 os_vif-3.2.0/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.154118 os_vif-3.2.0/playbooks/openstack-tox-functional-ovs-with-sudo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-07-07 14:33:59.000000 os_vif-3.2.0/playbooks/openstack-tox-functional-ovs-with-sudo/Debian.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-07-07 14:33:59.000000 os_vif-3.2.0/playbooks/openstack-tox-functional-ovs-with-sudo/Gentoo.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-07-07 14:33:59.000000 os_vif-3.2.0/playbooks/openstack-tox-functional-ovs-with-sudo/RedHat.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-07-07 14:33:59.000000 os_vif-3.2.0/playbooks/openstack-tox-functional-ovs-with-sudo/Suse.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      566 2023-07-07 14:33:59.000000 os_vif-3.2.0/playbooks/openstack-tox-functional-ovs-with-sudo/pre.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.138118 os_vif-3.2.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.162118 os_vif-3.2.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/OVSVif-hybrid-unplug-f37bf57bc8e913de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/add-abstract-ovsdb-api-8f04df58d4ed5b73.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/add-fast-path-vhostuser-support-fe87e558326909b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/add-no-op-plugin-763a6703e7328a24.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/add-ovs-representor-portprofile-5f8290e5a40bf0a4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/add-ovs-vhostuser-support-2ba8de51c1f3a244.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/add-ovsdb-native-322fffb49c91503d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2079 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/always-plug-vifs-for-ovs-1d033fc49a9c6c4e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/brctl-removal-a5b0e69b865afa57.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/bug-1892132-812e6d5ce0588ebb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/contextlib-and-nested-with-statements-2747a9ebb9a5bfd7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2011 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/default-qos-policy-for-ovs-26f8806046a59c82.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      711 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/default-to-native-ovsdb-driver-112fb5adf6e19a30.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/do-not-force-mac-ageing-c6e8d750130c5740.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/drop-py36-support-0e9b07073f6ad73f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/drop-python2-support-7a4bc7d31253c1e5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/ensure-ovs-bridge-a0c1b51f469c92d0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/extend-vhostuser-object-fada14a1457d4e56.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/fix-ovs-plugin-describe-049750609559f1ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/fix-stevedore-entrypoints-8002ec7a5166c977.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/fix-vif-openvswitch-fa0d19be9dd668e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/generic-datapath-offloads-41cabb6842b41533.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/initial-release-2c71d6bbf55f763b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/oslo-config-opts-entrypoints-e83f907b686d774a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1659 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/per-port-bridge-c6a50179a0256de3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/port-profile-info-linux-bridge-4800f5a0b7328615.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/port-profile-info-ovs-63b46a3eafc11de2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/prevent-lb-reply-arp-6459133bfb056069.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/remove_iptools_implementation-2eb866573a680e61.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      981 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/revert-always-plug-port-for-ovs-hybrid-plug-false-dc015985cbc5443b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/vhost-user-mtu-support-cbc7d02a6665fab1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/notes/vhost-user-reconnect-fa4cbb731b787f71.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.166118 os_vif-3.2.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.166118 os_vif-3.2.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.166118 os_vif-3.2.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1843 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-07-07 14:33:59.000000 os_vif-3.2.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2023-07-07 14:33:59.000000 os_vif-3.2.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1143 2023-07-07 14:34:40.174118 os_vif-3.2.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-07-07 14:33:59.000000 os_vif-3.2.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2023-07-07 14:33:59.000000 os_vif-3.2.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2437 2023-07-07 14:33:59.000000 os_vif-3.2.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.166118 os_vif-3.2.0/vif_plug_linux_bridge/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_linux_bridge/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_linux_bridge/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20641 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_linux_bridge/iptables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4949 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_linux_bridge/linux_bridge.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9481 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_linux_bridge/linux_net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_linux_bridge/privsep.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.166118 os_vif-3.2.0/vif_plug_linux_bridge/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_linux_bridge/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.166118 os_vif-3.2.0/vif_plug_linux_bridge/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_linux_bridge/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6740 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_linux_bridge/tests/unit/test_linux_net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4803 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_linux_bridge/tests/unit/test_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.166118 os_vif-3.2.0/vif_plug_noop/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_noop/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1629 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_noop/noop.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.166118 os_vif-3.2.0/vif_plug_noop/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_noop/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.166118 os_vif-3.2.0/vif_plug_noop/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_noop/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1236 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_noop/tests/unit/test_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.170118 os_vif-3.2.0/vif_plug_ovs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_ovs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_ovs/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1328 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_ovs/exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14289 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_ovs/linux_net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23740 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_ovs/ovs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.170118 os_vif-3.2.0/vif_plug_ovs/ovsdb/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_ovs/ovsdb/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1293 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_ovs/ovsdb/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3028 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_ovs/ovsdb/impl_idl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14437 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_ovs/ovsdb/impl_vsctl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10599 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_ovs/ovsdb/ovsdb_lib.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1100 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_ovs/privsep.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.170118 os_vif-3.2.0/vif_plug_ovs/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_ovs/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.170118 os_vif-3.2.0/vif_plug_ovs/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_ovs/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1872 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_ovs/tests/functional/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.170118 os_vif-3.2.0/vif_plug_ovs/tests/functional/ovsdb/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_ovs/tests/functional/ovsdb/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13513 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_ovs/tests/functional/ovsdb/test_ovsdb_lib.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6648 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_ovs/tests/functional/test_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.174118 os_vif-3.2.0/vif_plug_ovs/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_ovs/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:34:40.174118 os_vif-3.2.0/vif_plug_ovs/tests/unit/ovsdb/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_ovs/tests/unit/ovsdb/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10705 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_ovs/tests/unit/ovsdb/test_ovsdb_lib.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17532 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_ovs/tests/unit/test_linux_net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31199 2023-07-07 14:33:59.000000 os_vif-3.2.0/vif_plug_ovs/tests/unit/test_plugin.py
```

### Comparing `os_vif-3.1.1/.zuul.yaml` & `os_vif-3.2.0/.zuul.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -116,24 +116,14 @@
     vars:
       devstack_local_conf:
         post-config:
           $NOVA_CONF:
             os_vif_ovs:
               per_port_bridge: true
 
-# TODO(gmann): As per the 2023.1 testing runtime, we need to run at least
-# one job on Focal. This job can be removed as per the future testing
-# runtime (whenever we drop the Ubuntu Focal testing).
-- job:
-    name: os-vif-ovn-ubuntu-focal
-    description: |
-      os-vif ovn job (tests hybrid-plug=false) testing on Ubuntu Focal(20.04)
-    parent: os-vif-ovn
-    nodeset: openstack-single-node-focal
-
 - job:
     name: os-vif-linuxbridge
     parent: os-vif-tempest-base
     description: |
       os-vif linux bridge job derived from neutron-tempest-linuxbridge
     vars:
       devstack_services:
@@ -178,17 +168,15 @@
       - openstack-cover-jobs
     check:
       jobs:
         - kuryr-kubernetes-tempest:
             voting: false
         - openstack-tox-functional-ovs-with-sudo
         - os-vif-ovn
-        - os-vif-ovn-ubuntu-focal
         - os-vif-ovs-iptables
         - os-vif-linuxbridge
     gate:
       jobs:
         - openstack-tox-functional-ovs-with-sudo
         - os-vif-ovn
-        - os-vif-ovn-ubuntu-focal
         - os-vif-ovs-iptables
         - os-vif-linuxbridge
```

### Comparing `os_vif-3.1.1/AUTHORS` & `os_vif-3.2.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/CONTRIBUTING.rst` & `os_vif-3.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/ChangeLog` & `os_vif-3.2.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+3.2.0
+-----
+
+* remove focal based jobs
+* set default qos policy
+* Update master for stable/2023.1
+
 3.1.1
 -----
 
 * Increase the swap size to 8GB in tempest jobs
 * Implement "BaseCommand" result property
 * Update gate jobs as per the 2023.1 cycle testing runtime
 * Make tox.ini tox 4.0.0 compatible
```

### Comparing `os_vif-3.1.1/LICENSE` & `os_vif-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/PKG-INFO` & `os_vif-3.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: os_vif
-Version: 3.1.1
+Version: 3.2.0
 Summary: A library for plugging and unplugging virtual interfaces in OpenStack.
 Home-page: https://docs.openstack.org/os-vif/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `os_vif-3.1.1/README.rst` & `os_vif-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/doc/source/conf.py` & `os_vif-3.2.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/doc/source/contributor/contributing.rst` & `os_vif-3.2.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/doc/source/index.rst` & `os_vif-3.2.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/doc/source/reference/glossary.rst` & `os_vif-3.2.0/doc/source/reference/glossary.rst`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/doc/source/user/host-info.rst` & `os_vif-3.2.0/doc/source/user/host-info.rst`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/doc/source/user/plugins/linux-bridge.rst` & `os_vif-3.2.0/doc/source/user/plugins/linux-bridge.rst`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/doc/source/user/plugins/noop.rst` & `os_vif-3.2.0/doc/source/user/plugins/noop.rst`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/doc/source/user/plugins/ovs.rst` & `os_vif-3.2.0/doc/source/user/plugins/ovs.rst`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/doc/source/user/usage.rst` & `os_vif-3.2.0/doc/source/user/usage.rst`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/doc/source/user/vif-types.rst` & `os_vif-3.2.0/doc/source/user/vif-types.rst`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/__init__.py` & `os_vif-3.2.0/os_vif/__init__.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/exception.py` & `os_vif-3.2.0/os_vif/exception.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/i18n.py` & `os_vif-3.2.0/os_vif/i18n.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/internal/__init__.py` & `os_vif-3.2.0/os_vif/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/internal/ip/api.py` & `os_vif-3.2.0/os_vif/internal/ip/api.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/internal/ip/ip_command.py` & `os_vif-3.2.0/os_vif/internal/ip/ip_command.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/internal/ip/linux/impl_pyroute2.py` & `os_vif-3.2.0/os_vif/internal/ip/linux/impl_pyroute2.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/internal/ip/windows/impl_netifaces.py` & `os_vif-3.2.0/os_vif/internal/ip/windows/impl_netifaces.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/objects/__init__.py` & `os_vif-3.2.0/os_vif/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/objects/base.py` & `os_vif-3.2.0/os_vif/objects/base.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/objects/fields.py` & `os_vif-3.2.0/os_vif/objects/fields.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/objects/fixed_ip.py` & `os_vif-3.2.0/os_vif/objects/fixed_ip.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/objects/host_info.py` & `os_vif-3.2.0/os_vif/objects/host_info.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/objects/instance_info.py` & `os_vif-3.2.0/os_vif/objects/instance_info.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/objects/network.py` & `os_vif-3.2.0/os_vif/objects/network.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/objects/route.py` & `os_vif-3.2.0/os_vif/objects/route.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/objects/subnet.py` & `os_vif-3.2.0/os_vif/objects/subnet.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/objects/vif.py` & `os_vif-3.2.0/os_vif/objects/vif.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/opts.py` & `os_vif-3.2.0/os_vif/opts.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/plugin.py` & `os_vif-3.2.0/os_vif/plugin.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/tests/functional/base.py` & `os_vif-3.2.0/os_vif/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/tests/functional/internal/command/ip/test_impl_pyroute2.py` & `os_vif-3.2.0/os_vif/tests/functional/internal/command/ip/test_impl_pyroute2.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import os
 import re
+import time
 
 from oslo_concurrency import processutils
 from oslo_utils import excutils
 
 from os_vif.internal.ip.api import ip as ip_lib
 from os_vif.tests.functional import base
 from os_vif.tests.functional import privsep
@@ -35,14 +36,20 @@
                              'name', device, 'type', dev_type, 'vlan', 'id',
                              vlan_id)
         elif 'veth' == dev_type:
             _execute_command('ip', 'link', 'add', device, 'type', dev_type,
                              'peer', 'name', peer)
         elif 'dummy' == dev_type:
             _execute_command('ip', 'link', 'add', device, 'type', dev_type)
+        # ensure that the device exists to prevent racing
+        # with other ip commands
+        for _ in range(10):
+            if self.exist_device(device):
+                return
+            time.sleep(0.1)
 
     def del_device(self, device):
         if self.exist_device(device):
             _execute_command('ip', 'link', 'del', device)
 
     def set_status_up(self, device):
         _execute_command('ip', 'link', 'set', device, 'up')
```

### Comparing `os_vif-3.1.1/os_vif/tests/functional/privsep.py` & `os_vif-3.2.0/os_vif/tests/functional/privsep.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/tests/unit/base.py` & `os_vif-3.2.0/os_vif/tests/unit/base.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/tests/unit/internal/ip/linux/test_impl_pyroute2.py` & `os_vif-3.2.0/os_vif/tests/unit/internal/ip/linux/test_impl_pyroute2.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/tests/unit/internal/ip/test_api.py` & `os_vif-3.2.0/os_vif/tests/unit/internal/ip/test_api.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/tests/unit/internal/ip/windows/test_impl_netifaces.py` & `os_vif-3.2.0/os_vif/tests/unit/internal/ip/windows/test_impl_netifaces.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/tests/unit/test_base.py` & `os_vif-3.2.0/os_vif/tests/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/tests/unit/test_exception.py` & `os_vif-3.2.0/os_vif/tests/unit/test_exception.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/tests/unit/test_host_info.py` & `os_vif-3.2.0/os_vif/tests/unit/test_host_info.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/tests/unit/test_objects.py` & `os_vif-3.2.0/os_vif/tests/unit/test_objects.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/tests/unit/test_os_vif.py` & `os_vif-3.2.0/os_vif/tests/unit/test_os_vif.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/tests/unit/test_vif.py` & `os_vif-3.2.0/os_vif/tests/unit/test_vif.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/utils.py` & `os_vif-3.2.0/os_vif/utils.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif/version.py` & `os_vif-3.2.0/os_vif/version.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/os_vif.egg-info/PKG-INFO` & `os_vif-3.2.0/os_vif.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: os-vif
-Version: 3.1.1
+Version: 3.2.0
 Summary: A library for plugging and unplugging virtual interfaces in OpenStack.
 Home-page: https://docs.openstack.org/os-vif/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `os_vif-3.1.1/os_vif.egg-info/SOURCES.txt` & `os_vif-3.2.0/os_vif.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
 releasenotes/notes/add-ovs-representor-portprofile-5f8290e5a40bf0a4.yaml
 releasenotes/notes/add-ovs-vhostuser-support-2ba8de51c1f3a244.yaml
 releasenotes/notes/add-ovsdb-native-322fffb49c91503d.yaml
 releasenotes/notes/always-plug-vifs-for-ovs-1d033fc49a9c6c4e.yaml
 releasenotes/notes/brctl-removal-a5b0e69b865afa57.yaml
 releasenotes/notes/bug-1892132-812e6d5ce0588ebb.yaml
 releasenotes/notes/contextlib-and-nested-with-statements-2747a9ebb9a5bfd7.yaml
+releasenotes/notes/default-qos-policy-for-ovs-26f8806046a59c82.yaml
 releasenotes/notes/default-to-native-ovsdb-driver-112fb5adf6e19a30.yaml
 releasenotes/notes/do-not-force-mac-ageing-c6e8d750130c5740.yaml
 releasenotes/notes/drop-py36-support-0e9b07073f6ad73f.yaml
 releasenotes/notes/drop-python2-support-7a4bc7d31253c1e5.yaml
 releasenotes/notes/ensure-ovs-bridge-a0c1b51f469c92d0.yaml
 releasenotes/notes/extend-vhostuser-object-fada14a1457d4e56.yaml
 releasenotes/notes/fix-ovs-plugin-describe-049750609559f1ba.yaml
@@ -113,14 +114,15 @@
 releasenotes/notes/port-profile-info-linux-bridge-4800f5a0b7328615.yaml
 releasenotes/notes/port-profile-info-ovs-63b46a3eafc11de2.yaml
 releasenotes/notes/prevent-lb-reply-arp-6459133bfb056069.yaml
 releasenotes/notes/remove_iptools_implementation-2eb866573a680e61.yaml
 releasenotes/notes/revert-always-plug-port-for-ovs-hybrid-plug-false-dc015985cbc5443b.yaml
 releasenotes/notes/vhost-user-mtu-support-cbc7d02a6665fab1.yaml
 releasenotes/notes/vhost-user-reconnect-fa4cbb731b787f71.yaml
+releasenotes/source/2023.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
```

### Comparing `os_vif-3.1.1/playbooks/openstack-tox-functional-ovs-with-sudo/pre.yaml` & `os_vif-3.2.0/playbooks/openstack-tox-functional-ovs-with-sudo/pre.yaml`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/releasenotes/notes/add-ovsdb-native-322fffb49c91503d.yaml` & `os_vif-3.2.0/releasenotes/notes/add-ovsdb-native-322fffb49c91503d.yaml`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/releasenotes/notes/always-plug-vifs-for-ovs-1d033fc49a9c6c4e.yaml` & `os_vif-3.2.0/releasenotes/notes/always-plug-vifs-for-ovs-1d033fc49a9c6c4e.yaml`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/releasenotes/notes/brctl-removal-a5b0e69b865afa57.yaml` & `os_vif-3.2.0/releasenotes/notes/brctl-removal-a5b0e69b865afa57.yaml`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/releasenotes/notes/default-to-native-ovsdb-driver-112fb5adf6e19a30.yaml` & `os_vif-3.2.0/releasenotes/notes/default-to-native-ovsdb-driver-112fb5adf6e19a30.yaml`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/releasenotes/notes/do-not-force-mac-ageing-c6e8d750130c5740.yaml` & `os_vif-3.2.0/releasenotes/notes/do-not-force-mac-ageing-c6e8d750130c5740.yaml`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/releasenotes/notes/generic-datapath-offloads-41cabb6842b41533.yaml` & `os_vif-3.2.0/releasenotes/notes/generic-datapath-offloads-41cabb6842b41533.yaml`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/releasenotes/notes/per-port-bridge-c6a50179a0256de3.yaml` & `os_vif-3.2.0/releasenotes/notes/per-port-bridge-c6a50179a0256de3.yaml`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/releasenotes/notes/revert-always-plug-port-for-ovs-hybrid-plug-false-dc015985cbc5443b.yaml` & `os_vif-3.2.0/releasenotes/notes/revert-always-plug-port-for-ovs-hybrid-plug-false-dc015985cbc5443b.yaml`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/releasenotes/notes/vhost-user-reconnect-fa4cbb731b787f71.yaml` & `os_vif-3.2.0/releasenotes/notes/vhost-user-reconnect-fa4cbb731b787f71.yaml`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/releasenotes/source/conf.py` & `os_vif-3.2.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/requirements.txt` & `os_vif-3.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/setup.cfg` & `os_vif-3.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/setup.py` & `os_vif-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/tox.ini` & `os_vif-3.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/vif_plug_linux_bridge/constants.py` & `os_vif-3.2.0/vif_plug_linux_bridge/constants.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/vif_plug_linux_bridge/iptables.py` & `os_vif-3.2.0/vif_plug_linux_bridge/iptables.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/vif_plug_linux_bridge/linux_bridge.py` & `os_vif-3.2.0/vif_plug_linux_bridge/linux_bridge.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/vif_plug_linux_bridge/linux_net.py` & `os_vif-3.2.0/vif_plug_linux_bridge/linux_net.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/vif_plug_linux_bridge/privsep.py` & `os_vif-3.2.0/vif_plug_linux_bridge/privsep.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/vif_plug_linux_bridge/tests/unit/test_linux_net.py` & `os_vif-3.2.0/vif_plug_linux_bridge/tests/unit/test_linux_net.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/vif_plug_linux_bridge/tests/unit/test_plugin.py` & `os_vif-3.2.0/vif_plug_linux_bridge/tests/unit/test_plugin.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/vif_plug_noop/noop.py` & `os_vif-3.2.0/vif_plug_noop/noop.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/vif_plug_noop/tests/unit/test_plugin.py` & `os_vif-3.2.0/vif_plug_noop/tests/unit/test_plugin.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/vif_plug_ovs/constants.py` & `os_vif-3.2.0/vif_plug_ovs/constants.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/vif_plug_ovs/exception.py` & `os_vif-3.2.0/vif_plug_ovs/exception.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/vif_plug_ovs/linux_net.py` & `os_vif-3.2.0/vif_plug_ovs/linux_net.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/vif_plug_ovs/ovs.py` & `os_vif-3.2.0/vif_plug_ovs/ovs.py`

 * *Files 15% similar despite different names*

```diff
@@ -98,15 +98,34 @@
                     'to the ovs bridge. This should only be set to True '
                     'when using the neutron ovs ml2 agent.'),
         cfg.BoolOpt('per_port_bridge', default=False,
                     help='Controls if VIF should be plugged into a per-port '
                     'bridge. This is experimental and controls the plugging '
                     'behavior when not using hybrid-plug.'
                     'This is only used on linux and should be set to false '
-                    'in all other cases such as ironic smartnic ports.')
+                    'in all other cases such as ironic smartnic ports.'),
+        cfg.StrOpt('default_qos_type',
+                   choices=[
+                       'linux-htb', 'linux-hfsc', 'linux-sfq', 'linux-codel',
+                       'linux-fq_codel', 'linux-noop'
+                       ],
+                   default='linux-noop',
+                   help="""
+                   The default qos type to apply to ovs ports.
+                   linux-noop is the default. ovs will not modify
+                   the qdisc on the port if linux-noop is specified.
+                   This allows operators to manage QOS out of band
+                   of OVS. For more information see the ovs man pages
+                   https://manpages.debian.org/testing/openvswitch-common/ovs-vswitchd.conf.db.5.en.html#type~4
+
+                   Note: This will only be set when a port is first created
+                   on the ovs bridge to ensure that the qos type can be
+                   managed via neutron if required for bandwidth limiting
+                   and other use-cases.
+                   """),
     )
 
     def __init__(self, config):
         super(OvsPlugin, self).__init__(config)
         self.ovsdb = ovsdb_lib.BaseOVS(self.config)
 
     @staticmethod
@@ -155,14 +174,22 @@
             ])
 
     def _get_mtu(self, vif):
         if vif.network and vif.network.mtu:
             return vif.network.mtu
         return self.config.network_device_mtu
 
+    def supports_tc_qdisc(self, vif) -> bool:
+        if self._get_vif_datapath_type(vif) != constants.OVS_DATAPATH_SYSTEM:
+            return False
+        if sys.platform == constants.PLATFORM_WIN32:
+            return False
+
+        return True
+
     def _create_vif_port(self, vif, vif_name, instance_info, **kwargs):
         mtu = self._get_mtu(vif)
         # NOTE(sean-k-mooney): As part of a partial fix to bug #1734320
         # we introduced the isolate_vif config option to enable isolation
         # of the vif prior to neutron wiring up the interface. To do
         # this we take advantage of the fact the ml2/ovs uses the
         # implementation defined VLAN 4095 as a dead VLAN to indicate
@@ -171,14 +198,27 @@
         # deployment such as ODL or OVN as such operator must opt-in
         # to this behaviour by setting the isolate_vif config option.
         # TODO(sean-k-mooney): Extend neutron to record what ml2 driver
         # bound the interface in the vif binding details so isolation
         # can be enabled automatically in the future.
         if self.config.isolate_vif:
             kwargs['tag'] = constants.DEAD_VLAN
+        qos_type = self._get_qos_type(vif)
+        if qos_type is not None:
+            # NOTE(sean-k-mooney): If the port is not already created
+            # on the bridge we need to set the default qos type to
+            # ensure that the port is created with the correct qos
+            # type. This is only needed for the linux kernel datapath
+            # as the qos type is not managed by neutron for the other
+            # datapaths.
+            # This is a mitigation for the performance regression
+            # introduced by the fix for bug #1734320. See bug #2017868
+            # for more details.
+            if not self.ovsdb.port_exists(vif_name, vif.network.bridge):
+                kwargs['qos_type'] = qos_type
         bridge = kwargs.pop('bridge', vif.network.bridge)
         self.ovsdb.create_ovs_vif_port(
             bridge,
             vif_name,
             vif.port_profile.interface_id,
             vif.address, instance_info.uuid,
             mtu=mtu,
@@ -378,17 +418,26 @@
         bridge, and delete both veth devices.
         """
 
         v1_name, v2_name = self.get_veth_pair_names(vif)
 
         linux_net.delete_bridge(linux_bridge_name, v1_name)
 
-        self.ovsdb.delete_ovs_vif_port(vif.network.bridge, v2_name)
+        qos_type = self._get_qos_type(vif)
+        self.ovsdb.delete_ovs_vif_port(
+            vif.network.bridge, v2_name, qos_type=qos_type
+        )
         self._delete_bridge_if_trunk(vif)
 
+    def _get_qos_type(self, vif):
+        qos_type = None
+        if self.supports_tc_qdisc(vif):
+            qos_type = self.config.default_qos_type
+        return qos_type
+
     def _unplug_vif_windows(self, vif, instance_info):
         """Remove port from OVS."""
         self.ovsdb.delete_ovs_vif_port(vif.network.bridge, vif.id,
                                        delete_netdev=False)
         self._delete_bridge_if_trunk(vif)
 
     def _unplug_port_bridge(self, vif, instance_info):
@@ -396,24 +445,30 @@
         # NOTE(sean-k-mooney): the port name prefix should not be
         # changed to avoid loosing ports on upgrade.
         port_bridge_name = self.gen_port_name('pb', vif.id)
         port_bridge_patch = self.gen_port_name('pbp', vif.id, max_length=64)
         int_bridge_patch = self.gen_port_name('ibp', vif.id, max_length=64)
         self.ovsdb.delete_ovs_vif_port(vif.network.bridge, int_bridge_patch)
         self.ovsdb.delete_ovs_vif_port(port_bridge_name, port_bridge_patch)
-        self.ovsdb.delete_ovs_vif_port(port_bridge_name, vif.vif_name)
+        qos_type = self._get_qos_type(vif)
+        self.ovsdb.delete_ovs_vif_port(
+            port_bridge_name, vif.vif_name, qos_type=qos_type
+        )
         self.ovsdb.delete_ovs_bridge(port_bridge_name)
         self._delete_bridge_if_trunk(vif)
 
     def _unplug_vif_generic(self, vif, instance_info):
         """Remove port from OVS."""
         # NOTE(sean-k-mooney): even with the partial revert of change
         # Iaf15fa7a678ec2624f7c12f634269c465fbad930 this should be correct
         # so this is not removed.
-        self.ovsdb.delete_ovs_vif_port(vif.network.bridge, vif.vif_name)
+        qos_type = self._get_qos_type(vif)
+        self.ovsdb.delete_ovs_vif_port(
+            vif.network.bridge, vif.vif_name, qos_type=qos_type
+        )
         self._delete_bridge_if_trunk(vif)
 
     def _unplug_vf(self, vif):
         """Remove port from OVS."""
         datapath = self._get_vif_datapath_type(vif)
         if datapath == constants.OVS_DATAPATH_SYSTEM:
             pci_slot = vif.dev_address
@@ -424,16 +479,19 @@
         else:
             representor = linux_net.get_dpdk_representor_port_name(
                 vif.id)
 
         # The representor interface can't be deleted because it bind the
         # SR-IOV VF, therefore we just need to remove it from the ovs bridge
         # and set the status to down
+        qos_type = self._get_qos_type(vif)
         self.ovsdb.delete_ovs_vif_port(
-            vif.network.bridge, representor, delete_netdev=False)
+            vif.network.bridge, representor, delete_netdev=False,
+            qos_type=qos_type
+        )
         if datapath == constants.OVS_DATAPATH_SYSTEM:
             linux_net.set_interface_state(representor, 'down')
         self._delete_bridge_if_trunk(vif)
 
     def unplug(self, vif, instance_info):
         if not hasattr(vif, "port_profile"):
             raise exception.MissingPortProfile()
```

### Comparing `os_vif-3.1.1/vif_plug_ovs/ovsdb/api.py` & `os_vif-3.2.0/vif_plug_ovs/ovsdb/api.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/vif_plug_ovs/ovsdb/impl_idl.py` & `os_vif-3.2.0/vif_plug_ovs/ovsdb/impl_idl.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from ovsdbapp.backend.ovs_idl import connection
 from ovsdbapp.backend.ovs_idl import idlutils
 from ovsdbapp.backend.ovs_idl import vlog
 from ovsdbapp.schema.open_vswitch import impl_idl
 
 from vif_plug_ovs.ovsdb import api
 
-REQUIRED_TABLES = ('Interface', 'Port', 'Bridge', 'Open_vSwitch')
+REQUIRED_TABLES = ('Interface', 'Port', 'Bridge', 'Open_vSwitch', 'QoS')
 
 
 def idl_factory(config):
     conn = config.connection
     schema_name = 'Open_vSwitch'
     helper = idlutils.get_schema_helper(conn, schema_name)
     for table in REQUIRED_TABLES:
@@ -44,14 +44,15 @@
 
 class NeutronOvsdbIdl(impl_idl.OvsdbIdl, api.ImplAPI):
     """IDL interface for OVS database back-end
 
     This class provides an OVSDB IDL (Open vSwitch Database Interface
     Definition Language) interface to the OVS back-end.
     """
+
     def __init__(self, conn):
         vlog.use_python_logger()
         super(NeutronOvsdbIdl, self).__init__(conn)
 
     def _get_table_columns(self, table):
         return list(self.tables[table].columns)
```

### Comparing `os_vif-3.1.1/vif_plug_ovs/ovsdb/impl_vsctl.py` & `os_vif-3.2.0/vif_plug_ovs/ovsdb/impl_vsctl.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/vif_plug_ovs/ovsdb/ovsdb_lib.py` & `os_vif-3.2.0/vif_plug_ovs/ovsdb/ovsdb_lib.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import sys
+import uuid
 
 from oslo_log import log as logging
 
 from vif_plug_ovs import constants
 from vif_plug_ovs import linux_net
 from vif_plug_ovs.ovsdb import api as ovsdb_api
 
 
 LOG = logging.getLogger(__name__)
+QOS_UUID_NAMESPACE = uuid.UUID("68da264a-847f-42a8-8ab0-5e774aee3d95")
 
 
 class BaseOVS(object):
 
     def __init__(self, config):
         self.timeout = config.ovs_vsctl_timeout
         self.connection = config.ovsdb_connection
@@ -138,15 +140,16 @@
             txn.add(self.ovsdb.add_port(port_bridge, port_bridge_port))
             txn.add(
                 self.ovsdb.db_set('Interface', port_bridge_port, *col_values))
 
     def create_ovs_vif_port(
         self, bridge, dev, iface_id, mac, instance_id,
         mtu=None, interface_type=None, vhost_server_path=None,
-        tag=None, pf_pci=None, vf_num=None, set_ids=True, datapath_type=None
+        tag=None, pf_pci=None, vf_num=None, set_ids=True, datapath_type=None,
+        qos_type=None
     ):
         """Create OVS port
 
         :param bridge: bridge name to create the port on.
         :param dev: port name.
         :param iface_id: port ID.
         :param mac: port MAC.
@@ -155,14 +158,15 @@
         :param interface_type: OVS interface type.
         :param vhost_server_path: path to socket file of vhost server.
         :param tag: OVS interface tag.
         :param pf_pci: PCI address of PF for dpdk representor port.
         :param vf_num: VF number of PF for dpdk representor port.
         :param set_ids: set external ids on port (bool).
         :param datapath_type: datapath type for port's bridge
+        :param qos_type: qos type for a port
 
         .. note:: create DPDK representor port by setting all three values:
             `interface_type`, `pf_pci` and `vf_num`. if interface type is
             not `OVS_DPDK_INTERFACE_TYPE` then `pf_pci` and `vf_num` values
             are ignored.
         """
         external_ids = {'iface-id': iface_id,
@@ -177,30 +181,75 @@
                                {'vhost-server-path': vhost_server_path}))
         if (interface_type == constants.OVS_DPDK_INTERFACE_TYPE and
                 pf_pci and vf_num):
             devargs_string = "{PF_PCI},representor=[{VF_NUM}]".format(
                 PF_PCI=pf_pci, VF_NUM=vf_num)
             col_values.append(('options',
                               {'dpdk-devargs': devargs_string}))
+        # create qos record if qos type is specified
+        # and get the qos id. This is done outside of the transaction
+        # because we need the qos id to set the qos on the port.
+        # The qos uuid cannot be set when creating the record so we
+        # have to look it up after the record is created. this means
+        # we need to create the qos record outside of the transaction
+        # that creates the port.
+        qid = None
+        if qos_type:
+            self.delete_qos_if_exists(dev, qos_type)
+            qos_id = uuid.uuid5(QOS_UUID_NAMESPACE, dev)
+            qos_external_ids = {'id': str(qos_id), '_type': qos_type}
+            self.ovsdb.db_create(
+                'QoS', type=qos_type, external_ids=qos_external_ids
+                ).execute(check_error=True)
+            record = self.get_qos(dev, qos_type)
+            qid = record[0]['_uuid']
+
         with self.ovsdb.transaction() as txn:
             if datapath_type:
                 txn.add(self.ovsdb.add_br(bridge, may_exist=True,
                                           datapath_type=datapath_type))
             txn.add(self.ovsdb.add_port(bridge, dev))
             if tag:
                 txn.add(self.ovsdb.db_set('Port', dev, ('tag', tag)))
+            if qid:
+                txn.add(self.ovsdb.db_set('Port', dev, ('qos', qid)))
             if col_values:
                 txn.add(self.ovsdb.db_set('Interface', dev, *col_values))
             self.update_device_mtu(
                 txn, dev, mtu, interface_type=interface_type
             )
 
+    def port_exists(self, port_name, bridge):
+        ports = self.ovsdb.list_ports(bridge).execute()
+        return ports is not None and port_name in ports
+
+    def get_qos(self, dev, qos_type):
+        qos_id = uuid.uuid5(QOS_UUID_NAMESPACE, dev)
+        external_ids = {'id': str(qos_id), '_type': qos_type}
+        return self.ovsdb.db_find(
+            'QoS', ('external_ids', '=', external_ids),
+            colmuns=['_uuid']
+        ).execute()
+
+    def delete_qos_if_exists(self, dev, qos_type):
+        qos_ids = self.get_qos(dev, qos_type)
+        if qos_ids is not None and len(qos_ids) > 0:
+            for qos_id in qos_ids:
+                if '_uuid' in qos_id:
+                    self.ovsdb.db_destroy(
+                        'QoS', str(qos_id['_uuid'])
+                    ).execute()
+
     def update_ovs_vif_port(self, dev, mtu=None, interface_type=None):
         with self.ovsdb.transaction() as txn:
             self.update_device_mtu(
                 txn, dev, mtu, interface_type=interface_type
             )
 
-    def delete_ovs_vif_port(self, bridge, dev, delete_netdev=True):
+    def delete_ovs_vif_port(
+            self, bridge, dev, delete_netdev=True, qos_type=None
+    ):
         self.ovsdb.del_port(dev, bridge=bridge, if_exists=True).execute()
+        if qos_type:
+            self.delete_qos_if_exists(dev, qos_type)
         if delete_netdev:
             linux_net.delete_net_dev(dev)
```

### Comparing `os_vif-3.1.1/vif_plug_ovs/privsep.py` & `os_vif-3.2.0/vif_plug_ovs/privsep.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/vif_plug_ovs/tests/functional/base.py` & `os_vif-3.2.0/vif_plug_ovs/tests/functional/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,14 +21,30 @@
 
     COMPONENT_NAME = 'vif_plug_ovs'
     PRIVILEGED_GROUP = 'vif_plug_ovs_privileged'
 
     def _check_bridge(self, name):
         return self._ovsdb.br_exists(name).execute()
 
+    def _check_port(self, name, bridge):
+        return self.ovs.port_exists(name, bridge)
+
+    def _check_parameter(self, table, port, parameter, expected_value):
+        def get_value():
+            return self._ovsdb.db_get(table, port, parameter).execute()
+
+        def check_value():
+            val = get_value()
+            return val == expected_value
+        self.assertTrue(
+            wait_until_true(check_value, timeout=2, sleep=0.5),
+            f"Parameter {parameter} of {table} {port} is {get_value()} "
+            f"not {expected_value}"
+        )
+
     def _add_bridge(self, name, may_exist=True, datapath_type=None):
         self._ovsdb.add_br(name, may_exist=may_exist,
                            datapath_type=datapath_type).execute()
         self.assertTrue(self._check_bridge(name))
 
     def _del_bridge(self, name):
         self._ovsdb.del_br(name).execute()
```

### Comparing `os_vif-3.1.1/vif_plug_ovs/tests/unit/ovsdb/test_ovsdb_lib.py` & `os_vif-3.2.0/vif_plug_ovs/tests/unit/ovsdb/test_ovsdb_lib.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/vif_plug_ovs/tests/unit/test_linux_net.py` & `os_vif-3.2.0/vif_plug_ovs/tests/unit/test_linux_net.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.1.1/vif_plug_ovs/tests/unit/test_plugin.py` & `os_vif-3.2.0/vif_plug_ovs/tests/unit/test_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,15 +358,17 @@
     @mock.patch.object(ovsdb_lib.BaseOVS, 'delete_ovs_vif_port')
     @mock.patch.object(linux_net, 'delete_bridge')
     @mock.patch.object(ovs, 'sys')
     def test_unplug_ovs_bridge(self, mock_sys, delete_bridge,
                                delete_ovs_vif_port, delete_ovs_bridge):
         calls = {
             'delete_bridge': [mock.call('qbrvif-xxx-yyy', 'qvbb679325f-ca')],
-            'delete_ovs_vif_port': [mock.call('br0', 'qvob679325f-ca')]
+            'delete_ovs_vif_port': [mock.call(
+                'br0', 'qvob679325f-ca', qos_type='linux-noop'
+            )]
         }
         mock_sys.platform = 'linux'
         plugin = ovs.OvsPlugin.load(constants.PLUGIN_NAME)
         plugin.unplug(self.vif_ovs_hybrid, self.instance)
         delete_bridge.assert_has_calls(calls['delete_bridge'])
         delete_ovs_vif_port.assert_has_calls(calls['delete_ovs_vif_port'])
         delete_ovs_bridge.assert_not_called()
@@ -506,16 +508,20 @@
 
             'get_ifname_by_pci_address': [mock.call('0002:24:12.3',
                                           pf_interface=True,
                                           switchdev=True)],
             'get_vf_num_by_pci_address': [mock.call('0002:24:12.3')],
             'get_representor_port': [mock.call('eth0', '2')],
             'set_interface_state': [mock.call('eth0_2', 'down')],
-            'delete_ovs_vif_port': [mock.call('br0', 'eth0_2',
-                                              delete_netdev=False)]
+            'delete_ovs_vif_port': [
+                mock.call(
+                    'br0', 'eth0_2', delete_netdev=False,
+                    qos_type='linux-noop'
+                )
+            ]
         }
 
         get_ifname_by_pci_address.return_value = 'eth0'
         get_vf_num_by_pci_address.return_value = '2'
         get_representor_port.return_value = 'eth0_2'
         plugin = ovs.OvsPlugin.load(constants.PLUGIN_NAME)
         plugin.unplug(self.vif_ovs_vf_passthrough, self.instance)
@@ -598,16 +604,21 @@
                                 get_dpdk_representor_port_name,
                                 delete_ovs_bridge):
         devname = 'vfrb679325f-ca'
         get_dpdk_representor_port_name.return_value = devname
         calls = {
             'get_dpdk_representor_port_name': [mock.call(
                 self.vif_ovs_vf_dpdk.id)],
-            'delete_ovs_vif_port': [mock.call('br0', devname,
-                                              delete_netdev=False)]}
+            'delete_ovs_vif_port': [
+                mock.call(
+                    'br0', devname, delete_netdev=False,
+                    qos_type=None
+                )
+            ]
+        }
         plugin = ovs.OvsPlugin.load(constants.PLUGIN_NAME)
         plugin.unplug(self.vif_ovs_vf_dpdk, self.instance)
         get_dpdk_representor_port_name.assert_has_calls(
             calls['get_dpdk_representor_port_name'])
         delete_ovs_vif_port.assert_has_calls(calls['delete_ovs_vif_port'])
         delete_ovs_bridge.assert_not_called()
 
@@ -632,15 +643,15 @@
             self, delete_ovs_bridge, delete_ovs_vif_port):
         plugin = ovs.OvsPlugin.load(constants.PLUGIN_NAME)
         plugin._unplug_port_bridge(self.vif_ovs, self.instance)
         calls = [
             mock.call('br0', 'ibpb679325f-ca89-4ee0-a8be-6db1409b69ea'),
             mock.call(
                 'pbb679325f-ca8', 'pbpb679325f-ca89-4ee0-a8be-6db1409b69ea'),
-            mock.call('pbb679325f-ca8', 'tap-xxx-yyy-zzz')
+            mock.call('pbb679325f-ca8', 'tap-xxx-yyy-zzz', qos_type=None)
         ]
         delete_ovs_vif_port.assert_has_calls(calls)
         delete_ovs_bridge.assert_called_once_with('pbb679325f-ca8')
 
     @mock.patch.object(ip_lib, 'exists', return_value=True)
     @mock.patch.object(ovs.OvsPlugin, '_unplug_bridge')
     def test_unplug_hybrid_bridge(self, m_unplug_bridge, m_ip_lib_exists):
```

