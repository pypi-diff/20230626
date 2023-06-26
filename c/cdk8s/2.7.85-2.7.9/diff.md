# Comparing `tmp/cdk8s-2.7.85.tar.gz` & `tmp/cdk8s-2.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-2.7.85.tar", last modified: Mon Jun 26 00:23:20 2023, max compression
+gzip compressed data, was "cdk8s-2.7.9.tar", last modified: Thu Feb 23 00:28:21 2023, max compression
```

## Comparing `cdk8s-2.7.85.tar` & `cdk8s-2.7.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:23:20.255100 cdk8s-2.7.85/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-26 00:23:04.000000 cdk8s-2.7.85/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 00:23:04.000000 cdk8s-2.7.85/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-26 00:23:04.000000 cdk8s-2.7.85/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-26 00:23:20.255100 cdk8s-2.7.85/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-26 00:23:04.000000 cdk8s-2.7.85/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 00:23:04.000000 cdk8s-2.7.85/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 00:23:20.255100 cdk8s-2.7.85/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-26 00:23:04.000000 cdk8s-2.7.85/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:23:20.251100 cdk8s-2.7.85/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:23:20.255100 cdk8s-2.7.85/src/cdk8s/
--rw-r--r--   0 runner    (1001) docker     (123)   138472 2023-06-26 00:23:04.000000 cdk8s-2.7.85/src/cdk8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:23:20.255100 cdk8s-2.7.85/src/cdk8s/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-26 00:23:04.000000 cdk8s-2.7.85/src/cdk8s/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   298132 2023-06-26 00:23:04.000000 cdk8s-2.7.85/src/cdk8s/_jsii/cdk8s@2.7.85.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 00:23:04.000000 cdk8s-2.7.85/src/cdk8s/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:23:20.255100 cdk8s-2.7.85/src/cdk8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-26 00:23:20.000000 cdk8s-2.7.85/src/cdk8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-26 00:23:20.000000 cdk8s-2.7.85/src/cdk8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 00:23:20.000000 cdk8s-2.7.85/src/cdk8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 00:23:20.000000 cdk8s-2.7.85/src/cdk8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 00:23:20.000000 cdk8s-2.7.85/src/cdk8s.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 00:28:21.392573 cdk8s-2.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-23 00:28:07.000000 cdk8s-2.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-23 00:28:07.000000 cdk8s-2.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-23 00:28:07.000000 cdk8s-2.7.9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-02-23 00:28:21.392573 cdk8s-2.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-02-23 00:28:07.000000 cdk8s-2.7.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-23 00:28:07.000000 cdk8s-2.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 00:28:21.392573 cdk8s-2.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-02-23 00:28:07.000000 cdk8s-2.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 00:28:21.388573 cdk8s-2.7.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 00:28:21.388573 cdk8s-2.7.9/src/cdk8s/
+-rw-r--r--   0 runner    (1001) docker     (123)   136004 2023-02-23 00:28:07.000000 cdk8s-2.7.9/src/cdk8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 00:28:21.392573 cdk8s-2.7.9/src/cdk8s/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-02-23 00:28:07.000000 cdk8s-2.7.9/src/cdk8s/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   286735 2023-02-23 00:28:07.000000 cdk8s-2.7.9/src/cdk8s/_jsii/cdk8s@2.7.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 00:28:07.000000 cdk8s-2.7.9/src/cdk8s/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 00:28:21.392573 cdk8s-2.7.9/src/cdk8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-02-23 00:28:21.000000 cdk8s-2.7.9/src/cdk8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-23 00:28:21.000000 cdk8s-2.7.9/src/cdk8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 00:28:21.000000 cdk8s-2.7.9/src/cdk8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-23 00:28:21.000000 cdk8s-2.7.9/src/cdk8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-23 00:28:21.000000 cdk8s-2.7.9/src/cdk8s.egg-info/top_level.txt
```

### Comparing `cdk8s-2.7.85/LICENSE` & `cdk8s-2.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-2.7.85/PKG-INFO` & `cdk8s-2.7.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: cdk8s
-Version: 2.7.85
+Version: 2.7.9
 Summary: This is the core library of Cloud Development Kit (CDK) for Kubernetes (cdk8s). cdk8s apps synthesize into standard Kubernetes manifests which can be applied to any Kubernetes cluster.
 Home-page: https://github.com/cdk8s-team/cdk8s-core.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-core.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
```

### Comparing `cdk8s-2.7.85/README.md` & `cdk8s-2.7.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-2.7.85/setup.py` & `cdk8s-2.7.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s",
-    "version": "2.7.85",
+    "version": "2.7.9",
     "description": "This is the core library of Cloud Development Kit (CDK) for Kubernetes (cdk8s). cdk8s apps synthesize into standard Kubernetes manifests which can be applied to any Kubernetes cluster.",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-core.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,37 +22,36 @@
     },
     "packages": [
         "cdk8s",
         "cdk8s._jsii"
     ],
     "package_data": {
         "cdk8s._jsii": [
-            "cdk8s@2.7.85.jsii.tgz"
+            "cdk8s@2.7.9.jsii.tgz"
         ],
         "cdk8s": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.81.0, <2.0.0",
+        "jsii>=1.75.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `cdk8s-2.7.85/src/cdk8s/__init__.py` & `cdk8s-2.7.9/src/cdk8s/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,28 +69,14 @@
             type_hints = typing.get_type_hints(_typecheckingstub__7c3471c86f94453ef4d9efec6bd8f9cf9dbac2f11db69184e091d0a4f6d502be)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = ApiObjectProps(api_version=api_version, kind=kind, metadata=metadata)
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="isApiObject")
-    @builtins.classmethod
-    def is_api_object(cls, o: typing.Any) -> builtins.bool:
-        '''Return whether the given object is an ``ApiObject``.
-
-        We do attribute detection since we can't reliably use 'instanceof'.
-
-        :param o: The object to check.
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7e1861e2a67b17cc03b65ec7686045b40569487efa29052a042f312c20d14b2c)
-            check_type(argname="argument o", value=o, expected_type=type_hints["o"])
-        return typing.cast(builtins.bool, jsii.sinvoke(cls, "isApiObject", [o]))
-
     @jsii.member(jsii_name="of")
     @builtins.classmethod
     def of(cls, c: _constructs_77d1e7e8.IConstruct) -> "ApiObject":
         '''Returns the ``ApiObject`` named ``Resource`` which is a child of the given construct.
 
         If ``c`` is an ``ApiObject``, it is returned directly. Throws an
         exception if the construct does not have a child named ``Default`` *or* if
@@ -760,34 +746,28 @@
     jsii_type="cdk8s.Chart",
 ):
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
-        disable_resource_name_hashes: typing.Optional[builtins.bool] = None,
         labels: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         namespace: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
-        :param disable_resource_name_hashes: The autogenerated resource name by default is suffixed with a stable hash of the construct path. Setting this property to true drops the hash suffix. Default: false
         :param labels: Labels to apply to all resources in this chart. Default: - no common labels
         :param namespace: The default namespace for all objects defined in this chart (directly or indirectly). This namespace will only apply to objects that don't have a ``namespace`` explicitly defined for them. Default: - no namespace is synthesized (usually this implies "default")
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__aac62dbd05c99a5228dff367434c3e3fca0fb00c841ecd71382b9acd3fc1e30d)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        props = ChartProps(
-            disable_resource_name_hashes=disable_resource_name_hashes,
-            labels=labels,
-            namespace=namespace,
-        )
+        props = ChartProps(labels=labels, namespace=namespace)
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @jsii.member(jsii_name="isChart")
     @builtins.classmethod
     def is_chart(cls, x: typing.Any) -> builtins.bool:
         '''Return whether the given object is a Chart.
@@ -875,58 +855,38 @@
         '''The default namespace for all objects in this chart.'''
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "namespace"))
 
 
 @jsii.data_type(
     jsii_type="cdk8s.ChartProps",
     jsii_struct_bases=[],
-    name_mapping={
-        "disable_resource_name_hashes": "disableResourceNameHashes",
-        "labels": "labels",
-        "namespace": "namespace",
-    },
+    name_mapping={"labels": "labels", "namespace": "namespace"},
 )
 class ChartProps:
     def __init__(
         self,
         *,
-        disable_resource_name_hashes: typing.Optional[builtins.bool] = None,
         labels: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         namespace: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param disable_resource_name_hashes: The autogenerated resource name by default is suffixed with a stable hash of the construct path. Setting this property to true drops the hash suffix. Default: false
         :param labels: Labels to apply to all resources in this chart. Default: - no common labels
         :param namespace: The default namespace for all objects defined in this chart (directly or indirectly). This namespace will only apply to objects that don't have a ``namespace`` explicitly defined for them. Default: - no namespace is synthesized (usually this implies "default")
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__587cc3f5a3d7a6cc9a5690888b75875a8059bcf784bfae23dedf362a06743ee3)
-            check_type(argname="argument disable_resource_name_hashes", value=disable_resource_name_hashes, expected_type=type_hints["disable_resource_name_hashes"])
             check_type(argname="argument labels", value=labels, expected_type=type_hints["labels"])
             check_type(argname="argument namespace", value=namespace, expected_type=type_hints["namespace"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
-        if disable_resource_name_hashes is not None:
-            self._values["disable_resource_name_hashes"] = disable_resource_name_hashes
         if labels is not None:
             self._values["labels"] = labels
         if namespace is not None:
             self._values["namespace"] = namespace
 
     @builtins.property
-    def disable_resource_name_hashes(self) -> typing.Optional[builtins.bool]:
-        '''The autogenerated resource name by default is suffixed with a stable hash of the construct path.
-
-        Setting this property to true drops the hash suffix.
-
-        :default: false
-        '''
-        result = self._values.get("disable_resource_name_hashes")
-        return typing.cast(typing.Optional[builtins.bool], result)
-
-    @builtins.property
     def labels(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''Labels to apply to all resources in this chart.
 
         :default: - no common labels
         '''
         result = self._values.get("labels")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
@@ -2739,20 +2699,14 @@
     api_version: builtins.str,
     kind: builtins.str,
     metadata: typing.Optional[typing.Union[ApiObjectMetadata, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__7e1861e2a67b17cc03b65ec7686045b40569487efa29052a042f312c20d14b2c(
-    o: typing.Any,
-) -> None:
-    """Type checking stubs"""
-    pass
-
 def _typecheckingstub__7c55b2fcd45f38255c26ac00ed411c9af6ec5ea8ba6920c18afedcc214149a4e(
     c: _constructs_77d1e7e8.IConstruct,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__82881106c470fdf7ed8e821d53730213ae34215c35ed597f7708178c0df728bf(
@@ -2831,15 +2785,14 @@
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__aac62dbd05c99a5228dff367434c3e3fca0fb00c841ecd71382b9acd3fc1e30d(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
-    disable_resource_name_hashes: typing.Optional[builtins.bool] = None,
     labels: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     namespace: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__2ac1ee14ad96a56047185b46392b2fba722962d47ed4174705c5dc48101cec6e(
@@ -2864,15 +2817,14 @@
     api_object: ApiObject,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__587cc3f5a3d7a6cc9a5690888b75875a8059bcf784bfae23dedf362a06743ee3(
     *,
-    disable_resource_name_hashes: typing.Optional[builtins.bool] = None,
     labels: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     namespace: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__dc2c750519e19d88bad3a5fad0784148fee43e03a55bddfc61438556ab6bb698(
```

### Comparing `cdk8s-2.7.85/src/cdk8s.egg-info/PKG-INFO` & `cdk8s-2.7.9/src/cdk8s.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: cdk8s
-Version: 2.7.85
+Version: 2.7.9
 Summary: This is the core library of Cloud Development Kit (CDK) for Kubernetes (cdk8s). cdk8s apps synthesize into standard Kubernetes manifests which can be applied to any Kubernetes cluster.
 Home-page: https://github.com/cdk8s-team/cdk8s-core.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-core.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
```

