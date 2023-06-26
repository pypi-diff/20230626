# Comparing `tmp/mypy-boto3-connect-1.26.79.tar.gz` & `tmp/mypy-boto3-connect-1.26.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connect-1.26.79.tar", last modified: Fri Feb 24 21:22:49 2023, max compression
+gzip compressed data, was "mypy-boto3-connect-1.26.88.tar", last modified: Thu Mar  9 20:38:41 2023, max compression
```

## Comparing `mypy-boto3-connect-1.26.79.tar` & `mypy-boto3-connect-1.26.88.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.733199 mypy-boto3-connect-1.26.79/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-24 21:21:57.000000 mypy-boto3-connect-1.26.79/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    39436 2023-02-24 21:22:49.733199 mypy-boto3-connect-1.26.79/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37949 2023-02-24 21:21:57.000000 mypy-boto3-connect-1.26.79/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.721198 mypy-boto3-connect-1.26.79/mypy_boto3_connect/
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-02-24 21:21:57.000000 mypy-boto3-connect-1.26.79/mypy_boto3_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-02-24 21:21:57.000000 mypy-boto3-connect-1.26.79/mypy_boto3_connect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-02-24 21:21:57.000000 mypy-boto3-connect-1.26.79/mypy_boto3_connect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   129963 2023-02-24 21:21:59.000000 mypy-boto3-connect-1.26.79/mypy_boto3_connect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   129749 2023-02-24 21:21:58.000000 mypy-boto3-connect-1.26.79/mypy_boto3_connect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-02-24 21:22:00.000000 mypy-boto3-connect-1.26.79/mypy_boto3_connect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    22658 2023-02-24 21:21:59.000000 mypy-boto3-connect-1.26.79/mypy_boto3_connect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    45555 2023-02-24 21:21:59.000000 mypy-boto3-connect-1.26.79/mypy_boto3_connect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    45515 2023-02-24 21:21:59.000000 mypy-boto3-connect-1.26.79/mypy_boto3_connect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 21:21:57.000000 mypy-boto3-connect-1.26.79/mypy_boto3_connect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   173899 2023-02-24 21:22:05.000000 mypy-boto3-connect-1.26.79/mypy_boto3_connect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   173646 2023-02-24 21:22:03.000000 mypy-boto3-connect-1.26.79/mypy_boto3_connect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-24 21:21:57.000000 mypy-boto3-connect-1.26.79/mypy_boto3_connect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.733199 mypy-boto3-connect-1.26.79/mypy_boto3_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    39436 2023-02-24 21:22:49.000000 mypy-boto3-connect-1.26.79/mypy_boto3_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-02-24 21:22:49.000000 mypy-boto3-connect-1.26.79/mypy_boto3_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 21:22:49.000000 mypy-boto3-connect-1.26.79/mypy_boto3_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 21:22:49.000000 mypy-boto3-connect-1.26.79/mypy_boto3_connect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-24 21:22:49.000000 mypy-boto3-connect-1.26.79/mypy_boto3_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-24 21:22:49.000000 mypy-boto3-connect-1.26.79/mypy_boto3_connect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 21:22:49.733199 mypy-boto3-connect-1.26.79/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-02-24 21:21:57.000000 mypy-boto3-connect-1.26.79/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:41.666347 mypy-boto3-connect-1.26.88/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-09 20:36:01.000000 mypy-boto3-connect-1.26.88/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    39659 2023-03-09 20:38:41.666347 mypy-boto3-connect-1.26.88/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    38172 2023-03-09 20:36:01.000000 mypy-boto3-connect-1.26.88/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:41.666347 mypy-boto3-connect-1.26.88/mypy_boto3_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-03-09 20:36:01.000000 mypy-boto3-connect-1.26.88/mypy_boto3_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-03-09 20:36:01.000000 mypy-boto3-connect-1.26.88/mypy_boto3_connect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-09 20:36:01.000000 mypy-boto3-connect-1.26.88/mypy_boto3_connect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130813 2023-03-09 20:36:03.000000 mypy-boto3-connect-1.26.88/mypy_boto3_connect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130598 2023-03-09 20:36:02.000000 mypy-boto3-connect-1.26.88/mypy_boto3_connect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22683 2023-03-09 20:36:04.000000 mypy-boto3-connect-1.26.88/mypy_boto3_connect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22681 2023-03-09 20:36:04.000000 mypy-boto3-connect-1.26.88/mypy_boto3_connect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    45555 2023-03-09 20:36:03.000000 mypy-boto3-connect-1.26.88/mypy_boto3_connect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45515 2023-03-09 20:36:03.000000 mypy-boto3-connect-1.26.88/mypy_boto3_connect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 20:36:01.000000 mypy-boto3-connect-1.26.88/mypy_boto3_connect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   176117 2023-03-09 20:36:09.000000 mypy-boto3-connect-1.26.88/mypy_boto3_connect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   175862 2023-03-09 20:36:06.000000 mypy-boto3-connect-1.26.88/mypy_boto3_connect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-09 20:36:01.000000 mypy-boto3-connect-1.26.88/mypy_boto3_connect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:41.666347 mypy-boto3-connect-1.26.88/mypy_boto3_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    39659 2023-03-09 20:38:41.000000 mypy-boto3-connect-1.26.88/mypy_boto3_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-09 20:38:41.000000 mypy-boto3-connect-1.26.88/mypy_boto3_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 20:38:41.000000 mypy-boto3-connect-1.26.88/mypy_boto3_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 20:38:41.000000 mypy-boto3-connect-1.26.88/mypy_boto3_connect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-09 20:38:41.000000 mypy-boto3-connect-1.26.88/mypy_boto3_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-09 20:38:41.000000 mypy-boto3-connect-1.26.88/mypy_boto3_connect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 20:38:41.666347 mypy-boto3-connect-1.26.88/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-03-09 20:36:01.000000 mypy-boto3-connect-1.26.88/setup.py
```

### Comparing `mypy-boto3-connect-1.26.79/LICENSE` & `mypy-boto3-connect-1.26.88/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.26.79/PKG-INFO` & `mypy-boto3-connect-1.26.88/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connect
-Version: 1.26.79
-Summary: Type annotations for boto3.Connect 1.26.79 service generated with mypy-boto3-builder 7.12.4
+Version: 1.26.88
+Summary: Type annotations for boto3.Connect 1.26.88 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connect?color=blue)](https://pypistats.org/packages/mypy-boto3-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Connect 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[boto3.Connect 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -636,14 +636,15 @@
     RoutingProfileQueueReferenceTypeDef,
     DisassociateSecurityKeyRequestRequestTypeDef,
     DismissUserContactRequestRequestTypeDef,
     DistributionTypeDef,
     EmailReferenceTypeDef,
     EncryptionConfigTypeDef,
     EventBridgeActionDefinitionTypeDef,
+    FilterV2TypeDef,
     FiltersTypeDef,
     GetContactAttributesRequestRequestTypeDef,
     GetFederationTokenRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     GetTaskTemplateRequestRequestTypeDef,
     GetTrafficDistributionRequestRequestTypeDef,
     HierarchyGroupConditionTypeDef,
@@ -701,14 +702,16 @@
     ListTrafficDistributionGroupsRequestRequestTypeDef,
     TrafficDistributionGroupSummaryTypeDef,
     ListUseCasesRequestRequestTypeDef,
     UseCaseTypeDef,
     ListUserHierarchyGroupsRequestRequestTypeDef,
     ListUsersRequestRequestTypeDef,
     UserSummaryTypeDef,
+    MetricFilterV2TypeDef,
+    ThresholdV2TypeDef,
     MonitorContactRequestRequestTypeDef,
     NotificationRecipientTypeTypeDef,
     NumberReferenceTypeDef,
     ParticipantDetailsTypeDef,
     ParticipantTimerValueTypeDef,
     PersistentChatTypeDef,
     PhoneNumberQuickConnectConfigTypeDef,
@@ -896,14 +899,15 @@
     ListRoutingProfilesResponseTypeDef,
     ListSecurityKeysResponseTypeDef,
     ListSecurityProfilesResponseTypeDef,
     ListTaskTemplatesResponseTypeDef,
     ListTrafficDistributionGroupsResponseTypeDef,
     ListUseCasesResponseTypeDef,
     ListUsersResponseTypeDef,
+    MetricV2TypeDef,
     SendNotificationActionDefinitionTypeDef,
     ParticipantTimerConfigurationTypeDef,
     StartChatContactRequestRequestTypeDef,
     QueueSearchCriteriaTypeDef,
     RoutingProfileSearchCriteriaTypeDef,
     SecurityProfileSearchCriteriaTypeDef,
     UserSearchCriteriaTypeDef,
@@ -946,14 +950,16 @@
     HistoricalMetricDataTypeDef,
     CreateHoursOfOperationRequestRequestTypeDef,
     HoursOfOperationTypeDef,
     UpdateHoursOfOperationRequestRequestTypeDef,
     DescribeInstanceResponseTypeDef,
     TaskTemplateConstraintsTypeDef,
     TaskTemplateDefaultsTypeDef,
+    GetMetricDataV2RequestRequestTypeDef,
+    MetricDataV2TypeDef,
     ChatParticipantRoleConfigTypeDef,
     CreateQuickConnectRequestRequestTypeDef,
     QuickConnectTypeDef,
     UpdateQuickConnectConfigRequestRequestTypeDef,
     ListContactReferencesResponseTypeDef,
     RuleActionTypeDef,
     SearchUsersResponseTypeDef,
@@ -974,20 +980,22 @@
     DescribeUserHierarchyGroupResponseTypeDef,
     HistoricalMetricResultTypeDef,
     DescribeHoursOfOperationResponseTypeDef,
     CreateTaskTemplateRequestRequestTypeDef,
     GetTaskTemplateResponseTypeDef,
     UpdateTaskTemplateRequestRequestTypeDef,
     UpdateTaskTemplateResponseTypeDef,
+    MetricResultV2TypeDef,
     UpdateParticipantRoleConfigChannelInfoTypeDef,
     DescribeQuickConnectResponseTypeDef,
     CreateRuleRequestRequestTypeDef,
     RuleTypeDef,
     UpdateRuleRequestRequestTypeDef,
     GetMetricDataResponseTypeDef,
+    GetMetricDataV2ResponseTypeDef,
     UpdateParticipantRoleConfigRequestRequestTypeDef,
     DescribeRuleResponseTypeDef,
 )
 
 
 def get_structure() -> ActionSummaryTypeDef:
     return {...}
```

### Comparing `mypy-boto3-connect-1.26.79/README.md` & `mypy-boto3-connect-1.26.88/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connect?color=blue)](https://pypistats.org/packages/mypy-boto3-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Connect 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[boto3.Connect 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -604,14 +604,15 @@
     RoutingProfileQueueReferenceTypeDef,
     DisassociateSecurityKeyRequestRequestTypeDef,
     DismissUserContactRequestRequestTypeDef,
     DistributionTypeDef,
     EmailReferenceTypeDef,
     EncryptionConfigTypeDef,
     EventBridgeActionDefinitionTypeDef,
+    FilterV2TypeDef,
     FiltersTypeDef,
     GetContactAttributesRequestRequestTypeDef,
     GetFederationTokenRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     GetTaskTemplateRequestRequestTypeDef,
     GetTrafficDistributionRequestRequestTypeDef,
     HierarchyGroupConditionTypeDef,
@@ -669,14 +670,16 @@
     ListTrafficDistributionGroupsRequestRequestTypeDef,
     TrafficDistributionGroupSummaryTypeDef,
     ListUseCasesRequestRequestTypeDef,
     UseCaseTypeDef,
     ListUserHierarchyGroupsRequestRequestTypeDef,
     ListUsersRequestRequestTypeDef,
     UserSummaryTypeDef,
+    MetricFilterV2TypeDef,
+    ThresholdV2TypeDef,
     MonitorContactRequestRequestTypeDef,
     NotificationRecipientTypeTypeDef,
     NumberReferenceTypeDef,
     ParticipantDetailsTypeDef,
     ParticipantTimerValueTypeDef,
     PersistentChatTypeDef,
     PhoneNumberQuickConnectConfigTypeDef,
@@ -864,14 +867,15 @@
     ListRoutingProfilesResponseTypeDef,
     ListSecurityKeysResponseTypeDef,
     ListSecurityProfilesResponseTypeDef,
     ListTaskTemplatesResponseTypeDef,
     ListTrafficDistributionGroupsResponseTypeDef,
     ListUseCasesResponseTypeDef,
     ListUsersResponseTypeDef,
+    MetricV2TypeDef,
     SendNotificationActionDefinitionTypeDef,
     ParticipantTimerConfigurationTypeDef,
     StartChatContactRequestRequestTypeDef,
     QueueSearchCriteriaTypeDef,
     RoutingProfileSearchCriteriaTypeDef,
     SecurityProfileSearchCriteriaTypeDef,
     UserSearchCriteriaTypeDef,
@@ -914,14 +918,16 @@
     HistoricalMetricDataTypeDef,
     CreateHoursOfOperationRequestRequestTypeDef,
     HoursOfOperationTypeDef,
     UpdateHoursOfOperationRequestRequestTypeDef,
     DescribeInstanceResponseTypeDef,
     TaskTemplateConstraintsTypeDef,
     TaskTemplateDefaultsTypeDef,
+    GetMetricDataV2RequestRequestTypeDef,
+    MetricDataV2TypeDef,
     ChatParticipantRoleConfigTypeDef,
     CreateQuickConnectRequestRequestTypeDef,
     QuickConnectTypeDef,
     UpdateQuickConnectConfigRequestRequestTypeDef,
     ListContactReferencesResponseTypeDef,
     RuleActionTypeDef,
     SearchUsersResponseTypeDef,
@@ -942,20 +948,22 @@
     DescribeUserHierarchyGroupResponseTypeDef,
     HistoricalMetricResultTypeDef,
     DescribeHoursOfOperationResponseTypeDef,
     CreateTaskTemplateRequestRequestTypeDef,
     GetTaskTemplateResponseTypeDef,
     UpdateTaskTemplateRequestRequestTypeDef,
     UpdateTaskTemplateResponseTypeDef,
+    MetricResultV2TypeDef,
     UpdateParticipantRoleConfigChannelInfoTypeDef,
     DescribeQuickConnectResponseTypeDef,
     CreateRuleRequestRequestTypeDef,
     RuleTypeDef,
     UpdateRuleRequestRequestTypeDef,
     GetMetricDataResponseTypeDef,
+    GetMetricDataV2ResponseTypeDef,
     UpdateParticipantRoleConfigRequestRequestTypeDef,
     DescribeRuleResponseTypeDef,
 )
 
 
 def get_structure() -> ActionSummaryTypeDef:
     return {...}
```

### Comparing `mypy-boto3-connect-1.26.79/mypy_boto3_connect/__init__.py` & `mypy-boto3-connect-1.26.88/mypy_boto3_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.26.79/mypy_boto3_connect/__init__.pyi` & `mypy-boto3-connect-1.26.88/mypy_boto3_connect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.26.79/mypy_boto3_connect/__main__.py` & `mypy-boto3-connect-1.26.88/mypy_boto3_connect/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Connect 1.26.79\nVersion:         1.26.79\nBuilder version:"
-        " 7.12.4\nDocs:           "
+        "Type annotations for boto3.Connect 1.26.88\nVersion:         1.26.88\nBuilder version:"
+        " 7.12.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.79")
+    print("1.26.88")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-connect-1.26.79/mypy_boto3_connect/client.py` & `mypy-boto3-connect-1.26.88/mypy_boto3_connect/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,19 +131,21 @@
     DescribeTrafficDistributionGroupResponseTypeDef,
     DescribeUserHierarchyGroupResponseTypeDef,
     DescribeUserHierarchyStructureResponseTypeDef,
     DescribeUserResponseTypeDef,
     DescribeVocabularyResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     FiltersTypeDef,
+    FilterV2TypeDef,
     GetContactAttributesResponseTypeDef,
     GetCurrentMetricDataResponseTypeDef,
     GetCurrentUserDataResponseTypeDef,
     GetFederationTokenResponseTypeDef,
     GetMetricDataResponseTypeDef,
+    GetMetricDataV2ResponseTypeDef,
     GetTaskTemplateResponseTypeDef,
     GetTrafficDistributionResponseTypeDef,
     HierarchyStructureUpdateTypeDef,
     HistoricalMetricTypeDef,
     HoursOfOperationConfigTypeDef,
     InstanceStorageConfigTypeDef,
     LexBotTypeDef,
@@ -177,14 +179,15 @@
     ListTagsForResourceResponseTypeDef,
     ListTaskTemplatesResponseTypeDef,
     ListTrafficDistributionGroupsResponseTypeDef,
     ListUseCasesResponseTypeDef,
     ListUserHierarchyGroupsResponseTypeDef,
     ListUsersResponseTypeDef,
     MediaConcurrencyTypeDef,
+    MetricV2TypeDef,
     MonitorContactResponseTypeDef,
     OutboundCallerConfigTypeDef,
     ParticipantDetailsTypeDef,
     PersistentChatTypeDef,
     QueueSearchCriteriaTypeDef,
     QueueSearchFilterTypeDef,
     QuickConnectConfigTypeDef,
@@ -1215,14 +1218,33 @@
         """
         Gets historical metric data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_metric_data)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_metric_data)
         """
 
+    def get_metric_data_v2(
+        self,
+        *,
+        ResourceArn: str,
+        StartTime: Union[datetime, str],
+        EndTime: Union[datetime, str],
+        Filters: Sequence[FilterV2TypeDef],
+        Metrics: Sequence[MetricV2TypeDef],
+        Groupings: Sequence[str] = ...,
+        NextToken: str = ...,
+        MaxResults: int = ...
+    ) -> GetMetricDataV2ResponseTypeDef:
+        """
+        Gets metric data from the specified Amazon Connect instance.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_metric_data_v2)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_metric_data_v2)
+        """
+
     def get_task_template(
         self, *, InstanceId: str, TaskTemplateId: str, SnapshotVersion: str = ...
     ) -> GetTaskTemplateResponseTypeDef:
         """
         Gets details about a specific task template in the specified Amazon Connect
         instance.
```

### Comparing `mypy-boto3-connect-1.26.79/mypy_boto3_connect/client.pyi` & `mypy-boto3-connect-1.26.88/mypy_boto3_connect/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -131,19 +131,21 @@
     DescribeTrafficDistributionGroupResponseTypeDef,
     DescribeUserHierarchyGroupResponseTypeDef,
     DescribeUserHierarchyStructureResponseTypeDef,
     DescribeUserResponseTypeDef,
     DescribeVocabularyResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     FiltersTypeDef,
+    FilterV2TypeDef,
     GetContactAttributesResponseTypeDef,
     GetCurrentMetricDataResponseTypeDef,
     GetCurrentUserDataResponseTypeDef,
     GetFederationTokenResponseTypeDef,
     GetMetricDataResponseTypeDef,
+    GetMetricDataV2ResponseTypeDef,
     GetTaskTemplateResponseTypeDef,
     GetTrafficDistributionResponseTypeDef,
     HierarchyStructureUpdateTypeDef,
     HistoricalMetricTypeDef,
     HoursOfOperationConfigTypeDef,
     InstanceStorageConfigTypeDef,
     LexBotTypeDef,
@@ -177,14 +179,15 @@
     ListTagsForResourceResponseTypeDef,
     ListTaskTemplatesResponseTypeDef,
     ListTrafficDistributionGroupsResponseTypeDef,
     ListUseCasesResponseTypeDef,
     ListUserHierarchyGroupsResponseTypeDef,
     ListUsersResponseTypeDef,
     MediaConcurrencyTypeDef,
+    MetricV2TypeDef,
     MonitorContactResponseTypeDef,
     OutboundCallerConfigTypeDef,
     ParticipantDetailsTypeDef,
     PersistentChatTypeDef,
     QueueSearchCriteriaTypeDef,
     QueueSearchFilterTypeDef,
     QuickConnectConfigTypeDef,
@@ -1131,14 +1134,32 @@
     ) -> GetMetricDataResponseTypeDef:
         """
         Gets historical metric data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_metric_data)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_metric_data)
         """
+    def get_metric_data_v2(
+        self,
+        *,
+        ResourceArn: str,
+        StartTime: Union[datetime, str],
+        EndTime: Union[datetime, str],
+        Filters: Sequence[FilterV2TypeDef],
+        Metrics: Sequence[MetricV2TypeDef],
+        Groupings: Sequence[str] = ...,
+        NextToken: str = ...,
+        MaxResults: int = ...
+    ) -> GetMetricDataV2ResponseTypeDef:
+        """
+        Gets metric data from the specified Amazon Connect instance.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_metric_data_v2)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_metric_data_v2)
+        """
     def get_task_template(
         self, *, InstanceId: str, TaskTemplateId: str, SnapshotVersion: str = ...
     ) -> GetTaskTemplateResponseTypeDef:
         """
         Gets details about a specific task template in the specified Amazon Connect
         instance.
```

### Comparing `mypy-boto3-connect-1.26.79/mypy_boto3_connect/literals.py` & `mypy-boto3-connect-1.26.88/mypy_boto3_connect/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -741,14 +741,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
```

### Comparing `mypy-boto3-connect-1.26.79/mypy_boto3_connect/literals.pyi` & `mypy-boto3-connect-1.26.88/mypy_boto3_connect/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -739,14 +739,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
```

### Comparing `mypy-boto3-connect-1.26.79/mypy_boto3_connect/paginator.py` & `mypy-boto3-connect-1.26.88/mypy_boto3_connect/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.26.79/mypy_boto3_connect/paginator.pyi` & `mypy-boto3-connect-1.26.88/mypy_boto3_connect/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.26.79/mypy_boto3_connect/type_defs.py` & `mypy-boto3-connect-1.26.88/mypy_boto3_connect/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,15 @@
     "RoutingProfileQueueReferenceTypeDef",
     "DisassociateSecurityKeyRequestRequestTypeDef",
     "DismissUserContactRequestRequestTypeDef",
     "DistributionTypeDef",
     "EmailReferenceTypeDef",
     "EncryptionConfigTypeDef",
     "EventBridgeActionDefinitionTypeDef",
+    "FilterV2TypeDef",
     "FiltersTypeDef",
     "GetContactAttributesRequestRequestTypeDef",
     "GetFederationTokenRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetTaskTemplateRequestRequestTypeDef",
     "GetTrafficDistributionRequestRequestTypeDef",
     "HierarchyGroupConditionTypeDef",
@@ -241,14 +242,16 @@
     "ListTrafficDistributionGroupsRequestRequestTypeDef",
     "TrafficDistributionGroupSummaryTypeDef",
     "ListUseCasesRequestRequestTypeDef",
     "UseCaseTypeDef",
     "ListUserHierarchyGroupsRequestRequestTypeDef",
     "ListUsersRequestRequestTypeDef",
     "UserSummaryTypeDef",
+    "MetricFilterV2TypeDef",
+    "ThresholdV2TypeDef",
     "MonitorContactRequestRequestTypeDef",
     "NotificationRecipientTypeTypeDef",
     "NumberReferenceTypeDef",
     "ParticipantDetailsTypeDef",
     "ParticipantTimerValueTypeDef",
     "PersistentChatTypeDef",
     "PhoneNumberQuickConnectConfigTypeDef",
@@ -436,14 +439,15 @@
     "ListRoutingProfilesResponseTypeDef",
     "ListSecurityKeysResponseTypeDef",
     "ListSecurityProfilesResponseTypeDef",
     "ListTaskTemplatesResponseTypeDef",
     "ListTrafficDistributionGroupsResponseTypeDef",
     "ListUseCasesResponseTypeDef",
     "ListUsersResponseTypeDef",
+    "MetricV2TypeDef",
     "SendNotificationActionDefinitionTypeDef",
     "ParticipantTimerConfigurationTypeDef",
     "StartChatContactRequestRequestTypeDef",
     "QueueSearchCriteriaTypeDef",
     "RoutingProfileSearchCriteriaTypeDef",
     "SecurityProfileSearchCriteriaTypeDef",
     "UserSearchCriteriaTypeDef",
@@ -486,14 +490,16 @@
     "HistoricalMetricDataTypeDef",
     "CreateHoursOfOperationRequestRequestTypeDef",
     "HoursOfOperationTypeDef",
     "UpdateHoursOfOperationRequestRequestTypeDef",
     "DescribeInstanceResponseTypeDef",
     "TaskTemplateConstraintsTypeDef",
     "TaskTemplateDefaultsTypeDef",
+    "GetMetricDataV2RequestRequestTypeDef",
+    "MetricDataV2TypeDef",
     "ChatParticipantRoleConfigTypeDef",
     "CreateQuickConnectRequestRequestTypeDef",
     "QuickConnectTypeDef",
     "UpdateQuickConnectConfigRequestRequestTypeDef",
     "ListContactReferencesResponseTypeDef",
     "RuleActionTypeDef",
     "SearchUsersResponseTypeDef",
@@ -514,20 +520,22 @@
     "DescribeUserHierarchyGroupResponseTypeDef",
     "HistoricalMetricResultTypeDef",
     "DescribeHoursOfOperationResponseTypeDef",
     "CreateTaskTemplateRequestRequestTypeDef",
     "GetTaskTemplateResponseTypeDef",
     "UpdateTaskTemplateRequestRequestTypeDef",
     "UpdateTaskTemplateResponseTypeDef",
+    "MetricResultV2TypeDef",
     "UpdateParticipantRoleConfigChannelInfoTypeDef",
     "DescribeQuickConnectResponseTypeDef",
     "CreateRuleRequestRequestTypeDef",
     "RuleTypeDef",
     "UpdateRuleRequestRequestTypeDef",
     "GetMetricDataResponseTypeDef",
+    "GetMetricDataV2ResponseTypeDef",
     "UpdateParticipantRoleConfigRequestRequestTypeDef",
     "DescribeRuleResponseTypeDef",
 )
 
 ActionSummaryTypeDef = TypedDict(
     "ActionSummaryTypeDef",
     {
@@ -1654,14 +1662,23 @@
 EventBridgeActionDefinitionTypeDef = TypedDict(
     "EventBridgeActionDefinitionTypeDef",
     {
         "Name": str,
     },
 )
 
+FilterV2TypeDef = TypedDict(
+    "FilterV2TypeDef",
+    {
+        "FilterKey": str,
+        "FilterValues": Sequence[str],
+    },
+    total=False,
+)
+
 FiltersTypeDef = TypedDict(
     "FiltersTypeDef",
     {
         "Queues": Sequence[str],
         "Channels": Sequence[ChannelType],
         "RoutingProfiles": Sequence[str],
     },
@@ -2686,14 +2703,32 @@
         "Id": str,
         "Arn": str,
         "Username": str,
     },
     total=False,
 )
 
+MetricFilterV2TypeDef = TypedDict(
+    "MetricFilterV2TypeDef",
+    {
+        "MetricFilterKey": str,
+        "MetricFilterValues": Sequence[str],
+    },
+    total=False,
+)
+
+ThresholdV2TypeDef = TypedDict(
+    "ThresholdV2TypeDef",
+    {
+        "Comparison": str,
+        "ThresholdValue": float,
+    },
+    total=False,
+)
+
 _RequiredMonitorContactRequestRequestTypeDef = TypedDict(
     "_RequiredMonitorContactRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
         "UserId": str,
     },
@@ -5322,14 +5357,24 @@
     {
         "UserSummaryList": List[UserSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+MetricV2TypeDef = TypedDict(
+    "MetricV2TypeDef",
+    {
+        "Name": str,
+        "Threshold": Sequence[ThresholdV2TypeDef],
+        "MetricFilters": Sequence[MetricFilterV2TypeDef],
+    },
+    total=False,
+)
+
 _RequiredSendNotificationActionDefinitionTypeDef = TypedDict(
     "_RequiredSendNotificationActionDefinitionTypeDef",
     {
         "DeliveryMethod": Literal["EMAIL"],
         "Content": str,
         "ContentType": Literal["PLAIN_TEXT"],
         "Recipient": NotificationRecipientTypeTypeDef,
@@ -6031,14 +6076,50 @@
     "TaskTemplateDefaultsTypeDef",
     {
         "DefaultFieldValues": Sequence[TaskTemplateDefaultFieldValueTypeDef],
     },
     total=False,
 )
 
+_RequiredGetMetricDataV2RequestRequestTypeDef = TypedDict(
+    "_RequiredGetMetricDataV2RequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Filters": Sequence[FilterV2TypeDef],
+        "Metrics": Sequence[MetricV2TypeDef],
+    },
+)
+_OptionalGetMetricDataV2RequestRequestTypeDef = TypedDict(
+    "_OptionalGetMetricDataV2RequestRequestTypeDef",
+    {
+        "Groupings": Sequence[str],
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class GetMetricDataV2RequestRequestTypeDef(
+    _RequiredGetMetricDataV2RequestRequestTypeDef, _OptionalGetMetricDataV2RequestRequestTypeDef
+):
+    pass
+
+
+MetricDataV2TypeDef = TypedDict(
+    "MetricDataV2TypeDef",
+    {
+        "Metric": MetricV2TypeDef,
+        "Value": float,
+    },
+    total=False,
+)
+
 ChatParticipantRoleConfigTypeDef = TypedDict(
     "ChatParticipantRoleConfigTypeDef",
     {
         "ParticipantTimerConfigList": Sequence[ParticipantTimerConfigurationTypeDef],
     },
 )
 
@@ -6474,14 +6555,23 @@
         "Status": TaskTemplateStatusType,
         "LastModifiedTime": datetime,
         "CreatedTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+MetricResultV2TypeDef = TypedDict(
+    "MetricResultV2TypeDef",
+    {
+        "Dimensions": Dict[str, str],
+        "Collections": List[MetricDataV2TypeDef],
+    },
+    total=False,
+)
+
 UpdateParticipantRoleConfigChannelInfoTypeDef = TypedDict(
     "UpdateParticipantRoleConfigChannelInfoTypeDef",
     {
         "Chat": ChatParticipantRoleConfigTypeDef,
     },
     total=False,
 )
@@ -6565,14 +6655,23 @@
     {
         "NextToken": str,
         "MetricResults": List[HistoricalMetricResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetMetricDataV2ResponseTypeDef = TypedDict(
+    "GetMetricDataV2ResponseTypeDef",
+    {
+        "NextToken": str,
+        "MetricResults": List[MetricResultV2TypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateParticipantRoleConfigRequestRequestTypeDef = TypedDict(
     "UpdateParticipantRoleConfigRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
         "ChannelConfiguration": UpdateParticipantRoleConfigChannelInfoTypeDef,
     },
```

### Comparing `mypy-boto3-connect-1.26.79/mypy_boto3_connect/type_defs.pyi` & `mypy-boto3-connect-1.26.88/mypy_boto3_connect/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -175,14 +175,15 @@
     "RoutingProfileQueueReferenceTypeDef",
     "DisassociateSecurityKeyRequestRequestTypeDef",
     "DismissUserContactRequestRequestTypeDef",
     "DistributionTypeDef",
     "EmailReferenceTypeDef",
     "EncryptionConfigTypeDef",
     "EventBridgeActionDefinitionTypeDef",
+    "FilterV2TypeDef",
     "FiltersTypeDef",
     "GetContactAttributesRequestRequestTypeDef",
     "GetFederationTokenRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetTaskTemplateRequestRequestTypeDef",
     "GetTrafficDistributionRequestRequestTypeDef",
     "HierarchyGroupConditionTypeDef",
@@ -240,14 +241,16 @@
     "ListTrafficDistributionGroupsRequestRequestTypeDef",
     "TrafficDistributionGroupSummaryTypeDef",
     "ListUseCasesRequestRequestTypeDef",
     "UseCaseTypeDef",
     "ListUserHierarchyGroupsRequestRequestTypeDef",
     "ListUsersRequestRequestTypeDef",
     "UserSummaryTypeDef",
+    "MetricFilterV2TypeDef",
+    "ThresholdV2TypeDef",
     "MonitorContactRequestRequestTypeDef",
     "NotificationRecipientTypeTypeDef",
     "NumberReferenceTypeDef",
     "ParticipantDetailsTypeDef",
     "ParticipantTimerValueTypeDef",
     "PersistentChatTypeDef",
     "PhoneNumberQuickConnectConfigTypeDef",
@@ -435,14 +438,15 @@
     "ListRoutingProfilesResponseTypeDef",
     "ListSecurityKeysResponseTypeDef",
     "ListSecurityProfilesResponseTypeDef",
     "ListTaskTemplatesResponseTypeDef",
     "ListTrafficDistributionGroupsResponseTypeDef",
     "ListUseCasesResponseTypeDef",
     "ListUsersResponseTypeDef",
+    "MetricV2TypeDef",
     "SendNotificationActionDefinitionTypeDef",
     "ParticipantTimerConfigurationTypeDef",
     "StartChatContactRequestRequestTypeDef",
     "QueueSearchCriteriaTypeDef",
     "RoutingProfileSearchCriteriaTypeDef",
     "SecurityProfileSearchCriteriaTypeDef",
     "UserSearchCriteriaTypeDef",
@@ -485,14 +489,16 @@
     "HistoricalMetricDataTypeDef",
     "CreateHoursOfOperationRequestRequestTypeDef",
     "HoursOfOperationTypeDef",
     "UpdateHoursOfOperationRequestRequestTypeDef",
     "DescribeInstanceResponseTypeDef",
     "TaskTemplateConstraintsTypeDef",
     "TaskTemplateDefaultsTypeDef",
+    "GetMetricDataV2RequestRequestTypeDef",
+    "MetricDataV2TypeDef",
     "ChatParticipantRoleConfigTypeDef",
     "CreateQuickConnectRequestRequestTypeDef",
     "QuickConnectTypeDef",
     "UpdateQuickConnectConfigRequestRequestTypeDef",
     "ListContactReferencesResponseTypeDef",
     "RuleActionTypeDef",
     "SearchUsersResponseTypeDef",
@@ -513,20 +519,22 @@
     "DescribeUserHierarchyGroupResponseTypeDef",
     "HistoricalMetricResultTypeDef",
     "DescribeHoursOfOperationResponseTypeDef",
     "CreateTaskTemplateRequestRequestTypeDef",
     "GetTaskTemplateResponseTypeDef",
     "UpdateTaskTemplateRequestRequestTypeDef",
     "UpdateTaskTemplateResponseTypeDef",
+    "MetricResultV2TypeDef",
     "UpdateParticipantRoleConfigChannelInfoTypeDef",
     "DescribeQuickConnectResponseTypeDef",
     "CreateRuleRequestRequestTypeDef",
     "RuleTypeDef",
     "UpdateRuleRequestRequestTypeDef",
     "GetMetricDataResponseTypeDef",
+    "GetMetricDataV2ResponseTypeDef",
     "UpdateParticipantRoleConfigRequestRequestTypeDef",
     "DescribeRuleResponseTypeDef",
 )
 
 ActionSummaryTypeDef = TypedDict(
     "ActionSummaryTypeDef",
     {
@@ -1623,14 +1631,23 @@
 EventBridgeActionDefinitionTypeDef = TypedDict(
     "EventBridgeActionDefinitionTypeDef",
     {
         "Name": str,
     },
 )
 
+FilterV2TypeDef = TypedDict(
+    "FilterV2TypeDef",
+    {
+        "FilterKey": str,
+        "FilterValues": Sequence[str],
+    },
+    total=False,
+)
+
 FiltersTypeDef = TypedDict(
     "FiltersTypeDef",
     {
         "Queues": Sequence[str],
         "Channels": Sequence[ChannelType],
         "RoutingProfiles": Sequence[str],
     },
@@ -2597,14 +2614,32 @@
         "Id": str,
         "Arn": str,
         "Username": str,
     },
     total=False,
 )
 
+MetricFilterV2TypeDef = TypedDict(
+    "MetricFilterV2TypeDef",
+    {
+        "MetricFilterKey": str,
+        "MetricFilterValues": Sequence[str],
+    },
+    total=False,
+)
+
+ThresholdV2TypeDef = TypedDict(
+    "ThresholdV2TypeDef",
+    {
+        "Comparison": str,
+        "ThresholdValue": float,
+    },
+    total=False,
+)
+
 _RequiredMonitorContactRequestRequestTypeDef = TypedDict(
     "_RequiredMonitorContactRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
         "UserId": str,
     },
@@ -5121,14 +5156,24 @@
     {
         "UserSummaryList": List[UserSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+MetricV2TypeDef = TypedDict(
+    "MetricV2TypeDef",
+    {
+        "Name": str,
+        "Threshold": Sequence[ThresholdV2TypeDef],
+        "MetricFilters": Sequence[MetricFilterV2TypeDef],
+    },
+    total=False,
+)
+
 _RequiredSendNotificationActionDefinitionTypeDef = TypedDict(
     "_RequiredSendNotificationActionDefinitionTypeDef",
     {
         "DeliveryMethod": Literal["EMAIL"],
         "Content": str,
         "ContentType": Literal["PLAIN_TEXT"],
         "Recipient": NotificationRecipientTypeTypeDef,
@@ -5802,14 +5847,48 @@
     "TaskTemplateDefaultsTypeDef",
     {
         "DefaultFieldValues": Sequence[TaskTemplateDefaultFieldValueTypeDef],
     },
     total=False,
 )
 
+_RequiredGetMetricDataV2RequestRequestTypeDef = TypedDict(
+    "_RequiredGetMetricDataV2RequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Filters": Sequence[FilterV2TypeDef],
+        "Metrics": Sequence[MetricV2TypeDef],
+    },
+)
+_OptionalGetMetricDataV2RequestRequestTypeDef = TypedDict(
+    "_OptionalGetMetricDataV2RequestRequestTypeDef",
+    {
+        "Groupings": Sequence[str],
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class GetMetricDataV2RequestRequestTypeDef(
+    _RequiredGetMetricDataV2RequestRequestTypeDef, _OptionalGetMetricDataV2RequestRequestTypeDef
+):
+    pass
+
+MetricDataV2TypeDef = TypedDict(
+    "MetricDataV2TypeDef",
+    {
+        "Metric": MetricV2TypeDef,
+        "Value": float,
+    },
+    total=False,
+)
+
 ChatParticipantRoleConfigTypeDef = TypedDict(
     "ChatParticipantRoleConfigTypeDef",
     {
         "ParticipantTimerConfigList": Sequence[ParticipantTimerConfigurationTypeDef],
     },
 )
 
@@ -6225,14 +6304,23 @@
         "Status": TaskTemplateStatusType,
         "LastModifiedTime": datetime,
         "CreatedTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+MetricResultV2TypeDef = TypedDict(
+    "MetricResultV2TypeDef",
+    {
+        "Dimensions": Dict[str, str],
+        "Collections": List[MetricDataV2TypeDef],
+    },
+    total=False,
+)
+
 UpdateParticipantRoleConfigChannelInfoTypeDef = TypedDict(
     "UpdateParticipantRoleConfigChannelInfoTypeDef",
     {
         "Chat": ChatParticipantRoleConfigTypeDef,
     },
     total=False,
 )
@@ -6312,14 +6400,23 @@
     {
         "NextToken": str,
         "MetricResults": List[HistoricalMetricResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetMetricDataV2ResponseTypeDef = TypedDict(
+    "GetMetricDataV2ResponseTypeDef",
+    {
+        "NextToken": str,
+        "MetricResults": List[MetricResultV2TypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateParticipantRoleConfigRequestRequestTypeDef = TypedDict(
     "UpdateParticipantRoleConfigRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
         "ChannelConfiguration": UpdateParticipantRoleConfigChannelInfoTypeDef,
     },
```

### Comparing `mypy-boto3-connect-1.26.79/mypy_boto3_connect.egg-info/PKG-INFO` & `mypy-boto3-connect-1.26.88/mypy_boto3_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connect
-Version: 1.26.79
-Summary: Type annotations for boto3.Connect 1.26.79 service generated with mypy-boto3-builder 7.12.4
+Version: 1.26.88
+Summary: Type annotations for boto3.Connect 1.26.88 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connect?color=blue)](https://pypistats.org/packages/mypy-boto3-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Connect 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[boto3.Connect 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -636,14 +636,15 @@
     RoutingProfileQueueReferenceTypeDef,
     DisassociateSecurityKeyRequestRequestTypeDef,
     DismissUserContactRequestRequestTypeDef,
     DistributionTypeDef,
     EmailReferenceTypeDef,
     EncryptionConfigTypeDef,
     EventBridgeActionDefinitionTypeDef,
+    FilterV2TypeDef,
     FiltersTypeDef,
     GetContactAttributesRequestRequestTypeDef,
     GetFederationTokenRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     GetTaskTemplateRequestRequestTypeDef,
     GetTrafficDistributionRequestRequestTypeDef,
     HierarchyGroupConditionTypeDef,
@@ -701,14 +702,16 @@
     ListTrafficDistributionGroupsRequestRequestTypeDef,
     TrafficDistributionGroupSummaryTypeDef,
     ListUseCasesRequestRequestTypeDef,
     UseCaseTypeDef,
     ListUserHierarchyGroupsRequestRequestTypeDef,
     ListUsersRequestRequestTypeDef,
     UserSummaryTypeDef,
+    MetricFilterV2TypeDef,
+    ThresholdV2TypeDef,
     MonitorContactRequestRequestTypeDef,
     NotificationRecipientTypeTypeDef,
     NumberReferenceTypeDef,
     ParticipantDetailsTypeDef,
     ParticipantTimerValueTypeDef,
     PersistentChatTypeDef,
     PhoneNumberQuickConnectConfigTypeDef,
@@ -896,14 +899,15 @@
     ListRoutingProfilesResponseTypeDef,
     ListSecurityKeysResponseTypeDef,
     ListSecurityProfilesResponseTypeDef,
     ListTaskTemplatesResponseTypeDef,
     ListTrafficDistributionGroupsResponseTypeDef,
     ListUseCasesResponseTypeDef,
     ListUsersResponseTypeDef,
+    MetricV2TypeDef,
     SendNotificationActionDefinitionTypeDef,
     ParticipantTimerConfigurationTypeDef,
     StartChatContactRequestRequestTypeDef,
     QueueSearchCriteriaTypeDef,
     RoutingProfileSearchCriteriaTypeDef,
     SecurityProfileSearchCriteriaTypeDef,
     UserSearchCriteriaTypeDef,
@@ -946,14 +950,16 @@
     HistoricalMetricDataTypeDef,
     CreateHoursOfOperationRequestRequestTypeDef,
     HoursOfOperationTypeDef,
     UpdateHoursOfOperationRequestRequestTypeDef,
     DescribeInstanceResponseTypeDef,
     TaskTemplateConstraintsTypeDef,
     TaskTemplateDefaultsTypeDef,
+    GetMetricDataV2RequestRequestTypeDef,
+    MetricDataV2TypeDef,
     ChatParticipantRoleConfigTypeDef,
     CreateQuickConnectRequestRequestTypeDef,
     QuickConnectTypeDef,
     UpdateQuickConnectConfigRequestRequestTypeDef,
     ListContactReferencesResponseTypeDef,
     RuleActionTypeDef,
     SearchUsersResponseTypeDef,
@@ -974,20 +980,22 @@
     DescribeUserHierarchyGroupResponseTypeDef,
     HistoricalMetricResultTypeDef,
     DescribeHoursOfOperationResponseTypeDef,
     CreateTaskTemplateRequestRequestTypeDef,
     GetTaskTemplateResponseTypeDef,
     UpdateTaskTemplateRequestRequestTypeDef,
     UpdateTaskTemplateResponseTypeDef,
+    MetricResultV2TypeDef,
     UpdateParticipantRoleConfigChannelInfoTypeDef,
     DescribeQuickConnectResponseTypeDef,
     CreateRuleRequestRequestTypeDef,
     RuleTypeDef,
     UpdateRuleRequestRequestTypeDef,
     GetMetricDataResponseTypeDef,
+    GetMetricDataV2ResponseTypeDef,
     UpdateParticipantRoleConfigRequestRequestTypeDef,
     DescribeRuleResponseTypeDef,
 )
 
 
 def get_structure() -> ActionSummaryTypeDef:
     return {...}
```

### Comparing `mypy-boto3-connect-1.26.79/mypy_boto3_connect.egg-info/SOURCES.txt` & `mypy-boto3-connect-1.26.88/mypy_boto3_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.26.79/setup.py` & `mypy-boto3-connect-1.26.88/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-connect",
-    version="1.26.79",
+    version="1.26.88",
     packages=["mypy_boto3_connect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Connect 1.26.79 service generated with mypy-boto3-builder"
-        " 7.12.4"
+        "Type annotations for boto3.Connect 1.26.88 service generated with mypy-boto3-builder"
+        " 7.12.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

