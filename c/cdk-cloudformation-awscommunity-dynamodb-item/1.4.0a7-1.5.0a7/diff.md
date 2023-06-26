# Comparing `tmp/cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7.tar.gz` & `tmp/cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/awscommunity-dynamodb-item/dist/python/cdk-cloudformati", last modified: Mon Jun  5 06:13:02 2023, max compression
+gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/awscommunity-dynamodb-item/dist/python/cdk-cloudformati", last modified: Mon Jun 26 06:18:01 2023, max compression
```

## Comparing `cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7.tar` & `cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-05 06:13:02.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-06-05 06:12:55.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/LICENSE
--rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-06-05 06:12:55.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/MANIFEST.in
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2984 2023-06-05 06:13:02.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2023 2023-06-05 06:12:55.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/README.md
--rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-06-05 06:12:55.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/pyproject.toml
--rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-06-05 06:13:02.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/setup.cfg
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1951 2023-06-05 06:12:55.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/setup.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-05 06:13:02.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/src/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-05 06:13:02.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    10738 2023-06-05 06:12:55.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item/__init__.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-05 06:13:02.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item/_jsii/
--rw-r--r--   0 superchain  (1001) superchain  (1001)      468 2023-06-05 06:12:55.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item/_jsii/__init__.py
--rw-r--r--   0 superchain  (1001) superchain  (1001)    18376 2023-06-05 06:12:55.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item/_jsii/awscommunity-dynamodb-item@1.4.0-alpha.7.jsii.tgz
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-06-05 06:12:55.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item/py.typed
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-05 06:13:02.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item.egg-info/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2984 2023-06-05 06:13:01.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item.egg-info/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      712 2023-06-05 06:13:01.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item.egg-info/SOURCES.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-06-05 06:13:01.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item.egg-info/dependency_links.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)      112 2023-06-05 06:13:01.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item.egg-info/requires.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       46 2023-06-05 06:13:01.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item.egg-info/top_level.txt
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-26 06:18:01.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-06-26 06:17:53.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/LICENSE
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-06-26 06:17:53.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/MANIFEST.in
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     3002 2023-06-26 06:18:01.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2035 2023-06-26 06:17:53.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/README.md
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-06-26 06:17:53.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/pyproject.toml
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-06-26 06:18:01.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/setup.cfg
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1957 2023-06-26 06:17:53.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/setup.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-26 06:18:01.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/src/
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-26 06:18:01.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    10762 2023-06-26 06:17:53.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item/__init__.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-26 06:18:01.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item/_jsii/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      468 2023-06-26 06:17:53.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item/_jsii/__init__.py
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    18407 2023-06-26 06:17:53.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item/_jsii/awscommunity-dynamodb-item@1.5.0-alpha.7.jsii.tgz
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-06-26 06:17:53.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item/py.typed
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-26 06:18:01.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item.egg-info/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     3002 2023-06-26 06:18:01.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item.egg-info/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      712 2023-06-26 06:18:01.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item.egg-info/SOURCES.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-06-26 06:18:01.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item.egg-info/dependency_links.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      112 2023-06-26 06:18:01.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item.egg-info/requires.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       46 2023-06-26 06:18:01.000000 cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item.egg-info/top_level.txt
```

### Comparing `cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/LICENSE` & `cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/PKG-INFO` & `cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-awscommunity-dynamodb-item
-Version: 1.4.0a7
+Version: 1.5.0a7
 Summary: This resource will manage the lifecycle of items in a DynamoDB table
-Home-page: https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git
+Home-page: https://github.com/aws-cloudformation/community-registry-extensions.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -19,23 +19,23 @@
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # awscommunity-dynamodb-item
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::DynamoDB::Item` v1.4.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::DynamoDB::Item` v1.5.0.
 
 ## Description
 
 This resource will manage the lifecycle of items in a DynamoDB table
 
 ## References
 
-* [Source](https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git)
+* [Source](https://github.com/aws-cloudformation/community-registry-extensions.git)
 
 ## Usage
 
 In order to use this library, you will need to activate this AWS CloudFormation Registry type in your account. You can do this via the AWS Management Console or using the [AWS CLI](https://aws.amazon.com/cli/) using the following command:
 
 ```sh
 aws cloudformation activate-type \
@@ -55,13 +55,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::DynamoDB::Item`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-dynamodb-item+v1.4.0).
-* Issues related to `AwsCommunity::DynamoDB::Item` should be reported to the [publisher](https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-dynamodb-item+v1.5.0).
+* Issues related to `AwsCommunity::DynamoDB::Item` should be reported to the [publisher](https://github.com/aws-cloudformation/community-registry-extensions.git).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/README.md` & `cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # awscommunity-dynamodb-item
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::DynamoDB::Item` v1.4.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::DynamoDB::Item` v1.5.0.
 
 ## Description
 
 This resource will manage the lifecycle of items in a DynamoDB table
 
 ## References
 
-* [Source](https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git)
+* [Source](https://github.com/aws-cloudformation/community-registry-extensions.git)
 
 ## Usage
 
 In order to use this library, you will need to activate this AWS CloudFormation Registry type in your account. You can do this via the AWS Management Console or using the [AWS CLI](https://aws.amazon.com/cli/) using the following command:
 
 ```sh
 aws cloudformation activate-type \
@@ -32,13 +32,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::DynamoDB::Item`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-dynamodb-item+v1.4.0).
-* Issues related to `AwsCommunity::DynamoDB::Item` should be reported to the [publisher](https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-dynamodb-item+v1.5.0).
+* Issues related to `AwsCommunity::DynamoDB::Item` should be reported to the [publisher](https://github.com/aws-cloudformation/community-registry-extensions.git).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/setup.py` & `cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-cloudformation-awscommunity-dynamodb-item",
-    "version": "1.4.0.a7",
+    "version": "1.5.0.a7",
     "description": "This resource will manage the lifecycle of items in a DynamoDB table",
     "license": "Apache-2.0",
-    "url": "https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git",
+    "url": "https://github.com/aws-cloudformation/community-registry-extensions.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
     },
     "project_urls": {
         "Source": "https://github.com/cdklabs/cdk-cloudformation.git"
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_cloudformation_awscommunity_dynamodb_item",
         "cdk_cloudformation_awscommunity_dynamodb_item._jsii"
     ],
     "package_data": {
         "cdk_cloudformation_awscommunity_dynamodb_item._jsii": [
-            "awscommunity-dynamodb-item@1.4.0-alpha.7.jsii.tgz"
+            "awscommunity-dynamodb-item@1.5.0-alpha.7.jsii.tgz"
         ],
         "cdk_cloudformation_awscommunity_dynamodb_item": [
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

### Comparing `cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item/__init__.py` & `cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 '''
 # awscommunity-dynamodb-item
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::DynamoDB::Item` v1.4.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::DynamoDB::Item` v1.5.0.
 
 ## Description
 
 This resource will manage the lifecycle of items in a DynamoDB table
 
 ## References
 
-* [Source](https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git)
+* [Source](https://github.com/aws-cloudformation/community-registry-extensions.git)
 
 ## Usage
 
 In order to use this library, you will need to activate this AWS CloudFormation Registry type in your account. You can do this via the AWS Management Console or using the [AWS CLI](https://aws.amazon.com/cli/) using the following command:
 
 ```sh
 aws cloudformation activate-type \
@@ -33,16 +33,16 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::DynamoDB::Item`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-dynamodb-item+v1.4.0).
-* Issues related to `AwsCommunity::DynamoDB::Item` should be reported to the [publisher](https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-dynamodb-item+v1.5.0).
+* Issues related to `AwsCommunity::DynamoDB::Item` should be reported to the [publisher](https://github.com/aws-cloudformation/community-registry-extensions.git).
 
 ## License
 
 Distributed under the Apache-2.0 License.
 '''
 import abc
 import builtins
@@ -66,15 +66,15 @@
     _aws_cdk_ceddda9d.CfnResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdk-cloudformation/awscommunity-dynamodb-item.CfnItem",
 ):
     '''A CloudFormation ``AwsCommunity::DynamoDB::Item``.
 
     :cloudformationResource: AwsCommunity::DynamoDB::Item
-    :link: https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git
+    :link: https://github.com/aws-cloudformation/community-registry-extensions.git
     '''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
@@ -105,15 +105,15 @@
         return typing.cast(builtins.str, jsii.sget(cls, "CFN_RESOURCE_TYPE_NAME"))
 
     @builtins.property
     @jsii.member(jsii_name="attrCompositeKey")
     def attr_composite_key(self) -> builtins.str:
         '''Attribute ``AwsCommunity::DynamoDB::Item.CompositeKey``.
 
-        :link: https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git
+        :link: https://github.com/aws-cloudformation/community-registry-extensions.git
         '''
         return typing.cast(builtins.str, jsii.get(self, "attrCompositeKey"))
 
     @builtins.property
     @jsii.member(jsii_name="props")
     def props(self) -> "CfnItemProps":
         '''Resource props.'''
```

### Comparing `cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item.egg-info/PKG-INFO` & `cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-awscommunity-dynamodb-item
-Version: 1.4.0a7
+Version: 1.5.0a7
 Summary: This resource will manage the lifecycle of items in a DynamoDB table
-Home-page: https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git
+Home-page: https://github.com/aws-cloudformation/community-registry-extensions.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -19,23 +19,23 @@
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # awscommunity-dynamodb-item
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::DynamoDB::Item` v1.4.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::DynamoDB::Item` v1.5.0.
 
 ## Description
 
 This resource will manage the lifecycle of items in a DynamoDB table
 
 ## References
 
-* [Source](https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git)
+* [Source](https://github.com/aws-cloudformation/community-registry-extensions.git)
 
 ## Usage
 
 In order to use this library, you will need to activate this AWS CloudFormation Registry type in your account. You can do this via the AWS Management Console or using the [AWS CLI](https://aws.amazon.com/cli/) using the following command:
 
 ```sh
 aws cloudformation activate-type \
@@ -55,13 +55,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::DynamoDB::Item`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-dynamodb-item+v1.4.0).
-* Issues related to `AwsCommunity::DynamoDB::Item` should be reported to the [publisher](https://github.com/aws-cloudformation/aws-cloudformation-rpdk.git).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-dynamodb-item+v1.5.0).
+* Issues related to `AwsCommunity::DynamoDB::Item` should be reported to the [publisher](https://github.com/aws-cloudformation/community-registry-extensions.git).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-awscommunity-dynamodb-item-1.4.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item.egg-info/SOURCES.txt` & `cdk-cloudformation-awscommunity-dynamodb-item-1.5.0a7/src/cdk_cloudformation_awscommunity_dynamodb_item.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_cloudformation_awscommunity_dynamodb_item/py.typed
 src/cdk_cloudformation_awscommunity_dynamodb_item.egg-info/PKG-INFO
 src/cdk_cloudformation_awscommunity_dynamodb_item.egg-info/SOURCES.txt
 src/cdk_cloudformation_awscommunity_dynamodb_item.egg-info/dependency_links.txt
 src/cdk_cloudformation_awscommunity_dynamodb_item.egg-info/requires.txt
 src/cdk_cloudformation_awscommunity_dynamodb_item.egg-info/top_level.txt
 src/cdk_cloudformation_awscommunity_dynamodb_item/_jsii/__init__.py
-src/cdk_cloudformation_awscommunity_dynamodb_item/_jsii/awscommunity-dynamodb-item@1.4.0-alpha.7.jsii.tgz
+src/cdk_cloudformation_awscommunity_dynamodb_item/_jsii/awscommunity-dynamodb-item@1.5.0-alpha.7.jsii.tgz
```

