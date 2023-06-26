# Comparing `tmp/dask-kubernetes-2023.3.2.tar.gz` & `tmp/dask-kubernetes-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-kubernetes-2023.3.2.tar", last modified: Thu Mar 30 13:14:12 2023, max compression
+gzip compressed data, was "dask-kubernetes-2023.6.0.tar", last modified: Mon Jun 26 10:34:03 2023, max compression
```

## Comparing `dask-kubernetes-2023.3.2.tar` & `dask-kubernetes-2023.6.0.tar`

### file list

```diff
@@ -1,114 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.304029 dask-kubernetes-2023.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-03-30 13:14:12.304029 dask-kubernetes-2023.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.308029 dask-kubernetes-2023.3.2/dask_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-30 13:14:12.308029 dask-kubernetes-2023.3.2/dask_kubernetes/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.300029 dask-kubernetes-2023.3.2/dask_kubernetes/aiopykube/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/aiopykube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/aiopykube/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/aiopykube/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/aiopykube/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/aiopykube/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.300029 dask-kubernetes-2023.3.2/dask_kubernetes/aiopykube/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/aiopykube/tests/test_pykube_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/aiopykube/tests/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.300029 dask-kubernetes-2023.3.2/dask_kubernetes/classic/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/classic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28557 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/classic/kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.300029 dask-kubernetes-2023.3.2/dask_kubernetes/classic/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/classic/tests/config-demo.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/classic/tests/fake_gcp_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    28677 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/classic/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/classic/tests/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.300029 dask-kubernetes-2023.3.2/dask_kubernetes/common/
--rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/common/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/common/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/common/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.300029 dask-kubernetes-2023.3.2/dask_kubernetes/common/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/common/tests/test_kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/common/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.300029 dask-kubernetes-2023.3.2/dask_kubernetes/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.300029 dask-kubernetes-2023.3.2/dask_kubernetes/helm/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/helm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/helm/helmcluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.300029 dask-kubernetes-2023.3.2/dask_kubernetes/helm/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.300029 dask-kubernetes-2023.3.2/dask_kubernetes/helm/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/helm/tests/resources/values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/helm/tests/test_helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/kubernetes.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.300029 dask-kubernetes-2023.3.2/dask_kubernetes/operator/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.300029 dask-kubernetes-2023.3.2/dask_kubernetes/operator/controller/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31019 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/controller/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.300029 dask-kubernetes-2023.3.2/dask_kubernetes/operator/controller/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/controller/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.300029 dask-kubernetes-2023.3.2/dask_kubernetes/operator/controller/plugins/noop/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/controller/plugins/noop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/controller/plugins/noop/noop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.300029 dask-kubernetes-2023.3.2/dask_kubernetes/operator/controller/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.304029 dask-kubernetes-2023.3.2/dask_kubernetes/operator/controller/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16428 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/controller/tests/test_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.304029 dask-kubernetes-2023.3.2/dask_kubernetes/operator/customresources/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/customresources/daskautoscaler.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/customresources/daskautoscaler.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/customresources/daskcluster.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/customresources/daskcluster.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/customresources/daskjob.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/customresources/daskjob.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/customresources/daskworkergroup.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/customresources/daskworkergroup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/customresources/templates.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.296028 dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.304029 dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/chartpress.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.304029 dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.304029 dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   283457 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   471055 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   140466 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.304029 dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/rolebinding.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/serviceaccount.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.304029 dask-kubernetes-2023.3.2/dask_kubernetes/operator/kubecluster/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/kubecluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/kubecluster/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    39891 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/kubecluster/kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.304029 dask-kubernetes-2023.3.2/dask_kubernetes/operator/kubecluster/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/kubecluster/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/kubecluster/tests/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:14:12.300029 dask-kubernetes-2023.3.2/dask_kubernetes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-03-30 13:14:12.000000 dask-kubernetes-2023.3.2/dask_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-03-30 13:14:12.000000 dask-kubernetes-2023.3.2/dask_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 13:14:12.000000 dask-kubernetes-2023.3.2/dask_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-30 13:14:12.000000 dask-kubernetes-2023.3.2/dask_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 13:14:12.000000 dask-kubernetes-2023.3.2/dask_kubernetes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-30 13:14:12.000000 dask-kubernetes-2023.3.2/dask_kubernetes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-30 13:14:12.000000 dask-kubernetes-2023.3.2/dask_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-03-30 13:14:12.308029 dask-kubernetes-2023.3.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      969 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68747 2023-03-30 13:14:06.000000 dask-kubernetes-2023.3.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.161355 dask-kubernetes-2023.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-26 10:34:03.165355 dask-kubernetes-2023.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.165355 dask-kubernetes-2023.6.0/dask_kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-26 10:34:03.165355 dask-kubernetes-2023.6.0/dask_kubernetes/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.145355 dask-kubernetes-2023.6.0/dask_kubernetes/aiopykube/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/aiopykube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/aiopykube/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/aiopykube/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/aiopykube/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/aiopykube/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.149355 dask-kubernetes-2023.6.0/dask_kubernetes/aiopykube/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/aiopykube/tests/test_pykube_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/aiopykube/tests/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.149355 dask-kubernetes-2023.6.0/dask_kubernetes/classic/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/classic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28558 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/classic/kubecluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.153355 dask-kubernetes-2023.6.0/dask_kubernetes/classic/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/classic/tests/config-demo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/classic/tests/fake_gcp_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28838 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/classic/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/classic/tests/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.153355 dask-kubernetes-2023.6.0/dask_kubernetes/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.153355 dask-kubernetes-2023.6.0/dask_kubernetes/common/
+-rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/common/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/common/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/common/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.153355 dask-kubernetes-2023.6.0/dask_kubernetes/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/common/tests/test_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/common/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.153355 dask-kubernetes-2023.6.0/dask_kubernetes/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.153355 dask-kubernetes-2023.6.0/dask_kubernetes/helm/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/helm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/helm/helmcluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.153355 dask-kubernetes-2023.6.0/dask_kubernetes/helm/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.153355 dask-kubernetes-2023.6.0/dask_kubernetes/helm/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/helm/tests/resources/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/helm/tests/test_helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/kubernetes.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.153355 dask-kubernetes-2023.6.0/dask_kubernetes/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.153355 dask-kubernetes-2023.6.0/dask_kubernetes/operator/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37016 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/controller/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.157355 dask-kubernetes-2023.6.0/dask_kubernetes/operator/controller/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/controller/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.157355 dask-kubernetes-2023.6.0/dask_kubernetes/operator/controller/plugins/noop/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/controller/plugins/noop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/controller/plugins/noop/noop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.157355 dask-kubernetes-2023.6.0/dask_kubernetes/operator/controller/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.157355 dask-kubernetes-2023.6.0/dask_kubernetes/operator/controller/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    24649 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/controller/tests/test_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.157355 dask-kubernetes-2023.6.0/dask_kubernetes/operator/customresources/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/customresources/daskautoscaler.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/customresources/daskautoscaler.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/customresources/daskcluster.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/customresources/daskcluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/customresources/daskjob.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/customresources/daskjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/customresources/daskworkergroup.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/customresources/daskworkergroup.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/customresources/templates.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.137355 dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.157355 dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/chartpress.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.157355 dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.161355 dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   283847 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   471240 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   140704 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.161355 dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/rolebinding.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/serviceaccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.161355 dask-kubernetes-2023.6.0/dask_kubernetes/operator/kubecluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/kubecluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/kubecluster/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42764 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/kubecluster/kubecluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.161355 dask-kubernetes-2023.6.0/dask_kubernetes/operator/kubecluster/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/kubecluster/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/kubecluster/tests/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:34:03.145355 dask-kubernetes-2023.6.0/dask_kubernetes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-26 10:34:03.000000 dask-kubernetes-2023.6.0/dask_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-26 10:34:03.000000 dask-kubernetes-2023.6.0/dask_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 10:34:03.000000 dask-kubernetes-2023.6.0/dask_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-26 10:34:03.000000 dask-kubernetes-2023.6.0/dask_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 10:34:03.000000 dask-kubernetes-2023.6.0/dask_kubernetes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 10:34:03.000000 dask-kubernetes-2023.6.0/dask_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 10:34:03.000000 dask-kubernetes-2023.6.0/dask_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-26 10:34:03.165355 dask-kubernetes-2023.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1032 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68747 2023-06-26 10:33:56.000000 dask-kubernetes-2023.6.0/versioneer.py
```

### Comparing `dask-kubernetes-2023.3.2/LICENSE` & `dask-kubernetes-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/PKG-INFO` & `dask-kubernetes-2023.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: dask-kubernetes
-Version: 2023.3.2
+Version: 2023.6.0
 Summary: Native Kubernetes integration for Dask
 Home-page: https://github.com/dask/dask-kubernetes
 Maintainer: Jacob Tomlinson
 License: BSD
-Description: Dask Kubernetes
-        ===============
-        
-        
-        .. image:: https://github.com/dask/dask-kubernetes/workflows/CI/badge.svg
-           :target: https://github.com/dask/dask-kubernetes/actions?query=workflow%3ACI
-        
-        .. image:: https://img.shields.io/readthedocs/dask-kubernetes?color=%232980B9&logo=read-the-docs&logoColor=white
-           :target: https://kubernetes.dask.org/
-           :alt: Read the Docs
-        
-        .. image:: https://img.shields.io/readthedocs/dask-kubernetes?color=%232980B9&label=developer%20docs&logo=read-the-docs&logoColor=white
-           :target: https://kubernetes.dask.org/releasing.html
-           :alt: Read the Docs Developer
-        
-        .. image:: https://img.shields.io/pypi/v/dask-kubernetes
-           :target: https://pypi.org/project/dask-kubernetes/
-           :alt: PyPI
-        
-        .. image:: https://img.shields.io/conda/vn/conda-forge/dask-kubernetes
-           :target: https://anaconda.org/conda-forge/dask-kubernetes
-           :alt: Conda Forge
-        
-        .. image:: https://img.shields.io/badge/python%20support-3.8%7C3.9%7C3.10-blue
-           :target: https://kubernetes.dask.org/en/latest/installing.html#supported-versions
-           :alt: Python Support
-        
-        .. image:: https://img.shields.io/badge/Kubernetes%20support-1.22%7C1.23%7C1.24%7C1.25-blue
-           :target: https://kubernetes.dask.org/en/latest/installing.html#supported-versions
-           :alt: Kubernetes Support
-        
-        
-        Native Kubernetes integration for Dask.
-        
 Keywords: dask,kubernetes,distributed
-Platform: UNKNOWN
-Requires-Python: >=3.8
+Requires-Python: >=3.9
+License-File: LICENSE
+
+Dask Kubernetes
+===============
+
+
+.. image:: https://github.com/dask/dask-kubernetes/workflows/CI/badge.svg
+   :target: https://github.com/dask/dask-kubernetes/actions?query=workflow%3ACI
+
+.. image:: https://img.shields.io/readthedocs/dask-kubernetes?color=%232980B9&logo=read-the-docs&logoColor=white
+   :target: https://kubernetes.dask.org/
+   :alt: Read the Docs
+
+.. image:: https://img.shields.io/readthedocs/dask-kubernetes?color=%232980B9&label=developer%20docs&logo=read-the-docs&logoColor=white
+   :target: https://kubernetes.dask.org/releasing.html
+   :alt: Read the Docs Developer
+
+.. image:: https://img.shields.io/pypi/v/dask-kubernetes
+   :target: https://pypi.org/project/dask-kubernetes/
+   :alt: PyPI
+
+.. image:: https://img.shields.io/conda/vn/conda-forge/dask-kubernetes
+   :target: https://anaconda.org/conda-forge/dask-kubernetes
+   :alt: Conda Forge
+
+.. image:: https://img.shields.io/badge/python%20support-3.9%7C3.10-blue
+   :target: https://kubernetes.dask.org/en/latest/installing.html#supported-versions
+   :alt: Python Support
+
+.. image:: https://img.shields.io/badge/Kubernetes%20support-1.24%7C1.25%7C1.26%7C1.27-blue
+   :target: https://kubernetes.dask.org/en/latest/installing.html#supported-versions
+   :alt: Kubernetes Support
+
+
+Native Kubernetes integration for Dask.
```

### Comparing `dask-kubernetes-2023.3.2/README.rst` & `dask-kubernetes-2023.6.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -17,17 +17,17 @@
    :target: https://pypi.org/project/dask-kubernetes/
    :alt: PyPI
 
 .. image:: https://img.shields.io/conda/vn/conda-forge/dask-kubernetes
    :target: https://anaconda.org/conda-forge/dask-kubernetes
    :alt: Conda Forge
 
-.. image:: https://img.shields.io/badge/python%20support-3.8%7C3.9%7C3.10-blue
+.. image:: https://img.shields.io/badge/python%20support-3.9%7C3.10-blue
    :target: https://kubernetes.dask.org/en/latest/installing.html#supported-versions
    :alt: Python Support
 
-.. image:: https://img.shields.io/badge/Kubernetes%20support-1.22%7C1.23%7C1.24%7C1.25-blue
+.. image:: https://img.shields.io/badge/Kubernetes%20support-1.24%7C1.25%7C1.26%7C1.27-blue
    :target: https://kubernetes.dask.org/en/latest/installing.html#supported-versions
    :alt: Kubernetes Support
 
 
 Native Kubernetes integration for Dask.
```

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/__init__.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/aiopykube/dask.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/aiopykube/dask.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/aiopykube/mixins.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/aiopykube/mixins.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/aiopykube/objects.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/aiopykube/objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/aiopykube/query.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/aiopykube/query.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/aiopykube/tests/test_pykube_objects.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/aiopykube/tests/test_pykube_objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/aiopykube/tests/test_query.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/aiopykube/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/classic/kubecluster.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/classic/kubecluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 logger = logging.getLogger(__name__)
 
 SCHEDULER_PORT = 8786
 
 
 class Pod(ProcessInterface):
     """A superclass for Kubernetes Pods
+
     See Also
     --------
     Worker
     Scheduler
     """
 
     def __init__(
```

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/classic/tests/config-demo.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/classic/tests/config-demo.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/classic/tests/test_async.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/classic/tests/test_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import asyncio
 import base64
 import getpass
 import os
 import random
 from time import time
 import yaml
+import sys
 
 import kubernetes_asyncio as kubernetes
 import pytest
 
 import dask
 from dask.distributed import Client, wait
 import dask_kubernetes
@@ -778,14 +779,15 @@
 async def test_start_with_workers(k8s_cluster, pod_spec):
     async with KubeCluster(pod_spec, n_workers=2, **cluster_kwargs) as cluster:
         async with Client(cluster, asynchronous=True) as client:
             await client.wait_for_workers(2)
 
 
 @pytest.mark.asyncio
+@pytest.mark.xfail(reason="Flaky in CI and classic is deprecated anyway")
 async def test_adapt_delete(cluster, ns):
     """
     testing whether KubeCluster.adapt will bring
     back deleted worker pod (issue #244)
     """
     core_api = cluster.core_api
 
@@ -820,14 +822,15 @@
     while len(cluster.scheduler_info["workers"]) != 2:
         await asyncio.sleep(0.1)
         assert time() < start + 60
     assert len(cluster.scheduler_info["workers"]) == 2
 
 
 @pytest.mark.asyncio
+@pytest.mark.xfail(reason="Failing in CI with FileNotFoundError")
 async def test_auto_refresh(cluster):
     config = {
         "apiVersion": "v1",
         "clusters": [
             {
                 "cluster": {"certificate-authority-data": "", "server": ""},
                 "name": "mock_gcp_config",
@@ -849,15 +852,15 @@
             {
                 "name": "mock_gcp_config",
                 "user": {
                     "auth-provider": {
                         "config": {
                             "access-token": "",
                             "cmd-args": "--fake-arg arg",
-                            "cmd-path": f"python {TEST_DIR}/fake_gcp_auth.py",
+                            "cmd-path": f"{sys.executable} {TEST_DIR}/fake_gcp_auth.py",
                             "expiry": "",
                             "expiry-key": "{.credential.token_expiry}",
                             "toekn-key": "{.credential.access_token}",
                         },
                         "name": "gcp",
                     }
                 },
```

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/classic/tests/test_sync.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/classic/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/common/auth.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/common/auth.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/common/networking.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/common/networking.py`

 * *Files 3% similar despite different names*

```diff
@@ -192,16 +192,22 @@
             )
         return address
 
 
 async def wait_for_scheduler(api, cluster_name, namespace, timeout=None):
     pod_start_time = None
     while True:
+        async with kubernetes.client.api_client.ApiClient() as api_client:
+            k8s_api = kubernetes.client.CoreV1Api(api_client)
+            pods = await k8s_api.list_namespaced_pod(
+                namespace=namespace,
+                label_selector=f"dask.org/component=scheduler,dask.org/cluster-name={cluster_name}",
+            )
         pod = await Pod.objects(api, namespace=namespace).get_by_name(
-            cluster_name + "-scheduler"
+            pods.items[0].metadata.name
         )
         phase = pod.obj["status"]["phase"]
         if phase == "Running":
             if not pod_start_time:
                 pod_start_time = time.time()
             conditions = {
                 c["type"]: c["status"] for c in pod.obj["status"]["conditions"]
```

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/common/objects.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/common/objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/common/tests/test_kind.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/common/tests/test_kind.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/common/tests/test_objects.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/common/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/common/utils.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/common/utils.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/conftest.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import pytest
 
 import pathlib
 import os
 import subprocess
 import tempfile
+import uuid
 
 from kopf.testing import KopfRunner
 from pytest_kind.cluster import KindCluster
 
-from dask_kubernetes.common.utils import check_dependency, get_current_namespace
+from dask_kubernetes.common.utils import check_dependency
 
 DIR = pathlib.Path(__file__).parent.absolute()
 
 check_dependency("helm")
 check_dependency("kubectl")
 check_dependency("docker")
 
@@ -56,66 +57,71 @@
             ["istioctl", "install", "--set", "profile=demo", "-y"], check=True
         )
         k8s_cluster.kubectl(
             "label", "namespace", "default", "istio-injection=enabled", "--overwrite"
         )
 
 
-@pytest.fixture(scope="session")
+@pytest.fixture(autouse=True)
 def ns(k8s_cluster):
-    return get_current_namespace()
-
-
-def run_generate(crd_path, patch_path, temp_path):
-    subprocess.run(
-        ["k8s-crd-resolver", "-r", "-j", patch_path, crd_path, temp_path],
-        check=True,
-        env={**os.environ},
-    )
+    ns = "dask-k8s-pytest-" + uuid.uuid4().hex[:10]
+    k8s_cluster.kubectl("create", "ns", ns)
+    yield ns
+    k8s_cluster.kubectl("delete", "ns", ns, "--wait=false", "--ignore-not-found=true")
 
 
 @pytest.fixture(scope="session", autouse=True)
 def install_gateway(k8s_cluster):
-    check_dependency("helm")
-    # To ensure the operator can coexist with Gateway
-    subprocess.run(
-        [
-            "helm",
-            "upgrade",
-            "dask-gateway",
-            "dask-gateway",
-            "--install",
-            "--repo=https://helm.dask.org",
-            "--create-namespace",
-            "--namespace",
-            "dask-gateway",
-        ],
-        check=True,
-        env={**os.environ},
-    )
-    yield
-    subprocess.run(
-        [
-            "helm",
-            "delete",
-            "--namespace",
-            "dask-gateway",
-            "dask-gateway",
-        ],
-        check=True,
-        env={**os.environ},
-    )
+    if bool(os.environ.get("TEST_DASK_GATEWAY", False)):
+        check_dependency("helm")
+        # To ensure the operator can coexist with Gateway
+        subprocess.run(
+            [
+                "helm",
+                "upgrade",
+                "dask-gateway",
+                "dask-gateway",
+                "--install",
+                "--repo=https://helm.dask.org",
+                "--create-namespace",
+                "--namespace",
+                "dask-gateway",
+            ],
+            check=True,
+            env={**os.environ},
+        )
+        yield
+        subprocess.run(
+            [
+                "helm",
+                "delete",
+                "--namespace",
+                "dask-gateway",
+                "dask-gateway",
+            ],
+            check=True,
+            env={**os.environ},
+        )
+    else:
+        yield
 
 
 @pytest.fixture(scope="session", autouse=True)
 def customresources(k8s_cluster):
 
     temp_dir = tempfile.TemporaryDirectory()
     crd_path = os.path.join(DIR, "operator", "customresources")
 
+    def run_generate(crd_path, patch_path, temp_path):
+        subprocess.run(
+            ["k8s-crd-resolver", "-r", "-j", patch_path, crd_path, temp_path],
+            check=True,
+            env={**os.environ},
+        )
+
     for crd in ["daskcluster", "daskworkergroup", "daskjob", "daskautoscaler"]:
         run_generate(
             os.path.join(crd_path, f"{crd}.yaml"),
             os.path.join(crd_path, f"{crd}.patch.yaml"),
             os.path.join(temp_dir.name, f"{crd}.yaml"),
         )
```

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/experimental/__init__.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/helm/helmcluster.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/helm/helmcluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/helm/tests/test_helm.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/helm/tests/test_helm.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/kubernetes.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/kubernetes.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/controller/controller.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/controller/controller.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import asyncio
-import copy
 from collections import defaultdict
 import time
 from contextlib import suppress
 from datetime import datetime
 from uuid import uuid4
 
 import aiohttp
 import kopf
 import kubernetes_asyncio as kubernetes
 from importlib_metadata import entry_points
 from kubernetes_asyncio.client import ApiException
 
+from dask_kubernetes.operator._objects import DaskCluster
 from dask_kubernetes.common.auth import ClusterAuth
 from dask_kubernetes.common.networking import get_scheduler_address
-from dask_kubernetes.aiopykube import HTTPClient, KubeConfig
-from dask_kubernetes.aiopykube.dask import DaskCluster
-from distributed.core import rpc
+from distributed.core import rpc, clean_exception
+from distributed.protocol.pickle import dumps
 
 _ANNOTATION_NAMESPACES_TO_IGNORE = (
     "kopf.zalando.org",
     "kubectl.kubernetes.io",
 )
 _LABEL_NAMESPACES_TO_IGNORE = ()
 
@@ -56,30 +55,42 @@
         for label_key, label_value in meta.labels.items()
         if not any(
             label_key.startswith(namespace) for namespace in _LABEL_NAMESPACES_TO_IGNORE
         )
     }
 
 
-def build_scheduler_pod_spec(cluster_name, spec, annotations, labels):
+def build_scheduler_deployment_spec(
+    cluster_name, namespace, pod_spec, annotations, labels
+):
     labels.update(
         **{
             "dask.org/cluster-name": cluster_name,
             "dask.org/component": "scheduler",
             "sidecar.istio.io/inject": "false",
         }
     )
+    metadata = {
+        "name": f"{cluster_name}-scheduler",
+        "labels": labels,
+        "annotations": annotations,
+    }
+    spec = {}
+    spec["replicas"] = 1
+    spec["selector"] = {
+        "matchLabels": labels,
+    }
+    spec["template"] = {
+        "metadata": metadata,
+        "spec": pod_spec,
+    }
     return {
-        "apiVersion": "v1",
-        "kind": "Pod",
-        "metadata": {
-            "name": f"{cluster_name}-scheduler",
-            "labels": labels,
-            "annotations": annotations,
-        },
+        "apiVersion": "apps/v1",
+        "kind": "Deployment",
+        "metadata": metadata,
         "spec": spec,
     }
 
 
 def build_scheduler_service_spec(cluster_name, spec, annotations, labels):
     labels.update(
         **{
@@ -95,53 +106,64 @@
             "labels": labels,
             "annotations": annotations,
         },
         "spec": spec,
     }
 
 
-def build_worker_pod_spec(
-    worker_group_name, namespace, cluster_name, uuid, spec, annotations, labels
+def build_worker_deployment_spec(
+    worker_group_name, namespace, cluster_name, uuid, pod_spec, annotations, labels
 ):
-    spec = copy.deepcopy(spec)
     labels.update(
         **{
             "dask.org/cluster-name": cluster_name,
             "dask.org/workergroup-name": worker_group_name,
             "dask.org/component": "worker",
             "sidecar.istio.io/inject": "false",
         }
     )
     worker_name = f"{worker_group_name}-worker-{uuid}"
-    pod_spec = {
-        "apiVersion": "v1",
-        "kind": "Pod",
-        "metadata": {
-            "name": worker_name,
-            "labels": labels,
-            "annotations": annotations,
-        },
+    metadata = {
+        "name": worker_name,
+        "labels": labels,
+        "annotations": annotations,
+    }
+    spec = {}
+    spec["replicas"] = 1  # make_worker_spec returns dict with a replicas key?
+    spec["selector"] = {
+        "matchLabels": labels,
+    }
+    spec["template"] = {
+        "metadata": metadata,
+        "spec": pod_spec,
+    }
+    deployment_spec = {
+        "apiVersion": "apps/v1",
+        "kind": "Deployment",
+        "metadata": metadata,
         "spec": spec,
     }
     env = [
         {
             "name": "DASK_WORKER_NAME",
             "value": worker_name,
         },
         {
             "name": "DASK_SCHEDULER_ADDRESS",
             "value": f"tcp://{cluster_name}-scheduler.{namespace}.svc.cluster.local:8786",
         },
     ]
-    for i in range(len(pod_spec["spec"]["containers"])):
-        if "env" in pod_spec["spec"]["containers"][i]:
-            pod_spec["spec"]["containers"][i]["env"].extend(env)
+    for i in range(len(deployment_spec["spec"]["template"]["spec"]["containers"])):
+        if "env" in deployment_spec["spec"]["template"]["spec"]["containers"][i]:
+            deployment_spec["spec"]["template"]["spec"]["containers"][i]["env"].extend(
+                env
+            )
         else:
-            pod_spec["spec"]["containers"][i]["env"] = env
-    return pod_spec
+            deployment_spec["spec"]["template"]["spec"]["containers"][i]["env"] = env
+    return deployment_spec
 
 
 def get_job_runner_pod_name(job_name):
     return f"{job_name}-runner"
 
 
 def build_job_pod_spec(job_name, cluster_name, namespace, spec, annotations, labels):
@@ -260,61 +282,81 @@
     logger.info("Creating Dask cluster components.")
     async with kubernetes.client.api_client.ApiClient() as api_client:
         api = kubernetes.client.CoreV1Api(api_client)
         custom_api = kubernetes.client.CustomObjectsApi(api_client)
 
         annotations = _get_annotations(meta)
         labels = _get_labels(meta)
-        # TODO Check for existing scheduler pod
         scheduler_spec = spec.get("scheduler", {})
         if "metadata" in scheduler_spec:
             if "annotations" in scheduler_spec["metadata"]:
                 annotations.update(**scheduler_spec["metadata"]["annotations"])
             if "labels" in scheduler_spec["metadata"]:
                 labels.update(**scheduler_spec["metadata"]["labels"])
-        data = build_scheduler_pod_spec(
-            name, scheduler_spec.get("spec"), annotations, labels
+        data = build_scheduler_deployment_spec(
+            name, namespace, scheduler_spec.get("spec"), annotations, labels
         )
         kopf.adopt(data)
-        await api.create_namespaced_pod(
+        pod = await api.list_namespaced_pod(
             namespace=namespace,
-            body=data,
+            label_selector=f"dask.org/component=scheduler,dask.org/cluster-name={name}",
         )
-        logger.info(f"Scheduler pod {data['metadata']['name']} created in {namespace}.")
+        if not pod.items:
+            await kubernetes.client.AppsV1Api(api_client).create_namespaced_deployment(
+                namespace=namespace,
+                body=data,
+            )
+            logger.info(
+                f"Scheduler deployment {data['metadata']['name']} created in {namespace}."
+            )
 
-        # TODO Check for existing scheduler service
         data = build_scheduler_service_spec(
             name, scheduler_spec.get("service"), annotations, labels
         )
         kopf.adopt(data)
-        await api.create_namespaced_service(
+        service = await api.list_namespaced_service(
             namespace=namespace,
-            body=data,
+            label_selector=f"dask.org/component=scheduler,dask.org/cluster-name={name}",
         )
+        if not service.items:
+            await api.create_namespaced_service(
+                namespace=namespace,
+                body=data,
+            )
         logger.info(
             f"Scheduler service {data['metadata']['name']} created in {namespace}."
         )
 
         worker_spec = spec.get("worker", {})
         annotations = _get_annotations(meta)
         labels = _get_labels(meta)
         if "metadata" in worker_spec:
             if "annotations" in worker_spec["metadata"]:
                 annotations.update(**worker_spec["metadata"]["annotations"])
             if "labels" in worker_spec["metadata"]:
                 labels.update(**worker_spec["metadata"]["labels"])
         data = build_default_worker_group_spec(name, worker_spec, annotations, labels)
-        await custom_api.create_namespaced_custom_object(
+        worker_group = await custom_api.list_namespaced_custom_object(
             group="kubernetes.dask.org",
             version="v1",
             plural="daskworkergroups",
             namespace=namespace,
-            body=data,
+            label_selector=f"dask.org/component=workergroup,dask.org/cluster-name={name}",
         )
-        logger.info(f"Worker group {data['metadata']['name']} created in {namespace}.")
+        if not worker_group["items"]:
+            await custom_api.create_namespaced_custom_object(
+                group="kubernetes.dask.org",
+                version="v1",
+                plural="daskworkergroups",
+                namespace=namespace,
+                body=data,
+            )
+            logger.info(
+                f"Worker group {data['metadata']['name']} created in {namespace}."
+            )
     patch.status["phase"] = "Pending"
 
 
 @kopf.on.field("service", field="status", labels={"dask.org/component": "scheduler"})
 async def handle_scheduler_service_status(
     spec, labels, status, namespace, logger, **kwargs
 ):
@@ -322,18 +364,16 @@
     if spec["type"] == "LoadBalancer" and not len(
         status.get("load_balancer", {}).get("ingress", [])
     ):
         phase = "Pending"
     # Otherwise mark it as Running
     else:
         phase = "Running"
-
-    api = HTTPClient(KubeConfig.from_env())
-    cluster = await DaskCluster.objects(api, namespace=namespace).get_by_name(
-        labels["dask.org/cluster-name"]
+    cluster = await DaskCluster.get(
+        labels["dask.org/cluster-name"], namespace=namespace
     )
     await cluster.patch({"status": {"phase": phase}})
 
 
 @kopf.on.create("daskworkergroup.kubernetes.dask.org")
 async def daskworkergroup_create(spec, name, namespace, logger, **kwargs):
     async with kubernetes.client.api_client.ApiClient() as api_client:
@@ -392,15 +432,15 @@
             logger.debug(
                 "Received %d response from scheduler API with body %s",
                 resp.status,
                 await resp.text(),
             )
 
     # Otherwise try gracefully retiring via the RPC
-    logger.info(
+    logger.debug(
         f"Scaling {worker_group_name} failed via the HTTP API, falling back to the Dask RPC"
     )
     # Dask version mismatches between the operator and scheduler may cause this to fail in any number of unexpected ways
     with suppress(Exception):
         comm_address = await get_scheduler_address(
             scheduler_service_name,
             namespace,
@@ -411,26 +451,95 @@
                 n=n_workers,
                 attribute="name",
             )
             await scheduler_comm.retire_workers(names=workers_to_close)
             return workers_to_close
 
     # Finally fall back to last-in-first-out scaling
-    logger.info(
+    logger.debug(
         f"Scaling {worker_group_name} failed via the Dask RPC, falling back to LIFO scaling"
     )
     async with kubernetes.client.api_client.ApiClient() as api_client:
         api = kubernetes.client.CoreV1Api(api_client)
         workers = await api.list_namespaced_pod(
             namespace=namespace,
             label_selector=f"dask.org/workergroup-name={worker_group_name}",
         )
         return [w["metadata"]["name"] for w in workers.items[:-n_workers]]
 
 
+async def check_scheduler_idle(scheduler_service_name, namespace, logger):
+    # Try getting idle time via HTTP API
+    dashboard_address = await get_scheduler_address(
+        scheduler_service_name,
+        namespace,
+        port_name="http-dashboard",
+        allow_external=False,
+    )
+    async with aiohttp.ClientSession() as session:
+        url = f"{dashboard_address}/api/v1/check_idle"
+        async with session.get(url) as resp:
+            if resp.status <= 300:
+                idle_since = (await resp.json())["idle_since"]
+                if idle_since:
+                    logger.debug("Scheduler idle since: %s", idle_since)
+                return idle_since
+            logger.debug(
+                "Received %d response from scheduler API with body %s",
+                resp.status,
+                await resp.text(),
+            )
+
+    # Otherwise try gracefully checking via the RPC
+    logger.debug(
+        f"Checking {scheduler_service_name} idleness failed via the HTTP API, falling back to the Dask RPC"
+    )
+    # Dask version mismatches between the operator and scheduler may cause this to fail in any number of unexpected ways
+    with suppress(Exception):
+        comm_address = await get_scheduler_address(
+            scheduler_service_name,
+            namespace,
+            allow_external=False,
+        )
+        async with rpc(comm_address) as scheduler_comm:
+            idle_since = await scheduler_comm.check_idle()
+            if idle_since:
+                logger.debug("Scheduler idle since: %s", idle_since)
+            return idle_since
+
+    # Finally fall back to code injection via the Dask RPC for distributed<=2023.3.1
+    logger.debug(
+        f"Checking {scheduler_service_name} idleness failed via the Dask RPC, falling back to run_on_scheduler"
+    )
+
+    def idle_since(dask_scheduler=None):
+        if not dask_scheduler.idle_timeout:
+            dask_scheduler.idle_timeout = 300
+        dask_scheduler.check_idle()
+        return dask_scheduler.idle_since
+
+    comm_address = await get_scheduler_address(
+        scheduler_service_name,
+        namespace,
+        allow_external=False,
+    )
+    async with rpc(comm_address) as scheduler_comm:
+        response = await scheduler_comm.run_function(
+            function=dumps(idle_since),
+        )
+        if response["status"] == "error":
+            typ, exc, tb = clean_exception(**response)
+            raise exc.with_traceback(tb)
+        else:
+            idle_since = response["result"]
+            if idle_since:
+                logger.debug("Scheduler idle since: %s", idle_since)
+            return idle_since
+
+
 async def get_desired_workers(scheduler_service_name, namespace, logger):
     # Try gracefully retiring via the HTTP API
     dashboard_address = await get_scheduler_address(
         scheduler_service_name,
         namespace,
         port_name="http-dashboard",
         allow_external=False,
@@ -457,14 +566,37 @@
             "Unable to get number of desired workers from scheduler"
         ) from e
 
 
 worker_group_scale_locks = defaultdict(lambda: asyncio.Lock())
 
 
+@kopf.on.field("daskcluster.kubernetes.dask.org", field="spec.worker.replicas")
+async def daskcluster_default_worker_group_replica_update(
+    name, namespace, meta, spec, old, new, body, logger, **kwargs
+):
+    if old is None:
+        return
+    worker_group_name = f"{name}-default"
+
+    async with kubernetes.client.api_client.ApiClient() as api_client:
+        custom_objects_api = kubernetes.client.CustomObjectsApi(api_client)
+        custom_objects_api.api_client.set_default_header(
+            "content-type", "application/merge-patch+json"
+        )
+        await custom_objects_api.patch_namespaced_custom_object_scale(
+            group="kubernetes.dask.org",
+            version="v1",
+            plural="daskworkergroups",
+            namespace=namespace,
+            name=worker_group_name,
+            body={"spec": {"replicas": new}},
+        )
+
+
 @kopf.on.field("daskworkergroup.kubernetes.dask.org", field="spec.worker.replicas")
 async def daskworkergroup_replica_update(
     name, namespace, meta, spec, new, body, logger, **kwargs
 ):
     cluster_name = spec["cluster"]
 
     # Replica updates can come in quick succession and the changes must be applied atomically to ensure
@@ -506,26 +638,28 @@
             if "metadata" in worker_spec:
                 if "annotations" in worker_spec["metadata"]:
                     annotations.update(**worker_spec["metadata"]["annotations"])
                 if "labels" in worker_spec["metadata"]:
                     labels.update(**worker_spec["metadata"]["labels"])
             if workers_needed > 0:
                 for _ in range(workers_needed):
-                    data = build_worker_pod_spec(
+                    data = build_worker_deployment_spec(
                         worker_group_name=name,
                         namespace=namespace,
                         cluster_name=cluster_name,
                         uuid=uuid4().hex[:10],
-                        spec=worker_spec["spec"],
+                        pod_spec=worker_spec["spec"],
                         annotations=annotations,
                         labels=labels,
                     )
                     kopf.adopt(data, owner=body)
                     kopf.label(data, labels=cluster_labels)
-                    await corev1api.create_namespaced_pod(
+                    await kubernetes.client.AppsV1Api(
+                        api_client
+                    ).create_namespaced_deployment(
                         namespace=namespace,
                         body=data,
                     )
                 logger.info(
                     f"Scaled worker group {name} up to {desired_workers} workers."
                 )
             if workers_needed < 0:
@@ -534,15 +668,17 @@
                     scheduler_service_name=f"{cluster_name}-scheduler",
                     worker_group_name=name,
                     namespace=namespace,
                     logger=logger,
                 )
                 logger.info(f"Workers to close: {worker_ids}")
                 for wid in worker_ids:
-                    await corev1api.delete_namespaced_pod(
+                    await kubernetes.client.AppsV1Api(
+                        api_client
+                    ).delete_namespaced_deployment(
                         name=wid,
                         namespace=namespace,
                     )
                 logger.info(
                     f"Scaled worker group {name} down to {desired_workers} workers."
                 )
 
@@ -748,16 +884,20 @@
 @kopf.timer("daskautoscaler.kubernetes.dask.org", interval=5.0)
 async def daskautoscaler_adapt(spec, name, namespace, logger, **kwargs):
     async with kubernetes.client.api_client.ApiClient() as api_client:
         coreapi = kubernetes.client.CoreV1Api(api_client)
 
         pod_ready = False
         try:
+            pods = await coreapi.list_namespaced_pod(
+                namespace=namespace,
+                label_selector=f"dask.org/component=scheduler,dask.org/cluster-name={spec['cluster']}",
+            )
             scheduler_pod = await coreapi.read_namespaced_pod(
-                f"{spec['cluster']}-scheduler", namespace
+                pods.items[0].metadata.name, namespace
             )
             if scheduler_pod.status.phase == "Running":
                 pod_ready = True
         except ApiException as e:
             if e.status != 404:
                 raise e
 
@@ -854,7 +994,24 @@
                 current_replicas,
                 desired_workers,
             )
         else:
             logger.debug(
                 "Not autoscaling %s with %d workers", spec["cluster"], current_replicas
             )
+
+
+@kopf.timer("daskcluster.kubernetes.dask.org", interval=5.0)
+async def daskcluster_autoshutdown(spec, name, namespace, logger, **kwargs):
+    if spec["idleTimeout"]:
+        try:
+            idle_since = await check_scheduler_idle(
+                scheduler_service_name=f"{name}-scheduler",
+                namespace=namespace,
+                logger=logger,
+            )
+        except Exception as e:
+            logger.warn("Unable to connect to scheduler, skipping autoshutdown check.")
+            return
+        if idle_since and time.time() > idle_since + spec["idleTimeout"]:
+            cluster = await DaskCluster.get(name, namespace=namespace)
+            await cluster.delete()
```

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 apiVersion: kubernetes.dask.org/v1
 kind: DaskJob
 metadata:
   name: failed-job
-  namespace: default
 spec:
   job:
     spec:
       restartPolicy: Never
       containers:
         - name: job
           image: "dask-kubernetes:dev"
```

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 apiVersion: kubernetes.dask.org/v1
 kind: DaskCluster
 metadata:
   name: simple
-  namespace: default
   labels:
     test-label: "label-value"
   annotations:
     test-annotation: "annotation-value"
     "kopf.zalando.org/foobar": "should-not-be-propagated"
     "kubectl.kubernetes.io": "should-not-be-propagated"
 spec:
```

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 apiVersion: kubernetes.dask.org/v1
 kind: DaskJob
 metadata:
   name: simple-job
-  namespace: default
   annotations:
     test-annotation: "annotation-value"
     "kopf.zalando.org/foobar": "should-not-be-propagated"
     "kubectl.kubernetes.io": "should-not-be-propagated"
 spec:
   job:
     spec:
```

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 apiVersion: kubernetes.dask.org/v1
 kind: DaskWorkerGroup
 metadata:
   name: simple-additional
-  namespace: default
 spec:
   cluster: simple
   worker:
     replicas: 2
     spec:
       containers:
         - name: worker
```

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/customresources/daskautoscaler.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/customresources/daskautoscaler.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -9,14 +9,28 @@
     kind: DaskAutoscaler
     plural: daskautoscalers
     singular: daskautoscaler
   versions:
     - name: v1
       served: true
       storage: true
+      additionalPrinterColumns:
+        - name: Cluster
+          type: string
+          description: Cluster to autoscale
+          jsonPath: .spec.cluster
+        - name: Minimum
+          type: integer
+          jsonPath: .spec.minimum
+        - name: Maximum
+          type: integer
+          jsonPath: .spec.maximum
+        - name: Age
+          type: date
+          jsonPath: .metadata.creationTimestamp
       schema:
         openAPIV3Schema:
           type: object
           properties:
             spec:
               type: object
               required:
```

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/customresources/daskcluster.patch.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/customresources/daskcluster.patch.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/customresources/daskjob.patch.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/customresources/daskjob.patch.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/customresources/daskjob.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/customresources/daskjob.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,24 @@
     singular: daskjob
     shortNames:
       - djb
   versions:
     - name: v1
       served: true
       storage: true
+      additionalPrinterColumns:
+        - name: Status
+          type: string
+          jsonPath: .status.jobStatus
+        - name: Number Of Workers
+          type: integer
+          jsonPath: .spec.cluster.spec.worker.replicas
+        - name: Age
+          type: date
+          jsonPath: .metadata.creationTimestamp
       schema:
         openAPIV3Schema:
           type: object
           properties:
             status:
               properties:
                 clusterName:
@@ -53,14 +63,7 @@
                       $ref: 'python://dask_kubernetes/operator/customresources/templates.yaml#/definitions/dask.k8s.api.v1.SimpleObjectMeta'
                     spec:
                       $ref: 'python://k8s_crd_resolver/schemata/k8s-1.21.1.json#/definitions/io.k8s.api.core.v1.PodSpec'
                 cluster:
                   $ref: 'python://dask_kubernetes/operator/customresources/templates.yaml#/definitions/dask.k8s.api.v1.DaskCluster'
       subresources:
         status: {}
-      additionalPrinterColumns:
-        - jsonPath: .status.jobStatus
-          name: Status
-          type: string
-        - jsonPath: .spec.cluster.spec.worker.replicas
-          name: Number Of Workers
-          type: integer
```

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/customresources/templates.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/customresources/templates.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -63,11 +63,15 @@
             description: Status of the Dask cluster
       spec:
         type: object
         required:
         - scheduler
         - worker
         properties:
+          idleTimeout:
+            type: integer
+            description: Delete cluster if scheduler is idle for longer than this timeout. Set to 0 to never auto cleanup.
+            default: 0
           scheduler:
             $ref: 'python://dask_kubernetes/operator/customresources/templates.yaml#/definitions/dask.k8s.api.v1.DaskScheduler'
           worker:
             $ref: 'python://dask_kubernetes/operator/customresources/templates.yaml#/definitions/dask.k8s.api.v1.DaskWorker'
```

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/chartpress.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/chartpress.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,29 @@
   group: kubernetes.dask.org
   names:
     kind: DaskAutoscaler
     plural: daskautoscalers
     singular: daskautoscaler
   scope: Namespaced
   versions:
-  - name: v1
+  - additionalPrinterColumns:
+    - description: Cluster to autoscale
+      jsonPath: .spec.cluster
+      name: Cluster
+      type: string
+    - jsonPath: .spec.minimum
+      name: Minimum
+      type: integer
+    - jsonPath: .spec.maximum
+      name: Maximum
+      type: integer
+    - jsonPath: .metadata.creationTimestamp
+      name: Age
+      type: date
+    name: v1
     schema:
       openAPIV3Schema:
         properties:
           spec:
             properties:
               cluster:
                 description: Name of the cluster to associate this worker group with
```

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,34 @@
     plural: daskclusters
     shortNames:
     - daskcluster
     - dsk
     singular: daskcluster
   scope: Namespaced
   versions:
-  - name: v1
+  - additionalPrinterColumns:
+    - description: The number of desired worker Pods
+      jsonPath: .spec.worker.replicas
+      name: Workers
+      type: integer
+    - jsonPath: .status.phase
+      name: Status
+      type: string
+    - jsonPath: .metadata.creationTimestamp
+      name: Age
+      type: date
+    name: v1
     schema:
       openAPIV3Schema:
         properties:
           spec:
             properties:
+              idleTimeout:
+                default: 0
+                type: integer
               scheduler:
                 properties:
                   metadata:
                     properties:
                       annotations:
                         additionalProperties:
                           type: string
```

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -15,24 +15,30 @@
   - additionalPrinterColumns:
     - jsonPath: .status.jobStatus
       name: Status
       type: string
     - jsonPath: .spec.cluster.spec.worker.replicas
       name: Number Of Workers
       type: integer
+    - jsonPath: .metadata.creationTimestamp
+      name: Age
+      type: date
     name: v1
     schema:
       openAPIV3Schema:
         properties:
           spec:
             properties:
               cluster:
                 properties:
                   spec:
                     properties:
+                      idleTimeout:
+                        default: 0
+                        type: integer
                       scheduler:
                         properties:
                           metadata:
                             properties:
                               annotations:
                                 additionalProperties:
                                   type: string
```

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,23 @@
     kind: DaskWorkerGroup
     plural: daskworkergroups
     shortNames:
     - daskworkers
     singular: daskworkergroup
   scope: Namespaced
   versions:
-  - name: v1
+  - additionalPrinterColumns:
+    - description: The number of desired worker Pods
+      jsonPath: .spec.worker.replicas
+      name: Workers
+      type: integer
+    - jsonPath: .metadata.creationTimestamp
+      name: Age
+      type: date
+    name: v1
     schema:
       openAPIV3Schema:
         properties:
           spec:
             properties:
               cluster:
                 description: Name of the cluster to associate this worker group with
```

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/kubecluster/discovery.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/kubecluster/discovery.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/kubecluster/kubecluster.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/kubecluster/kubecluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,17 @@
         doesn't exist, or connect to an existing one if it does.
         You can also set ``CreateMode.CREATE_ONLY`` to raise an exception if a cluster
         with that name already exists. Or ``CreateMode.CONNECT_ONLY`` to raise an exception
         if a cluster with that name doesn't exist.
     shutdown_on_close: bool (optional)
         Whether or not to delete the cluster resource when this object is closed.
         Defaults to ``True`` when creating a cluster and ``False`` when connecting to an existing one.
+    idle_timeout: int (optional)
+        If set Kubernetes will delete the cluster automatically if the scheduler is idle for longer than
+        this timeout in seconds.
     resource_timeout: int (optional)
         Time in seconds to wait for Kubernetes resources to enter their expected state.
         Example: If the ``DaskCluster`` resource that gets created isn't moved into a known ``status.phase``
         by the controller then it is likely the controller isn't running or is malfunctioning and we time
         out and clean up with a useful error.
         Example 2: If the scheduler Pod enters a ``CrashBackoffLoop`` state for longer than this timeout we
         give up with a useful error.
@@ -166,21 +169,23 @@
         resources=None,
         env=None,
         worker_command=None,
         auth=ClusterAuth.DEFAULT,
         port_forward_cluster_ip=None,
         create_mode=None,
         shutdown_on_close=None,
+        idle_timeout=None,
         resource_timeout=None,
         scheduler_service_type=None,
         custom_cluster_spec=None,
         scheduler_forward_port=None,
+        loop=None,
+        asynchronous=False,
         **kwargs,
     ):
-
         name = dask.config.get("kubernetes.name", override_with=name)
         self.namespace = (
             dask.config.get("kubernetes.namespace", override_with=namespace)
             or get_current_namespace()
         )
         self.image = dask.config.get("kubernetes.image", override_with=image)
         self.n_workers = dask.config.get(
@@ -216,34 +221,63 @@
         )
         self.scheduler_service_type = dask.config.get(
             "kubernetes.scheduler-service-type", override_with=scheduler_service_type
         )
         self.scheduler_forward_port = dask.config.get(
             "kubernetes.scheduler-forward-port", override_with=scheduler_forward_port
         )
+        self.idle_timeout = dask.config.get(
+            "kubernetes.idle-timeout", override_with=idle_timeout
+        )
 
         if self._custom_cluster_spec:
             if isinstance(self._custom_cluster_spec, str):
                 with open(self._custom_cluster_spec) as f:
                     self._custom_cluster_spec = yaml.safe_load(f.read())
             name = self._custom_cluster_spec["metadata"]["name"]
 
         if isinstance(self.worker_command, str):
             self.worker_command = self.worker_command.split(" ")
 
+        try:
+            # Validate `resources` param is a dictionary whose
+            # keys must either be 'limits' or 'requests'
+            assert isinstance(
+                self.resources, dict
+            ), f"resources must be dict type, found {type(resources)}"
+            for field in self.resources:
+                if field in ("limits", "requests"):
+                    assert isinstance(
+                        self.resources[field], dict
+                    ), f"key of '{field}' must be dict type"
+                else:
+                    raise ValueError(f"resources has unknown field '{field}'")
+        except AssertionError as e:
+            raise TypeError from e
+
         name = name.format(
             user=getpass.getuser(), uuid=str(uuid.uuid4())[:10], **os.environ
         )
         self.k8s_api = HTTPClient(KubeConfig.from_env())
         self._instances.add(self)
         self._rich_spinner = Spinner("dots", speed=0.5)
         self._startup_component_status = {}
 
-        super().__init__(name=name, **kwargs)
-        if not self.asynchronous:
+        super().__init__(name=name, loop=loop, asynchronous=asynchronous, **kwargs)
+
+        # If https://github.com/dask/distributed/pull/7941 is merged we can
+        # simplify the next 8 lines to ``if not self.called_from_running_loop:``
+        try:
+            called_from_running_loop = (
+                getattr(loop, "asyncio_loop", None) is asyncio.get_running_loop()
+            )
+        except RuntimeError:
+            called_from_running_loop = asynchronous
+
+        if not called_from_running_loop:
             self._loop_runner.start()
             self.sync(self._start)
 
     def _log(self, log):
         temp = self.quiet
         self.quiet = True
         super()._log(log)
@@ -255,15 +289,16 @@
         return format_dashboard_link(host, self.forwarded_dashboard_port)
 
     async def _start(self):
         try:
             watch_component_status_task = asyncio.create_task(
                 self._watch_component_status()
             )
-            show_rich_output_task = asyncio.create_task(self._show_rich_output())
+            if not self.quiet:
+                show_rich_output_task = asyncio.create_task(self._show_rich_output())
             await ClusterAuth.load_first(self.auth)
             cluster_exists = (await self._get_cluster()) is not None
 
             if cluster_exists and self.create_mode == CreateMode.CREATE_ONLY:
                 raise ValueError(
                     f"Cluster {self.name} already exists and create mode is '{CreateMode.CREATE_ONLY}'"
                 )
@@ -279,15 +314,16 @@
                 self._log("Creating cluster")
                 await self._create_cluster()
 
             await super()._start()
             self._log(f"Ready, dashboard available at {self.dashboard_link}")
         finally:
             watch_component_status_task.cancel()
-            show_rich_output_task.cancel()
+            if not self.quiet:
+                show_rich_output_task.cancel()
 
     def __await__(self):
         async def _():
             if self.status == Status.created:
                 await self._start()
             return self
 
@@ -306,32 +342,36 @@
                     name=self.name,
                     env=self.env,
                     resources=self.resources,
                     worker_command=self.worker_command,
                     n_workers=self.n_workers,
                     image=self.image,
                     scheduler_service_type=self.scheduler_service_type,
+                    idle_timeout=self.idle_timeout,
                 )
             else:
                 data = self._custom_cluster_spec
             try:
                 self._log("Creating DaskCluster object")
                 await custom_objects_api.create_namespaced_custom_object(
                     group="kubernetes.dask.org",
                     version="v1",
                     plural="daskclusters",
                     namespace=self.namespace,
                     body=data,
                 )
             except kubernetes.client.ApiException as e:
-                raise RuntimeError(
-                    "Failed to create DaskCluster resource. "
-                    "Are the Dask Custom Resource Definitions installed? "
-                    "https://kubernetes.dask.org/en/latest/operator.html#installing-the-operator"
-                ) from e
+                if e.status == 404:
+                    raise RuntimeError(
+                        "Failed to create DaskCluster resource."
+                        "Are the Dask Custom Resource Definitions installed? "
+                        "https://kubernetes.dask.org/en/latest/operator.html#installing-the-operator"
+                    ) from e
+                else:
+                    raise e
 
             try:
                 self._log("Waiting for controller to action cluster")
                 await self._wait_for_controller()
             except TimeoutError as e:
                 await self._close()
                 raise e
@@ -341,19 +381,23 @@
                     self.k8s_api,
                     self.name,
                     self.namespace,
                     timeout=self._resource_timeout,
                 )
             except CrashLoopBackOffError as e:
                 logs = await self._get_logs()
+                pods = await core_api.list_namespaced_pod(
+                    namespace=self.namespace,
+                    label_selector=f"dask.org/component=scheduler,dask.org/cluster-name={self.name}",
+                )
                 await self._close()
                 raise SchedulerStartupError(
                     "Scheduler failed to start.",
                     "Scheduler Pod logs:",
-                    logs[self.name + "-scheduler"],
+                    logs[pods.items[0].metadata.name],
                 ) from e
             self._log("Waiting for scheduler service")
             await wait_for_service(core_api, f"{self.name}-scheduler", self.namespace)
             scheduler_address = await self._get_scheduler_address()
             self._log("Connecting to scheduler")
             await wait_for_scheduler_comm(scheduler_address)
             self.scheduler_comm = rpc(scheduler_address)
@@ -460,30 +504,38 @@
                 ).get_by_name(self.name)
                 self._startup_component_status["cluster"] = cluster.obj["status"][
                     "phase"
                 ]
 
             # Get Scheduler Pod status
             with suppress(pykube.exceptions.ObjectDoesNotExist):
-                pod = await Pod.objects(
-                    self.k8s_api, namespace=self.namespace
-                ).get_by_name(self.name + "-scheduler")
-                phase = pod.obj["status"]["phase"]
-                if phase == "Running":
-                    conditions = {
-                        c["type"]: c["status"] for c in pod.obj["status"]["conditions"]
-                    }
-                    if "Ready" not in conditions or conditions["Ready"] != "True":
-                        phase = "Health Checking"
-                    if "containerStatuses" in pod.obj["status"]:
-                        for container in pod.obj["status"]["containerStatuses"]:
-                            if "waiting" in container["state"]:
-                                phase = container["state"]["waiting"]["reason"]
+                async with kubernetes.client.api_client.ApiClient() as api_client:
+                    core_api = kubernetes.client.CoreV1Api(api_client)
+                    pods = await core_api.list_namespaced_pod(
+                        namespace=self.namespace,
+                        label_selector=f"dask.org/component=scheduler,dask.org/cluster-name={self.name}",
+                    )
+                if pods.items:
+                    pod = await Pod.objects(
+                        self.k8s_api, namespace=self.namespace
+                    ).get_by_name(pods.items[0].metadata.name)
+                    phase = pod.obj["status"]["phase"]
+                    if phase == "Running":
+                        conditions = {
+                            c["type"]: c["status"]
+                            for c in pod.obj["status"]["conditions"]
+                        }
+                        if "Ready" not in conditions or conditions["Ready"] != "True":
+                            phase = "Health Checking"
+                        if "containerStatuses" in pod.obj["status"]:
+                            for container in pod.obj["status"]["containerStatuses"]:
+                                if "waiting" in container["state"]:
+                                    phase = container["state"]["waiting"]["reason"]
 
-                self._startup_component_status["schedulerpod"] = phase
+                    self._startup_component_status["schedulerpod"] = phase
 
             # Get Scheduler Service status
             with suppress(pykube.exceptions.ObjectDoesNotExist):
                 await Service.objects(self.k8s_api).get_by_name(
                     self.name + "-scheduler"
                 )
                 self._startup_component_status["schedulerservice"] = "Created"
@@ -498,15 +550,15 @@
             await asyncio.sleep(1)
 
     async def generate_rich_output(self):
         table = Table(show_header=False, box=box.SIMPLE, expand=True)
         table.add_column("Component")
         table.add_column("Status", justify="right")
 
-        for (label, component) in [
+        for label, component in [
             ("DaskCluster", "cluster"),
             ("Scheduler Pod", "schedulerpod"),
             ("Scheduler Service", "schedulerservice"),
             ("Default Worker Group", "workergroup"),
         ]:
             try:
                 status = self._startup_component_status[component]
@@ -697,15 +749,15 @@
                 name=f"{self.name}-{name}",
             )
 
     def close(self, timeout=3600):
         """Delete the dask cluster"""
         return self.sync(self._close, timeout=timeout)
 
-    async def _close(self, timeout=None):
+    async def _close(self, timeout=3600):
         await super()._close()
         if self.shutdown_on_close:
             async with kubernetes.client.api_client.ApiClient() as api_client:
                 custom_objects_api = kubernetes.client.CustomObjectsApi(api_client)
                 try:
                     await custom_objects_api.delete_namespaced_custom_object(
                         group="kubernetes.dask.org",
@@ -766,14 +818,17 @@
                 group="kubernetes.dask.org",
                 version="v1",
                 plural="daskworkergroups",
                 namespace=self.namespace,
                 name=f"{self.name}-{worker_group}",
                 body={"spec": {"replicas": n}},
             )
+            for instance in self._instances:
+                if instance.name == self.name:
+                    instance.scheduler_info = self.scheduler_info
 
     def adapt(self, minimum=None, maximum=None):
         """Turn on adaptivity
 
         Parameters
         ----------
         minimum : int
@@ -842,25 +897,31 @@
         name: str
             Name of the cluster to connect to
 
         Examples
         --------
         >>> cluster = KubeCluster.from_name(name="simple-cluster")
         """
-        return cls(name=name, create_mode=CreateMode.CONNECT_ONLY, **kwargs)
+        defaults = {"create_mode": CreateMode.CONNECT_ONLY, "shutdown_on_close": False}
+        kwargs = defaults | kwargs
+        return cls(
+            name=name,
+            **kwargs,
+        )
 
 
 def make_cluster_spec(
     name,
     image="ghcr.io/dask/dask:latest",
     n_workers=None,
     resources=None,
     env=None,
     worker_command="dask-worker",
     scheduler_service_type="ClusterIP",
+    idle_timeout=0,
 ):
     """Generate a ``DaskCluster`` kubernetes resource.
 
     Populate a template with some common options to generate a ``DaskCluster`` kubernetes resource.
 
     Parameters
     ----------
@@ -872,20 +933,23 @@
         Number of workers in the default worker group
     resources: dict (optional)
         Resource limits to set on scheduler and workers
     env: dict (optional)
         Environment variables to set on scheduler and workers
     worker_command: str (optional)
         Worker command to use when starting the workers
+    idle_timeout: int (optional)
+        Timeout to cleanup idle cluster
     """
     return {
         "apiVersion": "kubernetes.dask.org/v1",
         "kind": "DaskCluster",
         "metadata": {"name": name},
         "spec": {
+            "idleTimeout": idle_timeout,
             "worker": make_worker_spec(
                 env=env,
                 resources=resources,
                 worker_command=worker_command,
                 n_workers=n_workers,
                 image=image,
             ),
```

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/kubecluster/tests/conftest.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/kubecluster/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/kubecluster/tests/test_discovery.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/kubecluster/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py` & `dask-kubernetes-2023.6.0/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import pytest
+import kubernetes_asyncio as kubernetes
 
 from dask.distributed import Client
 from distributed.utils import TimeoutError
 
+from dask_kubernetes.operator._objects import DaskCluster
 from dask_kubernetes.operator import KubeCluster, make_cluster_spec
 from dask_kubernetes.exceptions import SchedulerStartupError
 
 
 def test_experimental_shim():
     with pytest.deprecated_call():
         from dask_kubernetes.experimental import KubeCluster as ExperimentalKubeCluster
@@ -90,21 +92,38 @@
         ) as cluster2:
             with Client(cluster1) as client1, Client(cluster2) as client2:
                 assert cluster1.loop is cluster2.loop is client1.loop is client2.loop
                 assert client1.submit(lambda x: x + 1, 10).result() == 11
                 assert client2.submit(lambda x: x + 1, 10).result() == 11
 
 
-def test_cluster_from_name(kopf_runner, docker_image, ns):
+@pytest.mark.asyncio
+async def test_cluster_from_name(kopf_runner, docker_image, ns):
     with kopf_runner:
-        with KubeCluster(
-            name="abc", namespace=ns, image=docker_image, n_workers=1
+        async with KubeCluster(
+            name="abc",
+            namespace=ns,
+            image=docker_image,
+            n_workers=1,
+            asynchronous=True,
         ) as firstcluster:
-            with KubeCluster.from_name("abc", namespace=ns) as secondcluster:
+            async with KubeCluster.from_name(
+                "abc", namespace=ns, asynchronous=True
+            ) as secondcluster:
                 assert firstcluster == secondcluster
+            cluster = await DaskCluster.get("abc", namespace=ns)
+            assert cluster.status["phase"] == "Running"
+
+
+def test_cluster_scheduler_info_updated(kopf_runner, docker_image, ns):
+    with kopf_runner:
+        with KubeCluster(name="abc", namespace=ns, image=docker_image) as firstcluster:
+            with KubeCluster.from_name("abc", namespace=ns) as secondcluster:
+                firstcluster.scale(1)
+                assert firstcluster.scheduler_info == secondcluster.scheduler_info
 
 
 def test_additional_worker_groups(kopf_runner, docker_image):
     with kopf_runner:
         with KubeCluster(
             name="additionalgroups", n_workers=1, image=docker_image
         ) as cluster:
@@ -119,19 +138,19 @@
     with pytest.raises(TimeoutError, match="is the Dask Operator running"):
         KubeCluster(name="noop", n_workers=1, image=docker_image, resource_timeout=1)
 
 
 def test_cluster_crashloopbackoff(kopf_runner, docker_image):
     with kopf_runner:
         with pytest.raises(SchedulerStartupError, match="Scheduler failed to start"):
-            spec = make_cluster_spec(name="foo", n_workers=1)
+            spec = make_cluster_spec(name="crashloopbackoff", n_workers=1)
             spec["spec"]["scheduler"]["spec"]["containers"][0]["args"][
                 0
             ] = "dask-schmeduler"
-            KubeCluster(custom_cluster_spec=spec, resource_timeout=1)
+            KubeCluster(custom_cluster_spec=spec, resource_timeout=1, idle_timeout=2)
 
 
 def test_adapt(kopf_runner, docker_image):
     with kopf_runner:
         with KubeCluster(
             name="adaptive",
             image=docker_image,
@@ -149,7 +168,27 @@
 
 def test_custom_spec(kopf_runner, docker_image):
     with kopf_runner:
         spec = make_cluster_spec("customspec", image=docker_image)
         with KubeCluster(custom_cluster_spec=spec, n_workers=1) as cluster:
             with Client(cluster) as client:
                 assert client.submit(lambda x: x + 1, 10).result() == 11
+
+
+def test_typo_resource_limits(kopf_runner):
+    with kopf_runner:
+        with pytest.raises(ValueError):
+            KubeCluster(
+                name="foo",
+                resources={
+                    "limit": {  # <-- Typo, should be `limits`
+                        "CPU": "1",
+                    },
+                },
+            )
+
+
+@pytest.mark.xfail(reason="Intermittently fails in CI")
+def test_invalid_kwargs_exception(kopf_runner):
+    with kopf_runner:
+        with pytest.raises(kubernetes.client.ApiException):
+            KubeCluster(name="foo", n_workers="1")
```

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes.egg-info/PKG-INFO` & `dask-kubernetes-2023.6.0/dask_kubernetes.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: dask-kubernetes
-Version: 2023.3.2
+Version: 2023.6.0
 Summary: Native Kubernetes integration for Dask
 Home-page: https://github.com/dask/dask-kubernetes
 Maintainer: Jacob Tomlinson
 License: BSD
-Description: Dask Kubernetes
-        ===============
-        
-        
-        .. image:: https://github.com/dask/dask-kubernetes/workflows/CI/badge.svg
-           :target: https://github.com/dask/dask-kubernetes/actions?query=workflow%3ACI
-        
-        .. image:: https://img.shields.io/readthedocs/dask-kubernetes?color=%232980B9&logo=read-the-docs&logoColor=white
-           :target: https://kubernetes.dask.org/
-           :alt: Read the Docs
-        
-        .. image:: https://img.shields.io/readthedocs/dask-kubernetes?color=%232980B9&label=developer%20docs&logo=read-the-docs&logoColor=white
-           :target: https://kubernetes.dask.org/releasing.html
-           :alt: Read the Docs Developer
-        
-        .. image:: https://img.shields.io/pypi/v/dask-kubernetes
-           :target: https://pypi.org/project/dask-kubernetes/
-           :alt: PyPI
-        
-        .. image:: https://img.shields.io/conda/vn/conda-forge/dask-kubernetes
-           :target: https://anaconda.org/conda-forge/dask-kubernetes
-           :alt: Conda Forge
-        
-        .. image:: https://img.shields.io/badge/python%20support-3.8%7C3.9%7C3.10-blue
-           :target: https://kubernetes.dask.org/en/latest/installing.html#supported-versions
-           :alt: Python Support
-        
-        .. image:: https://img.shields.io/badge/Kubernetes%20support-1.22%7C1.23%7C1.24%7C1.25-blue
-           :target: https://kubernetes.dask.org/en/latest/installing.html#supported-versions
-           :alt: Kubernetes Support
-        
-        
-        Native Kubernetes integration for Dask.
-        
 Keywords: dask,kubernetes,distributed
-Platform: UNKNOWN
-Requires-Python: >=3.8
+Requires-Python: >=3.9
+License-File: LICENSE
+
+Dask Kubernetes
+===============
+
+
+.. image:: https://github.com/dask/dask-kubernetes/workflows/CI/badge.svg
+   :target: https://github.com/dask/dask-kubernetes/actions?query=workflow%3ACI
+
+.. image:: https://img.shields.io/readthedocs/dask-kubernetes?color=%232980B9&logo=read-the-docs&logoColor=white
+   :target: https://kubernetes.dask.org/
+   :alt: Read the Docs
+
+.. image:: https://img.shields.io/readthedocs/dask-kubernetes?color=%232980B9&label=developer%20docs&logo=read-the-docs&logoColor=white
+   :target: https://kubernetes.dask.org/releasing.html
+   :alt: Read the Docs Developer
+
+.. image:: https://img.shields.io/pypi/v/dask-kubernetes
+   :target: https://pypi.org/project/dask-kubernetes/
+   :alt: PyPI
+
+.. image:: https://img.shields.io/conda/vn/conda-forge/dask-kubernetes
+   :target: https://anaconda.org/conda-forge/dask-kubernetes
+   :alt: Conda Forge
+
+.. image:: https://img.shields.io/badge/python%20support-3.9%7C3.10-blue
+   :target: https://kubernetes.dask.org/en/latest/installing.html#supported-versions
+   :alt: Python Support
+
+.. image:: https://img.shields.io/badge/Kubernetes%20support-1.24%7C1.25%7C1.26%7C1.27-blue
+   :target: https://kubernetes.dask.org/en/latest/installing.html#supported-versions
+   :alt: Kubernetes Support
+
+
+Native Kubernetes integration for Dask.
```

### Comparing `dask-kubernetes-2023.3.2/dask_kubernetes.egg-info/SOURCES.txt` & `dask-kubernetes-2023.6.0/dask_kubernetes.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,26 +28,29 @@
 dask_kubernetes/aiopykube/tests/test_query.py
 dask_kubernetes/classic/__init__.py
 dask_kubernetes/classic/kubecluster.py
 dask_kubernetes/classic/tests/config-demo.yaml
 dask_kubernetes/classic/tests/fake_gcp_auth.py
 dask_kubernetes/classic/tests/test_async.py
 dask_kubernetes/classic/tests/test_sync.py
+dask_kubernetes/cli/__init__.py
+dask_kubernetes/cli/cli.py
 dask_kubernetes/common/auth.py
 dask_kubernetes/common/networking.py
 dask_kubernetes/common/objects.py
 dask_kubernetes/common/utils.py
 dask_kubernetes/common/tests/test_kind.py
 dask_kubernetes/common/tests/test_objects.py
 dask_kubernetes/experimental/__init__.py
 dask_kubernetes/helm/__init__.py
 dask_kubernetes/helm/helmcluster.py
 dask_kubernetes/helm/tests/test_helm.py
 dask_kubernetes/helm/tests/resources/values.yaml
 dask_kubernetes/operator/__init__.py
+dask_kubernetes/operator/_objects.py
 dask_kubernetes/operator/controller/__init__.py
 dask_kubernetes/operator/controller/controller.py
 dask_kubernetes/operator/controller/plugins/__init__.py
 dask_kubernetes/operator/controller/plugins/noop/__init__.py
 dask_kubernetes/operator/controller/plugins/noop/noop.py
 dask_kubernetes/operator/controller/tests/test_controller.py
 dask_kubernetes/operator/controller/tests/resources/failedjob.yaml
```

### Comparing `dask-kubernetes-2023.3.2/setup.cfg` & `dask-kubernetes-2023.6.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 000003b0: 3120 2020 2020 2020 2023 2041 6d62 6967  1        # Ambig
 000003c0: 756f 7573 2076 6172 6961 626c 6520 6e61  uous variable na
 000003d0: 6d65 730a 0957 3530 342c 2020 2020 2020  mes..W504,      
 000003e0: 2023 206c 696e 6520 6272 6561 6b20 6166   # line break af
 000003f0: 7465 7220 6269 6e61 7279 206f 7065 7261  ter binary opera
 00000400: 746f 720a 6d61 782d 6c69 6e65 2d6c 656e  tor.max-line-len
 00000410: 6774 6820 3d20 3132 300a 0a5b 7665 7273  gth = 120..[vers
-00000420: 696f 6e65 6572 5d0a 7663 7320 3d20 6769  ioneer].vcs = gi
+00000420: 696f 6e65 6572 5d0a 5643 5320 3d20 6769  ioneer].VCS = gi
 00000430: 740a 7374 796c 6520 3d20 7065 7034 3430  t.style = pep440
 00000440: 0a76 6572 7369 6f6e 6669 6c65 5f73 6f75  .versionfile_sou
 00000450: 7263 6520 3d20 6461 736b 5f6b 7562 6572  rce = dask_kuber
 00000460: 6e65 7465 732f 5f76 6572 7369 6f6e 2e70  netes/_version.p
 00000470: 790a 7665 7273 696f 6e66 696c 655f 6275  y.versionfile_bu
 00000480: 696c 6420 3d20 6461 736b 5f6b 7562 6572  ild = dask_kuber
 00000490: 6e65 7465 732f 5f76 6572 7369 6f6e 2e70  netes/_version.p
```

### Comparing `dask-kubernetes-2023.3.2/setup.py` & `dask-kubernetes-2023.6.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,18 @@
     keywords="dask,kubernetes,distributed",
     license="BSD",
     packages=find_packages(),
     include_package_data=True,
     long_description=(open("README.rst").read() if exists("README.rst") else ""),
     zip_safe=False,
     install_requires=list(open("requirements.txt").read().strip().split("\n")),
-    python_requires=">=3.8",
+    python_requires=">=3.9",
     entry_points="""
         [dask_cluster_discovery]
         helmcluster=dask_kubernetes.helm:discover
         kubecluster=dask_kubernetes.operator:discover
         [dask_operator_plugin]
         noop=dask_kubernetes.operator.controller.plugins.noop
+        [dask_cli]
+        kubernetes=dask_kubernetes.cli:main
       """,
 )
```

### Comparing `dask-kubernetes-2023.3.2/versioneer.py` & `dask-kubernetes-2023.6.0/versioneer.py`

 * *Files identical despite different names*

