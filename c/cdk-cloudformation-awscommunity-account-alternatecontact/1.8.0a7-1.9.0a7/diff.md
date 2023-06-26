# Comparing `tmp/cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7.tar.gz` & `tmp/cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/awscommunity-account-alternatecontact/dist/python/cdk-c", last modified: Mon Jun  5 06:13:13 2023, max compression
+gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/awscommunity-account-alternatecontact/dist/python/cdk-c", last modified: Mon Jun 26 06:17:55 2023, max compression
```

## Comparing `cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7.tar` & `cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-05 06:13:13.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-06-05 06:13:06.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/LICENSE
--rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-06-05 06:13:06.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/MANIFEST.in
--rw-r--r--   0 superchain  (1001) superchain  (1001)     3082 2023-06-05 06:13:13.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2108 2023-06-05 06:13:06.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/README.md
--rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-06-05 06:13:06.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/pyproject.toml
--rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-06-05 06:13:13.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/setup.cfg
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2019 2023-06-05 06:13:06.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/setup.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-05 06:13:13.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/src/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-05 06:13:13.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    11596 2023-06-05 06:13:06.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/__init__.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-05 06:13:13.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/_jsii/
--rw-r--r--   0 superchain  (1001) superchain  (1001)      490 2023-06-05 06:13:06.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/_jsii/__init__.py
--rw-r--r--   0 superchain  (1001) superchain  (1001)    18447 2023-06-05 06:13:06.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/_jsii/awscommunity-account-alternatecontact@1.8.0-alpha.7.jsii.tgz
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-06-05 06:13:06.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/py.typed
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-05 06:13:13.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     3082 2023-06-05 06:13:13.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      822 2023-06-05 06:13:13.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/SOURCES.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-06-05 06:13:13.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/dependency_links.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)      112 2023-06-05 06:13:13.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/requires.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       57 2023-06-05 06:13:13.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/top_level.txt
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-26 06:17:55.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-06-26 06:17:49.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/LICENSE
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-06-26 06:17:49.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/MANIFEST.in
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     3082 2023-06-26 06:17:55.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2108 2023-06-26 06:17:49.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/README.md
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-06-26 06:17:49.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/pyproject.toml
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-06-26 06:17:55.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/setup.cfg
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2019 2023-06-26 06:17:49.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/setup.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-26 06:17:55.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/src/
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-26 06:17:55.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    11596 2023-06-26 06:17:49.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/__init__.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-26 06:17:55.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/_jsii/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      490 2023-06-26 06:17:49.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/_jsii/__init__.py
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    18438 2023-06-26 06:17:49.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/_jsii/awscommunity-account-alternatecontact@1.9.0-alpha.7.jsii.tgz
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-06-26 06:17:49.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/py.typed
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-06-26 06:17:55.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     3082 2023-06-26 06:17:55.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      822 2023-06-26 06:17:55.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/SOURCES.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-06-26 06:17:55.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/dependency_links.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      112 2023-06-26 06:17:55.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/requires.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       57 2023-06-26 06:17:55.000000 cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/top_level.txt
```

### Comparing `cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/LICENSE` & `cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/PKG-INFO` & `cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-awscommunity-account-alternatecontact
-Version: 1.8.0a7
+Version: 1.9.0a7
 Summary: An alternate contact attached to an Amazon Web Services account.
 Home-page: https://github.com/aws-cloudformation/community-registry-extensions.git
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
 
 # awscommunity-account-alternatecontact
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Account::AlternateContact` v1.8.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Account::AlternateContact` v1.9.0.
 
 ## Description
 
 An alternate contact attached to an Amazon Web Services account.
 
 ## References
 
@@ -55,13 +55,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::Account::AlternateContact`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-account-alternatecontact+v1.8.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-account-alternatecontact+v1.9.0).
 * Issues related to `AwsCommunity::Account::AlternateContact` should be reported to the [publisher](https://github.com/aws-cloudformation/community-registry-extensions.git).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/README.md` & `cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # awscommunity-account-alternatecontact
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Account::AlternateContact` v1.8.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Account::AlternateContact` v1.9.0.
 
 ## Description
 
 An alternate contact attached to an Amazon Web Services account.
 
 ## References
 
@@ -32,13 +32,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::Account::AlternateContact`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-account-alternatecontact+v1.8.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-account-alternatecontact+v1.9.0).
 * Issues related to `AwsCommunity::Account::AlternateContact` should be reported to the [publisher](https://github.com/aws-cloudformation/community-registry-extensions.git).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/setup.py` & `cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-cloudformation-awscommunity-account-alternatecontact",
-    "version": "1.8.0.a7",
+    "version": "1.9.0.a7",
     "description": "An alternate contact attached to an Amazon Web Services account.",
     "license": "Apache-2.0",
     "url": "https://github.com/aws-cloudformation/community-registry-extensions.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_cloudformation_awscommunity_account_alternatecontact",
         "cdk_cloudformation_awscommunity_account_alternatecontact._jsii"
     ],
     "package_data": {
         "cdk_cloudformation_awscommunity_account_alternatecontact._jsii": [
-            "awscommunity-account-alternatecontact@1.8.0-alpha.7.jsii.tgz"
+            "awscommunity-account-alternatecontact@1.9.0-alpha.7.jsii.tgz"
         ],
         "cdk_cloudformation_awscommunity_account_alternatecontact": [
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

### Comparing `cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/__init__.py` & `cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # awscommunity-account-alternatecontact
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Account::AlternateContact` v1.8.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Account::AlternateContact` v1.9.0.
 
 ## Description
 
 An alternate contact attached to an Amazon Web Services account.
 
 ## References
 
@@ -33,15 +33,15 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::Account::AlternateContact`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-account-alternatecontact+v1.8.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-account-alternatecontact+v1.9.0).
 * Issues related to `AwsCommunity::Account::AlternateContact` should be reported to the [publisher](https://github.com/aws-cloudformation/community-registry-extensions.git).
 
 ## License
 
 Distributed under the Apache-2.0 License.
 '''
 import abc
```

### Comparing `cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/PKG-INFO` & `cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-awscommunity-account-alternatecontact
-Version: 1.8.0a7
+Version: 1.9.0a7
 Summary: An alternate contact attached to an Amazon Web Services account.
 Home-page: https://github.com/aws-cloudformation/community-registry-extensions.git
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
 
 # awscommunity-account-alternatecontact
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Account::AlternateContact` v1.8.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `AwsCommunity::Account::AlternateContact` v1.9.0.
 
 ## Description
 
 An alternate contact attached to an Amazon Web Services account.
 
 ## References
 
@@ -55,13 +55,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `AwsCommunity::Account::AlternateContact`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-account-alternatecontact+v1.8.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fawscommunity-account-alternatecontact+v1.9.0).
 * Issues related to `AwsCommunity::Account::AlternateContact` should be reported to the [publisher](https://github.com/aws-cloudformation/community-registry-extensions.git).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-awscommunity-account-alternatecontact-1.8.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/SOURCES.txt` & `cdk-cloudformation-awscommunity-account-alternatecontact-1.9.0a7/src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_cloudformation_awscommunity_account_alternatecontact/py.typed
 src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/PKG-INFO
 src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/SOURCES.txt
 src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/dependency_links.txt
 src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/requires.txt
 src/cdk_cloudformation_awscommunity_account_alternatecontact.egg-info/top_level.txt
 src/cdk_cloudformation_awscommunity_account_alternatecontact/_jsii/__init__.py
-src/cdk_cloudformation_awscommunity_account_alternatecontact/_jsii/awscommunity-account-alternatecontact@1.8.0-alpha.7.jsii.tgz
+src/cdk_cloudformation_awscommunity_account_alternatecontact/_jsii/awscommunity-account-alternatecontact@1.9.0-alpha.7.jsii.tgz
```

