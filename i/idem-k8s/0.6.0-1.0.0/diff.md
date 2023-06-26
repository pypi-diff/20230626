# Comparing `tmp/idem-k8s-0.6.0.tar.gz` & `tmp/idem-k8s-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-k8s-0.6.0.tar", last modified: Fri Apr 28 14:35:30 2023, max compression
+gzip compressed data, was "idem-k8s-1.0.0.tar", last modified: Mon Jun 26 15:50:08 2023, max compression
```

## Comparing `idem-k8s-0.6.0.tar` & `idem-k8s-1.0.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/
--rw-r--r--   0 root         (0) root         (0)    11336 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7122 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6284 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/acct/k8s/
--rw-r--r--   0 root         (0) root         (0)      547 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/acct/k8s/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/autogen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/autogen/k8s/
--rw-r--r--   0 root         (0) root         (0)     1580 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/autogen/k8s/init.py
--rw-r--r--   0 root         (0) root         (0)     6464 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/autogen/k8s/openapi_spec_parser.py
--rw-r--r--   0 root         (0) root         (0)     3901 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/autogen/k8s/plugin.py
--rw-r--r--   0 root         (0) root         (0)    10897 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/autogen/k8s/template.py
--rw-r--r--   0 root         (0) root         (0)      631 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/autogen/k8s/type.py
--rw-r--r--   0 root         (0) root         (0)      486 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/exec/k8s/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/exec/k8s/apiregistration_k8s_io/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/exec/k8s/apiregistration_k8s_io/v1/
--rw-r--r--   0 root         (0) root         (0)     3837 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/exec/k8s/apiregistration_k8s_io/v1/api_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/exec/k8s/core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/exec/k8s/core/v1/
--rw-r--r--   0 root         (0) root         (0)     4356 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/exec/k8s/core/v1/persistent_volume_claim.py
--rw-r--r--   0 root         (0) root         (0)     2578 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/exec/k8s/core/v1/service.py
--rw-r--r--   0 root         (0) root         (0)      574 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/exec/k8s/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/exec/k8s/rbac/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/exec/k8s/rbac/v1/
--rw-r--r--   0 root         (0) root         (0)     4595 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/exec/k8s/rbac/v1/role_binding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/states/k8s/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/states/k8s/apiregistration_k8s_io/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/states/k8s/apiregistration_k8s_io/v1/
--rw-r--r--   0 root         (0) root         (0)     9891 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/apiregistration_k8s_io/v1/api_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/states/k8s/apps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/states/k8s/apps/v1/
--rw-r--r--   0 root         (0) root         (0)    13115 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/apps/v1/daemon_set.py
--rw-r--r--   0 root         (0) root         (0)    13334 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/apps/v1/deployment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/states/k8s/core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/
--rw-r--r--   0 root         (0) root         (0)    10073 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/config_map.py
--rw-r--r--   0 root         (0) root         (0)     9167 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/namespace.py
--rw-r--r--   0 root         (0) root         (0)    11017 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/persistent_volume_claim.py
--rw-r--r--   0 root         (0) root         (0)     9756 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/secret.py
--rw-r--r--   0 root         (0) root         (0)    11114 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/service.py
--rw-r--r--   0 root         (0) root         (0)    10444 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/service_account.py
--rw-r--r--   0 root         (0) root         (0)      165 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/states/k8s/rbac/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/idem_k8s/states/k8s/rbac/v1/
--rw-r--r--   0 root         (0) root         (0)     8356 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/rbac/v1/cluster_role.py
--rw-r--r--   0 root         (0) root         (0)     9040 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/rbac/v1/cluster_role_binding.py
--rw-r--r--   0 root         (0) root         (0)     9953 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/rbac/v1/role_binding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/states/k8s/storage_k8s_io/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/idem_k8s/states/k8s/storage_k8s_io/v1/
--rw-r--r--   0 root         (0) root         (0)    10373 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/storage_k8s_io/v1/storage_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/idem_k8s/tool/k8s/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/tool/k8s/apiregistration_k8s_io/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/idem_k8s/tool/k8s/apiregistration_k8s_io/v1/
--rw-r--r--   0 root         (0) root         (0)      653 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/apiregistration_k8s_io/v1/api_service_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/tool/k8s/apps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/idem_k8s/tool/k8s/apps/v1/
--rw-r--r--   0 root         (0) root         (0)      905 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/apps/v1/daemon_set_utils.py
--rw-r--r--   0 root         (0) root         (0)     3051 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/apps/v1/deployment_utils.py
--rw-r--r--   0 root         (0) root         (0)     2297 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/client.py
--rw-r--r--   0 root         (0) root         (0)     1280 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/comment_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/tool/k8s/core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/
--rw-r--r--   0 root         (0) root         (0)      714 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/config_map_utils.py
--rw-r--r--   0 root         (0) root         (0)      665 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/namespace_utils.py
--rw-r--r--   0 root         (0) root         (0)      756 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/persistent_volume_claim_utils.py
--rw-r--r--   0 root         (0) root         (0)      694 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/secret_utils.py
--rw-r--r--   0 root         (0) root         (0)      779 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/service_account_utils.py
--rw-r--r--   0 root         (0) root         (0)      845 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/service_utils.py
--rw-r--r--   0 root         (0) root         (0)     1529 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/custom_waiter.py
--rw-r--r--   0 root         (0) root         (0)     3138 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/marshaller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/tool/k8s/rbac/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/idem_k8s/tool/k8s/rbac/v1/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/rbac/v1/cluster_role_binding_utils.py
--rw-r--r--   0 root         (0) root         (0)      700 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/rbac/v1/cluster_role_utils.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/rbac/v1/role_binding_utils.py
--rw-r--r--   0 root         (0) root         (0)     1992 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/resolve.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/state_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/tool/k8s/storage_k8s_io/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/idem_k8s/tool/k8s/storage_k8s_io/v1/
--rw-r--r--   0 root         (0) root         (0)      848 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/storage_k8s_io/v1/storage_class_utils.py
--rw-r--r--   0 root         (0) root         (0)     1340 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/test_state_utils.py
--rw-r--r--   0 root         (0) root         (0)     1550 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/waiter_utils.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-28 14:35:30.000000 idem-k8s-0.6.0/idem_k8s/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7122 2023-04-28 14:35:30.000000 idem-k8s-0.6.0/idem_k8s.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2225 2023-04-28 14:35:30.000000 idem-k8s-0.6.0/idem_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 14:35:30.000000 idem-k8s-0.6.0/idem_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-28 14:35:30.000000 idem-k8s-0.6.0/idem_k8s.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      144 2023-04-28 14:35:30.000000 idem-k8s-0.6.0/idem_k8s.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-28 14:35:30.000000 idem-k8s-0.6.0/idem_k8s.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2783 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.207196 idem-k8s-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11336 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7122 2023-06-26 15:50:08.207196 idem-k8s-1.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6284 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/acct/k8s/
+-rw-r--r--   0 root         (0) root         (0)      547 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/acct/k8s/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/autogen/k8s/
+-rw-r--r--   0 root         (0) root         (0)     1580 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/autogen/k8s/init.py
+-rw-r--r--   0 root         (0) root         (0)     6464 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/autogen/k8s/openapi_spec_parser.py
+-rw-r--r--   0 root         (0) root         (0)     3901 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/autogen/k8s/plugin.py
+-rw-r--r--   0 root         (0) root         (0)    10897 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/autogen/k8s/template.py
+-rw-r--r--   0 root         (0) root         (0)      631 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/autogen/k8s/type.py
+-rw-r--r--   0 root         (0) root         (0)      486 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/exec/k8s/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/exec/k8s/apiregistration_k8s_io/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/exec/k8s/apiregistration_k8s_io/v1/
+-rw-r--r--   0 root         (0) root         (0)     3837 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/exec/k8s/apiregistration_k8s_io/v1/api_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/exec/k8s/core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/exec/k8s/core/v1/
+-rw-r--r--   0 root         (0) root         (0)     4356 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/exec/k8s/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 root         (0) root         (0)     2578 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/exec/k8s/core/v1/service.py
+-rw-r--r--   0 root         (0) root         (0)      574 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/exec/k8s/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/exec/k8s/rbac/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/exec/k8s/rbac/v1/
+-rw-r--r--   0 root         (0) root         (0)     4595 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/exec/k8s/rbac/v1/role_binding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/states/k8s/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/states/k8s/apiregistration_k8s_io/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/states/k8s/apiregistration_k8s_io/v1/
+-rw-r--r--   0 root         (0) root         (0)     9891 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/states/k8s/apiregistration_k8s_io/v1/api_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/states/k8s/apps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/states/k8s/apps/v1/
+-rw-r--r--   0 root         (0) root         (0)    13115 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/states/k8s/apps/v1/daemon_set.py
+-rw-r--r--   0 root         (0) root         (0)    13334 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/states/k8s/apps/v1/deployment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/states/k8s/core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.207196 idem-k8s-1.0.0/idem_k8s/states/k8s/core/v1/
+-rw-r--r--   0 root         (0) root         (0)    10073 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/states/k8s/core/v1/config_map.py
+-rw-r--r--   0 root         (0) root         (0)     9167 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/states/k8s/core/v1/namespace.py
+-rw-r--r--   0 root         (0) root         (0)    11017 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/states/k8s/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 root         (0) root         (0)     9756 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/states/k8s/core/v1/secret.py
+-rw-r--r--   0 root         (0) root         (0)    11114 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/states/k8s/core/v1/service.py
+-rw-r--r--   0 root         (0) root         (0)    10444 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/states/k8s/core/v1/service_account.py
+-rw-r--r--   0 root         (0) root         (0)      165 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/states/k8s/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/states/k8s/rbac/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.207196 idem-k8s-1.0.0/idem_k8s/states/k8s/rbac/v1/
+-rw-r--r--   0 root         (0) root         (0)     8356 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/states/k8s/rbac/v1/cluster_role.py
+-rw-r--r--   0 root         (0) root         (0)     9040 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/states/k8s/rbac/v1/cluster_role_binding.py
+-rw-r--r--   0 root         (0) root         (0)     9953 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/states/k8s/rbac/v1/role_binding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/states/k8s/storage_k8s_io/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.207196 idem-k8s-1.0.0/idem_k8s/states/k8s/storage_k8s_io/v1/
+-rw-r--r--   0 root         (0) root         (0)    10373 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/states/k8s/storage_k8s_io/v1/storage_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.207196 idem-k8s-1.0.0/idem_k8s/tool/k8s/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/tool/k8s/apiregistration_k8s_io/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.207196 idem-k8s-1.0.0/idem_k8s/tool/k8s/apiregistration_k8s_io/v1/
+-rw-r--r--   0 root         (0) root         (0)      653 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/tool/k8s/apiregistration_k8s_io/v1/api_service_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/tool/k8s/apps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.207196 idem-k8s-1.0.0/idem_k8s/tool/k8s/apps/v1/
+-rw-r--r--   0 root         (0) root         (0)      905 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/tool/k8s/apps/v1/daemon_set_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3051 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/tool/k8s/apps/v1/deployment_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/tool/k8s/client.py
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/tool/k8s/comment_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/tool/k8s/core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.207196 idem-k8s-1.0.0/idem_k8s/tool/k8s/core/v1/
+-rw-r--r--   0 root         (0) root         (0)      714 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/tool/k8s/core/v1/config_map_utils.py
+-rw-r--r--   0 root         (0) root         (0)      665 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/tool/k8s/core/v1/namespace_utils.py
+-rw-r--r--   0 root         (0) root         (0)      756 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/tool/k8s/core/v1/persistent_volume_claim_utils.py
+-rw-r--r--   0 root         (0) root         (0)      694 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/tool/k8s/core/v1/secret_utils.py
+-rw-r--r--   0 root         (0) root         (0)      779 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/tool/k8s/core/v1/service_account_utils.py
+-rw-r--r--   0 root         (0) root         (0)      845 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/tool/k8s/core/v1/service_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/tool/k8s/custom_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     3138 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/tool/k8s/marshaller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/tool/k8s/rbac/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.207196 idem-k8s-1.0.0/idem_k8s/tool/k8s/rbac/v1/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/tool/k8s/rbac/v1/cluster_role_binding_utils.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/tool/k8s/rbac/v1/cluster_role_utils.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/tool/k8s/rbac/v1/role_binding_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/tool/k8s/resolve.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/tool/k8s/state_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s/tool/k8s/storage_k8s_io/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.207196 idem-k8s-1.0.0/idem_k8s/tool/k8s/storage_k8s_io/v1/
+-rw-r--r--   0 root         (0) root         (0)      848 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/tool/k8s/storage_k8s_io/v1/storage_class_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/tool/k8s/test_state_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/idem_k8s/tool/k8s/waiter_utils.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-26 15:50:07.000000 idem-k8s-1.0.0/idem_k8s/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:50:08.203196 idem-k8s-1.0.0/idem_k8s.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7122 2023-06-26 15:50:08.000000 idem-k8s-1.0.0/idem_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-06-26 15:50:08.000000 idem-k8s-1.0.0/idem_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 15:50:08.000000 idem-k8s-1.0.0/idem_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-26 15:50:08.000000 idem-k8s-1.0.0/idem_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      144 2023-06-26 15:50:08.000000 idem-k8s-1.0.0/idem_k8s.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-26 15:50:08.000000 idem-k8s-1.0.0/idem_k8s.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-26 15:50:08.207196 idem-k8s-1.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2783 2023-06-26 15:49:54.000000 idem-k8s-1.0.0/setup.py
```

### Comparing `idem-k8s-0.6.0/LICENSE` & `idem-k8s-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/PKG-INFO` & `idem-k8s-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-k8s
-Version: 0.6.0
+Version: 1.0.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Naresh
 Author-email: nkumar5@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
@@ -98,15 +98,15 @@
    -n idem_k8s \
    --resource apps/v1/DaemonSet  # resource for which state files are generated
 
 The ``resource`` argument follows the format: ``group/version/kind``
 
 For example, to add a resource state for Deployment, the argument is: ``apps/v1/Deployment``
 
-For more information, see the `Kubernetes resource objects documentation <https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.22/#-strong-api-groups-strong>`__.
+For more information, see the `Kubernetes resource objects documentation <https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.23/#-strong-api-groups-strong>`__.
 
 Usage
 =====
 
 Setup
 -----
```

### Comparing `idem-k8s-0.6.0/README.rst` & `idem-k8s-1.0.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
    -n idem_k8s \
    --resource apps/v1/DaemonSet  # resource for which state files are generated
 
 The ``resource`` argument follows the format: ``group/version/kind``
 
 For example, to add a resource state for Deployment, the argument is: ``apps/v1/Deployment``
 
-For more information, see the `Kubernetes resource objects documentation <https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.22/#-strong-api-groups-strong>`__.
+For more information, see the `Kubernetes resource objects documentation <https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.23/#-strong-api-groups-strong>`__.
 
 Usage
 =====
 
 Setup
 -----
```

### Comparing `idem-k8s-0.6.0/idem_k8s/acct/k8s/init.py` & `idem-k8s-1.0.0/idem_k8s/acct/k8s/init.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/autogen/k8s/init.py` & `idem-k8s-1.0.0/idem_k8s/autogen/k8s/init.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/autogen/k8s/openapi_spec_parser.py` & `idem-k8s-1.0.0/idem_k8s/autogen/k8s/openapi_spec_parser.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/autogen/k8s/plugin.py` & `idem-k8s-1.0.0/idem_k8s/autogen/k8s/plugin.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/autogen/k8s/template.py` & `idem-k8s-1.0.0/idem_k8s/autogen/k8s/template.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/autogen/k8s/type.py` & `idem-k8s-1.0.0/idem_k8s/autogen/k8s/type.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/exec/k8s/apiregistration_k8s_io/v1/api_service.py` & `idem-k8s-1.0.0/idem_k8s/exec/k8s/apiregistration_k8s_io/v1/api_service.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/exec/k8s/core/v1/persistent_volume_claim.py` & `idem-k8s-1.0.0/idem_k8s/exec/k8s/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/exec/k8s/core/v1/service.py` & `idem-k8s-1.0.0/idem_k8s/exec/k8s/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/exec/k8s/init.py` & `idem-k8s-1.0.0/idem_k8s/exec/k8s/init.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/exec/k8s/rbac/v1/role_binding.py` & `idem-k8s-1.0.0/idem_k8s/exec/k8s/rbac/v1/role_binding.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/states/k8s/apiregistration_k8s_io/v1/api_service.py` & `idem-k8s-1.0.0/idem_k8s/states/k8s/apiregistration_k8s_io/v1/api_service.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/states/k8s/apps/v1/daemon_set.py` & `idem-k8s-1.0.0/idem_k8s/states/k8s/apps/v1/daemon_set.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/states/k8s/apps/v1/deployment.py` & `idem-k8s-1.0.0/idem_k8s/states/k8s/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/config_map.py` & `idem-k8s-1.0.0/idem_k8s/states/k8s/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/namespace.py` & `idem-k8s-1.0.0/idem_k8s/states/k8s/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/persistent_volume_claim.py` & `idem-k8s-1.0.0/idem_k8s/states/k8s/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/secret.py` & `idem-k8s-1.0.0/idem_k8s/states/k8s/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/service.py` & `idem-k8s-1.0.0/idem_k8s/states/k8s/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/service_account.py` & `idem-k8s-1.0.0/idem_k8s/states/k8s/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/states/k8s/rbac/v1/cluster_role.py` & `idem-k8s-1.0.0/idem_k8s/states/k8s/rbac/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/states/k8s/rbac/v1/cluster_role_binding.py` & `idem-k8s-1.0.0/idem_k8s/states/k8s/rbac/v1/cluster_role_binding.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/states/k8s/rbac/v1/role_binding.py` & `idem-k8s-1.0.0/idem_k8s/states/k8s/rbac/v1/role_binding.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/states/k8s/storage_k8s_io/v1/storage_class.py` & `idem-k8s-1.0.0/idem_k8s/states/k8s/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/tool/k8s/apiregistration_k8s_io/v1/api_service_utils.py` & `idem-k8s-1.0.0/idem_k8s/tool/k8s/apiregistration_k8s_io/v1/api_service_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/tool/k8s/apps/v1/daemon_set_utils.py` & `idem-k8s-1.0.0/idem_k8s/tool/k8s/apps/v1/daemon_set_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/tool/k8s/apps/v1/deployment_utils.py` & `idem-k8s-1.0.0/idem_k8s/tool/k8s/apps/v1/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/tool/k8s/client.py` & `idem-k8s-1.0.0/idem_k8s/tool/k8s/client.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/tool/k8s/comment_utils.py` & `idem-k8s-1.0.0/idem_k8s/tool/k8s/comment_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/config_map_utils.py` & `idem-k8s-1.0.0/idem_k8s/tool/k8s/core/v1/config_map_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/namespace_utils.py` & `idem-k8s-1.0.0/idem_k8s/tool/k8s/core/v1/namespace_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/persistent_volume_claim_utils.py` & `idem-k8s-1.0.0/idem_k8s/tool/k8s/core/v1/persistent_volume_claim_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/secret_utils.py` & `idem-k8s-1.0.0/idem_k8s/tool/k8s/core/v1/secret_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/service_account_utils.py` & `idem-k8s-1.0.0/idem_k8s/tool/k8s/core/v1/service_account_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/service_utils.py` & `idem-k8s-1.0.0/idem_k8s/tool/k8s/core/v1/service_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/tool/k8s/custom_waiter.py` & `idem-k8s-1.0.0/idem_k8s/tool/k8s/custom_waiter.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/tool/k8s/marshaller.py` & `idem-k8s-1.0.0/idem_k8s/tool/k8s/marshaller.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/tool/k8s/rbac/v1/cluster_role_binding_utils.py` & `idem-k8s-1.0.0/idem_k8s/tool/k8s/rbac/v1/cluster_role_binding_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/tool/k8s/rbac/v1/cluster_role_utils.py` & `idem-k8s-1.0.0/idem_k8s/tool/k8s/rbac/v1/cluster_role_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/tool/k8s/rbac/v1/role_binding_utils.py` & `idem-k8s-1.0.0/idem_k8s/tool/k8s/rbac/v1/role_binding_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/tool/k8s/resolve.py` & `idem-k8s-1.0.0/idem_k8s/tool/k8s/resolve.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/tool/k8s/state_utils.py` & `idem-k8s-1.0.0/idem_k8s/tool/k8s/state_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/tool/k8s/storage_k8s_io/v1/storage_class_utils.py` & `idem-k8s-1.0.0/idem_k8s/tool/k8s/storage_k8s_io/v1/storage_class_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/tool/k8s/test_state_utils.py` & `idem-k8s-1.0.0/idem_k8s/tool/k8s/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s/tool/k8s/waiter_utils.py` & `idem-k8s-1.0.0/idem_k8s/tool/k8s/waiter_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/idem_k8s.egg-info/PKG-INFO` & `idem-k8s-1.0.0/idem_k8s.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-k8s
-Version: 0.6.0
+Version: 1.0.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Naresh
 Author-email: nkumar5@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
@@ -98,15 +98,15 @@
    -n idem_k8s \
    --resource apps/v1/DaemonSet  # resource for which state files are generated
 
 The ``resource`` argument follows the format: ``group/version/kind``
 
 For example, to add a resource state for Deployment, the argument is: ``apps/v1/Deployment``
 
-For more information, see the `Kubernetes resource objects documentation <https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.22/#-strong-api-groups-strong>`__.
+For more information, see the `Kubernetes resource objects documentation <https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.23/#-strong-api-groups-strong>`__.
 
 Usage
 =====
 
 Setup
 -----
```

### Comparing `idem-k8s-0.6.0/idem_k8s.egg-info/SOURCES.txt` & `idem-k8s-1.0.0/idem_k8s.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.6.0/setup.py` & `idem-k8s-1.0.0/setup.py`

 * *Files identical despite different names*

