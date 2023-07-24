# Comparing `tmp/magnum_cluster_api-0.8.1.tar.gz` & `tmp/magnum_cluster_api-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnum_cluster_api-0.8.1.tar", max compression
+gzip compressed data, was "magnum_cluster_api-0.9.0.tar", max compression
```

## Comparing `magnum_cluster_api-0.8.1.tar` & `magnum_cluster_api-0.9.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0    10142 2023-07-07 03:54:37.672372 magnum_cluster_api-0.8.1/LICENSE
--rw-r--r--   0        0        0     3369 2023-07-07 03:54:37.672372 magnum_cluster_api-0.8.1/README.md
--rw-r--r--   0        0        0        0 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/.gitkeep
--rw-r--r--   0        0        0      349 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/.helmignore
--rw-r--r--   0        0        0      437 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/Chart.yaml
--rw-r--r--   0        0        0    29122 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/README.md
--rw-r--r--   0        0        0    14987 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl
--rw-r--r--   0        0        0      827 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt
--rw-r--r--   0        0        0     4034 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl
--rw-r--r--   0        0        0     2982 2023-07-07 03:54:41.956405 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml
--rw-r--r--   0        0        0      534 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml
--rw-r--r--   0        0        0    13204 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml
--rw-r--r--   0        0        0      508 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/pdb.yaml
--rw-r--r--   0        0        0      972 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml
--rw-r--r--   0        0        0      758 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml
--rw-r--r--   0        0        0      564 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml
--rw-r--r--   0        0        0     1807 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml
--rw-r--r--   0        0        0      527 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml
--rw-r--r--   0        0        0      989 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml
--rw-r--r--   0        0        0     1180 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml
--rw-r--r--   0        0        0      528 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml
--rw-r--r--   0        0        0      960 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml
--rw-r--r--   0        0        0      663 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml
--rw-r--r--   0        0        0    18003 2023-07-07 03:54:41.876404 magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/values.yaml
--rw-r--r--   0        0        0     1977 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/clients.py
--rw-r--r--   0        0        0        0 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/cmd/__init__.py
--rw-r--r--   0        0        0     5005 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/cmd/image_builder.py
--rw-r--r--   0        0        0     6891 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/cmd/image_loader.py
--rw-r--r--   0        0        0      956 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/cmd/proxy.py
--rw-r--r--   0        0        0     3460 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/conf.py
--rw-r--r--   0        0        0    14323 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/driver.py
--rw-r--r--   0        0        0     1219 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/exceptions.py
--rw-r--r--   0        0        0     3276 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/helm.py
--rw-r--r--   0        0        0     3460 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/image_utils.py
--rw-r--r--   0        0        0     1116 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/images.py
--rw-r--r--   0        0        0        0 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/integrations/__init__.py
--rw-r--r--   0        0        0     1759 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/integrations/cinder.py
--rw-r--r--   0        0        0      839 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/integrations/cloud_provider.py
--rw-r--r--   0        0        0     3012 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/integrations/common.py
--rw-r--r--   0        0        0      948 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/integrations/manila.py
--rw-r--r--   0        0        0        0 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/__init__.py
--rw-r--r--   0        0        0     4941 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/audit/policy.yaml
--rw-r--r--   0        0        0   235191 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/calico/v3.24.2.yaml
--rw-r--r--   0        0        0      623 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml
--rw-r--r--   0        0        0     1430 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml
--rw-r--r--   0        0        0     2263 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml
--rw-r--r--   0        0        0     4506 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin-rbac.yaml
--rw-r--r--   0        0        0     4034 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin.yaml
--rw-r--r--   0        0        0      609 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin-rbac.yaml
--rw-r--r--   0        0        0     3307 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin.yaml
--rw-r--r--   0        0        0      194 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/cinder-csi/csi-cinder-driver.yaml
--rw-r--r--   0        0        0     3377 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin-rbac.yaml
--rw-r--r--   0        0        0     3944 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin.yaml
--rw-r--r--   0        0        0     1513 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin-rbac.yaml
--rw-r--r--   0        0        0     2988 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin.yaml
--rw-r--r--   0        0        0      143 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/manila-csi/csidriver.yaml
--rw-r--r--   0        0        0     3127 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/nfs-csi/csi-nfs-controller.yaml
--rw-r--r--   0        0        0      170 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/nfs-csi/csi-nfs-driverinfo.yaml
--rw-r--r--   0        0        0     3530 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/nfs-csi/csi-nfs-node.yaml
--rw-r--r--   0        0        0     1423 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/nfs-csi/rbac-csi-nfs.yaml
--rw-r--r--   0        0        0     1526 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/monitor.py
--rw-r--r--   0        0        0     5673 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/objects.py
--rw-r--r--   0        0        0      828 2023-07-07 03:54:37.676372 magnum_cluster_api-0.8.1/magnum_cluster_api/privsep/__init__.py
--rw-r--r--   0        0        0     1333 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/privsep/haproxy.py
--rw-r--r--   0        0        0    11719 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/proxy/manager.py
--rw-r--r--   0        0        0     3616 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/proxy/structs.py
--rw-r--r--   0        0        0      580 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/proxy/templates/haproxy.cfg.j2
--rw-r--r--   0        0        0     1511 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/proxy/utils.py
--rw-r--r--   0        0        0    84573 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/resources.py
--rw-r--r--   0        0        0     1492 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/service.py
--rw-r--r--   0        0        0     3124 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/tests/functional/conftest.py
--rw-r--r--   0        0        0      666 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/tests/functional/test_clusters.py
--rw-r--r--   0        0        0      942 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/conftest.py
--rw-r--r--   0        0        0     6504 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_helm.py
--rw-r--r--   0        0        0     1731 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_image_utils.py
--rw-r--r--   0        0        0     3105 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_images.py
--rw-r--r--   0        0        0     5366 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_objects.py
--rw-r--r--   0        0        0     1735 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_resources.py
--rw-r--r--   0        0        0     1192 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_utils.py
--rw-r--r--   0        0        0     8746 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/magnum_cluster_api/utils.py
--rw-r--r--   0        0        0     1333 2023-07-07 03:54:37.680372 magnum_cluster_api-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     4551 1970-01-01 00:00:00.000000 magnum_cluster_api-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-07-24 16:45:25.134403 magnum_cluster_api-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3369 2023-07-24 16:45:25.134403 magnum_cluster_api-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-24 16:45:25.134403 magnum_cluster_api-0.9.0/magnum_cluster_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 16:45:25.134403 magnum_cluster_api-0.9.0/magnum_cluster_api/charts/.gitkeep
+-rw-r--r--   0        0        0      349 2023-07-24 16:45:28.674498 magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/.helmignore
+-rw-r--r--   0        0        0      437 2023-07-24 16:45:28.674498 magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/Chart.yaml
+-rw-r--r--   0        0        0    29122 2023-07-24 16:45:28.674498 magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/README.md
+-rw-r--r--   0        0        0    14987 2023-07-24 16:45:28.674498 magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl
+-rw-r--r--   0        0        0      827 2023-07-24 16:45:28.674498 magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt
+-rw-r--r--   0        0        0     4034 2023-07-24 16:45:28.674498 magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl
+-rw-r--r--   0        0        0     2982 2023-07-24 16:45:28.706499 magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml
+-rw-r--r--   0        0        0      534 2023-07-24 16:45:28.674498 magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml
+-rw-r--r--   0        0        0    13204 2023-07-24 16:45:28.674498 magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml
+-rw-r--r--   0        0        0      508 2023-07-24 16:45:28.674498 magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/pdb.yaml
+-rw-r--r--   0        0        0      972 2023-07-24 16:45:28.674498 magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml
+-rw-r--r--   0        0        0      758 2023-07-24 16:45:28.674498 magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml
+-rw-r--r--   0        0        0      564 2023-07-24 16:45:28.674498 magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml
+-rw-r--r--   0        0        0     1807 2023-07-24 16:45:28.674498 magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml
+-rw-r--r--   0        0        0      527 2023-07-24 16:45:28.674498 magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml
+-rw-r--r--   0        0        0      989 2023-07-24 16:45:28.674498 magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml
+-rw-r--r--   0        0        0     1180 2023-07-24 16:45:28.674498 magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml
+-rw-r--r--   0        0        0      528 2023-07-24 16:45:28.674498 magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0      960 2023-07-24 16:45:28.674498 magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml
+-rw-r--r--   0        0        0      663 2023-07-24 16:45:28.674498 magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml
+-rw-r--r--   0        0        0    18003 2023-07-24 16:45:28.674498 magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/values.yaml
+-rw-r--r--   0        0        0     1977 2023-07-24 16:45:25.134403 magnum_cluster_api-0.9.0/magnum_cluster_api/clients.py
+-rw-r--r--   0        0        0        0 2023-07-24 16:45:25.134403 magnum_cluster_api-0.9.0/magnum_cluster_api/cmd/__init__.py
+-rw-r--r--   0        0        0     5005 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/cmd/image_builder.py
+-rw-r--r--   0        0        0     6946 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/cmd/image_loader.py
+-rw-r--r--   0        0        0      956 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/cmd/proxy.py
+-rw-r--r--   0        0        0     3460 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/conf.py
+-rw-r--r--   0        0        0    14601 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/driver.py
+-rw-r--r--   0        0        0     1419 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/exceptions.py
+-rw-r--r--   0        0        0     3276 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/helm.py
+-rw-r--r--   0        0        0     3460 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/image_utils.py
+-rw-r--r--   0        0        0     1116 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/images.py
+-rw-r--r--   0        0        0        0 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/integrations/__init__.py
+-rw-r--r--   0        0        0     1759 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/integrations/cinder.py
+-rw-r--r--   0        0        0      839 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/integrations/cloud_provider.py
+-rw-r--r--   0        0        0     3012 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/integrations/common.py
+-rw-r--r--   0        0        0      948 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/integrations/manila.py
+-rw-r--r--   0        0        0        0 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/__init__.py
+-rw-r--r--   0        0        0     4941 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/audit/policy.yaml
+-rw-r--r--   0        0        0   235191 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/calico/v3.24.2.yaml
+-rw-r--r--   0        0        0      623 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml
+-rw-r--r--   0        0        0     1430 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml
+-rw-r--r--   0        0        0     2263 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml
+-rw-r--r--   0        0        0     4506 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin-rbac.yaml
+-rw-r--r--   0        0        0     4034 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin.yaml
+-rw-r--r--   0        0        0      609 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin-rbac.yaml
+-rw-r--r--   0        0        0     3307 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin.yaml
+-rw-r--r--   0        0        0      194 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/cinder-csi/csi-cinder-driver.yaml
+-rw-r--r--   0        0        0     3377 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin-rbac.yaml
+-rw-r--r--   0        0        0     3944 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin.yaml
+-rw-r--r--   0        0        0     1513 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin-rbac.yaml
+-rw-r--r--   0        0        0     2988 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin.yaml
+-rw-r--r--   0        0        0      143 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/manila-csi/csidriver.yaml
+-rw-r--r--   0        0        0     3127 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-controller.yaml
+-rw-r--r--   0        0        0      170 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-driverinfo.yaml
+-rw-r--r--   0        0        0     3530 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-node.yaml
+-rw-r--r--   0        0        0     1423 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/nfs-csi/rbac-csi-nfs.yaml
+-rw-r--r--   0        0        0     1526 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/monitor.py
+-rw-r--r--   0        0        0     5673 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/objects.py
+-rw-r--r--   0        0        0      828 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/privsep/__init__.py
+-rw-r--r--   0        0        0     1333 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/privsep/haproxy.py
+-rw-r--r--   0        0        0    11719 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/proxy/manager.py
+-rw-r--r--   0        0        0     3616 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/proxy/structs.py
+-rw-r--r--   0        0        0      580 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/proxy/templates/haproxy.cfg.j2
+-rw-r--r--   0        0        0     1511 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/proxy/utils.py
+-rw-r--r--   0        0        0    85939 2023-07-24 16:45:25.138403 magnum_cluster_api-0.9.0/magnum_cluster_api/resources.py
+-rw-r--r--   0        0        0     1492 2023-07-24 16:45:25.142403 magnum_cluster_api-0.9.0/magnum_cluster_api/service.py
+-rw-r--r--   0        0        0     3124 2023-07-24 16:45:25.142403 magnum_cluster_api-0.9.0/magnum_cluster_api/tests/functional/conftest.py
+-rw-r--r--   0        0        0      666 2023-07-24 16:45:25.142403 magnum_cluster_api-0.9.0/magnum_cluster_api/tests/functional/test_clusters.py
+-rw-r--r--   0        0        0      942 2023-07-24 16:45:25.142403 magnum_cluster_api-0.9.0/magnum_cluster_api/tests/unit/conftest.py
+-rw-r--r--   0        0        0     6504 2023-07-24 16:45:25.142403 magnum_cluster_api-0.9.0/magnum_cluster_api/tests/unit/test_helm.py
+-rw-r--r--   0        0        0     1731 2023-07-24 16:45:25.142403 magnum_cluster_api-0.9.0/magnum_cluster_api/tests/unit/test_image_utils.py
+-rw-r--r--   0        0        0     3105 2023-07-24 16:45:25.142403 magnum_cluster_api-0.9.0/magnum_cluster_api/tests/unit/test_images.py
+-rw-r--r--   0        0        0     5366 2023-07-24 16:45:25.142403 magnum_cluster_api-0.9.0/magnum_cluster_api/tests/unit/test_objects.py
+-rw-r--r--   0        0        0     1735 2023-07-24 16:45:25.142403 magnum_cluster_api-0.9.0/magnum_cluster_api/tests/unit/test_resources.py
+-rw-r--r--   0        0        0     1192 2023-07-24 16:45:25.142403 magnum_cluster_api-0.9.0/magnum_cluster_api/tests/unit/test_utils.py
+-rw-r--r--   0        0        0     9600 2023-07-24 16:45:25.142403 magnum_cluster_api-0.9.0/magnum_cluster_api/utils.py
+-rw-r--r--   0        0        0     1335 2023-07-24 16:45:25.142403 magnum_cluster_api-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4537 1970-01-01 00:00:00.000000 magnum_cluster_api-0.9.0/PKG-INFO
```

### Comparing `magnum_cluster_api-0.8.1/LICENSE` & `magnum_cluster_api-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/README.md` & `magnum_cluster_api-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/README.md` & `magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/README.md`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl` & `magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt` & `magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl` & `magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/charts/cluster-autoscaler/values.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/charts/cluster-autoscaler/values.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/clients.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/clients.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/cmd/image_builder.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/cmd/image_builder.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/cmd/image_loader.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/cmd/image_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,17 @@
         f.write(r.content)
         f.close()
 
         # Make it executable
         os.chmod(f.name, 0o755)
 
         # Run the command
-        output = subprocess.check_output([f.name, "config", "images", "list"])
+        output = subprocess.check_output(
+            [f.name, "config", "images", "list", "--kubernetes-version", version]
+        )
 
         # Remove the temporary file
         os.unlink(f.name)
 
     # Parse the output
     return output.decode().replace("k8s.gcr.io", "registry.k8s.io").splitlines()
```

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/cmd/proxy.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/cmd/proxy.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/conf.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/conf.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/driver.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     def create_cluster(self, context, cluster, cluster_create_timeout):
         # NOTE(mnaser): We want to set the `stack_id` as early as possible to
         #               make sure we can use it in the cluster creation.
         cluster.stack_id = utils.generate_cluster_api_name(self.k8s_api)
         cluster.save()
 
-        utils.validate_cluster(cluster)
+        utils.validate_cluster(cluster, context)
 
         osc = clients.get_openstack_api(context)
 
         resources.Namespace(self.k8s_api).apply()
 
         credential = osc.keystone().client.application_credentials.create(
             user=cluster.user_id,
@@ -47,19 +47,21 @@
             self.k8s_api,
             cluster,
             osc.url_for(service_type="identity", interface="public"),
             osc.cinder_region_name(),
             credential,
         ).apply()
 
-        resources.ApiCertificateAuthoritySecret(self.k8s_api, cluster).apply()
-        resources.EtcdCertificateAuthoritySecret(self.k8s_api, cluster).apply()
-        resources.FrontProxyCertificateAuthoritySecret(self.k8s_api, cluster).apply()
+        resources.ApiCertificateAuthoritySecret(context, self.k8s_api, cluster).apply()
+        resources.EtcdCertificateAuthoritySecret(context, self.k8s_api, cluster).apply()
+        resources.FrontProxyCertificateAuthoritySecret(
+            context, self.k8s_api, cluster
+        ).apply()
         resources.ServiceAccountCertificateAuthoritySecret(
-            self.k8s_api, cluster
+            context, self.k8s_api, cluster
         ).apply()
 
         resources.apply_cluster_from_magnum_cluster(context, self.k8s_api, cluster)
 
     def _get_cluster_status_reason(self, capi_cluster):
         capi_cluster_status_reason = ""
         capi_ops_cluster_status_reason = ""
@@ -153,21 +155,25 @@
                     name=cluster.uuid,
                     user=cluster.user_id,
                 ).delete()
             except keystoneauth1.exceptions.http.NotFound:
                 pass
 
             resources.CloudConfigSecret(self.k8s_api, cluster).delete()
-            resources.ApiCertificateAuthoritySecret(self.k8s_api, cluster).delete()
-            resources.EtcdCertificateAuthoritySecret(self.k8s_api, cluster).delete()
+            resources.ApiCertificateAuthoritySecret(
+                context, self.k8s_api, cluster
+            ).delete()
+            resources.EtcdCertificateAuthoritySecret(
+                context, self.k8s_api, cluster
+            ).delete()
             resources.FrontProxyCertificateAuthoritySecret(
-                self.k8s_api, cluster
+                context, self.k8s_api, cluster
             ).delete()
             resources.ServiceAccountCertificateAuthoritySecret(
-                self.k8s_api, cluster
+                context, self.k8s_api, cluster
             ).delete()
 
             cluster.status_reason = None
             cluster.status = "DELETE_COMPLETE"
             cluster.save()
 
     def update_cluster(self, context, cluster, scale_manager=None, rollback=False):
@@ -178,15 +184,15 @@
         context,
         cluster,
         resize_manager,
         node_count,
         nodes_to_remove,
         nodegroup=None,
     ):
-        utils.validate_cluster(cluster)
+        utils.validate_cluster(cluster, context)
 
         if nodegroup is None:
             nodegroup = cluster.default_ng_worker
 
         if nodes_to_remove:
             machines = objects.Machine.objects(self.k8s_api).filter(
                 namespace="magnum-system",
@@ -268,14 +274,15 @@
 
         resources.ClusterResourceSet(self.k8s_api, cluster).delete()
         resources.ClusterResourcesConfigMap(context, self.k8s_api, cluster).delete()
         resources.Cluster(context, self.k8s_api, cluster).delete()
         resources.ClusterAutoscalerHelmRelease(self.k8s_api, cluster).delete()
 
     def create_nodegroup(self, context, cluster, nodegroup):
+        utils.validate_nodegroup(nodegroup, context)
         resources.apply_cluster_from_magnum_cluster(
             context, self.k8s_api, cluster, skip_auto_scaling_release=True
         )
 
     def update_nodegroup_status(self, context, cluster, nodegroup):
         action = nodegroup.status.split("_")[0]
 
@@ -323,14 +330,15 @@
 
     def update_nodegroup(self, context, cluster, nodegroup):
         # TODO
 
         # NOTE(okozachenko1203): First we save the nodegroup status because update_cluster_status()
         #                        could be finished before update_nodegroup().
         nodegroup.save()
+        utils.validate_nodegroup(nodegroup, context)
         resources.apply_cluster_from_magnum_cluster(
             context, self.k8s_api, cluster, skip_auto_scaling_release=True
         )
         # NOTE(okozachenko1203): We set the cluster status as UPDATE_IN_PROGRESS again at the end because
         #                        update_cluster_status() could be finished and cluster status has been set as
         #                        UPDATE_COMPLETE before nodegroup_conductor.Handler.nodegroup_update finished.
         cluster.status = "UPDATE_IN_PROGRESS"
```

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/exceptions.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 
+from magnum.common import exception
+from magnum.i18n import _
+
+
 class HelmException(Exception):
     pass
 
 
 class HelmReleaseNotFound(HelmException):
     pass
 
@@ -47,7 +51,11 @@
 
 class ClusterAPIReconcileTimeout(Exception):
     pass
 
 
 class ClusterMasterCountEven(Exception):
     pass
+
+
+class OpenstackFlavorInvalidName(exception.InvalidName):
+    message = _("Expected a flavor name but received flavor id %(flavor)s.")
```

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/helm.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/helm.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/image_utils.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/image_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/images.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/images.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/integrations/cinder.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/integrations/cinder.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/integrations/cloud_provider.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/integrations/cloud_provider.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/integrations/common.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/integrations/common.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/integrations/manila.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/integrations/manila.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/audit/policy.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/audit/policy.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/calico/v3.24.2.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/calico/v3.24.2.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin-rbac.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin-rbac.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin-rbac.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin-rbac.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/nfs-csi/csi-nfs-controller.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-controller.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/nfs-csi/csi-nfs-node.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-node.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/manifests/nfs-csi/rbac-csi-nfs.yaml` & `magnum_cluster_api-0.9.0/magnum_cluster_api/manifests/nfs-csi/rbac-csi-nfs.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/monitor.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/monitor.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/objects.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/objects.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/privsep/__init__.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/privsep/__init__.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/privsep/haproxy.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/privsep/haproxy.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/proxy/manager.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/proxy/manager.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/proxy/structs.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/proxy/structs.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/proxy/templates/haproxy.cfg.j2` & `magnum_cluster_api-0.9.0/magnum_cluster_api/proxy/templates/haproxy.cfg.j2`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/proxy/utils.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/proxy/utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/resources.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,19 @@
 import types
 
 import certifi
 import pkg_resources
 import pykube
 import yaml
 from magnum import objects as magnum_objects
-from magnum.common import cert_manager, context, neutron
+from magnum.common import context, neutron
 from magnum.common import utils as magnum_utils
+from magnum.common.cert_manager import cert_manager
 from magnum.common.x509 import operations as x509
+from magnum.conductor.handlers.common import cert_manager as cert_manager_handlers
 from oslo_config import cfg
 from oslo_serialization import base64
 from oslo_utils import encodeutils
 
 from magnum_cluster_api import clients, helm, image_utils, images, objects, utils
 from magnum_cluster_api.integrations import cinder, cloud_provider, manila
 
@@ -374,33 +376,38 @@
                     ],
                 },
             },
         )
 
 
 class CertificateAuthoritySecret(ClusterBase):
+    def __init__(
+        self, context: context.RequestContext, api: pykube.HTTPClient, cluster: any
+    ):
+        super().__init__(api, cluster)
+        self.context = context
+
     def delete(self) -> None:
         resource = self.get_or_none()
         if resource:
             resource.delete()
 
     def get_or_none(self) -> pykube.Secret:
         return pykube.Secret.objects(self.api, namespace="magnum-system").get_or_none(
             name=f"{self.cluster.stack_id}-{self.CERT}"
         )
 
+    def get_certificate(self) -> cert_manager.Cert:
+        raise NotImplementedError()
+
     def get_object(self) -> pykube.Secret:
         cert_ref = getattr(self.cluster, self.REF)
         if cert_ref is None:
             raise Exception("Certificate for %s doesn't exist." % self.REF)
-
-        ca_cert = cert_manager.get_backend().CertManager.get_cert(
-            cert_ref,
-            resource_ref=self.cluster.uuid,
-        )
+        ca_cert = self.get_certificate()
 
         return pykube.Secret(
             self.api,
             {
                 "apiVersion": pykube.Secret.version,
                 "kind": pykube.Secret.kind,
                 "type": "kubernetes.io/tls",
@@ -421,29 +428,47 @@
         )
 
 
 class ApiCertificateAuthoritySecret(CertificateAuthoritySecret):
     CERT = "ca"
     REF = "ca_cert_ref"
 
+    def get_certificate(self) -> cert_manager.Cert:
+        return cert_manager_handlers.get_cluster_ca_certificate(
+            self.cluster, self.context, "kubernetes"
+        )
+
 
 class EtcdCertificateAuthoritySecret(CertificateAuthoritySecret):
     CERT = "etcd"
     REF = "etcd_ca_cert_ref"
 
+    def get_certificate(self) -> cert_manager.Cert:
+        return cert_manager_handlers.get_cluster_ca_certificate(
+            self.cluster, self.context, "etcd"
+        )
+
 
 class FrontProxyCertificateAuthoritySecret(CertificateAuthoritySecret):
     CERT = "proxy"
     REF = "front_proxy_ca_cert_ref"
 
+    def get_certificate(self) -> cert_manager.Cert:
+        return cert_manager_handlers.get_cluster_ca_certificate(
+            self.cluster, self.context, "front-proxy"
+        )
+
 
 class ServiceAccountCertificateAuthoritySecret(CertificateAuthoritySecret):
     CERT = "sa"
     REF = "magnum_cert_ref"
 
+    def get_certificate(self) -> cert_manager.Cert:
+        return cert_manager_handlers.get_cluster_magnum_cert(self.cluster, self.context)
+
 
 class CloudConfigSecret(ClusterBase):
     def __init__(
         self,
         api: pykube.HTTPClient,
         cluster: any,
         auth_url: str = None,
@@ -665,15 +690,15 @@
                             "ref": {
                                 "apiVersion": objects.OpenStackMachineTemplate.version,
                                 "kind": objects.OpenStackMachineTemplate.kind,
                                 "name": CLUSTER_CLASS_NAME,
                             },
                         },
                         "machineHealthCheck": {
-                            "maxUnhealthy": "33%",
+                            "maxUnhealthy": "80%",
                             "unhealthyConditions": [
                                 {
                                     "type": "Ready",
                                     "status": "False",
                                     "timeout": "5m",
                                 },
                                 {
@@ -708,15 +733,15 @@
                                             "apiVersion": objects.OpenStackMachineTemplate.version,
                                             "kind": objects.OpenStackMachineTemplate.kind,
                                             "name": CLUSTER_CLASS_NAME,
                                         }
                                     },
                                 },
                                 "machineHealthCheck": {
-                                    "maxUnhealthy": "33%",
+                                    "maxUnhealthy": "80%",
                                     "unhealthyConditions": [
                                         {
                                             "type": "Ready",
                                             "status": "False",
                                             "timeout": "5m",
                                         },
                                         {
@@ -1479,15 +1504,19 @@
             "class": "default-worker",
             "name": ng.name,
             "replicas": None if auto_scaling_enabled else ng.node_count,
             "metadata": {
                 "annotations": {
                     AUTOSCALE_ANNOTATION_MIN: f"{utils.get_node_group_min_node_count(ng)}",  # noqa: E501
                     AUTOSCALE_ANNOTATION_MAX: f"{utils.get_node_group_max_node_count(context, ng)}",  # noqa: E501
-                }
+                },
+                "labels": {
+                    f"node-role.kubernetes.io/{ng.role}": "",
+                    "node.cluster.x-k8s.io/nodegroup": ng.name,
+                },
             }
             if auto_scaling_enabled
             else {},
             "failureDomain": utils.get_cluster_label(cluster, "availability_zone", ""),
             "machineHealthCheck": {
                 "enable": utils.get_cluster_label_as_bool(
                     cluster, "auto_healing_enabled", True
@@ -1605,14 +1634,19 @@
                             ],
                         },
                     },
                     "topology": {
                         "class": CLUSTER_CLASS_NAME,
                         "version": utils.get_kube_tag(self.cluster),
                         "controlPlane": {
+                            "metadata": {
+                                "labels": {
+                                    "node-role.kubernetes.io/master": "",
+                                }
+                            },
                             "replicas": self.cluster.master_count,
                             "machineHealthCheck": {
                                 "enable": utils.get_cluster_label_as_bool(
                                     self.cluster, "auto_healing_enabled", True
                                 )
                             },
                         },
```

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/service.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/service.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/tests/functional/conftest.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/tests/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/tests/functional/test_clusters.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/tests/functional/test_clusters.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/conftest.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_helm.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/tests/unit/test_helm.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_image_utils.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/tests/unit/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_images.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/tests/unit/test_images.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_objects.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/tests/unit/test_objects.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_resources.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/tests/unit/test_resources.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/tests/unit/test_utils.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.8.1/magnum_cluster_api/utils.py` & `magnum_cluster_api-0.9.0/magnum_cluster_api/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -257,11 +257,37 @@
 def format_event_message(event: pykube.Event):
     return "%s: %s" % (
         event.obj["reason"],
         event.obj["message"],
     )
 
 
-def validate_cluster(cluster: magnum_objects.Cluster):
+def validate_flavor_name(cli: clients.OpenStackClients, flavor: str):
+    """Check if a flavor with this specified name exists"""
+
+    if flavor is None:
+        return
+    flavor_list = cli.nova().flavors.list()
+    for f in flavor_list:
+        if f.name == flavor:
+            return
+        if f.id == flavor:
+            raise mcapi_exceptions.OpenstackFlavorInvalidName(flavor=flavor)
+    raise exception.FlavorNotFound(flavor=flavor)
+
+
+def validate_cluster(cluster: magnum_objects.Cluster, ctx: context.RequestContext):
     # Check master count
     if (cluster.master_count % 2) == 0:
         raise mcapi_exceptions.ClusterMasterCountEven
+    # Validate flavors
+    osc = clients.get_openstack_api(ctx)
+    validate_flavor_name(osc, cluster.master_flavor_id)
+    validate_flavor_name(osc, cluster.flavor_id)
+
+
+def validate_nodegroup(
+    nodegroup: magnum_objects.NodeGroup, ctx: context.RequestContext
+):
+    # Validate flavors
+    osc = clients.get_openstack_api(ctx)
+    validate_flavor_name(osc, nodegroup.flavor_id)
```

### Comparing `magnum_cluster_api-0.8.1/pyproject.toml` & `magnum_cluster_api-0.9.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magnum-cluster-api"
-version = "0.8.1"
+version = "0.9.0"
 description = "Cluster API driver for Magnum"
 authors = ["Mohammed Naser <mnaser@vexxhost.com>"]
 readme = "README.md"
 packages = [{include = "magnum_cluster_api"}]
 include = ["magnum_cluster_api/charts/**/*"]
 
 [tool.poetry.dependencies]
@@ -20,16 +20,16 @@
 pykube-ng = "*"
 pyroute2 = ">=0.3.4"
 python = "^3.6"
 "python-manilaclient" = ">=3.3.2"
 requests = ">=2.27.1"
 semver = "^2.0.0"
 shortuuid = "*"
-diskcache = "^5.6.1"
-platformdirs = "^2.4.0"
+diskcache = ">=5.6.1"
+platformdirs = ">=2.4.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "<7"
 pytest-mock = "^3.6.1"
 
 [build-system]
 requires = ["setuptools", "poetry-core"]
```

### Comparing `magnum_cluster_api-0.8.1/PKG-INFO` & `magnum_cluster_api-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: magnum-cluster-api
-Version: 0.8.1
+Version: 0.9.0
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
-Requires-Dist: diskcache (>=5.6.1,<6.0.0)
+Requires-Dist: diskcache (>=5.6.1)
 Requires-Dist: magnum (>=14.0.0)
 Requires-Dist: oslo.concurrency (>=4.5.0)
 Requires-Dist: oslo.config (>=8.8.0)
 Requires-Dist: oslo.context (>=4.1.0)
 Requires-Dist: oslo.log (>=4.7.0)
 Requires-Dist: oslo.privsep (>=2.7.0)
 Requires-Dist: oslo.service (>=2.8.0)
-Requires-Dist: platformdirs (>=2.4.0,<3.0.0)
+Requires-Dist: platformdirs (>=2.4.0)
 Requires-Dist: pykube-ng
 Requires-Dist: pyroute2 (>=0.3.4)
 Requires-Dist: python-manilaclient (>=3.3.2)
 Requires-Dist: requests (>=2.27.1)
 Requires-Dist: semver (>=2.0.0,<3.0.0)
 Requires-Dist: shortuuid
 Description-Content-Type: text/markdown
```

