# Comparing `tmp/hdn-research-environment-2.1.9.tar.gz` & `tmp/hdn-research-environment-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hdn-research-environment-2.1.9.tar", last modified: Mon Jun 19 12:35:22 2023, max compression
+gzip compressed data, was "dist/hdn-research-environment-2.2.0.tar", last modified: Mon Jun 26 17:43:39 2023, max compression
```

## Comparing `hdn-research-environment-2.1.9.tar` & `hdn-research-environment-2.2.0.tar`

### file list

```diff
@@ -1,97 +1,98 @@
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.1.9/LICENSE
--rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.1.9/MANIFEST.in
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.1.9/README.md
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.9/environment/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/environment/api/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/api/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/environment/api/v1/
--rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/api/v1/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/api/v1/auth.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/api/v1/decorators.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/environment/api/v2/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1572 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/api/v2/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      942 2023-05-30 18:52:36.000000 hdn-research-environment-2.1.9/environment/api/v2/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.9/environment/apps.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3175 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.9/environment/constants.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/deserializers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.1.9/environment/entities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      818 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/exceptions.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3711 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.9/environment/forms.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1720 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.9/environment/mailers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.9/environment/managers.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/environment/migrations/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/migrations/0001_initial.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/migrations/0002_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/migrations/0003_cloudidentity_is_workspace_done.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/migrations/0004_auto_20220309_0330.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/migrations/0005_workflow.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/migrations/0006_delete_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/migrations/0007_billingaccountsharinginvite.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/migrations/0008_workflow_workspace_name.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1364 2023-05-31 14:40:16.000000 hdn-research-environment-2.1.9/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.9/environment/migrations/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2518 2023-06-18 19:04:20.000000 hdn-research-environment-2.1.9/environment/models.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    20237 2023-06-19 11:01:13.000000 hdn-research-environment-2.1.9/environment/services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     4545 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.9/environment/signals.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/environment/static/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/environment/static/environment/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/environment/static/environment/css/
--rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.1.9/environment/static/environment/css/create_research_environment.css
--rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.9/environment/static/environment/css/environment-base.css
--rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/static/environment/css/manage_billing_account.css
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/environment/static/environment/js/
--rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.1.9/environment/static/environment/js/cookie.js
--rw-r--r--   0 karolszuster   (501) staff       (20)      291 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.9/environment/static/environment/js/forms.js
--rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/static/environment/js/gpu_disabling.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/static/environment/js/pricing_change.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     2652 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.9/environment/tasks.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/environment/templates/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/environment/templates/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)     6839 2023-06-19 11:34:53.000000 hdn-research-environment-2.1.9/environment/templates/environment/_available_environments_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1419 2023-06-19 12:34:04.000000 hdn-research-environment-2.1.9/environment/templates/environment/_available_projects_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1916 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.9/environment/templates/environment/_billing_accounts_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     3305 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.9/environment/templates/environment/_environment_tabs.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1073 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.9/environment/templates/environment/base_environment_home.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     4417 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.9/environment/templates/environment/create_research_environment.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1149 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.9/environment/templates/environment/create_workspace.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/environment/templates/environment/email/
--rw-r--r--   0 karolszuster   (501) staff       (20)      272 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.9/environment/templates/environment/email/billing_sharing_confirmation.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      351 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.9/environment/templates/environment/email/environment_access_expired.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1163 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.9/environment/templates/environment/identity_provisioning.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     5942 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.9/environment/templates/environment/manage_billing_account.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      562 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.9/environment/templates/environment/manage_shared_billing_invitation.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1649 2023-06-19 11:33:54.000000 hdn-research-environment-2.1.9/environment/templates/environment/research_environments.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/environment/templates/tag/
--rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.9/environment/templates/tag/environment_action_button.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1473 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.9/environment/templates/tag/environment_modal_button.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/environment/templatetags/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.9/environment/templatetags/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3518 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.9/environment/templatetags/action_buttons.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/environment/tests/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.9/environment/tests/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/tests/helpers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/tests/mocks.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/tests/test_decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/tests/test_services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/tests/test_signals.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/tests/test_utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.1.9/environment/tests/test_validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/tests/test_views.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1555 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/urls.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.9/environment/utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.9/environment/validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    14586 2023-06-19 11:01:13.000000 hdn-research-environment-2.1.9/environment/views.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/hdn_research_environment.egg-info/
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/hdn_research_environment.egg-info/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)     3200 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/hdn_research_environment.egg-info/SOURCES.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/hdn_research_environment.egg-info/dependency_links.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/hdn_research_environment.egg-info/requires.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/hdn_research_environment.egg-info/top_level.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.1.9/pyproject.toml
--rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-06-19 12:35:22.000000 hdn-research-environment-2.1.9/setup.cfg
--rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.1.9/setup.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.2.0/LICENSE
+-rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.2.0/MANIFEST.in
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.2.0/README.md
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.2.0/environment/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/api/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/api/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/api/v1/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/api/v1/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/api/v1/auth.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/api/v1/decorators.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/api/v2/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1726 2023-06-26 17:42:34.000000 hdn-research-environment-2.2.0/environment/api/v2/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      942 2023-05-30 18:52:36.000000 hdn-research-environment-2.2.0/environment/api/v2/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.2.0/environment/apps.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3175 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/constants.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/deserializers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.2.0/environment/entities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      869 2023-06-26 17:42:34.000000 hdn-research-environment-2.2.0/environment/exceptions.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3711 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/forms.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1720 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/mailers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.2.0/environment/managers.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/migrations/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/migrations/0001_initial.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/migrations/0002_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/migrations/0003_cloudidentity_is_workspace_done.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/migrations/0004_auto_20220309_0330.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/migrations/0005_workflow.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/migrations/0006_delete_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/migrations/0007_billingaccountsharinginvite.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/migrations/0008_workflow_workspace_name.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1364 2023-05-31 14:40:16.000000 hdn-research-environment-2.2.0/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.2.0/environment/migrations/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2518 2023-06-18 19:04:20.000000 hdn-research-environment-2.2.0/environment/models.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    20869 2023-06-26 17:42:34.000000 hdn-research-environment-2.2.0/environment/services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4545 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/signals.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/static/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/static/environment/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/static/environment/css/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.2.0/environment/static/environment/css/create_research_environment.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.2.0/environment/static/environment/css/environment-base.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/static/environment/css/manage_billing_account.css
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/static/environment/js/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.2.0/environment/static/environment/js/cookie.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)      291 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/static/environment/js/forms.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/static/environment/js/gpu_disabling.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/static/environment/js/pricing_change.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2652 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/tasks.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/templates/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/templates/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     6560 2023-06-26 17:42:34.000000 hdn-research-environment-2.2.0/environment/templates/environment/_available_environments_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1419 2023-06-19 12:34:04.000000 hdn-research-environment-2.2.0/environment/templates/environment/_available_projects_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1916 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/templates/environment/_billing_accounts_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3297 2023-06-26 17:42:34.000000 hdn-research-environment-2.2.0/environment/templates/environment/_environment_tabs.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1073 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/templates/environment/base_environment_home.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3863 2023-06-26 17:42:41.000000 hdn-research-environment-2.2.0/environment/templates/environment/create_research_environment.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1644 2023-06-26 17:42:41.000000 hdn-research-environment-2.2.0/environment/templates/environment/create_workspace.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/templates/environment/email/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      272 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/templates/environment/email/billing_sharing_confirmation.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      351 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/templates/environment/email/environment_access_expired.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1163 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/templates/environment/identity_provisioning.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5942 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/templates/environment/manage_billing_account.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      562 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/templates/environment/manage_shared_billing_invitation.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1649 2023-06-19 11:33:54.000000 hdn-research-environment-2.2.0/environment/templates/environment/research_environments.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/templates/tag/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.2.0/environment/templates/tag/environment_action_button.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1473 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/templates/tag/environment_modal_button.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1957 2023-06-26 17:42:34.000000 hdn-research-environment-2.2.0/environment/templates/tag/workspace_destroy_modal_button.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/templatetags/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.2.0/environment/templatetags/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4409 2023-06-26 17:42:34.000000 hdn-research-environment-2.2.0/environment/templatetags/action_buttons.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/tests/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.2.0/environment/tests/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/tests/helpers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/tests/mocks.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/tests/test_decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/tests/test_services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/tests/test_signals.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/tests/test_utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.2.0/environment/tests/test_validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/tests/test_views.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1634 2023-06-26 17:42:34.000000 hdn-research-environment-2.2.0/environment/urls.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.2.0/environment/validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    15553 2023-06-26 17:42:41.000000 hdn-research-environment-2.2.0/environment/views.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/hdn_research_environment.egg-info/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/hdn_research_environment.egg-info/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3262 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/hdn_research_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/hdn_research_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/hdn_research_environment.egg-info/requires.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/hdn_research_environment.egg-info/top_level.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.2.0/pyproject.toml
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/setup.cfg
+-rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.2.0/setup.py
```

### Comparing `hdn-research-environment-2.1.9/LICENSE` & `hdn-research-environment-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/PKG-INFO` & `hdn-research-environment-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 2.1.9
+Version: 2.2.0
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-2.1.9/environment/api/v1/__init__.py` & `hdn-research-environment-2.2.0/environment/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/api/v1/auth.py` & `hdn-research-environment-2.2.0/environment/api/v1/auth.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/api/v1/decorators.py` & `hdn-research-environment-2.2.0/environment/api/v1/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/api/v2/__init__.py` & `hdn-research-environment-2.2.0/environment/api/v2/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,7 +58,12 @@
 def create_workspace(email: str, billing_account_id: str, region: str) -> Request:
     json = {
         "email": email,
         "billing_account_id": billing_account_id,
         "region": region,
     }
     return Request("POST", url="/workspace/create", json=json)
+
+
+@api_request
+def delete_workspace(email: str, gcp_project_id: str) -> Request:
+    return Request("DELETE", url=f"/workspace/{email}/{gcp_project_id}")
```

### Comparing `hdn-research-environment-2.1.9/environment/api/v2/decorators.py` & `hdn-research-environment-2.2.0/environment/api/v2/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/constants.py` & `hdn-research-environment-2.2.0/environment/constants.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/decorators.py` & `hdn-research-environment-2.2.0/environment/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/deserializers.py` & `hdn-research-environment-2.2.0/environment/deserializers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/entities.py` & `hdn-research-environment-2.2.0/environment/entities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/exceptions.py` & `hdn-research-environment-2.2.0/environment/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,7 +52,11 @@
 
 class GetWorkspacesListFailed(Exception):
     pass
 
 
 class CreateWorkspaceFailed(Exception):
     pass
+
+
+class DeleteWorkspaceFailed(Exception):
+    pass
```

### Comparing `hdn-research-environment-2.1.9/environment/forms.py` & `hdn-research-environment-2.2.0/environment/forms.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/mailers.py` & `hdn-research-environment-2.2.0/environment/mailers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/migrations/0001_initial.py` & `hdn-research-environment-2.2.0/environment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/migrations/0002_billingsetup.py` & `hdn-research-environment-2.2.0/environment/migrations/0002_billingsetup.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/migrations/0005_workflow.py` & `hdn-research-environment-2.2.0/environment/migrations/0005_workflow.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/migrations/0007_billingaccountsharinginvite.py` & `hdn-research-environment-2.2.0/environment/migrations/0007_billingaccountsharinginvite.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py` & `hdn-research-environment-2.2.0/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/models.py` & `hdn-research-environment-2.2.0/environment/models.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/services.py` & `hdn-research-environment-2.2.0/environment/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Tuple, Iterable, Optional, Dict
 from collections import defaultdict
 
-from django.db.models import Model
+from django.db.models import Model, Q
 from django.contrib.sites.shortcuts import get_current_site
 from django.apps import apps
 from google.cloud.workflows import executions_v1beta
 from google.cloud.workflows.executions_v1beta.types import executions
 
 import environment.constants as constants
 import environment.mailers as mailers
@@ -22,14 +22,15 @@
     BillingAccessRevokationFailed,
     EnvironmentCreationFailed,
     GetAvailableEnvironmentsFailed,
     GetWorkspaceDetailsFailed,
     GetBillingAccountsListFailed,
     GetWorkspacesListFailed,
     CreateWorkspaceFailed,
+    DeleteWorkspaceFailed,
 )
 from environment.deserializers import (
     deserialize_research_environments,
     deserialize_workspace_details,
     deserialize_workspaces,
 )
 from environment.entities import (
@@ -175,22 +176,41 @@
         email=user.cloud_identity.email,
         billing_account_id=billing_account_id,
         region=region,
     )
     if not response.ok:
         error_message = response.json()["error"]
         raise CreateWorkspaceFailed(error_message)
+
     execution_resource_name = response.json()["execution-name"]
     persist_workflow(
         user=user,
         execution_resource_name=execution_resource_name,
         type=Workflow.WORKSPACE_CREATE,
     )
 
 
+def delete_workspace(user: User, gcp_project_id: str):
+    response = api_v2.delete_workspace(
+        email=user.cloud_identity.email,
+        gcp_project_id=gcp_project_id,
+    )
+    if not response.ok:
+        error_message = response.json()["error"]
+        raise DeleteWorkspaceFailed(error_message)
+
+    execution_resource_name = response.json()["execution-name"]
+    persist_workflow(
+        user=user,
+        execution_resource_name=execution_resource_name,
+        type=Workflow.WORKSPACE_DESTROY,
+        workspace_name=gcp_project_id,
+    )
+
+
 def _create_workbench_kwargs(
     user: User,
     project: PublishedProject,
     workspace_name: str,
     instance_type: str,
     environment_type: str,
     persistent_disk: int,
@@ -356,17 +376,18 @@
     return [
         (environment, project, workflows)
         for project, environment, workflows in project_environment_workflow_triplets
         if environment is None and workflows.exists()
     ]
 
 
-def get_workspace_creation_workflows(user: User) -> Iterable[Workflow]:
+def get_workspace_workflows(user: User) -> Iterable[Workflow]:
     return Workflow.objects.filter(
-        user=user, type=Workflow.WORKSPACE_CREATE, status=Workflow.INPROGRESS
+        (Q(type=Workflow.WORKSPACE_CREATE) | Q(type=Workflow.WORKSPACE_DESTROY))
+        & Q(user=user, status=Workflow.INPROGRESS)
     )
 
 
 def get_environment_project_pairs_with_expired_access(
     user: User,
 ) -> Iterable[Tuple[ResearchEnvironment, PublishedProject]]:
     all_environment_project_pairs = get_environments_with_projects(user)
```

### Comparing `hdn-research-environment-2.1.9/environment/signals.py` & `hdn-research-environment-2.2.0/environment/signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/static/environment/css/environment-base.css` & `hdn-research-environment-2.2.0/environment/static/environment/css/environment-base.css`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/static/environment/js/cookie.js` & `hdn-research-environment-2.2.0/environment/static/environment/js/cookie.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/static/environment/js/gpu_disabling.js` & `hdn-research-environment-2.2.0/environment/static/environment/js/gpu_disabling.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/static/environment/js/pricing_change.js` & `hdn-research-environment-2.2.0/environment/static/environment/js/pricing_change.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/tasks.py` & `hdn-research-environment-2.2.0/environment/tasks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/templates/environment/_available_environments_list.html` & `hdn-research-environment-2.2.0/environment/templates/environment/_available_environments_list.html`

 * *Files 16% similar despite different names*

```diff
@@ -3,121 +3,124 @@
 {% if recent_workflow %}
     {% if recent_workflow_failed %}
     <div class="alert alert-danger" role="alert">
             {{ recent_workflow.get_type_display }}
             {% if recent_workflow.project %}
                 {{ recent_workflow.project }}
             {% endif %}
-            failed! {{ workflow_finished_message }}
+            failed! {{ workflow_finished_message|default_if_none:"Try again later." }}
         </div>
     {% elif recent_workflow_succeeded %}
         <div class="alert alert-success" role="alert">
             {{ recent_workflow.get_type_display }}
             {% if recent_workflow.project %}
                 {{ recent_workflow.project }}
             {% endif %}
-            finished! {{ workflow_finished_message }}
+            finished! {{ workflow_finished_message|default_if_none:"" }}
         </div>
     {% endif %}
 {% endif %}
 
 <div class="d-flex flex-column align-items-end px-4 mb-3">
     <a class="btn btn-primary btn-sm" href="{% url 'create_workspace' %}">
       + Workspace
     </a>
 </div>
 
 <div id="accordion">
-    {% for workflow in workspace_creation_workflows %}
+    {% for workflow in workspace_workflows %}
         <div class="card">
             <div class="card-header""{{ heading }}">
                 <div>
                     <h6 class="mb-0">
-                        <div class="d-flex align-items-center">
-                            <div style="margin-right: 1.5rem">
-                                Provisioning
+                        <div class="d-flex align-items-center justify-content-between">
+                            <div>
+                                {% if workflow.type == 5 %}
+                                    Creating Workspace...
+                                {% else %}
+                                    Destroying {{ workflow.workspace_name }}...
+                                {% endif %}
                             </div>
-                            <div class="loader" style="font-size: 3.5px; margin: 0;">Loading...</div>
+                            <div class="loader" style="font-size: 3.5px; margin: 0; margin-right: 0.3rem;">Loading...</div>
                         </div>
                     </h6>
                 </div>
             </div>
         </div>
     {% endfor %}
 
     {% for workspace, environments_project_workflow_triplets in workspace_project_environment_workflow_triplets_dict.items %}
-        {% with collapse="collapse-"|add:workspace.gcp_project_id heading="heading-"|add:workspace.gcp_project_id %}
-            <div class="card">
-                <div class="card-header py-3" id="{{ heading }}">
-                    <div data-toggle="collapse" data-target="#{{ collapse }}" aria-expanded="true" aria-controls="{{ collapse }}">
+        <div class="card">
+            <div class="card-header py-3" id="{{ heading }}">
+                <div class="d-flex justify-content-between">
+                    <div>
                         <h6 class="mb-0">
                             {{ workspace.gcp_project_id }}
                         </h6>
                         <small>
                             <span class="d-inline font-weight-bold" style="padding-top: 0.375rem;">
                                 Billing Account:
                             </span>
                             <span class="d-inline font-weight-normal">
                                 {{ workspace.billing_name }}
                             </span>
                         </small>
                     </div>
+                    {% workspace_destroy_modal_button workspace=workspace environments_project_workflow_triplets=environments_project_workflow_triplets %}
                 </div>
+            </div>
 
-                <div id="{{ collapse }}" class="collapse show" aria-labelledby="{{ heading }}" data-parent="#accordion">
-                    <div class="card-body">
-                        {% if environments_project_workflow_triplets|length %}
-                            <ul class="list-group list-group-flush">
-                                {% for environment, project, workflows in environments_project_workflow_triplets %}
-                                    <li class="list-group-item">
-                                        <div class="row">
-                                            <div class="col-md-3">
-                                                <a href="{% url 'published_project' project.slug project.version %}" target="_blank">
-                                                    {{ project }}
-                                                </a>
-                                            </div>
-                                            <div class="col-md-3">
-                                                <small>
-                                                    <i>Environment type:</i> {{ environment.type.value|capfirst }}<br>
-                                                    <i>Instance type:</i> {{ environment.instance_type.value }}<br>
-                                                    <i>Region:</i> {{ environment.region.value }}
-                                                </small>
-                                            </div>
-                                            <div class="col-md-2">
-                                                {% if workflows.exists %}
-                                                    {{ workflows.first.get_type_display }}
+            <div class="card-body">
+                {% if environments_project_workflow_triplets|length %}
+                    <ul class="list-group list-group-flush">
+                        {% for environment, project, workflows in environments_project_workflow_triplets %}
+                            <li class="list-group-item">
+                                <div class="row">
+                                    <div class="col-md-3">
+                                        <a href="{% url 'published_project' project.slug project.version %}" target="_blank">
+                                            {{ project }}
+                                        </a>
+                                    </div>
+                                    <div class="col-md-3">
+                                        <small>
+                                            <i>Environment type:</i> {{ environment.type.value|capfirst }}<br>
+                                            <i>Instance type:</i> {{ environment.instance_type.value }}<br>
+                                            <i>Region:</i> {{ environment.region.value }}
+                                        </small>
+                                    </div>
+                                    <div class="col-md-2">
+                                        {% if workflows.exists %}
+                                            {{ workflows.first.get_type_display }}
+                                        {% else %}
+                                            {{ environment.status.value|capfirst }}
+                                        {% endif %}
+                                    </div>
+                                    <div class="col-md-4">
+                                        <div class="d-flex flex-wrap">
+                                            {% if workflows.exists %}
+                                                <div class="loader" style="margin: 18px; font-size: 5px">Loading...</div>
+                                            {% elif environment.is_running or environment.is_paused %}
+                                                {% if environment.is_running %}
+                                                    <a href="{{ environment.url }}" target="_blank" class="btn btn-sm btn-success m-1">Open</a>
+                                                    {% environment_modal_button environment=environment project=project button_type="modal_pause" %}
                                                 {% else %}
-                                                    {{ environment.status.value|capfirst }}
+                                                    {% environment_modal_button environment=environment project=project button_type="modal_start" %}
                                                 {% endif %}
-                                            </div>
-                                            <div class="col-md-4">
-                                                <div class="d-flex flex-wrap">
-                                                    {% if workflows.exists %}
-                                                        <div class="loader" style="margin: 18px; font-size: 5px">Loading...</div>
-                                                    {% elif environment.is_running or environment.is_paused %}
-                                                        {% if environment.is_running %}
-                                                            <a href="{{ environment.url }}" target="_blank" class="btn btn-sm btn-success m-1">Open</a>
-                                                            {% environment_modal_button environment=environment project=project button_type="modal_pause" %}
-                                                        {% else %}
-                                                            {% environment_modal_button environment=environment project=project button_type="modal_start" %}
-                                                        {% endif %}
-                                                        {% environment_modal_button environment=environment project=project button_type="modal_instance" %}
-                                                        {% environment_modal_button environment=environment project=project button_type="modal_destroy" %}
-                                                    {% endif %}
-                                                </div>
-                                            </div>
+                                                {% environment_modal_button environment=environment project=project button_type="modal_instance" %}
+                                                {% environment_modal_button environment=environment project=project button_type="modal_destroy" %}
+                                            {% endif %}
                                         </div>
-                                    </li>
-                                {% endfor %}
-                            </ul>
-                        {% else %}
-                            <div class="text-center">
-                                You don't have any workbenches in this workspace.<br>
-                                Create one in the "Projects" tab.
-                            </div>
-                        {% endif %}
+                                    </div>
+                                </div>
+                            </li>
+                        {% endfor %}
+                    </ul>
+                {% else %}
+                    <div class="text-center">
+                        You don't have any workbenches in this workspace.<br>
+                        Create one in the "Projects" tab.
                     </div>
-                </div>
+                {% endif %}
             </div>
-        {% endwith %}
+        </div>
     {% endfor %}
 </div>
```

#### html2text {}

```diff
@@ -1,28 +1,30 @@
 {% load action_buttons %} {% if recent_workflow %} {% if recent_workflow_failed
 %}
 {{ recent_workflow.get_type_display }} {% if recent_workflow.project %} {
-{ recent_workflow.project }} {% endif %} failed! {{ workflow_finished_message
-}}
+{ recent_workflow.project }} {% endif %} failed! {
+{ workflow_finished_message|default_if_none:"Try again later." }}
 {% elif recent_workflow_succeeded %}
 {{ recent_workflow.get_type_display }} {% if recent_workflow.project %} {
-{ recent_workflow.project }} {% endif %} finished! {{ workflow_finished_message
-}}
+{ recent_workflow.project }} {% endif %} finished! {
+{ workflow_finished_message|default_if_none:"" }}
 {% endif %} {% endif %}
 +_Workspace
-{% for workflow in workspace_creation_workflows %}
+{% for workflow in workspace_workflows %}
 {{ heading }}">
-Provisioning
+{% if workflow.type == 5 %} Creating Workspace... {% else %} Destroying {
+{ workflow.workspace_name }}... {% endif %}
 Loading...
 {% endfor %} {% for workspace, environments_project_workflow_triplets in
-workspace_project_environment_workflow_triplets_dict.items %} {% with
-collapse="collapse-"|add:workspace.gcp_project_id heading="heading-"|add:
-workspace.gcp_project_id %}
+workspace_project_environment_workflow_triplets_dict.items %}
 * {{ workspace.gcp_project_id }} *
  Billing Account:   {{ workspace.billing_name }}
+{% workspace_destroy_modal_button workspace=workspace
+environments_project_workflow_triplets=environments_project_workflow_triplets
+%}
 {% if environments_project_workflow_triplets|length %}
     * {% for environment, project, workflows in
       environments_project_workflow_triplets %}
     * {{_project_}}
       Environment type: {{ environment.type.value|capfirst }}
       Instance type: {{ environment.instance_type.value }}
       Region: {{ environment.region.value }}
@@ -40,8 +42,8 @@
       environment=environment project=project button_type="modal_destroy" %} {%
       endif %}
     * {% endfor %}
 {% else %}
 You don't have any workbenches in this workspace.
 Create one in the "Projects" tab.
 {% endif %}
-{% endwith %} {% endfor %}
+{% endfor %}
```

### Comparing `hdn-research-environment-2.1.9/environment/templates/environment/_available_projects_list.html` & `hdn-research-environment-2.2.0/environment/templates/environment/_available_projects_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/templates/environment/_billing_accounts_list.html` & `hdn-research-environment-2.2.0/environment/templates/environment/_billing_accounts_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/templates/environment/_environment_tabs.html` & `hdn-research-environment-2.2.0/environment/templates/environment/_environment_tabs.html`

 * *Files 2% similar despite different names*

```diff
@@ -104,11 +104,11 @@
 
     {% for environment, project, workflows in environment_project_workflow_triplets %}
         {% for workflow in workflows %}
             scheduleExecutionPolling("{{ workflow.execution_resource_name }}", true);
         {% endfor %}
     {% endfor %}
 
-    {% for workflow in workspace_creation_workflows %}
+    {% for workflow in workspace_workflows %}
         scheduleExecutionPolling("{{ workflow.execution_resource_name }}", true);
     {% endfor %}
-</script>
+</script>
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
     * Running_Environments__{{_environment_project_workflow_triplets|length_}}_
     * Available_Projects__{
       {_available_project_environment_workflow_triplets|length_}}_
     * Billing
 {% include "environment/_available_environments_list.html" %}
 {% include "environment/_available_projects_list.html" %}
 {% include "environment/_billing_accounts_list.html" %}
+
```

### Comparing `hdn-research-environment-2.1.9/environment/templates/environment/base_environment_home.html` & `hdn-research-environment-2.2.0/environment/templates/environment/base_environment_home.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/templates/environment/create_research_environment.html` & `hdn-research-environment-2.2.0/environment/templates/environment/create_research_environment.html`

 * *Files 5% similar despite different names*

```diff
@@ -25,34 +25,21 @@
     </h1>
     <div class="container-body">
       <div class="card" style="width: 36rem;">
         <div class="card-body">
           <h3 class="card-title">
               Project: <span class="font-italic">{{ project.title }}</span>
           </h3>
-
-          {% if exceeded_quotas|length > 0 %}
-              <div>
-                  <p style="color:red">You have exceeded the following quotas:</p>
-                  <ul>
-                      {% for quota in exceeded_quotas %}
-                          <li>{{ quota }}</li>
-                      {% endfor %}
-                  </ul>
-                  <a href="{% url 'research_environments' %}"><button class="btn btn-primary">Return</button></a>
-              </div>
-          {% else %}
-              <form class="single-submit-form" action="{% url 'create_research_environment' project_slug=project.slug project_version=project.version %}" method="post" style="width: 24rem;">
-                  {% csrf_token %}
-                  {{ form }}
-                  <button class="btn btn-primary mt-3" type="submit">
-                      Create environment
-                  </button>
-              </form>
-          {% endif %}
+          <form class="single-submit-form" action="{% url 'create_research_environment' project_slug=project.slug project_version=project.version %}" method="post" style="width: 24rem;">
+            {% csrf_token %}
+            {{ form }}
+            <button class="btn btn-primary mt-3" type="submit">
+              Create environment
+            </button>
+          </form>
         </div>
       </div>
       <div class="card billing-information">
         <div class="card-body">
           <h3 class="card-title">
             Projected Costs
           </h3>
```

#### html2text {}

```diff
@@ -3,23 +3,15 @@
 %}
  {% endblock %} {% block local_css %}
 
  {% endblock %} {% block content %}
 {% include "message_snippet.html" %}
 ****** Create Research Environment ******
 **** Project: {{ project.title }} ****
-{% if exceeded_quotas|length > 0 %}
-You have exceeded the following quotas:
-    * {% for quota in exceeded_quotas %}
-    * {{ quota }}
-    * {% endfor %}
-Return
-{% else %}
 {% csrf_token %} {{ form }}  Create environment
-{% endif %}
 **** Projected Costs ****
 The currently selected configuration will cost approximately:
 ** Instance Costs **
 {% for region_name, region_instances in instance_projected_costs.items %} {%
 for resource, cost in region_instances %}
 Instance: {{ cost }} $/hour
 {% endfor %} {% endfor %}
```

### Comparing `hdn-research-environment-2.1.9/environment/templates/environment/create_workspace.html` & `hdn-research-environment-2.2.0/environment/templates/environment/create_workspace.html`

 * *Files 11% similar despite different names*

```diff
@@ -20,22 +20,34 @@
   {% include "message_snippet.html" %}
     <h1 class="mb-4">
       Create Workspace
     </h1>
     <div class="container-body">
       <div class="card" style="width: 36rem;">
         <div class="card-body">
-          <form class="single-submit-form" action="{% url 'create_workspace' %}" method="post" style="width: 24rem;">
-            {% csrf_token %}
-            {{ form }}
-            <button
-              class="btn btn-primary mt-3"
-              type="submit"
-            >
-                Create workspace
-            </button>
-          </form>
+          {% if exceeded_quotas|length > 0 %}
+            <div>
+              <p style="color:red">You have exceeded the following quotas:</p>
+              <ul>
+                {% for quota in exceeded_quotas %}
+                    <li>{{ quota }}</li>
+                {% endfor %}
+              </ul>
+              <a href="{% url 'research_environments' %}"><button class="btn btn-primary">Return</button></a>
+            </div>
+          {% else %}
+            <form class="single-submit-form" action="{% url 'create_workspace' %}" method="post" style="width: 24rem;">
+              {% csrf_token %}
+              {{ form }}
+              <button
+                class="btn btn-primary mt-3"
+                type="submit"
+              >
+                  Create workspace
+              </button>
+            </form>
+          {% endif %}
         </div>
       </div>
     </div>
 </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -2,9 +2,17 @@
 block title %}Create Research Environment{% endblock %} {% block local_js_top
 %}
  {% endblock %} {% block local_css %}
 
  {% endblock %} {% block content %}
 {% include "message_snippet.html" %}
 ****** Create Workspace ******
+{% if exceeded_quotas|length > 0 %}
+You have exceeded the following quotas:
+    * {% for quota in exceeded_quotas %}
+    * {{ quota }}
+    * {% endfor %}
+Return
+{% else %}
 {% csrf_token %} {{ form }}  Create workspace
+{% endif %}
 {% endblock %}
```

### Comparing `hdn-research-environment-2.1.9/environment/templates/environment/identity_provisioning.html` & `hdn-research-environment-2.2.0/environment/templates/environment/identity_provisioning.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/templates/environment/manage_billing_account.html` & `hdn-research-environment-2.2.0/environment/templates/environment/manage_billing_account.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/templates/environment/manage_shared_billing_invitation.html` & `hdn-research-environment-2.2.0/environment/templates/environment/manage_shared_billing_invitation.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/templates/environment/research_environments.html` & `hdn-research-environment-2.2.0/environment/templates/environment/research_environments.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/templates/tag/environment_modal_button.html` & `hdn-research-environment-2.2.0/environment/templates/tag/environment_modal_button.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/templatetags/action_buttons.py` & `hdn-research-environment-2.2.0/environment/templatetags/action_buttons.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import json
+from typing import Iterable, Tuple
 
 from django import template
 from django.urls import reverse
 from django.db.models import Model
 
-from environment.entities import ResearchEnvironment
+from environment.entities import ResearchEnvironment, ResearchWorkspace
 from environment.constants import INSTANCE_TYPE_SPECIFICATION
+from environment.models import Workflow
 
 
 PublishedProject = Model
 
 
 register = template.Library()
 
@@ -112,7 +114,28 @@
         "button_text": data["button_text"],
         "button_type": button_type,
         "url": reverse(data["url_name"]),
         "http_method": data["http_method"],
         "request_data": json.dumps(request_data),
     }
     return result_data
+
+
+@register.inclusion_tag("tag/workspace_destroy_modal_button.html")
+def workspace_destroy_modal_button(
+    workspace: ResearchWorkspace,
+    environments_project_workflow_triplets: Iterable[
+        Tuple[ResearchEnvironment, PublishedProject, Iterable[Workflow]]
+    ],
+) -> dict:
+    print(environments_project_workflow_triplets)
+    request_data = {"gcp_project_id": workspace.gcp_project_id}
+    result_data = {
+        "workspace": workspace,
+        "modal_id": f"workspace-delete-{workspace.gcp_project_id}",
+        "button_type": "workspace_delete",
+        "request_url": reverse("delete_workspace"),
+        "request_method": "DELETE",
+        "request_data": json.dumps(request_data),
+        "disabled": len(environments_project_workflow_triplets) > 0,
+    }
+    return result_data
```

### Comparing `hdn-research-environment-2.1.9/environment/tests/helpers.py` & `hdn-research-environment-2.2.0/environment/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/tests/mocks.py` & `hdn-research-environment-2.2.0/environment/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/tests/test_decorators.py` & `hdn-research-environment-2.2.0/environment/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/tests/test_services.py` & `hdn-research-environment-2.2.0/environment/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/tests/test_signals.py` & `hdn-research-environment-2.2.0/environment/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/tests/test_utilities.py` & `hdn-research-environment-2.2.0/environment/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/tests/test_validators.py` & `hdn-research-environment-2.2.0/environment/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/tests/test_views.py` & `hdn-research-environment-2.2.0/environment/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/urls.py` & `hdn-research-environment-2.2.0/environment/urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,8 +48,9 @@
     ),
     path(
         "execution/check-status",
         views.check_execution_status,
         name="check_execution_status",
     ),
     path("workspace/create", views.create_workspace, name="create_workspace"),
+    path("workspace/delete", views.delete_workspace, name="delete_workspace"),
 ]
```

### Comparing `hdn-research-environment-2.1.9/environment/utilities.py` & `hdn-research-environment-2.2.0/environment/utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.9/environment/views.py` & `hdn-research-environment-2.2.0/environment/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,16 +64,18 @@
         billing_accounts_list_future = executor.submit(
             services.get_billing_accounts_list, request.user
         )
 
     workspaces_list = workspaces_list_future.result()
     billing_accounts_list = billing_accounts_list_future.result()
 
-    environment_project_workflow_triplets = services.get_environments_with_projects(user=request.user)
-    workspace_creation_workflows = services.get_workspace_creation_workflows(user=request.user)
+    environment_project_workflow_triplets = services.get_environments_with_projects(
+        user=request.user
+    )
+    workspace_workflows = services.get_workspace_workflows(user=request.user)
 
     environments = map(lambda pair: pair[0], environment_project_workflow_triplets)
     available_project_environment_workflow_triplets = (
         services.get_available_projects_with_environments(
             request.user,
             environments,
         )
@@ -91,19 +93,30 @@
         services.sort_environments_per_workspace(
             environment_projects_pairs_with_creating,
             workspaces_list,
             billing_accounts_list,
         )
     )
 
+    inprogress_workspaces = [
+        workflow.workspace_name
+        for workflow in workspace_workflows
+        if workflow.workspace_name
+    ]
+    triplets_without_inprogress_workspaces = {
+        workspace: workbenches
+        for workspace, workbenches in sorted_environments_project_workflow_triplets_dict.items()
+        if workspace.gcp_project_id not in inprogress_workspaces
+    }
+
     context = {
         "available_project_environment_workflow_triplets": available_project_environment_workflow_triplets,
         "environment_project_workflow_triplets": environment_projects_pairs_with_creating,
-        "workspace_project_environment_workflow_triplets_dict": sorted_environments_project_workflow_triplets_dict,
-        "workspace_creation_workflows": workspace_creation_workflows,
+        "workspace_project_environment_workflow_triplets_dict": triplets_without_inprogress_workspaces,
+        "workspace_workflows": workspace_workflows,
         "billing_accounts_list": billing_accounts_list,
     }
 
     return render(
         request,
         "environment/research_environments.html",
         context,
@@ -117,23 +130,25 @@
     with concurrent.futures.ThreadPoolExecutor() as executor:
         workspaces_list_future = executor.submit(
             services.get_workspaces_list, request.user
         )
         billing_accounts_list_future = executor.submit(
             services.get_billing_accounts_list, request.user
         )
-        workspace_creation_workflows_future = executor.submit(
-            services.get_workspace_creation_workflows, request.user
+        workspace_workflows_future = executor.submit(
+            services.get_workspace_workflows, request.user
         )
 
     workspaces_list = workspaces_list_future.result()
     billing_accounts_list = billing_accounts_list_future.result()
-    workspace_creation_workflows = workspace_creation_workflows_future.result()
+    workspace_workflows = workspace_workflows_future.result()
 
-    environment_project_workflow_triplets = services.get_environments_with_projects(user=request.user)
+    environment_project_workflow_triplets = services.get_environments_with_projects(
+        user=request.user
+    )
 
     environments = map(lambda pair: pair[0], environment_project_workflow_triplets)
     available_project_environment_workflow_triplets = (
         services.get_available_projects_with_environments(
             request.user,
             environments,
         )
@@ -151,30 +166,43 @@
         services.sort_environments_per_workspace(
             environment_projects_pairs_with_creating,
             workspaces_list,
             billing_accounts_list,
         )
     )
 
+    inprogress_workspaces = [
+        workflow.workspace_name
+        for workflow in workspace_workflows
+        if workflow.workspace_name
+    ]
+    triplets_without_inprogress_workspaces = {
+        workspace: workbenches
+        for workspace, workbenches in sorted_environments_project_workflow_triplets_dict.items()
+        if workspace.gcp_project_id not in inprogress_workspaces
+    }
+
     context = {
         "available_project_environment_workflow_triplets": available_project_environment_workflow_triplets,
         "environment_project_workflow_triplets": environment_projects_pairs_with_creating,
-        "workspace_project_environment_workflow_triplets_dict": sorted_environments_project_workflow_triplets_dict,
-        "workspace_creation_workflows": workspace_creation_workflows,
+        "workspace_project_environment_workflow_triplets_dict": triplets_without_inprogress_workspaces,
+        "workspace_workflows": workspace_workflows,
         "billing_accounts_list": billing_accounts_list,
     }
 
     execution_resource_name = request.GET.get("execution_resource_name")
     if execution_resource_name:
         workflow = Workflow.objects.get(execution_resource_name=execution_resource_name)
         workflow_state_context = {
             "recent_workflow": workflow,
             "recent_workflow_failed": workflow.status == Workflow.FAILED,
             "recent_workflow_succeeded": workflow.status == Workflow.SUCCESS,
-            "workflow_finished_message": services.workflow_finished_message(workflow=workflow)
+            "workflow_finished_message": services.workflow_finished_message(
+                workflow=workflow
+            ),
         }
         context = {**context, **workflow_state_context}
 
     return render(
         request,
         "environment/_environment_tabs.html",
         context,
@@ -245,15 +273,14 @@
                 )
     else:
         form = CreateResearchEnvironmentForm(workspace_list=workspaces_list)
 
     context = {
         "form": form,
         "project": project,
-        "exceeded_quotas": [],
         "instance_projected_costs": constants.INSTANCE_PROJECTED_COSTS,
         "gpu_projected_costs": constants.GPU_PROJECTED_COSTS,
         "data_storage_projected_costs": constants.DATA_STORAGE_PROJECTED_COSTS,
     }
     return render(request, "environment/create_research_environment.html", context)
 
 
@@ -381,14 +408,26 @@
         workbench_id=data["workbench_id"],
         region=Region(data["region"]),
         gcp_project_id=data["gcp_project_id"],
     )
     return JsonResponse({})
 
 
+@require_DELETE
+@login_required
+@cloud_identity_required
+def delete_workspace(request):
+    data = json.loads(request.body)
+    services.delete_workspace(
+        user=request.user,
+        gcp_project_id=data["gcp_project_id"],
+    )
+    return JsonResponse({})
+
+
 @require_GET
 @login_required
 @cloud_identity_required
 def check_execution_status(request):
     execution_resource_name = request.GET["execution_resource_name"]
     execution_state = services.get_execution_state(
         execution_resource_name=execution_resource_name
```

### Comparing `hdn-research-environment-2.1.9/hdn_research_environment.egg-info/PKG-INFO` & `hdn-research-environment-2.2.0/hdn_research_environment.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 2.1.9
+Version: 2.2.0
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-2.1.9/hdn_research_environment.egg-info/SOURCES.txt` & `hdn-research-environment-2.2.0/hdn_research_environment.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 environment/templates/environment/manage_billing_account.html
 environment/templates/environment/manage_shared_billing_invitation.html
 environment/templates/environment/research_environments.html
 environment/templates/environment/email/billing_sharing_confirmation.html
 environment/templates/environment/email/environment_access_expired.html
 environment/templates/tag/environment_action_button.html
 environment/templates/tag/environment_modal_button.html
+environment/templates/tag/workspace_destroy_modal_button.html
 environment/templatetags/__init__.py
 environment/templatetags/action_buttons.py
 environment/tests/__init__.py
 environment/tests/helpers.py
 environment/tests/mocks.py
 environment/tests/test_decorators.py
 environment/tests/test_services.py
```

### Comparing `hdn-research-environment-2.1.9/setup.cfg` & `hdn-research-environment-2.2.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hdn-research-environment
-version = 2.1.9
+version = 2.2.0
 description = A Django app for supporting cloud-native research environments
 long_description = file: README.rst
 url = https://www.healthdatanexus.ai/
 author = Your Name
 author_email = yourname@example.com
 license = BSD-3-Clause  # Example license
 classifiers =
```

