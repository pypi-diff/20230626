# Comparing `tmp/cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7.tar.gz` & `tmp/cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/awscommunity-applicationautoscaling-scheduledaction/dis", last modified: Mon Jun  5 06:13:08 2023, max compression
+gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/awscommunity-applicationautoscaling-scheduledaction/dis", last modified: Mon Jun 26 06:18:18 2023, max compression
```

## Comparing `cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7.tar` & `cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-05 06:13:08.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-06-05 06:13:02.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/LICENSE
--rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-06-05 06:13:02.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/MANIFEST.in
--rw-r--r--   0 superchain  (1001) superchain  (1001)     3136 2023-06-05 06:13:08.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2175 2023-06-05 06:13:02.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/README.md
--rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-06-05 06:13:02.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/pyproject.toml
--rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-06-05 06:13:08.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/setup.cfg
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2076 2023-06-05 06:13:02.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/setup.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-05 06:13:08.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/src/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-05 06:13:08.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    16645 2023-06-05 06:13:02.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction/__init__.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-05 06:13:08.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction/_jsii/
--rw-r--r--   0 superchain  (1001) superchain  (1001)      518 2023-06-05 06:13:02.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction/_jsii/__init__.py
--rw-r--r--   0 superchain  (1001) superchain  (1001)    18923 2023-06-05 06:13:02.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction/_jsii/awscommunity-applicationautoscaling-scheduledaction@1.3.0-alpha.7.jsii.tgz
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-06-05 06:13:02.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction/py.typed
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-05 06:13:08.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction.egg-info/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     3136 2023-06-05 06:13:08.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction.egg-info/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      962 2023-06-05 06:13:08.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction.egg-info/SOURCES.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-06-05 06:13:08.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction.egg-info/dependency_links.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)      112 2023-06-05 06:13:08.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction.egg-info/requires.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       71 2023-06-05 06:13:08.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction.egg-info/top_level.txt
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-26 06:18:18.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-06-26 06:18:10.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/LICENSE
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-06-26 06:18:10.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/MANIFEST.in
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     3136 2023-06-26 06:18:18.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2175 2023-06-26 06:18:10.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/README.md
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-06-26 06:18:10.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/pyproject.toml
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-06-26 06:18:18.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/setup.cfg
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2076 2023-06-26 06:18:10.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/setup.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-26 06:18:18.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/src/
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-26 06:18:18.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    16645 2023-06-26 06:18:10.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction/__init__.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-26 06:18:18.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction/_jsii/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      518 2023-06-26 06:18:10.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction/_jsii/__init__.py
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    18958 2023-06-26 06:18:10.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction/_jsii/awscommunity-applicationautoscaling-scheduledaction@1.4.0-alpha.7.jsii.tgz
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-06-26 06:18:10.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction/py.typed
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-26 06:18:18.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction.egg-info/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     3136 2023-06-26 06:18:18.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction.egg-info/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      962 2023-06-26 06:18:18.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction.egg-info/SOURCES.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-06-26 06:18:18.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction.egg-info/dependency_links.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      112 2023-06-26 06:18:18.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction.egg-info/requires.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       71 2023-06-26 06:18:18.000000 cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction.egg-info/top_level.txt
```

### Comparing `cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/LICENSE` & `cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/PKG-INFO` & `cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction
-Version: 1.3.0a7
+Version: 1.4.0a7
 Summary: Application Autoscaling Scheduled Action.
 Home-page: https://github.com/aws-cloudformation/community-registry-extensions
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # awscommunity-applicationautoscaling-scheduledaction
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::ApplicationAutoscaling::ScheduledAction` v1.3.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::ApplicationAutoscaling::ScheduledAction` v1.4.0.
 
 ## Description
 
 Application Autoscaling Scheduled Action.
 
 ## References
 
@@ -55,13 +55,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::ApplicationAutoscaling::ScheduledAction`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-applicationautoscaling-scheduledaction+v1.3.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-applicationautoscaling-scheduledaction+v1.4.0).
 * Issues related to `AwsCommunity::ApplicationAutoscaling::ScheduledAction` should be reported to the [publisher](https://github.com/aws-cloudformation/community-registry-extensions).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/README.md` & `cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # awscommunity-applicationautoscaling-scheduledaction
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::ApplicationAutoscaling::ScheduledAction` v1.3.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::ApplicationAutoscaling::ScheduledAction` v1.4.0.
 
 ## Description
 
 Application Autoscaling Scheduled Action.
 
 ## References
 
@@ -32,13 +32,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::ApplicationAutoscaling::ScheduledAction`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-applicationautoscaling-scheduledaction+v1.3.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-applicationautoscaling-scheduledaction+v1.4.0).
 * Issues related to `AwsCommunity::ApplicationAutoscaling::ScheduledAction` should be reported to the [publisher](https://github.com/aws-cloudformation/community-registry-extensions).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/setup.py` & `cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction",
-    "version": "1.3.0.a7",
+    "version": "1.4.0.a7",
     "description": "Application Autoscaling Scheduled Action.",
     "license": "Apache-2.0",
     "url": "https://github.com/aws-cloudformation/community-registry-extensions",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction",
         "cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction._jsii"
     ],
     "package_data": {
         "cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction._jsii": [
-            "awscommunity-applicationautoscaling-scheduledaction@1.3.0-alpha.7.jsii.tgz"
+            "awscommunity-applicationautoscaling-scheduledaction@1.4.0-alpha.7.jsii.tgz"
         ],
         "cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.82.0, <3.0.0",
-        "constructs>=10.2.43, <11.0.0",
-        "jsii>=1.82.0, <2.0.0",
+        "aws-cdk-lib>=2.85.0, <3.0.0",
+        "constructs>=10.2.60, <11.0.0",
+        "jsii>=1.84.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction/__init__.py` & `cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # awscommunity-applicationautoscaling-scheduledaction
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::ApplicationAutoscaling::ScheduledAction` v1.3.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::ApplicationAutoscaling::ScheduledAction` v1.4.0.
 
 ## Description
 
 Application Autoscaling Scheduled Action.
 
 ## References
 
@@ -33,15 +33,15 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::ApplicationAutoscaling::ScheduledAction`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-applicationautoscaling-scheduledaction+v1.3.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-applicationautoscaling-scheduledaction+v1.4.0).
 * Issues related to `AwsCommunity::ApplicationAutoscaling::ScheduledAction` should be reported to the [publisher](https://github.com/aws-cloudformation/community-registry-extensions).
 
 ## License
 
 Distributed under the Apache-2.0 License.
 '''
 import abc
```

### Comparing `cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction/_jsii/__init__.py` & `cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction/_jsii/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 from typeguard import check_type
 
 import aws_cdk._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@cdk-cloudformation/awscommunity-applicationautoscaling-scheduledaction",
-    "1.3.0-alpha.7",
+    "1.4.0-alpha.7",
     __name__[0:-6],
-    "awscommunity-applicationautoscaling-scheduledaction@1.3.0-alpha.7.jsii.tgz",
+    "awscommunity-applicationautoscaling-scheduledaction@1.4.0-alpha.7.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction.egg-info/PKG-INFO` & `cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction
-Version: 1.3.0a7
+Version: 1.4.0a7
 Summary: Application Autoscaling Scheduled Action.
 Home-page: https://github.com/aws-cloudformation/community-registry-extensions
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # awscommunity-applicationautoscaling-scheduledaction
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::ApplicationAutoscaling::ScheduledAction` v1.3.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::ApplicationAutoscaling::ScheduledAction` v1.4.0.
 
 ## Description
 
 Application Autoscaling Scheduled Action.
 
 ## References
 
@@ -55,13 +55,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::ApplicationAutoscaling::ScheduledAction`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-applicationautoscaling-scheduledaction+v1.3.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-applicationautoscaling-scheduledaction+v1.4.0).
 * Issues related to `AwsCommunity::ApplicationAutoscaling::ScheduledAction` should be reported to the [publisher](https://github.com/aws-cloudformation/community-registry-extensions).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.3.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction.egg-info/SOURCES.txt` & `cdk-cloudformation-awscommunity-applicationautoscaling-scheduledaction-1.4.0a7/src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction/py.typed
 src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction.egg-info/PKG-INFO
 src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction.egg-info/SOURCES.txt
 src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction.egg-info/dependency_links.txt
 src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction.egg-info/requires.txt
 src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction.egg-info/top_level.txt
 src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction/_jsii/__init__.py
-src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction/_jsii/awscommunity-applicationautoscaling-scheduledaction@1.3.0-alpha.7.jsii.tgz
+src/cdk_cloudformation_awscommunity_applicationautoscaling_scheduledaction/_jsii/awscommunity-applicationautoscaling-scheduledaction@1.4.0-alpha.7.jsii.tgz
```

