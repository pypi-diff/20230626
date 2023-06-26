# Comparing `tmp/pulumi_opsgenie-1.3.0a1687672889.tar.gz` & `tmp/pulumi_opsgenie-1.3.0a1687799894.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_opsgenie-1.3.0a1687672889.tar", last modified: Sun Jun 25 06:07:02 2023, max compression
+gzip compressed data, was "pulumi_opsgenie-1.3.0a1687799894.tar", last modified: Mon Jun 26 17:22:31 2023, max compression
```

## Comparing `pulumi_opsgenie-1.3.0a1687672889.tar` & `pulumi_opsgenie-1.3.0a1687799894.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:07:02.973142 pulumi_opsgenie-1.3.0a1687672889/
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-25 06:07:02.973142 pulumi_opsgenie-1.3.0a1687672889/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:07:02.973142 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   179600 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    57892 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/alert_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    33460 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/api_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:07:02.973142 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/custom_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    23692 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/email_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/escalation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/get_escalation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9977 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/get_heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/get_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/get_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/get_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    23842 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    23703 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/incident_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    27020 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/integration_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    34667 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/notification_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    30482 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/notification_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)   160301 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14376 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    25415 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/schedule_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10881 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/service_incident_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    19469 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/team.py
--rw-r--r--   0 runner    (1001) docker     (123)    26743 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/team_routing_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    26257 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/user_contact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:07:02.973142 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 06:07:02.973142 pulumi_opsgenie-1.3.0a1687672889/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-25 06:07:02.000000 pulumi_opsgenie-1.3.0a1687672889/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:22:31.105456 pulumi_opsgenie-1.3.0a1687799894/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-26 17:22:31.105456 pulumi_opsgenie-1.3.0a1687799894/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:22:31.105456 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179600 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57892 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/alert_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32958 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/api_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:22:31.105456 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/custom_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23084 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/email_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17617 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/escalation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_escalation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9977 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23842 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23703 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/incident_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15598 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/integration_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34667 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/notification_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30482 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/notification_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)   160301 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14376 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25289 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/schedule_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10881 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/service_incident_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19469 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26743 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/team_routing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26257 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/user_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:22:31.105456 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-26 17:22:31.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-26 17:22:31.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:22:31.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:22:31.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 17:22:31.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 17:22:31.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:22:31.105456 pulumi_opsgenie-1.3.0a1687799894/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/setup.py
```

### Comparing `pulumi_opsgenie-1.3.0a1687672889/PKG-INFO` & `pulumi_opsgenie-1.3.0a1687799894/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_opsgenie
-Version: 1.3.0a1687672889
+Version: 1.3.0a1687799894
 Summary: A Pulumi package for creating and managing opsgenie cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-opsgenie
 Keywords: pulumi opsgenie
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_opsgenie-1.3.0a1687672889/README.md` & `pulumi_opsgenie-1.3.0a1687799894/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/__init__.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/_inputs.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/_utilities.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/alert_policy.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/alert_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/api_integration.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/api_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -383,37 +383,37 @@
         import pulumi_opsgenie as opsgenie
 
         example_api_integration_api_integration = opsgenie.ApiIntegration("example-api-integrationApiIntegration",
             type="API",
             responders=[
                 opsgenie.ApiIntegrationResponderArgs(
                     type="user",
-                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                    id=opsgenie_user["user"]["id"],
                 ),
                 opsgenie.ApiIntegrationResponderArgs(
                     type="user",
-                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                    id=opsgenie_user["fahri"]["id"],
                 ),
             ])
         example_api_integration_index_api_integration_api_integration = opsgenie.ApiIntegration("example-api-integrationIndex/apiIntegrationApiIntegration",
             type="Prometheus",
             responders=[opsgenie.ApiIntegrationResponderArgs(
                 type="user",
-                id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                id=opsgenie_user["user"]["id"],
             )],
             enabled=False,
             allow_write_access=False,
             ignore_responders_from_payload=True,
             suppress_notifications=True,
             owner_team_id=opsgenie_team["team"]["id"])
         test3 = opsgenie.ApiIntegration("test3",
             type="Webhook",
             responders=[opsgenie.ApiIntegrationResponderArgs(
                 type="user",
-                id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                id=opsgenie_user["user"]["id"],
             )],
             enabled=False,
             allow_write_access=False,
             suppress_notifications=True,
             webhook_url="https://api.example.com/v1",
             headers={
                 "header1": value1,
@@ -456,37 +456,37 @@
         import pulumi_opsgenie as opsgenie
 
         example_api_integration_api_integration = opsgenie.ApiIntegration("example-api-integrationApiIntegration",
             type="API",
             responders=[
                 opsgenie.ApiIntegrationResponderArgs(
                     type="user",
-                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                    id=opsgenie_user["user"]["id"],
                 ),
                 opsgenie.ApiIntegrationResponderArgs(
                     type="user",
-                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                    id=opsgenie_user["fahri"]["id"],
                 ),
             ])
         example_api_integration_index_api_integration_api_integration = opsgenie.ApiIntegration("example-api-integrationIndex/apiIntegrationApiIntegration",
             type="Prometheus",
             responders=[opsgenie.ApiIntegrationResponderArgs(
                 type="user",
-                id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                id=opsgenie_user["user"]["id"],
             )],
             enabled=False,
             allow_write_access=False,
             ignore_responders_from_payload=True,
             suppress_notifications=True,
             owner_team_id=opsgenie_team["team"]["id"])
         test3 = opsgenie.ApiIntegration("test3",
             type="Webhook",
             responders=[opsgenie.ApiIntegrationResponderArgs(
                 type="user",
-                id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                id=opsgenie_user["user"]["id"],
             )],
             enabled=False,
             allow_write_access=False,
             suppress_notifications=True,
             webhook_url="https://api.example.com/v1",
             headers={
                 "header1": value1,
```

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/config/vars.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/custom_role.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/custom_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/email_integration.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/email_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -267,37 +267,37 @@
         import pulumi_opsgenie as opsgenie
 
         test_email_integration = opsgenie.EmailIntegration("testEmailIntegration", email_username="fahri")
         test_index_email_integration_email_integration = opsgenie.EmailIntegration("testIndex/emailIntegrationEmailIntegration",
             responders=[
                 opsgenie.EmailIntegrationResponderArgs(
                     type="user",
-                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                    id=opsgenie_user["test"]["id"],
                 ),
                 opsgenie.EmailIntegrationResponderArgs(
                     type="schedule",
-                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                    id=opsgenie_schedule["test"]["id"],
                 ),
                 opsgenie.EmailIntegrationResponderArgs(
                     type="escalation",
-                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                    id=opsgenie_escalation["test"]["id"],
                 ),
                 opsgenie.EmailIntegrationResponderArgs(
                     type="team",
-                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                    id=opsgenie_team["test2"]["id"],
                 ),
             ],
             email_username="test",
             enabled=True,
             ignore_responders_from_payload=True,
             suppress_notifications=True)
         test_opsgenie_index_email_integration_email_integration = opsgenie.EmailIntegration("testOpsgenieIndex/emailIntegrationEmailIntegration",
             responders=[opsgenie.EmailIntegrationResponderArgs(
                 type="user",
-                id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                id=opsgenie_user["test"]["id"],
             )],
             email_username="test",
             enabled=True,
             ignore_responders_from_payload=True,
             suppress_notifications=True,
             owner_team_id=opsgenie_team_genies["id"])
         ```
@@ -335,37 +335,37 @@
         import pulumi_opsgenie as opsgenie
 
         test_email_integration = opsgenie.EmailIntegration("testEmailIntegration", email_username="fahri")
         test_index_email_integration_email_integration = opsgenie.EmailIntegration("testIndex/emailIntegrationEmailIntegration",
             responders=[
                 opsgenie.EmailIntegrationResponderArgs(
                     type="user",
-                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                    id=opsgenie_user["test"]["id"],
                 ),
                 opsgenie.EmailIntegrationResponderArgs(
                     type="schedule",
-                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                    id=opsgenie_schedule["test"]["id"],
                 ),
                 opsgenie.EmailIntegrationResponderArgs(
                     type="escalation",
-                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                    id=opsgenie_escalation["test"]["id"],
                 ),
                 opsgenie.EmailIntegrationResponderArgs(
                     type="team",
-                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                    id=opsgenie_team["test2"]["id"],
                 ),
             ],
             email_username="test",
             enabled=True,
             ignore_responders_from_payload=True,
             suppress_notifications=True)
         test_opsgenie_index_email_integration_email_integration = opsgenie.EmailIntegration("testOpsgenieIndex/emailIntegrationEmailIntegration",
             responders=[opsgenie.EmailIntegrationResponderArgs(
                 type="user",
-                id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                id=opsgenie_user["test"]["id"],
             )],
             email_username="test",
             enabled=True,
             ignore_responders_from_payload=True,
             suppress_notifications=True,
             owner_team_id=opsgenie_team_genies["id"])
         ```
```

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/escalation.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/escalation.py`

 * *Files 4% similar despite different names*

```diff
@@ -219,23 +219,23 @@
             )],
             rules=[opsgenie.EscalationRuleArgs(
                 condition="if-not-acked",
                 delay=1,
                 notify_type="default",
                 recipients=[
                     opsgenie.EscalationRuleRecipientArgs(
-                        id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                        id=opsgenie_user["test"]["id"],
                         type="user",
                     ),
                     opsgenie.EscalationRuleRecipientArgs(
-                        id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                        id=opsgenie_team["test"]["id"],
                         type="team",
                     ),
                     opsgenie.EscalationRuleRecipientArgs(
-                        id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                        id=opsgenie_schedule["test"]["id"],
                         type="schedule",
                     ),
                 ],
             )])
         ```
 
         ## Import
@@ -280,23 +280,23 @@
             )],
             rules=[opsgenie.EscalationRuleArgs(
                 condition="if-not-acked",
                 delay=1,
                 notify_type="default",
                 recipients=[
                     opsgenie.EscalationRuleRecipientArgs(
-                        id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                        id=opsgenie_user["test"]["id"],
                         type="user",
                     ),
                     opsgenie.EscalationRuleRecipientArgs(
-                        id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                        id=opsgenie_team["test"]["id"],
                         type="team",
                     ),
                     opsgenie.EscalationRuleRecipientArgs(
-                        id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                        id=opsgenie_schedule["test"]["id"],
                         type="schedule",
                     ),
                 ],
             )])
         ```
 
         ## Import
```

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/get_escalation.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_escalation.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/get_heartbeat.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_heartbeat.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/get_schedule.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/get_service.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/get_team.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/get_user.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/heartbeat.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/incident_template.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/incident_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/integration_action.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/notification_rule.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,588 +7,627 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
 
-__all__ = ['IntegrationActionArgs', 'IntegrationAction']
+__all__ = ['NotificationRuleArgs', 'NotificationRule']
 
 @pulumi.input_type
-class IntegrationActionArgs:
+class NotificationRuleArgs:
     def __init__(__self__, *,
-                 integration_id: pulumi.Input[str],
-                 acknowledges: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAcknowledgeArgs']]]] = None,
-                 add_notes: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAddNoteArgs']]]] = None,
-                 closes: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCloseArgs']]]] = None,
-                 creates: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCreateArgs']]]] = None,
-                 ignores: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionIgnoreArgs']]]] = None):
+                 action_type: pulumi.Input[str],
+                 username: pulumi.Input[str],
+                 criterias: Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleCriteriaArgs']]]] = None,
+                 enabled: Optional[pulumi.Input[bool]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 notification_times: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 order: Optional[pulumi.Input[int]] = None,
+                 repeats: Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleRepeatArgs']]]] = None,
+                 schedules: Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleScheduleArgs']]]] = None,
+                 steps: Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleStepArgs']]]] = None,
+                 time_restrictions: Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleTimeRestrictionArgs']]]] = None):
         """
-        The set of arguments for constructing a IntegrationAction resource.
-        :param pulumi.Input[str] integration_id: ID of the parent integration resource to bind to.
+        The set of arguments for constructing a NotificationRule resource.
+        :param pulumi.Input[str] action_type: Type of the action that notification rule will have. Allowed values: `create-alert`, `acknowledged-alert`, `closed-alert`, `assigned-alert`, `add-note`, `schedule-start`, `schedule-end`, `incoming-call-routing`
+        :param pulumi.Input[str] username: Username of user to which this notification rule belongs to.
+        :param pulumi.Input[bool] enabled: If policy should be enabled. Default: `true`
+        :param pulumi.Input[str] name: Name of the notification policy
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] notification_times: List of Time Periods that notification for schedule start/end will be sent. Allowed values: `just-before`, `15-minutes-ago`, `1-hour-ago`, `1-day-ago`. If `action_type` is `schedule-start` or `schedule-end` then it is required.
+        :param pulumi.Input[int] order: Order of the condition in conditions list
+        :param pulumi.Input[Sequence[pulumi.Input['NotificationRuleStepArgs']]] steps: Notification rule steps to take (eg. SMS or email message). This is a block, structure is documented below.
         """
-        pulumi.set(__self__, "integration_id", integration_id)
-        if acknowledges is not None:
-            pulumi.set(__self__, "acknowledges", acknowledges)
-        if add_notes is not None:
-            pulumi.set(__self__, "add_notes", add_notes)
-        if closes is not None:
-            pulumi.set(__self__, "closes", closes)
-        if creates is not None:
-            pulumi.set(__self__, "creates", creates)
-        if ignores is not None:
-            pulumi.set(__self__, "ignores", ignores)
+        pulumi.set(__self__, "action_type", action_type)
+        pulumi.set(__self__, "username", username)
+        if criterias is not None:
+            pulumi.set(__self__, "criterias", criterias)
+        if enabled is not None:
+            pulumi.set(__self__, "enabled", enabled)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if notification_times is not None:
+            pulumi.set(__self__, "notification_times", notification_times)
+        if order is not None:
+            pulumi.set(__self__, "order", order)
+        if repeats is not None:
+            pulumi.set(__self__, "repeats", repeats)
+        if schedules is not None:
+            pulumi.set(__self__, "schedules", schedules)
+        if steps is not None:
+            pulumi.set(__self__, "steps", steps)
+        if time_restrictions is not None:
+            pulumi.set(__self__, "time_restrictions", time_restrictions)
 
     @property
-    @pulumi.getter(name="integrationId")
-    def integration_id(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="actionType")
+    def action_type(self) -> pulumi.Input[str]:
         """
-        ID of the parent integration resource to bind to.
+        Type of the action that notification rule will have. Allowed values: `create-alert`, `acknowledged-alert`, `closed-alert`, `assigned-alert`, `add-note`, `schedule-start`, `schedule-end`, `incoming-call-routing`
         """
-        return pulumi.get(self, "integration_id")
+        return pulumi.get(self, "action_type")
 
-    @integration_id.setter
-    def integration_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "integration_id", value)
+    @action_type.setter
+    def action_type(self, value: pulumi.Input[str]):
+        pulumi.set(self, "action_type", value)
 
     @property
     @pulumi.getter
-    def acknowledges(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAcknowledgeArgs']]]]:
-        return pulumi.get(self, "acknowledges")
+    def username(self) -> pulumi.Input[str]:
+        """
+        Username of user to which this notification rule belongs to.
+        """
+        return pulumi.get(self, "username")
+
+    @username.setter
+    def username(self, value: pulumi.Input[str]):
+        pulumi.set(self, "username", value)
+
+    @property
+    @pulumi.getter
+    def criterias(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleCriteriaArgs']]]]:
+        return pulumi.get(self, "criterias")
+
+    @criterias.setter
+    def criterias(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleCriteriaArgs']]]]):
+        pulumi.set(self, "criterias", value)
+
+    @property
+    @pulumi.getter
+    def enabled(self) -> Optional[pulumi.Input[bool]]:
+        """
+        If policy should be enabled. Default: `true`
+        """
+        return pulumi.get(self, "enabled")
+
+    @enabled.setter
+    def enabled(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enabled", value)
 
-    @acknowledges.setter
-    def acknowledges(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAcknowledgeArgs']]]]):
-        pulumi.set(self, "acknowledges", value)
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Name of the notification policy
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="addNotes")
-    def add_notes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAddNoteArgs']]]]:
-        return pulumi.get(self, "add_notes")
+    @pulumi.getter(name="notificationTimes")
+    def notification_times(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        List of Time Periods that notification for schedule start/end will be sent. Allowed values: `just-before`, `15-minutes-ago`, `1-hour-ago`, `1-day-ago`. If `action_type` is `schedule-start` or `schedule-end` then it is required.
+        """
+        return pulumi.get(self, "notification_times")
 
-    @add_notes.setter
-    def add_notes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAddNoteArgs']]]]):
-        pulumi.set(self, "add_notes", value)
+    @notification_times.setter
+    def notification_times(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "notification_times", value)
 
     @property
     @pulumi.getter
-    def closes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCloseArgs']]]]:
-        return pulumi.get(self, "closes")
+    def order(self) -> Optional[pulumi.Input[int]]:
+        """
+        Order of the condition in conditions list
+        """
+        return pulumi.get(self, "order")
 
-    @closes.setter
-    def closes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCloseArgs']]]]):
-        pulumi.set(self, "closes", value)
+    @order.setter
+    def order(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "order", value)
 
     @property
     @pulumi.getter
-    def creates(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCreateArgs']]]]:
-        return pulumi.get(self, "creates")
+    def repeats(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleRepeatArgs']]]]:
+        return pulumi.get(self, "repeats")
 
-    @creates.setter
-    def creates(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCreateArgs']]]]):
-        pulumi.set(self, "creates", value)
+    @repeats.setter
+    def repeats(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleRepeatArgs']]]]):
+        pulumi.set(self, "repeats", value)
 
     @property
     @pulumi.getter
-    def ignores(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionIgnoreArgs']]]]:
-        return pulumi.get(self, "ignores")
+    def schedules(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleScheduleArgs']]]]:
+        return pulumi.get(self, "schedules")
 
-    @ignores.setter
-    def ignores(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionIgnoreArgs']]]]):
-        pulumi.set(self, "ignores", value)
+    @schedules.setter
+    def schedules(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleScheduleArgs']]]]):
+        pulumi.set(self, "schedules", value)
+
+    @property
+    @pulumi.getter
+    def steps(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleStepArgs']]]]:
+        """
+        Notification rule steps to take (eg. SMS or email message). This is a block, structure is documented below.
+        """
+        return pulumi.get(self, "steps")
+
+    @steps.setter
+    def steps(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleStepArgs']]]]):
+        pulumi.set(self, "steps", value)
+
+    @property
+    @pulumi.getter(name="timeRestrictions")
+    def time_restrictions(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleTimeRestrictionArgs']]]]:
+        return pulumi.get(self, "time_restrictions")
+
+    @time_restrictions.setter
+    def time_restrictions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleTimeRestrictionArgs']]]]):
+        pulumi.set(self, "time_restrictions", value)
 
 
 @pulumi.input_type
-class _IntegrationActionState:
+class _NotificationRuleState:
     def __init__(__self__, *,
-                 acknowledges: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAcknowledgeArgs']]]] = None,
-                 add_notes: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAddNoteArgs']]]] = None,
-                 closes: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCloseArgs']]]] = None,
-                 creates: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCreateArgs']]]] = None,
-                 ignores: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionIgnoreArgs']]]] = None,
-                 integration_id: Optional[pulumi.Input[str]] = None):
+                 action_type: Optional[pulumi.Input[str]] = None,
+                 criterias: Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleCriteriaArgs']]]] = None,
+                 enabled: Optional[pulumi.Input[bool]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 notification_times: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 order: Optional[pulumi.Input[int]] = None,
+                 repeats: Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleRepeatArgs']]]] = None,
+                 schedules: Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleScheduleArgs']]]] = None,
+                 steps: Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleStepArgs']]]] = None,
+                 time_restrictions: Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleTimeRestrictionArgs']]]] = None,
+                 username: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering IntegrationAction resources.
-        :param pulumi.Input[str] integration_id: ID of the parent integration resource to bind to.
+        Input properties used for looking up and filtering NotificationRule resources.
+        :param pulumi.Input[str] action_type: Type of the action that notification rule will have. Allowed values: `create-alert`, `acknowledged-alert`, `closed-alert`, `assigned-alert`, `add-note`, `schedule-start`, `schedule-end`, `incoming-call-routing`
+        :param pulumi.Input[bool] enabled: If policy should be enabled. Default: `true`
+        :param pulumi.Input[str] name: Name of the notification policy
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] notification_times: List of Time Periods that notification for schedule start/end will be sent. Allowed values: `just-before`, `15-minutes-ago`, `1-hour-ago`, `1-day-ago`. If `action_type` is `schedule-start` or `schedule-end` then it is required.
+        :param pulumi.Input[int] order: Order of the condition in conditions list
+        :param pulumi.Input[Sequence[pulumi.Input['NotificationRuleStepArgs']]] steps: Notification rule steps to take (eg. SMS or email message). This is a block, structure is documented below.
+        :param pulumi.Input[str] username: Username of user to which this notification rule belongs to.
         """
-        if acknowledges is not None:
-            pulumi.set(__self__, "acknowledges", acknowledges)
-        if add_notes is not None:
-            pulumi.set(__self__, "add_notes", add_notes)
-        if closes is not None:
-            pulumi.set(__self__, "closes", closes)
-        if creates is not None:
-            pulumi.set(__self__, "creates", creates)
-        if ignores is not None:
-            pulumi.set(__self__, "ignores", ignores)
-        if integration_id is not None:
-            pulumi.set(__self__, "integration_id", integration_id)
+        if action_type is not None:
+            pulumi.set(__self__, "action_type", action_type)
+        if criterias is not None:
+            pulumi.set(__self__, "criterias", criterias)
+        if enabled is not None:
+            pulumi.set(__self__, "enabled", enabled)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if notification_times is not None:
+            pulumi.set(__self__, "notification_times", notification_times)
+        if order is not None:
+            pulumi.set(__self__, "order", order)
+        if repeats is not None:
+            pulumi.set(__self__, "repeats", repeats)
+        if schedules is not None:
+            pulumi.set(__self__, "schedules", schedules)
+        if steps is not None:
+            pulumi.set(__self__, "steps", steps)
+        if time_restrictions is not None:
+            pulumi.set(__self__, "time_restrictions", time_restrictions)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter(name="actionType")
+    def action_type(self) -> Optional[pulumi.Input[str]]:
+        """
+        Type of the action that notification rule will have. Allowed values: `create-alert`, `acknowledged-alert`, `closed-alert`, `assigned-alert`, `add-note`, `schedule-start`, `schedule-end`, `incoming-call-routing`
+        """
+        return pulumi.get(self, "action_type")
+
+    @action_type.setter
+    def action_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "action_type", value)
 
     @property
     @pulumi.getter
-    def acknowledges(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAcknowledgeArgs']]]]:
-        return pulumi.get(self, "acknowledges")
+    def criterias(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleCriteriaArgs']]]]:
+        return pulumi.get(self, "criterias")
+
+    @criterias.setter
+    def criterias(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleCriteriaArgs']]]]):
+        pulumi.set(self, "criterias", value)
+
+    @property
+    @pulumi.getter
+    def enabled(self) -> Optional[pulumi.Input[bool]]:
+        """
+        If policy should be enabled. Default: `true`
+        """
+        return pulumi.get(self, "enabled")
+
+    @enabled.setter
+    def enabled(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enabled", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Name of the notification policy
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter(name="notificationTimes")
+    def notification_times(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        List of Time Periods that notification for schedule start/end will be sent. Allowed values: `just-before`, `15-minutes-ago`, `1-hour-ago`, `1-day-ago`. If `action_type` is `schedule-start` or `schedule-end` then it is required.
+        """
+        return pulumi.get(self, "notification_times")
 
-    @acknowledges.setter
-    def acknowledges(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAcknowledgeArgs']]]]):
-        pulumi.set(self, "acknowledges", value)
+    @notification_times.setter
+    def notification_times(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "notification_times", value)
 
     @property
-    @pulumi.getter(name="addNotes")
-    def add_notes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAddNoteArgs']]]]:
-        return pulumi.get(self, "add_notes")
+    @pulumi.getter
+    def order(self) -> Optional[pulumi.Input[int]]:
+        """
+        Order of the condition in conditions list
+        """
+        return pulumi.get(self, "order")
 
-    @add_notes.setter
-    def add_notes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAddNoteArgs']]]]):
-        pulumi.set(self, "add_notes", value)
+    @order.setter
+    def order(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "order", value)
 
     @property
     @pulumi.getter
-    def closes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCloseArgs']]]]:
-        return pulumi.get(self, "closes")
+    def repeats(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleRepeatArgs']]]]:
+        return pulumi.get(self, "repeats")
 
-    @closes.setter
-    def closes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCloseArgs']]]]):
-        pulumi.set(self, "closes", value)
+    @repeats.setter
+    def repeats(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleRepeatArgs']]]]):
+        pulumi.set(self, "repeats", value)
 
     @property
     @pulumi.getter
-    def creates(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCreateArgs']]]]:
-        return pulumi.get(self, "creates")
+    def schedules(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleScheduleArgs']]]]:
+        return pulumi.get(self, "schedules")
 
-    @creates.setter
-    def creates(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCreateArgs']]]]):
-        pulumi.set(self, "creates", value)
+    @schedules.setter
+    def schedules(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleScheduleArgs']]]]):
+        pulumi.set(self, "schedules", value)
 
     @property
     @pulumi.getter
-    def ignores(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionIgnoreArgs']]]]:
-        return pulumi.get(self, "ignores")
+    def steps(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleStepArgs']]]]:
+        """
+        Notification rule steps to take (eg. SMS or email message). This is a block, structure is documented below.
+        """
+        return pulumi.get(self, "steps")
 
-    @ignores.setter
-    def ignores(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionIgnoreArgs']]]]):
-        pulumi.set(self, "ignores", value)
+    @steps.setter
+    def steps(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleStepArgs']]]]):
+        pulumi.set(self, "steps", value)
 
     @property
-    @pulumi.getter(name="integrationId")
-    def integration_id(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="timeRestrictions")
+    def time_restrictions(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleTimeRestrictionArgs']]]]:
+        return pulumi.get(self, "time_restrictions")
+
+    @time_restrictions.setter
+    def time_restrictions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleTimeRestrictionArgs']]]]):
+        pulumi.set(self, "time_restrictions", value)
+
+    @property
+    @pulumi.getter
+    def username(self) -> Optional[pulumi.Input[str]]:
         """
-        ID of the parent integration resource to bind to.
+        Username of user to which this notification rule belongs to.
         """
-        return pulumi.get(self, "integration_id")
+        return pulumi.get(self, "username")
 
-    @integration_id.setter
-    def integration_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "integration_id", value)
+    @username.setter
+    def username(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "username", value)
 
 
-class IntegrationAction(pulumi.CustomResource):
+class NotificationRule(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 acknowledges: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionAcknowledgeArgs']]]]] = None,
-                 add_notes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionAddNoteArgs']]]]] = None,
-                 closes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionCloseArgs']]]]] = None,
-                 creates: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionCreateArgs']]]]] = None,
-                 ignores: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionIgnoreArgs']]]]] = None,
-                 integration_id: Optional[pulumi.Input[str]] = None,
+                 action_type: Optional[pulumi.Input[str]] = None,
+                 criterias: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NotificationRuleCriteriaArgs']]]]] = None,
+                 enabled: Optional[pulumi.Input[bool]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 notification_times: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 order: Optional[pulumi.Input[int]] = None,
+                 repeats: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NotificationRuleRepeatArgs']]]]] = None,
+                 schedules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NotificationRuleScheduleArgs']]]]] = None,
+                 steps: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NotificationRuleStepArgs']]]]] = None,
+                 time_restrictions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NotificationRuleTimeRestrictionArgs']]]]] = None,
+                 username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Manages advanced actions for Integrations within Opsgenie. This applies for the following resources:
-        * `ApiIntegration`
-        * `EmailIntegration`
-
-        The actions that are supported are:
-        * `create`
-        * `close`
-        * `acknowledge`
-        * `add_note`
-        * `ignore`
+        Manages a Notification Rule within Opsgenie.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
-        test_action = opsgenie.IntegrationAction("testAction",
-            integration_id=opsgenie_api_integration["test"]["id"],
-            creates=[
-                opsgenie.IntegrationActionCreateArgs(
-                    name="create action",
-                    tags=[
-                        "CRITICAL",
-                        "SEV-0",
-                    ],
-                    user="Example-service",
-                    note="{{note}}",
-                    alias="{{alias}}",
-                    source="{{source}}",
-                    message="{{message}}",
-                    description="{{description}}",
-                    entity="{{entity}}",
-                    alert_actions=["Runbook ID#342"],
-                    filters=[opsgenie.IntegrationActionCreateFilterArgs(
-                        type="match-all-conditions",
-                        conditions=[opsgenie.IntegrationActionCreateFilterConditionArgs(
-                            field="priority",
-                            operation="equals",
-                            expected_value="P1",
-                        )],
-                    )],
-                    responders=[opsgenie.IntegrationActionCreateResponderArgs(
-                        id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-                        type="team",
-                    )],
-                ),
-                opsgenie.IntegrationActionCreateArgs(
-                    name="Create medium priority alerts",
-                    tags=[
-                        "SEVERE",
-                        "SEV-1",
-                    ],
-                    priority="P3",
-                    filters=[opsgenie.IntegrationActionCreateFilterArgs(
-                        type="match-all-conditions",
-                        conditions=[opsgenie.IntegrationActionCreateFilterConditionArgs(
-                            field="priority",
-                            operation="equals",
-                            expected_value="P2",
-                        )],
-                    )],
-                ),
-                opsgenie.IntegrationActionCreateArgs(
-                    name="Create alert with priority from message",
-                    custom_priority="{{message.substringAfter(\\"[custom]\\")}}",
-                    filters=[opsgenie.IntegrationActionCreateFilterArgs(
-                        type="match-all-conditions",
-                        conditions=[
-                            opsgenie.IntegrationActionCreateFilterConditionArgs(
-                                field="tags",
-                                operation="contains",
-                                expected_value="P5",
-                            ),
-                            opsgenie.IntegrationActionCreateFilterConditionArgs(
-                                field="message",
-                                operation="starts-with",
-                                expected_value="[custom]",
-                            ),
-                        ],
-                    )],
-                ),
+        test_user = opsgenie.User("testUser",
+            username="Example user",
+            full_name="Name Lastname",
+            role="User")
+        test_notification_rule = opsgenie.NotificationRule("testNotificationRule",
+            username=test_user.username,
+            action_type="schedule-end",
+            notification_times=[
+                "just-before",
+                "15-minutes-ago",
             ],
-            closes=[opsgenie.IntegrationActionCloseArgs(
-                name="Low priority alerts",
-                filters=[opsgenie.IntegrationActionCloseFilterArgs(
-                    type="match-any-condition",
-                    conditions=[
-                        opsgenie.IntegrationActionCloseFilterConditionArgs(
-                            field="priority",
-                            operation="equals",
-                            expected_value="P5",
-                        ),
-                        opsgenie.IntegrationActionCloseFilterConditionArgs(
-                            field="message",
-                            operation="contains",
-                            expected_value="DEBUG",
-                        ),
-                    ],
-                )],
-            )],
-            acknowledges=[opsgenie.IntegrationActionAcknowledgeArgs(
-                name="Auto-ack test alerts",
-                filters=[opsgenie.IntegrationActionAcknowledgeFilterArgs(
-                    type="match-all-conditions",
-                    conditions=[
-                        opsgenie.IntegrationActionAcknowledgeFilterConditionArgs(
-                            field="message",
-                            not_=True,
-                            operation="contains",
-                            expected_value="TEST",
-                        ),
-                        opsgenie.IntegrationActionAcknowledgeFilterConditionArgs(
-                            field="priority",
-                            operation="equals",
-                            expected_value="P5",
-                        ),
-                    ],
-                )],
-            )],
-            add_notes=[opsgenie.IntegrationActionAddNoteArgs(
-                name="Add note to all alerts",
-                note="Created from test integration",
-                filters=[opsgenie.IntegrationActionAddNoteFilterArgs(
-                    type="match-all",
-                )],
-            )],
-            ignores=[opsgenie.IntegrationActionIgnoreArgs(
-                name="Ignore alerts with ignore tag",
-                filters=[opsgenie.IntegrationActionIgnoreFilterArgs(
-                    type="match-all-conditions",
-                    conditions=[opsgenie.IntegrationActionIgnoreFilterConditionArgs(
-                        field="tags",
-                        operation="contains",
-                        expected_value="ignore",
-                    )],
+            steps=[opsgenie.NotificationRuleStepArgs(
+                contacts=[opsgenie.NotificationRuleStepContactArgs(
+                    method="email",
+                    to="example@user.com",
                 )],
             )])
         ```
 
+        ## Import
+
+        Notification policies can be imported using the `user_id/notification_rule_id`, e.g.
+
+        ```sh
+         $ pulumi import opsgenie:index/notificationRule:NotificationRule test user_id/notification_rule_id`
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] integration_id: ID of the parent integration resource to bind to.
+        :param pulumi.Input[str] action_type: Type of the action that notification rule will have. Allowed values: `create-alert`, `acknowledged-alert`, `closed-alert`, `assigned-alert`, `add-note`, `schedule-start`, `schedule-end`, `incoming-call-routing`
+        :param pulumi.Input[bool] enabled: If policy should be enabled. Default: `true`
+        :param pulumi.Input[str] name: Name of the notification policy
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] notification_times: List of Time Periods that notification for schedule start/end will be sent. Allowed values: `just-before`, `15-minutes-ago`, `1-hour-ago`, `1-day-ago`. If `action_type` is `schedule-start` or `schedule-end` then it is required.
+        :param pulumi.Input[int] order: Order of the condition in conditions list
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NotificationRuleStepArgs']]]] steps: Notification rule steps to take (eg. SMS or email message). This is a block, structure is documented below.
+        :param pulumi.Input[str] username: Username of user to which this notification rule belongs to.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: IntegrationActionArgs,
+                 args: NotificationRuleArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Manages advanced actions for Integrations within Opsgenie. This applies for the following resources:
-        * `ApiIntegration`
-        * `EmailIntegration`
-
-        The actions that are supported are:
-        * `create`
-        * `close`
-        * `acknowledge`
-        * `add_note`
-        * `ignore`
+        Manages a Notification Rule within Opsgenie.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
-        test_action = opsgenie.IntegrationAction("testAction",
-            integration_id=opsgenie_api_integration["test"]["id"],
-            creates=[
-                opsgenie.IntegrationActionCreateArgs(
-                    name="create action",
-                    tags=[
-                        "CRITICAL",
-                        "SEV-0",
-                    ],
-                    user="Example-service",
-                    note="{{note}}",
-                    alias="{{alias}}",
-                    source="{{source}}",
-                    message="{{message}}",
-                    description="{{description}}",
-                    entity="{{entity}}",
-                    alert_actions=["Runbook ID#342"],
-                    filters=[opsgenie.IntegrationActionCreateFilterArgs(
-                        type="match-all-conditions",
-                        conditions=[opsgenie.IntegrationActionCreateFilterConditionArgs(
-                            field="priority",
-                            operation="equals",
-                            expected_value="P1",
-                        )],
-                    )],
-                    responders=[opsgenie.IntegrationActionCreateResponderArgs(
-                        id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-                        type="team",
-                    )],
-                ),
-                opsgenie.IntegrationActionCreateArgs(
-                    name="Create medium priority alerts",
-                    tags=[
-                        "SEVERE",
-                        "SEV-1",
-                    ],
-                    priority="P3",
-                    filters=[opsgenie.IntegrationActionCreateFilterArgs(
-                        type="match-all-conditions",
-                        conditions=[opsgenie.IntegrationActionCreateFilterConditionArgs(
-                            field="priority",
-                            operation="equals",
-                            expected_value="P2",
-                        )],
-                    )],
-                ),
-                opsgenie.IntegrationActionCreateArgs(
-                    name="Create alert with priority from message",
-                    custom_priority="{{message.substringAfter(\\"[custom]\\")}}",
-                    filters=[opsgenie.IntegrationActionCreateFilterArgs(
-                        type="match-all-conditions",
-                        conditions=[
-                            opsgenie.IntegrationActionCreateFilterConditionArgs(
-                                field="tags",
-                                operation="contains",
-                                expected_value="P5",
-                            ),
-                            opsgenie.IntegrationActionCreateFilterConditionArgs(
-                                field="message",
-                                operation="starts-with",
-                                expected_value="[custom]",
-                            ),
-                        ],
-                    )],
-                ),
+        test_user = opsgenie.User("testUser",
+            username="Example user",
+            full_name="Name Lastname",
+            role="User")
+        test_notification_rule = opsgenie.NotificationRule("testNotificationRule",
+            username=test_user.username,
+            action_type="schedule-end",
+            notification_times=[
+                "just-before",
+                "15-minutes-ago",
             ],
-            closes=[opsgenie.IntegrationActionCloseArgs(
-                name="Low priority alerts",
-                filters=[opsgenie.IntegrationActionCloseFilterArgs(
-                    type="match-any-condition",
-                    conditions=[
-                        opsgenie.IntegrationActionCloseFilterConditionArgs(
-                            field="priority",
-                            operation="equals",
-                            expected_value="P5",
-                        ),
-                        opsgenie.IntegrationActionCloseFilterConditionArgs(
-                            field="message",
-                            operation="contains",
-                            expected_value="DEBUG",
-                        ),
-                    ],
-                )],
-            )],
-            acknowledges=[opsgenie.IntegrationActionAcknowledgeArgs(
-                name="Auto-ack test alerts",
-                filters=[opsgenie.IntegrationActionAcknowledgeFilterArgs(
-                    type="match-all-conditions",
-                    conditions=[
-                        opsgenie.IntegrationActionAcknowledgeFilterConditionArgs(
-                            field="message",
-                            not_=True,
-                            operation="contains",
-                            expected_value="TEST",
-                        ),
-                        opsgenie.IntegrationActionAcknowledgeFilterConditionArgs(
-                            field="priority",
-                            operation="equals",
-                            expected_value="P5",
-                        ),
-                    ],
-                )],
-            )],
-            add_notes=[opsgenie.IntegrationActionAddNoteArgs(
-                name="Add note to all alerts",
-                note="Created from test integration",
-                filters=[opsgenie.IntegrationActionAddNoteFilterArgs(
-                    type="match-all",
-                )],
-            )],
-            ignores=[opsgenie.IntegrationActionIgnoreArgs(
-                name="Ignore alerts with ignore tag",
-                filters=[opsgenie.IntegrationActionIgnoreFilterArgs(
-                    type="match-all-conditions",
-                    conditions=[opsgenie.IntegrationActionIgnoreFilterConditionArgs(
-                        field="tags",
-                        operation="contains",
-                        expected_value="ignore",
-                    )],
+            steps=[opsgenie.NotificationRuleStepArgs(
+                contacts=[opsgenie.NotificationRuleStepContactArgs(
+                    method="email",
+                    to="example@user.com",
                 )],
             )])
         ```
 
+        ## Import
+
+        Notification policies can be imported using the `user_id/notification_rule_id`, e.g.
+
+        ```sh
+         $ pulumi import opsgenie:index/notificationRule:NotificationRule test user_id/notification_rule_id`
+        ```
+
         :param str resource_name: The name of the resource.
-        :param IntegrationActionArgs args: The arguments to use to populate this resource's properties.
+        :param NotificationRuleArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(IntegrationActionArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(NotificationRuleArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 acknowledges: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionAcknowledgeArgs']]]]] = None,
-                 add_notes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionAddNoteArgs']]]]] = None,
-                 closes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionCloseArgs']]]]] = None,
-                 creates: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionCreateArgs']]]]] = None,
-                 ignores: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionIgnoreArgs']]]]] = None,
-                 integration_id: Optional[pulumi.Input[str]] = None,
+                 action_type: Optional[pulumi.Input[str]] = None,
+                 criterias: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NotificationRuleCriteriaArgs']]]]] = None,
+                 enabled: Optional[pulumi.Input[bool]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 notification_times: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 order: Optional[pulumi.Input[int]] = None,
+                 repeats: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NotificationRuleRepeatArgs']]]]] = None,
+                 schedules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NotificationRuleScheduleArgs']]]]] = None,
+                 steps: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NotificationRuleStepArgs']]]]] = None,
+                 time_restrictions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NotificationRuleTimeRestrictionArgs']]]]] = None,
+                 username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = IntegrationActionArgs.__new__(IntegrationActionArgs)
+            __props__ = NotificationRuleArgs.__new__(NotificationRuleArgs)
 
-            __props__.__dict__["acknowledges"] = acknowledges
-            __props__.__dict__["add_notes"] = add_notes
-            __props__.__dict__["closes"] = closes
-            __props__.__dict__["creates"] = creates
-            __props__.__dict__["ignores"] = ignores
-            if integration_id is None and not opts.urn:
-                raise TypeError("Missing required property 'integration_id'")
-            __props__.__dict__["integration_id"] = integration_id
-        super(IntegrationAction, __self__).__init__(
-            'opsgenie:index/integrationAction:IntegrationAction',
+            if action_type is None and not opts.urn:
+                raise TypeError("Missing required property 'action_type'")
+            __props__.__dict__["action_type"] = action_type
+            __props__.__dict__["criterias"] = criterias
+            __props__.__dict__["enabled"] = enabled
+            __props__.__dict__["name"] = name
+            __props__.__dict__["notification_times"] = notification_times
+            __props__.__dict__["order"] = order
+            __props__.__dict__["repeats"] = repeats
+            __props__.__dict__["schedules"] = schedules
+            __props__.__dict__["steps"] = steps
+            __props__.__dict__["time_restrictions"] = time_restrictions
+            if username is None and not opts.urn:
+                raise TypeError("Missing required property 'username'")
+            __props__.__dict__["username"] = username
+        super(NotificationRule, __self__).__init__(
+            'opsgenie:index/notificationRule:NotificationRule',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            acknowledges: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionAcknowledgeArgs']]]]] = None,
-            add_notes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionAddNoteArgs']]]]] = None,
-            closes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionCloseArgs']]]]] = None,
-            creates: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionCreateArgs']]]]] = None,
-            ignores: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionIgnoreArgs']]]]] = None,
-            integration_id: Optional[pulumi.Input[str]] = None) -> 'IntegrationAction':
+            action_type: Optional[pulumi.Input[str]] = None,
+            criterias: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NotificationRuleCriteriaArgs']]]]] = None,
+            enabled: Optional[pulumi.Input[bool]] = None,
+            name: Optional[pulumi.Input[str]] = None,
+            notification_times: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            order: Optional[pulumi.Input[int]] = None,
+            repeats: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NotificationRuleRepeatArgs']]]]] = None,
+            schedules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NotificationRuleScheduleArgs']]]]] = None,
+            steps: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NotificationRuleStepArgs']]]]] = None,
+            time_restrictions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NotificationRuleTimeRestrictionArgs']]]]] = None,
+            username: Optional[pulumi.Input[str]] = None) -> 'NotificationRule':
         """
-        Get an existing IntegrationAction resource's state with the given name, id, and optional extra
+        Get an existing NotificationRule resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] integration_id: ID of the parent integration resource to bind to.
+        :param pulumi.Input[str] action_type: Type of the action that notification rule will have. Allowed values: `create-alert`, `acknowledged-alert`, `closed-alert`, `assigned-alert`, `add-note`, `schedule-start`, `schedule-end`, `incoming-call-routing`
+        :param pulumi.Input[bool] enabled: If policy should be enabled. Default: `true`
+        :param pulumi.Input[str] name: Name of the notification policy
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] notification_times: List of Time Periods that notification for schedule start/end will be sent. Allowed values: `just-before`, `15-minutes-ago`, `1-hour-ago`, `1-day-ago`. If `action_type` is `schedule-start` or `schedule-end` then it is required.
+        :param pulumi.Input[int] order: Order of the condition in conditions list
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NotificationRuleStepArgs']]]] steps: Notification rule steps to take (eg. SMS or email message). This is a block, structure is documented below.
+        :param pulumi.Input[str] username: Username of user to which this notification rule belongs to.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _IntegrationActionState.__new__(_IntegrationActionState)
+        __props__ = _NotificationRuleState.__new__(_NotificationRuleState)
 
-        __props__.__dict__["acknowledges"] = acknowledges
-        __props__.__dict__["add_notes"] = add_notes
-        __props__.__dict__["closes"] = closes
-        __props__.__dict__["creates"] = creates
-        __props__.__dict__["ignores"] = ignores
-        __props__.__dict__["integration_id"] = integration_id
-        return IntegrationAction(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["action_type"] = action_type
+        __props__.__dict__["criterias"] = criterias
+        __props__.__dict__["enabled"] = enabled
+        __props__.__dict__["name"] = name
+        __props__.__dict__["notification_times"] = notification_times
+        __props__.__dict__["order"] = order
+        __props__.__dict__["repeats"] = repeats
+        __props__.__dict__["schedules"] = schedules
+        __props__.__dict__["steps"] = steps
+        __props__.__dict__["time_restrictions"] = time_restrictions
+        __props__.__dict__["username"] = username
+        return NotificationRule(resource_name, opts=opts, __props__=__props__)
+
+    @property
+    @pulumi.getter(name="actionType")
+    def action_type(self) -> pulumi.Output[str]:
+        """
+        Type of the action that notification rule will have. Allowed values: `create-alert`, `acknowledged-alert`, `closed-alert`, `assigned-alert`, `add-note`, `schedule-start`, `schedule-end`, `incoming-call-routing`
+        """
+        return pulumi.get(self, "action_type")
 
     @property
     @pulumi.getter
-    def acknowledges(self) -> pulumi.Output[Optional[Sequence['outputs.IntegrationActionAcknowledge']]]:
-        return pulumi.get(self, "acknowledges")
+    def criterias(self) -> pulumi.Output[Optional[Sequence['outputs.NotificationRuleCriteria']]]:
+        return pulumi.get(self, "criterias")
 
     @property
-    @pulumi.getter(name="addNotes")
-    def add_notes(self) -> pulumi.Output[Optional[Sequence['outputs.IntegrationActionAddNote']]]:
-        return pulumi.get(self, "add_notes")
+    @pulumi.getter
+    def enabled(self) -> pulumi.Output[Optional[bool]]:
+        """
+        If policy should be enabled. Default: `true`
+        """
+        return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter
-    def closes(self) -> pulumi.Output[Optional[Sequence['outputs.IntegrationActionClose']]]:
-        return pulumi.get(self, "closes")
+    def name(self) -> pulumi.Output[str]:
+        """
+        Name of the notification policy
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="notificationTimes")
+    def notification_times(self) -> pulumi.Output[Optional[Sequence[str]]]:
+        """
+        List of Time Periods that notification for schedule start/end will be sent. Allowed values: `just-before`, `15-minutes-ago`, `1-hour-ago`, `1-day-ago`. If `action_type` is `schedule-start` or `schedule-end` then it is required.
+        """
+        return pulumi.get(self, "notification_times")
 
     @property
     @pulumi.getter
-    def creates(self) -> pulumi.Output[Optional[Sequence['outputs.IntegrationActionCreate']]]:
-        return pulumi.get(self, "creates")
+    def order(self) -> pulumi.Output[int]:
+        """
+        Order of the condition in conditions list
+        """
+        return pulumi.get(self, "order")
+
+    @property
+    @pulumi.getter
+    def repeats(self) -> pulumi.Output[Optional[Sequence['outputs.NotificationRuleRepeat']]]:
+        return pulumi.get(self, "repeats")
+
+    @property
+    @pulumi.getter
+    def schedules(self) -> pulumi.Output[Optional[Sequence['outputs.NotificationRuleSchedule']]]:
+        return pulumi.get(self, "schedules")
 
     @property
     @pulumi.getter
-    def ignores(self) -> pulumi.Output[Optional[Sequence['outputs.IntegrationActionIgnore']]]:
-        return pulumi.get(self, "ignores")
+    def steps(self) -> pulumi.Output[Optional[Sequence['outputs.NotificationRuleStep']]]:
+        """
+        Notification rule steps to take (eg. SMS or email message). This is a block, structure is documented below.
+        """
+        return pulumi.get(self, "steps")
 
     @property
-    @pulumi.getter(name="integrationId")
-    def integration_id(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="timeRestrictions")
+    def time_restrictions(self) -> pulumi.Output[Optional[Sequence['outputs.NotificationRuleTimeRestriction']]]:
+        return pulumi.get(self, "time_restrictions")
+
+    @property
+    @pulumi.getter
+    def username(self) -> pulumi.Output[str]:
         """
-        ID of the parent integration resource to bind to.
+        Username of user to which this notification rule belongs to.
         """
-        return pulumi.get(self, "integration_id")
+        return pulumi.get(self, "username")
```

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/maintenance.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/maintenance.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.Maintenance("test",
             description="geniemaintenance-%s",
             rules=[opsgenie.MaintenanceRuleArgs(
                 entities=[opsgenie.MaintenanceRuleEntityArgs(
-                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                    id=opsgenie_email_integration["test"]["id"],
                     type="integration",
                 )],
                 state="enabled",
             )],
             times=[opsgenie.MaintenanceTimeArgs(
                 end_date="2019-06-%dT17:50:00Z",
                 start_date="2019-06-20T17:45:00Z",
@@ -186,15 +186,15 @@
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.Maintenance("test",
             description="geniemaintenance-%s",
             rules=[opsgenie.MaintenanceRuleArgs(
                 entities=[opsgenie.MaintenanceRuleEntityArgs(
-                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                    id=opsgenie_email_integration["test"]["id"],
                     type="integration",
                 )],
                 state="enabled",
             )],
             times=[opsgenie.MaintenanceTimeArgs(
                 end_date="2019-06-%dT17:50:00Z",
                 start_date="2019-06-20T17:45:00Z",
```

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/notification_policy.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/notification_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/outputs.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/provider.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/schedule.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/schedule_rotation.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/schedule_rotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,15 +296,15 @@
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.ScheduleRotation("test",
             end_date="2019-06-20T17:30:00Z",
             length=6,
             participants=[opsgenie.ScheduleRotationParticipantArgs(
-                id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                id=opsgenie_user["test"]["id"],
                 type="user",
             )],
             schedule_id=opsgenie_schedule["test"]["id"],
             start_date="2019-06-18T17:00:00Z",
             time_restrictions=[opsgenie.ScheduleRotationTimeRestrictionArgs(
                 restriction=[opsgenie.ScheduleRotationTimeRestrictionRestrictionArgs(
                     end_hour=10,
@@ -350,15 +350,15 @@
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.ScheduleRotation("test",
             end_date="2019-06-20T17:30:00Z",
             length=6,
             participants=[opsgenie.ScheduleRotationParticipantArgs(
-                id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                id=opsgenie_user["test"]["id"],
                 type="user",
             )],
             schedule_id=opsgenie_schedule["test"]["id"],
             start_date="2019-06-18T17:00:00Z",
             time_restrictions=[opsgenie.ScheduleRotationTimeRestrictionArgs(
                 restriction=[opsgenie.ScheduleRotationTimeRestrictionRestrictionArgs(
                     end_hour=10,
```

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/service.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/service_incident_rule.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/service_incident_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/team.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/team_routing_rule.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/team_routing_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/user.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie/user_contact.py` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/user_contact.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie.egg-info/PKG-INFO` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-opsgenie
-Version: 1.3.0a1687672889
+Version: 1.3.0a1687799894
 Summary: A Pulumi package for creating and managing opsgenie cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-opsgenie
 Keywords: pulumi opsgenie
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_opsgenie-1.3.0a1687672889/pulumi_opsgenie.egg-info/SOURCES.txt` & `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687672889/setup.py` & `pulumi_opsgenie-1.3.0a1687799894/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.3.0a1687672889"
-PLUGIN_VERSION = "1.3.0-alpha.1687672889+d9f00119"
+VERSION = "1.3.0a1687799894"
+PLUGIN_VERSION = "1.3.0-alpha.1687799894+4e4f7c35"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'opsgenie', PLUGIN_VERSION])
         except OSError as error:
```

