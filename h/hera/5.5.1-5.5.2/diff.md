# Comparing `tmp/hera-5.5.1.tar.gz` & `tmp/hera-5.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hera-5.5.1.tar", max compression
+gzip compressed data, was "hera-5.5.2.tar", max compression
```

## Comparing `hera-5.5.1.tar` & `hera-5.5.2.tar`

### file list

```diff
@@ -1,137 +1,137 @@
--rw-r--r--   0        0        0     1066 2023-06-23 08:51:02.711439 hera-5.5.1/LICENSE
--rw-r--r--   0        0        0    12133 2023-06-23 08:51:02.711439 hera-5.5.1/README.md
--rw-r--r--   0        0        0     3530 2023-06-23 08:51:22.599661 hera-5.5.1/pyproject.toml
--rw-r--r--   0        0        0      522 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/__init__.py
--rw-r--r--   0        0        0      300 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/_version.py
--rw-r--r--   0        0        0     1289 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/auth/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/__init__.py
--rw-r--r--   0        0        0     3267 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/models/__init__.py
--rw-r--r--   0        0        0     1418 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/models/eventsource.py
--rw-r--r--   0        0        0      861 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/models/eventsource.pyi
--rw-r--r--   0        0        0      144 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/models/google/__init__.py
--rw-r--r--   0        0        0      347 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/models/google/protobuf.py
--rw-r--r--   0        0        0      164 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/models/google/protobuf.pyi
--rw-r--r--   0        0        0        0 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/models/grpc/__init__.py
--rw-r--r--   0        0        0      144 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/models/grpc/gateway/__init__.py
--rw-r--r--   0        0        0      691 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/models/grpc/gateway/runtime.py
--rw-r--r--   0        0        0      470 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/models/grpc/gateway/runtime.pyi
--rw-r--r--   0        0        0        0 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/models/io/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/models/io/argoproj/__init__.py
--rw-r--r--   0        0        0      144 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/models/io/argoproj/events/__init__.py
--rw-r--r--   0        0        0   102993 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/models/io/argoproj/events/v1alpha1.py
--rw-r--r--   0        0        0    25271 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/models/io/argoproj/events/v1alpha1.pyi
--rw-r--r--   0        0        0      144 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/models/io/argoproj/workflow/__init__.py
--rw-r--r--   0        0        0   144549 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/models/io/argoproj/workflow/v1alpha1.py
--rw-r--r--   0        0        0    31958 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi
--rw-r--r--   0        0        0        0 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/models/io/k8s/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/models/io/k8s/api/__init__.py
--rw-r--r--   0        0        0      144 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/models/io/k8s/api/core/__init__.py
--rw-r--r--   0        0        0   127883 2023-06-23 08:51:02.735439 hera-5.5.1/src/hera/events/models/io/k8s/api/core/v1.py
--rw-r--r--   0        0        0    18004 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/events/models/io/k8s/api/core/v1.pyi
--rw-r--r--   0        0        0      144 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/events/models/io/k8s/api/policy/__init__.py
--rw-r--r--   0        0        0     1751 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/events/models/io/k8s/api/policy/v1beta1.py
--rw-r--r--   0        0        0      376 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/events/models/io/k8s/api/policy/v1beta1.pyi
--rw-r--r--   0        0        0        0 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/events/models/io/k8s/apimachinery/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/events/models/io/k8s/apimachinery/pkg/__init__.py
--rw-r--r--   0        0        0      144 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/events/models/io/k8s/apimachinery/pkg/api/__init__.py
--rw-r--r--   0        0        0     3161 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py
--rw-r--r--   0        0        0      105 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.pyi
--rw-r--r--   0        0        0        0 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/events/models/io/k8s/apimachinery/pkg/apis/__init__.py
--rw-r--r--   0        0        0      144 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
--rw-r--r--   0        0        0    22218 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
--rw-r--r--   0        0        0     2064 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
--rw-r--r--   0        0        0      144 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/events/models/io/k8s/apimachinery/pkg/util/__init__.py
--rw-r--r--   0        0        0      277 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.py
--rw-r--r--   0        0        0      108 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.pyi
--rw-r--r--   0        0        0     1453 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/events/models/sensor.py
--rw-r--r--   0        0        0      887 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/events/models/sensor.pyi
--rw-r--r--   0        0        0    27607 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/events/service.py
--rw-r--r--   0        0        0     2186 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/exceptions/__init__.py
--rw-r--r--   0        0        0      282 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/expr/__init__.py
--rw-r--r--   0        0        0    12021 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/expr/_node.py
--rw-r--r--   0        0        0      647 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/expr/_sprig.py
--rw-r--r--   0        0        0        0 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/py.typed
--rw-r--r--   0        0        0      188 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/shared/__init__.py
--rw-r--r--   0        0        0      269 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/shared/_base_model.py
--rw-r--r--   0        0        0     4997 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/shared/_global_config.py
--rw-r--r--   0        0        0      513 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/shared/serialization.py
--rw-r--r--   0        0        0     4585 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/__init__.py
--rw-r--r--   0        0        0     2912 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/_context.py
--rw-r--r--   0        0        0     4741 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/_inspect.py
--rw-r--r--   0        0        0    41532 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/_mixins.py
--rw-r--r--   0        0        0    32815 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/_unparse.py
--rw-r--r--   0        0        0       25 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/action.py
--rw-r--r--   0        0        0     1115 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/archive.py
--rw-r--r--   0        0        0     7697 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/artifact.py
--rw-r--r--   0        0        0     3640 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/cluster_workflow_template.py
--rw-r--r--   0        0        0     3464 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/container.py
--rw-r--r--   0        0        0     7280 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/container_set.py
--rw-r--r--   0        0        0     9088 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/cron_workflow.py
--rw-r--r--   0        0        0     2877 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/dag.py
--rw-r--r--   0        0        0     2241 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/data.py
--rw-r--r--   0        0        0     4855 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/env.py
--rw-r--r--   0        0        0     1329 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/env_from.py
--rw-r--r--   0        0        0      208 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/exceptions.py
--rw-r--r--   0        0        0     2346 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/http_template.py
--rw-r--r--   0        0        0       30 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/memoize.py
--rw-r--r--   0        0        0     4418 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/metrics.py
--rw-r--r--   0        0        0     6913 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/models/__init__.py
--rw-r--r--   0        0        0     1418 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/models/eventsource.py
--rw-r--r--   0        0        0      861 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/models/eventsource.pyi
--rw-r--r--   0        0        0      144 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/models/google/__init__.py
--rw-r--r--   0        0        0      347 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/models/google/protobuf.py
--rw-r--r--   0        0        0      164 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/models/google/protobuf.pyi
--rw-r--r--   0        0        0        0 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/models/grpc/__init__.py
--rw-r--r--   0        0        0      144 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/models/grpc/gateway/__init__.py
--rw-r--r--   0        0        0      691 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/models/grpc/gateway/runtime.py
--rw-r--r--   0        0        0      470 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/models/grpc/gateway/runtime.pyi
--rw-r--r--   0        0        0        0 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/models/io/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/models/io/argoproj/__init__.py
--rw-r--r--   0        0        0      144 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/models/io/argoproj/events/__init__.py
--rw-r--r--   0        0        0   102993 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/models/io/argoproj/events/v1alpha1.py
--rw-r--r--   0        0        0    25271 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi
--rw-r--r--   0        0        0      144 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/models/io/argoproj/workflow/__init__.py
--rw-r--r--   0        0        0   144549 2023-06-23 08:51:02.739439 hera-5.5.1/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py
--rw-r--r--   0        0        0    31958 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi
--rw-r--r--   0        0        0        0 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/io/k8s/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/io/k8s/api/__init__.py
--rw-r--r--   0        0        0      144 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/io/k8s/api/core/__init__.py
--rw-r--r--   0        0        0   127883 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/io/k8s/api/core/v1.py
--rw-r--r--   0        0        0    18004 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/io/k8s/api/core/v1.pyi
--rw-r--r--   0        0        0      144 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/io/k8s/api/policy/__init__.py
--rw-r--r--   0        0        0     1751 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py
--rw-r--r--   0        0        0      376 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/io/k8s/api/policy/v1beta1.pyi
--rw-r--r--   0        0        0        0 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/io/k8s/apimachinery/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/__init__.py
--rw-r--r--   0        0        0      144 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/__init__.py
--rw-r--r--   0        0        0     3161 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py
--rw-r--r--   0        0        0      105 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.pyi
--rw-r--r--   0        0        0        0 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/__init__.py
--rw-r--r--   0        0        0      144 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
--rw-r--r--   0        0        0    22218 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
--rw-r--r--   0        0        0     2064 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
--rw-r--r--   0        0        0      144 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/__init__.py
--rw-r--r--   0        0        0      277 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.py
--rw-r--r--   0        0        0      108 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.pyi
--rw-r--r--   0        0        0     1453 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/sensor.py
--rw-r--r--   0        0        0      887 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/models/sensor.pyi
--rw-r--r--   0        0        0      722 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/operator.py
--rw-r--r--   0        0        0     4084 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/parameter.py
--rw-r--r--   0        0        0     1076 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/protocol.py
--rw-r--r--   0        0        0     3146 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/resource.py
--rw-r--r--   0        0        0     5262 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/resources.py
--rw-r--r--   0        0        0     1856 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/retry_strategy.py
--rw-r--r--   0        0        0     3707 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/runner.py
--rw-r--r--   0        0        0    16736 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/script.py
--rw-r--r--   0        0        0    55301 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/service.py
--rw-r--r--   0        0        0     6747 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/steps.py
--rw-r--r--   0        0        0     3332 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/suspend.py
--rw-r--r--   0        0        0     7959 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/task.py
--rw-r--r--   0        0        0       27 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/toleration.py
--rw-r--r--   0        0        0     2007 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/user_container.py
--rw-r--r--   0        0        0     2610 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/validators.py
--rw-r--r--   0        0        0    18709 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/volume.py
--rw-r--r--   0        0        0    22337 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/workflow.py
--rw-r--r--   0        0        0      911 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/workflow_status.py
--rw-r--r--   0        0        0     7450 2023-06-23 08:51:02.743439 hera-5.5.1/src/hera/workflows/workflow_template.py
--rw-r--r--   0        0        0    13556 1970-01-01 00:00:00.000000 hera-5.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-26 15:59:36.612145 hera-5.5.2/LICENSE
+-rw-r--r--   0        0        0    12133 2023-06-26 15:59:36.612145 hera-5.5.2/README.md
+-rw-r--r--   0        0        0     3530 2023-06-26 15:59:54.520722 hera-5.5.2/pyproject.toml
+-rw-r--r--   0        0        0      522 2023-06-26 15:59:36.632146 hera-5.5.2/src/hera/__init__.py
+-rw-r--r--   0        0        0      300 2023-06-26 15:59:36.632146 hera-5.5.2/src/hera/_version.py
+-rw-r--r--   0        0        0     1289 2023-06-26 15:59:36.632146 hera-5.5.2/src/hera/auth/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 15:59:36.632146 hera-5.5.2/src/hera/events/__init__.py
+-rw-r--r--   0        0        0     3267 2023-06-26 15:59:36.632146 hera-5.5.2/src/hera/events/models/__init__.py
+-rw-r--r--   0        0        0     1418 2023-06-26 15:59:36.632146 hera-5.5.2/src/hera/events/models/eventsource.py
+-rw-r--r--   0        0        0      861 2023-06-26 15:59:36.632146 hera-5.5.2/src/hera/events/models/eventsource.pyi
+-rw-r--r--   0        0        0      144 2023-06-26 15:59:36.632146 hera-5.5.2/src/hera/events/models/google/__init__.py
+-rw-r--r--   0        0        0      347 2023-06-26 15:59:36.632146 hera-5.5.2/src/hera/events/models/google/protobuf.py
+-rw-r--r--   0        0        0      164 2023-06-26 15:59:36.632146 hera-5.5.2/src/hera/events/models/google/protobuf.pyi
+-rw-r--r--   0        0        0        0 2023-06-26 15:59:36.632146 hera-5.5.2/src/hera/events/models/grpc/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-26 15:59:36.632146 hera-5.5.2/src/hera/events/models/grpc/gateway/__init__.py
+-rw-r--r--   0        0        0      691 2023-06-26 15:59:36.632146 hera-5.5.2/src/hera/events/models/grpc/gateway/runtime.py
+-rw-r--r--   0        0        0      470 2023-06-26 15:59:36.632146 hera-5.5.2/src/hera/events/models/grpc/gateway/runtime.pyi
+-rw-r--r--   0        0        0        0 2023-06-26 15:59:36.632146 hera-5.5.2/src/hera/events/models/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 15:59:36.632146 hera-5.5.2/src/hera/events/models/io/argoproj/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-26 15:59:36.632146 hera-5.5.2/src/hera/events/models/io/argoproj/events/__init__.py
+-rw-r--r--   0        0        0   102993 2023-06-26 15:59:36.632146 hera-5.5.2/src/hera/events/models/io/argoproj/events/v1alpha1.py
+-rw-r--r--   0        0        0    25271 2023-06-26 15:59:36.632146 hera-5.5.2/src/hera/events/models/io/argoproj/events/v1alpha1.pyi
+-rw-r--r--   0        0        0      144 2023-06-26 15:59:36.632146 hera-5.5.2/src/hera/events/models/io/argoproj/workflow/__init__.py
+-rw-r--r--   0        0        0   144549 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/io/argoproj/workflow/v1alpha1.py
+-rw-r--r--   0        0        0    31958 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi
+-rw-r--r--   0        0        0        0 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/io/k8s/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/io/k8s/api/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/io/k8s/api/core/__init__.py
+-rw-r--r--   0        0        0   127883 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/io/k8s/api/core/v1.py
+-rw-r--r--   0        0        0    18004 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/io/k8s/api/core/v1.pyi
+-rw-r--r--   0        0        0      144 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/io/k8s/api/policy/__init__.py
+-rw-r--r--   0        0        0     1751 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/io/k8s/api/policy/v1beta1.py
+-rw-r--r--   0        0        0      376 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/io/k8s/api/policy/v1beta1.pyi
+-rw-r--r--   0        0        0        0 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/io/k8s/apimachinery/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/io/k8s/apimachinery/pkg/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/io/k8s/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0        0        0     3161 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py
+-rw-r--r--   0        0        0      105 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.pyi
+-rw-r--r--   0        0        0        0 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/io/k8s/apimachinery/pkg/apis/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
+-rw-r--r--   0        0        0    22218 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
+-rw-r--r--   0        0        0     2064 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
+-rw-r--r--   0        0        0      144 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/io/k8s/apimachinery/pkg/util/__init__.py
+-rw-r--r--   0        0        0      277 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.py
+-rw-r--r--   0        0        0      108 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.pyi
+-rw-r--r--   0        0        0     1453 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/sensor.py
+-rw-r--r--   0        0        0      887 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/models/sensor.pyi
+-rw-r--r--   0        0        0    27607 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/events/service.py
+-rw-r--r--   0        0        0     2186 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/exceptions/__init__.py
+-rw-r--r--   0        0        0      282 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/expr/__init__.py
+-rw-r--r--   0        0        0    12021 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/expr/_node.py
+-rw-r--r--   0        0        0      647 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/expr/_sprig.py
+-rw-r--r--   0        0        0        0 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/py.typed
+-rw-r--r--   0        0        0      188 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/shared/__init__.py
+-rw-r--r--   0        0        0      269 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/shared/_base_model.py
+-rw-r--r--   0        0        0     4997 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/shared/_global_config.py
+-rw-r--r--   0        0        0      513 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/shared/serialization.py
+-rw-r--r--   0        0        0     4585 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/workflows/__init__.py
+-rw-r--r--   0        0        0     2912 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/workflows/_context.py
+-rw-r--r--   0        0        0     4741 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/workflows/_inspect.py
+-rw-r--r--   0        0        0    41532 2023-06-26 15:59:36.636146 hera-5.5.2/src/hera/workflows/_mixins.py
+-rw-r--r--   0        0        0    32815 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/_unparse.py
+-rw-r--r--   0        0        0       25 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/action.py
+-rw-r--r--   0        0        0     1115 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/archive.py
+-rw-r--r--   0        0        0     7697 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/artifact.py
+-rw-r--r--   0        0        0     3640 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/cluster_workflow_template.py
+-rw-r--r--   0        0        0     3464 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/container.py
+-rw-r--r--   0        0        0     7280 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/container_set.py
+-rw-r--r--   0        0        0     9088 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/cron_workflow.py
+-rw-r--r--   0        0        0     2877 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/dag.py
+-rw-r--r--   0        0        0     2241 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/data.py
+-rw-r--r--   0        0        0     4855 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/env.py
+-rw-r--r--   0        0        0     1329 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/env_from.py
+-rw-r--r--   0        0        0      208 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/exceptions.py
+-rw-r--r--   0        0        0     2346 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/http_template.py
+-rw-r--r--   0        0        0       30 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/memoize.py
+-rw-r--r--   0        0        0     4418 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/metrics.py
+-rw-r--r--   0        0        0     6913 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/__init__.py
+-rw-r--r--   0        0        0     1418 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/eventsource.py
+-rw-r--r--   0        0        0      861 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/eventsource.pyi
+-rw-r--r--   0        0        0      144 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/google/__init__.py
+-rw-r--r--   0        0        0      347 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/google/protobuf.py
+-rw-r--r--   0        0        0      164 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/google/protobuf.pyi
+-rw-r--r--   0        0        0        0 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/grpc/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/grpc/gateway/__init__.py
+-rw-r--r--   0        0        0      691 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/grpc/gateway/runtime.py
+-rw-r--r--   0        0        0      470 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/grpc/gateway/runtime.pyi
+-rw-r--r--   0        0        0        0 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/argoproj/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/argoproj/events/__init__.py
+-rw-r--r--   0        0        0   102993 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/argoproj/events/v1alpha1.py
+-rw-r--r--   0        0        0    25271 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi
+-rw-r--r--   0        0        0      144 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/argoproj/workflow/__init__.py
+-rw-r--r--   0        0        0   144549 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py
+-rw-r--r--   0        0        0    31958 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi
+-rw-r--r--   0        0        0        0 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/k8s/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/k8s/api/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/k8s/api/core/__init__.py
+-rw-r--r--   0        0        0   127883 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/k8s/api/core/v1.py
+-rw-r--r--   0        0        0    18004 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/k8s/api/core/v1.pyi
+-rw-r--r--   0        0        0      144 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/k8s/api/policy/__init__.py
+-rw-r--r--   0        0        0     1751 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py
+-rw-r--r--   0        0        0      376 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/k8s/api/policy/v1beta1.pyi
+-rw-r--r--   0        0        0        0 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/k8s/apimachinery/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0        0        0     3161 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py
+-rw-r--r--   0        0        0      105 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.pyi
+-rw-r--r--   0        0        0        0 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
+-rw-r--r--   0        0        0    22218 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
+-rw-r--r--   0        0        0     2064 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
+-rw-r--r--   0        0        0      144 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/__init__.py
+-rw-r--r--   0        0        0      277 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.py
+-rw-r--r--   0        0        0      108 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.pyi
+-rw-r--r--   0        0        0     1453 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/sensor.py
+-rw-r--r--   0        0        0      887 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/models/sensor.pyi
+-rw-r--r--   0        0        0      722 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/operator.py
+-rw-r--r--   0        0        0     4084 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/parameter.py
+-rw-r--r--   0        0        0     1076 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/protocol.py
+-rw-r--r--   0        0        0     3146 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/resource.py
+-rw-r--r--   0        0        0     5262 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/resources.py
+-rw-r--r--   0        0        0     1856 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/retry_strategy.py
+-rw-r--r--   0        0        0     3703 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/runner.py
+-rw-r--r--   0        0        0    16736 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/script.py
+-rw-r--r--   0        0        0    55301 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/service.py
+-rw-r--r--   0        0        0     6747 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/steps.py
+-rw-r--r--   0        0        0     3332 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/suspend.py
+-rw-r--r--   0        0        0     7959 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/task.py
+-rw-r--r--   0        0        0       27 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/toleration.py
+-rw-r--r--   0        0        0     2007 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/user_container.py
+-rw-r--r--   0        0        0     2610 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/validators.py
+-rw-r--r--   0        0        0    18709 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/volume.py
+-rw-r--r--   0        0        0    22337 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/workflow.py
+-rw-r--r--   0        0        0      911 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/workflow_status.py
+-rw-r--r--   0        0        0     7450 2023-06-26 15:59:36.640146 hera-5.5.2/src/hera/workflows/workflow_template.py
+-rw-r--r--   0        0        0    13556 1970-01-01 00:00:00.000000 hera-5.5.2/PKG-INFO
```

### Comparing `hera-5.5.1/LICENSE` & `hera-5.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/README.md` & `hera-5.5.2/README.md`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/pyproject.toml` & `hera-5.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "hera"  # project-name
 # The version is automatically substituted by the CI
-version = "5.5.1"
+version = "5.5.2"
 description = "Hera is a Python framework for constructing and submitting Argo Workflows. The main goal of Hera is to make Argo Workflows more accessible by abstracting away some setup that is typically necessary for constructing Argo workflows."
 authors = ["Flaviu Vadan <flaviu.vadan@dynotx.com>", "Sambhav Kothari <sambhavs.email@gmail.com>", "Elliot Gunton <elliotgunton@gmail.com>"]
 maintainers = ["Flaviu Vadan <flaviu.vadan@dynotx.com>", "Sambhav Kothari <sambhavs.email@gmail.com>", "Elliot Gunton <elliotgunton@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/argoproj-labs/hera"
 repository = "https://github.com/argoproj-labs/hera"
```

### Comparing `hera-5.5.1/src/hera/__init__.py` & `hera-5.5.2/src/hera/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/auth/__init__.py` & `hera-5.5.2/src/hera/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/events/models/__init__.py` & `hera-5.5.2/src/hera/events/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/events/models/eventsource.py` & `hera-5.5.2/src/hera/events/models/eventsource.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/events/models/eventsource.pyi` & `hera-5.5.2/src/hera/events/models/eventsource.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/events/models/grpc/gateway/runtime.py` & `hera-5.5.2/src/hera/events/models/grpc/gateway/runtime.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/events/models/io/argoproj/events/v1alpha1.py` & `hera-5.5.2/src/hera/events/models/io/argoproj/events/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/events/models/io/argoproj/events/v1alpha1.pyi` & `hera-5.5.2/src/hera/events/models/io/argoproj/events/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/events/models/io/argoproj/workflow/v1alpha1.py` & `hera-5.5.2/src/hera/events/models/io/argoproj/workflow/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi` & `hera-5.5.2/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/events/models/io/k8s/api/core/v1.py` & `hera-5.5.2/src/hera/events/models/io/k8s/api/core/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/events/models/io/k8s/api/core/v1.pyi` & `hera-5.5.2/src/hera/events/models/io/k8s/api/core/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/events/models/io/k8s/api/policy/v1beta1.py` & `hera-5.5.2/src/hera/events/models/io/k8s/api/policy/v1beta1.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py` & `hera-5.5.2/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py` & `hera-5.5.2/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi` & `hera-5.5.2/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/events/models/sensor.py` & `hera-5.5.2/src/hera/events/models/sensor.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/events/models/sensor.pyi` & `hera-5.5.2/src/hera/events/models/sensor.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/events/service.py` & `hera-5.5.2/src/hera/events/service.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/exceptions/__init__.py` & `hera-5.5.2/src/hera/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/expr/_node.py` & `hera-5.5.2/src/hera/expr/_node.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/expr/_sprig.py` & `hera-5.5.2/src/hera/expr/_sprig.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/shared/_global_config.py` & `hera-5.5.2/src/hera/shared/_global_config.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/shared/serialization.py` & `hera-5.5.2/src/hera/shared/serialization.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/__init__.py` & `hera-5.5.2/src/hera/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/_context.py` & `hera-5.5.2/src/hera/workflows/_context.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/_inspect.py` & `hera-5.5.2/src/hera/workflows/_inspect.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/_mixins.py` & `hera-5.5.2/src/hera/workflows/_mixins.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/_unparse.py` & `hera-5.5.2/src/hera/workflows/_unparse.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/archive.py` & `hera-5.5.2/src/hera/workflows/archive.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/artifact.py` & `hera-5.5.2/src/hera/workflows/artifact.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/cluster_workflow_template.py` & `hera-5.5.2/src/hera/workflows/cluster_workflow_template.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/container.py` & `hera-5.5.2/src/hera/workflows/container.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/container_set.py` & `hera-5.5.2/src/hera/workflows/container_set.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/cron_workflow.py` & `hera-5.5.2/src/hera/workflows/cron_workflow.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/dag.py` & `hera-5.5.2/src/hera/workflows/dag.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/data.py` & `hera-5.5.2/src/hera/workflows/data.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/env.py` & `hera-5.5.2/src/hera/workflows/env.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/env_from.py` & `hera-5.5.2/src/hera/workflows/env_from.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/http_template.py` & `hera-5.5.2/src/hera/workflows/http_template.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/metrics.py` & `hera-5.5.2/src/hera/workflows/metrics.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/models/__init__.py` & `hera-5.5.2/src/hera/workflows/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/models/eventsource.py` & `hera-5.5.2/src/hera/workflows/models/eventsource.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/models/eventsource.pyi` & `hera-5.5.2/src/hera/workflows/models/eventsource.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/models/grpc/gateway/runtime.py` & `hera-5.5.2/src/hera/workflows/models/grpc/gateway/runtime.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/models/io/argoproj/events/v1alpha1.py` & `hera-5.5.2/src/hera/workflows/models/io/argoproj/events/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi` & `hera-5.5.2/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py` & `hera-5.5.2/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi` & `hera-5.5.2/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/models/io/k8s/api/core/v1.py` & `hera-5.5.2/src/hera/workflows/models/io/k8s/api/core/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/models/io/k8s/api/core/v1.pyi` & `hera-5.5.2/src/hera/workflows/models/io/k8s/api/core/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py` & `hera-5.5.2/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py` & `hera-5.5.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py` & `hera-5.5.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi` & `hera-5.5.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/models/sensor.py` & `hera-5.5.2/src/hera/workflows/models/sensor.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/models/sensor.pyi` & `hera-5.5.2/src/hera/workflows/models/sensor.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/operator.py` & `hera-5.5.2/src/hera/workflows/operator.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/parameter.py` & `hera-5.5.2/src/hera/workflows/parameter.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/protocol.py` & `hera-5.5.2/src/hera/workflows/protocol.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/resource.py` & `hera-5.5.2/src/hera/workflows/resource.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/resources.py` & `hera-5.5.2/src/hera/workflows/resources.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/retry_strategy.py` & `hera-5.5.2/src/hera/workflows/retry_strategy.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/runner.py` & `hera-5.5.2/src/hera/workflows/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     # if the function is wrapped, unwrap it
     # this may happen if the function is decorated with @script
     if hasattr(function, "wrapped_function"):
         function = function.wrapped_function
     # convert the kwargs list to a dict
     kwargs = {}
     for kwarg in kwargs_list:
-        if not kwarg.get("name") or not kwarg.get("value"):
+        if "name" not in kwarg or "value" not in kwarg:
             continue
         # sanitize the key for python
         key = serialize(kwarg["name"]).replace("-", "_")
         value = kwarg["value"]
         kwargs[key] = value
     function = validate_arguments(function)
     function = _ignore_unmatched_kwargs(function)
```

### Comparing `hera-5.5.1/src/hera/workflows/script.py` & `hera-5.5.2/src/hera/workflows/script.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/service.py` & `hera-5.5.2/src/hera/workflows/service.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/steps.py` & `hera-5.5.2/src/hera/workflows/steps.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/suspend.py` & `hera-5.5.2/src/hera/workflows/suspend.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/task.py` & `hera-5.5.2/src/hera/workflows/task.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/user_container.py` & `hera-5.5.2/src/hera/workflows/user_container.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/validators.py` & `hera-5.5.2/src/hera/workflows/validators.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/volume.py` & `hera-5.5.2/src/hera/workflows/volume.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/workflow.py` & `hera-5.5.2/src/hera/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/workflow_status.py` & `hera-5.5.2/src/hera/workflows/workflow_status.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/src/hera/workflows/workflow_template.py` & `hera-5.5.2/src/hera/workflows/workflow_template.py`

 * *Files identical despite different names*

### Comparing `hera-5.5.1/PKG-INFO` & `hera-5.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hera
-Version: 5.5.1
+Version: 5.5.2
 Summary: Hera is a Python framework for constructing and submitting Argo Workflows. The main goal of Hera is to make Argo Workflows more accessible by abstracting away some setup that is typically necessary for constructing Argo workflows.
 Home-page: https://github.com/argoproj-labs/hera
 License: MIT
 Author: Flaviu Vadan
 Author-email: flaviu.vadan@dynotx.com
 Maintainer: Flaviu Vadan
 Maintainer-email: flaviu.vadan@dynotx.com
```

