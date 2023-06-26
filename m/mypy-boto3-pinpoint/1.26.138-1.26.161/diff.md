# Comparing `tmp/mypy-boto3-pinpoint-1.26.138.tar.gz` & `tmp/mypy-boto3-pinpoint-1.26.161.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pinpoint-1.26.138.tar", last modified: Mon May 22 19:33:39 2023, max compression
+gzip compressed data, was "mypy-boto3-pinpoint-1.26.161.tar", last modified: Mon Jun 26 19:32:47 2023, max compression
```

## Comparing `mypy-boto3-pinpoint-1.26.138.tar` & `mypy-boto3-pinpoint-1.26.161.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:33:39.893547 mypy-boto3-pinpoint-1.26.138/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29010 2023-05-22 19:33:39.893547 mypy-boto3-pinpoint-1.26.138/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27517 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:33:39.893547 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79752 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    79624 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10566 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   158826 2023-05-22 19:31:54.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   158609 2023-05-22 19:31:52.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:33:39.893547 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29010 2023-05-22 19:33:39.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-22 19:33:39.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:33:39.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:33:39.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-22 19:33:39.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 19:33:39.000000 mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 19:33:39.893547 mypy-boto3-pinpoint-1.26.138/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-22 19:31:49.000000 mypy-boto3-pinpoint-1.26.138/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:32:47.914569 mypy-boto3-pinpoint-1.26.161/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-26 19:32:34.000000 mypy-boto3-pinpoint-1.26.161/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29052 2023-06-26 19:32:47.914569 mypy-boto3-pinpoint-1.26.161/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27559 2023-06-26 19:32:34.000000 mypy-boto3-pinpoint-1.26.161/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:32:47.914569 mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-26 19:32:34.000000 mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-26 19:32:34.000000 mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-26 19:32:34.000000 mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79752 2023-06-26 19:32:34.000000 mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79624 2023-06-26 19:32:34.000000 mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-06-26 19:32:35.000000 mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10801 2023-06-26 19:32:35.000000 mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 19:32:34.000000 mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   159276 2023-06-26 19:32:38.000000 mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   159059 2023-06-26 19:32:37.000000 mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 19:32:34.000000 mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:32:47.914569 mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29052 2023-06-26 19:32:47.000000 mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-26 19:32:47.000000 mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:32:47.000000 mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:32:47.000000 mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-26 19:32:47.000000 mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 19:32:47.000000 mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 19:32:47.914569 mypy-boto3-pinpoint-1.26.161/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-26 19:32:34.000000 mypy-boto3-pinpoint-1.26.161/setup.py
```

### Comparing `mypy-boto3-pinpoint-1.26.138/LICENSE` & `mypy-boto3-pinpoint-1.26.161/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.26.138/PKG-INFO` & `mypy-boto3-pinpoint-1.26.161/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint
-Version: 1.26.138
-Summary: Type annotations for boto3.Pinpoint 1.26.138 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.161
+Summary: Type annotations for boto3.Pinpoint 1.26.161 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.26.138](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.26.161](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -301,14 +301,15 @@
     ModeType,
     OperatorType,
     RecencyTypeType,
     SegmentTypeType,
     SourceTypeType,
     StateType,
     TemplateTypeType,
+    TimezoneEstimationMethodsElementType,
     TypeType,
     PinpointServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
@@ -358,15 +359,14 @@
     CampaignStateTypeDef,
     CustomDeliveryConfigurationTypeDef,
     CampaignSmsMessageTypeDef,
     ChannelResponseTypeDef,
     ClosedDaysRuleTypeDef,
     WaitTimeTypeDef,
     CreateApplicationRequestTypeDef,
-    ResponseMetadataTypeDef,
     EmailTemplateRequestTypeDef,
     CreateTemplateMessageBodyTypeDef,
     ExportJobRequestTypeDef,
     ImportJobRequestTypeDef,
     TemplateCreateMessageBodyTypeDef,
     CreateRecommenderConfigurationTypeDef,
     RecommenderConfigurationResponseTypeDef,
@@ -409,14 +409,15 @@
     GCMMessageTypeDef,
     SMSMessageTypeDef,
     VoiceMessageTypeDef,
     EmailChannelRequestTypeDef,
     JourneyEmailMessageTypeDef,
     RawEmailTypeDef,
     EmailTemplateResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     EndpointDemographicTypeDef,
     EndpointLocationTypeDef,
     EndpointUserTypeDef,
     EndpointItemResponseTypeDef,
     EndpointMessageResultTypeDef,
     EndpointSendConfigurationTypeDef,
     MetricDimensionTypeDef,
@@ -502,14 +503,15 @@
     NumberValidateRequestTypeDef,
     NumberValidateResponseTypeDef,
     OpenHoursRuleTypeDef,
     WriteEventStreamTypeDef,
     RandomSplitEntryTypeDef,
     RecencyDimensionTypeDef,
     UpdateAttributesRequestTypeDef,
+    ResponseMetadataTypeDef,
     ResultRowValueTypeDef,
     SMSChannelRequestTypeDef,
     SegmentConditionTypeDef,
     SegmentReferenceTypeDef,
     SegmentImportResourceTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SimpleEmailPartTypeDef,
@@ -519,50 +521,49 @@
     TemplateVersionResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRecommenderConfigurationTypeDef,
     VoiceChannelRequestTypeDef,
     VerificationResponseTypeDef,
     VerifyOTPMessageRequestParametersTypeDef,
     UpdateAdmChannelRequestRequestTypeDef,
+    DeleteAdmChannelResponseTypeDef,
+    GetAdmChannelResponseTypeDef,
+    UpdateAdmChannelResponseTypeDef,
     UpdateApnsChannelRequestRequestTypeDef,
+    DeleteApnsChannelResponseTypeDef,
+    GetApnsChannelResponseTypeDef,
+    UpdateApnsChannelResponseTypeDef,
     UpdateApnsSandboxChannelRequestRequestTypeDef,
+    DeleteApnsSandboxChannelResponseTypeDef,
+    GetApnsSandboxChannelResponseTypeDef,
+    UpdateApnsSandboxChannelResponseTypeDef,
     UpdateApnsVoipChannelRequestRequestTypeDef,
+    DeleteApnsVoipChannelResponseTypeDef,
+    GetApnsVoipChannelResponseTypeDef,
+    UpdateApnsVoipChannelResponseTypeDef,
     UpdateApnsVoipSandboxChannelRequestRequestTypeDef,
+    DeleteApnsVoipSandboxChannelResponseTypeDef,
+    GetApnsVoipSandboxChannelResponseTypeDef,
+    UpdateApnsVoipSandboxChannelResponseTypeDef,
     ActivitiesResponseTypeDef,
     ApplicationsResponseTypeDef,
+    CreateAppResponseTypeDef,
+    DeleteAppResponseTypeDef,
+    GetAppResponseTypeDef,
     ApplicationSettingsResourceTypeDef,
     WriteApplicationSettingsRequestTypeDef,
+    RemoveAttributesResponseTypeDef,
     UpdateBaiduChannelRequestRequestTypeDef,
+    DeleteBaiduChannelResponseTypeDef,
+    GetBaiduChannelResponseTypeDef,
+    UpdateBaiduChannelResponseTypeDef,
     ChannelsResponseTypeDef,
     ClosedDaysTypeDef,
     WaitActivityTypeDef,
     CreateAppRequestRequestTypeDef,
-    CreateAppResponseTypeDef,
-    DeleteAdmChannelResponseTypeDef,
-    DeleteApnsChannelResponseTypeDef,
-    DeleteApnsSandboxChannelResponseTypeDef,
-    DeleteApnsVoipChannelResponseTypeDef,
-    DeleteApnsVoipSandboxChannelResponseTypeDef,
-    DeleteAppResponseTypeDef,
-    DeleteBaiduChannelResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAdmChannelResponseTypeDef,
-    GetApnsChannelResponseTypeDef,
-    GetApnsSandboxChannelResponseTypeDef,
-    GetApnsVoipChannelResponseTypeDef,
-    GetApnsVoipSandboxChannelResponseTypeDef,
-    GetAppResponseTypeDef,
-    GetBaiduChannelResponseTypeDef,
-    RemoveAttributesResponseTypeDef,
-    UpdateAdmChannelResponseTypeDef,
-    UpdateApnsChannelResponseTypeDef,
-    UpdateApnsSandboxChannelResponseTypeDef,
-    UpdateApnsVoipChannelResponseTypeDef,
-    UpdateApnsVoipSandboxChannelResponseTypeDef,
-    UpdateBaiduChannelResponseTypeDef,
     CreateEmailTemplateRequestRequestTypeDef,
     UpdateEmailTemplateRequestRequestTypeDef,
     CreateEmailTemplateResponseTypeDef,
     CreatePushTemplateResponseTypeDef,
     CreateSmsTemplateResponseTypeDef,
     CreateVoiceTemplateResponseTypeDef,
     CreateExportJobRequestRequestTypeDef,
```

### Comparing `mypy-boto3-pinpoint-1.26.138/README.md` & `mypy-boto3-pinpoint-1.26.161/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.26.138](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.26.161](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -269,14 +269,15 @@
     ModeType,
     OperatorType,
     RecencyTypeType,
     SegmentTypeType,
     SourceTypeType,
     StateType,
     TemplateTypeType,
+    TimezoneEstimationMethodsElementType,
     TypeType,
     PinpointServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
@@ -326,15 +327,14 @@
     CampaignStateTypeDef,
     CustomDeliveryConfigurationTypeDef,
     CampaignSmsMessageTypeDef,
     ChannelResponseTypeDef,
     ClosedDaysRuleTypeDef,
     WaitTimeTypeDef,
     CreateApplicationRequestTypeDef,
-    ResponseMetadataTypeDef,
     EmailTemplateRequestTypeDef,
     CreateTemplateMessageBodyTypeDef,
     ExportJobRequestTypeDef,
     ImportJobRequestTypeDef,
     TemplateCreateMessageBodyTypeDef,
     CreateRecommenderConfigurationTypeDef,
     RecommenderConfigurationResponseTypeDef,
@@ -377,14 +377,15 @@
     GCMMessageTypeDef,
     SMSMessageTypeDef,
     VoiceMessageTypeDef,
     EmailChannelRequestTypeDef,
     JourneyEmailMessageTypeDef,
     RawEmailTypeDef,
     EmailTemplateResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     EndpointDemographicTypeDef,
     EndpointLocationTypeDef,
     EndpointUserTypeDef,
     EndpointItemResponseTypeDef,
     EndpointMessageResultTypeDef,
     EndpointSendConfigurationTypeDef,
     MetricDimensionTypeDef,
@@ -470,14 +471,15 @@
     NumberValidateRequestTypeDef,
     NumberValidateResponseTypeDef,
     OpenHoursRuleTypeDef,
     WriteEventStreamTypeDef,
     RandomSplitEntryTypeDef,
     RecencyDimensionTypeDef,
     UpdateAttributesRequestTypeDef,
+    ResponseMetadataTypeDef,
     ResultRowValueTypeDef,
     SMSChannelRequestTypeDef,
     SegmentConditionTypeDef,
     SegmentReferenceTypeDef,
     SegmentImportResourceTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SimpleEmailPartTypeDef,
@@ -487,50 +489,49 @@
     TemplateVersionResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRecommenderConfigurationTypeDef,
     VoiceChannelRequestTypeDef,
     VerificationResponseTypeDef,
     VerifyOTPMessageRequestParametersTypeDef,
     UpdateAdmChannelRequestRequestTypeDef,
+    DeleteAdmChannelResponseTypeDef,
+    GetAdmChannelResponseTypeDef,
+    UpdateAdmChannelResponseTypeDef,
     UpdateApnsChannelRequestRequestTypeDef,
+    DeleteApnsChannelResponseTypeDef,
+    GetApnsChannelResponseTypeDef,
+    UpdateApnsChannelResponseTypeDef,
     UpdateApnsSandboxChannelRequestRequestTypeDef,
+    DeleteApnsSandboxChannelResponseTypeDef,
+    GetApnsSandboxChannelResponseTypeDef,
+    UpdateApnsSandboxChannelResponseTypeDef,
     UpdateApnsVoipChannelRequestRequestTypeDef,
+    DeleteApnsVoipChannelResponseTypeDef,
+    GetApnsVoipChannelResponseTypeDef,
+    UpdateApnsVoipChannelResponseTypeDef,
     UpdateApnsVoipSandboxChannelRequestRequestTypeDef,
+    DeleteApnsVoipSandboxChannelResponseTypeDef,
+    GetApnsVoipSandboxChannelResponseTypeDef,
+    UpdateApnsVoipSandboxChannelResponseTypeDef,
     ActivitiesResponseTypeDef,
     ApplicationsResponseTypeDef,
+    CreateAppResponseTypeDef,
+    DeleteAppResponseTypeDef,
+    GetAppResponseTypeDef,
     ApplicationSettingsResourceTypeDef,
     WriteApplicationSettingsRequestTypeDef,
+    RemoveAttributesResponseTypeDef,
     UpdateBaiduChannelRequestRequestTypeDef,
+    DeleteBaiduChannelResponseTypeDef,
+    GetBaiduChannelResponseTypeDef,
+    UpdateBaiduChannelResponseTypeDef,
     ChannelsResponseTypeDef,
     ClosedDaysTypeDef,
     WaitActivityTypeDef,
     CreateAppRequestRequestTypeDef,
-    CreateAppResponseTypeDef,
-    DeleteAdmChannelResponseTypeDef,
-    DeleteApnsChannelResponseTypeDef,
-    DeleteApnsSandboxChannelResponseTypeDef,
-    DeleteApnsVoipChannelResponseTypeDef,
-    DeleteApnsVoipSandboxChannelResponseTypeDef,
-    DeleteAppResponseTypeDef,
-    DeleteBaiduChannelResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAdmChannelResponseTypeDef,
-    GetApnsChannelResponseTypeDef,
-    GetApnsSandboxChannelResponseTypeDef,
-    GetApnsVoipChannelResponseTypeDef,
-    GetApnsVoipSandboxChannelResponseTypeDef,
-    GetAppResponseTypeDef,
-    GetBaiduChannelResponseTypeDef,
-    RemoveAttributesResponseTypeDef,
-    UpdateAdmChannelResponseTypeDef,
-    UpdateApnsChannelResponseTypeDef,
-    UpdateApnsSandboxChannelResponseTypeDef,
-    UpdateApnsVoipChannelResponseTypeDef,
-    UpdateApnsVoipSandboxChannelResponseTypeDef,
-    UpdateBaiduChannelResponseTypeDef,
     CreateEmailTemplateRequestRequestTypeDef,
     UpdateEmailTemplateRequestRequestTypeDef,
     CreateEmailTemplateResponseTypeDef,
     CreatePushTemplateResponseTypeDef,
     CreateSmsTemplateResponseTypeDef,
     CreateVoiceTemplateResponseTypeDef,
     CreateExportJobRequestRequestTypeDef,
```

### Comparing `mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/__main__.py` & `mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Pinpoint 1.26.138\nVersion:         1.26.138\nBuilder version:"
+        "Type annotations for boto3.Pinpoint 1.26.161\nVersion:         1.26.161\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.138")
+    print("1.26.161")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/client.py` & `mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/client.pyi` & `mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/literals.py` & `mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     "ModeType",
     "OperatorType",
     "RecencyTypeType",
     "SegmentTypeType",
     "SourceTypeType",
     "StateType",
     "TemplateTypeType",
+    "TimezoneEstimationMethodsElementType",
     "TypeType",
     "PinpointServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
@@ -130,14 +131,15 @@
 ModeType = Literal["DELIVERY", "FILTER"]
 OperatorType = Literal["ALL", "ANY"]
 RecencyTypeType = Literal["ACTIVE", "INACTIVE"]
 SegmentTypeType = Literal["DIMENSIONAL", "IMPORT"]
 SourceTypeType = Literal["ALL", "ANY", "NONE"]
 StateType = Literal["ACTIVE", "CANCELLED", "CLOSED", "COMPLETED", "DRAFT", "PAUSED"]
 TemplateTypeType = Literal["EMAIL", "INAPP", "PUSH", "SMS", "VOICE"]
+TimezoneEstimationMethodsElementType = Literal["PHONE_NUMBER", "POSTAL_CODE"]
 TypeType = Literal["ALL", "ANY", "NONE"]
 PinpointServiceName = Literal["pinpoint"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -194,14 +196,15 @@
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
+    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -373,14 +376,16 @@
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "osis",
     "outposts",
     "panorama",
+    "payment-cryptography",
+    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -464,14 +469,15 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
     "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
```

### Comparing `mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/literals.pyi` & `mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     "ModeType",
     "OperatorType",
     "RecencyTypeType",
     "SegmentTypeType",
     "SourceTypeType",
     "StateType",
     "TemplateTypeType",
+    "TimezoneEstimationMethodsElementType",
     "TypeType",
     "PinpointServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
@@ -128,14 +129,15 @@
 ModeType = Literal["DELIVERY", "FILTER"]
 OperatorType = Literal["ALL", "ANY"]
 RecencyTypeType = Literal["ACTIVE", "INACTIVE"]
 SegmentTypeType = Literal["DIMENSIONAL", "IMPORT"]
 SourceTypeType = Literal["ALL", "ANY", "NONE"]
 StateType = Literal["ACTIVE", "CANCELLED", "CLOSED", "COMPLETED", "DRAFT", "PAUSED"]
 TemplateTypeType = Literal["EMAIL", "INAPP", "PUSH", "SMS", "VOICE"]
+TimezoneEstimationMethodsElementType = Literal["PHONE_NUMBER", "POSTAL_CODE"]
 TypeType = Literal["ALL", "ANY", "NONE"]
 PinpointServiceName = Literal["pinpoint"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -192,14 +194,15 @@
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
+    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -371,14 +374,16 @@
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "osis",
     "outposts",
     "panorama",
+    "payment-cryptography",
+    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -462,14 +467,15 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
     "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
```

### Comparing `mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/type_defs.py` & `mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -40,23 +40,23 @@
     ModeType,
     OperatorType,
     RecencyTypeType,
     SegmentTypeType,
     SourceTypeType,
     StateType,
     TemplateTypeType,
+    TimezoneEstimationMethodsElementType,
     TypeType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ADMChannelRequestTypeDef",
     "ADMChannelResponseTypeDef",
     "ADMMessageTypeDef",
     "APNSChannelRequestTypeDef",
     "APNSChannelResponseTypeDef",
     "APNSMessageTypeDef",
@@ -86,15 +86,14 @@
     "CampaignStateTypeDef",
     "CustomDeliveryConfigurationTypeDef",
     "CampaignSmsMessageTypeDef",
     "ChannelResponseTypeDef",
     "ClosedDaysRuleTypeDef",
     "WaitTimeTypeDef",
     "CreateApplicationRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "EmailTemplateRequestTypeDef",
     "CreateTemplateMessageBodyTypeDef",
     "ExportJobRequestTypeDef",
     "ImportJobRequestTypeDef",
     "TemplateCreateMessageBodyTypeDef",
     "CreateRecommenderConfigurationTypeDef",
     "RecommenderConfigurationResponseTypeDef",
@@ -137,14 +136,15 @@
     "GCMMessageTypeDef",
     "SMSMessageTypeDef",
     "VoiceMessageTypeDef",
     "EmailChannelRequestTypeDef",
     "JourneyEmailMessageTypeDef",
     "RawEmailTypeDef",
     "EmailTemplateResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EndpointDemographicTypeDef",
     "EndpointLocationTypeDef",
     "EndpointUserTypeDef",
     "EndpointItemResponseTypeDef",
     "EndpointMessageResultTypeDef",
     "EndpointSendConfigurationTypeDef",
     "MetricDimensionTypeDef",
@@ -230,14 +230,15 @@
     "NumberValidateRequestTypeDef",
     "NumberValidateResponseTypeDef",
     "OpenHoursRuleTypeDef",
     "WriteEventStreamTypeDef",
     "RandomSplitEntryTypeDef",
     "RecencyDimensionTypeDef",
     "UpdateAttributesRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ResultRowValueTypeDef",
     "SMSChannelRequestTypeDef",
     "SegmentConditionTypeDef",
     "SegmentReferenceTypeDef",
     "SegmentImportResourceTypeDef",
     "SendOTPMessageRequestParametersTypeDef",
     "SimpleEmailPartTypeDef",
@@ -247,50 +248,49 @@
     "TemplateVersionResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateRecommenderConfigurationTypeDef",
     "VoiceChannelRequestTypeDef",
     "VerificationResponseTypeDef",
     "VerifyOTPMessageRequestParametersTypeDef",
     "UpdateAdmChannelRequestRequestTypeDef",
+    "DeleteAdmChannelResponseTypeDef",
+    "GetAdmChannelResponseTypeDef",
+    "UpdateAdmChannelResponseTypeDef",
     "UpdateApnsChannelRequestRequestTypeDef",
+    "DeleteApnsChannelResponseTypeDef",
+    "GetApnsChannelResponseTypeDef",
+    "UpdateApnsChannelResponseTypeDef",
     "UpdateApnsSandboxChannelRequestRequestTypeDef",
+    "DeleteApnsSandboxChannelResponseTypeDef",
+    "GetApnsSandboxChannelResponseTypeDef",
+    "UpdateApnsSandboxChannelResponseTypeDef",
     "UpdateApnsVoipChannelRequestRequestTypeDef",
+    "DeleteApnsVoipChannelResponseTypeDef",
+    "GetApnsVoipChannelResponseTypeDef",
+    "UpdateApnsVoipChannelResponseTypeDef",
     "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
+    "DeleteApnsVoipSandboxChannelResponseTypeDef",
+    "GetApnsVoipSandboxChannelResponseTypeDef",
+    "UpdateApnsVoipSandboxChannelResponseTypeDef",
     "ActivitiesResponseTypeDef",
     "ApplicationsResponseTypeDef",
+    "CreateAppResponseTypeDef",
+    "DeleteAppResponseTypeDef",
+    "GetAppResponseTypeDef",
     "ApplicationSettingsResourceTypeDef",
     "WriteApplicationSettingsRequestTypeDef",
+    "RemoveAttributesResponseTypeDef",
     "UpdateBaiduChannelRequestRequestTypeDef",
+    "DeleteBaiduChannelResponseTypeDef",
+    "GetBaiduChannelResponseTypeDef",
+    "UpdateBaiduChannelResponseTypeDef",
     "ChannelsResponseTypeDef",
     "ClosedDaysTypeDef",
     "WaitActivityTypeDef",
     "CreateAppRequestRequestTypeDef",
-    "CreateAppResponseTypeDef",
-    "DeleteAdmChannelResponseTypeDef",
-    "DeleteApnsChannelResponseTypeDef",
-    "DeleteApnsSandboxChannelResponseTypeDef",
-    "DeleteApnsVoipChannelResponseTypeDef",
-    "DeleteApnsVoipSandboxChannelResponseTypeDef",
-    "DeleteAppResponseTypeDef",
-    "DeleteBaiduChannelResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetAdmChannelResponseTypeDef",
-    "GetApnsChannelResponseTypeDef",
-    "GetApnsSandboxChannelResponseTypeDef",
-    "GetApnsVoipChannelResponseTypeDef",
-    "GetApnsVoipSandboxChannelResponseTypeDef",
-    "GetAppResponseTypeDef",
-    "GetBaiduChannelResponseTypeDef",
-    "RemoveAttributesResponseTypeDef",
-    "UpdateAdmChannelResponseTypeDef",
-    "UpdateApnsChannelResponseTypeDef",
-    "UpdateApnsSandboxChannelResponseTypeDef",
-    "UpdateApnsVoipChannelResponseTypeDef",
-    "UpdateApnsVoipSandboxChannelResponseTypeDef",
-    "UpdateBaiduChannelResponseTypeDef",
     "CreateEmailTemplateRequestRequestTypeDef",
     "UpdateEmailTemplateRequestRequestTypeDef",
     "CreateEmailTemplateResponseTypeDef",
     "CreatePushTemplateResponseTypeDef",
     "CreateSmsTemplateResponseTypeDef",
     "CreateVoiceTemplateResponseTypeDef",
     "CreateExportJobRequestRequestTypeDef",
@@ -517,21 +517,19 @@
     "_OptionalADMChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-
 class ADMChannelRequestTypeDef(
     _RequiredADMChannelRequestTypeDef, _OptionalADMChannelRequestTypeDef
 ):
     pass
 
-
 _RequiredADMChannelResponseTypeDef = TypedDict(
     "_RequiredADMChannelResponseTypeDef",
     {
         "Platform": str,
     },
 )
 _OptionalADMChannelResponseTypeDef = TypedDict(
@@ -546,21 +544,19 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class ADMChannelResponseTypeDef(
     _RequiredADMChannelResponseTypeDef, _OptionalADMChannelResponseTypeDef
 ):
     pass
 
-
 ADMMessageTypeDef = TypedDict(
     "ADMMessageTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "ConsolidationKey": str,
         "Data": Mapping[str, str],
@@ -615,21 +611,19 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class APNSChannelResponseTypeDef(
     _RequiredAPNSChannelResponseTypeDef, _OptionalAPNSChannelResponseTypeDef
 ):
     pass
 
-
 APNSMessageTypeDef = TypedDict(
     "APNSMessageTypeDef",
     {
         "APNSPushType": str,
         "Action": ActionType,
         "Badge": int,
         "Body": str,
@@ -700,21 +694,19 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class APNSSandboxChannelResponseTypeDef(
     _RequiredAPNSSandboxChannelResponseTypeDef, _OptionalAPNSSandboxChannelResponseTypeDef
 ):
     pass
 
-
 APNSVoipChannelRequestTypeDef = TypedDict(
     "APNSVoipChannelRequestTypeDef",
     {
         "BundleId": str,
         "Certificate": str,
         "DefaultAuthenticationMethod": str,
         "Enabled": bool,
@@ -746,21 +738,19 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class APNSVoipChannelResponseTypeDef(
     _RequiredAPNSVoipChannelResponseTypeDef, _OptionalAPNSVoipChannelResponseTypeDef
 ):
     pass
 
-
 APNSVoipSandboxChannelRequestTypeDef = TypedDict(
     "APNSVoipSandboxChannelRequestTypeDef",
     {
         "BundleId": str,
         "Certificate": str,
         "DefaultAuthenticationMethod": str,
         "Enabled": bool,
@@ -792,21 +782,19 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class APNSVoipSandboxChannelResponseTypeDef(
     _RequiredAPNSVoipSandboxChannelResponseTypeDef, _OptionalAPNSVoipSandboxChannelResponseTypeDef
 ):
     pass
 
-
 _RequiredActivityResponseTypeDef = TypedDict(
     "_RequiredActivityResponseTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
         "Id": str,
     },
@@ -825,19 +813,17 @@
         "TotalEndpointCount": int,
         "TreatmentId": str,
         "ExecutionMetrics": Dict[str, str],
     },
     total=False,
 )
 
-
 class ActivityResponseTypeDef(_RequiredActivityResponseTypeDef, _OptionalActivityResponseTypeDef):
     pass
 
-
 ContactCenterActivityTypeDef = TypedDict(
     "ContactCenterActivityTypeDef",
     {
         "NextActivity": str,
     },
     total=False,
 )
@@ -852,19 +838,17 @@
     "_OptionalHoldoutActivityTypeDef",
     {
         "NextActivity": str,
     },
     total=False,
 )
 
-
 class HoldoutActivityTypeDef(_RequiredHoldoutActivityTypeDef, _OptionalHoldoutActivityTypeDef):
     pass
 
-
 AddressConfigurationTypeDef = TypedDict(
     "AddressConfigurationTypeDef",
     {
         "BodyOverride": str,
         "ChannelType": ChannelTypeType,
         "Context": Mapping[str, str],
         "RawContent": str,
@@ -903,21 +887,19 @@
     {
         "tags": Dict[str, str],
         "CreationDate": str,
     },
     total=False,
 )
 
-
 class ApplicationResponseTypeDef(
     _RequiredApplicationResponseTypeDef, _OptionalApplicationResponseTypeDef
 ):
     pass
 
-
 CampaignHookTypeDef = TypedDict(
     "CampaignHookTypeDef",
     {
         "LambdaFunctionName": str,
         "Mode": ModeType,
         "WebUrl": str,
     },
@@ -955,21 +937,19 @@
     "_OptionalAttributeDimensionTypeDef",
     {
         "AttributeType": AttributeTypeType,
     },
     total=False,
 )
 
-
 class AttributeDimensionTypeDef(
     _RequiredAttributeDimensionTypeDef, _OptionalAttributeDimensionTypeDef
 ):
     pass
 
-
 _RequiredAttributesResourceTypeDef = TypedDict(
     "_RequiredAttributesResourceTypeDef",
     {
         "ApplicationId": str,
         "AttributeType": str,
     },
 )
@@ -977,21 +957,19 @@
     "_OptionalAttributesResourceTypeDef",
     {
         "Attributes": List[str],
     },
     total=False,
 )
 
-
 class AttributesResourceTypeDef(
     _RequiredAttributesResourceTypeDef, _OptionalAttributesResourceTypeDef
 ):
     pass
 
-
 _RequiredBaiduChannelRequestTypeDef = TypedDict(
     "_RequiredBaiduChannelRequestTypeDef",
     {
         "ApiKey": str,
         "SecretKey": str,
     },
 )
@@ -999,21 +977,19 @@
     "_OptionalBaiduChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-
 class BaiduChannelRequestTypeDef(
     _RequiredBaiduChannelRequestTypeDef, _OptionalBaiduChannelRequestTypeDef
 ):
     pass
 
-
 _RequiredBaiduChannelResponseTypeDef = TypedDict(
     "_RequiredBaiduChannelResponseTypeDef",
     {
         "Credential": str,
         "Platform": str,
     },
 )
@@ -1029,21 +1005,19 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class BaiduChannelResponseTypeDef(
     _RequiredBaiduChannelResponseTypeDef, _OptionalBaiduChannelResponseTypeDef
 ):
     pass
 
-
 BaiduMessageTypeDef = TypedDict(
     "BaiduMessageTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "Data": Mapping[str, str],
         "IconReference": str,
@@ -1098,21 +1072,19 @@
     "_OptionalCustomDeliveryConfigurationTypeDef",
     {
         "EndpointTypes": Sequence[EndpointTypesElementType],
     },
     total=False,
 )
 
-
 class CustomDeliveryConfigurationTypeDef(
     _RequiredCustomDeliveryConfigurationTypeDef, _OptionalCustomDeliveryConfigurationTypeDef
 ):
     pass
 
-
 CampaignSmsMessageTypeDef = TypedDict(
     "CampaignSmsMessageTypeDef",
     {
         "Body": str,
         "MessageType": MessageTypeType,
         "OriginationNumber": str,
         "SenderId": str,
@@ -1167,32 +1139,19 @@
     "_OptionalCreateApplicationRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateApplicationRequestTypeDef(
     _RequiredCreateApplicationRequestTypeDef, _OptionalCreateApplicationRequestTypeDef
 ):
     pass
 
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 EmailTemplateRequestTypeDef = TypedDict(
     "EmailTemplateRequestTypeDef",
     {
         "DefaultSubstitutions": str,
         "HtmlPart": str,
         "RecommenderId": str,
         "Subject": str,
@@ -1225,19 +1184,17 @@
     {
         "SegmentId": str,
         "SegmentVersion": int,
     },
     total=False,
 )
 
-
 class ExportJobRequestTypeDef(_RequiredExportJobRequestTypeDef, _OptionalExportJobRequestTypeDef):
     pass
 
-
 _RequiredImportJobRequestTypeDef = TypedDict(
     "_RequiredImportJobRequestTypeDef",
     {
         "Format": FormatType,
         "RoleArn": str,
         "S3Url": str,
     },
@@ -1250,19 +1207,17 @@
         "RegisterEndpoints": bool,
         "SegmentId": str,
         "SegmentName": str,
     },
     total=False,
 )
 
-
 class ImportJobRequestTypeDef(_RequiredImportJobRequestTypeDef, _OptionalImportJobRequestTypeDef):
     pass
 
-
 TemplateCreateMessageBodyTypeDef = TypedDict(
     "TemplateCreateMessageBodyTypeDef",
     {
         "Arn": str,
         "Message": str,
         "RequestID": str,
     },
@@ -1286,21 +1241,19 @@
         "RecommendationTransformerUri": str,
         "RecommendationsDisplayName": str,
         "RecommendationsPerMessage": int,
     },
     total=False,
 )
 
-
 class CreateRecommenderConfigurationTypeDef(
     _RequiredCreateRecommenderConfigurationTypeDef, _OptionalCreateRecommenderConfigurationTypeDef
 ):
     pass
 
-
 _RequiredRecommenderConfigurationResponseTypeDef = TypedDict(
     "_RequiredRecommenderConfigurationResponseTypeDef",
     {
         "CreationDate": str,
         "Id": str,
         "LastModifiedDate": str,
         "RecommendationProviderRoleArn": str,
@@ -1317,22 +1270,20 @@
         "RecommendationTransformerUri": str,
         "RecommendationsDisplayName": str,
         "RecommendationsPerMessage": int,
     },
     total=False,
 )
 
-
 class RecommenderConfigurationResponseTypeDef(
     _RequiredRecommenderConfigurationResponseTypeDef,
     _OptionalRecommenderConfigurationResponseTypeDef,
 ):
     pass
 
-
 SMSTemplateRequestTypeDef = TypedDict(
     "SMSTemplateRequestTypeDef",
     {
         "Body": str,
         "DefaultSubstitutions": str,
         "RecommenderId": str,
         "tags": Mapping[str, str],
@@ -1376,21 +1327,19 @@
         "BorderRadius": int,
         "Link": str,
         "TextColor": str,
     },
     total=False,
 )
 
-
 class DefaultButtonConfigurationTypeDef(
     _RequiredDefaultButtonConfigurationTypeDef, _OptionalDefaultButtonConfigurationTypeDef
 ):
     pass
 
-
 DefaultMessageTypeDef = TypedDict(
     "DefaultMessageTypeDef",
     {
         "Body": str,
         "Substitutions": Mapping[str, Sequence[str]],
     },
     total=False,
@@ -1509,43 +1458,39 @@
         "MessagesPerSecond": int,
         "RoleArn": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class EmailChannelResponseTypeDef(
     _RequiredEmailChannelResponseTypeDef, _OptionalEmailChannelResponseTypeDef
 ):
     pass
 
-
 _RequiredDeleteEmailTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteEmailTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteEmailTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class DeleteEmailTemplateRequestRequestTypeDef(
     _RequiredDeleteEmailTemplateRequestRequestTypeDef,
     _OptionalDeleteEmailTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 MessageBodyTypeDef = TypedDict(
     "MessageBodyTypeDef",
     {
         "Message": str,
         "RequestID": str,
     },
     total=False,
@@ -1580,19 +1525,17 @@
         "ExternalId": str,
         "LastModifiedDate": str,
         "LastUpdatedBy": str,
     },
     total=False,
 )
 
-
 class EventStreamTypeDef(_RequiredEventStreamTypeDef, _OptionalEventStreamTypeDef):
     pass
 
-
 DeleteGcmChannelRequestRequestTypeDef = TypedDict(
     "DeleteGcmChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -1615,43 +1558,39 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class GCMChannelResponseTypeDef(
     _RequiredGCMChannelResponseTypeDef, _OptionalGCMChannelResponseTypeDef
 ):
     pass
 
-
 _RequiredDeleteInAppTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteInAppTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteInAppTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteInAppTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class DeleteInAppTemplateRequestRequestTypeDef(
     _RequiredDeleteInAppTemplateRequestRequestTypeDef,
     _OptionalDeleteInAppTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteJourneyRequestRequestTypeDef = TypedDict(
     "DeleteJourneyRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
     },
 )
@@ -1666,22 +1605,20 @@
     "_OptionalDeletePushTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class DeletePushTemplateRequestRequestTypeDef(
     _RequiredDeletePushTemplateRequestRequestTypeDef,
     _OptionalDeletePushTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteRecommenderConfigurationRequestRequestTypeDef",
     {
         "RecommenderId": str,
     },
 )
 
@@ -1722,42 +1659,38 @@
         "ShortCode": str,
         "TransactionalMessagesPerSecond": int,
         "Version": int,
     },
     total=False,
 )
 
-
 class SMSChannelResponseTypeDef(
     _RequiredSMSChannelResponseTypeDef, _OptionalSMSChannelResponseTypeDef
 ):
     pass
 
-
 _RequiredDeleteSmsTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteSmsTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteSmsTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteSmsTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class DeleteSmsTemplateRequestRequestTypeDef(
     _RequiredDeleteSmsTemplateRequestRequestTypeDef, _OptionalDeleteSmsTemplateRequestRequestTypeDef
 ):
     pass
 
-
 DeleteUserEndpointsRequestRequestTypeDef = TypedDict(
     "DeleteUserEndpointsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "UserId": str,
     },
 )
@@ -1787,43 +1720,39 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class VoiceChannelResponseTypeDef(
     _RequiredVoiceChannelResponseTypeDef, _OptionalVoiceChannelResponseTypeDef
 ):
     pass
 
-
 _RequiredDeleteVoiceTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteVoiceTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteVoiceTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteVoiceTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class DeleteVoiceTemplateRequestRequestTypeDef(
     _RequiredDeleteVoiceTemplateRequestRequestTypeDef,
     _OptionalDeleteVoiceTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 GCMMessageTypeDef = TypedDict(
     "GCMMessageTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "CollapseKey": str,
         "Data": Mapping[str, str],
@@ -1885,21 +1814,19 @@
         "ConfigurationSet": str,
         "Enabled": bool,
         "RoleArn": str,
     },
     total=False,
 )
 
-
 class EmailChannelRequestTypeDef(
     _RequiredEmailChannelRequestTypeDef, _OptionalEmailChannelRequestTypeDef
 ):
     pass
 
-
 JourneyEmailMessageTypeDef = TypedDict(
     "JourneyEmailMessageTypeDef",
     {
         "FromAddress": str,
     },
     total=False,
 )
@@ -1933,20 +1860,25 @@
         "TemplateDescription": str,
         "TextPart": str,
         "Version": str,
     },
     total=False,
 )
 
-
 class EmailTemplateResponseTypeDef(
     _RequiredEmailTemplateResponseTypeDef, _OptionalEmailTemplateResponseTypeDef
 ):
     pass
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 EndpointDemographicTypeDef = TypedDict(
     "EndpointDemographicTypeDef",
     {
         "AppVersion": str,
         "Locale": str,
         "Make": str,
@@ -2004,21 +1936,19 @@
         "MessageId": str,
         "StatusMessage": str,
         "UpdatedToken": str,
     },
     total=False,
 )
 
-
 class EndpointMessageResultTypeDef(
     _RequiredEndpointMessageResultTypeDef, _OptionalEndpointMessageResultTypeDef
 ):
     pass
 
-
 EndpointSendConfigurationTypeDef = TypedDict(
     "EndpointSendConfigurationTypeDef",
     {
         "BodyOverride": str,
         "Context": Mapping[str, str],
         "RawContent": str,
         "Substitutions": Mapping[str, Sequence[str]],
@@ -2045,19 +1975,17 @@
     "_OptionalSetDimensionTypeDef",
     {
         "DimensionType": DimensionTypeType,
     },
     total=False,
 )
 
-
 class SetDimensionTypeDef(_RequiredSetDimensionTypeDef, _OptionalSetDimensionTypeDef):
     pass
 
-
 EventItemResponseTypeDef = TypedDict(
     "EventItemResponseTypeDef",
     {
         "Message": str,
         "StatusCode": int,
     },
     total=False,
@@ -2075,19 +2003,17 @@
     {
         "Duration": int,
         "StopTimestamp": str,
     },
     total=False,
 )
 
-
 class SessionTypeDef(_RequiredSessionTypeDef, _OptionalSessionTypeDef):
     pass
 
-
 _RequiredExportJobResourceTypeDef = TypedDict(
     "_RequiredExportJobResourceTypeDef",
     {
         "RoleArn": str,
         "S3UrlPrefix": str,
     },
 )
@@ -2096,42 +2022,38 @@
     {
         "SegmentId": str,
         "SegmentVersion": int,
     },
     total=False,
 )
 
-
 class ExportJobResourceTypeDef(
     _RequiredExportJobResourceTypeDef, _OptionalExportJobResourceTypeDef
 ):
     pass
 
-
 _RequiredGCMChannelRequestTypeDef = TypedDict(
     "_RequiredGCMChannelRequestTypeDef",
     {
         "ApiKey": str,
     },
 )
 _OptionalGCMChannelRequestTypeDef = TypedDict(
     "_OptionalGCMChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-
 class GCMChannelRequestTypeDef(
     _RequiredGCMChannelRequestTypeDef, _OptionalGCMChannelRequestTypeDef
 ):
     pass
 
-
 GPSCoordinatesTypeDef = TypedDict(
     "GPSCoordinatesTypeDef",
     {
         "Latitude": float,
         "Longitude": float,
     },
 )
@@ -2192,22 +2114,20 @@
         "NextToken": str,
         "PageSize": str,
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class GetApplicationDateRangeKpiRequestRequestTypeDef(
     _RequiredGetApplicationDateRangeKpiRequestRequestTypeDef,
     _OptionalGetApplicationDateRangeKpiRequestRequestTypeDef,
 ):
     pass
 
-
 GetApplicationSettingsRequestRequestTypeDef = TypedDict(
     "GetApplicationSettingsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2239,22 +2159,20 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetCampaignActivitiesRequestRequestTypeDef(
     _RequiredGetCampaignActivitiesRequestRequestTypeDef,
     _OptionalGetCampaignActivitiesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetCampaignDateRangeKpiRequestRequestTypeDef = TypedDict(
     "_RequiredGetCampaignDateRangeKpiRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
         "KpiName": str,
     },
@@ -2266,22 +2184,20 @@
         "NextToken": str,
         "PageSize": str,
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class GetCampaignDateRangeKpiRequestRequestTypeDef(
     _RequiredGetCampaignDateRangeKpiRequestRequestTypeDef,
     _OptionalGetCampaignDateRangeKpiRequestRequestTypeDef,
 ):
     pass
 
-
 GetCampaignRequestRequestTypeDef = TypedDict(
     "GetCampaignRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
     },
 )
@@ -2307,22 +2223,20 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetCampaignVersionsRequestRequestTypeDef(
     _RequiredGetCampaignVersionsRequestRequestTypeDef,
     _OptionalGetCampaignVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetCampaignsRequestRequestTypeDef = TypedDict(
     "_RequiredGetCampaignsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalGetCampaignsRequestRequestTypeDef = TypedDict(
@@ -2330,21 +2244,19 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetCampaignsRequestRequestTypeDef(
     _RequiredGetCampaignsRequestRequestTypeDef, _OptionalGetCampaignsRequestRequestTypeDef
 ):
     pass
 
-
 GetChannelsRequestRequestTypeDef = TypedDict(
     "GetChannelsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2365,21 +2277,19 @@
     "_OptionalGetEmailTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class GetEmailTemplateRequestRequestTypeDef(
     _RequiredGetEmailTemplateRequestRequestTypeDef, _OptionalGetEmailTemplateRequestRequestTypeDef
 ):
     pass
 
-
 GetEndpointRequestRequestTypeDef = TypedDict(
     "GetEndpointRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EndpointId": str,
     },
 )
@@ -2410,21 +2320,19 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetExportJobsRequestRequestTypeDef(
     _RequiredGetExportJobsRequestRequestTypeDef, _OptionalGetExportJobsRequestRequestTypeDef
 ):
     pass
 
-
 GetGcmChannelRequestRequestTypeDef = TypedDict(
     "GetGcmChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2447,21 +2355,19 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetImportJobsRequestRequestTypeDef(
     _RequiredGetImportJobsRequestRequestTypeDef, _OptionalGetImportJobsRequestRequestTypeDef
 ):
     pass
 
-
 GetInAppMessagesRequestRequestTypeDef = TypedDict(
     "GetInAppMessagesRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EndpointId": str,
     },
 )
@@ -2476,21 +2382,19 @@
     "_OptionalGetInAppTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class GetInAppTemplateRequestRequestTypeDef(
     _RequiredGetInAppTemplateRequestRequestTypeDef, _OptionalGetInAppTemplateRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetJourneyDateRangeKpiRequestRequestTypeDef = TypedDict(
     "_RequiredGetJourneyDateRangeKpiRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
         "KpiName": str,
     },
@@ -2502,22 +2406,20 @@
         "NextToken": str,
         "PageSize": str,
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class GetJourneyDateRangeKpiRequestRequestTypeDef(
     _RequiredGetJourneyDateRangeKpiRequestRequestTypeDef,
     _OptionalGetJourneyDateRangeKpiRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetJourneyExecutionActivityMetricsRequestRequestTypeDef = TypedDict(
     "_RequiredGetJourneyExecutionActivityMetricsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "JourneyActivityId": str,
         "JourneyId": str,
     },
@@ -2527,22 +2429,20 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
-
 class GetJourneyExecutionActivityMetricsRequestRequestTypeDef(
     _RequiredGetJourneyExecutionActivityMetricsRequestRequestTypeDef,
     _OptionalGetJourneyExecutionActivityMetricsRequestRequestTypeDef,
 ):
     pass
 
-
 JourneyExecutionActivityMetricsResponseTypeDef = TypedDict(
     "JourneyExecutionActivityMetricsResponseTypeDef",
     {
         "ActivityType": str,
         "ApplicationId": str,
         "JourneyActivityId": str,
         "JourneyId": str,
@@ -2563,22 +2463,20 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
-
 class GetJourneyExecutionMetricsRequestRequestTypeDef(
     _RequiredGetJourneyExecutionMetricsRequestRequestTypeDef,
     _OptionalGetJourneyExecutionMetricsRequestRequestTypeDef,
 ):
     pass
 
-
 JourneyExecutionMetricsResponseTypeDef = TypedDict(
     "JourneyExecutionMetricsResponseTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
         "LastEvaluatedTime": str,
         "Metrics": Dict[str, str],
@@ -2607,22 +2505,20 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
-
 class GetJourneyRunExecutionActivityMetricsRequestRequestTypeDef(
     _RequiredGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef,
     _OptionalGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef,
 ):
     pass
 
-
 JourneyRunExecutionActivityMetricsResponseTypeDef = TypedDict(
     "JourneyRunExecutionActivityMetricsResponseTypeDef",
     {
         "ActivityType": str,
         "ApplicationId": str,
         "JourneyActivityId": str,
         "JourneyId": str,
@@ -2645,22 +2541,20 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
-
 class GetJourneyRunExecutionMetricsRequestRequestTypeDef(
     _RequiredGetJourneyRunExecutionMetricsRequestRequestTypeDef,
     _OptionalGetJourneyRunExecutionMetricsRequestRequestTypeDef,
 ):
     pass
 
-
 JourneyRunExecutionMetricsResponseTypeDef = TypedDict(
     "JourneyRunExecutionMetricsResponseTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
         "LastEvaluatedTime": str,
         "Metrics": Dict[str, str],
@@ -2680,42 +2574,38 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetJourneyRunsRequestRequestTypeDef(
     _RequiredGetJourneyRunsRequestRequestTypeDef, _OptionalGetJourneyRunsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetPushTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredGetPushTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalGetPushTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalGetPushTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class GetPushTemplateRequestRequestTypeDef(
     _RequiredGetPushTemplateRequestRequestTypeDef, _OptionalGetPushTemplateRequestRequestTypeDef
 ):
     pass
 
-
 GetRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "GetRecommenderConfigurationRequestRequestTypeDef",
     {
         "RecommenderId": str,
     },
 )
 
@@ -2740,22 +2630,20 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetSegmentExportJobsRequestRequestTypeDef(
     _RequiredGetSegmentExportJobsRequestRequestTypeDef,
     _OptionalGetSegmentExportJobsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetSegmentImportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSegmentImportJobsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "SegmentId": str,
     },
 )
@@ -2764,22 +2652,20 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetSegmentImportJobsRequestRequestTypeDef(
     _RequiredGetSegmentImportJobsRequestRequestTypeDef,
     _OptionalGetSegmentImportJobsRequestRequestTypeDef,
 ):
     pass
 
-
 GetSegmentRequestRequestTypeDef = TypedDict(
     "GetSegmentRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "SegmentId": str,
     },
 )
@@ -2805,22 +2691,20 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetSegmentVersionsRequestRequestTypeDef(
     _RequiredGetSegmentVersionsRequestRequestTypeDef,
     _OptionalGetSegmentVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetSegmentsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSegmentsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalGetSegmentsRequestRequestTypeDef = TypedDict(
@@ -2828,21 +2712,19 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetSegmentsRequestRequestTypeDef(
     _RequiredGetSegmentsRequestRequestTypeDef, _OptionalGetSegmentsRequestRequestTypeDef
 ):
     pass
 
-
 GetSmsChannelRequestRequestTypeDef = TypedDict(
     "GetSmsChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2856,21 +2738,19 @@
     "_OptionalGetSmsTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class GetSmsTemplateRequestRequestTypeDef(
     _RequiredGetSmsTemplateRequestRequestTypeDef, _OptionalGetSmsTemplateRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredSMSTemplateResponseTypeDef = TypedDict(
     "_RequiredSMSTemplateResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": TemplateTypeType,
@@ -2886,21 +2766,19 @@
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
-
 class SMSTemplateResponseTypeDef(
     _RequiredSMSTemplateResponseTypeDef, _OptionalSMSTemplateResponseTypeDef
 ):
     pass
 
-
 GetUserEndpointsRequestRequestTypeDef = TypedDict(
     "GetUserEndpointsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "UserId": str,
     },
 )
@@ -2922,21 +2800,19 @@
     "_OptionalGetVoiceTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class GetVoiceTemplateRequestRequestTypeDef(
     _RequiredGetVoiceTemplateRequestRequestTypeDef, _OptionalGetVoiceTemplateRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredVoiceTemplateResponseTypeDef = TypedDict(
     "_RequiredVoiceTemplateResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": TemplateTypeType,
@@ -2953,21 +2829,19 @@
         "TemplateDescription": str,
         "Version": str,
         "VoiceId": str,
     },
     total=False,
 )
 
-
 class VoiceTemplateResponseTypeDef(
     _RequiredVoiceTemplateResponseTypeDef, _OptionalVoiceTemplateResponseTypeDef
 ):
     pass
 
-
 _RequiredImportJobResourceTypeDef = TypedDict(
     "_RequiredImportJobResourceTypeDef",
     {
         "Format": FormatType,
         "RoleArn": str,
         "S3Url": str,
     },
@@ -2980,21 +2854,19 @@
         "RegisterEndpoints": bool,
         "SegmentId": str,
         "SegmentName": str,
     },
     total=False,
 )
 
-
 class ImportJobResourceTypeDef(
     _RequiredImportJobResourceTypeDef, _OptionalImportJobResourceTypeDef
 ):
     pass
 
-
 InAppMessageBodyConfigTypeDef = TypedDict(
     "InAppMessageBodyConfigTypeDef",
     {
         "Alignment": AlignmentType,
         "Body": str,
         "TextColor": str,
     },
@@ -3010,21 +2882,19 @@
     "_OptionalOverrideButtonConfigurationTypeDef",
     {
         "Link": str,
     },
     total=False,
 )
 
-
 class OverrideButtonConfigurationTypeDef(
     _RequiredOverrideButtonConfigurationTypeDef, _OptionalOverrideButtonConfigurationTypeDef
 ):
     pass
 
-
 InAppMessageHeaderConfigTypeDef = TypedDict(
     "InAppMessageHeaderConfigTypeDef",
     {
         "Alignment": AlignmentType,
         "Header": str,
         "TextColor": str,
     },
@@ -3109,21 +2979,19 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class ListJourneysRequestRequestTypeDef(
     _RequiredListJourneysRequestRequestTypeDef, _OptionalListJourneysRequestRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -3146,22 +3014,20 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
-
 class ListTemplateVersionsRequestRequestTypeDef(
     _RequiredListTemplateVersionsRequestRequestTypeDef,
     _OptionalListTemplateVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListTemplatesRequestRequestTypeDef = TypedDict(
     "ListTemplatesRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": str,
         "Prefix": str,
         "TemplateType": str,
@@ -3201,19 +3067,17 @@
         "MessageId": str,
         "StatusMessage": str,
         "UpdatedToken": str,
     },
     total=False,
 )
 
-
 class MessageResultTypeDef(_RequiredMessageResultTypeDef, _OptionalMessageResultTypeDef):
     pass
 
-
 NumberValidateRequestTypeDef = TypedDict(
     "NumberValidateRequestTypeDef",
     {
         "IsoCountryCode": str,
         "PhoneNumber": str,
     },
     total=False,
@@ -3278,14 +3142,25 @@
     "UpdateAttributesRequestTypeDef",
     {
         "Blacklist": Sequence[str],
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 ResultRowValueTypeDef = TypedDict(
     "ResultRowValueTypeDef",
     {
         "Key": str,
         "Type": str,
         "Value": str,
     },
@@ -3318,19 +3193,17 @@
     "_OptionalSegmentReferenceTypeDef",
     {
         "Version": int,
     },
     total=False,
 )
 
-
 class SegmentReferenceTypeDef(_RequiredSegmentReferenceTypeDef, _OptionalSegmentReferenceTypeDef):
     pass
 
-
 _RequiredSegmentImportResourceTypeDef = TypedDict(
     "_RequiredSegmentImportResourceTypeDef",
     {
         "ExternalId": str,
         "Format": FormatType,
         "RoleArn": str,
         "S3Url": str,
@@ -3341,21 +3214,19 @@
     "_OptionalSegmentImportResourceTypeDef",
     {
         "ChannelCounts": Dict[str, int],
     },
     total=False,
 )
 
-
 class SegmentImportResourceTypeDef(
     _RequiredSegmentImportResourceTypeDef, _OptionalSegmentImportResourceTypeDef
 ):
     pass
 
-
 _RequiredSendOTPMessageRequestParametersTypeDef = TypedDict(
     "_RequiredSendOTPMessageRequestParametersTypeDef",
     {
         "BrandName": str,
         "Channel": str,
         "DestinationIdentity": str,
         "OriginationIdentity": str,
@@ -3371,21 +3242,19 @@
         "Language": str,
         "TemplateId": str,
         "ValidityPeriod": int,
     },
     total=False,
 )
 
-
 class SendOTPMessageRequestParametersTypeDef(
     _RequiredSendOTPMessageRequestParametersTypeDef, _OptionalSendOTPMessageRequestParametersTypeDef
 ):
     pass
 
-
 SimpleEmailPartTypeDef = TypedDict(
     "SimpleEmailPartTypeDef",
     {
         "Charset": str,
         "Data": str,
     },
     total=False,
@@ -3425,19 +3294,17 @@
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
-
 class TemplateResponseTypeDef(_RequiredTemplateResponseTypeDef, _OptionalTemplateResponseTypeDef):
     pass
 
-
 _RequiredTemplateVersionResponseTypeDef = TypedDict(
     "_RequiredTemplateVersionResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": str,
@@ -3449,21 +3316,19 @@
         "DefaultSubstitutions": str,
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
-
 class TemplateVersionResponseTypeDef(
     _RequiredTemplateVersionResponseTypeDef, _OptionalTemplateVersionResponseTypeDef
 ):
     pass
 
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -3485,21 +3350,19 @@
         "RecommendationTransformerUri": str,
         "RecommendationsDisplayName": str,
         "RecommendationsPerMessage": int,
     },
     total=False,
 )
 
-
 class UpdateRecommenderConfigurationTypeDef(
     _RequiredUpdateRecommenderConfigurationTypeDef, _OptionalUpdateRecommenderConfigurationTypeDef
 ):
     pass
 
-
 VoiceChannelRequestTypeDef = TypedDict(
     "VoiceChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -3525,335 +3388,324 @@
     "UpdateAdmChannelRequestRequestTypeDef",
     {
         "ADMChannelRequest": ADMChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
 
-UpdateApnsChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsChannelRequestRequestTypeDef",
+DeleteAdmChannelResponseTypeDef = TypedDict(
+    "DeleteAdmChannelResponseTypeDef",
     {
-        "APNSChannelRequest": APNSChannelRequestTypeDef,
-        "ApplicationId": str,
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateApnsSandboxChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsSandboxChannelRequestRequestTypeDef",
+GetAdmChannelResponseTypeDef = TypedDict(
+    "GetAdmChannelResponseTypeDef",
     {
-        "APNSSandboxChannelRequest": APNSSandboxChannelRequestTypeDef,
-        "ApplicationId": str,
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateApnsVoipChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsVoipChannelRequestRequestTypeDef",
+UpdateAdmChannelResponseTypeDef = TypedDict(
+    "UpdateAdmChannelResponseTypeDef",
     {
-        "APNSVoipChannelRequest": APNSVoipChannelRequestTypeDef,
-        "ApplicationId": str,
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateApnsVoipSandboxChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
+UpdateApnsChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsChannelRequestRequestTypeDef",
     {
-        "APNSVoipSandboxChannelRequest": APNSVoipSandboxChannelRequestTypeDef,
+        "APNSChannelRequest": APNSChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
 
-_RequiredActivitiesResponseTypeDef = TypedDict(
-    "_RequiredActivitiesResponseTypeDef",
+DeleteApnsChannelResponseTypeDef = TypedDict(
+    "DeleteApnsChannelResponseTypeDef",
     {
-        "Item": List[ActivityResponseTypeDef],
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalActivitiesResponseTypeDef = TypedDict(
-    "_OptionalActivitiesResponseTypeDef",
+
+GetApnsChannelResponseTypeDef = TypedDict(
+    "GetApnsChannelResponseTypeDef",
     {
-        "NextToken": str,
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class ActivitiesResponseTypeDef(
-    _RequiredActivitiesResponseTypeDef, _OptionalActivitiesResponseTypeDef
-):
-    pass
-
-
-ApplicationsResponseTypeDef = TypedDict(
-    "ApplicationsResponseTypeDef",
+UpdateApnsChannelResponseTypeDef = TypedDict(
+    "UpdateApnsChannelResponseTypeDef",
     {
-        "Item": List[ApplicationResponseTypeDef],
-        "NextToken": str,
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-_RequiredApplicationSettingsResourceTypeDef = TypedDict(
-    "_RequiredApplicationSettingsResourceTypeDef",
+UpdateApnsSandboxChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsSandboxChannelRequestRequestTypeDef",
     {
+        "APNSSandboxChannelRequest": APNSSandboxChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
-_OptionalApplicationSettingsResourceTypeDef = TypedDict(
-    "_OptionalApplicationSettingsResourceTypeDef",
+
+DeleteApnsSandboxChannelResponseTypeDef = TypedDict(
+    "DeleteApnsSandboxChannelResponseTypeDef",
     {
-        "CampaignHook": CampaignHookTypeDef,
-        "LastModifiedDate": str,
-        "Limits": CampaignLimitsTypeDef,
-        "QuietTime": QuietTimeTypeDef,
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
+GetApnsSandboxChannelResponseTypeDef = TypedDict(
+    "GetApnsSandboxChannelResponseTypeDef",
+    {
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
-class ApplicationSettingsResourceTypeDef(
-    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
-):
-    pass
-
-
-WriteApplicationSettingsRequestTypeDef = TypedDict(
-    "WriteApplicationSettingsRequestTypeDef",
+UpdateApnsSandboxChannelResponseTypeDef = TypedDict(
+    "UpdateApnsSandboxChannelResponseTypeDef",
     {
-        "CampaignHook": CampaignHookTypeDef,
-        "CloudWatchMetricsEnabled": bool,
-        "EventTaggingEnabled": bool,
-        "Limits": CampaignLimitsTypeDef,
-        "QuietTime": QuietTimeTypeDef,
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-UpdateBaiduChannelRequestRequestTypeDef = TypedDict(
-    "UpdateBaiduChannelRequestRequestTypeDef",
+UpdateApnsVoipChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsVoipChannelRequestRequestTypeDef",
     {
+        "APNSVoipChannelRequest": APNSVoipChannelRequestTypeDef,
         "ApplicationId": str,
-        "BaiduChannelRequest": BaiduChannelRequestTypeDef,
     },
 )
 
-ChannelsResponseTypeDef = TypedDict(
-    "ChannelsResponseTypeDef",
+DeleteApnsVoipChannelResponseTypeDef = TypedDict(
+    "DeleteApnsVoipChannelResponseTypeDef",
     {
-        "Channels": Dict[str, ChannelResponseTypeDef],
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ClosedDaysTypeDef = TypedDict(
-    "ClosedDaysTypeDef",
+GetApnsVoipChannelResponseTypeDef = TypedDict(
+    "GetApnsVoipChannelResponseTypeDef",
     {
-        "EMAIL": Sequence[ClosedDaysRuleTypeDef],
-        "SMS": Sequence[ClosedDaysRuleTypeDef],
-        "PUSH": Sequence[ClosedDaysRuleTypeDef],
-        "VOICE": Sequence[ClosedDaysRuleTypeDef],
-        "CUSTOM": Sequence[ClosedDaysRuleTypeDef],
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-WaitActivityTypeDef = TypedDict(
-    "WaitActivityTypeDef",
+UpdateApnsVoipChannelResponseTypeDef = TypedDict(
+    "UpdateApnsVoipChannelResponseTypeDef",
     {
-        "NextActivity": str,
-        "WaitTime": WaitTimeTypeDef,
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-CreateAppRequestRequestTypeDef = TypedDict(
-    "CreateAppRequestRequestTypeDef",
+UpdateApnsVoipSandboxChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
     {
-        "CreateApplicationRequest": CreateApplicationRequestTypeDef,
+        "APNSVoipSandboxChannelRequest": APNSVoipSandboxChannelRequestTypeDef,
+        "ApplicationId": str,
     },
 )
 
-CreateAppResponseTypeDef = TypedDict(
-    "CreateAppResponseTypeDef",
+DeleteApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "DeleteApnsVoipSandboxChannelResponseTypeDef",
     {
-        "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteAdmChannelResponseTypeDef = TypedDict(
-    "DeleteAdmChannelResponseTypeDef",
+GetApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "GetApnsVoipSandboxChannelResponseTypeDef",
     {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteApnsChannelResponseTypeDef = TypedDict(
-    "DeleteApnsChannelResponseTypeDef",
+UpdateApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "UpdateApnsVoipSandboxChannelResponseTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteApnsSandboxChannelResponseTypeDef = TypedDict(
-    "DeleteApnsSandboxChannelResponseTypeDef",
+_RequiredActivitiesResponseTypeDef = TypedDict(
+    "_RequiredActivitiesResponseTypeDef",
     {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Item": List[ActivityResponseTypeDef],
     },
 )
-
-DeleteApnsVoipChannelResponseTypeDef = TypedDict(
-    "DeleteApnsVoipChannelResponseTypeDef",
+_OptionalActivitiesResponseTypeDef = TypedDict(
+    "_OptionalActivitiesResponseTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": str,
     },
+    total=False,
 )
 
-DeleteApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "DeleteApnsVoipSandboxChannelResponseTypeDef",
+class ActivitiesResponseTypeDef(
+    _RequiredActivitiesResponseTypeDef, _OptionalActivitiesResponseTypeDef
+):
+    pass
+
+ApplicationsResponseTypeDef = TypedDict(
+    "ApplicationsResponseTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Item": List[ApplicationResponseTypeDef],
+        "NextToken": str,
     },
+    total=False,
 )
 
-DeleteAppResponseTypeDef = TypedDict(
-    "DeleteAppResponseTypeDef",
+CreateAppResponseTypeDef = TypedDict(
+    "CreateAppResponseTypeDef",
     {
         "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteBaiduChannelResponseTypeDef = TypedDict(
-    "DeleteBaiduChannelResponseTypeDef",
+DeleteAppResponseTypeDef = TypedDict(
+    "DeleteAppResponseTypeDef",
     {
-        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationResponse": ApplicationResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+GetAppResponseTypeDef = TypedDict(
+    "GetAppResponseTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationResponse": ApplicationResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetAdmChannelResponseTypeDef = TypedDict(
-    "GetAdmChannelResponseTypeDef",
+_RequiredApplicationSettingsResourceTypeDef = TypedDict(
+    "_RequiredApplicationSettingsResourceTypeDef",
     {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationId": str,
     },
 )
-
-GetApnsChannelResponseTypeDef = TypedDict(
-    "GetApnsChannelResponseTypeDef",
+_OptionalApplicationSettingsResourceTypeDef = TypedDict(
+    "_OptionalApplicationSettingsResourceTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CampaignHook": CampaignHookTypeDef,
+        "LastModifiedDate": str,
+        "Limits": CampaignLimitsTypeDef,
+        "QuietTime": QuietTimeTypeDef,
     },
+    total=False,
 )
 
-GetApnsSandboxChannelResponseTypeDef = TypedDict(
-    "GetApnsSandboxChannelResponseTypeDef",
+class ApplicationSettingsResourceTypeDef(
+    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
+):
+    pass
+
+WriteApplicationSettingsRequestTypeDef = TypedDict(
+    "WriteApplicationSettingsRequestTypeDef",
     {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CampaignHook": CampaignHookTypeDef,
+        "CloudWatchMetricsEnabled": bool,
+        "EventTaggingEnabled": bool,
+        "Limits": CampaignLimitsTypeDef,
+        "QuietTime": QuietTimeTypeDef,
     },
+    total=False,
 )
 
-GetApnsVoipChannelResponseTypeDef = TypedDict(
-    "GetApnsVoipChannelResponseTypeDef",
+RemoveAttributesResponseTypeDef = TypedDict(
+    "RemoveAttributesResponseTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AttributesResource": AttributesResourceTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "GetApnsVoipSandboxChannelResponseTypeDef",
+UpdateBaiduChannelRequestRequestTypeDef = TypedDict(
+    "UpdateBaiduChannelRequestRequestTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationId": str,
+        "BaiduChannelRequest": BaiduChannelRequestTypeDef,
     },
 )
 
-GetAppResponseTypeDef = TypedDict(
-    "GetAppResponseTypeDef",
+DeleteBaiduChannelResponseTypeDef = TypedDict(
+    "DeleteBaiduChannelResponseTypeDef",
     {
-        "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBaiduChannelResponseTypeDef = TypedDict(
     "GetBaiduChannelResponseTypeDef",
     {
         "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveAttributesResponseTypeDef = TypedDict(
-    "RemoveAttributesResponseTypeDef",
-    {
-        "AttributesResource": AttributesResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateAdmChannelResponseTypeDef = TypedDict(
-    "UpdateAdmChannelResponseTypeDef",
-    {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateApnsChannelResponseTypeDef = TypedDict(
-    "UpdateApnsChannelResponseTypeDef",
+UpdateBaiduChannelResponseTypeDef = TypedDict(
+    "UpdateBaiduChannelResponseTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateApnsSandboxChannelResponseTypeDef = TypedDict(
-    "UpdateApnsSandboxChannelResponseTypeDef",
+ChannelsResponseTypeDef = TypedDict(
+    "ChannelsResponseTypeDef",
     {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Channels": Dict[str, ChannelResponseTypeDef],
     },
 )
 
-UpdateApnsVoipChannelResponseTypeDef = TypedDict(
-    "UpdateApnsVoipChannelResponseTypeDef",
+ClosedDaysTypeDef = TypedDict(
+    "ClosedDaysTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "EMAIL": Sequence[ClosedDaysRuleTypeDef],
+        "SMS": Sequence[ClosedDaysRuleTypeDef],
+        "PUSH": Sequence[ClosedDaysRuleTypeDef],
+        "VOICE": Sequence[ClosedDaysRuleTypeDef],
+        "CUSTOM": Sequence[ClosedDaysRuleTypeDef],
     },
+    total=False,
 )
 
-UpdateApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "UpdateApnsVoipSandboxChannelResponseTypeDef",
+WaitActivityTypeDef = TypedDict(
+    "WaitActivityTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextActivity": str,
+        "WaitTime": WaitTimeTypeDef,
     },
+    total=False,
 )
 
-UpdateBaiduChannelResponseTypeDef = TypedDict(
-    "UpdateBaiduChannelResponseTypeDef",
+CreateAppRequestRequestTypeDef = TypedDict(
+    "CreateAppRequestRequestTypeDef",
     {
-        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CreateApplicationRequest": CreateApplicationRequestTypeDef,
     },
 )
 
 CreateEmailTemplateRequestRequestTypeDef = TypedDict(
     "CreateEmailTemplateRequestRequestTypeDef",
     {
         "EmailTemplateRequest": EmailTemplateRequestTypeDef,
@@ -3873,51 +3725,49 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
-
 class UpdateEmailTemplateRequestRequestTypeDef(
     _RequiredUpdateEmailTemplateRequestRequestTypeDef,
     _OptionalUpdateEmailTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 CreateEmailTemplateResponseTypeDef = TypedDict(
     "CreateEmailTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePushTemplateResponseTypeDef = TypedDict(
     "CreatePushTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSmsTemplateResponseTypeDef = TypedDict(
     "CreateSmsTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateVoiceTemplateResponseTypeDef = TypedDict(
     "CreateVoiceTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateExportJobRequestRequestTypeDef = TypedDict(
     "CreateExportJobRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -3933,46 +3783,46 @@
     },
 )
 
 CreateInAppTemplateResponseTypeDef = TypedDict(
     "CreateInAppTemplateResponseTypeDef",
     {
         "TemplateCreateMessageBody": TemplateCreateMessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "CreateRecommenderConfigurationRequestRequestTypeDef",
     {
         "CreateRecommenderConfiguration": CreateRecommenderConfigurationTypeDef,
     },
 )
 
 CreateRecommenderConfigurationResponseTypeDef = TypedDict(
     "CreateRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRecommenderConfigurationResponseTypeDef = TypedDict(
     "DeleteRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRecommenderConfigurationResponseTypeDef = TypedDict(
     "GetRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListRecommenderConfigurationsResponseTypeDef = TypedDict(
     "_RequiredListRecommenderConfigurationsResponseTypeDef",
     {
         "Item": List[RecommenderConfigurationResponseTypeDef],
@@ -3982,27 +3832,25 @@
     "_OptionalListRecommenderConfigurationsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListRecommenderConfigurationsResponseTypeDef(
     _RequiredListRecommenderConfigurationsResponseTypeDef,
     _OptionalListRecommenderConfigurationsResponseTypeDef,
 ):
     pass
 
-
 UpdateRecommenderConfigurationResponseTypeDef = TypedDict(
     "UpdateRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSmsTemplateRequestRequestTypeDef = TypedDict(
     "CreateSmsTemplateRequestRequestTypeDef",
     {
         "SMSTemplateRequest": SMSTemplateRequestTypeDef,
@@ -4022,21 +3870,19 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
-
 class UpdateSmsTemplateRequestRequestTypeDef(
     _RequiredUpdateSmsTemplateRequestRequestTypeDef, _OptionalUpdateSmsTemplateRequestRequestTypeDef
 ):
     pass
 
-
 CreateVoiceTemplateRequestRequestTypeDef = TypedDict(
     "CreateVoiceTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "VoiceTemplateRequest": VoiceTemplateRequestTypeDef,
     },
 )
@@ -4053,22 +3899,20 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
-
 class UpdateVoiceTemplateRequestRequestTypeDef(
     _RequiredUpdateVoiceTemplateRequestRequestTypeDef,
     _OptionalUpdateVoiceTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 CustomMessageActivityTypeDef = TypedDict(
     "CustomMessageActivityTypeDef",
     {
         "DeliveryUri": str,
         "EndpointTypes": Sequence[EndpointTypesElementType],
         "MessageConfig": JourneyCustomMessageTypeDef,
         "NextActivity": str,
@@ -4117,243 +3961,241 @@
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
-
 class PushNotificationTemplateResponseTypeDef(
     _RequiredPushNotificationTemplateResponseTypeDef,
     _OptionalPushNotificationTemplateResponseTypeDef,
 ):
     pass
 
-
 DeleteEmailChannelResponseTypeDef = TypedDict(
     "DeleteEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEmailChannelResponseTypeDef = TypedDict(
     "GetEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEmailChannelResponseTypeDef = TypedDict(
     "UpdateEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEmailTemplateResponseTypeDef = TypedDict(
     "DeleteEmailTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteInAppTemplateResponseTypeDef = TypedDict(
     "DeleteInAppTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeletePushTemplateResponseTypeDef = TypedDict(
     "DeletePushTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSmsTemplateResponseTypeDef = TypedDict(
     "DeleteSmsTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVoiceTemplateResponseTypeDef = TypedDict(
     "DeleteVoiceTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEmailTemplateResponseTypeDef = TypedDict(
     "UpdateEmailTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEndpointResponseTypeDef = TypedDict(
     "UpdateEndpointResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEndpointsBatchResponseTypeDef = TypedDict(
     "UpdateEndpointsBatchResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateInAppTemplateResponseTypeDef = TypedDict(
     "UpdateInAppTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePushTemplateResponseTypeDef = TypedDict(
     "UpdatePushTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSmsTemplateResponseTypeDef = TypedDict(
     "UpdateSmsTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTemplateActiveVersionResponseTypeDef = TypedDict(
     "UpdateTemplateActiveVersionResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVoiceTemplateResponseTypeDef = TypedDict(
     "UpdateVoiceTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEventStreamResponseTypeDef = TypedDict(
     "DeleteEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEventStreamResponseTypeDef = TypedDict(
     "GetEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutEventStreamResponseTypeDef = TypedDict(
     "PutEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteGcmChannelResponseTypeDef = TypedDict(
     "DeleteGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGcmChannelResponseTypeDef = TypedDict(
     "GetGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGcmChannelResponseTypeDef = TypedDict(
     "UpdateGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSmsChannelResponseTypeDef = TypedDict(
     "DeleteSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSmsChannelResponseTypeDef = TypedDict(
     "GetSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSmsChannelResponseTypeDef = TypedDict(
     "UpdateSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVoiceChannelResponseTypeDef = TypedDict(
     "DeleteVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceChannelResponseTypeDef = TypedDict(
     "GetVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVoiceChannelResponseTypeDef = TypedDict(
     "UpdateVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEmailChannelRequestRequestTypeDef = TypedDict(
     "UpdateEmailChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -4372,15 +4214,15 @@
     total=False,
 )
 
 GetEmailTemplateResponseTypeDef = TypedDict(
     "GetEmailTemplateResponseTypeDef",
     {
         "EmailTemplateResponse": EmailTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EndpointBatchItemTypeDef = TypedDict(
     "EndpointBatchItemTypeDef",
     {
         "Address": str,
@@ -4468,21 +4310,19 @@
     {
         "RequestId": str,
         "Result": Dict[str, Dict[str, EndpointMessageResultTypeDef]],
     },
     total=False,
 )
 
-
 class SendUsersMessageResponseTypeDef(
     _RequiredSendUsersMessageResponseTypeDef, _OptionalSendUsersMessageResponseTypeDef
 ):
     pass
 
-
 EventDimensionsTypeDef = TypedDict(
     "EventDimensionsTypeDef",
     {
         "Attributes": Mapping[str, AttributeDimensionTypeDef],
         "EventType": SetDimensionTypeDef,
         "Metrics": Mapping[str, MetricDimensionTypeDef],
     },
@@ -4529,19 +4369,17 @@
         "Metrics": Mapping[str, float],
         "SdkName": str,
         "Session": SessionTypeDef,
     },
     total=False,
 )
 
-
 class EventTypeDef(_RequiredEventTypeDef, _OptionalEventTypeDef):
     pass
 
-
 _RequiredExportJobResponseTypeDef = TypedDict(
     "_RequiredExportJobResponseTypeDef",
     {
         "ApplicationId": str,
         "CreationDate": str,
         "Definition": ExportJobResourceTypeDef,
         "Id": str,
@@ -4559,21 +4397,19 @@
         "TotalFailures": int,
         "TotalPieces": int,
         "TotalProcessed": int,
     },
     total=False,
 )
 
-
 class ExportJobResponseTypeDef(
     _RequiredExportJobResponseTypeDef, _OptionalExportJobResponseTypeDef
 ):
     pass
 
-
 UpdateGcmChannelRequestRequestTypeDef = TypedDict(
     "UpdateGcmChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "GCMChannelRequest": GCMChannelRequestTypeDef,
     },
 )
@@ -4588,68 +4424,66 @@
     "_OptionalGPSPointDimensionTypeDef",
     {
         "RangeInKilometers": float,
     },
     total=False,
 )
 
-
 class GPSPointDimensionTypeDef(
     _RequiredGPSPointDimensionTypeDef, _OptionalGPSPointDimensionTypeDef
 ):
     pass
 
-
 GetJourneyExecutionActivityMetricsResponseTypeDef = TypedDict(
     "GetJourneyExecutionActivityMetricsResponseTypeDef",
     {
         "JourneyExecutionActivityMetricsResponse": JourneyExecutionActivityMetricsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJourneyExecutionMetricsResponseTypeDef = TypedDict(
     "GetJourneyExecutionMetricsResponseTypeDef",
     {
         "JourneyExecutionMetricsResponse": JourneyExecutionMetricsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJourneyRunExecutionActivityMetricsResponseTypeDef = TypedDict(
     "GetJourneyRunExecutionActivityMetricsResponseTypeDef",
     {
         "JourneyRunExecutionActivityMetricsResponse": (
             JourneyRunExecutionActivityMetricsResponseTypeDef
         ),
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJourneyRunExecutionMetricsResponseTypeDef = TypedDict(
     "GetJourneyRunExecutionMetricsResponseTypeDef",
     {
         "JourneyRunExecutionMetricsResponse": JourneyRunExecutionMetricsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSmsTemplateResponseTypeDef = TypedDict(
     "GetSmsTemplateResponseTypeDef",
     {
         "SMSTemplateResponse": SMSTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceTemplateResponseTypeDef = TypedDict(
     "GetVoiceTemplateResponseTypeDef",
     {
         "VoiceTemplateResponse": VoiceTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredImportJobResponseTypeDef = TypedDict(
     "_RequiredImportJobResponseTypeDef",
     {
         "ApplicationId": str,
@@ -4670,21 +4504,19 @@
         "TotalFailures": int,
         "TotalPieces": int,
         "TotalProcessed": int,
     },
     total=False,
 )
 
-
 class ImportJobResponseTypeDef(
     _RequiredImportJobResponseTypeDef, _OptionalImportJobResponseTypeDef
 ):
     pass
 
-
 InAppMessageButtonTypeDef = TypedDict(
     "InAppMessageButtonTypeDef",
     {
         "Android": OverrideButtonConfigurationTypeDef,
         "DefaultConfig": DefaultButtonConfigurationTypeDef,
         "IOS": OverrideButtonConfigurationTypeDef,
         "Web": OverrideButtonConfigurationTypeDef,
@@ -4713,21 +4545,19 @@
     "_OptionalJourneyRunsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class JourneyRunsResponseTypeDef(
     _RequiredJourneyRunsResponseTypeDef, _OptionalJourneyRunsResponseTypeDef
 ):
     pass
 
-
 SMSMessageActivityTypeDef = TypedDict(
     "SMSMessageActivityTypeDef",
     {
         "MessageConfig": JourneySMSMessageTypeDef,
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
@@ -4744,15 +4574,15 @@
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "TagsModel": TagsModelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -4772,31 +4602,29 @@
         "EndpointResult": Dict[str, EndpointMessageResultTypeDef],
         "RequestId": str,
         "Result": Dict[str, MessageResultTypeDef],
     },
     total=False,
 )
 
-
 class MessageResponseTypeDef(_RequiredMessageResponseTypeDef, _OptionalMessageResponseTypeDef):
     pass
 
-
 PhoneNumberValidateRequestRequestTypeDef = TypedDict(
     "PhoneNumberValidateRequestRequestTypeDef",
     {
         "NumberValidateRequest": NumberValidateRequestTypeDef,
     },
 )
 
 PhoneNumberValidateResponseTypeDef = TypedDict(
     "PhoneNumberValidateResponseTypeDef",
     {
         "NumberValidateResponse": NumberValidateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OpenHoursTypeDef = TypedDict(
     "OpenHoursTypeDef",
     {
         "EMAIL": Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]],
@@ -4905,21 +4733,19 @@
     "_OptionalTemplatesResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class TemplatesResponseTypeDef(
     _RequiredTemplatesResponseTypeDef, _OptionalTemplatesResponseTypeDef
 ):
     pass
 
-
 _RequiredTemplateVersionsResponseTypeDef = TypedDict(
     "_RequiredTemplateVersionsResponseTypeDef",
     {
         "Item": List[TemplateVersionResponseTypeDef],
     },
 )
 _OptionalTemplateVersionsResponseTypeDef = TypedDict(
@@ -4928,21 +4754,19 @@
         "Message": str,
         "NextToken": str,
         "RequestID": str,
     },
     total=False,
 )
 
-
 class TemplateVersionsResponseTypeDef(
     _RequiredTemplateVersionsResponseTypeDef, _OptionalTemplateVersionsResponseTypeDef
 ):
     pass
 
-
 UpdateRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateRecommenderConfigurationRequestRequestTypeDef",
     {
         "RecommenderId": str,
         "UpdateRecommenderConfiguration": UpdateRecommenderConfigurationTypeDef,
     },
 )
@@ -4955,15 +4779,15 @@
     },
 )
 
 VerifyOTPMessageResponseTypeDef = TypedDict(
     "VerifyOTPMessageResponseTypeDef",
     {
         "VerificationResponse": VerificationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VerifyOTPMessageRequestRequestTypeDef = TypedDict(
     "VerifyOTPMessageRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -4971,39 +4795,39 @@
     },
 )
 
 GetCampaignActivitiesResponseTypeDef = TypedDict(
     "GetCampaignActivitiesResponseTypeDef",
     {
         "ActivitiesResponse": ActivitiesResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAppsResponseTypeDef = TypedDict(
     "GetAppsResponseTypeDef",
     {
         "ApplicationsResponse": ApplicationsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetApplicationSettingsResponseTypeDef = TypedDict(
     "GetApplicationSettingsResponseTypeDef",
     {
         "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateApplicationSettingsResponseTypeDef = TypedDict(
     "UpdateApplicationSettingsResponseTypeDef",
     {
         "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateApplicationSettingsRequestRequestTypeDef = TypedDict(
     "UpdateApplicationSettingsRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -5011,23 +4835,23 @@
     },
 )
 
 GetChannelsResponseTypeDef = TypedDict(
     "GetChannelsResponseTypeDef",
     {
         "ChannelsResponse": ChannelsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRecommenderConfigurationsResponseTypeDef = TypedDict(
     "GetRecommenderConfigurationsResponseTypeDef",
     {
         "ListRecommenderConfigurationsResponse": ListRecommenderConfigurationsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePushTemplateRequestRequestTypeDef = TypedDict(
     "CreatePushTemplateRequestRequestTypeDef",
     {
         "PushNotificationTemplateRequest": PushNotificationTemplateRequestTypeDef,
@@ -5047,27 +4871,25 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
-
 class UpdatePushTemplateRequestRequestTypeDef(
     _RequiredUpdatePushTemplateRequestRequestTypeDef,
     _OptionalUpdatePushTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 GetPushTemplateResponseTypeDef = TypedDict(
     "GetPushTemplateResponseTypeDef",
     {
         "PushNotificationTemplateResponse": PushNotificationTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EndpointBatchRequestTypeDef = TypedDict(
     "EndpointBatchRequestTypeDef",
     {
         "Item": Sequence[EndpointBatchItemTypeDef],
@@ -5083,38 +4905,38 @@
     },
 )
 
 DeleteEndpointResponseTypeDef = TypedDict(
     "DeleteEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EndpointsResponseTypeDef = TypedDict(
     "EndpointsResponseTypeDef",
     {
         "Item": List[EndpointResponseTypeDef],
     },
 )
 
 GetEndpointResponseTypeDef = TypedDict(
     "GetEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SendUsersMessagesResponseTypeDef = TypedDict(
     "SendUsersMessagesResponseTypeDef",
     {
         "SendUsersMessageResponse": SendUsersMessageResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CampaignEventFilterTypeDef = TypedDict(
     "CampaignEventFilterTypeDef",
     {
         "Dimensions": EventDimensionsTypeDef,
@@ -5155,15 +4977,15 @@
     },
 )
 
 CreateExportJobResponseTypeDef = TypedDict(
     "CreateExportJobResponseTypeDef",
     {
         "ExportJobResponse": ExportJobResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredExportJobsResponseTypeDef = TypedDict(
     "_RequiredExportJobsResponseTypeDef",
     {
         "Item": List[ExportJobResponseTypeDef],
@@ -5173,26 +4995,24 @@
     "_OptionalExportJobsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ExportJobsResponseTypeDef(
     _RequiredExportJobsResponseTypeDef, _OptionalExportJobsResponseTypeDef
 ):
     pass
 
-
 GetExportJobResponseTypeDef = TypedDict(
     "GetExportJobResponseTypeDef",
     {
         "ExportJobResponse": ExportJobResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SegmentLocationTypeDef = TypedDict(
     "SegmentLocationTypeDef",
     {
         "Country": SetDimensionTypeDef,
@@ -5201,23 +5021,23 @@
     total=False,
 )
 
 CreateImportJobResponseTypeDef = TypedDict(
     "CreateImportJobResponseTypeDef",
     {
         "ImportJobResponse": ImportJobResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetImportJobResponseTypeDef = TypedDict(
     "GetImportJobResponseTypeDef",
     {
         "ImportJobResponse": ImportJobResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredImportJobsResponseTypeDef = TypedDict(
     "_RequiredImportJobsResponseTypeDef",
     {
         "Item": List[ImportJobResponseTypeDef],
@@ -5227,21 +5047,19 @@
     "_OptionalImportJobsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ImportJobsResponseTypeDef(
     _RequiredImportJobsResponseTypeDef, _OptionalImportJobsResponseTypeDef
 ):
     pass
 
-
 InAppMessageContentTypeDef = TypedDict(
     "InAppMessageContentTypeDef",
     {
         "BackgroundColor": str,
         "BodyConfig": InAppMessageBodyConfigTypeDef,
         "HeaderConfig": InAppMessageHeaderConfigTypeDef,
         "ImageUrl": str,
@@ -5251,31 +5069,31 @@
     total=False,
 )
 
 GetJourneyRunsResponseTypeDef = TypedDict(
     "GetJourneyRunsResponseTypeDef",
     {
         "JourneyRunsResponse": JourneyRunsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SendMessagesResponseTypeDef = TypedDict(
     "SendMessagesResponseTypeDef",
     {
         "MessageResponse": MessageResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SendOTPMessageResponseTypeDef = TypedDict(
     "SendOTPMessageResponseTypeDef",
     {
         "MessageResponse": MessageResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BaseKpiResultTypeDef = TypedDict(
     "BaseKpiResultTypeDef",
     {
         "Rows": List[ResultRowTypeDef],
@@ -5296,23 +5114,23 @@
     total=False,
 )
 
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "TemplatesResponse": TemplatesResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTemplateVersionsResponseTypeDef = TypedDict(
     "ListTemplateVersionsResponseTypeDef",
     {
         "TemplateVersionsResponse": TemplateVersionsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEndpointsBatchRequestRequestTypeDef = TypedDict(
     "UpdateEndpointsBatchRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -5320,23 +5138,23 @@
     },
 )
 
 DeleteUserEndpointsResponseTypeDef = TypedDict(
     "DeleteUserEndpointsResponseTypeDef",
     {
         "EndpointsResponse": EndpointsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUserEndpointsResponseTypeDef = TypedDict(
     "GetUserEndpointsResponseTypeDef",
     {
         "EndpointsResponse": EndpointsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InAppCampaignScheduleTypeDef = TypedDict(
     "InAppCampaignScheduleTypeDef",
     {
         "EndDate": str,
@@ -5361,56 +5179,54 @@
         "IsLocalTime": bool,
         "QuietTime": QuietTimeTypeDef,
         "Timezone": str,
     },
     total=False,
 )
 
-
 class ScheduleTypeDef(_RequiredScheduleTypeDef, _OptionalScheduleTypeDef):
     pass
 
-
 EventStartConditionTypeDef = TypedDict(
     "EventStartConditionTypeDef",
     {
         "EventFilter": EventFilterTypeDef,
         "SegmentId": str,
     },
     total=False,
 )
 
 PutEventsResponseTypeDef = TypedDict(
     "PutEventsResponseTypeDef",
     {
         "EventsResponse": EventsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventsRequestTypeDef = TypedDict(
     "EventsRequestTypeDef",
     {
         "BatchItem": Mapping[str, EventsBatchTypeDef],
     },
 )
 
 GetExportJobsResponseTypeDef = TypedDict(
     "GetExportJobsResponseTypeDef",
     {
         "ExportJobsResponse": ExportJobsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentExportJobsResponseTypeDef = TypedDict(
     "GetSegmentExportJobsResponseTypeDef",
     {
         "ExportJobsResponse": ExportJobsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SegmentDimensionsTypeDef = TypedDict(
     "SegmentDimensionsTypeDef",
     {
         "Attributes": Mapping[str, AttributeDimensionTypeDef],
@@ -5423,23 +5239,23 @@
     total=False,
 )
 
 GetImportJobsResponseTypeDef = TypedDict(
     "GetImportJobsResponseTypeDef",
     {
         "ImportJobsResponse": ImportJobsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentImportJobsResponseTypeDef = TypedDict(
     "GetSegmentImportJobsResponseTypeDef",
     {
         "ImportJobsResponse": ImportJobsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CampaignInAppMessageTypeDef = TypedDict(
     "CampaignInAppMessageTypeDef",
     {
         "Body": str,
@@ -5491,21 +5307,19 @@
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
-
 class InAppTemplateResponseTypeDef(
     _RequiredInAppTemplateResponseTypeDef, _OptionalInAppTemplateResponseTypeDef
 ):
     pass
 
-
 _RequiredApplicationDateRangeKpiResponseTypeDef = TypedDict(
     "_RequiredApplicationDateRangeKpiResponseTypeDef",
     {
         "ApplicationId": str,
         "EndTime": datetime,
         "KpiName": str,
         "KpiResult": BaseKpiResultTypeDef,
@@ -5516,21 +5330,19 @@
     "_OptionalApplicationDateRangeKpiResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ApplicationDateRangeKpiResponseTypeDef(
     _RequiredApplicationDateRangeKpiResponseTypeDef, _OptionalApplicationDateRangeKpiResponseTypeDef
 ):
     pass
 
-
 _RequiredCampaignDateRangeKpiResponseTypeDef = TypedDict(
     "_RequiredCampaignDateRangeKpiResponseTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
         "EndTime": datetime,
         "KpiName": str,
@@ -5542,21 +5354,19 @@
     "_OptionalCampaignDateRangeKpiResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class CampaignDateRangeKpiResponseTypeDef(
     _RequiredCampaignDateRangeKpiResponseTypeDef, _OptionalCampaignDateRangeKpiResponseTypeDef
 ):
     pass
 
-
 _RequiredJourneyDateRangeKpiResponseTypeDef = TypedDict(
     "_RequiredJourneyDateRangeKpiResponseTypeDef",
     {
         "ApplicationId": str,
         "EndTime": datetime,
         "JourneyId": str,
         "KpiName": str,
@@ -5568,21 +5378,19 @@
     "_OptionalJourneyDateRangeKpiResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class JourneyDateRangeKpiResponseTypeDef(
     _RequiredJourneyDateRangeKpiResponseTypeDef, _OptionalJourneyDateRangeKpiResponseTypeDef
 ):
     pass
 
-
 DirectMessageConfigurationTypeDef = TypedDict(
     "DirectMessageConfigurationTypeDef",
     {
         "ADMMessage": ADMMessageTypeDef,
         "APNSMessage": APNSMessageTypeDef,
         "BaiduMessage": BaiduMessageTypeDef,
         "DefaultMessage": DefaultMessageTypeDef,
@@ -5685,51 +5493,49 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
-
 class UpdateInAppTemplateRequestRequestTypeDef(
     _RequiredUpdateInAppTemplateRequestRequestTypeDef,
     _OptionalUpdateInAppTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 GetInAppTemplateResponseTypeDef = TypedDict(
     "GetInAppTemplateResponseTypeDef",
     {
         "InAppTemplateResponse": InAppTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetApplicationDateRangeKpiResponseTypeDef = TypedDict(
     "GetApplicationDateRangeKpiResponseTypeDef",
     {
         "ApplicationDateRangeKpiResponse": ApplicationDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCampaignDateRangeKpiResponseTypeDef = TypedDict(
     "GetCampaignDateRangeKpiResponseTypeDef",
     {
         "CampaignDateRangeKpiResponse": CampaignDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJourneyDateRangeKpiResponseTypeDef = TypedDict(
     "GetJourneyDateRangeKpiResponseTypeDef",
     {
         "JourneyDateRangeKpiResponse": JourneyDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMessageRequestTypeDef = TypedDict(
     "_RequiredMessageRequestTypeDef",
     {
         "MessageConfiguration": DirectMessageConfigurationTypeDef,
@@ -5743,19 +5549,17 @@
         "Endpoints": Mapping[str, EndpointSendConfigurationTypeDef],
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TraceId": str,
     },
     total=False,
 )
 
-
 class MessageRequestTypeDef(_RequiredMessageRequestTypeDef, _OptionalMessageRequestTypeDef):
     pass
 
-
 _RequiredSendUsersMessageRequestTypeDef = TypedDict(
     "_RequiredSendUsersMessageRequestTypeDef",
     {
         "MessageConfiguration": DirectMessageConfigurationTypeDef,
         "Users": Mapping[str, EndpointSendConfigurationTypeDef],
     },
 )
@@ -5765,21 +5569,19 @@
         "Context": Mapping[str, str],
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TraceId": str,
     },
     total=False,
 )
 
-
 class SendUsersMessageRequestTypeDef(
     _RequiredSendUsersMessageRequestTypeDef, _OptionalSendUsersMessageRequestTypeDef
 ):
     pass
 
-
 SegmentGroupListTypeDef = TypedDict(
     "SegmentGroupListTypeDef",
     {
         "Groups": Sequence[SegmentGroupTypeDef],
         "Include": IncludeType,
     },
     total=False,
@@ -5820,21 +5622,19 @@
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TreatmentDescription": str,
         "TreatmentName": str,
     },
     total=False,
 )
 
-
 class TreatmentResourceTypeDef(
     _RequiredTreatmentResourceTypeDef, _OptionalTreatmentResourceTypeDef
 ):
     pass
 
-
 _RequiredWriteTreatmentResourceTypeDef = TypedDict(
     "_RequiredWriteTreatmentResourceTypeDef",
     {
         "SizePercent": int,
     },
 )
 _OptionalWriteTreatmentResourceTypeDef = TypedDict(
@@ -5846,21 +5646,19 @@
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TreatmentDescription": str,
         "TreatmentName": str,
     },
     total=False,
 )
 
-
 class WriteTreatmentResourceTypeDef(
     _RequiredWriteTreatmentResourceTypeDef, _OptionalWriteTreatmentResourceTypeDef
 ):
     pass
 
-
 InAppMessagesResponseTypeDef = TypedDict(
     "InAppMessagesResponseTypeDef",
     {
         "InAppMessageCampaigns": List[InAppMessageCampaignTypeDef],
     },
     total=False,
 )
@@ -5901,19 +5699,17 @@
         "SegmentGroups": SegmentGroupListTypeDef,
         "tags": Dict[str, str],
         "Version": int,
     },
     total=False,
 )
 
-
 class SegmentResponseTypeDef(_RequiredSegmentResponseTypeDef, _OptionalSegmentResponseTypeDef):
     pass
 
-
 WriteSegmentRequestTypeDef = TypedDict(
     "WriteSegmentRequestTypeDef",
     {
         "Dimensions": SegmentDimensionsTypeDef,
         "Name": str,
         "SegmentGroups": SegmentGroupListTypeDef,
         "tags": Mapping[str, str],
@@ -5975,19 +5771,17 @@
         "TreatmentName": str,
         "Version": int,
         "Priority": int,
     },
     total=False,
 )
 
-
 class CampaignResponseTypeDef(_RequiredCampaignResponseTypeDef, _OptionalCampaignResponseTypeDef):
     pass
 
-
 WriteCampaignRequestTypeDef = TypedDict(
     "WriteCampaignRequestTypeDef",
     {
         "AdditionalTreatments": Sequence[WriteTreatmentResourceTypeDef],
         "CustomDeliveryConfiguration": CustomDeliveryConfigurationTypeDef,
         "Description": str,
         "HoldoutPercent": int,
@@ -6008,47 +5802,47 @@
     total=False,
 )
 
 GetInAppMessagesResponseTypeDef = TypedDict(
     "GetInAppMessagesResponseTypeDef",
     {
         "InAppMessagesResponse": InAppMessagesResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSegmentResponseTypeDef = TypedDict(
     "CreateSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSegmentResponseTypeDef = TypedDict(
     "DeleteSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentResponseTypeDef = TypedDict(
     "GetSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentVersionResponseTypeDef = TypedDict(
     "GetSegmentVersionResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSegmentsResponseTypeDef = TypedDict(
     "_RequiredSegmentsResponseTypeDef",
     {
         "Item": List[SegmentResponseTypeDef],
@@ -6058,24 +5852,22 @@
     "_OptionalSegmentsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class SegmentsResponseTypeDef(_RequiredSegmentsResponseTypeDef, _OptionalSegmentsResponseTypeDef):
     pass
 
-
 UpdateSegmentResponseTypeDef = TypedDict(
     "UpdateSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSegmentRequestRequestTypeDef = TypedDict(
     "CreateSegmentRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -6120,58 +5912,56 @@
     "_OptionalCampaignsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class CampaignsResponseTypeDef(
     _RequiredCampaignsResponseTypeDef, _OptionalCampaignsResponseTypeDef
 ):
     pass
 
-
 CreateCampaignResponseTypeDef = TypedDict(
     "CreateCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteCampaignResponseTypeDef = TypedDict(
     "DeleteCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCampaignResponseTypeDef = TypedDict(
     "GetCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCampaignVersionResponseTypeDef = TypedDict(
     "GetCampaignVersionResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCampaignResponseTypeDef = TypedDict(
     "UpdateCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCampaignRequestRequestTypeDef = TypedDict(
     "CreateCampaignRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -6188,23 +5978,23 @@
     },
 )
 
 GetSegmentVersionsResponseTypeDef = TypedDict(
     "GetSegmentVersionsResponseTypeDef",
     {
         "SegmentsResponse": SegmentsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentsResponseTypeDef = TypedDict(
     "GetSegmentsResponseTypeDef",
     {
         "SegmentsResponse": SegmentsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredJourneyResponseTypeDef = TypedDict(
     "_RequiredJourneyResponseTypeDef",
     {
         "ApplicationId": str,
@@ -6229,23 +6019,22 @@
         "tags": Dict[str, str],
         "WaitForQuietTime": bool,
         "RefreshOnSegmentUpdate": bool,
         "JourneyChannelSettings": JourneyChannelSettingsTypeDef,
         "SendingSchedule": bool,
         "OpenHours": OpenHoursTypeDef,
         "ClosedDays": ClosedDaysTypeDef,
+        "TimezoneEstimationMethods": List[TimezoneEstimationMethodsElementType],
     },
     total=False,
 )
 
-
 class JourneyResponseTypeDef(_RequiredJourneyResponseTypeDef, _OptionalJourneyResponseTypeDef):
     pass
 
-
 _RequiredWriteJourneyRequestTypeDef = TypedDict(
     "_RequiredWriteJourneyRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalWriteJourneyRequestTypeDef = TypedDict(
@@ -6264,62 +6053,61 @@
         "State": StateType,
         "WaitForQuietTime": bool,
         "RefreshOnSegmentUpdate": bool,
         "JourneyChannelSettings": JourneyChannelSettingsTypeDef,
         "SendingSchedule": bool,
         "OpenHours": OpenHoursTypeDef,
         "ClosedDays": ClosedDaysTypeDef,
+        "TimezoneEstimationMethods": Sequence[TimezoneEstimationMethodsElementType],
     },
     total=False,
 )
 
-
 class WriteJourneyRequestTypeDef(
     _RequiredWriteJourneyRequestTypeDef, _OptionalWriteJourneyRequestTypeDef
 ):
     pass
 
-
 GetCampaignVersionsResponseTypeDef = TypedDict(
     "GetCampaignVersionsResponseTypeDef",
     {
         "CampaignsResponse": CampaignsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCampaignsResponseTypeDef = TypedDict(
     "GetCampaignsResponseTypeDef",
     {
         "CampaignsResponse": CampaignsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateJourneyResponseTypeDef = TypedDict(
     "CreateJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteJourneyResponseTypeDef = TypedDict(
     "DeleteJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJourneyResponseTypeDef = TypedDict(
     "GetJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredJourneysResponseTypeDef = TypedDict(
     "_RequiredJourneysResponseTypeDef",
     {
         "Item": List[JourneyResponseTypeDef],
@@ -6329,32 +6117,30 @@
     "_OptionalJourneysResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class JourneysResponseTypeDef(_RequiredJourneysResponseTypeDef, _OptionalJourneysResponseTypeDef):
     pass
 
-
 UpdateJourneyResponseTypeDef = TypedDict(
     "UpdateJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateJourneyStateResponseTypeDef = TypedDict(
     "UpdateJourneyStateResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateJourneyRequestRequestTypeDef = TypedDict(
     "CreateJourneyRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -6371,10 +6157,10 @@
     },
 )
 
 ListJourneysResponseTypeDef = TypedDict(
     "ListJourneysResponseTypeDef",
     {
         "JourneysResponse": JourneysResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint/type_defs.pyi` & `mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,22 +40,24 @@
     ModeType,
     OperatorType,
     RecencyTypeType,
     SegmentTypeType,
     SourceTypeType,
     StateType,
     TemplateTypeType,
+    TimezoneEstimationMethodsElementType,
     TypeType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ADMChannelRequestTypeDef",
     "ADMChannelResponseTypeDef",
     "ADMMessageTypeDef",
     "APNSChannelRequestTypeDef",
     "APNSChannelResponseTypeDef",
     "APNSMessageTypeDef",
@@ -85,15 +87,14 @@
     "CampaignStateTypeDef",
     "CustomDeliveryConfigurationTypeDef",
     "CampaignSmsMessageTypeDef",
     "ChannelResponseTypeDef",
     "ClosedDaysRuleTypeDef",
     "WaitTimeTypeDef",
     "CreateApplicationRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "EmailTemplateRequestTypeDef",
     "CreateTemplateMessageBodyTypeDef",
     "ExportJobRequestTypeDef",
     "ImportJobRequestTypeDef",
     "TemplateCreateMessageBodyTypeDef",
     "CreateRecommenderConfigurationTypeDef",
     "RecommenderConfigurationResponseTypeDef",
@@ -136,14 +137,15 @@
     "GCMMessageTypeDef",
     "SMSMessageTypeDef",
     "VoiceMessageTypeDef",
     "EmailChannelRequestTypeDef",
     "JourneyEmailMessageTypeDef",
     "RawEmailTypeDef",
     "EmailTemplateResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EndpointDemographicTypeDef",
     "EndpointLocationTypeDef",
     "EndpointUserTypeDef",
     "EndpointItemResponseTypeDef",
     "EndpointMessageResultTypeDef",
     "EndpointSendConfigurationTypeDef",
     "MetricDimensionTypeDef",
@@ -229,14 +231,15 @@
     "NumberValidateRequestTypeDef",
     "NumberValidateResponseTypeDef",
     "OpenHoursRuleTypeDef",
     "WriteEventStreamTypeDef",
     "RandomSplitEntryTypeDef",
     "RecencyDimensionTypeDef",
     "UpdateAttributesRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ResultRowValueTypeDef",
     "SMSChannelRequestTypeDef",
     "SegmentConditionTypeDef",
     "SegmentReferenceTypeDef",
     "SegmentImportResourceTypeDef",
     "SendOTPMessageRequestParametersTypeDef",
     "SimpleEmailPartTypeDef",
@@ -246,50 +249,49 @@
     "TemplateVersionResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateRecommenderConfigurationTypeDef",
     "VoiceChannelRequestTypeDef",
     "VerificationResponseTypeDef",
     "VerifyOTPMessageRequestParametersTypeDef",
     "UpdateAdmChannelRequestRequestTypeDef",
+    "DeleteAdmChannelResponseTypeDef",
+    "GetAdmChannelResponseTypeDef",
+    "UpdateAdmChannelResponseTypeDef",
     "UpdateApnsChannelRequestRequestTypeDef",
+    "DeleteApnsChannelResponseTypeDef",
+    "GetApnsChannelResponseTypeDef",
+    "UpdateApnsChannelResponseTypeDef",
     "UpdateApnsSandboxChannelRequestRequestTypeDef",
+    "DeleteApnsSandboxChannelResponseTypeDef",
+    "GetApnsSandboxChannelResponseTypeDef",
+    "UpdateApnsSandboxChannelResponseTypeDef",
     "UpdateApnsVoipChannelRequestRequestTypeDef",
+    "DeleteApnsVoipChannelResponseTypeDef",
+    "GetApnsVoipChannelResponseTypeDef",
+    "UpdateApnsVoipChannelResponseTypeDef",
     "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
+    "DeleteApnsVoipSandboxChannelResponseTypeDef",
+    "GetApnsVoipSandboxChannelResponseTypeDef",
+    "UpdateApnsVoipSandboxChannelResponseTypeDef",
     "ActivitiesResponseTypeDef",
     "ApplicationsResponseTypeDef",
+    "CreateAppResponseTypeDef",
+    "DeleteAppResponseTypeDef",
+    "GetAppResponseTypeDef",
     "ApplicationSettingsResourceTypeDef",
     "WriteApplicationSettingsRequestTypeDef",
+    "RemoveAttributesResponseTypeDef",
     "UpdateBaiduChannelRequestRequestTypeDef",
+    "DeleteBaiduChannelResponseTypeDef",
+    "GetBaiduChannelResponseTypeDef",
+    "UpdateBaiduChannelResponseTypeDef",
     "ChannelsResponseTypeDef",
     "ClosedDaysTypeDef",
     "WaitActivityTypeDef",
     "CreateAppRequestRequestTypeDef",
-    "CreateAppResponseTypeDef",
-    "DeleteAdmChannelResponseTypeDef",
-    "DeleteApnsChannelResponseTypeDef",
-    "DeleteApnsSandboxChannelResponseTypeDef",
-    "DeleteApnsVoipChannelResponseTypeDef",
-    "DeleteApnsVoipSandboxChannelResponseTypeDef",
-    "DeleteAppResponseTypeDef",
-    "DeleteBaiduChannelResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetAdmChannelResponseTypeDef",
-    "GetApnsChannelResponseTypeDef",
-    "GetApnsSandboxChannelResponseTypeDef",
-    "GetApnsVoipChannelResponseTypeDef",
-    "GetApnsVoipSandboxChannelResponseTypeDef",
-    "GetAppResponseTypeDef",
-    "GetBaiduChannelResponseTypeDef",
-    "RemoveAttributesResponseTypeDef",
-    "UpdateAdmChannelResponseTypeDef",
-    "UpdateApnsChannelResponseTypeDef",
-    "UpdateApnsSandboxChannelResponseTypeDef",
-    "UpdateApnsVoipChannelResponseTypeDef",
-    "UpdateApnsVoipSandboxChannelResponseTypeDef",
-    "UpdateBaiduChannelResponseTypeDef",
     "CreateEmailTemplateRequestRequestTypeDef",
     "UpdateEmailTemplateRequestRequestTypeDef",
     "CreateEmailTemplateResponseTypeDef",
     "CreatePushTemplateResponseTypeDef",
     "CreateSmsTemplateResponseTypeDef",
     "CreateVoiceTemplateResponseTypeDef",
     "CreateExportJobRequestRequestTypeDef",
@@ -516,19 +518,21 @@
     "_OptionalADMChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+
 class ADMChannelRequestTypeDef(
     _RequiredADMChannelRequestTypeDef, _OptionalADMChannelRequestTypeDef
 ):
     pass
 
+
 _RequiredADMChannelResponseTypeDef = TypedDict(
     "_RequiredADMChannelResponseTypeDef",
     {
         "Platform": str,
     },
 )
 _OptionalADMChannelResponseTypeDef = TypedDict(
@@ -543,19 +547,21 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class ADMChannelResponseTypeDef(
     _RequiredADMChannelResponseTypeDef, _OptionalADMChannelResponseTypeDef
 ):
     pass
 
+
 ADMMessageTypeDef = TypedDict(
     "ADMMessageTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "ConsolidationKey": str,
         "Data": Mapping[str, str],
@@ -610,19 +616,21 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class APNSChannelResponseTypeDef(
     _RequiredAPNSChannelResponseTypeDef, _OptionalAPNSChannelResponseTypeDef
 ):
     pass
 
+
 APNSMessageTypeDef = TypedDict(
     "APNSMessageTypeDef",
     {
         "APNSPushType": str,
         "Action": ActionType,
         "Badge": int,
         "Body": str,
@@ -693,19 +701,21 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class APNSSandboxChannelResponseTypeDef(
     _RequiredAPNSSandboxChannelResponseTypeDef, _OptionalAPNSSandboxChannelResponseTypeDef
 ):
     pass
 
+
 APNSVoipChannelRequestTypeDef = TypedDict(
     "APNSVoipChannelRequestTypeDef",
     {
         "BundleId": str,
         "Certificate": str,
         "DefaultAuthenticationMethod": str,
         "Enabled": bool,
@@ -737,19 +747,21 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class APNSVoipChannelResponseTypeDef(
     _RequiredAPNSVoipChannelResponseTypeDef, _OptionalAPNSVoipChannelResponseTypeDef
 ):
     pass
 
+
 APNSVoipSandboxChannelRequestTypeDef = TypedDict(
     "APNSVoipSandboxChannelRequestTypeDef",
     {
         "BundleId": str,
         "Certificate": str,
         "DefaultAuthenticationMethod": str,
         "Enabled": bool,
@@ -781,19 +793,21 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class APNSVoipSandboxChannelResponseTypeDef(
     _RequiredAPNSVoipSandboxChannelResponseTypeDef, _OptionalAPNSVoipSandboxChannelResponseTypeDef
 ):
     pass
 
+
 _RequiredActivityResponseTypeDef = TypedDict(
     "_RequiredActivityResponseTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
         "Id": str,
     },
@@ -812,17 +826,19 @@
         "TotalEndpointCount": int,
         "TreatmentId": str,
         "ExecutionMetrics": Dict[str, str],
     },
     total=False,
 )
 
+
 class ActivityResponseTypeDef(_RequiredActivityResponseTypeDef, _OptionalActivityResponseTypeDef):
     pass
 
+
 ContactCenterActivityTypeDef = TypedDict(
     "ContactCenterActivityTypeDef",
     {
         "NextActivity": str,
     },
     total=False,
 )
@@ -837,17 +853,19 @@
     "_OptionalHoldoutActivityTypeDef",
     {
         "NextActivity": str,
     },
     total=False,
 )
 
+
 class HoldoutActivityTypeDef(_RequiredHoldoutActivityTypeDef, _OptionalHoldoutActivityTypeDef):
     pass
 
+
 AddressConfigurationTypeDef = TypedDict(
     "AddressConfigurationTypeDef",
     {
         "BodyOverride": str,
         "ChannelType": ChannelTypeType,
         "Context": Mapping[str, str],
         "RawContent": str,
@@ -886,19 +904,21 @@
     {
         "tags": Dict[str, str],
         "CreationDate": str,
     },
     total=False,
 )
 
+
 class ApplicationResponseTypeDef(
     _RequiredApplicationResponseTypeDef, _OptionalApplicationResponseTypeDef
 ):
     pass
 
+
 CampaignHookTypeDef = TypedDict(
     "CampaignHookTypeDef",
     {
         "LambdaFunctionName": str,
         "Mode": ModeType,
         "WebUrl": str,
     },
@@ -936,19 +956,21 @@
     "_OptionalAttributeDimensionTypeDef",
     {
         "AttributeType": AttributeTypeType,
     },
     total=False,
 )
 
+
 class AttributeDimensionTypeDef(
     _RequiredAttributeDimensionTypeDef, _OptionalAttributeDimensionTypeDef
 ):
     pass
 
+
 _RequiredAttributesResourceTypeDef = TypedDict(
     "_RequiredAttributesResourceTypeDef",
     {
         "ApplicationId": str,
         "AttributeType": str,
     },
 )
@@ -956,19 +978,21 @@
     "_OptionalAttributesResourceTypeDef",
     {
         "Attributes": List[str],
     },
     total=False,
 )
 
+
 class AttributesResourceTypeDef(
     _RequiredAttributesResourceTypeDef, _OptionalAttributesResourceTypeDef
 ):
     pass
 
+
 _RequiredBaiduChannelRequestTypeDef = TypedDict(
     "_RequiredBaiduChannelRequestTypeDef",
     {
         "ApiKey": str,
         "SecretKey": str,
     },
 )
@@ -976,19 +1000,21 @@
     "_OptionalBaiduChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+
 class BaiduChannelRequestTypeDef(
     _RequiredBaiduChannelRequestTypeDef, _OptionalBaiduChannelRequestTypeDef
 ):
     pass
 
+
 _RequiredBaiduChannelResponseTypeDef = TypedDict(
     "_RequiredBaiduChannelResponseTypeDef",
     {
         "Credential": str,
         "Platform": str,
     },
 )
@@ -1004,19 +1030,21 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class BaiduChannelResponseTypeDef(
     _RequiredBaiduChannelResponseTypeDef, _OptionalBaiduChannelResponseTypeDef
 ):
     pass
 
+
 BaiduMessageTypeDef = TypedDict(
     "BaiduMessageTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "Data": Mapping[str, str],
         "IconReference": str,
@@ -1071,19 +1099,21 @@
     "_OptionalCustomDeliveryConfigurationTypeDef",
     {
         "EndpointTypes": Sequence[EndpointTypesElementType],
     },
     total=False,
 )
 
+
 class CustomDeliveryConfigurationTypeDef(
     _RequiredCustomDeliveryConfigurationTypeDef, _OptionalCustomDeliveryConfigurationTypeDef
 ):
     pass
 
+
 CampaignSmsMessageTypeDef = TypedDict(
     "CampaignSmsMessageTypeDef",
     {
         "Body": str,
         "MessageType": MessageTypeType,
         "OriginationNumber": str,
         "SenderId": str,
@@ -1138,29 +1168,20 @@
     "_OptionalCreateApplicationRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateApplicationRequestTypeDef(
     _RequiredCreateApplicationRequestTypeDef, _OptionalCreateApplicationRequestTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
 
 EmailTemplateRequestTypeDef = TypedDict(
     "EmailTemplateRequestTypeDef",
     {
         "DefaultSubstitutions": str,
         "HtmlPart": str,
         "RecommenderId": str,
@@ -1194,17 +1215,19 @@
     {
         "SegmentId": str,
         "SegmentVersion": int,
     },
     total=False,
 )
 
+
 class ExportJobRequestTypeDef(_RequiredExportJobRequestTypeDef, _OptionalExportJobRequestTypeDef):
     pass
 
+
 _RequiredImportJobRequestTypeDef = TypedDict(
     "_RequiredImportJobRequestTypeDef",
     {
         "Format": FormatType,
         "RoleArn": str,
         "S3Url": str,
     },
@@ -1217,17 +1240,19 @@
         "RegisterEndpoints": bool,
         "SegmentId": str,
         "SegmentName": str,
     },
     total=False,
 )
 
+
 class ImportJobRequestTypeDef(_RequiredImportJobRequestTypeDef, _OptionalImportJobRequestTypeDef):
     pass
 
+
 TemplateCreateMessageBodyTypeDef = TypedDict(
     "TemplateCreateMessageBodyTypeDef",
     {
         "Arn": str,
         "Message": str,
         "RequestID": str,
     },
@@ -1251,19 +1276,21 @@
         "RecommendationTransformerUri": str,
         "RecommendationsDisplayName": str,
         "RecommendationsPerMessage": int,
     },
     total=False,
 )
 
+
 class CreateRecommenderConfigurationTypeDef(
     _RequiredCreateRecommenderConfigurationTypeDef, _OptionalCreateRecommenderConfigurationTypeDef
 ):
     pass
 
+
 _RequiredRecommenderConfigurationResponseTypeDef = TypedDict(
     "_RequiredRecommenderConfigurationResponseTypeDef",
     {
         "CreationDate": str,
         "Id": str,
         "LastModifiedDate": str,
         "RecommendationProviderRoleArn": str,
@@ -1280,20 +1307,22 @@
         "RecommendationTransformerUri": str,
         "RecommendationsDisplayName": str,
         "RecommendationsPerMessage": int,
     },
     total=False,
 )
 
+
 class RecommenderConfigurationResponseTypeDef(
     _RequiredRecommenderConfigurationResponseTypeDef,
     _OptionalRecommenderConfigurationResponseTypeDef,
 ):
     pass
 
+
 SMSTemplateRequestTypeDef = TypedDict(
     "SMSTemplateRequestTypeDef",
     {
         "Body": str,
         "DefaultSubstitutions": str,
         "RecommenderId": str,
         "tags": Mapping[str, str],
@@ -1337,19 +1366,21 @@
         "BorderRadius": int,
         "Link": str,
         "TextColor": str,
     },
     total=False,
 )
 
+
 class DefaultButtonConfigurationTypeDef(
     _RequiredDefaultButtonConfigurationTypeDef, _OptionalDefaultButtonConfigurationTypeDef
 ):
     pass
 
+
 DefaultMessageTypeDef = TypedDict(
     "DefaultMessageTypeDef",
     {
         "Body": str,
         "Substitutions": Mapping[str, Sequence[str]],
     },
     total=False,
@@ -1468,39 +1499,43 @@
         "MessagesPerSecond": int,
         "RoleArn": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class EmailChannelResponseTypeDef(
     _RequiredEmailChannelResponseTypeDef, _OptionalEmailChannelResponseTypeDef
 ):
     pass
 
+
 _RequiredDeleteEmailTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteEmailTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteEmailTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class DeleteEmailTemplateRequestRequestTypeDef(
     _RequiredDeleteEmailTemplateRequestRequestTypeDef,
     _OptionalDeleteEmailTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 MessageBodyTypeDef = TypedDict(
     "MessageBodyTypeDef",
     {
         "Message": str,
         "RequestID": str,
     },
     total=False,
@@ -1535,17 +1570,19 @@
         "ExternalId": str,
         "LastModifiedDate": str,
         "LastUpdatedBy": str,
     },
     total=False,
 )
 
+
 class EventStreamTypeDef(_RequiredEventStreamTypeDef, _OptionalEventStreamTypeDef):
     pass
 
+
 DeleteGcmChannelRequestRequestTypeDef = TypedDict(
     "DeleteGcmChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -1568,39 +1605,43 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class GCMChannelResponseTypeDef(
     _RequiredGCMChannelResponseTypeDef, _OptionalGCMChannelResponseTypeDef
 ):
     pass
 
+
 _RequiredDeleteInAppTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteInAppTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteInAppTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteInAppTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class DeleteInAppTemplateRequestRequestTypeDef(
     _RequiredDeleteInAppTemplateRequestRequestTypeDef,
     _OptionalDeleteInAppTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteJourneyRequestRequestTypeDef = TypedDict(
     "DeleteJourneyRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
     },
 )
@@ -1615,20 +1656,22 @@
     "_OptionalDeletePushTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class DeletePushTemplateRequestRequestTypeDef(
     _RequiredDeletePushTemplateRequestRequestTypeDef,
     _OptionalDeletePushTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteRecommenderConfigurationRequestRequestTypeDef",
     {
         "RecommenderId": str,
     },
 )
 
@@ -1669,38 +1712,42 @@
         "ShortCode": str,
         "TransactionalMessagesPerSecond": int,
         "Version": int,
     },
     total=False,
 )
 
+
 class SMSChannelResponseTypeDef(
     _RequiredSMSChannelResponseTypeDef, _OptionalSMSChannelResponseTypeDef
 ):
     pass
 
+
 _RequiredDeleteSmsTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteSmsTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteSmsTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteSmsTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class DeleteSmsTemplateRequestRequestTypeDef(
     _RequiredDeleteSmsTemplateRequestRequestTypeDef, _OptionalDeleteSmsTemplateRequestRequestTypeDef
 ):
     pass
 
+
 DeleteUserEndpointsRequestRequestTypeDef = TypedDict(
     "DeleteUserEndpointsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "UserId": str,
     },
 )
@@ -1730,39 +1777,43 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class VoiceChannelResponseTypeDef(
     _RequiredVoiceChannelResponseTypeDef, _OptionalVoiceChannelResponseTypeDef
 ):
     pass
 
+
 _RequiredDeleteVoiceTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteVoiceTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteVoiceTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteVoiceTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class DeleteVoiceTemplateRequestRequestTypeDef(
     _RequiredDeleteVoiceTemplateRequestRequestTypeDef,
     _OptionalDeleteVoiceTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 GCMMessageTypeDef = TypedDict(
     "GCMMessageTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "CollapseKey": str,
         "Data": Mapping[str, str],
@@ -1824,19 +1875,21 @@
         "ConfigurationSet": str,
         "Enabled": bool,
         "RoleArn": str,
     },
     total=False,
 )
 
+
 class EmailChannelRequestTypeDef(
     _RequiredEmailChannelRequestTypeDef, _OptionalEmailChannelRequestTypeDef
 ):
     pass
 
+
 JourneyEmailMessageTypeDef = TypedDict(
     "JourneyEmailMessageTypeDef",
     {
         "FromAddress": str,
     },
     total=False,
 )
@@ -1870,19 +1923,28 @@
         "TemplateDescription": str,
         "TextPart": str,
         "Version": str,
     },
     total=False,
 )
 
+
 class EmailTemplateResponseTypeDef(
     _RequiredEmailTemplateResponseTypeDef, _OptionalEmailTemplateResponseTypeDef
 ):
     pass
 
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EndpointDemographicTypeDef = TypedDict(
     "EndpointDemographicTypeDef",
     {
         "AppVersion": str,
         "Locale": str,
         "Make": str,
         "Model": str,
@@ -1939,19 +2001,21 @@
         "MessageId": str,
         "StatusMessage": str,
         "UpdatedToken": str,
     },
     total=False,
 )
 
+
 class EndpointMessageResultTypeDef(
     _RequiredEndpointMessageResultTypeDef, _OptionalEndpointMessageResultTypeDef
 ):
     pass
 
+
 EndpointSendConfigurationTypeDef = TypedDict(
     "EndpointSendConfigurationTypeDef",
     {
         "BodyOverride": str,
         "Context": Mapping[str, str],
         "RawContent": str,
         "Substitutions": Mapping[str, Sequence[str]],
@@ -1978,17 +2042,19 @@
     "_OptionalSetDimensionTypeDef",
     {
         "DimensionType": DimensionTypeType,
     },
     total=False,
 )
 
+
 class SetDimensionTypeDef(_RequiredSetDimensionTypeDef, _OptionalSetDimensionTypeDef):
     pass
 
+
 EventItemResponseTypeDef = TypedDict(
     "EventItemResponseTypeDef",
     {
         "Message": str,
         "StatusCode": int,
     },
     total=False,
@@ -2006,17 +2072,19 @@
     {
         "Duration": int,
         "StopTimestamp": str,
     },
     total=False,
 )
 
+
 class SessionTypeDef(_RequiredSessionTypeDef, _OptionalSessionTypeDef):
     pass
 
+
 _RequiredExportJobResourceTypeDef = TypedDict(
     "_RequiredExportJobResourceTypeDef",
     {
         "RoleArn": str,
         "S3UrlPrefix": str,
     },
 )
@@ -2025,38 +2093,42 @@
     {
         "SegmentId": str,
         "SegmentVersion": int,
     },
     total=False,
 )
 
+
 class ExportJobResourceTypeDef(
     _RequiredExportJobResourceTypeDef, _OptionalExportJobResourceTypeDef
 ):
     pass
 
+
 _RequiredGCMChannelRequestTypeDef = TypedDict(
     "_RequiredGCMChannelRequestTypeDef",
     {
         "ApiKey": str,
     },
 )
 _OptionalGCMChannelRequestTypeDef = TypedDict(
     "_OptionalGCMChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+
 class GCMChannelRequestTypeDef(
     _RequiredGCMChannelRequestTypeDef, _OptionalGCMChannelRequestTypeDef
 ):
     pass
 
+
 GPSCoordinatesTypeDef = TypedDict(
     "GPSCoordinatesTypeDef",
     {
         "Latitude": float,
         "Longitude": float,
     },
 )
@@ -2117,20 +2189,22 @@
         "NextToken": str,
         "PageSize": str,
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class GetApplicationDateRangeKpiRequestRequestTypeDef(
     _RequiredGetApplicationDateRangeKpiRequestRequestTypeDef,
     _OptionalGetApplicationDateRangeKpiRequestRequestTypeDef,
 ):
     pass
 
+
 GetApplicationSettingsRequestRequestTypeDef = TypedDict(
     "GetApplicationSettingsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2162,20 +2236,22 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetCampaignActivitiesRequestRequestTypeDef(
     _RequiredGetCampaignActivitiesRequestRequestTypeDef,
     _OptionalGetCampaignActivitiesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetCampaignDateRangeKpiRequestRequestTypeDef = TypedDict(
     "_RequiredGetCampaignDateRangeKpiRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
         "KpiName": str,
     },
@@ -2187,20 +2263,22 @@
         "NextToken": str,
         "PageSize": str,
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class GetCampaignDateRangeKpiRequestRequestTypeDef(
     _RequiredGetCampaignDateRangeKpiRequestRequestTypeDef,
     _OptionalGetCampaignDateRangeKpiRequestRequestTypeDef,
 ):
     pass
 
+
 GetCampaignRequestRequestTypeDef = TypedDict(
     "GetCampaignRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
     },
 )
@@ -2226,20 +2304,22 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetCampaignVersionsRequestRequestTypeDef(
     _RequiredGetCampaignVersionsRequestRequestTypeDef,
     _OptionalGetCampaignVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetCampaignsRequestRequestTypeDef = TypedDict(
     "_RequiredGetCampaignsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalGetCampaignsRequestRequestTypeDef = TypedDict(
@@ -2247,19 +2327,21 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetCampaignsRequestRequestTypeDef(
     _RequiredGetCampaignsRequestRequestTypeDef, _OptionalGetCampaignsRequestRequestTypeDef
 ):
     pass
 
+
 GetChannelsRequestRequestTypeDef = TypedDict(
     "GetChannelsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2280,19 +2362,21 @@
     "_OptionalGetEmailTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class GetEmailTemplateRequestRequestTypeDef(
     _RequiredGetEmailTemplateRequestRequestTypeDef, _OptionalGetEmailTemplateRequestRequestTypeDef
 ):
     pass
 
+
 GetEndpointRequestRequestTypeDef = TypedDict(
     "GetEndpointRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EndpointId": str,
     },
 )
@@ -2323,19 +2407,21 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetExportJobsRequestRequestTypeDef(
     _RequiredGetExportJobsRequestRequestTypeDef, _OptionalGetExportJobsRequestRequestTypeDef
 ):
     pass
 
+
 GetGcmChannelRequestRequestTypeDef = TypedDict(
     "GetGcmChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2358,19 +2444,21 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetImportJobsRequestRequestTypeDef(
     _RequiredGetImportJobsRequestRequestTypeDef, _OptionalGetImportJobsRequestRequestTypeDef
 ):
     pass
 
+
 GetInAppMessagesRequestRequestTypeDef = TypedDict(
     "GetInAppMessagesRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EndpointId": str,
     },
 )
@@ -2385,19 +2473,21 @@
     "_OptionalGetInAppTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class GetInAppTemplateRequestRequestTypeDef(
     _RequiredGetInAppTemplateRequestRequestTypeDef, _OptionalGetInAppTemplateRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetJourneyDateRangeKpiRequestRequestTypeDef = TypedDict(
     "_RequiredGetJourneyDateRangeKpiRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
         "KpiName": str,
     },
@@ -2409,20 +2499,22 @@
         "NextToken": str,
         "PageSize": str,
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class GetJourneyDateRangeKpiRequestRequestTypeDef(
     _RequiredGetJourneyDateRangeKpiRequestRequestTypeDef,
     _OptionalGetJourneyDateRangeKpiRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetJourneyExecutionActivityMetricsRequestRequestTypeDef = TypedDict(
     "_RequiredGetJourneyExecutionActivityMetricsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "JourneyActivityId": str,
         "JourneyId": str,
     },
@@ -2432,20 +2524,22 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
+
 class GetJourneyExecutionActivityMetricsRequestRequestTypeDef(
     _RequiredGetJourneyExecutionActivityMetricsRequestRequestTypeDef,
     _OptionalGetJourneyExecutionActivityMetricsRequestRequestTypeDef,
 ):
     pass
 
+
 JourneyExecutionActivityMetricsResponseTypeDef = TypedDict(
     "JourneyExecutionActivityMetricsResponseTypeDef",
     {
         "ActivityType": str,
         "ApplicationId": str,
         "JourneyActivityId": str,
         "JourneyId": str,
@@ -2466,20 +2560,22 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
+
 class GetJourneyExecutionMetricsRequestRequestTypeDef(
     _RequiredGetJourneyExecutionMetricsRequestRequestTypeDef,
     _OptionalGetJourneyExecutionMetricsRequestRequestTypeDef,
 ):
     pass
 
+
 JourneyExecutionMetricsResponseTypeDef = TypedDict(
     "JourneyExecutionMetricsResponseTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
         "LastEvaluatedTime": str,
         "Metrics": Dict[str, str],
@@ -2508,20 +2604,22 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
+
 class GetJourneyRunExecutionActivityMetricsRequestRequestTypeDef(
     _RequiredGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef,
     _OptionalGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef,
 ):
     pass
 
+
 JourneyRunExecutionActivityMetricsResponseTypeDef = TypedDict(
     "JourneyRunExecutionActivityMetricsResponseTypeDef",
     {
         "ActivityType": str,
         "ApplicationId": str,
         "JourneyActivityId": str,
         "JourneyId": str,
@@ -2544,20 +2642,22 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
+
 class GetJourneyRunExecutionMetricsRequestRequestTypeDef(
     _RequiredGetJourneyRunExecutionMetricsRequestRequestTypeDef,
     _OptionalGetJourneyRunExecutionMetricsRequestRequestTypeDef,
 ):
     pass
 
+
 JourneyRunExecutionMetricsResponseTypeDef = TypedDict(
     "JourneyRunExecutionMetricsResponseTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
         "LastEvaluatedTime": str,
         "Metrics": Dict[str, str],
@@ -2577,38 +2677,42 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetJourneyRunsRequestRequestTypeDef(
     _RequiredGetJourneyRunsRequestRequestTypeDef, _OptionalGetJourneyRunsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetPushTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredGetPushTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalGetPushTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalGetPushTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class GetPushTemplateRequestRequestTypeDef(
     _RequiredGetPushTemplateRequestRequestTypeDef, _OptionalGetPushTemplateRequestRequestTypeDef
 ):
     pass
 
+
 GetRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "GetRecommenderConfigurationRequestRequestTypeDef",
     {
         "RecommenderId": str,
     },
 )
 
@@ -2633,20 +2737,22 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetSegmentExportJobsRequestRequestTypeDef(
     _RequiredGetSegmentExportJobsRequestRequestTypeDef,
     _OptionalGetSegmentExportJobsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetSegmentImportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSegmentImportJobsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "SegmentId": str,
     },
 )
@@ -2655,20 +2761,22 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetSegmentImportJobsRequestRequestTypeDef(
     _RequiredGetSegmentImportJobsRequestRequestTypeDef,
     _OptionalGetSegmentImportJobsRequestRequestTypeDef,
 ):
     pass
 
+
 GetSegmentRequestRequestTypeDef = TypedDict(
     "GetSegmentRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "SegmentId": str,
     },
 )
@@ -2694,20 +2802,22 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetSegmentVersionsRequestRequestTypeDef(
     _RequiredGetSegmentVersionsRequestRequestTypeDef,
     _OptionalGetSegmentVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetSegmentsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSegmentsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalGetSegmentsRequestRequestTypeDef = TypedDict(
@@ -2715,19 +2825,21 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetSegmentsRequestRequestTypeDef(
     _RequiredGetSegmentsRequestRequestTypeDef, _OptionalGetSegmentsRequestRequestTypeDef
 ):
     pass
 
+
 GetSmsChannelRequestRequestTypeDef = TypedDict(
     "GetSmsChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2741,19 +2853,21 @@
     "_OptionalGetSmsTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class GetSmsTemplateRequestRequestTypeDef(
     _RequiredGetSmsTemplateRequestRequestTypeDef, _OptionalGetSmsTemplateRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredSMSTemplateResponseTypeDef = TypedDict(
     "_RequiredSMSTemplateResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": TemplateTypeType,
@@ -2769,19 +2883,21 @@
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
+
 class SMSTemplateResponseTypeDef(
     _RequiredSMSTemplateResponseTypeDef, _OptionalSMSTemplateResponseTypeDef
 ):
     pass
 
+
 GetUserEndpointsRequestRequestTypeDef = TypedDict(
     "GetUserEndpointsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "UserId": str,
     },
 )
@@ -2803,19 +2919,21 @@
     "_OptionalGetVoiceTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class GetVoiceTemplateRequestRequestTypeDef(
     _RequiredGetVoiceTemplateRequestRequestTypeDef, _OptionalGetVoiceTemplateRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredVoiceTemplateResponseTypeDef = TypedDict(
     "_RequiredVoiceTemplateResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": TemplateTypeType,
@@ -2832,19 +2950,21 @@
         "TemplateDescription": str,
         "Version": str,
         "VoiceId": str,
     },
     total=False,
 )
 
+
 class VoiceTemplateResponseTypeDef(
     _RequiredVoiceTemplateResponseTypeDef, _OptionalVoiceTemplateResponseTypeDef
 ):
     pass
 
+
 _RequiredImportJobResourceTypeDef = TypedDict(
     "_RequiredImportJobResourceTypeDef",
     {
         "Format": FormatType,
         "RoleArn": str,
         "S3Url": str,
     },
@@ -2857,19 +2977,21 @@
         "RegisterEndpoints": bool,
         "SegmentId": str,
         "SegmentName": str,
     },
     total=False,
 )
 
+
 class ImportJobResourceTypeDef(
     _RequiredImportJobResourceTypeDef, _OptionalImportJobResourceTypeDef
 ):
     pass
 
+
 InAppMessageBodyConfigTypeDef = TypedDict(
     "InAppMessageBodyConfigTypeDef",
     {
         "Alignment": AlignmentType,
         "Body": str,
         "TextColor": str,
     },
@@ -2885,19 +3007,21 @@
     "_OptionalOverrideButtonConfigurationTypeDef",
     {
         "Link": str,
     },
     total=False,
 )
 
+
 class OverrideButtonConfigurationTypeDef(
     _RequiredOverrideButtonConfigurationTypeDef, _OptionalOverrideButtonConfigurationTypeDef
 ):
     pass
 
+
 InAppMessageHeaderConfigTypeDef = TypedDict(
     "InAppMessageHeaderConfigTypeDef",
     {
         "Alignment": AlignmentType,
         "Header": str,
         "TextColor": str,
     },
@@ -2982,19 +3106,21 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class ListJourneysRequestRequestTypeDef(
     _RequiredListJourneysRequestRequestTypeDef, _OptionalListJourneysRequestRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -3017,20 +3143,22 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
+
 class ListTemplateVersionsRequestRequestTypeDef(
     _RequiredListTemplateVersionsRequestRequestTypeDef,
     _OptionalListTemplateVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ListTemplatesRequestRequestTypeDef = TypedDict(
     "ListTemplatesRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": str,
         "Prefix": str,
         "TemplateType": str,
@@ -3070,17 +3198,19 @@
         "MessageId": str,
         "StatusMessage": str,
         "UpdatedToken": str,
     },
     total=False,
 )
 
+
 class MessageResultTypeDef(_RequiredMessageResultTypeDef, _OptionalMessageResultTypeDef):
     pass
 
+
 NumberValidateRequestTypeDef = TypedDict(
     "NumberValidateRequestTypeDef",
     {
         "IsoCountryCode": str,
         "PhoneNumber": str,
     },
     total=False,
@@ -3145,14 +3275,25 @@
     "UpdateAttributesRequestTypeDef",
     {
         "Blacklist": Sequence[str],
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 ResultRowValueTypeDef = TypedDict(
     "ResultRowValueTypeDef",
     {
         "Key": str,
         "Type": str,
         "Value": str,
     },
@@ -3185,17 +3326,19 @@
     "_OptionalSegmentReferenceTypeDef",
     {
         "Version": int,
     },
     total=False,
 )
 
+
 class SegmentReferenceTypeDef(_RequiredSegmentReferenceTypeDef, _OptionalSegmentReferenceTypeDef):
     pass
 
+
 _RequiredSegmentImportResourceTypeDef = TypedDict(
     "_RequiredSegmentImportResourceTypeDef",
     {
         "ExternalId": str,
         "Format": FormatType,
         "RoleArn": str,
         "S3Url": str,
@@ -3206,19 +3349,21 @@
     "_OptionalSegmentImportResourceTypeDef",
     {
         "ChannelCounts": Dict[str, int],
     },
     total=False,
 )
 
+
 class SegmentImportResourceTypeDef(
     _RequiredSegmentImportResourceTypeDef, _OptionalSegmentImportResourceTypeDef
 ):
     pass
 
+
 _RequiredSendOTPMessageRequestParametersTypeDef = TypedDict(
     "_RequiredSendOTPMessageRequestParametersTypeDef",
     {
         "BrandName": str,
         "Channel": str,
         "DestinationIdentity": str,
         "OriginationIdentity": str,
@@ -3234,19 +3379,21 @@
         "Language": str,
         "TemplateId": str,
         "ValidityPeriod": int,
     },
     total=False,
 )
 
+
 class SendOTPMessageRequestParametersTypeDef(
     _RequiredSendOTPMessageRequestParametersTypeDef, _OptionalSendOTPMessageRequestParametersTypeDef
 ):
     pass
 
+
 SimpleEmailPartTypeDef = TypedDict(
     "SimpleEmailPartTypeDef",
     {
         "Charset": str,
         "Data": str,
     },
     total=False,
@@ -3286,17 +3433,19 @@
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
+
 class TemplateResponseTypeDef(_RequiredTemplateResponseTypeDef, _OptionalTemplateResponseTypeDef):
     pass
 
+
 _RequiredTemplateVersionResponseTypeDef = TypedDict(
     "_RequiredTemplateVersionResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": str,
@@ -3308,19 +3457,21 @@
         "DefaultSubstitutions": str,
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
+
 class TemplateVersionResponseTypeDef(
     _RequiredTemplateVersionResponseTypeDef, _OptionalTemplateVersionResponseTypeDef
 ):
     pass
 
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -3342,19 +3493,21 @@
         "RecommendationTransformerUri": str,
         "RecommendationsDisplayName": str,
         "RecommendationsPerMessage": int,
     },
     total=False,
 )
 
+
 class UpdateRecommenderConfigurationTypeDef(
     _RequiredUpdateRecommenderConfigurationTypeDef, _OptionalUpdateRecommenderConfigurationTypeDef
 ):
     pass
 
+
 VoiceChannelRequestTypeDef = TypedDict(
     "VoiceChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -3380,331 +3533,328 @@
     "UpdateAdmChannelRequestRequestTypeDef",
     {
         "ADMChannelRequest": ADMChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
 
-UpdateApnsChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsChannelRequestRequestTypeDef",
+DeleteAdmChannelResponseTypeDef = TypedDict(
+    "DeleteAdmChannelResponseTypeDef",
     {
-        "APNSChannelRequest": APNSChannelRequestTypeDef,
-        "ApplicationId": str,
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateApnsSandboxChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsSandboxChannelRequestRequestTypeDef",
+GetAdmChannelResponseTypeDef = TypedDict(
+    "GetAdmChannelResponseTypeDef",
     {
-        "APNSSandboxChannelRequest": APNSSandboxChannelRequestTypeDef,
-        "ApplicationId": str,
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateApnsVoipChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsVoipChannelRequestRequestTypeDef",
+UpdateAdmChannelResponseTypeDef = TypedDict(
+    "UpdateAdmChannelResponseTypeDef",
     {
-        "APNSVoipChannelRequest": APNSVoipChannelRequestTypeDef,
-        "ApplicationId": str,
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateApnsVoipSandboxChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
+UpdateApnsChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsChannelRequestRequestTypeDef",
     {
-        "APNSVoipSandboxChannelRequest": APNSVoipSandboxChannelRequestTypeDef,
+        "APNSChannelRequest": APNSChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
 
-_RequiredActivitiesResponseTypeDef = TypedDict(
-    "_RequiredActivitiesResponseTypeDef",
+DeleteApnsChannelResponseTypeDef = TypedDict(
+    "DeleteApnsChannelResponseTypeDef",
     {
-        "Item": List[ActivityResponseTypeDef],
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalActivitiesResponseTypeDef = TypedDict(
-    "_OptionalActivitiesResponseTypeDef",
+
+GetApnsChannelResponseTypeDef = TypedDict(
+    "GetApnsChannelResponseTypeDef",
     {
-        "NextToken": str,
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class ActivitiesResponseTypeDef(
-    _RequiredActivitiesResponseTypeDef, _OptionalActivitiesResponseTypeDef
-):
-    pass
-
-ApplicationsResponseTypeDef = TypedDict(
-    "ApplicationsResponseTypeDef",
+UpdateApnsChannelResponseTypeDef = TypedDict(
+    "UpdateApnsChannelResponseTypeDef",
     {
-        "Item": List[ApplicationResponseTypeDef],
-        "NextToken": str,
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-_RequiredApplicationSettingsResourceTypeDef = TypedDict(
-    "_RequiredApplicationSettingsResourceTypeDef",
+UpdateApnsSandboxChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsSandboxChannelRequestRequestTypeDef",
     {
+        "APNSSandboxChannelRequest": APNSSandboxChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
-_OptionalApplicationSettingsResourceTypeDef = TypedDict(
-    "_OptionalApplicationSettingsResourceTypeDef",
+
+DeleteApnsSandboxChannelResponseTypeDef = TypedDict(
+    "DeleteApnsSandboxChannelResponseTypeDef",
     {
-        "CampaignHook": CampaignHookTypeDef,
-        "LastModifiedDate": str,
-        "Limits": CampaignLimitsTypeDef,
-        "QuietTime": QuietTimeTypeDef,
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class ApplicationSettingsResourceTypeDef(
-    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
-):
-    pass
+GetApnsSandboxChannelResponseTypeDef = TypedDict(
+    "GetApnsSandboxChannelResponseTypeDef",
+    {
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
-WriteApplicationSettingsRequestTypeDef = TypedDict(
-    "WriteApplicationSettingsRequestTypeDef",
+UpdateApnsSandboxChannelResponseTypeDef = TypedDict(
+    "UpdateApnsSandboxChannelResponseTypeDef",
     {
-        "CampaignHook": CampaignHookTypeDef,
-        "CloudWatchMetricsEnabled": bool,
-        "EventTaggingEnabled": bool,
-        "Limits": CampaignLimitsTypeDef,
-        "QuietTime": QuietTimeTypeDef,
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-UpdateBaiduChannelRequestRequestTypeDef = TypedDict(
-    "UpdateBaiduChannelRequestRequestTypeDef",
+UpdateApnsVoipChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsVoipChannelRequestRequestTypeDef",
     {
+        "APNSVoipChannelRequest": APNSVoipChannelRequestTypeDef,
         "ApplicationId": str,
-        "BaiduChannelRequest": BaiduChannelRequestTypeDef,
     },
 )
 
-ChannelsResponseTypeDef = TypedDict(
-    "ChannelsResponseTypeDef",
+DeleteApnsVoipChannelResponseTypeDef = TypedDict(
+    "DeleteApnsVoipChannelResponseTypeDef",
     {
-        "Channels": Dict[str, ChannelResponseTypeDef],
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ClosedDaysTypeDef = TypedDict(
-    "ClosedDaysTypeDef",
+GetApnsVoipChannelResponseTypeDef = TypedDict(
+    "GetApnsVoipChannelResponseTypeDef",
     {
-        "EMAIL": Sequence[ClosedDaysRuleTypeDef],
-        "SMS": Sequence[ClosedDaysRuleTypeDef],
-        "PUSH": Sequence[ClosedDaysRuleTypeDef],
-        "VOICE": Sequence[ClosedDaysRuleTypeDef],
-        "CUSTOM": Sequence[ClosedDaysRuleTypeDef],
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-WaitActivityTypeDef = TypedDict(
-    "WaitActivityTypeDef",
+UpdateApnsVoipChannelResponseTypeDef = TypedDict(
+    "UpdateApnsVoipChannelResponseTypeDef",
     {
-        "NextActivity": str,
-        "WaitTime": WaitTimeTypeDef,
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-CreateAppRequestRequestTypeDef = TypedDict(
-    "CreateAppRequestRequestTypeDef",
+UpdateApnsVoipSandboxChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
     {
-        "CreateApplicationRequest": CreateApplicationRequestTypeDef,
+        "APNSVoipSandboxChannelRequest": APNSVoipSandboxChannelRequestTypeDef,
+        "ApplicationId": str,
     },
 )
 
-CreateAppResponseTypeDef = TypedDict(
-    "CreateAppResponseTypeDef",
+DeleteApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "DeleteApnsVoipSandboxChannelResponseTypeDef",
     {
-        "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteAdmChannelResponseTypeDef = TypedDict(
-    "DeleteAdmChannelResponseTypeDef",
+GetApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "GetApnsVoipSandboxChannelResponseTypeDef",
     {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteApnsChannelResponseTypeDef = TypedDict(
-    "DeleteApnsChannelResponseTypeDef",
+UpdateApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "UpdateApnsVoipSandboxChannelResponseTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteApnsSandboxChannelResponseTypeDef = TypedDict(
-    "DeleteApnsSandboxChannelResponseTypeDef",
+_RequiredActivitiesResponseTypeDef = TypedDict(
+    "_RequiredActivitiesResponseTypeDef",
     {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Item": List[ActivityResponseTypeDef],
     },
 )
-
-DeleteApnsVoipChannelResponseTypeDef = TypedDict(
-    "DeleteApnsVoipChannelResponseTypeDef",
+_OptionalActivitiesResponseTypeDef = TypedDict(
+    "_OptionalActivitiesResponseTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": str,
     },
+    total=False,
 )
 
-DeleteApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "DeleteApnsVoipSandboxChannelResponseTypeDef",
+
+class ActivitiesResponseTypeDef(
+    _RequiredActivitiesResponseTypeDef, _OptionalActivitiesResponseTypeDef
+):
+    pass
+
+
+ApplicationsResponseTypeDef = TypedDict(
+    "ApplicationsResponseTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Item": List[ApplicationResponseTypeDef],
+        "NextToken": str,
     },
+    total=False,
 )
 
-DeleteAppResponseTypeDef = TypedDict(
-    "DeleteAppResponseTypeDef",
+CreateAppResponseTypeDef = TypedDict(
+    "CreateAppResponseTypeDef",
     {
         "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteBaiduChannelResponseTypeDef = TypedDict(
-    "DeleteBaiduChannelResponseTypeDef",
+DeleteAppResponseTypeDef = TypedDict(
+    "DeleteAppResponseTypeDef",
     {
-        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationResponse": ApplicationResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+GetAppResponseTypeDef = TypedDict(
+    "GetAppResponseTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationResponse": ApplicationResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetAdmChannelResponseTypeDef = TypedDict(
-    "GetAdmChannelResponseTypeDef",
+_RequiredApplicationSettingsResourceTypeDef = TypedDict(
+    "_RequiredApplicationSettingsResourceTypeDef",
     {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationId": str,
     },
 )
-
-GetApnsChannelResponseTypeDef = TypedDict(
-    "GetApnsChannelResponseTypeDef",
+_OptionalApplicationSettingsResourceTypeDef = TypedDict(
+    "_OptionalApplicationSettingsResourceTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CampaignHook": CampaignHookTypeDef,
+        "LastModifiedDate": str,
+        "Limits": CampaignLimitsTypeDef,
+        "QuietTime": QuietTimeTypeDef,
     },
+    total=False,
 )
 
-GetApnsSandboxChannelResponseTypeDef = TypedDict(
-    "GetApnsSandboxChannelResponseTypeDef",
+
+class ApplicationSettingsResourceTypeDef(
+    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
+):
+    pass
+
+
+WriteApplicationSettingsRequestTypeDef = TypedDict(
+    "WriteApplicationSettingsRequestTypeDef",
     {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CampaignHook": CampaignHookTypeDef,
+        "CloudWatchMetricsEnabled": bool,
+        "EventTaggingEnabled": bool,
+        "Limits": CampaignLimitsTypeDef,
+        "QuietTime": QuietTimeTypeDef,
     },
+    total=False,
 )
 
-GetApnsVoipChannelResponseTypeDef = TypedDict(
-    "GetApnsVoipChannelResponseTypeDef",
+RemoveAttributesResponseTypeDef = TypedDict(
+    "RemoveAttributesResponseTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AttributesResource": AttributesResourceTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "GetApnsVoipSandboxChannelResponseTypeDef",
+UpdateBaiduChannelRequestRequestTypeDef = TypedDict(
+    "UpdateBaiduChannelRequestRequestTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationId": str,
+        "BaiduChannelRequest": BaiduChannelRequestTypeDef,
     },
 )
 
-GetAppResponseTypeDef = TypedDict(
-    "GetAppResponseTypeDef",
+DeleteBaiduChannelResponseTypeDef = TypedDict(
+    "DeleteBaiduChannelResponseTypeDef",
     {
-        "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBaiduChannelResponseTypeDef = TypedDict(
     "GetBaiduChannelResponseTypeDef",
     {
         "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveAttributesResponseTypeDef = TypedDict(
-    "RemoveAttributesResponseTypeDef",
-    {
-        "AttributesResource": AttributesResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateAdmChannelResponseTypeDef = TypedDict(
-    "UpdateAdmChannelResponseTypeDef",
-    {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateApnsChannelResponseTypeDef = TypedDict(
-    "UpdateApnsChannelResponseTypeDef",
+UpdateBaiduChannelResponseTypeDef = TypedDict(
+    "UpdateBaiduChannelResponseTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateApnsSandboxChannelResponseTypeDef = TypedDict(
-    "UpdateApnsSandboxChannelResponseTypeDef",
+ChannelsResponseTypeDef = TypedDict(
+    "ChannelsResponseTypeDef",
     {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Channels": Dict[str, ChannelResponseTypeDef],
     },
 )
 
-UpdateApnsVoipChannelResponseTypeDef = TypedDict(
-    "UpdateApnsVoipChannelResponseTypeDef",
+ClosedDaysTypeDef = TypedDict(
+    "ClosedDaysTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "EMAIL": Sequence[ClosedDaysRuleTypeDef],
+        "SMS": Sequence[ClosedDaysRuleTypeDef],
+        "PUSH": Sequence[ClosedDaysRuleTypeDef],
+        "VOICE": Sequence[ClosedDaysRuleTypeDef],
+        "CUSTOM": Sequence[ClosedDaysRuleTypeDef],
     },
+    total=False,
 )
 
-UpdateApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "UpdateApnsVoipSandboxChannelResponseTypeDef",
+WaitActivityTypeDef = TypedDict(
+    "WaitActivityTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextActivity": str,
+        "WaitTime": WaitTimeTypeDef,
     },
+    total=False,
 )
 
-UpdateBaiduChannelResponseTypeDef = TypedDict(
-    "UpdateBaiduChannelResponseTypeDef",
+CreateAppRequestRequestTypeDef = TypedDict(
+    "CreateAppRequestRequestTypeDef",
     {
-        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CreateApplicationRequest": CreateApplicationRequestTypeDef,
     },
 )
 
 CreateEmailTemplateRequestRequestTypeDef = TypedDict(
     "CreateEmailTemplateRequestRequestTypeDef",
     {
         "EmailTemplateRequest": EmailTemplateRequestTypeDef,
@@ -3724,49 +3874,51 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
+
 class UpdateEmailTemplateRequestRequestTypeDef(
     _RequiredUpdateEmailTemplateRequestRequestTypeDef,
     _OptionalUpdateEmailTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 CreateEmailTemplateResponseTypeDef = TypedDict(
     "CreateEmailTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePushTemplateResponseTypeDef = TypedDict(
     "CreatePushTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSmsTemplateResponseTypeDef = TypedDict(
     "CreateSmsTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateVoiceTemplateResponseTypeDef = TypedDict(
     "CreateVoiceTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateExportJobRequestRequestTypeDef = TypedDict(
     "CreateExportJobRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -3782,46 +3934,46 @@
     },
 )
 
 CreateInAppTemplateResponseTypeDef = TypedDict(
     "CreateInAppTemplateResponseTypeDef",
     {
         "TemplateCreateMessageBody": TemplateCreateMessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "CreateRecommenderConfigurationRequestRequestTypeDef",
     {
         "CreateRecommenderConfiguration": CreateRecommenderConfigurationTypeDef,
     },
 )
 
 CreateRecommenderConfigurationResponseTypeDef = TypedDict(
     "CreateRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRecommenderConfigurationResponseTypeDef = TypedDict(
     "DeleteRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRecommenderConfigurationResponseTypeDef = TypedDict(
     "GetRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListRecommenderConfigurationsResponseTypeDef = TypedDict(
     "_RequiredListRecommenderConfigurationsResponseTypeDef",
     {
         "Item": List[RecommenderConfigurationResponseTypeDef],
@@ -3831,25 +3983,27 @@
     "_OptionalListRecommenderConfigurationsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListRecommenderConfigurationsResponseTypeDef(
     _RequiredListRecommenderConfigurationsResponseTypeDef,
     _OptionalListRecommenderConfigurationsResponseTypeDef,
 ):
     pass
 
+
 UpdateRecommenderConfigurationResponseTypeDef = TypedDict(
     "UpdateRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSmsTemplateRequestRequestTypeDef = TypedDict(
     "CreateSmsTemplateRequestRequestTypeDef",
     {
         "SMSTemplateRequest": SMSTemplateRequestTypeDef,
@@ -3869,19 +4023,21 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
+
 class UpdateSmsTemplateRequestRequestTypeDef(
     _RequiredUpdateSmsTemplateRequestRequestTypeDef, _OptionalUpdateSmsTemplateRequestRequestTypeDef
 ):
     pass
 
+
 CreateVoiceTemplateRequestRequestTypeDef = TypedDict(
     "CreateVoiceTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "VoiceTemplateRequest": VoiceTemplateRequestTypeDef,
     },
 )
@@ -3898,20 +4054,22 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
+
 class UpdateVoiceTemplateRequestRequestTypeDef(
     _RequiredUpdateVoiceTemplateRequestRequestTypeDef,
     _OptionalUpdateVoiceTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 CustomMessageActivityTypeDef = TypedDict(
     "CustomMessageActivityTypeDef",
     {
         "DeliveryUri": str,
         "EndpointTypes": Sequence[EndpointTypesElementType],
         "MessageConfig": JourneyCustomMessageTypeDef,
         "NextActivity": str,
@@ -3960,241 +4118,243 @@
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
+
 class PushNotificationTemplateResponseTypeDef(
     _RequiredPushNotificationTemplateResponseTypeDef,
     _OptionalPushNotificationTemplateResponseTypeDef,
 ):
     pass
 
+
 DeleteEmailChannelResponseTypeDef = TypedDict(
     "DeleteEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEmailChannelResponseTypeDef = TypedDict(
     "GetEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEmailChannelResponseTypeDef = TypedDict(
     "UpdateEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEmailTemplateResponseTypeDef = TypedDict(
     "DeleteEmailTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteInAppTemplateResponseTypeDef = TypedDict(
     "DeleteInAppTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeletePushTemplateResponseTypeDef = TypedDict(
     "DeletePushTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSmsTemplateResponseTypeDef = TypedDict(
     "DeleteSmsTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVoiceTemplateResponseTypeDef = TypedDict(
     "DeleteVoiceTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEmailTemplateResponseTypeDef = TypedDict(
     "UpdateEmailTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEndpointResponseTypeDef = TypedDict(
     "UpdateEndpointResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEndpointsBatchResponseTypeDef = TypedDict(
     "UpdateEndpointsBatchResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateInAppTemplateResponseTypeDef = TypedDict(
     "UpdateInAppTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePushTemplateResponseTypeDef = TypedDict(
     "UpdatePushTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSmsTemplateResponseTypeDef = TypedDict(
     "UpdateSmsTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTemplateActiveVersionResponseTypeDef = TypedDict(
     "UpdateTemplateActiveVersionResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVoiceTemplateResponseTypeDef = TypedDict(
     "UpdateVoiceTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEventStreamResponseTypeDef = TypedDict(
     "DeleteEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEventStreamResponseTypeDef = TypedDict(
     "GetEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutEventStreamResponseTypeDef = TypedDict(
     "PutEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteGcmChannelResponseTypeDef = TypedDict(
     "DeleteGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGcmChannelResponseTypeDef = TypedDict(
     "GetGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGcmChannelResponseTypeDef = TypedDict(
     "UpdateGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSmsChannelResponseTypeDef = TypedDict(
     "DeleteSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSmsChannelResponseTypeDef = TypedDict(
     "GetSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSmsChannelResponseTypeDef = TypedDict(
     "UpdateSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVoiceChannelResponseTypeDef = TypedDict(
     "DeleteVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceChannelResponseTypeDef = TypedDict(
     "GetVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVoiceChannelResponseTypeDef = TypedDict(
     "UpdateVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEmailChannelRequestRequestTypeDef = TypedDict(
     "UpdateEmailChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -4213,15 +4373,15 @@
     total=False,
 )
 
 GetEmailTemplateResponseTypeDef = TypedDict(
     "GetEmailTemplateResponseTypeDef",
     {
         "EmailTemplateResponse": EmailTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EndpointBatchItemTypeDef = TypedDict(
     "EndpointBatchItemTypeDef",
     {
         "Address": str,
@@ -4309,19 +4469,21 @@
     {
         "RequestId": str,
         "Result": Dict[str, Dict[str, EndpointMessageResultTypeDef]],
     },
     total=False,
 )
 
+
 class SendUsersMessageResponseTypeDef(
     _RequiredSendUsersMessageResponseTypeDef, _OptionalSendUsersMessageResponseTypeDef
 ):
     pass
 
+
 EventDimensionsTypeDef = TypedDict(
     "EventDimensionsTypeDef",
     {
         "Attributes": Mapping[str, AttributeDimensionTypeDef],
         "EventType": SetDimensionTypeDef,
         "Metrics": Mapping[str, MetricDimensionTypeDef],
     },
@@ -4368,17 +4530,19 @@
         "Metrics": Mapping[str, float],
         "SdkName": str,
         "Session": SessionTypeDef,
     },
     total=False,
 )
 
+
 class EventTypeDef(_RequiredEventTypeDef, _OptionalEventTypeDef):
     pass
 
+
 _RequiredExportJobResponseTypeDef = TypedDict(
     "_RequiredExportJobResponseTypeDef",
     {
         "ApplicationId": str,
         "CreationDate": str,
         "Definition": ExportJobResourceTypeDef,
         "Id": str,
@@ -4396,19 +4560,21 @@
         "TotalFailures": int,
         "TotalPieces": int,
         "TotalProcessed": int,
     },
     total=False,
 )
 
+
 class ExportJobResponseTypeDef(
     _RequiredExportJobResponseTypeDef, _OptionalExportJobResponseTypeDef
 ):
     pass
 
+
 UpdateGcmChannelRequestRequestTypeDef = TypedDict(
     "UpdateGcmChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "GCMChannelRequest": GCMChannelRequestTypeDef,
     },
 )
@@ -4423,66 +4589,68 @@
     "_OptionalGPSPointDimensionTypeDef",
     {
         "RangeInKilometers": float,
     },
     total=False,
 )
 
+
 class GPSPointDimensionTypeDef(
     _RequiredGPSPointDimensionTypeDef, _OptionalGPSPointDimensionTypeDef
 ):
     pass
 
+
 GetJourneyExecutionActivityMetricsResponseTypeDef = TypedDict(
     "GetJourneyExecutionActivityMetricsResponseTypeDef",
     {
         "JourneyExecutionActivityMetricsResponse": JourneyExecutionActivityMetricsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJourneyExecutionMetricsResponseTypeDef = TypedDict(
     "GetJourneyExecutionMetricsResponseTypeDef",
     {
         "JourneyExecutionMetricsResponse": JourneyExecutionMetricsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJourneyRunExecutionActivityMetricsResponseTypeDef = TypedDict(
     "GetJourneyRunExecutionActivityMetricsResponseTypeDef",
     {
         "JourneyRunExecutionActivityMetricsResponse": (
             JourneyRunExecutionActivityMetricsResponseTypeDef
         ),
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJourneyRunExecutionMetricsResponseTypeDef = TypedDict(
     "GetJourneyRunExecutionMetricsResponseTypeDef",
     {
         "JourneyRunExecutionMetricsResponse": JourneyRunExecutionMetricsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSmsTemplateResponseTypeDef = TypedDict(
     "GetSmsTemplateResponseTypeDef",
     {
         "SMSTemplateResponse": SMSTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceTemplateResponseTypeDef = TypedDict(
     "GetVoiceTemplateResponseTypeDef",
     {
         "VoiceTemplateResponse": VoiceTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredImportJobResponseTypeDef = TypedDict(
     "_RequiredImportJobResponseTypeDef",
     {
         "ApplicationId": str,
@@ -4503,19 +4671,21 @@
         "TotalFailures": int,
         "TotalPieces": int,
         "TotalProcessed": int,
     },
     total=False,
 )
 
+
 class ImportJobResponseTypeDef(
     _RequiredImportJobResponseTypeDef, _OptionalImportJobResponseTypeDef
 ):
     pass
 
+
 InAppMessageButtonTypeDef = TypedDict(
     "InAppMessageButtonTypeDef",
     {
         "Android": OverrideButtonConfigurationTypeDef,
         "DefaultConfig": DefaultButtonConfigurationTypeDef,
         "IOS": OverrideButtonConfigurationTypeDef,
         "Web": OverrideButtonConfigurationTypeDef,
@@ -4544,19 +4714,21 @@
     "_OptionalJourneyRunsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class JourneyRunsResponseTypeDef(
     _RequiredJourneyRunsResponseTypeDef, _OptionalJourneyRunsResponseTypeDef
 ):
     pass
 
+
 SMSMessageActivityTypeDef = TypedDict(
     "SMSMessageActivityTypeDef",
     {
         "MessageConfig": JourneySMSMessageTypeDef,
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
@@ -4573,15 +4745,15 @@
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "TagsModel": TagsModelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -4601,29 +4773,31 @@
         "EndpointResult": Dict[str, EndpointMessageResultTypeDef],
         "RequestId": str,
         "Result": Dict[str, MessageResultTypeDef],
     },
     total=False,
 )
 
+
 class MessageResponseTypeDef(_RequiredMessageResponseTypeDef, _OptionalMessageResponseTypeDef):
     pass
 
+
 PhoneNumberValidateRequestRequestTypeDef = TypedDict(
     "PhoneNumberValidateRequestRequestTypeDef",
     {
         "NumberValidateRequest": NumberValidateRequestTypeDef,
     },
 )
 
 PhoneNumberValidateResponseTypeDef = TypedDict(
     "PhoneNumberValidateResponseTypeDef",
     {
         "NumberValidateResponse": NumberValidateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OpenHoursTypeDef = TypedDict(
     "OpenHoursTypeDef",
     {
         "EMAIL": Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]],
@@ -4732,19 +4906,21 @@
     "_OptionalTemplatesResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class TemplatesResponseTypeDef(
     _RequiredTemplatesResponseTypeDef, _OptionalTemplatesResponseTypeDef
 ):
     pass
 
+
 _RequiredTemplateVersionsResponseTypeDef = TypedDict(
     "_RequiredTemplateVersionsResponseTypeDef",
     {
         "Item": List[TemplateVersionResponseTypeDef],
     },
 )
 _OptionalTemplateVersionsResponseTypeDef = TypedDict(
@@ -4753,19 +4929,21 @@
         "Message": str,
         "NextToken": str,
         "RequestID": str,
     },
     total=False,
 )
 
+
 class TemplateVersionsResponseTypeDef(
     _RequiredTemplateVersionsResponseTypeDef, _OptionalTemplateVersionsResponseTypeDef
 ):
     pass
 
+
 UpdateRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateRecommenderConfigurationRequestRequestTypeDef",
     {
         "RecommenderId": str,
         "UpdateRecommenderConfiguration": UpdateRecommenderConfigurationTypeDef,
     },
 )
@@ -4778,15 +4956,15 @@
     },
 )
 
 VerifyOTPMessageResponseTypeDef = TypedDict(
     "VerifyOTPMessageResponseTypeDef",
     {
         "VerificationResponse": VerificationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VerifyOTPMessageRequestRequestTypeDef = TypedDict(
     "VerifyOTPMessageRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -4794,39 +4972,39 @@
     },
 )
 
 GetCampaignActivitiesResponseTypeDef = TypedDict(
     "GetCampaignActivitiesResponseTypeDef",
     {
         "ActivitiesResponse": ActivitiesResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAppsResponseTypeDef = TypedDict(
     "GetAppsResponseTypeDef",
     {
         "ApplicationsResponse": ApplicationsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetApplicationSettingsResponseTypeDef = TypedDict(
     "GetApplicationSettingsResponseTypeDef",
     {
         "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateApplicationSettingsResponseTypeDef = TypedDict(
     "UpdateApplicationSettingsResponseTypeDef",
     {
         "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateApplicationSettingsRequestRequestTypeDef = TypedDict(
     "UpdateApplicationSettingsRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -4834,23 +5012,23 @@
     },
 )
 
 GetChannelsResponseTypeDef = TypedDict(
     "GetChannelsResponseTypeDef",
     {
         "ChannelsResponse": ChannelsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRecommenderConfigurationsResponseTypeDef = TypedDict(
     "GetRecommenderConfigurationsResponseTypeDef",
     {
         "ListRecommenderConfigurationsResponse": ListRecommenderConfigurationsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePushTemplateRequestRequestTypeDef = TypedDict(
     "CreatePushTemplateRequestRequestTypeDef",
     {
         "PushNotificationTemplateRequest": PushNotificationTemplateRequestTypeDef,
@@ -4870,25 +5048,27 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
+
 class UpdatePushTemplateRequestRequestTypeDef(
     _RequiredUpdatePushTemplateRequestRequestTypeDef,
     _OptionalUpdatePushTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 GetPushTemplateResponseTypeDef = TypedDict(
     "GetPushTemplateResponseTypeDef",
     {
         "PushNotificationTemplateResponse": PushNotificationTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EndpointBatchRequestTypeDef = TypedDict(
     "EndpointBatchRequestTypeDef",
     {
         "Item": Sequence[EndpointBatchItemTypeDef],
@@ -4904,38 +5084,38 @@
     },
 )
 
 DeleteEndpointResponseTypeDef = TypedDict(
     "DeleteEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EndpointsResponseTypeDef = TypedDict(
     "EndpointsResponseTypeDef",
     {
         "Item": List[EndpointResponseTypeDef],
     },
 )
 
 GetEndpointResponseTypeDef = TypedDict(
     "GetEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SendUsersMessagesResponseTypeDef = TypedDict(
     "SendUsersMessagesResponseTypeDef",
     {
         "SendUsersMessageResponse": SendUsersMessageResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CampaignEventFilterTypeDef = TypedDict(
     "CampaignEventFilterTypeDef",
     {
         "Dimensions": EventDimensionsTypeDef,
@@ -4976,15 +5156,15 @@
     },
 )
 
 CreateExportJobResponseTypeDef = TypedDict(
     "CreateExportJobResponseTypeDef",
     {
         "ExportJobResponse": ExportJobResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredExportJobsResponseTypeDef = TypedDict(
     "_RequiredExportJobsResponseTypeDef",
     {
         "Item": List[ExportJobResponseTypeDef],
@@ -4994,24 +5174,26 @@
     "_OptionalExportJobsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ExportJobsResponseTypeDef(
     _RequiredExportJobsResponseTypeDef, _OptionalExportJobsResponseTypeDef
 ):
     pass
 
+
 GetExportJobResponseTypeDef = TypedDict(
     "GetExportJobResponseTypeDef",
     {
         "ExportJobResponse": ExportJobResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SegmentLocationTypeDef = TypedDict(
     "SegmentLocationTypeDef",
     {
         "Country": SetDimensionTypeDef,
@@ -5020,23 +5202,23 @@
     total=False,
 )
 
 CreateImportJobResponseTypeDef = TypedDict(
     "CreateImportJobResponseTypeDef",
     {
         "ImportJobResponse": ImportJobResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetImportJobResponseTypeDef = TypedDict(
     "GetImportJobResponseTypeDef",
     {
         "ImportJobResponse": ImportJobResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredImportJobsResponseTypeDef = TypedDict(
     "_RequiredImportJobsResponseTypeDef",
     {
         "Item": List[ImportJobResponseTypeDef],
@@ -5046,19 +5228,21 @@
     "_OptionalImportJobsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ImportJobsResponseTypeDef(
     _RequiredImportJobsResponseTypeDef, _OptionalImportJobsResponseTypeDef
 ):
     pass
 
+
 InAppMessageContentTypeDef = TypedDict(
     "InAppMessageContentTypeDef",
     {
         "BackgroundColor": str,
         "BodyConfig": InAppMessageBodyConfigTypeDef,
         "HeaderConfig": InAppMessageHeaderConfigTypeDef,
         "ImageUrl": str,
@@ -5068,31 +5252,31 @@
     total=False,
 )
 
 GetJourneyRunsResponseTypeDef = TypedDict(
     "GetJourneyRunsResponseTypeDef",
     {
         "JourneyRunsResponse": JourneyRunsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SendMessagesResponseTypeDef = TypedDict(
     "SendMessagesResponseTypeDef",
     {
         "MessageResponse": MessageResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SendOTPMessageResponseTypeDef = TypedDict(
     "SendOTPMessageResponseTypeDef",
     {
         "MessageResponse": MessageResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BaseKpiResultTypeDef = TypedDict(
     "BaseKpiResultTypeDef",
     {
         "Rows": List[ResultRowTypeDef],
@@ -5113,23 +5297,23 @@
     total=False,
 )
 
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "TemplatesResponse": TemplatesResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTemplateVersionsResponseTypeDef = TypedDict(
     "ListTemplateVersionsResponseTypeDef",
     {
         "TemplateVersionsResponse": TemplateVersionsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEndpointsBatchRequestRequestTypeDef = TypedDict(
     "UpdateEndpointsBatchRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -5137,23 +5321,23 @@
     },
 )
 
 DeleteUserEndpointsResponseTypeDef = TypedDict(
     "DeleteUserEndpointsResponseTypeDef",
     {
         "EndpointsResponse": EndpointsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUserEndpointsResponseTypeDef = TypedDict(
     "GetUserEndpointsResponseTypeDef",
     {
         "EndpointsResponse": EndpointsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InAppCampaignScheduleTypeDef = TypedDict(
     "InAppCampaignScheduleTypeDef",
     {
         "EndDate": str,
@@ -5178,54 +5362,56 @@
         "IsLocalTime": bool,
         "QuietTime": QuietTimeTypeDef,
         "Timezone": str,
     },
     total=False,
 )
 
+
 class ScheduleTypeDef(_RequiredScheduleTypeDef, _OptionalScheduleTypeDef):
     pass
 
+
 EventStartConditionTypeDef = TypedDict(
     "EventStartConditionTypeDef",
     {
         "EventFilter": EventFilterTypeDef,
         "SegmentId": str,
     },
     total=False,
 )
 
 PutEventsResponseTypeDef = TypedDict(
     "PutEventsResponseTypeDef",
     {
         "EventsResponse": EventsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventsRequestTypeDef = TypedDict(
     "EventsRequestTypeDef",
     {
         "BatchItem": Mapping[str, EventsBatchTypeDef],
     },
 )
 
 GetExportJobsResponseTypeDef = TypedDict(
     "GetExportJobsResponseTypeDef",
     {
         "ExportJobsResponse": ExportJobsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentExportJobsResponseTypeDef = TypedDict(
     "GetSegmentExportJobsResponseTypeDef",
     {
         "ExportJobsResponse": ExportJobsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SegmentDimensionsTypeDef = TypedDict(
     "SegmentDimensionsTypeDef",
     {
         "Attributes": Mapping[str, AttributeDimensionTypeDef],
@@ -5238,23 +5424,23 @@
     total=False,
 )
 
 GetImportJobsResponseTypeDef = TypedDict(
     "GetImportJobsResponseTypeDef",
     {
         "ImportJobsResponse": ImportJobsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentImportJobsResponseTypeDef = TypedDict(
     "GetSegmentImportJobsResponseTypeDef",
     {
         "ImportJobsResponse": ImportJobsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CampaignInAppMessageTypeDef = TypedDict(
     "CampaignInAppMessageTypeDef",
     {
         "Body": str,
@@ -5306,19 +5492,21 @@
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
+
 class InAppTemplateResponseTypeDef(
     _RequiredInAppTemplateResponseTypeDef, _OptionalInAppTemplateResponseTypeDef
 ):
     pass
 
+
 _RequiredApplicationDateRangeKpiResponseTypeDef = TypedDict(
     "_RequiredApplicationDateRangeKpiResponseTypeDef",
     {
         "ApplicationId": str,
         "EndTime": datetime,
         "KpiName": str,
         "KpiResult": BaseKpiResultTypeDef,
@@ -5329,19 +5517,21 @@
     "_OptionalApplicationDateRangeKpiResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ApplicationDateRangeKpiResponseTypeDef(
     _RequiredApplicationDateRangeKpiResponseTypeDef, _OptionalApplicationDateRangeKpiResponseTypeDef
 ):
     pass
 
+
 _RequiredCampaignDateRangeKpiResponseTypeDef = TypedDict(
     "_RequiredCampaignDateRangeKpiResponseTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
         "EndTime": datetime,
         "KpiName": str,
@@ -5353,19 +5543,21 @@
     "_OptionalCampaignDateRangeKpiResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class CampaignDateRangeKpiResponseTypeDef(
     _RequiredCampaignDateRangeKpiResponseTypeDef, _OptionalCampaignDateRangeKpiResponseTypeDef
 ):
     pass
 
+
 _RequiredJourneyDateRangeKpiResponseTypeDef = TypedDict(
     "_RequiredJourneyDateRangeKpiResponseTypeDef",
     {
         "ApplicationId": str,
         "EndTime": datetime,
         "JourneyId": str,
         "KpiName": str,
@@ -5377,19 +5569,21 @@
     "_OptionalJourneyDateRangeKpiResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class JourneyDateRangeKpiResponseTypeDef(
     _RequiredJourneyDateRangeKpiResponseTypeDef, _OptionalJourneyDateRangeKpiResponseTypeDef
 ):
     pass
 
+
 DirectMessageConfigurationTypeDef = TypedDict(
     "DirectMessageConfigurationTypeDef",
     {
         "ADMMessage": ADMMessageTypeDef,
         "APNSMessage": APNSMessageTypeDef,
         "BaiduMessage": BaiduMessageTypeDef,
         "DefaultMessage": DefaultMessageTypeDef,
@@ -5492,49 +5686,51 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
+
 class UpdateInAppTemplateRequestRequestTypeDef(
     _RequiredUpdateInAppTemplateRequestRequestTypeDef,
     _OptionalUpdateInAppTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 GetInAppTemplateResponseTypeDef = TypedDict(
     "GetInAppTemplateResponseTypeDef",
     {
         "InAppTemplateResponse": InAppTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetApplicationDateRangeKpiResponseTypeDef = TypedDict(
     "GetApplicationDateRangeKpiResponseTypeDef",
     {
         "ApplicationDateRangeKpiResponse": ApplicationDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCampaignDateRangeKpiResponseTypeDef = TypedDict(
     "GetCampaignDateRangeKpiResponseTypeDef",
     {
         "CampaignDateRangeKpiResponse": CampaignDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJourneyDateRangeKpiResponseTypeDef = TypedDict(
     "GetJourneyDateRangeKpiResponseTypeDef",
     {
         "JourneyDateRangeKpiResponse": JourneyDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMessageRequestTypeDef = TypedDict(
     "_RequiredMessageRequestTypeDef",
     {
         "MessageConfiguration": DirectMessageConfigurationTypeDef,
@@ -5548,17 +5744,19 @@
         "Endpoints": Mapping[str, EndpointSendConfigurationTypeDef],
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TraceId": str,
     },
     total=False,
 )
 
+
 class MessageRequestTypeDef(_RequiredMessageRequestTypeDef, _OptionalMessageRequestTypeDef):
     pass
 
+
 _RequiredSendUsersMessageRequestTypeDef = TypedDict(
     "_RequiredSendUsersMessageRequestTypeDef",
     {
         "MessageConfiguration": DirectMessageConfigurationTypeDef,
         "Users": Mapping[str, EndpointSendConfigurationTypeDef],
     },
 )
@@ -5568,19 +5766,21 @@
         "Context": Mapping[str, str],
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TraceId": str,
     },
     total=False,
 )
 
+
 class SendUsersMessageRequestTypeDef(
     _RequiredSendUsersMessageRequestTypeDef, _OptionalSendUsersMessageRequestTypeDef
 ):
     pass
 
+
 SegmentGroupListTypeDef = TypedDict(
     "SegmentGroupListTypeDef",
     {
         "Groups": Sequence[SegmentGroupTypeDef],
         "Include": IncludeType,
     },
     total=False,
@@ -5621,19 +5821,21 @@
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TreatmentDescription": str,
         "TreatmentName": str,
     },
     total=False,
 )
 
+
 class TreatmentResourceTypeDef(
     _RequiredTreatmentResourceTypeDef, _OptionalTreatmentResourceTypeDef
 ):
     pass
 
+
 _RequiredWriteTreatmentResourceTypeDef = TypedDict(
     "_RequiredWriteTreatmentResourceTypeDef",
     {
         "SizePercent": int,
     },
 )
 _OptionalWriteTreatmentResourceTypeDef = TypedDict(
@@ -5645,19 +5847,21 @@
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TreatmentDescription": str,
         "TreatmentName": str,
     },
     total=False,
 )
 
+
 class WriteTreatmentResourceTypeDef(
     _RequiredWriteTreatmentResourceTypeDef, _OptionalWriteTreatmentResourceTypeDef
 ):
     pass
 
+
 InAppMessagesResponseTypeDef = TypedDict(
     "InAppMessagesResponseTypeDef",
     {
         "InAppMessageCampaigns": List[InAppMessageCampaignTypeDef],
     },
     total=False,
 )
@@ -5698,17 +5902,19 @@
         "SegmentGroups": SegmentGroupListTypeDef,
         "tags": Dict[str, str],
         "Version": int,
     },
     total=False,
 )
 
+
 class SegmentResponseTypeDef(_RequiredSegmentResponseTypeDef, _OptionalSegmentResponseTypeDef):
     pass
 
+
 WriteSegmentRequestTypeDef = TypedDict(
     "WriteSegmentRequestTypeDef",
     {
         "Dimensions": SegmentDimensionsTypeDef,
         "Name": str,
         "SegmentGroups": SegmentGroupListTypeDef,
         "tags": Mapping[str, str],
@@ -5770,17 +5976,19 @@
         "TreatmentName": str,
         "Version": int,
         "Priority": int,
     },
     total=False,
 )
 
+
 class CampaignResponseTypeDef(_RequiredCampaignResponseTypeDef, _OptionalCampaignResponseTypeDef):
     pass
 
+
 WriteCampaignRequestTypeDef = TypedDict(
     "WriteCampaignRequestTypeDef",
     {
         "AdditionalTreatments": Sequence[WriteTreatmentResourceTypeDef],
         "CustomDeliveryConfiguration": CustomDeliveryConfigurationTypeDef,
         "Description": str,
         "HoldoutPercent": int,
@@ -5801,47 +6009,47 @@
     total=False,
 )
 
 GetInAppMessagesResponseTypeDef = TypedDict(
     "GetInAppMessagesResponseTypeDef",
     {
         "InAppMessagesResponse": InAppMessagesResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSegmentResponseTypeDef = TypedDict(
     "CreateSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSegmentResponseTypeDef = TypedDict(
     "DeleteSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentResponseTypeDef = TypedDict(
     "GetSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentVersionResponseTypeDef = TypedDict(
     "GetSegmentVersionResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSegmentsResponseTypeDef = TypedDict(
     "_RequiredSegmentsResponseTypeDef",
     {
         "Item": List[SegmentResponseTypeDef],
@@ -5851,22 +6059,24 @@
     "_OptionalSegmentsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class SegmentsResponseTypeDef(_RequiredSegmentsResponseTypeDef, _OptionalSegmentsResponseTypeDef):
     pass
 
+
 UpdateSegmentResponseTypeDef = TypedDict(
     "UpdateSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSegmentRequestRequestTypeDef = TypedDict(
     "CreateSegmentRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -5911,56 +6121,58 @@
     "_OptionalCampaignsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class CampaignsResponseTypeDef(
     _RequiredCampaignsResponseTypeDef, _OptionalCampaignsResponseTypeDef
 ):
     pass
 
+
 CreateCampaignResponseTypeDef = TypedDict(
     "CreateCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteCampaignResponseTypeDef = TypedDict(
     "DeleteCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCampaignResponseTypeDef = TypedDict(
     "GetCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCampaignVersionResponseTypeDef = TypedDict(
     "GetCampaignVersionResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCampaignResponseTypeDef = TypedDict(
     "UpdateCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCampaignRequestRequestTypeDef = TypedDict(
     "CreateCampaignRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -5977,23 +6189,23 @@
     },
 )
 
 GetSegmentVersionsResponseTypeDef = TypedDict(
     "GetSegmentVersionsResponseTypeDef",
     {
         "SegmentsResponse": SegmentsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentsResponseTypeDef = TypedDict(
     "GetSegmentsResponseTypeDef",
     {
         "SegmentsResponse": SegmentsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredJourneyResponseTypeDef = TypedDict(
     "_RequiredJourneyResponseTypeDef",
     {
         "ApplicationId": str,
@@ -6018,21 +6230,24 @@
         "tags": Dict[str, str],
         "WaitForQuietTime": bool,
         "RefreshOnSegmentUpdate": bool,
         "JourneyChannelSettings": JourneyChannelSettingsTypeDef,
         "SendingSchedule": bool,
         "OpenHours": OpenHoursTypeDef,
         "ClosedDays": ClosedDaysTypeDef,
+        "TimezoneEstimationMethods": List[TimezoneEstimationMethodsElementType],
     },
     total=False,
 )
 
+
 class JourneyResponseTypeDef(_RequiredJourneyResponseTypeDef, _OptionalJourneyResponseTypeDef):
     pass
 
+
 _RequiredWriteJourneyRequestTypeDef = TypedDict(
     "_RequiredWriteJourneyRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalWriteJourneyRequestTypeDef = TypedDict(
@@ -6051,60 +6266,63 @@
         "State": StateType,
         "WaitForQuietTime": bool,
         "RefreshOnSegmentUpdate": bool,
         "JourneyChannelSettings": JourneyChannelSettingsTypeDef,
         "SendingSchedule": bool,
         "OpenHours": OpenHoursTypeDef,
         "ClosedDays": ClosedDaysTypeDef,
+        "TimezoneEstimationMethods": Sequence[TimezoneEstimationMethodsElementType],
     },
     total=False,
 )
 
+
 class WriteJourneyRequestTypeDef(
     _RequiredWriteJourneyRequestTypeDef, _OptionalWriteJourneyRequestTypeDef
 ):
     pass
 
+
 GetCampaignVersionsResponseTypeDef = TypedDict(
     "GetCampaignVersionsResponseTypeDef",
     {
         "CampaignsResponse": CampaignsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCampaignsResponseTypeDef = TypedDict(
     "GetCampaignsResponseTypeDef",
     {
         "CampaignsResponse": CampaignsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateJourneyResponseTypeDef = TypedDict(
     "CreateJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteJourneyResponseTypeDef = TypedDict(
     "DeleteJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJourneyResponseTypeDef = TypedDict(
     "GetJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredJourneysResponseTypeDef = TypedDict(
     "_RequiredJourneysResponseTypeDef",
     {
         "Item": List[JourneyResponseTypeDef],
@@ -6114,30 +6332,32 @@
     "_OptionalJourneysResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class JourneysResponseTypeDef(_RequiredJourneysResponseTypeDef, _OptionalJourneysResponseTypeDef):
     pass
 
+
 UpdateJourneyResponseTypeDef = TypedDict(
     "UpdateJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateJourneyStateResponseTypeDef = TypedDict(
     "UpdateJourneyStateResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateJourneyRequestRequestTypeDef = TypedDict(
     "CreateJourneyRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -6154,10 +6374,10 @@
     },
 )
 
 ListJourneysResponseTypeDef = TypedDict(
     "ListJourneysResponseTypeDef",
     {
         "JourneysResponse": JourneysResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint.egg-info/PKG-INFO` & `mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint
-Version: 1.26.138
-Summary: Type annotations for boto3.Pinpoint 1.26.138 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.161
+Summary: Type annotations for boto3.Pinpoint 1.26.161 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.26.138](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.26.161](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -301,14 +301,15 @@
     ModeType,
     OperatorType,
     RecencyTypeType,
     SegmentTypeType,
     SourceTypeType,
     StateType,
     TemplateTypeType,
+    TimezoneEstimationMethodsElementType,
     TypeType,
     PinpointServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
@@ -358,15 +359,14 @@
     CampaignStateTypeDef,
     CustomDeliveryConfigurationTypeDef,
     CampaignSmsMessageTypeDef,
     ChannelResponseTypeDef,
     ClosedDaysRuleTypeDef,
     WaitTimeTypeDef,
     CreateApplicationRequestTypeDef,
-    ResponseMetadataTypeDef,
     EmailTemplateRequestTypeDef,
     CreateTemplateMessageBodyTypeDef,
     ExportJobRequestTypeDef,
     ImportJobRequestTypeDef,
     TemplateCreateMessageBodyTypeDef,
     CreateRecommenderConfigurationTypeDef,
     RecommenderConfigurationResponseTypeDef,
@@ -409,14 +409,15 @@
     GCMMessageTypeDef,
     SMSMessageTypeDef,
     VoiceMessageTypeDef,
     EmailChannelRequestTypeDef,
     JourneyEmailMessageTypeDef,
     RawEmailTypeDef,
     EmailTemplateResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     EndpointDemographicTypeDef,
     EndpointLocationTypeDef,
     EndpointUserTypeDef,
     EndpointItemResponseTypeDef,
     EndpointMessageResultTypeDef,
     EndpointSendConfigurationTypeDef,
     MetricDimensionTypeDef,
@@ -502,14 +503,15 @@
     NumberValidateRequestTypeDef,
     NumberValidateResponseTypeDef,
     OpenHoursRuleTypeDef,
     WriteEventStreamTypeDef,
     RandomSplitEntryTypeDef,
     RecencyDimensionTypeDef,
     UpdateAttributesRequestTypeDef,
+    ResponseMetadataTypeDef,
     ResultRowValueTypeDef,
     SMSChannelRequestTypeDef,
     SegmentConditionTypeDef,
     SegmentReferenceTypeDef,
     SegmentImportResourceTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SimpleEmailPartTypeDef,
@@ -519,50 +521,49 @@
     TemplateVersionResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRecommenderConfigurationTypeDef,
     VoiceChannelRequestTypeDef,
     VerificationResponseTypeDef,
     VerifyOTPMessageRequestParametersTypeDef,
     UpdateAdmChannelRequestRequestTypeDef,
+    DeleteAdmChannelResponseTypeDef,
+    GetAdmChannelResponseTypeDef,
+    UpdateAdmChannelResponseTypeDef,
     UpdateApnsChannelRequestRequestTypeDef,
+    DeleteApnsChannelResponseTypeDef,
+    GetApnsChannelResponseTypeDef,
+    UpdateApnsChannelResponseTypeDef,
     UpdateApnsSandboxChannelRequestRequestTypeDef,
+    DeleteApnsSandboxChannelResponseTypeDef,
+    GetApnsSandboxChannelResponseTypeDef,
+    UpdateApnsSandboxChannelResponseTypeDef,
     UpdateApnsVoipChannelRequestRequestTypeDef,
+    DeleteApnsVoipChannelResponseTypeDef,
+    GetApnsVoipChannelResponseTypeDef,
+    UpdateApnsVoipChannelResponseTypeDef,
     UpdateApnsVoipSandboxChannelRequestRequestTypeDef,
+    DeleteApnsVoipSandboxChannelResponseTypeDef,
+    GetApnsVoipSandboxChannelResponseTypeDef,
+    UpdateApnsVoipSandboxChannelResponseTypeDef,
     ActivitiesResponseTypeDef,
     ApplicationsResponseTypeDef,
+    CreateAppResponseTypeDef,
+    DeleteAppResponseTypeDef,
+    GetAppResponseTypeDef,
     ApplicationSettingsResourceTypeDef,
     WriteApplicationSettingsRequestTypeDef,
+    RemoveAttributesResponseTypeDef,
     UpdateBaiduChannelRequestRequestTypeDef,
+    DeleteBaiduChannelResponseTypeDef,
+    GetBaiduChannelResponseTypeDef,
+    UpdateBaiduChannelResponseTypeDef,
     ChannelsResponseTypeDef,
     ClosedDaysTypeDef,
     WaitActivityTypeDef,
     CreateAppRequestRequestTypeDef,
-    CreateAppResponseTypeDef,
-    DeleteAdmChannelResponseTypeDef,
-    DeleteApnsChannelResponseTypeDef,
-    DeleteApnsSandboxChannelResponseTypeDef,
-    DeleteApnsVoipChannelResponseTypeDef,
-    DeleteApnsVoipSandboxChannelResponseTypeDef,
-    DeleteAppResponseTypeDef,
-    DeleteBaiduChannelResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAdmChannelResponseTypeDef,
-    GetApnsChannelResponseTypeDef,
-    GetApnsSandboxChannelResponseTypeDef,
-    GetApnsVoipChannelResponseTypeDef,
-    GetApnsVoipSandboxChannelResponseTypeDef,
-    GetAppResponseTypeDef,
-    GetBaiduChannelResponseTypeDef,
-    RemoveAttributesResponseTypeDef,
-    UpdateAdmChannelResponseTypeDef,
-    UpdateApnsChannelResponseTypeDef,
-    UpdateApnsSandboxChannelResponseTypeDef,
-    UpdateApnsVoipChannelResponseTypeDef,
-    UpdateApnsVoipSandboxChannelResponseTypeDef,
-    UpdateBaiduChannelResponseTypeDef,
     CreateEmailTemplateRequestRequestTypeDef,
     UpdateEmailTemplateRequestRequestTypeDef,
     CreateEmailTemplateResponseTypeDef,
     CreatePushTemplateResponseTypeDef,
     CreateSmsTemplateResponseTypeDef,
     CreateVoiceTemplateResponseTypeDef,
     CreateExportJobRequestRequestTypeDef,
```

### Comparing `mypy-boto3-pinpoint-1.26.138/mypy_boto3_pinpoint.egg-info/SOURCES.txt` & `mypy-boto3-pinpoint-1.26.161/mypy_boto3_pinpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.26.138/setup.py` & `mypy-boto3-pinpoint-1.26.161/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pinpoint",
-    version="1.26.138",
+    version="1.26.161",
     packages=["mypy_boto3_pinpoint"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Pinpoint 1.26.138 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.Pinpoint 1.26.161 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

