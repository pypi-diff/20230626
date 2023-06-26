# Comparing `tmp/neulabs-cdk-constructs-0.4.8.tar.gz` & `tmp/neulabs-cdk-constructs-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neulabs-cdk-constructs-0.4.8.tar", last modified: Tue Jun 20 08:17:56 2023, max compression
+gzip compressed data, was "neulabs-cdk-constructs-0.5.0.tar", last modified: Mon Jun 26 15:52:51 2023, max compression
```

## Comparing `neulabs-cdk-constructs-0.4.8.tar` & `neulabs-cdk-constructs-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:17:56.850561 neulabs-cdk-constructs-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-20 08:17:42.000000 neulabs-cdk-constructs-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 08:17:42.000000 neulabs-cdk-constructs-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-20 08:17:56.850561 neulabs-cdk-constructs-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-20 08:17:42.000000 neulabs-cdk-constructs-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-20 08:17:42.000000 neulabs-cdk-constructs-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 08:17:56.850561 neulabs-cdk-constructs-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-20 08:17:42.000000 neulabs-cdk-constructs-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:17:56.846561 neulabs-cdk-constructs-0.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:17:56.850561 neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-20 08:17:42.000000 neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:17:56.850561 neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-20 08:17:42.000000 neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   115237 2023-06-20 08:17:42.000000 neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.4.8.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:17:56.850561 neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/aws_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)   299578 2023-06-20 08:17:42.000000 neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/aws_lambda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:17:56.850561 neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/newrelic/
--rw-r--r--   0 runner    (1001) docker     (123)    40572 2023-06-20 08:17:42.000000 neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/newrelic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:17:56.850561 neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/oidc/
--rw-r--r--   0 runner    (1001) docker     (123)    45448 2023-06-20 08:17:42.000000 neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 08:17:42.000000 neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:17:56.850561 neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/stack/
--rw-r--r--   0 runner    (1001) docker     (123)    24368 2023-06-20 08:17:42.000000 neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:17:56.850561 neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-20 08:17:42.000000 neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:17:56.850561 neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-20 08:17:56.000000 neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-20 08:17:56.000000 neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 08:17:56.000000 neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-20 08:17:56.000000 neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 08:17:56.000000 neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:52:51.526049 neulabs-cdk-constructs-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-26 15:52:36.000000 neulabs-cdk-constructs-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 15:52:36.000000 neulabs-cdk-constructs-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-26 15:52:51.526049 neulabs-cdk-constructs-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-26 15:52:36.000000 neulabs-cdk-constructs-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 15:52:36.000000 neulabs-cdk-constructs-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 15:52:51.526049 neulabs-cdk-constructs-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-26 15:52:36.000000 neulabs-cdk-constructs-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:52:51.522049 neulabs-cdk-constructs-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:52:51.522049 neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-26 15:52:36.000000 neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:52:51.526049 neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-26 15:52:36.000000 neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116946 2023-06-26 15:52:36.000000 neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.5.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:52:51.526049 neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/aws_lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)   306174 2023-06-26 15:52:36.000000 neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/aws_lambda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:52:51.526049 neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/newrelic/
+-rw-r--r--   0 runner    (1001) docker     (123)    42813 2023-06-26 15:52:36.000000 neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/newrelic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:52:51.526049 neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)    47689 2023-06-26 15:52:36.000000 neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:52:36.000000 neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:52:51.526049 neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/stack/
+-rw-r--r--   0 runner    (1001) docker     (123)    26609 2023-06-26 15:52:36.000000 neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:52:51.526049 neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-26 15:52:36.000000 neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:52:51.526049 neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-26 15:52:51.000000 neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-26 15:52:51.000000 neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:52:51.000000 neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-26 15:52:51.000000 neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 15:52:51.000000 neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs.egg-info/top_level.txt
```

### Comparing `neulabs-cdk-constructs-0.4.8/LICENSE` & `neulabs-cdk-constructs-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.8/PKG-INFO` & `neulabs-cdk-constructs-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neulabs-cdk-constructs
-Version: 0.4.8
+Version: 0.5.0
 Summary: neulabs-cdk-constructs
 Home-page: https://github.com/neulabscom/neulabs-cdk-constructs.git
 Author: Neulabs<tech@neulabs.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neulabscom/neulabs-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `neulabs-cdk-constructs-0.4.8/README.md` & `neulabs-cdk-constructs-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.8/setup.py` & `neulabs-cdk-constructs-0.5.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "neulabs-cdk-constructs",
-    "version": "0.4.8",
+    "version": "0.5.0",
     "description": "neulabs-cdk-constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/neulabscom/neulabs-cdk-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Neulabs<tech@neulabs.com>",
     "bdist_wheel": {
         "universal": true
@@ -27,25 +27,25 @@
         "neulabs_cdk_constructs.newrelic",
         "neulabs_cdk_constructs.oidc",
         "neulabs_cdk_constructs.stack",
         "neulabs_cdk_constructs.utils"
     ],
     "package_data": {
         "neulabs_cdk_constructs._jsii": [
-            "neulabs-cdk-constructs@0.4.8.jsii.tgz"
+            "neulabs-cdk-constructs@0.5.0.jsii.tgz"
         ],
         "neulabs_cdk_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib==2.82.0",
-        "aws-cdk.aws-apigatewayv2-alpha==2.82.0.a0",
-        "aws-cdk.aws-apigatewayv2-integrations-alpha==2.82.0.a0",
+        "aws-cdk-lib==2.85.0",
+        "aws-cdk.aws-apigatewayv2-alpha==2.85.0.a0",
+        "aws-cdk.aws-apigatewayv2-integrations-alpha==2.85.0.a0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.84.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/__init__.py` & `neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/_jsii/__init__.py` & `neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/_jsii/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 import aws_cdk._jsii
 import aws_cdk.aws_apigatewayv2_alpha._jsii
 import aws_cdk.aws_apigatewayv2_integrations_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "neulabs-cdk-constructs",
-    "0.4.8",
+    "0.5.0",
     __name__[0:-6],
-    "neulabs-cdk-constructs@0.4.8.jsii.tgz",
+    "neulabs-cdk-constructs@0.5.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/aws_lambda/__init__.py` & `neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/aws_lambda/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
         layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
         log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
         log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         memory_size: typing.Optional[jsii.Number] = None,
+        params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
         profiling: typing.Optional[builtins.bool] = None,
         profiling_group: typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup] = None,
         reserved_concurrent_executions: typing.Optional[jsii.Number] = None,
         role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         runtime_management_mode: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode] = None,
         security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
         timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
@@ -107,14 +108,15 @@
         :param initial_policy: Initial policy statements to add to the created Lambda Role. You can call ``addToRolePolicy`` to the created lambda to add statements post creation. Default: - No policy statements are added to the created Lambda role.
         :param insights_version: Specify the version of CloudWatch Lambda insights to use for monitoring. Default: - No Lambda Insights
         :param layers: A list of layers to add to the function's execution environment. You can configure your Lambda function to pull in additional code during initialization in the form of layers. Layers are packages of libraries or other dependencies that can be used by multiple functions. Default: - No layers.
         :param log_retention: The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.INFINITE
         :param log_retention_retry_options: When log retention is specified, a custom resource attempts to create the CloudWatch log group. These options control the retry policy when interacting with CloudWatch APIs. Default: - Default AWS SDK retry options.
         :param log_retention_role: The IAM role for the Lambda function associated with the custom resource that sets the retention policy. Default: - A new role is created.
         :param memory_size: The amount of memory, in MB, that is allocated to your Lambda function. Lambda uses this value to proportionally allocate the amount of CPU power. For more information, see Resource Model in the AWS Lambda Developer Guide. Default: 128
+        :param params_and_secrets: Specify the configuration of Parameters and Secrets Extension. Default: - No Parameters and Secrets Extension
         :param profiling: Enable profiling. Default: - No profiling.
         :param profiling_group: Profiling Group. Default: - A new profiling group will be created if ``profiling`` is set.
         :param reserved_concurrent_executions: The maximum of concurrent executions you want to reserve for the function. Default: - No specific limit - account limit.
         :param role: Lambda execution role. This is the role that will be assumed by the function upon execution. It controls the permissions that the function will have. The Role must be assumable by the 'lambda.amazonaws.com' service principal. The default Role automatically has permissions granted for Lambda execution. If you provide a Role, you must add the relevant AWS managed policies yourself. The relevant managed policies are "service-role/AWSLambdaBasicExecutionRole" and "service-role/AWSLambdaVPCAccessExecutionRole". Default: - A unique role will be generated for this lambda function. Both supplied and generated roles can always be changed by calling ``addToRolePolicy``.
         :param runtime_management_mode: Sets the runtime management configuration for a function's version. Default: Auto
         :param security_groups: The list of security groups to associate with the Lambda's network interfaces. Only used if 'vpc' is supplied. Default: - If the function is placed within a VPC and a security group is not specified, either by this or securityGroup prop, a dedicated security group will be created for this function.
         :param timeout: The function execution time (in seconds) after which Lambda terminates the function. Because the execution time affects cost, set this value based on the function's expected execution time. Default: Duration.seconds(3)
@@ -156,14 +158,15 @@
             initial_policy=initial_policy,
             insights_version=insights_version,
             layers=layers,
             log_retention=log_retention,
             log_retention_retry_options=log_retention_retry_options,
             log_retention_role=log_retention_role,
             memory_size=memory_size,
+            params_and_secrets=params_and_secrets,
             profiling=profiling,
             profiling_group=profiling_group,
             reserved_concurrent_executions=reserved_concurrent_executions,
             role=role,
             runtime_management_mode=runtime_management_mode,
             security_groups=security_groups,
             timeout=timeout,
@@ -231,14 +234,15 @@
         initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
         layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
         log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
         log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         memory_size: typing.Optional[jsii.Number] = None,
+        params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
         profiling: typing.Optional[builtins.bool] = None,
         profiling_group: typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup] = None,
         reserved_concurrent_executions: typing.Optional[jsii.Number] = None,
         role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         runtime_management_mode: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode] = None,
         security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
         timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
@@ -282,14 +286,15 @@
         :param initial_policy: Initial policy statements to add to the created Lambda Role. You can call ``addToRolePolicy`` to the created lambda to add statements post creation. Default: - No policy statements are added to the created Lambda role.
         :param insights_version: Specify the version of CloudWatch Lambda insights to use for monitoring. Default: - No Lambda Insights
         :param layers: A list of layers to add to the function's execution environment. You can configure your Lambda function to pull in additional code during initialization in the form of layers. Layers are packages of libraries or other dependencies that can be used by multiple functions. Default: - No layers.
         :param log_retention: The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.INFINITE
         :param log_retention_retry_options: When log retention is specified, a custom resource attempts to create the CloudWatch log group. These options control the retry policy when interacting with CloudWatch APIs. Default: - Default AWS SDK retry options.
         :param log_retention_role: The IAM role for the Lambda function associated with the custom resource that sets the retention policy. Default: - A new role is created.
         :param memory_size: The amount of memory, in MB, that is allocated to your Lambda function. Lambda uses this value to proportionally allocate the amount of CPU power. For more information, see Resource Model in the AWS Lambda Developer Guide. Default: 128
+        :param params_and_secrets: Specify the configuration of Parameters and Secrets Extension. Default: - No Parameters and Secrets Extension
         :param profiling: Enable profiling. Default: - No profiling.
         :param profiling_group: Profiling Group. Default: - A new profiling group will be created if ``profiling`` is set.
         :param reserved_concurrent_executions: The maximum of concurrent executions you want to reserve for the function. Default: - No specific limit - account limit.
         :param role: Lambda execution role. This is the role that will be assumed by the function upon execution. It controls the permissions that the function will have. The Role must be assumable by the 'lambda.amazonaws.com' service principal. The default Role automatically has permissions granted for Lambda execution. If you provide a Role, you must add the relevant AWS managed policies yourself. The relevant managed policies are "service-role/AWSLambdaBasicExecutionRole" and "service-role/AWSLambdaVPCAccessExecutionRole". Default: - A unique role will be generated for this lambda function. Both supplied and generated roles can always be changed by calling ``addToRolePolicy``.
         :param runtime_management_mode: Sets the runtime management configuration for a function's version. Default: Auto
         :param security_groups: The list of security groups to associate with the Lambda's network interfaces. Only used if 'vpc' is supplied. Default: - If the function is placed within a VPC and a security group is not specified, either by this or securityGroup prop, a dedicated security group will be created for this function.
         :param timeout: The function execution time (in seconds) after which Lambda terminates the function. Because the execution time affects cost, set this value based on the function's expected execution time. Default: Duration.seconds(3)
@@ -335,14 +340,15 @@
             initial_policy=initial_policy,
             insights_version=insights_version,
             layers=layers,
             log_retention=log_retention,
             log_retention_retry_options=log_retention_retry_options,
             log_retention_role=log_retention_role,
             memory_size=memory_size,
+            params_and_secrets=params_and_secrets,
             profiling=profiling,
             profiling_group=profiling_group,
             reserved_concurrent_executions=reserved_concurrent_executions,
             role=role,
             runtime_management_mode=runtime_management_mode,
             security_groups=security_groups,
             timeout=timeout,
@@ -398,14 +404,15 @@
         "initial_policy": "initialPolicy",
         "insights_version": "insightsVersion",
         "layers": "layers",
         "log_retention": "logRetention",
         "log_retention_retry_options": "logRetentionRetryOptions",
         "log_retention_role": "logRetentionRole",
         "memory_size": "memorySize",
+        "params_and_secrets": "paramsAndSecrets",
         "profiling": "profiling",
         "profiling_group": "profilingGroup",
         "reserved_concurrent_executions": "reservedConcurrentExecutions",
         "role": "role",
         "runtime_management_mode": "runtimeManagementMode",
         "security_groups": "securityGroups",
         "timeout": "timeout",
@@ -451,14 +458,15 @@
         initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
         layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
         log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
         log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         memory_size: typing.Optional[jsii.Number] = None,
+        params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
         profiling: typing.Optional[builtins.bool] = None,
         profiling_group: typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup] = None,
         reserved_concurrent_executions: typing.Optional[jsii.Number] = None,
         role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         runtime_management_mode: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode] = None,
         security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
         timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
@@ -500,14 +508,15 @@
         :param initial_policy: Initial policy statements to add to the created Lambda Role. You can call ``addToRolePolicy`` to the created lambda to add statements post creation. Default: - No policy statements are added to the created Lambda role.
         :param insights_version: Specify the version of CloudWatch Lambda insights to use for monitoring. Default: - No Lambda Insights
         :param layers: A list of layers to add to the function's execution environment. You can configure your Lambda function to pull in additional code during initialization in the form of layers. Layers are packages of libraries or other dependencies that can be used by multiple functions. Default: - No layers.
         :param log_retention: The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.INFINITE
         :param log_retention_retry_options: When log retention is specified, a custom resource attempts to create the CloudWatch log group. These options control the retry policy when interacting with CloudWatch APIs. Default: - Default AWS SDK retry options.
         :param log_retention_role: The IAM role for the Lambda function associated with the custom resource that sets the retention policy. Default: - A new role is created.
         :param memory_size: The amount of memory, in MB, that is allocated to your Lambda function. Lambda uses this value to proportionally allocate the amount of CPU power. For more information, see Resource Model in the AWS Lambda Developer Guide. Default: 128
+        :param params_and_secrets: Specify the configuration of Parameters and Secrets Extension. Default: - No Parameters and Secrets Extension
         :param profiling: Enable profiling. Default: - No profiling.
         :param profiling_group: Profiling Group. Default: - A new profiling group will be created if ``profiling`` is set.
         :param reserved_concurrent_executions: The maximum of concurrent executions you want to reserve for the function. Default: - No specific limit - account limit.
         :param role: Lambda execution role. This is the role that will be assumed by the function upon execution. It controls the permissions that the function will have. The Role must be assumable by the 'lambda.amazonaws.com' service principal. The default Role automatically has permissions granted for Lambda execution. If you provide a Role, you must add the relevant AWS managed policies yourself. The relevant managed policies are "service-role/AWSLambdaBasicExecutionRole" and "service-role/AWSLambdaVPCAccessExecutionRole". Default: - A unique role will be generated for this lambda function. Both supplied and generated roles can always be changed by calling ``addToRolePolicy``.
         :param runtime_management_mode: Sets the runtime management configuration for a function's version. Default: Auto
         :param security_groups: The list of security groups to associate with the Lambda's network interfaces. Only used if 'vpc' is supplied. Default: - If the function is placed within a VPC and a security group is not specified, either by this or securityGroup prop, a dedicated security group will be created for this function.
         :param timeout: The function execution time (in seconds) after which Lambda terminates the function. Because the execution time affects cost, set this value based on the function's expected execution time. Default: Duration.seconds(3)
@@ -560,14 +569,15 @@
             check_type(argname="argument initial_policy", value=initial_policy, expected_type=type_hints["initial_policy"])
             check_type(argname="argument insights_version", value=insights_version, expected_type=type_hints["insights_version"])
             check_type(argname="argument layers", value=layers, expected_type=type_hints["layers"])
             check_type(argname="argument log_retention", value=log_retention, expected_type=type_hints["log_retention"])
             check_type(argname="argument log_retention_retry_options", value=log_retention_retry_options, expected_type=type_hints["log_retention_retry_options"])
             check_type(argname="argument log_retention_role", value=log_retention_role, expected_type=type_hints["log_retention_role"])
             check_type(argname="argument memory_size", value=memory_size, expected_type=type_hints["memory_size"])
+            check_type(argname="argument params_and_secrets", value=params_and_secrets, expected_type=type_hints["params_and_secrets"])
             check_type(argname="argument profiling", value=profiling, expected_type=type_hints["profiling"])
             check_type(argname="argument profiling_group", value=profiling_group, expected_type=type_hints["profiling_group"])
             check_type(argname="argument reserved_concurrent_executions", value=reserved_concurrent_executions, expected_type=type_hints["reserved_concurrent_executions"])
             check_type(argname="argument role", value=role, expected_type=type_hints["role"])
             check_type(argname="argument runtime_management_mode", value=runtime_management_mode, expected_type=type_hints["runtime_management_mode"])
             check_type(argname="argument security_groups", value=security_groups, expected_type=type_hints["security_groups"])
             check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
@@ -637,14 +647,16 @@
             self._values["log_retention"] = log_retention
         if log_retention_retry_options is not None:
             self._values["log_retention_retry_options"] = log_retention_retry_options
         if log_retention_role is not None:
             self._values["log_retention_role"] = log_retention_role
         if memory_size is not None:
             self._values["memory_size"] = memory_size
+        if params_and_secrets is not None:
+            self._values["params_and_secrets"] = params_and_secrets
         if profiling is not None:
             self._values["profiling"] = profiling
         if profiling_group is not None:
             self._values["profiling_group"] = profiling_group
         if reserved_concurrent_executions is not None:
             self._values["reserved_concurrent_executions"] = reserved_concurrent_executions
         if role is not None:
@@ -992,14 +1004,27 @@
 
         :default: 128
         '''
         result = self._values.get("memory_size")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
+    def params_and_secrets(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion]:
+        '''Specify the configuration of Parameters and Secrets Extension.
+
+        :default: - No Parameters and Secrets Extension
+
+        :see: https://docs.aws.amazon.com/systems-manager/latest/userguide/ps-integration-lambda-extensions.html
+        '''
+        result = self._values.get("params_and_secrets")
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion], result)
+
+    @builtins.property
     def profiling(self) -> typing.Optional[builtins.bool]:
         '''Enable profiling.
 
         :default: - No profiling.
 
         :see: https://docs.aws.amazon.com/codeguru/latest/profiler-ug/setting-up-lambda.html
         '''
@@ -1276,14 +1301,15 @@
         "initial_policy": "initialPolicy",
         "insights_version": "insightsVersion",
         "layers": "layers",
         "log_retention": "logRetention",
         "log_retention_retry_options": "logRetentionRetryOptions",
         "log_retention_role": "logRetentionRole",
         "memory_size": "memorySize",
+        "params_and_secrets": "paramsAndSecrets",
         "profiling": "profiling",
         "profiling_group": "profilingGroup",
         "reserved_concurrent_executions": "reservedConcurrentExecutions",
         "role": "role",
         "runtime_management_mode": "runtimeManagementMode",
         "security_groups": "securityGroups",
         "timeout": "timeout",
@@ -1325,14 +1351,15 @@
         initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
         layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
         log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
         log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         memory_size: typing.Optional[jsii.Number] = None,
+        params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
         profiling: typing.Optional[builtins.bool] = None,
         profiling_group: typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup] = None,
         reserved_concurrent_executions: typing.Optional[jsii.Number] = None,
         role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         runtime_management_mode: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode] = None,
         security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
         timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
@@ -1370,14 +1397,15 @@
         :param initial_policy: Initial policy statements to add to the created Lambda Role. You can call ``addToRolePolicy`` to the created lambda to add statements post creation. Default: - No policy statements are added to the created Lambda role.
         :param insights_version: Specify the version of CloudWatch Lambda insights to use for monitoring. Default: - No Lambda Insights
         :param layers: A list of layers to add to the function's execution environment. You can configure your Lambda function to pull in additional code during initialization in the form of layers. Layers are packages of libraries or other dependencies that can be used by multiple functions. Default: - No layers.
         :param log_retention: The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.INFINITE
         :param log_retention_retry_options: When log retention is specified, a custom resource attempts to create the CloudWatch log group. These options control the retry policy when interacting with CloudWatch APIs. Default: - Default AWS SDK retry options.
         :param log_retention_role: The IAM role for the Lambda function associated with the custom resource that sets the retention policy. Default: - A new role is created.
         :param memory_size: The amount of memory, in MB, that is allocated to your Lambda function. Lambda uses this value to proportionally allocate the amount of CPU power. For more information, see Resource Model in the AWS Lambda Developer Guide. Default: 128
+        :param params_and_secrets: Specify the configuration of Parameters and Secrets Extension. Default: - No Parameters and Secrets Extension
         :param profiling: Enable profiling. Default: - No profiling.
         :param profiling_group: Profiling Group. Default: - A new profiling group will be created if ``profiling`` is set.
         :param reserved_concurrent_executions: The maximum of concurrent executions you want to reserve for the function. Default: - No specific limit - account limit.
         :param role: Lambda execution role. This is the role that will be assumed by the function upon execution. It controls the permissions that the function will have. The Role must be assumable by the 'lambda.amazonaws.com' service principal. The default Role automatically has permissions granted for Lambda execution. If you provide a Role, you must add the relevant AWS managed policies yourself. The relevant managed policies are "service-role/AWSLambdaBasicExecutionRole" and "service-role/AWSLambdaVPCAccessExecutionRole". Default: - A unique role will be generated for this lambda function. Both supplied and generated roles can always be changed by calling ``addToRolePolicy``.
         :param runtime_management_mode: Sets the runtime management configuration for a function's version. Default: Auto
         :param security_groups: The list of security groups to associate with the Lambda's network interfaces. Only used if 'vpc' is supplied. Default: - If the function is placed within a VPC and a security group is not specified, either by this or securityGroup prop, a dedicated security group will be created for this function.
         :param timeout: The function execution time (in seconds) after which Lambda terminates the function. Because the execution time affects cost, set this value based on the function's expected execution time. Default: Duration.seconds(3)
@@ -1424,14 +1452,15 @@
             check_type(argname="argument initial_policy", value=initial_policy, expected_type=type_hints["initial_policy"])
             check_type(argname="argument insights_version", value=insights_version, expected_type=type_hints["insights_version"])
             check_type(argname="argument layers", value=layers, expected_type=type_hints["layers"])
             check_type(argname="argument log_retention", value=log_retention, expected_type=type_hints["log_retention"])
             check_type(argname="argument log_retention_retry_options", value=log_retention_retry_options, expected_type=type_hints["log_retention_retry_options"])
             check_type(argname="argument log_retention_role", value=log_retention_role, expected_type=type_hints["log_retention_role"])
             check_type(argname="argument memory_size", value=memory_size, expected_type=type_hints["memory_size"])
+            check_type(argname="argument params_and_secrets", value=params_and_secrets, expected_type=type_hints["params_and_secrets"])
             check_type(argname="argument profiling", value=profiling, expected_type=type_hints["profiling"])
             check_type(argname="argument profiling_group", value=profiling_group, expected_type=type_hints["profiling_group"])
             check_type(argname="argument reserved_concurrent_executions", value=reserved_concurrent_executions, expected_type=type_hints["reserved_concurrent_executions"])
             check_type(argname="argument role", value=role, expected_type=type_hints["role"])
             check_type(argname="argument runtime_management_mode", value=runtime_management_mode, expected_type=type_hints["runtime_management_mode"])
             check_type(argname="argument security_groups", value=security_groups, expected_type=type_hints["security_groups"])
             check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
@@ -1500,14 +1529,16 @@
             self._values["log_retention"] = log_retention
         if log_retention_retry_options is not None:
             self._values["log_retention_retry_options"] = log_retention_retry_options
         if log_retention_role is not None:
             self._values["log_retention_role"] = log_retention_role
         if memory_size is not None:
             self._values["memory_size"] = memory_size
+        if params_and_secrets is not None:
+            self._values["params_and_secrets"] = params_and_secrets
         if profiling is not None:
             self._values["profiling"] = profiling
         if profiling_group is not None:
             self._values["profiling_group"] = profiling_group
         if reserved_concurrent_executions is not None:
             self._values["reserved_concurrent_executions"] = reserved_concurrent_executions
         if role is not None:
@@ -1841,14 +1872,27 @@
 
         :default: 128
         '''
         result = self._values.get("memory_size")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
+    def params_and_secrets(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion]:
+        '''Specify the configuration of Parameters and Secrets Extension.
+
+        :default: - No Parameters and Secrets Extension
+
+        :see: https://docs.aws.amazon.com/systems-manager/latest/userguide/ps-integration-lambda-extensions.html
+        '''
+        result = self._values.get("params_and_secrets")
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion], result)
+
+    @builtins.property
     def profiling(self) -> typing.Optional[builtins.bool]:
         '''Enable profiling.
 
         :default: - No profiling.
 
         :see: https://docs.aws.amazon.com/codeguru/latest/profiler-ug/setting-up-lambda.html
         '''
@@ -2087,14 +2131,15 @@
         initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
         layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
         log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
         log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         memory_size: typing.Optional[jsii.Number] = None,
+        params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
         profiling: typing.Optional[builtins.bool] = None,
         profiling_group: typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup] = None,
         reserved_concurrent_executions: typing.Optional[jsii.Number] = None,
         role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         runtime_management_mode: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode] = None,
         security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
         timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
@@ -2138,14 +2183,15 @@
         :param initial_policy: Initial policy statements to add to the created Lambda Role. You can call ``addToRolePolicy`` to the created lambda to add statements post creation. Default: - No policy statements are added to the created Lambda role.
         :param insights_version: Specify the version of CloudWatch Lambda insights to use for monitoring. Default: - No Lambda Insights
         :param layers: A list of layers to add to the function's execution environment. You can configure your Lambda function to pull in additional code during initialization in the form of layers. Layers are packages of libraries or other dependencies that can be used by multiple functions. Default: - No layers.
         :param log_retention: The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.INFINITE
         :param log_retention_retry_options: When log retention is specified, a custom resource attempts to create the CloudWatch log group. These options control the retry policy when interacting with CloudWatch APIs. Default: - Default AWS SDK retry options.
         :param log_retention_role: The IAM role for the Lambda function associated with the custom resource that sets the retention policy. Default: - A new role is created.
         :param memory_size: The amount of memory, in MB, that is allocated to your Lambda function. Lambda uses this value to proportionally allocate the amount of CPU power. For more information, see Resource Model in the AWS Lambda Developer Guide. Default: 128
+        :param params_and_secrets: Specify the configuration of Parameters and Secrets Extension. Default: - No Parameters and Secrets Extension
         :param profiling: Enable profiling. Default: - No profiling.
         :param profiling_group: Profiling Group. Default: - A new profiling group will be created if ``profiling`` is set.
         :param reserved_concurrent_executions: The maximum of concurrent executions you want to reserve for the function. Default: - No specific limit - account limit.
         :param role: Lambda execution role. This is the role that will be assumed by the function upon execution. It controls the permissions that the function will have. The Role must be assumable by the 'lambda.amazonaws.com' service principal. The default Role automatically has permissions granted for Lambda execution. If you provide a Role, you must add the relevant AWS managed policies yourself. The relevant managed policies are "service-role/AWSLambdaBasicExecutionRole" and "service-role/AWSLambdaVPCAccessExecutionRole". Default: - A unique role will be generated for this lambda function. Both supplied and generated roles can always be changed by calling ``addToRolePolicy``.
         :param runtime_management_mode: Sets the runtime management configuration for a function's version. Default: Auto
         :param security_groups: The list of security groups to associate with the Lambda's network interfaces. Only used if 'vpc' is supplied. Default: - If the function is placed within a VPC and a security group is not specified, either by this or securityGroup prop, a dedicated security group will be created for this function.
         :param timeout: The function execution time (in seconds) after which Lambda terminates the function. Because the execution time affects cost, set this value based on the function's expected execution time. Default: Duration.seconds(3)
@@ -2191,14 +2237,15 @@
             initial_policy=initial_policy,
             insights_version=insights_version,
             layers=layers,
             log_retention=log_retention,
             log_retention_retry_options=log_retention_retry_options,
             log_retention_role=log_retention_role,
             memory_size=memory_size,
+            params_and_secrets=params_and_secrets,
             profiling=profiling,
             profiling_group=profiling_group,
             reserved_concurrent_executions=reserved_concurrent_executions,
             role=role,
             runtime_management_mode=runtime_management_mode,
             security_groups=security_groups,
             timeout=timeout,
@@ -2257,14 +2304,15 @@
         initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
         layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
         log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
         log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         memory_size: typing.Optional[jsii.Number] = None,
+        params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
         profiling: typing.Optional[builtins.bool] = None,
         profiling_group: typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup] = None,
         reserved_concurrent_executions: typing.Optional[jsii.Number] = None,
         role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         runtime_management_mode: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode] = None,
         security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
         timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
@@ -2312,14 +2360,15 @@
         :param initial_policy: Initial policy statements to add to the created Lambda Role. You can call ``addToRolePolicy`` to the created lambda to add statements post creation. Default: - No policy statements are added to the created Lambda role.
         :param insights_version: Specify the version of CloudWatch Lambda insights to use for monitoring. Default: - No Lambda Insights
         :param layers: A list of layers to add to the function's execution environment. You can configure your Lambda function to pull in additional code during initialization in the form of layers. Layers are packages of libraries or other dependencies that can be used by multiple functions. Default: - No layers.
         :param log_retention: The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.INFINITE
         :param log_retention_retry_options: When log retention is specified, a custom resource attempts to create the CloudWatch log group. These options control the retry policy when interacting with CloudWatch APIs. Default: - Default AWS SDK retry options.
         :param log_retention_role: The IAM role for the Lambda function associated with the custom resource that sets the retention policy. Default: - A new role is created.
         :param memory_size: The amount of memory, in MB, that is allocated to your Lambda function. Lambda uses this value to proportionally allocate the amount of CPU power. For more information, see Resource Model in the AWS Lambda Developer Guide. Default: 128
+        :param params_and_secrets: Specify the configuration of Parameters and Secrets Extension. Default: - No Parameters and Secrets Extension
         :param profiling: Enable profiling. Default: - No profiling.
         :param profiling_group: Profiling Group. Default: - A new profiling group will be created if ``profiling`` is set.
         :param reserved_concurrent_executions: The maximum of concurrent executions you want to reserve for the function. Default: - No specific limit - account limit.
         :param role: Lambda execution role. This is the role that will be assumed by the function upon execution. It controls the permissions that the function will have. The Role must be assumable by the 'lambda.amazonaws.com' service principal. The default Role automatically has permissions granted for Lambda execution. If you provide a Role, you must add the relevant AWS managed policies yourself. The relevant managed policies are "service-role/AWSLambdaBasicExecutionRole" and "service-role/AWSLambdaVPCAccessExecutionRole". Default: - A unique role will be generated for this lambda function. Both supplied and generated roles can always be changed by calling ``addToRolePolicy``.
         :param runtime_management_mode: Sets the runtime management configuration for a function's version. Default: Auto
         :param security_groups: The list of security groups to associate with the Lambda's network interfaces. Only used if 'vpc' is supplied. Default: - If the function is placed within a VPC and a security group is not specified, either by this or securityGroup prop, a dedicated security group will be created for this function.
         :param timeout: The function execution time (in seconds) after which Lambda terminates the function. Because the execution time affects cost, set this value based on the function's expected execution time. Default: Duration.seconds(3)
@@ -2369,14 +2418,15 @@
             initial_policy=initial_policy,
             insights_version=insights_version,
             layers=layers,
             log_retention=log_retention,
             log_retention_retry_options=log_retention_retry_options,
             log_retention_role=log_retention_role,
             memory_size=memory_size,
+            params_and_secrets=params_and_secrets,
             profiling=profiling,
             profiling_group=profiling_group,
             reserved_concurrent_executions=reserved_concurrent_executions,
             role=role,
             runtime_management_mode=runtime_management_mode,
             security_groups=security_groups,
             timeout=timeout,
@@ -2504,14 +2554,15 @@
         "initial_policy": "initialPolicy",
         "insights_version": "insightsVersion",
         "layers": "layers",
         "log_retention": "logRetention",
         "log_retention_retry_options": "logRetentionRetryOptions",
         "log_retention_role": "logRetentionRole",
         "memory_size": "memorySize",
+        "params_and_secrets": "paramsAndSecrets",
         "profiling": "profiling",
         "profiling_group": "profilingGroup",
         "reserved_concurrent_executions": "reservedConcurrentExecutions",
         "role": "role",
         "runtime_management_mode": "runtimeManagementMode",
         "security_groups": "securityGroups",
         "timeout": "timeout",
@@ -2557,14 +2608,15 @@
         initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
         layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
         log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
         log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         memory_size: typing.Optional[jsii.Number] = None,
+        params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
         profiling: typing.Optional[builtins.bool] = None,
         profiling_group: typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup] = None,
         reserved_concurrent_executions: typing.Optional[jsii.Number] = None,
         role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         runtime_management_mode: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode] = None,
         security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
         timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
@@ -2606,14 +2658,15 @@
         :param initial_policy: Initial policy statements to add to the created Lambda Role. You can call ``addToRolePolicy`` to the created lambda to add statements post creation. Default: - No policy statements are added to the created Lambda role.
         :param insights_version: Specify the version of CloudWatch Lambda insights to use for monitoring. Default: - No Lambda Insights
         :param layers: A list of layers to add to the function's execution environment. You can configure your Lambda function to pull in additional code during initialization in the form of layers. Layers are packages of libraries or other dependencies that can be used by multiple functions. Default: - No layers.
         :param log_retention: The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.INFINITE
         :param log_retention_retry_options: When log retention is specified, a custom resource attempts to create the CloudWatch log group. These options control the retry policy when interacting with CloudWatch APIs. Default: - Default AWS SDK retry options.
         :param log_retention_role: The IAM role for the Lambda function associated with the custom resource that sets the retention policy. Default: - A new role is created.
         :param memory_size: The amount of memory, in MB, that is allocated to your Lambda function. Lambda uses this value to proportionally allocate the amount of CPU power. For more information, see Resource Model in the AWS Lambda Developer Guide. Default: 128
+        :param params_and_secrets: Specify the configuration of Parameters and Secrets Extension. Default: - No Parameters and Secrets Extension
         :param profiling: Enable profiling. Default: - No profiling.
         :param profiling_group: Profiling Group. Default: - A new profiling group will be created if ``profiling`` is set.
         :param reserved_concurrent_executions: The maximum of concurrent executions you want to reserve for the function. Default: - No specific limit - account limit.
         :param role: Lambda execution role. This is the role that will be assumed by the function upon execution. It controls the permissions that the function will have. The Role must be assumable by the 'lambda.amazonaws.com' service principal. The default Role automatically has permissions granted for Lambda execution. If you provide a Role, you must add the relevant AWS managed policies yourself. The relevant managed policies are "service-role/AWSLambdaBasicExecutionRole" and "service-role/AWSLambdaVPCAccessExecutionRole". Default: - A unique role will be generated for this lambda function. Both supplied and generated roles can always be changed by calling ``addToRolePolicy``.
         :param runtime_management_mode: Sets the runtime management configuration for a function's version. Default: Auto
         :param security_groups: The list of security groups to associate with the Lambda's network interfaces. Only used if 'vpc' is supplied. Default: - If the function is placed within a VPC and a security group is not specified, either by this or securityGroup prop, a dedicated security group will be created for this function.
         :param timeout: The function execution time (in seconds) after which Lambda terminates the function. Because the execution time affects cost, set this value based on the function's expected execution time. Default: Duration.seconds(3)
@@ -2664,14 +2717,15 @@
             check_type(argname="argument initial_policy", value=initial_policy, expected_type=type_hints["initial_policy"])
             check_type(argname="argument insights_version", value=insights_version, expected_type=type_hints["insights_version"])
             check_type(argname="argument layers", value=layers, expected_type=type_hints["layers"])
             check_type(argname="argument log_retention", value=log_retention, expected_type=type_hints["log_retention"])
             check_type(argname="argument log_retention_retry_options", value=log_retention_retry_options, expected_type=type_hints["log_retention_retry_options"])
             check_type(argname="argument log_retention_role", value=log_retention_role, expected_type=type_hints["log_retention_role"])
             check_type(argname="argument memory_size", value=memory_size, expected_type=type_hints["memory_size"])
+            check_type(argname="argument params_and_secrets", value=params_and_secrets, expected_type=type_hints["params_and_secrets"])
             check_type(argname="argument profiling", value=profiling, expected_type=type_hints["profiling"])
             check_type(argname="argument profiling_group", value=profiling_group, expected_type=type_hints["profiling_group"])
             check_type(argname="argument reserved_concurrent_executions", value=reserved_concurrent_executions, expected_type=type_hints["reserved_concurrent_executions"])
             check_type(argname="argument role", value=role, expected_type=type_hints["role"])
             check_type(argname="argument runtime_management_mode", value=runtime_management_mode, expected_type=type_hints["runtime_management_mode"])
             check_type(argname="argument security_groups", value=security_groups, expected_type=type_hints["security_groups"])
             check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
@@ -2747,14 +2801,16 @@
             self._values["log_retention"] = log_retention
         if log_retention_retry_options is not None:
             self._values["log_retention_retry_options"] = log_retention_retry_options
         if log_retention_role is not None:
             self._values["log_retention_role"] = log_retention_role
         if memory_size is not None:
             self._values["memory_size"] = memory_size
+        if params_and_secrets is not None:
+            self._values["params_and_secrets"] = params_and_secrets
         if profiling is not None:
             self._values["profiling"] = profiling
         if profiling_group is not None:
             self._values["profiling_group"] = profiling_group
         if reserved_concurrent_executions is not None:
             self._values["reserved_concurrent_executions"] = reserved_concurrent_executions
         if role is not None:
@@ -3090,14 +3146,27 @@
 
         :default: 128
         '''
         result = self._values.get("memory_size")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
+    def params_and_secrets(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion]:
+        '''Specify the configuration of Parameters and Secrets Extension.
+
+        :default: - No Parameters and Secrets Extension
+
+        :see: https://docs.aws.amazon.com/systems-manager/latest/userguide/ps-integration-lambda-extensions.html
+        '''
+        result = self._values.get("params_and_secrets")
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion], result)
+
+    @builtins.property
     def profiling(self) -> typing.Optional[builtins.bool]:
         '''Enable profiling.
 
         :default: - No profiling.
 
         :see: https://docs.aws.amazon.com/codeguru/latest/profiler-ug/setting-up-lambda.html
         '''
@@ -3347,14 +3416,15 @@
         "initial_policy": "initialPolicy",
         "insights_version": "insightsVersion",
         "layers": "layers",
         "log_retention": "logRetention",
         "log_retention_retry_options": "logRetentionRetryOptions",
         "log_retention_role": "logRetentionRole",
         "memory_size": "memorySize",
+        "params_and_secrets": "paramsAndSecrets",
         "profiling": "profiling",
         "profiling_group": "profilingGroup",
         "reserved_concurrent_executions": "reservedConcurrentExecutions",
         "role": "role",
         "runtime_management_mode": "runtimeManagementMode",
         "security_groups": "securityGroups",
         "timeout": "timeout",
@@ -3404,14 +3474,15 @@
         initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
         layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
         log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
         log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         memory_size: typing.Optional[jsii.Number] = None,
+        params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
         profiling: typing.Optional[builtins.bool] = None,
         profiling_group: typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup] = None,
         reserved_concurrent_executions: typing.Optional[jsii.Number] = None,
         role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         runtime_management_mode: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode] = None,
         security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
         timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
@@ -3457,14 +3528,15 @@
         :param initial_policy: Initial policy statements to add to the created Lambda Role. You can call ``addToRolePolicy`` to the created lambda to add statements post creation. Default: - No policy statements are added to the created Lambda role.
         :param insights_version: Specify the version of CloudWatch Lambda insights to use for monitoring. Default: - No Lambda Insights
         :param layers: A list of layers to add to the function's execution environment. You can configure your Lambda function to pull in additional code during initialization in the form of layers. Layers are packages of libraries or other dependencies that can be used by multiple functions. Default: - No layers.
         :param log_retention: The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.INFINITE
         :param log_retention_retry_options: When log retention is specified, a custom resource attempts to create the CloudWatch log group. These options control the retry policy when interacting with CloudWatch APIs. Default: - Default AWS SDK retry options.
         :param log_retention_role: The IAM role for the Lambda function associated with the custom resource that sets the retention policy. Default: - A new role is created.
         :param memory_size: The amount of memory, in MB, that is allocated to your Lambda function. Lambda uses this value to proportionally allocate the amount of CPU power. For more information, see Resource Model in the AWS Lambda Developer Guide. Default: 128
+        :param params_and_secrets: Specify the configuration of Parameters and Secrets Extension. Default: - No Parameters and Secrets Extension
         :param profiling: Enable profiling. Default: - No profiling.
         :param profiling_group: Profiling Group. Default: - A new profiling group will be created if ``profiling`` is set.
         :param reserved_concurrent_executions: The maximum of concurrent executions you want to reserve for the function. Default: - No specific limit - account limit.
         :param role: Lambda execution role. This is the role that will be assumed by the function upon execution. It controls the permissions that the function will have. The Role must be assumable by the 'lambda.amazonaws.com' service principal. The default Role automatically has permissions granted for Lambda execution. If you provide a Role, you must add the relevant AWS managed policies yourself. The relevant managed policies are "service-role/AWSLambdaBasicExecutionRole" and "service-role/AWSLambdaVPCAccessExecutionRole". Default: - A unique role will be generated for this lambda function. Both supplied and generated roles can always be changed by calling ``addToRolePolicy``.
         :param runtime_management_mode: Sets the runtime management configuration for a function's version. Default: Auto
         :param security_groups: The list of security groups to associate with the Lambda's network interfaces. Only used if 'vpc' is supplied. Default: - If the function is placed within a VPC and a security group is not specified, either by this or securityGroup prop, a dedicated security group will be created for this function.
         :param timeout: The function execution time (in seconds) after which Lambda terminates the function. Because the execution time affects cost, set this value based on the function's expected execution time. Default: Duration.seconds(3)
@@ -3521,14 +3593,15 @@
             check_type(argname="argument initial_policy", value=initial_policy, expected_type=type_hints["initial_policy"])
             check_type(argname="argument insights_version", value=insights_version, expected_type=type_hints["insights_version"])
             check_type(argname="argument layers", value=layers, expected_type=type_hints["layers"])
             check_type(argname="argument log_retention", value=log_retention, expected_type=type_hints["log_retention"])
             check_type(argname="argument log_retention_retry_options", value=log_retention_retry_options, expected_type=type_hints["log_retention_retry_options"])
             check_type(argname="argument log_retention_role", value=log_retention_role, expected_type=type_hints["log_retention_role"])
             check_type(argname="argument memory_size", value=memory_size, expected_type=type_hints["memory_size"])
+            check_type(argname="argument params_and_secrets", value=params_and_secrets, expected_type=type_hints["params_and_secrets"])
             check_type(argname="argument profiling", value=profiling, expected_type=type_hints["profiling"])
             check_type(argname="argument profiling_group", value=profiling_group, expected_type=type_hints["profiling_group"])
             check_type(argname="argument reserved_concurrent_executions", value=reserved_concurrent_executions, expected_type=type_hints["reserved_concurrent_executions"])
             check_type(argname="argument role", value=role, expected_type=type_hints["role"])
             check_type(argname="argument runtime_management_mode", value=runtime_management_mode, expected_type=type_hints["runtime_management_mode"])
             check_type(argname="argument security_groups", value=security_groups, expected_type=type_hints["security_groups"])
             check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
@@ -3605,14 +3678,16 @@
             self._values["log_retention"] = log_retention
         if log_retention_retry_options is not None:
             self._values["log_retention_retry_options"] = log_retention_retry_options
         if log_retention_role is not None:
             self._values["log_retention_role"] = log_retention_role
         if memory_size is not None:
             self._values["memory_size"] = memory_size
+        if params_and_secrets is not None:
+            self._values["params_and_secrets"] = params_and_secrets
         if profiling is not None:
             self._values["profiling"] = profiling
         if profiling_group is not None:
             self._values["profiling_group"] = profiling_group
         if reserved_concurrent_executions is not None:
             self._values["reserved_concurrent_executions"] = reserved_concurrent_executions
         if role is not None:
@@ -3962,14 +4037,27 @@
 
         :default: 128
         '''
         result = self._values.get("memory_size")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
+    def params_and_secrets(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion]:
+        '''Specify the configuration of Parameters and Secrets Extension.
+
+        :default: - No Parameters and Secrets Extension
+
+        :see: https://docs.aws.amazon.com/systems-manager/latest/userguide/ps-integration-lambda-extensions.html
+        '''
+        result = self._values.get("params_and_secrets")
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion], result)
+
+    @builtins.property
     def profiling(self) -> typing.Optional[builtins.bool]:
         '''Enable profiling.
 
         :default: - No profiling.
 
         :see: https://docs.aws.amazon.com/codeguru/latest/profiler-ug/setting-up-lambda.html
         '''
@@ -4285,14 +4373,15 @@
     initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
     layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
     log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
     log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     memory_size: typing.Optional[jsii.Number] = None,
+    params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
     profiling: typing.Optional[builtins.bool] = None,
     profiling_group: typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup] = None,
     reserved_concurrent_executions: typing.Optional[jsii.Number] = None,
     role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     runtime_management_mode: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode] = None,
     security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
     timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
@@ -4340,14 +4429,15 @@
     initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
     layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
     log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
     log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     memory_size: typing.Optional[jsii.Number] = None,
+    params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
     profiling: typing.Optional[builtins.bool] = None,
     profiling_group: typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup] = None,
     reserved_concurrent_executions: typing.Optional[jsii.Number] = None,
     role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     runtime_management_mode: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode] = None,
     security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
     timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
@@ -4387,14 +4477,15 @@
     initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
     layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
     log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
     log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     memory_size: typing.Optional[jsii.Number] = None,
+    params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
     profiling: typing.Optional[builtins.bool] = None,
     profiling_group: typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup] = None,
     reserved_concurrent_executions: typing.Optional[jsii.Number] = None,
     role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     runtime_management_mode: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode] = None,
     security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
     timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
@@ -4440,14 +4531,15 @@
     initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
     layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
     log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
     log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     memory_size: typing.Optional[jsii.Number] = None,
+    params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
     profiling: typing.Optional[builtins.bool] = None,
     profiling_group: typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup] = None,
     reserved_concurrent_executions: typing.Optional[jsii.Number] = None,
     role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     runtime_management_mode: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode] = None,
     security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
     timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
@@ -4497,14 +4589,15 @@
     initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
     layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
     log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
     log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     memory_size: typing.Optional[jsii.Number] = None,
+    params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
     profiling: typing.Optional[builtins.bool] = None,
     profiling_group: typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup] = None,
     reserved_concurrent_executions: typing.Optional[jsii.Number] = None,
     role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     runtime_management_mode: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode] = None,
     security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
     timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
@@ -4556,14 +4649,15 @@
     initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
     layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
     log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
     log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     memory_size: typing.Optional[jsii.Number] = None,
+    params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
     profiling: typing.Optional[builtins.bool] = None,
     profiling_group: typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup] = None,
     reserved_concurrent_executions: typing.Optional[jsii.Number] = None,
     role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     runtime_management_mode: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode] = None,
     security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
     timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
@@ -4614,14 +4708,15 @@
     initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
     layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
     log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
     log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     memory_size: typing.Optional[jsii.Number] = None,
+    params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
     profiling: typing.Optional[builtins.bool] = None,
     profiling_group: typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup] = None,
     reserved_concurrent_executions: typing.Optional[jsii.Number] = None,
     role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     runtime_management_mode: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode] = None,
     security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
     timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
@@ -4667,14 +4762,15 @@
     initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
     layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
     log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
     log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     memory_size: typing.Optional[jsii.Number] = None,
+    params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
     profiling: typing.Optional[builtins.bool] = None,
     profiling_group: typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup] = None,
     reserved_concurrent_executions: typing.Optional[jsii.Number] = None,
     role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     runtime_management_mode: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode] = None,
     security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
     timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
```

### Comparing `neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/newrelic/__init__.py` & `neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/newrelic/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         stage: builtins.str,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
         permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
+        suppress_template_indentation: typing.Optional[builtins.bool] = None,
         synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
@@ -79,14 +80,15 @@
         :param stage: 
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
         :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
+        :param suppress_template_indentation: Enable this flag to suppress indentation in generated CloudFormation templates. If not specified, the value of the ``@aws-cdk/core:suppressTemplateIndentation`` context key will be used. If that is not specified, then the default value ``false`` will be used. Default: - the value of ``@aws-cdk/core:suppressTemplateIndentation``, or ``false`` if that is not set.
         :param synthesizer: Synthesis method to use while deploying this stack. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used. If that is not specified, ``DefaultStackSynthesizer`` is used if ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no other synthesizer is specified. Default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
         :param tags: Stack tags that will be applied to all the taggable resources and the stack itself. Default: {}
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3d16994fa6098e1a11bee3003bb87e23e040f04cdc0edc42f729eccb764b26ca)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
@@ -100,14 +102,15 @@
             stage=stage,
             analytics_reporting=analytics_reporting,
             cross_region_references=cross_region_references,
             description=description,
             env=env,
             permissions_boundary=permissions_boundary,
             stack_name=stack_name,
+            suppress_template_indentation=suppress_template_indentation,
             synthesizer=synthesizer,
             tags=tags,
             termination_protection=termination_protection,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
@@ -320,14 +323,15 @@
     name_mapping={
         "analytics_reporting": "analyticsReporting",
         "cross_region_references": "crossRegionReferences",
         "description": "description",
         "env": "env",
         "permissions_boundary": "permissionsBoundary",
         "stack_name": "stackName",
+        "suppress_template_indentation": "suppressTemplateIndentation",
         "synthesizer": "synthesizer",
         "tags": "tags",
         "termination_protection": "terminationProtection",
         "stage": "stage",
         "new_relic_account_id": "newRelicAccountId",
         "new_relic_api_url_logs": "newRelicApiUrlLogs",
         "new_relic_api_url_metrics": "newRelicApiUrlMetrics",
@@ -341,14 +345,15 @@
         *,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
         permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
+        suppress_template_indentation: typing.Optional[builtins.bool] = None,
         synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
         stage: builtins.str,
         new_relic_account_id: builtins.str,
         new_relic_api_url_logs: EndpointUrlLogs,
         new_relic_api_url_metrics: EndpointUrlMetrics,
@@ -358,14 +363,15 @@
         '''
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
         :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
+        :param suppress_template_indentation: Enable this flag to suppress indentation in generated CloudFormation templates. If not specified, the value of the ``@aws-cdk/core:suppressTemplateIndentation`` context key will be used. If that is not specified, then the default value ``false`` will be used. Default: - the value of ``@aws-cdk/core:suppressTemplateIndentation``, or ``false`` if that is not set.
         :param synthesizer: Synthesis method to use while deploying this stack. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used. If that is not specified, ``DefaultStackSynthesizer`` is used if ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no other synthesizer is specified. Default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
         :param tags: Stack tags that will be applied to all the taggable resources and the stack itself. Default: {}
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
         :param stage: 
         :param new_relic_account_id: 
         :param new_relic_api_url_logs: 
         :param new_relic_api_url_metrics: 
@@ -378,14 +384,15 @@
             type_hints = typing.get_type_hints(_typecheckingstub__1b73444472d0b16a38d845ab8c4feabeadd9937eadb9c68ca1f7a002e868c7df)
             check_type(argname="argument analytics_reporting", value=analytics_reporting, expected_type=type_hints["analytics_reporting"])
             check_type(argname="argument cross_region_references", value=cross_region_references, expected_type=type_hints["cross_region_references"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument env", value=env, expected_type=type_hints["env"])
             check_type(argname="argument permissions_boundary", value=permissions_boundary, expected_type=type_hints["permissions_boundary"])
             check_type(argname="argument stack_name", value=stack_name, expected_type=type_hints["stack_name"])
+            check_type(argname="argument suppress_template_indentation", value=suppress_template_indentation, expected_type=type_hints["suppress_template_indentation"])
             check_type(argname="argument synthesizer", value=synthesizer, expected_type=type_hints["synthesizer"])
             check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
             check_type(argname="argument termination_protection", value=termination_protection, expected_type=type_hints["termination_protection"])
             check_type(argname="argument stage", value=stage, expected_type=type_hints["stage"])
             check_type(argname="argument new_relic_account_id", value=new_relic_account_id, expected_type=type_hints["new_relic_account_id"])
             check_type(argname="argument new_relic_api_url_logs", value=new_relic_api_url_logs, expected_type=type_hints["new_relic_api_url_logs"])
             check_type(argname="argument new_relic_api_url_metrics", value=new_relic_api_url_metrics, expected_type=type_hints["new_relic_api_url_metrics"])
@@ -407,14 +414,16 @@
             self._values["description"] = description
         if env is not None:
             self._values["env"] = env
         if permissions_boundary is not None:
             self._values["permissions_boundary"] = permissions_boundary
         if stack_name is not None:
             self._values["stack_name"] = stack_name
+        if suppress_template_indentation is not None:
+            self._values["suppress_template_indentation"] = suppress_template_indentation
         if synthesizer is not None:
             self._values["synthesizer"] = synthesizer
         if tags is not None:
             self._values["tags"] = tags
         if termination_protection is not None:
             self._values["termination_protection"] = termination_protection
 
@@ -540,14 +549,27 @@
 
         :default: - Derived from construct path.
         '''
         result = self._values.get("stack_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def suppress_template_indentation(self) -> typing.Optional[builtins.bool]:
+        '''Enable this flag to suppress indentation in generated CloudFormation templates.
+
+        If not specified, the value of the ``@aws-cdk/core:suppressTemplateIndentation``
+        context key will be used. If that is not specified, then the
+        default value ``false`` will be used.
+
+        :default: - the value of ``@aws-cdk/core:suppressTemplateIndentation``, or ``false`` if that is not set.
+        '''
+        result = self._values.get("suppress_template_indentation")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
     def synthesizer(self) -> typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer]:
         '''Synthesis method to use while deploying this stack.
 
         The Stack Synthesizer controls aspects of synthesis and deployment,
         like how assets are referenced and what IAM roles to use. For more
         information, see the README of the main CDK package.
 
@@ -650,14 +672,15 @@
     stage: builtins.str,
     analytics_reporting: typing.Optional[builtins.bool] = None,
     cross_region_references: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
     env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
     permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
     stack_name: typing.Optional[builtins.str] = None,
+    suppress_template_indentation: typing.Optional[builtins.bool] = None,
     synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
     tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     termination_protection: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
@@ -748,14 +771,15 @@
     *,
     analytics_reporting: typing.Optional[builtins.bool] = None,
     cross_region_references: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
     env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
     permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
     stack_name: typing.Optional[builtins.str] = None,
+    suppress_template_indentation: typing.Optional[builtins.bool] = None,
     synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
     tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     termination_protection: typing.Optional[builtins.bool] = None,
     stage: builtins.str,
     new_relic_account_id: builtins.str,
     new_relic_api_url_logs: EndpointUrlLogs,
     new_relic_api_url_metrics: EndpointUrlMetrics,
```

### Comparing `neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/oidc/__init__.py` & `neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/oidc/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         stage: builtins.str,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
         permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
+        suppress_template_indentation: typing.Optional[builtins.bool] = None,
         synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
@@ -67,14 +68,15 @@
         :param stage: 
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
         :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
+        :param suppress_template_indentation: Enable this flag to suppress indentation in generated CloudFormation templates. If not specified, the value of the ``@aws-cdk/core:suppressTemplateIndentation`` context key will be used. If that is not specified, then the default value ``false`` will be used. Default: - the value of ``@aws-cdk/core:suppressTemplateIndentation``, or ``false`` if that is not set.
         :param synthesizer: Synthesis method to use while deploying this stack. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used. If that is not specified, ``DefaultStackSynthesizer`` is used if ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no other synthesizer is specified. Default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
         :param tags: Stack tags that will be applied to all the taggable resources and the stack itself. Default: {}
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__71fabbd315f27662df384897235533205fa1984af573f69ade1128bc72da169d)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
@@ -93,14 +95,15 @@
             stage=stage,
             analytics_reporting=analytics_reporting,
             cross_region_references=cross_region_references,
             description=description,
             env=env,
             permissions_boundary=permissions_boundary,
             stack_name=stack_name,
+            suppress_template_indentation=suppress_template_indentation,
             synthesizer=synthesizer,
             tags=tags,
             termination_protection=termination_protection,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
@@ -310,14 +313,15 @@
     name_mapping={
         "analytics_reporting": "analyticsReporting",
         "cross_region_references": "crossRegionReferences",
         "description": "description",
         "env": "env",
         "permissions_boundary": "permissionsBoundary",
         "stack_name": "stackName",
+        "suppress_template_indentation": "suppressTemplateIndentation",
         "synthesizer": "synthesizer",
         "tags": "tags",
         "termination_protection": "terminationProtection",
         "stage": "stage",
         "github_repository": "githubRepository",
         "github_user": "githubUser",
         "token_action": "tokenAction",
@@ -336,14 +340,15 @@
         *,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
         permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
+        suppress_template_indentation: typing.Optional[builtins.bool] = None,
         synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
         stage: builtins.str,
         github_repository: builtins.str,
         github_user: builtins.str,
         token_action: "TokenActions",
@@ -358,14 +363,15 @@
         '''
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
         :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
+        :param suppress_template_indentation: Enable this flag to suppress indentation in generated CloudFormation templates. If not specified, the value of the ``@aws-cdk/core:suppressTemplateIndentation`` context key will be used. If that is not specified, then the default value ``false`` will be used. Default: - the value of ``@aws-cdk/core:suppressTemplateIndentation``, or ``false`` if that is not set.
         :param synthesizer: Synthesis method to use while deploying this stack. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used. If that is not specified, ``DefaultStackSynthesizer`` is used if ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no other synthesizer is specified. Default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
         :param tags: Stack tags that will be applied to all the taggable resources and the stack itself. Default: {}
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
         :param stage: 
         :param github_repository: 
         :param github_user: 
         :param token_action: 
@@ -383,14 +389,15 @@
             type_hints = typing.get_type_hints(_typecheckingstub__81f6128649596f1f89adf6d54553924e5a8f7172f0dbfd21eefa659cb4adb68d)
             check_type(argname="argument analytics_reporting", value=analytics_reporting, expected_type=type_hints["analytics_reporting"])
             check_type(argname="argument cross_region_references", value=cross_region_references, expected_type=type_hints["cross_region_references"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument env", value=env, expected_type=type_hints["env"])
             check_type(argname="argument permissions_boundary", value=permissions_boundary, expected_type=type_hints["permissions_boundary"])
             check_type(argname="argument stack_name", value=stack_name, expected_type=type_hints["stack_name"])
+            check_type(argname="argument suppress_template_indentation", value=suppress_template_indentation, expected_type=type_hints["suppress_template_indentation"])
             check_type(argname="argument synthesizer", value=synthesizer, expected_type=type_hints["synthesizer"])
             check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
             check_type(argname="argument termination_protection", value=termination_protection, expected_type=type_hints["termination_protection"])
             check_type(argname="argument stage", value=stage, expected_type=type_hints["stage"])
             check_type(argname="argument github_repository", value=github_repository, expected_type=type_hints["github_repository"])
             check_type(argname="argument github_user", value=github_user, expected_type=type_hints["github_user"])
             check_type(argname="argument token_action", value=token_action, expected_type=type_hints["token_action"])
@@ -415,14 +422,16 @@
             self._values["description"] = description
         if env is not None:
             self._values["env"] = env
         if permissions_boundary is not None:
             self._values["permissions_boundary"] = permissions_boundary
         if stack_name is not None:
             self._values["stack_name"] = stack_name
+        if suppress_template_indentation is not None:
+            self._values["suppress_template_indentation"] = suppress_template_indentation
         if synthesizer is not None:
             self._values["synthesizer"] = synthesizer
         if tags is not None:
             self._values["tags"] = tags
         if termination_protection is not None:
             self._values["termination_protection"] = termination_protection
         if cdk_bootstrap_role_name is not None:
@@ -562,14 +571,27 @@
 
         :default: - Derived from construct path.
         '''
         result = self._values.get("stack_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def suppress_template_indentation(self) -> typing.Optional[builtins.bool]:
+        '''Enable this flag to suppress indentation in generated CloudFormation templates.
+
+        If not specified, the value of the ``@aws-cdk/core:suppressTemplateIndentation``
+        context key will be used. If that is not specified, then the
+        default value ``false`` will be used.
+
+        :default: - the value of ``@aws-cdk/core:suppressTemplateIndentation``, or ``false`` if that is not set.
+        '''
+        result = self._values.get("suppress_template_indentation")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
     def synthesizer(self) -> typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer]:
         '''Synthesis method to use while deploying this stack.
 
         The Stack Synthesizer controls aspects of synthesis and deployment,
         like how assets are referenced and what IAM roles to use. For more
         information, see the README of the main CDK package.
 
@@ -719,14 +741,15 @@
     stage: builtins.str,
     analytics_reporting: typing.Optional[builtins.bool] = None,
     cross_region_references: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
     env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
     permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
     stack_name: typing.Optional[builtins.str] = None,
+    suppress_template_indentation: typing.Optional[builtins.bool] = None,
     synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
     tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     termination_protection: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
@@ -820,14 +843,15 @@
     *,
     analytics_reporting: typing.Optional[builtins.bool] = None,
     cross_region_references: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
     env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
     permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
     stack_name: typing.Optional[builtins.str] = None,
+    suppress_template_indentation: typing.Optional[builtins.bool] = None,
     synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
     tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     termination_protection: typing.Optional[builtins.bool] = None,
     stage: builtins.str,
     github_repository: builtins.str,
     github_user: builtins.str,
     token_action: TokenActions,
```

### Comparing `neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/stack/__init__.py` & `neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/stack/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,28 +31,30 @@
         stage: builtins.str,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
         permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
+        suppress_template_indentation: typing.Optional[builtins.bool] = None,
         synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param stage: 
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
         :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
+        :param suppress_template_indentation: Enable this flag to suppress indentation in generated CloudFormation templates. If not specified, the value of the ``@aws-cdk/core:suppressTemplateIndentation`` context key will be used. If that is not specified, then the default value ``false`` will be used. Default: - the value of ``@aws-cdk/core:suppressTemplateIndentation``, or ``false`` if that is not set.
         :param synthesizer: Synthesis method to use while deploying this stack. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used. If that is not specified, ``DefaultStackSynthesizer`` is used if ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no other synthesizer is specified. Default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
         :param tags: Stack tags that will be applied to all the taggable resources and the stack itself. Default: {}
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e4153b60b9209d8e364add8997864a1fbf9e22e728d8d4e8ef7a7bdd78f4fe13)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
@@ -61,14 +63,15 @@
             stage=stage,
             analytics_reporting=analytics_reporting,
             cross_region_references=cross_region_references,
             description=description,
             env=env,
             permissions_boundary=permissions_boundary,
             stack_name=stack_name,
+            suppress_template_indentation=suppress_template_indentation,
             synthesizer=synthesizer,
             tags=tags,
             termination_protection=termination_protection,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
@@ -124,14 +127,15 @@
     name_mapping={
         "analytics_reporting": "analyticsReporting",
         "cross_region_references": "crossRegionReferences",
         "description": "description",
         "env": "env",
         "permissions_boundary": "permissionsBoundary",
         "stack_name": "stackName",
+        "suppress_template_indentation": "suppressTemplateIndentation",
         "synthesizer": "synthesizer",
         "tags": "tags",
         "termination_protection": "terminationProtection",
         "stage": "stage",
     },
 )
 class BaseStackProps(_aws_cdk_ceddda9d.StackProps):
@@ -140,26 +144,28 @@
         *,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
         permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
+        suppress_template_indentation: typing.Optional[builtins.bool] = None,
         synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
         stage: builtins.str,
     ) -> None:
         '''
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
         :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
+        :param suppress_template_indentation: Enable this flag to suppress indentation in generated CloudFormation templates. If not specified, the value of the ``@aws-cdk/core:suppressTemplateIndentation`` context key will be used. If that is not specified, then the default value ``false`` will be used. Default: - the value of ``@aws-cdk/core:suppressTemplateIndentation``, or ``false`` if that is not set.
         :param synthesizer: Synthesis method to use while deploying this stack. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used. If that is not specified, ``DefaultStackSynthesizer`` is used if ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no other synthesizer is specified. Default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
         :param tags: Stack tags that will be applied to all the taggable resources and the stack itself. Default: {}
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
         :param stage: 
         '''
         if isinstance(env, dict):
             env = _aws_cdk_ceddda9d.Environment(**env)
@@ -167,14 +173,15 @@
             type_hints = typing.get_type_hints(_typecheckingstub__4d2e6f768ec47790d726319d10913ccfa23e362ae601f2be29634b1ab2282009)
             check_type(argname="argument analytics_reporting", value=analytics_reporting, expected_type=type_hints["analytics_reporting"])
             check_type(argname="argument cross_region_references", value=cross_region_references, expected_type=type_hints["cross_region_references"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument env", value=env, expected_type=type_hints["env"])
             check_type(argname="argument permissions_boundary", value=permissions_boundary, expected_type=type_hints["permissions_boundary"])
             check_type(argname="argument stack_name", value=stack_name, expected_type=type_hints["stack_name"])
+            check_type(argname="argument suppress_template_indentation", value=suppress_template_indentation, expected_type=type_hints["suppress_template_indentation"])
             check_type(argname="argument synthesizer", value=synthesizer, expected_type=type_hints["synthesizer"])
             check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
             check_type(argname="argument termination_protection", value=termination_protection, expected_type=type_hints["termination_protection"])
             check_type(argname="argument stage", value=stage, expected_type=type_hints["stage"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "stage": stage,
         }
@@ -186,14 +193,16 @@
             self._values["description"] = description
         if env is not None:
             self._values["env"] = env
         if permissions_boundary is not None:
             self._values["permissions_boundary"] = permissions_boundary
         if stack_name is not None:
             self._values["stack_name"] = stack_name
+        if suppress_template_indentation is not None:
+            self._values["suppress_template_indentation"] = suppress_template_indentation
         if synthesizer is not None:
             self._values["synthesizer"] = synthesizer
         if tags is not None:
             self._values["tags"] = tags
         if termination_protection is not None:
             self._values["termination_protection"] = termination_protection
 
@@ -319,14 +328,27 @@
 
         :default: - Derived from construct path.
         '''
         result = self._values.get("stack_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def suppress_template_indentation(self) -> typing.Optional[builtins.bool]:
+        '''Enable this flag to suppress indentation in generated CloudFormation templates.
+
+        If not specified, the value of the ``@aws-cdk/core:suppressTemplateIndentation``
+        context key will be used. If that is not specified, then the
+        default value ``false`` will be used.
+
+        :default: - the value of ``@aws-cdk/core:suppressTemplateIndentation``, or ``false`` if that is not set.
+        '''
+        result = self._values.get("suppress_template_indentation")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
     def synthesizer(self) -> typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer]:
         '''Synthesis method to use while deploying this stack.
 
         The Stack Synthesizer controls aspects of synthesis and deployment,
         like how assets are referenced and what IAM roles to use. For more
         information, see the README of the main CDK package.
 
@@ -391,14 +413,15 @@
     stage: builtins.str,
     analytics_reporting: typing.Optional[builtins.bool] = None,
     cross_region_references: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
     env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
     permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
     stack_name: typing.Optional[builtins.str] = None,
+    suppress_template_indentation: typing.Optional[builtins.bool] = None,
     synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
     tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     termination_protection: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
@@ -423,14 +446,15 @@
     *,
     analytics_reporting: typing.Optional[builtins.bool] = None,
     cross_region_references: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
     env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
     permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
     stack_name: typing.Optional[builtins.str] = None,
+    suppress_template_indentation: typing.Optional[builtins.bool] = None,
     synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
     tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     termination_protection: typing.Optional[builtins.bool] = None,
     stage: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs/utils/__init__.py` & `neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs.egg-info/PKG-INFO` & `neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neulabs-cdk-constructs
-Version: 0.4.8
+Version: 0.5.0
 Summary: neulabs-cdk-constructs
 Home-page: https://github.com/neulabscom/neulabs-cdk-constructs.git
 Author: Neulabs<tech@neulabs.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neulabscom/neulabs-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `neulabs-cdk-constructs-0.4.8/src/neulabs_cdk_constructs.egg-info/SOURCES.txt` & `neulabs-cdk-constructs-0.5.0/src/neulabs_cdk_constructs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 src/neulabs_cdk_constructs/py.typed
 src/neulabs_cdk_constructs.egg-info/PKG-INFO
 src/neulabs_cdk_constructs.egg-info/SOURCES.txt
 src/neulabs_cdk_constructs.egg-info/dependency_links.txt
 src/neulabs_cdk_constructs.egg-info/requires.txt
 src/neulabs_cdk_constructs.egg-info/top_level.txt
 src/neulabs_cdk_constructs/_jsii/__init__.py
-src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.4.8.jsii.tgz
+src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.5.0.jsii.tgz
 src/neulabs_cdk_constructs/aws_lambda/__init__.py
 src/neulabs_cdk_constructs/newrelic/__init__.py
 src/neulabs_cdk_constructs/oidc/__init__.py
 src/neulabs_cdk_constructs/stack/__init__.py
 src/neulabs_cdk_constructs/utils/__init__.py
```

