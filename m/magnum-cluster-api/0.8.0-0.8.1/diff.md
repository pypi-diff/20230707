# Comparing `tmp/magnum_cluster_api-0.8.0.tar.gz` & `tmp/magnum_cluster_api-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnum_cluster_api-0.8.0.tar", max compression
+gzip compressed data, was "magnum_cluster_api-0.8.1.tar", max compression
```

## Comparing `magnum_cluster_api-0.8.0.tar` & `magnum_cluster_api-0.8.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0    10142 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/LICENSE
--rw-r--r--   0        0        0     3353 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/README.md
--rw-r--r--   0        0        0        0 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/.gitkeep
--rw-r--r--   0        0        0      349 2023-07-05 04:18:35.515678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/.helmignore
--rw-r--r--   0        0        0      437 2023-07-05 04:18:35.511678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/Chart.yaml
--rw-r--r--   0        0        0    29122 2023-07-05 04:18:35.515678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/README.md
--rw-r--r--   0        0        0    14987 2023-07-05 04:18:35.515678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl
--rw-r--r--   0        0        0      827 2023-07-05 04:18:35.511678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt
--rw-r--r--   0        0        0     4034 2023-07-05 04:18:35.511678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl
--rw-r--r--   0        0        0     2982 2023-07-05 04:18:35.571678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml
--rw-r--r--   0        0        0      534 2023-07-05 04:18:35.511678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml
--rw-r--r--   0        0        0    13204 2023-07-05 04:18:35.511678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml
--rw-r--r--   0        0        0      508 2023-07-05 04:18:35.511678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/pdb.yaml
--rw-r--r--   0        0        0      972 2023-07-05 04:18:35.511678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml
--rw-r--r--   0        0        0      758 2023-07-05 04:18:35.511678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml
--rw-r--r--   0        0        0      564 2023-07-05 04:18:35.511678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml
--rw-r--r--   0        0        0     1807 2023-07-05 04:18:35.515678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml
--rw-r--r--   0        0        0      527 2023-07-05 04:18:35.515678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml
--rw-r--r--   0        0        0      989 2023-07-05 04:18:35.515678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml
--rw-r--r--   0        0        0     1180 2023-07-05 04:18:35.515678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml
--rw-r--r--   0        0        0      528 2023-07-05 04:18:35.515678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml
--rw-r--r--   0        0        0      960 2023-07-05 04:18:35.515678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml
--rw-r--r--   0        0        0      663 2023-07-05 04:18:35.515678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml
--rw-r--r--   0        0        0    18003 2023-07-05 04:18:35.511678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/values.yaml
--rw-r--r--   0        0        0     1977 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/clients.py
--rw-r--r--   0        0        0        0 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/cmd/__init__.py
--rw-r--r--   0        0        0     5005 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/cmd/image_builder.py
--rw-r--r--   0        0        0     4713 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/cmd/image_loader.py
--rw-r--r--   0        0        0      956 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/cmd/proxy.py
--rw-r--r--   0        0        0     3460 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/conf.py
--rw-r--r--   0        0        0    14117 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/driver.py
--rw-r--r--   0        0        0     1219 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/exceptions.py
--rw-r--r--   0        0        0     3486 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/helm.py
--rw-r--r--   0        0        0     3460 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/image_utils.py
--rw-r--r--   0        0        0     1116 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/images.py
--rw-r--r--   0        0        0        0 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/integrations/__init__.py
--rw-r--r--   0        0        0     1759 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/integrations/cinder.py
--rw-r--r--   0        0        0      839 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/integrations/cloud_provider.py
--rw-r--r--   0        0        0     3012 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/integrations/common.py
--rw-r--r--   0        0        0      948 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/integrations/manila.py
--rw-r--r--   0        0        0        0 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/__init__.py
--rw-r--r--   0        0        0     4941 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/audit/policy.yaml
--rw-r--r--   0        0        0   235191 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/calico/v3.24.2.yaml
--rw-r--r--   0        0        0      623 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml
--rw-r--r--   0        0        0     1430 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml
--rw-r--r--   0        0        0     2263 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml
--rw-r--r--   0        0        0     4506 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin-rbac.yaml
--rw-r--r--   0        0        0     4034 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin.yaml
--rw-r--r--   0        0        0      609 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin-rbac.yaml
--rw-r--r--   0        0        0     3307 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin.yaml
--rw-r--r--   0        0        0      194 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/cinder-csi/csi-cinder-driver.yaml
--rw-r--r--   0        0        0     3377 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin-rbac.yaml
--rw-r--r--   0        0        0     3944 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin.yaml
--rw-r--r--   0        0        0     1513 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin-rbac.yaml
--rw-r--r--   0        0        0     2988 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin.yaml
--rw-r--r--   0        0        0      143 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/manila-csi/csidriver.yaml
--rw-r--r--   0        0        0     3127 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-controller.yaml
--rw-r--r--   0        0        0      170 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-driverinfo.yaml
--rw-r--r--   0        0        0     3530 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-node.yaml
--rw-r--r--   0        0        0     1423 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/nfs-csi/rbac-csi-nfs.yaml
--rw-r--r--   0        0        0     1526 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/monitor.py
--rw-r--r--   0        0        0     5673 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/objects.py
--rw-r--r--   0        0        0      828 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/privsep/__init__.py
--rw-r--r--   0        0        0     1333 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/privsep/haproxy.py
--rw-r--r--   0        0        0    11719 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/proxy/manager.py
--rw-r--r--   0        0        0     3616 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/proxy/structs.py
--rw-r--r--   0        0        0      580 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/proxy/templates/haproxy.cfg.j2
--rw-r--r--   0        0        0     1511 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/proxy/utils.py
--rw-r--r--   0        0        0    84493 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/resources.py
--rw-r--r--   0        0        0     1492 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/service.py
--rw-r--r--   0        0        0     3124 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/tests/functional/conftest.py
--rw-r--r--   0        0        0      666 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/tests/functional/test_clusters.py
--rw-r--r--   0        0        0      942 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/conftest.py
--rw-r--r--   0        0        0     3813 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_helm.py
--rw-r--r--   0        0        0     1731 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_image_utils.py
--rw-r--r--   0        0        0     3105 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_images.py
--rw-r--r--   0        0        0     5366 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_objects.py
--rw-r--r--   0        0        0     1735 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_resources.py
--rw-r--r--   0        0        0     1192 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_utils.py
--rw-r--r--   0        0        0     8746 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/utils.py
--rw-r--r--   0        0        0     1288 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4448 1970-01-01 00:00:00.000000 magnum_cluster_api-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-07-07 03:54:37.672372 magnum_cluster_api-0.8.1/LICENSE
+-rw-r--r--   0        0        0     3369 2023-07-07 03:54:37.672372 magnum_cluster_api-0.8.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/.gitkeep
+-rw-r--r--   0        0        0      349 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/.helmignore
+-rw-r--r--   0        0        0      437 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/Chart.yaml
+-rw-r--r--   0        0        0    29122 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/README.md
+-rw-r--r--   0        0        0    14987 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl
+-rw-r--r--   0        0        0      827 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt
+-rw-r--r--   0        0        0     4034 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl
+-rw-r--r--   0        0        0     2982 2023-07-07 03:54:41.956405 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml
+-rw-r--r--   0        0        0      534 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml
+-rw-r--r--   0        0        0    13204 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml
+-rw-r--r--   0        0        0      508 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/pdb.yaml
+-rw-r--r--   0        0        0      972 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml
+-rw-r--r--   0        0        0      758 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml
+-rw-r--r--   0        0        0      564 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml
+-rw-r--r--   0        0        0     1807 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml
+-rw-r--r--   0        0        0      527 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml
+-rw-r--r--   0        0        0      989 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml
+-rw-r--r--   0        0        0     1180 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml
+-rw-r--r--   0        0        0      528 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0      960 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml
+-rw-r--r--   0        0        0      663 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml
+-rw-r--r--   0        0        0    18003 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/values.yaml
+-rw-r--r--   0        0        0     1977 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/clients.py
+-rw-r--r--   0        0        0        0 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/cmd/__init__.py
+-rw-r--r--   0        0        0     5005 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/cmd/image_builder.py
+-rw-r--r--   0        0        0     6891 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/cmd/image_loader.py
+-rw-r--r--   0        0        0      956 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/cmd/proxy.py
+-rw-r--r--   0        0        0     3460 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/conf.py
+-rw-r--r--   0        0        0    14323 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/driver.py
+-rw-r--r--   0        0        0     1219 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/exceptions.py
+-rw-r--r--   0        0        0     3276 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/helm.py
+-rw-r--r--   0        0        0     3460 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/image_utils.py
+-rw-r--r--   0        0        0     1116 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/images.py
+-rw-r--r--   0        0        0        0 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/integrations/__init__.py
+-rw-r--r--   0        0        0     1759 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/integrations/cinder.py
+-rw-r--r--   0        0        0      839 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/integrations/cloud_provider.py
+-rw-r--r--   0        0        0     3012 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/integrations/common.py
+-rw-r--r--   0        0        0      948 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/integrations/manila.py
+-rw-r--r--   0        0        0        0 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/__init__.py
+-rw-r--r--   0        0        0     4941 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/audit/policy.yaml
+-rw-r--r--   0        0        0   235191 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/calico/v3.24.2.yaml
+-rw-r--r--   0        0        0      623 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml
+-rw-r--r--   0        0        0     1430 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml
+-rw-r--r--   0        0        0     2263 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml
+-rw-r--r--   0        0        0     4506 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin-rbac.yaml
+-rw-r--r--   0        0        0     4034 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin.yaml
+-rw-r--r--   0        0        0      609 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin-rbac.yaml
+-rw-r--r--   0        0        0     3307 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin.yaml
+-rw-r--r--   0        0        0      194 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/cinder-csi/csi-cinder-driver.yaml
+-rw-r--r--   0        0        0     3377 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin-rbac.yaml
+-rw-r--r--   0        0        0     3944 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin.yaml
+-rw-r--r--   0        0        0     1513 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin-rbac.yaml
+-rw-r--r--   0        0        0     2988 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin.yaml
+-rw-r--r--   0        0        0      143 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/manila-csi/csidriver.yaml
+-rw-r--r--   0        0        0     3127 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/nfs-csi/csi-nfs-controller.yaml
+-rw-r--r--   0        0        0      170 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/nfs-csi/csi-nfs-driverinfo.yaml
+-rw-r--r--   0        0        0     3530 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/nfs-csi/csi-nfs-node.yaml
+-rw-r--r--   0        0        0     1423 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/nfs-csi/rbac-csi-nfs.yaml
+-rw-r--r--   0        0        0     1526 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/monitor.py
+-rw-r--r--   0        0        0     5673 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/objects.py
+-rw-r--r--   0        0        0      828 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/privsep/__init__.py
+-rw-r--r--   0        0        0     1333 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/privsep/haproxy.py
+-rw-r--r--   0        0        0    11719 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/proxy/manager.py
+-rw-r--r--   0        0        0     3616 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/proxy/structs.py
+-rw-r--r--   0        0        0      580 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/proxy/templates/haproxy.cfg.j2
+-rw-r--r--   0        0        0     1511 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/proxy/utils.py
+-rw-r--r--   0        0        0    84573 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/resources.py
+-rw-r--r--   0        0        0     1492 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/service.py
+-rw-r--r--   0        0        0     3124 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/tests/functional/conftest.py
+-rw-r--r--   0        0        0      666 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/tests/functional/test_clusters.py
+-rw-r--r--   0        0        0      942 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/conftest.py
+-rw-r--r--   0        0        0     6504 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_helm.py
+-rw-r--r--   0        0        0     1731 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_image_utils.py
+-rw-r--r--   0        0        0     3105 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_images.py
+-rw-r--r--   0        0        0     5366 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_objects.py
+-rw-r--r--   0        0        0     1735 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_resources.py
+-rw-r--r--   0        0        0     1192 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_utils.py
+-rw-r--r--   0        0        0     8746 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/utils.py
+-rw-r--r--   0        0        0     1333 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     4551 1970-01-01 00:00:00.000000 magnum_cluster_api-0.8.1/PKG-INFO
```

### Comparing `magnum_cluster_api-0.8.0/LICENSE` & `magnum_cluster_api-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/README.md` & `magnum_cluster_api-0.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
    ```
 
 1. Upload an image to use with Magnum and create cluster templates
 
    ```bash
    pushd /tmp
    source /opt/stack/openrc
-   for version in v1.23.13 v1.24.7 v1.25.3; do \
+   for version in v1.23.17 v1.24.15 v1.25.11 v1.26.6 v1.27.3; do \
       curl -LO https://object-storage.public.mtl1.vexxhost.net/swift/v1/a91f106f55e64246babde7402c21b87a/magnum-capi/ubuntu-2204-kube-${version}.qcow2; \
       openstack image create ubuntu-2204-kube-${version} --disk-format=qcow2 --container-format=bare --property os_distro=ubuntu --file=ubuntu-2204-kube-${version}.qcow2; \
       openstack coe cluster template create \
          --image $(openstack image show ubuntu-2204-kube-${version} -c id -f value) \
          --external-network public \
          --dns-nameserver 8.8.8.8 \
          --master-lb-enabled \
@@ -61,25 +61,25 @@
          --flavor m1.medium \
          --network-driver calico \
          --docker-storage-driver overlay2 \
          --coe kubernetes \
          --label kube_tag=${version} \
          k8s-${version};
    done;
-   popd /tmp
+   popd
    ```
 
 1. Spin up a new cluster using the Cluster API driver
 
    ```bash
    openstack coe cluster create \
-     --cluster-template k8s-v1.25.3 \
+     --cluster-template k8s-v1.25.11 \
      --master-count 3 \
      --node-count 2 \
-     k8s-v1.25.3
+     k8s-v1.25.11
    ```
 
 1. Once the cluster reaches `CREATE_COMPLETE` state, you can interact with it:
 
    ```bash
-   eval $(openstack coe cluster config k8s-cluster)
+   eval $(openstack coe cluster config k8s-v1.25.11)
    ```
```

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/README.md` & `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/README.md`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl` & `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt` & `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl` & `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/values.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/values.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/clients.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/clients.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/cmd/image_builder.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/cmd/image_builder.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/cmd/proxy.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/cmd/proxy.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/conf.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/conf.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/driver.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,17 @@
                         "cluster.x-k8s.io/delete-machine"
                     ] = "yes"
                     machine.update()
 
         nodegroup.node_count = node_count
         nodegroup.save()
 
-        resources.apply_cluster_from_magnum_cluster(context, self.k8s_api, cluster)
+        resources.apply_cluster_from_magnum_cluster(
+            context, self.k8s_api, cluster, skip_auto_scaling_release=True
+        )
 
     def upgrade_cluster(
         self,
         context,
         cluster: magnum_objects.Cluster,
         cluster_template: magnum_objects.ClusterTemplate,
         max_batch_size,
@@ -266,15 +268,17 @@
 
         resources.ClusterResourceSet(self.k8s_api, cluster).delete()
         resources.ClusterResourcesConfigMap(context, self.k8s_api, cluster).delete()
         resources.Cluster(context, self.k8s_api, cluster).delete()
         resources.ClusterAutoscalerHelmRelease(self.k8s_api, cluster).delete()
 
     def create_nodegroup(self, context, cluster, nodegroup):
-        resources.apply_cluster_from_magnum_cluster(context, self.k8s_api, cluster)
+        resources.apply_cluster_from_magnum_cluster(
+            context, self.k8s_api, cluster, skip_auto_scaling_release=True
+        )
 
     def update_nodegroup_status(self, context, cluster, nodegroup):
         action = nodegroup.status.split("_")[0]
 
         if nodegroup.role == "master":
             kcp = resources.get_kubeadm_control_plane(self.k8s_api, cluster)
             if kcp is None:
@@ -319,29 +323,32 @@
 
     def update_nodegroup(self, context, cluster, nodegroup):
         # TODO
 
         # NOTE(okozachenko1203): First we save the nodegroup status because update_cluster_status()
         #                        could be finished before update_nodegroup().
         nodegroup.save()
-        resources.apply_cluster_from_magnum_cluster(context, self.k8s_api, cluster)
+        resources.apply_cluster_from_magnum_cluster(
+            context, self.k8s_api, cluster, skip_auto_scaling_release=True
+        )
         # NOTE(okozachenko1203): We set the cluster status as UPDATE_IN_PROGRESS again at the end because
         #                        update_cluster_status() could be finished and cluster status has been set as
         #                        UPDATE_COMPLETE before nodegroup_conductor.Handler.nodegroup_update finished.
         cluster.status = "UPDATE_IN_PROGRESS"
         cluster.save()
 
     def delete_nodegroup(self, context, cluster, nodegroup):
         nodegroup.status = "DELETE_IN_PROGRESS"
         nodegroup.save()
 
         resources.apply_cluster_from_magnum_cluster(
             context,
             self.k8s_api,
             cluster,
+            skip_auto_scaling_release=True,
         )
 
     def get_monitor(self, context, cluster):
         return monitor.Monitor(context, cluster)
 
     # def rotate_ca_certificate(self, context, cluster):
     #     raise exception.NotSupported(
```

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/exceptions.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/helm.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/helm.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,20 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import yaml
 from oslo_concurrency import processutils
+from oslo_log import log as logging
 
 from magnum_cluster_api import exceptions
 
+LOG = logging.getLogger(__name__)
+
 
 class Command:
     def __call__(self, *args, **kwargs):
         return processutils.execute("helm", *self.COMMAND, *args, **kwargs)
 
 
 class VersionCommand(Command):
@@ -54,55 +57,38 @@
         except processutils.ProcessExecutionError as e:
             if "release: not found" in e.stderr:
                 raise exceptions.HelmReleaseNotFound(self.release_name)
             else:
                 raise
 
 
-class GetStatusReleaseCommand(ReleaseCommand):
-    COMMAND = ["status"]
-
-    def __call__(self):
-        try:
-            return super().__call__()
-        except processutils.ProcessExecutionError as e:
-            if "release: not found" in e.stderr:
-                raise exceptions.HelmReleaseNotFound(self.release_name)
-            else:
-                raise
-
-
 class UpgradeReleaseCommand(ReleaseCommand):
     COMMAND = ["upgrade"]
 
     def __init__(self, namespace, release_name, chart_ref, values={}):
         super().__init__(namespace, release_name)
         self.chart_ref = chart_ref
         self.values = values
 
     def __call__(self):
         try:
-            stdout, _ = GetStatusReleaseCommand(
-                namespace=self.namespace,
-                release_name=self.release_name,
-            )()
-
-            if "STATUS: pending" in stdout:
-                return "Other task is in progress"
-        except exceptions.HelmReleaseNotFound:
-            pass
-
-        return super().__call__(
-            self.chart_ref,
-            "--install",
-            "--wait",
-            "--values",
-            "-",
-            process_input=yaml.dump(self.values),
-        )
+            return super().__call__(
+                self.chart_ref,
+                "--install",
+                "--values",
+                "-",
+                process_input=yaml.dump(self.values),
+            )
+        except processutils.ProcessExecutionError as e:
+            if "UPGRADE FAILED: another operation" in e.stderr:
+                LOG.info("Helm release %s is already in progress", self.release_name)
+            elif "UPGRADE FAILED: release: already exists" in e.stderr:
+                LOG.info("Helm release %s already exists", self.release_name)
+            else:
+                raise
 
 
 class DeleteReleaseCommand(ReleaseCommand):
     COMMAND = ["delete"]
 
     def __init__(self, namespace, release_name, skip_missing=False):
         super().__init__(namespace, release_name)
```

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/image_utils.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/image_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/images.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/images.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/integrations/cinder.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/integrations/cinder.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/integrations/cloud_provider.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/integrations/cloud_provider.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/integrations/common.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/integrations/common.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/integrations/manila.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/integrations/manila.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/audit/policy.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/audit/policy.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/calico/v3.24.2.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/calico/v3.24.2.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin-rbac.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin-rbac.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin-rbac.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin-rbac.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-controller.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/nfs-csi/csi-nfs-controller.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-node.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/nfs-csi/csi-nfs-node.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/nfs-csi/rbac-csi-nfs.yaml` & `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/nfs-csi/rbac-csi-nfs.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/monitor.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/monitor.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/objects.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/objects.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/privsep/__init__.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/privsep/__init__.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/privsep/haproxy.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/privsep/haproxy.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/proxy/manager.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/proxy/manager.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/proxy/structs.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/proxy/structs.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/proxy/templates/haproxy.cfg.j2` & `magnum_cluster_api-0.8.1/magnum_cluster_api/proxy/templates/haproxy.cfg.j2`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/proxy/utils.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/proxy/utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/resources.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1784,14 +1784,15 @@
 
 
 def apply_cluster_from_magnum_cluster(
     context: context.RequestContext,
     api: pykube.HTTPClient,
     cluster: magnum_objects.Cluster,
     cluster_template: magnum_objects.ClusterTemplate = None,
+    skip_auto_scaling_release: bool = False,
 ) -> objects.Cluster:
     """
     Create a ClusterAPI cluster given a Magnum Cluster object.
     """
     create_cluster_class(api)
 
     if cluster_template is None:
@@ -1810,15 +1811,16 @@
             ng.labels[label] = cluster_template.labels[label]
             ng.save()
     cluster.save()
 
     ClusterResourcesConfigMap(context, api, cluster).apply()
     ClusterResourceSet(api, cluster).apply()
     Cluster(context, api, cluster).apply()
-    if utils.get_auto_scaling_enabled(cluster):
+
+    if not skip_auto_scaling_release and utils.get_auto_scaling_enabled(cluster):
         ClusterAutoscalerHelmRelease(api, cluster).apply()
 
 
 def get_kubeadm_control_plane(
     api: pykube.HTTPClient, cluster: magnum_objects.Cluster
 ) -> objects.KubeadmControlPlane:
     kcps = objects.KubeadmControlPlane.objects(api, namespace="magnum-system").filter(
```

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/service.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/service.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/tests/functional/conftest.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/tests/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/tests/functional/test_clusters.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/tests/functional/test_clusters.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/conftest.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_image_utils.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_images.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_images.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_objects.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_objects.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_resources.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_resources.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_utils.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/magnum_cluster_api/utils.py` & `magnum_cluster_api-0.8.1/magnum_cluster_api/utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.0/pyproject.toml` & `magnum_cluster_api-0.8.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magnum-cluster-api"
-version = "0.8.0"
+version = "0.8.1"
 description = "Cluster API driver for Magnum"
 authors = ["Mohammed Naser <mnaser@vexxhost.com>"]
 readme = "README.md"
 packages = [{include = "magnum_cluster_api"}]
 include = ["magnum_cluster_api/charts/**/*"]
 
 [tool.poetry.dependencies]
@@ -20,14 +20,16 @@
 pykube-ng = "*"
 pyroute2 = ">=0.3.4"
 python = "^3.6"
 "python-manilaclient" = ">=3.3.2"
 requests = ">=2.27.1"
 semver = "^2.0.0"
 shortuuid = "*"
+diskcache = "^5.6.1"
+platformdirs = "^2.4.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "<7"
 pytest-mock = "^3.6.1"
 
 [build-system]
 requires = ["setuptools", "poetry-core"]
```

### Comparing `magnum_cluster_api-0.8.0/PKG-INFO` & `magnum_cluster_api-0.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: magnum-cluster-api
-Version: 0.8.0
+Version: 0.8.1
 Summary: Cluster API driver for Magnum
 Author: Mohammed Naser
 Author-email: mnaser@vexxhost.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: certifi
 Requires-Dist: click (>=8.0.4)
+Requires-Dist: diskcache (>=5.6.1,<6.0.0)
 Requires-Dist: magnum (>=14.0.0)
 Requires-Dist: oslo.concurrency (>=4.5.0)
 Requires-Dist: oslo.config (>=8.8.0)
 Requires-Dist: oslo.context (>=4.1.0)
 Requires-Dist: oslo.log (>=4.7.0)
 Requires-Dist: oslo.privsep (>=2.7.0)
 Requires-Dist: oslo.service (>=2.8.0)
+Requires-Dist: platformdirs (>=2.4.0,<3.0.0)
 Requires-Dist: pykube-ng
 Requires-Dist: pyroute2 (>=0.3.4)
 Requires-Dist: python-manilaclient (>=3.3.2)
 Requires-Dist: requests (>=2.27.1)
 Requires-Dist: semver (>=2.0.0,<3.0.0)
 Requires-Dist: shortuuid
 Description-Content-Type: text/markdown
@@ -76,15 +78,15 @@
    ```
 
 1. Upload an image to use with Magnum and create cluster templates
 
    ```bash
    pushd /tmp
    source /opt/stack/openrc
-   for version in v1.23.13 v1.24.7 v1.25.3; do \
+   for version in v1.23.17 v1.24.15 v1.25.11 v1.26.6 v1.27.3; do \
       curl -LO https://object-storage.public.mtl1.vexxhost.net/swift/v1/a91f106f55e64246babde7402c21b87a/magnum-capi/ubuntu-2204-kube-${version}.qcow2; \
       openstack image create ubuntu-2204-kube-${version} --disk-format=qcow2 --container-format=bare --property os_distro=ubuntu --file=ubuntu-2204-kube-${version}.qcow2; \
       openstack coe cluster template create \
          --image $(openstack image show ubuntu-2204-kube-${version} -c id -f value) \
          --external-network public \
          --dns-nameserver 8.8.8.8 \
          --master-lb-enabled \
@@ -92,26 +94,26 @@
          --flavor m1.medium \
          --network-driver calico \
          --docker-storage-driver overlay2 \
          --coe kubernetes \
          --label kube_tag=${version} \
          k8s-${version};
    done;
-   popd /tmp
+   popd
    ```
 
 1. Spin up a new cluster using the Cluster API driver
 
    ```bash
    openstack coe cluster create \
-     --cluster-template k8s-v1.25.3 \
+     --cluster-template k8s-v1.25.11 \
      --master-count 3 \
      --node-count 2 \
-     k8s-v1.25.3
+     k8s-v1.25.11
    ```
 
 1. Once the cluster reaches `CREATE_COMPLETE` state, you can interact with it:
 
    ```bash
-   eval $(openstack coe cluster config k8s-cluster)
+   eval $(openstack coe cluster config k8s-v1.25.11)
    ```
```

