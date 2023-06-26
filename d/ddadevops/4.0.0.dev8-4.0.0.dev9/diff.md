# Comparing `tmp/ddadevops-4.0.0.dev8.tar.gz` & `tmp/ddadevops-4.0.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddadevops-4.0.0.dev8.tar", last modified: Fri Mar 17 14:56:16 2023, max compression
+gzip compressed data, was "ddadevops-4.0.0.dev9.tar", last modified: Fri Mar 17 14:59:47 2023, max compression
```

## Comparing `ddadevops-4.0.0.dev8.tar` & `ddadevops-4.0.0.dev9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:56:16.866872 ddadevops-4.0.0.dev8/
--rw-rw-r--   0 jem       (1000) jem       (1000)      137 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/MANIFEST.in
--rw-rw-r--   0 jem       (1000) jem       (1000)     7958 2023-03-17 14:56:16.866872 ddadevops-4.0.0.dev8/PKG-INFO
--rw-rw-r--   0 jem       (1000) jem       (1000)        0 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/__init__.py
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:56:16.862872 ddadevops-4.0.0.dev8/ddadevops/
--rw-rw-r--   0 jem       (1000) jem       (1000)    11357 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/ddadevops/LICENSE
--rw-rw-r--   0 jem       (1000) jem       (1000)     1501 2023-03-14 14:07:46.000000 ddadevops-4.0.0.dev8/ddadevops/__init__.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     2070 2023-03-16 12:54:27.000000 ddadevops-4.0.0.dev8/ddadevops/application.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     1962 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev8/ddadevops/aws_backend_properties_mixin.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     3815 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev8/ddadevops/aws_mfa_mixin.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     5988 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev8/ddadevops/aws_rds_pg_mixin.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     2648 2023-03-14 14:05:21.000000 ddadevops-4.0.0.dev8/ddadevops/c4k_mixin.py
--rw-rw-r--   0 jem       (1000) jem       (1000)      468 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev8/ddadevops/credential.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     1922 2023-03-16 13:01:31.000000 ddadevops-4.0.0.dev8/ddadevops/devops_build.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     2707 2023-03-14 17:43:27.000000 ddadevops-4.0.0.dev8/ddadevops/devops_docker_build.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     9996 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev8/ddadevops/devops_terraform_build.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     2885 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev8/ddadevops/digitalocean_backend_properties_mixin.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     3489 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev8/ddadevops/digitalocean_terraform_build.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     4283 2023-03-14 17:32:30.000000 ddadevops-4.0.0.dev8/ddadevops/domain.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     1265 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev8/ddadevops/exoscale_mixin.py
--rw-rw-r--   0 jem       (1000) jem       (1000)      981 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev8/ddadevops/hetzner_mixin.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     3494 2023-03-17 14:55:32.000000 ddadevops-4.0.0.dev8/ddadevops/infrastructure.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     4712 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev8/ddadevops/provs_k3s_mixin.py
--rw-rw-r--   0 jem       (1000) jem       (1000)      475 2023-03-17 12:15:02.000000 ddadevops-4.0.0.dev8/ddadevops/python_util.py
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:56:16.866872 ddadevops-4.0.0.dev8/ddadevops/release_mixin/
--rw-rw-r--   0 jem       (1000) jem       (1000)        0 2023-03-11 08:22:26.000000 ddadevops-4.0.0.dev8/ddadevops/release_mixin/__init__.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     1175 2023-03-11 08:22:26.000000 ddadevops-4.0.0.dev8/ddadevops/release_mixin/build.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     2724 2023-03-11 08:22:26.000000 ddadevops-4.0.0.dev8/ddadevops/release_mixin/domain.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     2100 2023-03-11 08:22:26.000000 ddadevops-4.0.0.dev8/ddadevops/release_mixin/infrastructure.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     8136 2023-03-11 08:22:26.000000 ddadevops-4.0.0.dev8/ddadevops/release_mixin/infrastructure_api.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     1808 2023-03-11 08:22:26.000000 ddadevops-4.0.0.dev8/ddadevops/release_mixin/release_mixin.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     1391 2023-03-11 08:22:26.000000 ddadevops-4.0.0.dev8/ddadevops/release_mixin/services.py
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:56:16.858873 ddadevops-4.0.0.dev8/ddadevops/src/
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:56:16.858873 ddadevops-4.0.0.dev8/ddadevops/src/main/
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:56:16.858873 ddadevops-4.0.0.dev8/ddadevops/src/main/resources/
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:56:16.858873 ddadevops-4.0.0.dev8/ddadevops/src/main/resources/docker/
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:56:16.858873 ddadevops-4.0.0.dev8/ddadevops/src/main/resources/docker/image/
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:56:16.866872 ddadevops-4.0.0.dev8/ddadevops/src/main/resources/docker/image/resources/
--rwxrwxr-x   0 jem       (1000) jem       (1000)      628 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/ddadevops/src/main/resources/docker/image/resources/install_functions.sh
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:56:16.866872 ddadevops-4.0.0.dev8/ddadevops/src/main/resources/terraform/
--rw-rw-r--   0 jem       (1000) jem       (1000)      111 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/ddadevops/src/main/resources/terraform/aws_backend_properties_vars.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       59 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/ddadevops/src/main/resources/terraform/aws_backend_with_properties.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       41 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/ddadevops/src/main/resources/terraform/aws_provider.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)      109 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/ddadevops/src/main/resources/terraform/do_backend_properties_vars.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)      191 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/ddadevops/src/main/resources/terraform/do_backend_with_properties.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       99 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/ddadevops/src/main/resources/terraform/do_mixin_vars.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)      145 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/ddadevops/src/main/resources/terraform/do_provider.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       67 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/ddadevops/src/main/resources/terraform/exoscale_mixin_vars.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       97 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/ddadevops/src/main/resources/terraform/exoscale_provider.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       31 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/ddadevops/src/main/resources/terraform/hetzner_mixin_vars.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       91 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/ddadevops/src/main/resources/terraform/hetzner_provider.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)      483 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/ddadevops/src/main/resources/terraform/provider_registry.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       40 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/ddadevops/src/main/resources/terraform/terraform_build_vars.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       46 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/ddadevops/src/main/resources/terraform/versions.tf
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:56:16.862872 ddadevops-4.0.0.dev8/ddadevops.egg-info/
--rw-rw-r--   0 jem       (1000) jem       (1000)     7958 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/ddadevops.egg-info/PKG-INFO
--rw-rw-r--   0 jem       (1000) jem       (1000)     1990 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/ddadevops.egg-info/SOURCES.txt
--rw-rw-r--   0 jem       (1000) jem       (1000)        1 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/ddadevops.egg-info/dependency_links.txt
--rw-rw-r--   0 jem       (1000) jem       (1000)        1 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/ddadevops.egg-info/namespace_packages.txt
--rw-rw-r--   0 jem       (1000) jem       (1000)       11 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/ddadevops.egg-info/top_level.txt
--rw-rw-r--   0 jem       (1000) jem       (1000)        1 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/ddadevops.egg-info/zip-safe
--rw-rw-r--   0 jem       (1000) jem       (1000)       38 2023-03-17 14:56:16.870872 ddadevops-4.0.0.dev8/setup.cfg
--rwxr-xr-x   0 jem       (1000) jem       (1000)     9507 2023-03-17 14:56:16.000000 ddadevops-4.0.0.dev8/setup.py
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:47.018865 ddadevops-4.0.0.dev9/
+-rw-rw-r--   0 jem       (1000) jem       (1000)      137 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/MANIFEST.in
+-rw-rw-r--   0 jem       (1000) jem       (1000)     7958 2023-03-17 14:59:47.018865 ddadevops-4.0.0.dev9/PKG-INFO
+-rw-rw-r--   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/__init__.py
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:47.014865 ddadevops-4.0.0.dev9/ddadevops/
+-rw-rw-r--   0 jem       (1000) jem       (1000)    11357 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/LICENSE
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1501 2023-03-14 14:07:46.000000 ddadevops-4.0.0.dev9/ddadevops/__init__.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2070 2023-03-16 12:54:27.000000 ddadevops-4.0.0.dev9/ddadevops/application.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1962 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev9/ddadevops/aws_backend_properties_mixin.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     3815 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev9/ddadevops/aws_mfa_mixin.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     5988 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev9/ddadevops/aws_rds_pg_mixin.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2648 2023-03-14 14:05:21.000000 ddadevops-4.0.0.dev9/ddadevops/c4k_mixin.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)      468 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev9/ddadevops/credential.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1922 2023-03-16 13:01:31.000000 ddadevops-4.0.0.dev9/ddadevops/devops_build.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2710 2023-03-17 14:59:22.000000 ddadevops-4.0.0.dev9/ddadevops/devops_docker_build.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     9996 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev9/ddadevops/devops_terraform_build.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2885 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev9/ddadevops/digitalocean_backend_properties_mixin.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     3489 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev9/ddadevops/digitalocean_terraform_build.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     4283 2023-03-14 17:32:30.000000 ddadevops-4.0.0.dev9/ddadevops/domain.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1265 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev9/ddadevops/exoscale_mixin.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)      981 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev9/ddadevops/hetzner_mixin.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     3494 2023-03-17 14:55:32.000000 ddadevops-4.0.0.dev9/ddadevops/infrastructure.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     4712 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev9/ddadevops/provs_k3s_mixin.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)      475 2023-03-17 12:15:02.000000 ddadevops-4.0.0.dev9/ddadevops/python_util.py
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:47.014865 ddadevops-4.0.0.dev9/ddadevops/release_mixin/
+-rw-rw-r--   0 jem       (1000) jem       (1000)        0 2023-03-11 08:22:26.000000 ddadevops-4.0.0.dev9/ddadevops/release_mixin/__init__.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1175 2023-03-11 08:22:26.000000 ddadevops-4.0.0.dev9/ddadevops/release_mixin/build.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2724 2023-03-11 08:22:26.000000 ddadevops-4.0.0.dev9/ddadevops/release_mixin/domain.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2100 2023-03-11 08:22:26.000000 ddadevops-4.0.0.dev9/ddadevops/release_mixin/infrastructure.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     8136 2023-03-11 08:22:26.000000 ddadevops-4.0.0.dev9/ddadevops/release_mixin/infrastructure_api.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1808 2023-03-11 08:22:26.000000 ddadevops-4.0.0.dev9/ddadevops/release_mixin/release_mixin.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1391 2023-03-11 08:22:26.000000 ddadevops-4.0.0.dev9/ddadevops/release_mixin/services.py
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:47.010865 ddadevops-4.0.0.dev9/ddadevops/src/
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:47.010865 ddadevops-4.0.0.dev9/ddadevops/src/main/
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:47.010865 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:47.010865 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/docker/
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:47.010865 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/docker/image/
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:47.014865 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/docker/image/resources/
+-rwxrwxr-x   0 jem       (1000) jem       (1000)      628 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/docker/image/resources/install_functions.sh
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:47.018865 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/
+-rw-rw-r--   0 jem       (1000) jem       (1000)      111 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/aws_backend_properties_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       59 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/aws_backend_with_properties.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       41 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/aws_provider.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)      109 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/do_backend_properties_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)      191 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/do_backend_with_properties.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       99 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/do_mixin_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)      145 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/do_provider.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       67 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/exoscale_mixin_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       97 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/exoscale_provider.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       31 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/hetzner_mixin_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       91 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/hetzner_provider.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)      483 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/provider_registry.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       40 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/terraform_build_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       46 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/versions.tf
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:47.014865 ddadevops-4.0.0.dev9/ddadevops.egg-info/
+-rw-rw-r--   0 jem       (1000) jem       (1000)     7958 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops.egg-info/PKG-INFO
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1990 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops.egg-info/SOURCES.txt
+-rw-rw-r--   0 jem       (1000) jem       (1000)        1 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops.egg-info/dependency_links.txt
+-rw-rw-r--   0 jem       (1000) jem       (1000)        1 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops.egg-info/namespace_packages.txt
+-rw-rw-r--   0 jem       (1000) jem       (1000)       11 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops.egg-info/top_level.txt
+-rw-rw-r--   0 jem       (1000) jem       (1000)        1 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops.egg-info/zip-safe
+-rw-rw-r--   0 jem       (1000) jem       (1000)       38 2023-03-17 14:59:47.018865 ddadevops-4.0.0.dev9/setup.cfg
+-rwxr-xr-x   0 jem       (1000) jem       (1000)     9507 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/setup.py
```

### Comparing `ddadevops-4.0.0.dev8/PKG-INFO` & `ddadevops-4.0.0.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddadevops
-Version: 4.0.0.dev8
+Version: 4.0.0.dev9
 Summary: tools to support builds combining gopass, terraform, dda-pallet, aws & hetzner-cloud
 Home-page: https://github.com/DomainDrivenArchitecture/dda-devops-build
 Author: meissa GmbH
 Author-email: buero@meissa-gmbh.de
 Maintainer: 
 Maintainer-email: 
 License: Apache Software License
```

### Comparing `ddadevops-4.0.0.dev8/ddadevops/LICENSE` & `ddadevops-4.0.0.dev9/ddadevops/LICENSE`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops/__init__.py` & `ddadevops-4.0.0.dev9/ddadevops/__init__.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops/application.py` & `ddadevops-4.0.0.dev9/ddadevops/application.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops/aws_backend_properties_mixin.py` & `ddadevops-4.0.0.dev9/ddadevops/aws_backend_properties_mixin.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops/aws_mfa_mixin.py` & `ddadevops-4.0.0.dev9/ddadevops/aws_mfa_mixin.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops/aws_rds_pg_mixin.py` & `ddadevops-4.0.0.dev9/ddadevops/aws_rds_pg_mixin.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops/c4k_mixin.py` & `ddadevops-4.0.0.dev9/ddadevops/c4k_mixin.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops/devops_build.py` & `ddadevops-4.0.0.dev9/ddadevops/devops_build.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops/devops_docker_build.py` & `ddadevops-4.0.0.dev9/ddadevops/devops_docker_build.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,8 +67,8 @@
 
     def dockerhub_publish(self):
         docker = self.repo.get_docker(self.project)
         self.docker_build_service.dockerhub_publish(docker)
 
     def test(self):
         docker = self.repo.get_docker(self.project)
-        self.test.dockerhub_publish(docker)
+        self.docker_build_service.test(docker)
```

### Comparing `ddadevops-4.0.0.dev8/ddadevops/devops_terraform_build.py` & `ddadevops-4.0.0.dev9/ddadevops/devops_terraform_build.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops/digitalocean_backend_properties_mixin.py` & `ddadevops-4.0.0.dev9/ddadevops/digitalocean_backend_properties_mixin.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops/digitalocean_terraform_build.py` & `ddadevops-4.0.0.dev9/ddadevops/digitalocean_terraform_build.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops/domain.py` & `ddadevops-4.0.0.dev9/ddadevops/domain.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops/exoscale_mixin.py` & `ddadevops-4.0.0.dev9/ddadevops/exoscale_mixin.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops/hetzner_mixin.py` & `ddadevops-4.0.0.dev9/ddadevops/hetzner_mixin.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops/infrastructure.py` & `ddadevops-4.0.0.dev9/ddadevops/infrastructure.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops/provs_k3s_mixin.py` & `ddadevops-4.0.0.dev9/ddadevops/provs_k3s_mixin.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops/release_mixin/build.py` & `ddadevops-4.0.0.dev9/ddadevops/release_mixin/build.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops/release_mixin/domain.py` & `ddadevops-4.0.0.dev9/ddadevops/release_mixin/domain.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops/release_mixin/infrastructure.py` & `ddadevops-4.0.0.dev9/ddadevops/release_mixin/infrastructure.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops/release_mixin/infrastructure_api.py` & `ddadevops-4.0.0.dev9/ddadevops/release_mixin/infrastructure_api.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops/release_mixin/release_mixin.py` & `ddadevops-4.0.0.dev9/ddadevops/release_mixin/release_mixin.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops/release_mixin/services.py` & `ddadevops-4.0.0.dev9/ddadevops/release_mixin/services.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops/src/main/resources/docker/image/resources/install_functions.sh` & `ddadevops-4.0.0.dev9/ddadevops/src/main/resources/docker/image/resources/install_functions.sh`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/ddadevops.egg-info/PKG-INFO` & `ddadevops-4.0.0.dev9/ddadevops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddadevops
-Version: 4.0.0.dev8
+Version: 4.0.0.dev9
 Summary: tools to support builds combining gopass, terraform, dda-pallet, aws & hetzner-cloud
 Home-page: https://github.com/DomainDrivenArchitecture/dda-devops-build
 Author: meissa GmbH
 Author-email: buero@meissa-gmbh.de
 Maintainer: 
 Maintainer-email: 
 License: Apache Software License
```

### Comparing `ddadevops-4.0.0.dev8/ddadevops.egg-info/SOURCES.txt` & `ddadevops-4.0.0.dev9/ddadevops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev8/setup.py` & `ddadevops-4.0.0.dev9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'ddadevops',
-        version = '4.0.0-dev8',
+        version = '4.0.0-dev9',
         description = 'tools to support builds combining gopass, terraform, dda-pallet, aws & hetzner-cloud',
         long_description = '# dda-devops-build\n\n[![Slack](https://img.shields.io/badge/chat-clojurians-green.svg?style=flat)](https://clojurians.slack.com/messages/#dda-pallet/) | [<img src="https://meissa-gmbh.de/img/community/Mastodon_Logotype.svg" width=20 alt="team@social.meissa-gmbh.de"> team@social.meissa-gmbh.de](https://social.meissa-gmbh.de/@team) | [Website & Blog](https://domaindrivenarchitecture.org)\n\n![release prod](https://github.com/DomainDrivenArchitecture/dda-devops-build/workflows/release%20prod/badge.svg)\n\ndda-devops-build provide a environment to tie several DevOps tools together for easy interoperation. Supported tools are:\n* aws with\n  * simple api-key auth\n  * mfa & assume-role auth\n* hetzner with simple api-key auth\n* terraform v0.11, v0.12 supporting\n  * local file backends\n  * s3 backends\n* docker / dockerhub\n* user / team credentials managed by gopass\n* dda-pallet\n\n# Setup\n\nEnsure that yout python3 version is at least Python 3.7!\n\n```\nsudo apt install python3-pip\npip3 install pip3 --upgrade\npip3 install pybuilder ddadevops deprecation\nexport PATH=$PATH:~/.local/bin\n\n# in case of using terraform\npip3 install dda-python-terraform packaging\n\n# in case of using AwsMixin\npip3 install boto3\n\n# in case of using AwsMfaMixin\npip3 install boto3 mfa\n```\n\n# Example Build\n\nlets assume the following project structure\n\n```\nmy-project\n   | -> my-module\n   |       | -> build.py\n   |       | -> some-terraform.tf\n   | -> an-other-module\n   | -> target  (here will the build happen)\n   |       | -> ...\n```\n\n```\nfrom pybuilder.core import task, init\nfrom ddadevops import *\n\nname = \'my-project\'\nMODULE = \'my-module\'\nPROJECT_ROOT_PATH = \'..\'\n\nclass MyBuild(DevopsTerraformBuild):\n    pass\n\n\n@init\ndef initialize(project):\n    project.build_depends_on(\'ddadevops>=0.5.0\')\n    account_name = \'my-aws-account-name\'\n    account_id = \'my-aws-account-id\'\n    stage = \'my stage i.e. dev|test|prod\'\n    additional_vars = {\'var_to_use_insied_terraform\': \'...\'}\n    additional_var_files = [\'variable-\' + account_name + \'-\' + stage + \'.tfvars\']\n    config = create_devops_terraform_build_config(stage, PROJECT_ROOT_PATH,\n                                                  MODULE, additional_vars,\n                                                  additional_tfvar_files=additional_var_files)\n    build = MyBuild(project, config)\n    build.initialize_build_dir()\n\n\n@task\ndef plan(project):\n    build = get_devops_build(project)\n    build.plan()\n\n\n@task\ndef apply(project):\n    build = get_devops_build(project)\n    build.apply()\n\n@task\ndef destroy(project):\n    build = get_devops_build(project)\n    build.destroy()\n\n@task\ndef tf_import(project):\n    build = get_devops_build(project)\n    build.tf_import(\'aws_resource.choosen_name\', \'the_aws_id\')\n```\n\n## Feature aws-backend\n\nWill use a file `backend.dev.live.properties` where dev is the [account-name], live is the  [stage].\n\nthe backend.dev.live.properties file content:\n```\nkey = ".."\nregion = "the aws region"\nprofile = "the profile used for aws"\nbucket = "the s3 bucket name"\nkms_key_id = "the aws key id"\n```\n\nthe build.py file content:\n```\nclass MyBuild(AwsBackendPropertiesMixin, DevopsTerraformBuild):\n    pass\n\n\n@init\ndef initialize(project):\n    project.build_depends_on(\'ddadevops>=1.0\')\n    account_name = \'my-aws-account-name\'\n    account_id = \'my-aws-account-id\'\n    stage = \'my stage i.e. dev|test|prod\'\n    additional_vars = {}\n    config = create_devops_terraform_build_config(stage, PROJECT_ROOT_PATH,\n                                                  MODULE, additional_vars)\n    config = add_aws_backend_properties_mixin_config(config, account_name)\n    build = MyBuild(project, config)\n    build.initialize_build_dir()\n```\n\n## Feature aws-mfa-assume-role\n\nIn order to use aws assume role in combination with the mfa-tool (`pip install mfa`):\n\nthe build.py file content:\n```\nclass MyBuild(class MyBuild(AwsMfaMixin, DevopsTerraformBuild):\n    pass\n\n\n@init\ndef initialize(project):\n    project.build_depends_on(\'ddadevops>=1.0\')\n    account_name = \'my-aws-account-name\'\n    account_id = \'my-aws-account-id\'\n    stage = \'my stage i.e. dev|test|prod\'\n    additional_vars = {}\n    config = create_devops_terraform_build_config(stage, PROJECT_ROOT_PATH,\n                                                  MODULE, additional_vars)\n    config = add_aws_backend_properties_mixin_config(config, account_name)\n    config = add_aws_mfa_mixin_config(config, account_id, \'eu-central-1\',\n                                      mfa_role=\'my_developer_role\',\n                                      mfa_account_prefix=\'company-\',\n                                      mfa_login_account_suffix=\'users_are_defined_here\')\n    build = MyBuild(project, config)\n    build.initialize_build_dir()\n\n@task\ndef access(project):\n    build = get_devops_build(project)\n    build.get_mfa_session()\n```\n\n## Feature DdaDockerBuild\n\nThe docker build supports image building, tagging, testing and login to dockerhost.\nFor bash based builds we support often used script-parts as predefined functions [see install_functions.sh](src/main/resources/docker/image/resources/install_functions.sh).\n\nA full working example: [doc/example/50_docker_module](doc/example/50_docker_module)\n\n## Feature AwsRdsPgMixin\n\nThe AwsRdsPgMixin provides \n* execute_pg_rds_sql - function will optionally resolve dns-c-names for trusted ssl-handshakes\n* alter_db_user_password\n* add_new_user\n* deactivate_user\n\nthe build.py file content:\n```\nclass MyBuild(..., AwsRdsPgMixin):\n    pass\n\n\n@init\ndef initialize(project):\n    project.build_depends_on(\'ddadevops>=1.0\')\n\n    ...\n    config = add_aws_rds_pg_mixin_config(config,\n                                         stage + "-db.bcsimport.kauf." + account_name + ".breuni.de",\n                                         "kauf_bcsimport",\n                                         rds_resolve_dns=True,)\n    build = MyBuild(project, config)\n    build.initialize_build_dir()\n\n@task\ndef rotate_credentials_in(project):\n    build = get_devops_build(project)\n    build.alter_db_user_password(\'/postgres/support\')\n    build.alter_db_user_password(\'/postgres/superuser\')\n    build.add_new_user(\'/postgres/superuser\', \'/postgres/app\', \'pg_group_role\')\n\n\n@task\ndef rotate_credentials_out(project):\n    build = get_devops_build(project)\n    build.deactivate_user(\'/postgres/superuser\', \'old_user_name\')\n```\n\n# Releasing and updating\n## Publish snapshot\n\n1. every push will be published as dev-dependency\n\n## Release\n\n```\nadjust version no in build.py to release version no.\ngit commit -am "release"\ngit tag -am "release" [release version no]\ngit push --follow-tags\nincrease version no in build.py\ngit commit -am "version bump"\ngit push\npip3 install --upgrade --user ddadevops\n```\n\n# License\n\nCopyright © 2021 meissa GmbH\nLicensed under the [Apache License, Version 2.0](LICENSE) (the "License")\n',
         long_description_content_type = 'text/markdown',
         classifiers = [
             'License :: OSI Approved :: Apache Software License',
             'Programming Language :: Python',
             'Programming Language :: Python :: 3',
```

