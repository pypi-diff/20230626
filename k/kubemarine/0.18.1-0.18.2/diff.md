# Comparing `tmp/kubemarine-0.18.1.tar.gz` & `tmp/kubemarine-0.18.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubemarine-0.18.1.tar", last modified: Mon Jun 19 10:32:52 2023, max compression
+gzip compressed data, was "kubemarine-0.18.2.tar", last modified: Fri Jun 23 09:56:57 2023, max compression
```

## Comparing `kubemarine-0.18.1.tar` & `kubemarine-0.18.2.tar`

### file list

```diff
@@ -1,241 +1,241 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.493515 kubemarine-0.18.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-19 10:32:36.000000 kubemarine-0.18.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      183 2023-06-19 10:32:36.000000 kubemarine-0.18.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12413 2023-06-19 10:32:52.493515 kubemarine-0.18.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8986 2023-06-19 10:32:36.000000 kubemarine-0.18.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.445515 kubemarine-0.18.1/bin/
--rwxr-xr-x   0 root         (0) root         (0)     1076 2023-06-19 10:32:36.000000 kubemarine-0.18.1/bin/kubemarine
--rw-r--r--   0 root         (0) root         (0)      657 2023-06-19 10:32:36.000000 kubemarine-0.18.1/bin/kubemarine.cmd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.453515 kubemarine-0.18.1/kubemarine/
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     8218 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/__main__.py
--rw-r--r--   0 root         (0) root         (0)    45051 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/admission.py
--rw-r--r--   0 root         (0) root         (0)     4862 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/apparmor.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/apt.py
--rw-r--r--   0 root         (0) root         (0)     4596 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/audit.py
--rw-r--r--   0 root         (0) root         (0)     2225 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/controlplane.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.457515 kubemarine-0.18.1/kubemarine/core/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2355 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/action.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/annotations.py
--rwxr-xr-x   0 root         (0) root         (0)    15520 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/cluster.py
--rw-r--r--   0 root         (0) root         (0)     4162 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/connections.py
--rwxr-xr-x   0 root         (0) root         (0)    23860 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/defaults.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/environment.py
--rw-r--r--   0 root         (0) root         (0)     5659 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/errors.py
--rw-r--r--   0 root         (0) root         (0)    16778 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/executor.py
--rwxr-xr-x   0 root         (0) root         (0)    18912 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/flow.py
--rwxr-xr-x   0 root         (0) root         (0)    41420 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/group.py
--rw-r--r--   0 root         (0) root         (0)    14424 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/log.py
--rw-r--r--   0 root         (0) root         (0)     1043 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/os.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/patch.py
--rw-r--r--   0 root         (0) root         (0)     8372 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/resources.py
--rw-r--r--   0 root         (0) root         (0)    15178 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/schema.py
--rw-r--r--   0 root         (0) root         (0)     2230 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/static.py
--rw-r--r--   0 root         (0) root         (0)     2110 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/summary.py
--rwxr-xr-x   0 root         (0) root         (0)    21325 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/utils.py
--rw-r--r--   0 root         (0) root         (0)     1671 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/yaml_merger.py
--rw-r--r--   0 root         (0) root         (0)     7067 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/coredns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.457515 kubemarine-0.18.1/kubemarine/cri/
--rw-r--r--   0 root         (0) root         (0)     2918 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/cri/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     6492 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/cri/containerd.py
--rwxr-xr-x   0 root         (0) root         (0)     3784 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/cri/docker.py
--rw-r--r--   0 root         (0) root         (0)    20072 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/demo.py
--rw-r--r--   0 root         (0) root         (0)     4664 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/etcd.py
--rw-r--r--   0 root         (0) root         (0)    10967 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/haproxy.py
--rw-r--r--   0 root         (0) root         (0)     2259 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/jinja.py
--rw-r--r--   0 root         (0) root         (0)     3437 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/k8s_certs.py
--rw-r--r--   0 root         (0) root         (0)    11269 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/keepalived.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.457515 kubemarine-0.18.1/kubemarine/kubernetes/
--rw-r--r--   0 root         (0) root         (0)    65136 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2189 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/kubernetes/daemonset.py
--rw-r--r--   0 root         (0) root         (0)     1753 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/kubernetes/deployment.py
--rw-r--r--   0 root         (0) root         (0)     3262 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/kubernetes/object.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/kubernetes/replicaset.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/kubernetes/statefulset.py
--rw-r--r--   0 root         (0) root         (0)     5780 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/kubernetes_accounts.py
--rw-r--r--   0 root         (0) root         (0)    29985 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/packages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.461515 kubemarine-0.18.1/kubemarine/patches/
--rw-r--r--   0 root         (0) root         (0)     1126 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/patches/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/patches/software_upgrade.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.461515 kubemarine-0.18.1/kubemarine/plugins/
--rwxr-xr-x   0 root         (0) root         (0)    40081 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3769 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/builtin.py
--rwxr-xr-x   0 root         (0) root         (0)    14938 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/calico.py
--rw-r--r--   0 root         (0) root         (0)     4842 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/kubernetes_dashboard.py
--rw-r--r--   0 root         (0) root         (0)     5721 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/local_path_provisioner.py
--rw-r--r--   0 root         (0) root         (0)    16606 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/manifest.py
--rw-r--r--   0 root         (0) root         (0)    19568 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/nginx_ingress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.465515 kubemarine-0.18.1/kubemarine/plugins/yaml/
--rw-r--r--   0 root         (0) root         (0)   222019 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml
--rw-r--r--   0 root         (0) root         (0)   239857 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml
--rw-r--r--   0 root         (0) root         (0)   243952 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)     7621 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)     7621 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15311 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15775 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15704 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.469515 kubemarine-0.18.1/kubemarine/procedures/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4919 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/add_node.py
--rwxr-xr-x   0 root         (0) root         (0)    20581 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/backup.py
--rwxr-xr-x   0 root         (0) root         (0)     2629 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/cert_renew.py
--rwxr-xr-x   0 root         (0) root         (0)    50185 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/check_iaas.py
--rwxr-xr-x   0 root         (0) root         (0)    72418 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/check_paas.py
--rwxr-xr-x   0 root         (0) root         (0)     5081 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/do.py
--rwxr-xr-x   0 root         (0) root         (0)    26620 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/install.py
--rwxr-xr-x   0 root         (0) root         (0)     1769 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/manage_psp.py
--rwxr-xr-x   0 root         (0) root         (0)     1667 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/manage_pss.py
--rwxr-xr-x   0 root         (0) root         (0)    14845 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/migrate_cri.py
--rw-r--r--   0 root         (0) root         (0)    19510 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/migrate_kubemarine.py
--rwxr-xr-x   0 root         (0) root         (0)     2380 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/reboot.py
--rwxr-xr-x   0 root         (0) root         (0)     6074 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/remove_node.py
--rwxr-xr-x   0 root         (0) root         (0)    13653 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/restore.py
--rwxr-xr-x   0 root         (0) root         (0)    11219 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/upgrade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.469515 kubemarine-0.18.1/kubemarine/resources/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.469515 kubemarine-0.18.1/kubemarine/resources/configurations/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/configurations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.469515 kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.473515 kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/internal/
--rw-r--r--   0 root         (0) root         (0)     3826 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml
--rw-r--r--   0 root         (0) root         (0)     5333 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/internal/packages.yaml
--rw-r--r--   0 root         (0) root         (0)     4067 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/internal/plugins.yaml
--rw-r--r--   0 root         (0) root         (0)     6255 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml
--rw-r--r--   0 root         (0) root         (0)     3177 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
--rw-r--r--   0 root         (0) root         (0)    25005 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/configurations/defaults.yaml
--rw-r--r--   0 root         (0) root         (0)    10638 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/configurations/globals.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.473515 kubemarine-0.18.1/kubemarine/resources/drop_ins/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/drop_ins/__init__.py
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/drop_ins/haproxy.conf
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/drop_ins/keepalived.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.445515 kubemarine-0.18.1/kubemarine/resources/etalons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.473515 kubemarine-0.18.1/kubemarine/resources/etalons/patches/
--rw-r--r--   0 root         (0) root         (0)     1126 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/etalons/patches/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/etalons/patches/software_upgrade.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.473515 kubemarine-0.18.1/kubemarine/resources/psp/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/psp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/psp/anyuid.yaml
--rw-r--r--   0 root         (0) root         (0)     1923 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/psp/default.yaml
--rw-r--r--   0 root         (0) root         (0)     1618 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/psp/host-network.yaml
--rw-r--r--   0 root         (0) root         (0)     1204 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/psp/privileged.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.473515 kubemarine-0.18.1/kubemarine/resources/reports/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/reports/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1773 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/reports/check_report.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.477515 kubemarine-0.18.1/kubemarine/resources/schemas/
--rw-r--r--   0 root         (0) root         (0)      832 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/add_node.json
--rw-r--r--   0 root         (0) root         (0)     2651 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/backup.json
--rw-r--r--   0 root         (0) root         (0)     1038 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/cert_renew.json
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/check_paas.json
--rw-r--r--   0 root         (0) root         (0)     3142 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/cluster.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.481515 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.481515 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/common/
--rw-r--r--   0 root         (0) root         (0)      520 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/common/node_ref.json
--rw-r--r--   0 root         (0) root         (0)     1722 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/common/utils.json
--rw-r--r--   0 root         (0) root         (0)      615 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/gateway_node.json
--rw-r--r--   0 root         (0) root         (0)     4072 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/globals.json
--rw-r--r--   0 root         (0) root         (0)     1501 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/node.json
--rw-r--r--   0 root         (0) root         (0)     2217 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/node_defaults.json
--rw-r--r--   0 root         (0) root         (0)      575 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugin_defaults.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.481515 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/
--rw-r--r--   0 root         (0) root         (0)     4806 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/calico.json
--rw-r--r--   0 root         (0) root         (0)     1161 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.485515 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json
--rw-r--r--   0 root         (0) root         (0)      689 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/config.json
--rw-r--r--   0 root         (0) root         (0)     3120 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/expect.json
--rw-r--r--   0 root         (0) root         (0)     1220 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/helm.json
--rw-r--r--   0 root         (0) root         (0)      606 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/python.json
--rw-r--r--   0 root         (0) root         (0)     2265 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/shell.json
--rw-r--r--   0 root         (0) root         (0)     2498 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/template.json
--rw-r--r--   0 root         (0) root         (0)     1780 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation.json
--rw-r--r--   0 root         (0) root         (0)     2901 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json
--rw-r--r--   0 root         (0) root         (0)     1628 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json
--rw-r--r--   0 root         (0) root         (0)     3201 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json
--rw-r--r--   0 root         (0) root         (0)      605 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins.json
--rw-r--r--   0 root         (0) root         (0)      749 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/procedures.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.485515 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/rbac/
--rw-r--r--   0 root         (0) root         (0)      661 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/rbac/account.json
--rw-r--r--   0 root         (0) root         (0)     3266 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/rbac/account_defaults.json
--rw-r--r--   0 root         (0) root         (0)     3759 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/rbac/psp.json
--rw-r--r--   0 root         (0) root         (0)     2453 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/rbac/pss.json
--rw-r--r--   0 root         (0) root         (0)      709 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/rbac.json
--rw-r--r--   0 root         (0) root         (0)     1951 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/registry.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.485515 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/
--rw-r--r--   0 root         (0) root         (0)     1855 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/audit.json
--rw-r--r--   0 root         (0) root         (0)     9668 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/coredns.json
--rw-r--r--   0 root         (0) root         (0)     2645 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/cri.json
--rw-r--r--   0 root         (0) root         (0)      644 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/etc_hosts.json
--rw-r--r--   0 root         (0) root         (0)     1963 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/kernel_security.json
--rw-r--r--   0 root         (0) root         (0)     4856 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/kubeadm.json
--rw-r--r--   0 root         (0) root         (0)      628 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json
--rw-r--r--   0 root         (0) root         (0)     3035 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json
--rw-r--r--   0 root         (0) root         (0)     2898 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/loadbalancer.json
--rw-r--r--   0 root         (0) root         (0)      936 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/modprobe.json
--rw-r--r--   0 root         (0) root         (0)     2302 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/ntp.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.485515 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/packages/
--rw-r--r--   0 root         (0) root         (0)     4198 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/packages/associations.json
--rw-r--r--   0 root         (0) root         (0)     5144 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/packages.json
--rw-r--r--   0 root         (0) root         (0)      479 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/resolv.conf.json
--rw-r--r--   0 root         (0) root         (0)     1176 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/sysctl.json
--rw-r--r--   0 root         (0) root         (0)     3302 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/thirdparties.json
--rw-r--r--   0 root         (0) root         (0)     1881 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services.json
--rw-r--r--   0 root         (0) root         (0)     3130 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/vrrp_ip.json
--rw-r--r--   0 root         (0) root         (0)      757 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/manage_psp.json
--rw-r--r--   0 root         (0) root         (0)     1657 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/manage_pss.json
--rw-r--r--   0 root         (0) root         (0)     1608 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/migrate_cri.json
--rw-r--r--   0 root         (0) root         (0)     2885 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/migrate_kubemarine.json
--rw-r--r--   0 root         (0) root         (0)      798 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/reboot.json
--rw-r--r--   0 root         (0) root         (0)      872 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/remove_node.json
--rw-r--r--   0 root         (0) root         (0)     3365 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/restore.json
--rw-r--r--   0 root         (0) root         (0)     2775 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/upgrade.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.489515 kubemarine-0.18.1/kubemarine/resources/scripts/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/scripts/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      288 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/scripts/check_haproxy.sh
--rw-r--r--   0 root         (0) root         (0)     1206 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/scripts/check_url_availability.py
--rwxr-xr-x   0 root         (0) root         (0)     3996 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/scripts/etcdctl.sh
--rw-r--r--   0 root         (0) root         (0)     1499 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/scripts/simple_tcp_listener.py
--rw-r--r--   0 root         (0) root         (0)     7984 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/selinux.py
--rw-r--r--   0 root         (0) root         (0)     3815 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/sysctl.py
--rw-r--r--   0 root         (0) root         (0)    26444 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.489515 kubemarine-0.18.1/kubemarine/templates/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)      667 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/admission.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     2259 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/haproxy.cfg.j2
--rw-r--r--   0 root         (0) root         (0)      714 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/keepalived.conf.j2
--rw-r--r--   0 root         (0) root         (0)     1126 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/kubelet.service.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.489515 kubemarine-0.18.1/kubemarine/templates/patches/
--rw-r--r--   0 root         (0) root         (0)      151 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/patches/control-plane-pod.json.j2
--rw-r--r--   0 root         (0) root         (0)       76 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/patches/kubelet.yaml.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.493515 kubemarine-0.18.1/kubemarine/templates/plugins/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      879 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/calico-ippool.yaml.j2
--rw-r--r--   0 root         (0) root         (0)      286 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/calico-kube-controllers-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      245 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/calico-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      436 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/calico-rr.sh.j2
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/calico-rr.yaml.j2
--rw-r--r--   0 root         (0) root         (0)      136 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/calicoctl.cfg.j2
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/dashboard-ingress.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     8826 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     8905 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     2749 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/iperf3.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     5401 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/local-path-provisioner.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     9973 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2
--rw-r--r--   0 root         (0) root         (0)    17847 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2
--rw-r--r--   0 root         (0) root         (0)    11284 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/testsuite.py
--rw-r--r--   0 root         (0) root         (0)    17436 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/thirdparties.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/version
--rw-r--r--   0 root         (0) root         (0)     4843 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/yum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.453515 kubemarine-0.18.1/kubemarine.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12413 2023-06-19 10:32:52.000000 kubemarine-0.18.1/kubemarine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9113 2023-06-19 10:32:52.000000 kubemarine-0.18.1/kubemarine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 10:32:52.000000 kubemarine-0.18.1/kubemarine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-19 10:32:52.000000 kubemarine-0.18.1/kubemarine.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      278 2023-06-19 10:32:52.000000 kubemarine-0.18.1/kubemarine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-19 10:32:52.000000 kubemarine-0.18.1/kubemarine.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2554 2023-06-19 10:32:36.000000 kubemarine-0.18.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 10:32:52.493515 kubemarine-0.18.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1628 2023-06-19 10:32:36.000000 kubemarine-0.18.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.685644 kubemarine-0.18.2/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-23 09:56:43.000000 kubemarine-0.18.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      183 2023-06-23 09:56:43.000000 kubemarine-0.18.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    12413 2023-06-23 09:56:57.685644 kubemarine-0.18.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8986 2023-06-23 09:56:43.000000 kubemarine-0.18.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.665644 kubemarine-0.18.2/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     1076 2023-06-23 09:56:43.000000 kubemarine-0.18.2/bin/kubemarine
+-rw-r--r--   0 root         (0) root         (0)      657 2023-06-23 09:56:43.000000 kubemarine-0.18.2/bin/kubemarine.cmd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.665644 kubemarine-0.18.2/kubemarine/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     8218 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    45051 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/admission.py
+-rw-r--r--   0 root         (0) root         (0)     4862 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/apparmor.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/apt.py
+-rw-r--r--   0 root         (0) root         (0)     4596 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/audit.py
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/controlplane.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.669644 kubemarine-0.18.2/kubemarine/core/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/action.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/annotations.py
+-rwxr-xr-x   0 root         (0) root         (0)    15520 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/connections.py
+-rwxr-xr-x   0 root         (0) root         (0)    23860 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/defaults.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/environment.py
+-rw-r--r--   0 root         (0) root         (0)     5659 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    16778 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/executor.py
+-rwxr-xr-x   0 root         (0) root         (0)    18912 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/flow.py
+-rwxr-xr-x   0 root         (0) root         (0)    41420 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/group.py
+-rw-r--r--   0 root         (0) root         (0)    14424 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/log.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/os.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/patch.py
+-rw-r--r--   0 root         (0) root         (0)     8372 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/resources.py
+-rw-r--r--   0 root         (0) root         (0)    15178 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/schema.py
+-rw-r--r--   0 root         (0) root         (0)     2230 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/static.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/summary.py
+-rwxr-xr-x   0 root         (0) root         (0)    21325 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/core/yaml_merger.py
+-rw-r--r--   0 root         (0) root         (0)     7067 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/coredns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.669644 kubemarine-0.18.2/kubemarine/cri/
+-rw-r--r--   0 root         (0) root         (0)     2918 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/cri/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6492 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/cri/containerd.py
+-rwxr-xr-x   0 root         (0) root         (0)     3784 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/cri/docker.py
+-rw-r--r--   0 root         (0) root         (0)    20072 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/demo.py
+-rw-r--r--   0 root         (0) root         (0)     4664 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/etcd.py
+-rw-r--r--   0 root         (0) root         (0)    10967 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/haproxy.py
+-rw-r--r--   0 root         (0) root         (0)     2259 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/jinja.py
+-rw-r--r--   0 root         (0) root         (0)     3437 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/k8s_certs.py
+-rw-r--r--   0 root         (0) root         (0)    11269 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/keepalived.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.669644 kubemarine-0.18.2/kubemarine/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)    65136 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/kubernetes/daemonset.py
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/kubernetes/deployment.py
+-rw-r--r--   0 root         (0) root         (0)     3262 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/kubernetes/object.py
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/kubernetes/replicaset.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/kubernetes/statefulset.py
+-rw-r--r--   0 root         (0) root         (0)     5780 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/kubernetes_accounts.py
+-rw-r--r--   0 root         (0) root         (0)    29985 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/packages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.669644 kubemarine-0.18.2/kubemarine/patches/
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/patches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/patches/software_upgrade.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.673644 kubemarine-0.18.2/kubemarine/plugins/
+-rwxr-xr-x   0 root         (0) root         (0)    41155 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3769 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/builtin.py
+-rwxr-xr-x   0 root         (0) root         (0)    14938 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/calico.py
+-rw-r--r--   0 root         (0) root         (0)     4842 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/kubernetes_dashboard.py
+-rw-r--r--   0 root         (0) root         (0)     5721 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/local_path_provisioner.py
+-rw-r--r--   0 root         (0) root         (0)    16606 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/manifest.py
+-rw-r--r--   0 root         (0) root         (0)    20211 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/nginx_ingress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.673644 kubemarine-0.18.2/kubemarine/plugins/yaml/
+-rw-r--r--   0 root         (0) root         (0)   222019 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   239857 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   243952 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     7621 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     7621 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15311 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15775 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15704 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.673644 kubemarine-0.18.2/kubemarine/procedures/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4919 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/add_node.py
+-rwxr-xr-x   0 root         (0) root         (0)    20581 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/backup.py
+-rwxr-xr-x   0 root         (0) root         (0)     2629 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/cert_renew.py
+-rwxr-xr-x   0 root         (0) root         (0)    50185 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/check_iaas.py
+-rwxr-xr-x   0 root         (0) root         (0)    72418 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/check_paas.py
+-rwxr-xr-x   0 root         (0) root         (0)     5081 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/do.py
+-rwxr-xr-x   0 root         (0) root         (0)    26620 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/install.py
+-rwxr-xr-x   0 root         (0) root         (0)     1769 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/manage_psp.py
+-rwxr-xr-x   0 root         (0) root         (0)     1667 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/manage_pss.py
+-rwxr-xr-x   0 root         (0) root         (0)    14845 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/migrate_cri.py
+-rw-r--r--   0 root         (0) root         (0)    19510 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/migrate_kubemarine.py
+-rwxr-xr-x   0 root         (0) root         (0)     2380 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/reboot.py
+-rwxr-xr-x   0 root         (0) root         (0)     6074 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/remove_node.py
+-rwxr-xr-x   0 root         (0) root         (0)    14048 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/restore.py
+-rwxr-xr-x   0 root         (0) root         (0)    11219 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/procedures/upgrade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.677644 kubemarine-0.18.2/kubemarine/resources/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.677644 kubemarine-0.18.2/kubemarine/resources/configurations/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/configurations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.677644 kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.677644 kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/internal/
+-rw-r--r--   0 root         (0) root         (0)     3826 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml
+-rw-r--r--   0 root         (0) root         (0)     5333 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/internal/packages.yaml
+-rw-r--r--   0 root         (0) root         (0)     4067 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/internal/plugins.yaml
+-rw-r--r--   0 root         (0) root         (0)     6255 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml
+-rw-r--r--   0 root         (0) root         (0)     3177 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
+-rw-r--r--   0 root         (0) root         (0)    25005 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/configurations/defaults.yaml
+-rw-r--r--   0 root         (0) root         (0)    10638 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/configurations/globals.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.677644 kubemarine-0.18.2/kubemarine/resources/drop_ins/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/drop_ins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/drop_ins/haproxy.conf
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/drop_ins/keepalived.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.665644 kubemarine-0.18.2/kubemarine/resources/etalons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.677644 kubemarine-0.18.2/kubemarine/resources/etalons/patches/
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/etalons/patches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/etalons/patches/software_upgrade.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.677644 kubemarine-0.18.2/kubemarine/resources/psp/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/psp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/psp/anyuid.yaml
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/psp/default.yaml
+-rw-r--r--   0 root         (0) root         (0)     1618 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/psp/host-network.yaml
+-rw-r--r--   0 root         (0) root         (0)     1204 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/psp/privileged.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.677644 kubemarine-0.18.2/kubemarine/resources/reports/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/reports/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/reports/check_report.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.677644 kubemarine-0.18.2/kubemarine/resources/schemas/
+-rw-r--r--   0 root         (0) root         (0)      832 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/add_node.json
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/backup.json
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/cert_renew.json
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/check_paas.json
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/cluster.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.681645 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.681645 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/common/
+-rw-r--r--   0 root         (0) root         (0)      520 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/common/node_ref.json
+-rw-r--r--   0 root         (0) root         (0)     1722 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/common/utils.json
+-rw-r--r--   0 root         (0) root         (0)      615 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/gateway_node.json
+-rw-r--r--   0 root         (0) root         (0)     4072 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/globals.json
+-rw-r--r--   0 root         (0) root         (0)     1501 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/node.json
+-rw-r--r--   0 root         (0) root         (0)     2217 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/node_defaults.json
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugin_defaults.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.681645 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/
+-rw-r--r--   0 root         (0) root         (0)     4806 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/calico.json
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.681645 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/config.json
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/expect.json
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/helm.json
+-rw-r--r--   0 root         (0) root         (0)      606 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/python.json
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/shell.json
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/template.json
+-rw-r--r--   0 root         (0) root         (0)     1780 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation.json
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json
+-rw-r--r--   0 root         (0) root         (0)     3201 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json
+-rw-r--r--   0 root         (0) root         (0)      605 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins.json
+-rw-r--r--   0 root         (0) root         (0)      749 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/procedures.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.681645 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/rbac/
+-rw-r--r--   0 root         (0) root         (0)      661 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/rbac/account.json
+-rw-r--r--   0 root         (0) root         (0)     3266 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/rbac/account_defaults.json
+-rw-r--r--   0 root         (0) root         (0)     3759 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/rbac/psp.json
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/rbac/pss.json
+-rw-r--r--   0 root         (0) root         (0)      709 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/rbac.json
+-rw-r--r--   0 root         (0) root         (0)     1951 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/registry.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.681645 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/
+-rw-r--r--   0 root         (0) root         (0)     1855 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/audit.json
+-rw-r--r--   0 root         (0) root         (0)     9668 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/coredns.json
+-rw-r--r--   0 root         (0) root         (0)     2645 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/cri.json
+-rw-r--r--   0 root         (0) root         (0)      644 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/etc_hosts.json
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/kernel_security.json
+-rw-r--r--   0 root         (0) root         (0)     4856 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/kubeadm.json
+-rw-r--r--   0 root         (0) root         (0)      628 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json
+-rw-r--r--   0 root         (0) root         (0)     3035 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json
+-rw-r--r--   0 root         (0) root         (0)     2898 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/loadbalancer.json
+-rw-r--r--   0 root         (0) root         (0)      936 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/modprobe.json
+-rw-r--r--   0 root         (0) root         (0)     2302 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/ntp.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.681645 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/packages/
+-rw-r--r--   0 root         (0) root         (0)     4198 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/packages/associations.json
+-rw-r--r--   0 root         (0) root         (0)     5144 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/packages.json
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/resolv.conf.json
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/sysctl.json
+-rw-r--r--   0 root         (0) root         (0)     3302 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/thirdparties.json
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services.json
+-rw-r--r--   0 root         (0) root         (0)     3130 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/definitions/vrrp_ip.json
+-rw-r--r--   0 root         (0) root         (0)      757 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/manage_psp.json
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/manage_pss.json
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/migrate_cri.json
+-rw-r--r--   0 root         (0) root         (0)     2885 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/migrate_kubemarine.json
+-rw-r--r--   0 root         (0) root         (0)      798 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/reboot.json
+-rw-r--r--   0 root         (0) root         (0)      872 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/remove_node.json
+-rw-r--r--   0 root         (0) root         (0)     3365 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/restore.json
+-rw-r--r--   0 root         (0) root         (0)     2775 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/schemas/upgrade.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.685644 kubemarine-0.18.2/kubemarine/resources/scripts/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/scripts/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      288 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/scripts/check_haproxy.sh
+-rw-r--r--   0 root         (0) root         (0)     1206 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/scripts/check_url_availability.py
+-rwxr-xr-x   0 root         (0) root         (0)     3996 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/scripts/etcdctl.sh
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/resources/scripts/simple_tcp_listener.py
+-rw-r--r--   0 root         (0) root         (0)     7984 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/selinux.py
+-rw-r--r--   0 root         (0) root         (0)     3815 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/sysctl.py
+-rw-r--r--   0 root         (0) root         (0)    26444 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.685644 kubemarine-0.18.2/kubemarine/templates/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      667 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/admission.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     2259 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/haproxy.cfg.j2
+-rw-r--r--   0 root         (0) root         (0)      714 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/keepalived.conf.j2
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/kubelet.service.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.685644 kubemarine-0.18.2/kubemarine/templates/patches/
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/patches/control-plane-pod.json.j2
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/patches/kubelet.yaml.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.685644 kubemarine-0.18.2/kubemarine/templates/plugins/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      879 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/calico-ippool.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)      286 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/calico-kube-controllers-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/calico-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      436 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/calico-rr.sh.j2
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/calico-rr.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)      136 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/calicoctl.cfg.j2
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/dashboard-ingress.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     8826 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     8905 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     2749 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/iperf3.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     5401 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/local-path-provisioner.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     9973 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)    17847 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)    11284 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/testsuite.py
+-rw-r--r--   0 root         (0) root         (0)    17436 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/thirdparties.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/version
+-rw-r--r--   0 root         (0) root         (0)     4843 2023-06-23 09:56:43.000000 kubemarine-0.18.2/kubemarine/yum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 09:56:57.669644 kubemarine-0.18.2/kubemarine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12413 2023-06-23 09:56:57.000000 kubemarine-0.18.2/kubemarine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9113 2023-06-23 09:56:57.000000 kubemarine-0.18.2/kubemarine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 09:56:57.000000 kubemarine-0.18.2/kubemarine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-23 09:56:57.000000 kubemarine-0.18.2/kubemarine.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      278 2023-06-23 09:56:57.000000 kubemarine-0.18.2/kubemarine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-23 09:56:57.000000 kubemarine-0.18.2/kubemarine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2554 2023-06-23 09:56:43.000000 kubemarine-0.18.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 09:56:57.685644 kubemarine-0.18.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-06-23 09:56:43.000000 kubemarine-0.18.2/setup.py
```

### Comparing `kubemarine-0.18.1/LICENSE` & `kubemarine-0.18.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/PKG-INFO` & `kubemarine-0.18.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubemarine
-Version: 0.18.1
+Version: 0.18.2
 Summary: Management tool for Kubernetes cluster deployment and maintenance
 Home-page: https://github.com/Netcracker/KubeMarine
 Author-email: Kubemarine Group <kubemarinegroup@netcracker.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Netcracker/KubeMarine
 Project-URL: Documentation, https://github.com/Netcracker/KubeMarine#documentation
 Project-URL: Issues, https://github.com/Netcracker/KubeMarine/issues/
@@ -33,36 +33,36 @@
 # Kubemarine
 
 Kubemarine is an open source, lightweight and powerful management tool built for end-to-end Kubernetes cluster deployment and maintenance. It is applicable for many purposes like simple and quick onboarding Kubernetes on local and production environments in different HA schemes depending on your aims, budget, and capabilities. Together with simplicity, Kubemarine can be a very flexible and customizable tool covering specific configurability cases on both deployment and maintenance stages. This library provides powerful CLI commands, as well as can be customized using a Python extension API.
 
 ## Highlights
 - Easy to use
 - Many procedures supported:
-  - [install](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#)
-  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#add-node-procedure)
-  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#remove-node-procedure)
-  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#upgrade-procedure)
-  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#backup-procedure)
-  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#restore-procedure)
-  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Kubecheck.md#iaas-procedure)
-  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Kubecheck.md#paas-procedure)
-  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#kubemarine-migration-procedure)
-  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#manage-psp-procedure)
-  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#manage-pss-procedure)
-  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#certificate-renew-procedure)
-  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#migration-cri-procedure)
-- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#configuration) for all operations, highly customizable
+  - [install](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#)
+  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#add-node-procedure)
+  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#remove-node-procedure)
+  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#upgrade-procedure)
+  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#backup-procedure)
+  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#restore-procedure)
+  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Kubecheck.md#iaas-procedure)
+  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Kubecheck.md#paas-procedure)
+  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#kubemarine-migration-procedure)
+  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#manage-psp-procedure)
+  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#manage-pss-procedure)
+  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#certificate-renew-procedure)
+  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#migration-cri-procedure)
+- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#configuration) for all operations, highly customizable
 - Default values of all parameters in configurations with a minimum of required parameters
-- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
-- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
-- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#custom-plugins-installation-procedures) support
-- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#installation-without-internet-resources) with private registries
-- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#dump-files)
+- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
+- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
+- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#custom-plugins-installation-procedures) support
+- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#installation-without-internet-resources) with private registries
+- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#dump-files)
 - Build supported as a package, container, and binary
-- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/PackageExtension.md)
+- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/PackageExtension.md)
 - Support different deployment schemes (all-in-one, mini-HA, HA, and so on)
 
 ## Kubemarine Binary Installation
 Proceed the following steps to install Kubemarine  on your environment:
 1. Download the binary file for your system from the latest [release](https://github.com/Netcracker/KubeMarine/releases)
 2. Move binary kubemarine to a separate folder 
 3. Now you can proceed to run Kubemarine! Try the following:
@@ -80,15 +80,15 @@
    ```bash
    python3 -m pip install --upgrade pip
    ```
    Windows:
    ```bash
    python -m pip install --upgrade pip
    ```
-1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#prerequisites-for-deployment-node).
+1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#prerequisites-for-deployment-node).
 1. Create and activate a [virtual environment](https://realpython.com/python-virtual-environments-a-primer/) if necessary.
 1. Install Kubemarine package.
 
    Linux / MacOS:
    ```bash
    python3 -m pip install kubemarine
    ```
@@ -99,15 +99,15 @@
 1. Now you can proceed to run Kubemarine! Try the following:
    ```bash
    kubemarine help
    ```
 
 
 ## Kubemarine Installation from Sources
-Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.1/README.md#kubemarine-package-installation).
+Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.2/README.md#kubemarine-package-installation).
 The exception is instead of installing the package from [PyPI](https://pypi.org/project/kubemarine/), do the following:
 1. [Download the latest release](https://github.com/netcracker/kubemarine/releases) or clone the repository:
    ```bash
    git clone https://github.com/netcracker/kubemarine.git
    ```
 1. Unpack the project from the archive if required:
    ```bash
@@ -128,24 +128,24 @@
    python -m pip install -e .
    ```
 1. Now you can proceed to run Kubemarine. Try the following:
     ```bash
     kubemarine help
     ```
 
-**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.18.1/Dockerfile) is also available.
+**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.18.2/Dockerfile) is also available.
 
 
 **Note:** Kubemarine debugging available via `kubemarine/__main__.py`.
 
 
 ## Running Cluster Installation
 To install a Kubernetes cluster using Kubemarine:
-1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#prerequisites-for-cluster-nodes).
-1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.18.1/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
+1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#prerequisites-for-cluster-nodes).
+1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.18.2/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
    ```yaml
    node_defaults:
      keyfile: "/home/username/.ssh/id_rsa"
      username: "centos"
 
    vrrp_ips:
      - 192.168.0.250
@@ -173,42 +173,42 @@
    kubemarine install
    ```
 1. Check the health of the newly installed cluster:
    ```bash
    kubemarine check_paas
    ```
 
-For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.18.1/README.md#documentation).
+For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.18.2/README.md#documentation).
 
 ## Kubemarine Docker Installation
 To start, download the Kubmarine image ```docker pull ghcr.io/netcracker/kubemarine:main```
 
 Run Kubemarine from the container, for example:
    ```
    docker run -it --mount type=bind,source=/root/cluster.yaml,target=/opt/kubemarine/cluster.yaml --mount type=bind,source=/root/rsa_key,target=/opt/kubemarine/rsa_key kubemarine install -c /opt/kubemarine/cluster.yaml
    ```
    *Note*: Do not forget to pass the inventory file and connection key inside the container.
    For more execution details, refer to ["Installation of Kubernetes using CLI" guide on Github](https://github.com/Netcracker/kubemarine/blob/main/documentation/Installation.md#installation-of-kubernetes-using-cli).
 
 ## Documentation
 The following documents and tutorials are available:
-- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md)
-- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md)
-- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Troubleshooting.md)
-- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Kubecheck.md)
-- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Logging.md)
+- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md)
+- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md)
+- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Troubleshooting.md)
+- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Kubecheck.md)
+- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Logging.md)
 
 Also, check out the following inventory examples:
-- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.1/examples/cluster.yaml)
-- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.1/examples/procedure.yaml)
+- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.2/examples/cluster.yaml)
+- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.2/examples/procedure.yaml)
 
 ## Issues, Questions
 If you have any problems while working with Kubemarine, feel free to open a [new issue](https://github.com/netcracker/kubemarine/issues) or even
 [PR](https://github.com/netcracker/kubemarine/pulls) with related changes.
-Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.18.1/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
+Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.18.2/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
 
-In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.18.1/SECURITY.md)
+In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.18.2/SECURITY.md)
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/netcracker/kubemarine/releases).
 
 ## License
-[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.18.1/LICENSE)
+[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.18.2/LICENSE)
```

### Comparing `kubemarine-0.18.1/README.md` & `kubemarine-0.18.2/README.md`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/bin/kubemarine` & `kubemarine-0.18.2/bin/kubemarine`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/bin/kubemarine.cmd` & `kubemarine-0.18.2/bin/kubemarine.cmd`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/__init__.py` & `kubemarine-0.18.2/kubemarine/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/__main__.py` & `kubemarine-0.18.2/kubemarine/__main__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/admission.py` & `kubemarine-0.18.2/kubemarine/admission.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/apparmor.py` & `kubemarine-0.18.2/kubemarine/apparmor.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/apt.py` & `kubemarine-0.18.2/kubemarine/apt.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/audit.py` & `kubemarine-0.18.2/kubemarine/audit.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/controlplane.py` & `kubemarine-0.18.2/kubemarine/controlplane.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/core/__init__.py` & `kubemarine-0.18.2/kubemarine/core/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/core/action.py` & `kubemarine-0.18.2/kubemarine/core/action.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/core/annotations.py` & `kubemarine-0.18.2/kubemarine/core/annotations.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/core/cluster.py` & `kubemarine-0.18.2/kubemarine/core/cluster.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/core/connections.py` & `kubemarine-0.18.2/kubemarine/core/connections.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/core/defaults.py` & `kubemarine-0.18.2/kubemarine/core/defaults.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/core/environment.py` & `kubemarine-0.18.2/kubemarine/core/environment.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/core/errors.py` & `kubemarine-0.18.2/kubemarine/core/errors.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/core/executor.py` & `kubemarine-0.18.2/kubemarine/core/executor.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/core/flow.py` & `kubemarine-0.18.2/kubemarine/core/flow.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/core/group.py` & `kubemarine-0.18.2/kubemarine/core/group.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/core/log.py` & `kubemarine-0.18.2/kubemarine/core/log.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/core/os.py` & `kubemarine-0.18.2/kubemarine/core/os.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/core/patch.py` & `kubemarine-0.18.2/kubemarine/core/patch.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/core/resources.py` & `kubemarine-0.18.2/kubemarine/core/resources.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/core/schema.py` & `kubemarine-0.18.2/kubemarine/core/schema.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/core/static.py` & `kubemarine-0.18.2/kubemarine/core/static.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/core/summary.py` & `kubemarine-0.18.2/kubemarine/core/summary.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/core/utils.py` & `kubemarine-0.18.2/kubemarine/core/utils.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/core/yaml_merger.py` & `kubemarine-0.18.2/kubemarine/core/yaml_merger.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/coredns.py` & `kubemarine-0.18.2/kubemarine/coredns.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/cri/__init__.py` & `kubemarine-0.18.2/kubemarine/cri/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/cri/containerd.py` & `kubemarine-0.18.2/kubemarine/cri/containerd.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/cri/docker.py` & `kubemarine-0.18.2/kubemarine/cri/docker.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/demo.py` & `kubemarine-0.18.2/kubemarine/demo.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/etcd.py` & `kubemarine-0.18.2/kubemarine/etcd.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/haproxy.py` & `kubemarine-0.18.2/kubemarine/haproxy.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/jinja.py` & `kubemarine-0.18.2/kubemarine/jinja.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/k8s_certs.py` & `kubemarine-0.18.2/kubemarine/k8s_certs.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/keepalived.py` & `kubemarine-0.18.2/kubemarine/keepalived.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/kubernetes/__init__.py` & `kubemarine-0.18.2/kubemarine/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/kubernetes/daemonset.py` & `kubemarine-0.18.2/kubemarine/kubernetes/daemonset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/kubernetes/deployment.py` & `kubemarine-0.18.2/kubemarine/kubernetes/deployment.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/kubernetes/object.py` & `kubemarine-0.18.2/kubemarine/kubernetes/object.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/kubernetes/replicaset.py` & `kubemarine-0.18.2/kubemarine/kubernetes/replicaset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/kubernetes/statefulset.py` & `kubemarine-0.18.2/kubemarine/kubernetes/statefulset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/kubernetes_accounts.py` & `kubemarine-0.18.2/kubemarine/kubernetes_accounts.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/packages.py` & `kubemarine-0.18.2/kubemarine/packages.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/patches/__init__.py` & `kubemarine-0.18.2/kubemarine/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/patches/software_upgrade.yaml` & `kubemarine-0.18.2/kubemarine/patches/software_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/plugins/__init__.py` & `kubemarine-0.18.2/kubemarine/plugins/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,30 +29,31 @@
 import zipfile
 from copy import deepcopy
 from distutils.dir_util import copy_tree
 from distutils.dir_util import remove_tree
 from distutils.dir_util import mkpath
 from itertools import chain
 from typing import Dict, List, Tuple
-
 import yaml
+import inspect
+from inspect import signature
 
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine import jinja, thirdparties
 from kubemarine.core import utils, static, errors, os as kos
 from kubemarine.core.yaml_merger import default_merger
 from kubemarine.core.group import NodeGroup, NodeGroupResult
 from kubemarine.kubernetes.daemonset import DaemonSet
 from kubemarine.kubernetes.deployment import Deployment
 from kubemarine.kubernetes.replicaset import ReplicaSet
 from kubemarine.kubernetes.statefulset import StatefulSet
 
 # list of plugins owned and managed by kubemarine
 oob_plugins = list(static.DEFAULTS["plugins"].keys())
-
+LOADED_MODULES = {}
 
 def verify_inventory(inventory, cluster):
     for plugin_name, plugin_item in inventory["plugins"].items():
         for step in plugin_item.get('installation', {}).get('procedures', []):
             for procedure_type, configs in step.items():
                 if procedure_types[procedure_type].get('verify') is not None:
                     procedure_types[procedure_type]['verify'](cluster, configs)
@@ -566,33 +567,66 @@
                               retries=config['deployments'].get('retries'))
 
         elif expect_type == 'pods':
             expect_pods(cluster, config['pods']['list'], namespace=config['pods'].get('namespace'),
                         timeout=config['pods'].get('timeout'),
                         retries=config['pods'].get('retries'))
 
-
 # **** PYTHON ****
 
-def verify_python(cluster, step):
-    # TODO: verify fields types and contents
-    return
+def get_python_module(module_path):
+    if module_path in LOADED_MODULES:
+        return LOADED_MODULES[module_path]
+
+    spec = importlib.util.spec_from_file_location('module', module_path)
+    try:
+        module = importlib.util.module_from_spec(spec)
+        spec.loader.exec_module(module)
+        LOADED_MODULES[module_path] = module
+    except Exception as e:
+        raise ValueError(f"Could not import module {module_path}: {e}")
+    return module 
 
 
-def apply_python(cluster, step, plugin_name=None):
+def get_python_method_args(cluster, step):
     module_path, _ = utils.determine_resource_absolute_file(step['module'])
     method_name = step['method']
     method_arguments = step.get('arguments', {})
 
-    cluster.log.debug("Running method %s from %s module..." % (method_name, module_path))
-    module_filename = os.path.basename(module_path)
-    spec = importlib.util.spec_from_file_location(os.path.splitext(module_filename)[0], module_path)
-    module = importlib.util.module_from_spec(spec)
-    spec.loader.exec_module(module)
-    getattr(module, method_name)(cluster, **method_arguments)
+    module = get_python_module(module_path)
+
+    # Check if the method exists
+    if not hasattr(module, method_name):
+        raise ValueError(f"Module {module_path} does not have method {method_name}")
+
+    # Get the method object
+    method = getattr(module, method_name)
+
+    # Get the signature of the method
+    signature = inspect.signature(method)
+
+    # Check if the passed arguments match the signature
+    try:
+        signature.bind(cluster=cluster, **method_arguments)
+    except TypeError as e:
+        raise ValueError(f"Invalid arguments for method {method_name}: {e}")
+
+    return method, method_arguments
+
+
+def verify_python(cluster, step):
+    method, method_arguments = get_python_method_args(cluster, step)
+    # Additional verification logic can be added here
+
+
+def apply_python(cluster, step, plugin_name=None):
+    method, method_arguments = get_python_method_args(cluster, step)
+
+    cluster.log.debug("Running method %s from %s module..." % (method.__name__, method.__module__))
+    method(cluster, **method_arguments)
 
 
 # **** THIRDPARTIES ****
 
 def verify_thirdparty(cluster, thirdparty):
     defined_thirdparties = list(cluster.inventory['services'].get('thirdparties', {}).keys())
     if thirdparty not in defined_thirdparties:
@@ -1028,8 +1062,8 @@
         'apply': apply_helm
     },
     'config': {
         'convert': convert_config,
         'verify': verify_config,
         'apply': apply_config
     },
-}
+}
```

### Comparing `kubemarine-0.18.1/kubemarine/plugins/builtin.py` & `kubemarine-0.18.2/kubemarine/plugins/builtin.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/plugins/calico.py` & `kubemarine-0.18.2/kubemarine/plugins/calico.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/plugins/kubernetes_dashboard.py` & `kubemarine-0.18.2/kubemarine/plugins/kubernetes_dashboard.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/plugins/local_path_provisioner.py` & `kubemarine-0.18.2/kubemarine/plugins/local_path_provisioner.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/plugins/manifest.py` & `kubemarine-0.18.2/kubemarine/plugins/manifest.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/plugins/nginx_ingress.py` & `kubemarine-0.18.2/kubemarine/plugins/nginx_ingress.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
+import ipaddress
 from typing import Optional, List
 
 from kubemarine.core import utils, log
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.group import NodeGroup
 from kubemarine.plugins.manifest import Processor, EnrichmentFunction, Manifest
 
@@ -181,14 +182,15 @@
             self.enrich_namespace_ingress_nginx,
             self.enrich_configmap_ingress_nginx_controller,
             self.add_configmap_ingress_nginx_controller,
             self.enrich_deployment_ingress_nginx_controller,
             self.enrich_ingressclass_nginx,
             self.enrich_job_ingress_nginx_admission_create,
             self.enrich_job_ingress_nginx_admission_patch,
+            self.enrich_service_ingress_nginx_controller,
         ]
 
     def enrich_namespace_ingress_nginx(self, manifest: Manifest):
         key = "Namespace_ingress-nginx"
         rbac = self.inventory['rbac']
         if rbac['admission'] == 'pss' and rbac['pss']['pod-security'] == 'enabled' \
                 and rbac['pss']['defaults']['enforce'] != 'privileged':
@@ -298,14 +300,23 @@
             plugin_service='webhook', container_name='create', is_init_container=False)
 
     def enrich_job_ingress_nginx_admission_patch(self, manifest: Manifest):
         key = "Job_ingress-nginx-admission-patch"
         self.enrich_image_for_container(manifest, key,
             plugin_service='webhook', container_name='patch', is_init_container=False)
 
+    def enrich_service_ingress_nginx_controller(self, manifest: Manifest):
+        # The method needs some rework in case of dual stack support
+        key = "Service_ingress-nginx-controller"
+        ip = self.inventory['services']['kubeadm']['networking']['serviceSubnet'].split('/')[0]
+        if type(ipaddress.ip_address(ip)) is ipaddress.IPv6Address:
+            source_yaml = manifest.get_obj(key, patch=True)
+            source_yaml['spec']['ipFamilies'] = ['IPv6']
+            self.log.verbose(f"The {key} has been patched in 'spec.ipFamilies' with 'IPv6'")
+
 
 class V1_2_X_IngressNginxManifestProcessor(IngressNginxManifestProcessor):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def get_enrichment_functions(self) -> List[EnrichmentFunction]:
         enrichment_functions = super().get_enrichment_functions()
```

### Comparing `kubemarine-0.18.1/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml` & `kubemarine-0.18.2/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml` & `kubemarine-0.18.2/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml` & `kubemarine-0.18.2/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml` & `kubemarine-0.18.2/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml` & `kubemarine-0.18.2/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml` & `kubemarine-0.18.2/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml` & `kubemarine-0.18.2/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml` & `kubemarine-0.18.2/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml` & `kubemarine-0.18.2/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml` & `kubemarine-0.18.2/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml` & `kubemarine-0.18.2/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/procedures/__init__.py` & `kubemarine-0.18.2/kubemarine/procedures/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/procedures/add_node.py` & `kubemarine-0.18.2/kubemarine/procedures/add_node.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/procedures/backup.py` & `kubemarine-0.18.2/kubemarine/procedures/backup.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/procedures/cert_renew.py` & `kubemarine-0.18.2/kubemarine/procedures/cert_renew.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/procedures/check_iaas.py` & `kubemarine-0.18.2/kubemarine/procedures/check_iaas.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/procedures/check_paas.py` & `kubemarine-0.18.2/kubemarine/procedures/check_paas.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/procedures/do.py` & `kubemarine-0.18.2/kubemarine/procedures/do.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/procedures/install.py` & `kubemarine-0.18.2/kubemarine/procedures/install.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/procedures/manage_psp.py` & `kubemarine-0.18.2/kubemarine/procedures/manage_psp.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/procedures/manage_pss.py` & `kubemarine-0.18.2/kubemarine/procedures/manage_pss.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/procedures/migrate_cri.py` & `kubemarine-0.18.2/kubemarine/procedures/migrate_cri.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/procedures/migrate_kubemarine.py` & `kubemarine-0.18.2/kubemarine/procedures/migrate_kubemarine.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/procedures/reboot.py` & `kubemarine-0.18.2/kubemarine/procedures/reboot.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/procedures/remove_node.py` & `kubemarine-0.18.2/kubemarine/procedures/remove_node.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/procedures/restore.py` & `kubemarine-0.18.2/kubemarine/procedures/restore.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from kubemarine.core import utils, flow, defaults
 from kubemarine.core.action import Action
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.group import NodeGroup
 from kubemarine.core.resources import DynamicResources
 from kubemarine.procedures import install, backup
 from kubemarine import system, kubernetes, etcd
+from kubemarine.core.executor import RemoteExecutor
 
 
 def missing_or_empty(file):
     if not os.path.exists(file):
         return True
     content = utils.read_external(file)
     if re.search(r'^\s*$', content):
@@ -139,17 +140,23 @@
 def import_nodes(cluster):
     for node in cluster.nodes['all'].get_ordered_members_list(provide_node_configs=True):
         node['connection'].put(os.path.join(cluster.context['backup_tmpdir'], 'nodes_data', '%s.tar.gz' % node['name']),
                                '/tmp/kubemarine-backup.tar.gz')
         cluster.log.debug('Backup \'%s\' uploaded' % node['name'])
 
     cluster.log.debug('Unpacking backup...')
-    result = cluster.nodes['all'].sudo(
-        'chattr -i /etc/resolv.conf; sudo tar xzvf /tmp/kubemarine-backup.tar.gz -C / --overwrite && sudo chattr +i /etc/resolv.conf')
-    cluster.log.debug(result)
+
+    with RemoteExecutor(cluster) as exe:
+        for node in cluster.nodes['all'].get_ordered_members_list(provide_node_configs=True):
+            cmd = f"readlink /etc/resolv.conf ;" \
+                  f"if [ $? -ne 0 ]; then sudo chattr -i /etc/resolv.conf; sudo tar xzvf /tmp/kubemarine-backup.tar.gz -C / --overwrite && sudo chattr +i /etc/resolv.conf; else sudo tar xzvf /tmp/kubemarine-backup.tar.gz -C / --overwrite; fi "
+            node['connection'].sudo(cmd)
+
+    result = exe.get_last_results_str()
+    cluster.log.debug('%s',result)
 
 
 def import_etcd(cluster: KubernetesCluster):
     etcd_all_certificates = cluster.procedure_inventory.get('restore_plan', {}).get('etcd', {}).get('certificates', {})
     etcd_cert = etcd_all_certificates.get('cert', cluster.globals['etcd']['default_arguments']['cert'])
     etcd_key = etcd_all_certificates.get('key', cluster.globals['etcd']['default_arguments']['key'])
     etcd_cacert = etcd_all_certificates.get('cacert', cluster.globals['etcd']['default_arguments']['cacert'])
```

### Comparing `kubemarine-0.18.1/kubemarine/procedures/upgrade.py` & `kubemarine-0.18.2/kubemarine/procedures/upgrade.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/__init__.py` & `kubemarine-0.18.2/kubemarine/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/configurations/__init__.py` & `kubemarine-0.18.2/kubemarine/resources/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml` & `kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/internal/packages.yaml` & `kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/internal/packages.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/internal/plugins.yaml` & `kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/internal/plugins.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml` & `kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml` & `kubemarine-0.18.2/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/configurations/defaults.yaml` & `kubemarine-0.18.2/kubemarine/resources/configurations/defaults.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/configurations/globals.yaml` & `kubemarine-0.18.2/kubemarine/resources/configurations/globals.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/drop_ins/__init__.py` & `kubemarine-0.18.2/kubemarine/resources/drop_ins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/etalons/patches/__init__.py` & `kubemarine-0.18.2/kubemarine/resources/etalons/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/etalons/patches/software_upgrade.yaml` & `kubemarine-0.18.2/kubemarine/resources/etalons/patches/software_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/psp/__init__.py` & `kubemarine-0.18.2/kubemarine/resources/psp/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/psp/anyuid.yaml` & `kubemarine-0.18.2/kubemarine/resources/psp/anyuid.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/psp/default.yaml` & `kubemarine-0.18.2/kubemarine/resources/psp/default.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/psp/host-network.yaml` & `kubemarine-0.18.2/kubemarine/resources/psp/host-network.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/psp/privileged.yaml` & `kubemarine-0.18.2/kubemarine/resources/psp/privileged.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/reports/__init__.py` & `kubemarine-0.18.2/kubemarine/resources/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/reports/check_report.css` & `kubemarine-0.18.2/kubemarine/resources/reports/check_report.css`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/add_node.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/add_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/backup.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/backup.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/cert_renew.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/cert_renew.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/cluster.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/cluster.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/common/node_ref.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/common/node_ref.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/common/utils.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/common/utils.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/gateway_node.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/gateway_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/globals.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/globals.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/node.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/node_defaults.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/node_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugin_defaults.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugin_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/calico.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/calico.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/config.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/config.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/expect.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/expect.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/helm.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/helm.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/python.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/python.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/shell.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/shell.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/template.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation/template.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/installation.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/plugins.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/procedures.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/procedures.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/rbac/account.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/rbac/account.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/rbac/account_defaults.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/rbac/account_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/rbac/psp.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/rbac/psp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/rbac/pss.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/rbac/pss.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/rbac.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/rbac.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/registry.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/registry.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/audit.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/audit.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/coredns.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/coredns.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/cri.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/cri.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/etc_hosts.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/etc_hosts.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/kernel_security.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/kernel_security.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/kubeadm.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/kubeadm.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/loadbalancer.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/loadbalancer.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/modprobe.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/modprobe.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/ntp.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/ntp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/packages/associations.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/packages/associations.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/packages.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/packages.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/sysctl.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/sysctl.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/thirdparties.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services/thirdparties.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/services.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/vrrp_ip.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/definitions/vrrp_ip.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/manage_psp.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/manage_psp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/manage_pss.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/manage_pss.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/migrate_cri.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/migrate_cri.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/migrate_kubemarine.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/migrate_kubemarine.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/reboot.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/reboot.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/remove_node.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/remove_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/restore.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/restore.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/schemas/upgrade.json` & `kubemarine-0.18.2/kubemarine/resources/schemas/upgrade.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/scripts/__init__.py` & `kubemarine-0.18.2/kubemarine/resources/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/scripts/check_url_availability.py` & `kubemarine-0.18.2/kubemarine/resources/scripts/check_url_availability.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/scripts/etcdctl.sh` & `kubemarine-0.18.2/kubemarine/resources/scripts/etcdctl.sh`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/resources/scripts/simple_tcp_listener.py` & `kubemarine-0.18.2/kubemarine/resources/scripts/simple_tcp_listener.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/selinux.py` & `kubemarine-0.18.2/kubemarine/selinux.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/sysctl.py` & `kubemarine-0.18.2/kubemarine/sysctl.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/system.py` & `kubemarine-0.18.2/kubemarine/system.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/templates/__init__.py` & `kubemarine-0.18.2/kubemarine/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/templates/admission.yaml.j2` & `kubemarine-0.18.2/kubemarine/templates/admission.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/templates/haproxy.cfg.j2` & `kubemarine-0.18.2/kubemarine/templates/haproxy.cfg.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/templates/keepalived.conf.j2` & `kubemarine-0.18.2/kubemarine/templates/keepalived.conf.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/templates/kubelet.service.j2` & `kubemarine-0.18.2/kubemarine/templates/kubelet.service.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/templates/plugins/__init__.py` & `kubemarine-0.18.2/kubemarine/templates/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/templates/plugins/calico-ippool.yaml.j2` & `kubemarine-0.18.2/kubemarine/templates/plugins/calico-ippool.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/templates/plugins/calico-rr.yaml.j2` & `kubemarine-0.18.2/kubemarine/templates/plugins/calico-rr.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2` & `kubemarine-0.18.2/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2` & `kubemarine-0.18.2/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/templates/plugins/iperf3.yaml.j2` & `kubemarine-0.18.2/kubemarine/templates/plugins/iperf3.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/templates/plugins/local-path-provisioner.yaml.j2` & `kubemarine-0.18.2/kubemarine/templates/plugins/local-path-provisioner.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2` & `kubemarine-0.18.2/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2` & `kubemarine-0.18.2/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/testsuite.py` & `kubemarine-0.18.2/kubemarine/testsuite.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/thirdparties.py` & `kubemarine-0.18.2/kubemarine/thirdparties.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine/yum.py` & `kubemarine-0.18.2/kubemarine/yum.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/kubemarine.egg-info/PKG-INFO` & `kubemarine-0.18.2/kubemarine.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubemarine
-Version: 0.18.1
+Version: 0.18.2
 Summary: Management tool for Kubernetes cluster deployment and maintenance
 Home-page: https://github.com/Netcracker/KubeMarine
 Author-email: Kubemarine Group <kubemarinegroup@netcracker.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Netcracker/KubeMarine
 Project-URL: Documentation, https://github.com/Netcracker/KubeMarine#documentation
 Project-URL: Issues, https://github.com/Netcracker/KubeMarine/issues/
@@ -33,36 +33,36 @@
 # Kubemarine
 
 Kubemarine is an open source, lightweight and powerful management tool built for end-to-end Kubernetes cluster deployment and maintenance. It is applicable for many purposes like simple and quick onboarding Kubernetes on local and production environments in different HA schemes depending on your aims, budget, and capabilities. Together with simplicity, Kubemarine can be a very flexible and customizable tool covering specific configurability cases on both deployment and maintenance stages. This library provides powerful CLI commands, as well as can be customized using a Python extension API.
 
 ## Highlights
 - Easy to use
 - Many procedures supported:
-  - [install](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#)
-  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#add-node-procedure)
-  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#remove-node-procedure)
-  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#upgrade-procedure)
-  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#backup-procedure)
-  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#restore-procedure)
-  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Kubecheck.md#iaas-procedure)
-  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Kubecheck.md#paas-procedure)
-  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#kubemarine-migration-procedure)
-  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#manage-psp-procedure)
-  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#manage-pss-procedure)
-  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#certificate-renew-procedure)
-  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#migration-cri-procedure)
-- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#configuration) for all operations, highly customizable
+  - [install](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#)
+  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#add-node-procedure)
+  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#remove-node-procedure)
+  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#upgrade-procedure)
+  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#backup-procedure)
+  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#restore-procedure)
+  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Kubecheck.md#iaas-procedure)
+  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Kubecheck.md#paas-procedure)
+  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#kubemarine-migration-procedure)
+  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#manage-psp-procedure)
+  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#manage-pss-procedure)
+  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#certificate-renew-procedure)
+  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md#migration-cri-procedure)
+- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#configuration) for all operations, highly customizable
 - Default values of all parameters in configurations with a minimum of required parameters
-- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
-- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
-- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#custom-plugins-installation-procedures) support
-- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#installation-without-internet-resources) with private registries
-- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#dump-files)
+- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
+- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
+- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#custom-plugins-installation-procedures) support
+- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#installation-without-internet-resources) with private registries
+- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#dump-files)
 - Build supported as a package, container, and binary
-- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/PackageExtension.md)
+- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/PackageExtension.md)
 - Support different deployment schemes (all-in-one, mini-HA, HA, and so on)
 
 ## Kubemarine Binary Installation
 Proceed the following steps to install Kubemarine  on your environment:
 1. Download the binary file for your system from the latest [release](https://github.com/Netcracker/KubeMarine/releases)
 2. Move binary kubemarine to a separate folder 
 3. Now you can proceed to run Kubemarine! Try the following:
@@ -80,15 +80,15 @@
    ```bash
    python3 -m pip install --upgrade pip
    ```
    Windows:
    ```bash
    python -m pip install --upgrade pip
    ```
-1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#prerequisites-for-deployment-node).
+1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#prerequisites-for-deployment-node).
 1. Create and activate a [virtual environment](https://realpython.com/python-virtual-environments-a-primer/) if necessary.
 1. Install Kubemarine package.
 
    Linux / MacOS:
    ```bash
    python3 -m pip install kubemarine
    ```
@@ -99,15 +99,15 @@
 1. Now you can proceed to run Kubemarine! Try the following:
    ```bash
    kubemarine help
    ```
 
 
 ## Kubemarine Installation from Sources
-Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.1/README.md#kubemarine-package-installation).
+Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.2/README.md#kubemarine-package-installation).
 The exception is instead of installing the package from [PyPI](https://pypi.org/project/kubemarine/), do the following:
 1. [Download the latest release](https://github.com/netcracker/kubemarine/releases) or clone the repository:
    ```bash
    git clone https://github.com/netcracker/kubemarine.git
    ```
 1. Unpack the project from the archive if required:
    ```bash
@@ -128,24 +128,24 @@
    python -m pip install -e .
    ```
 1. Now you can proceed to run Kubemarine. Try the following:
     ```bash
     kubemarine help
     ```
 
-**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.18.1/Dockerfile) is also available.
+**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.18.2/Dockerfile) is also available.
 
 
 **Note:** Kubemarine debugging available via `kubemarine/__main__.py`.
 
 
 ## Running Cluster Installation
 To install a Kubernetes cluster using Kubemarine:
-1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#prerequisites-for-cluster-nodes).
-1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.18.1/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
+1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#prerequisites-for-cluster-nodes).
+1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.18.2/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
    ```yaml
    node_defaults:
      keyfile: "/home/username/.ssh/id_rsa"
      username: "centos"
 
    vrrp_ips:
      - 192.168.0.250
@@ -173,42 +173,42 @@
    kubemarine install
    ```
 1. Check the health of the newly installed cluster:
    ```bash
    kubemarine check_paas
    ```
 
-For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.18.1/README.md#documentation).
+For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.18.2/README.md#documentation).
 
 ## Kubemarine Docker Installation
 To start, download the Kubmarine image ```docker pull ghcr.io/netcracker/kubemarine:main```
 
 Run Kubemarine from the container, for example:
    ```
    docker run -it --mount type=bind,source=/root/cluster.yaml,target=/opt/kubemarine/cluster.yaml --mount type=bind,source=/root/rsa_key,target=/opt/kubemarine/rsa_key kubemarine install -c /opt/kubemarine/cluster.yaml
    ```
    *Note*: Do not forget to pass the inventory file and connection key inside the container.
    For more execution details, refer to ["Installation of Kubernetes using CLI" guide on Github](https://github.com/Netcracker/kubemarine/blob/main/documentation/Installation.md#installation-of-kubernetes-using-cli).
 
 ## Documentation
 The following documents and tutorials are available:
-- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md)
-- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md)
-- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Troubleshooting.md)
-- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Kubecheck.md)
-- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Logging.md)
+- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Installation.md)
+- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Maintenance.md)
+- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Troubleshooting.md)
+- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Kubecheck.md)
+- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.18.2/documentation/Logging.md)
 
 Also, check out the following inventory examples:
-- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.1/examples/cluster.yaml)
-- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.1/examples/procedure.yaml)
+- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.2/examples/cluster.yaml)
+- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.2/examples/procedure.yaml)
 
 ## Issues, Questions
 If you have any problems while working with Kubemarine, feel free to open a [new issue](https://github.com/netcracker/kubemarine/issues) or even
 [PR](https://github.com/netcracker/kubemarine/pulls) with related changes.
-Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.18.1/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
+Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.18.2/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
 
-In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.18.1/SECURITY.md)
+In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.18.2/SECURITY.md)
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/netcracker/kubemarine/releases).
 
 ## License
-[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.18.1/LICENSE)
+[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.18.2/LICENSE)
```

### Comparing `kubemarine-0.18.1/kubemarine.egg-info/SOURCES.txt` & `kubemarine-0.18.2/kubemarine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.1/pyproject.toml` & `kubemarine-0.18.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 Documentation = "https://github.com/Netcracker/KubeMarine#documentation"
 Issues = "https://github.com/Netcracker/KubeMarine/issues/"
 
 # To change version with automatic push and triggering of the release workflow use
 # 1. pip install bumpver
 # 2. bumpver update --set-version <new version>
 [tool.bumpver]
-current_version = "0.18.1"
+current_version = "0.18.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version to {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `kubemarine-0.18.1/setup.py` & `kubemarine-0.18.2/setup.py`

 * *Files identical despite different names*

