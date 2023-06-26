# Comparing `tmp/pulser-0.9.2-py3-none-any.whl.zip` & `tmp/pulser-0.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 6761 bytes, number of entries: 5
--rw-r--r--  2.0 unx    11358 b- defN 23-Feb-16 16:52 pulser-0.9.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3869 b- defN 23-Feb-16 16:52 pulser-0.9.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-16 16:52 pulser-0.9.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Feb-16 16:52 pulser-0.9.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      381 b- defN 23-Feb-16 16:52 pulser-0.9.2.dist-info/RECORD
-5 files, 15701 bytes uncompressed, 6051 bytes compressed:  61.5%
+Zip file size: 6760 bytes, number of entries: 5
+-rw-r--r--  2.0 unx    11358 b- defN 23-Feb-24 14:04 pulser-0.9.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3869 b- defN 23-Feb-24 14:04 pulser-0.9.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Feb-24 14:04 pulser-0.9.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Feb-24 14:04 pulser-0.9.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      381 b- defN 23-Feb-24 14:04 pulser-0.9.3.dist-info/RECORD
+5 files, 15701 bytes uncompressed, 6050 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: pulser-0.9.2.dist-info/LICENSE
+Filename: pulser-0.9.3.dist-info/LICENSE
 Comment: 
 
-Filename: pulser-0.9.2.dist-info/METADATA
+Filename: pulser-0.9.3.dist-info/METADATA
 Comment: 
 
-Filename: pulser-0.9.2.dist-info/WHEEL
+Filename: pulser-0.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: pulser-0.9.2.dist-info/top_level.txt
+Filename: pulser-0.9.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pulser-0.9.2.dist-info/RECORD
+Filename: pulser-0.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pulser-0.9.2.dist-info/LICENSE` & `pulser-0.9.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pulser-0.9.2.dist-info/METADATA` & `pulser-0.9.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pulser
-Version: 0.9.2
+Version: 0.9.3
 Summary: A pulse-level composer for neutral-atom quantum devices.
 Home-page: https://github.com/pasqal-io/Pulser
 Author: Pulser Development Team
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pulser-core (==0.9.2)
-Requires-Dist: pulser-simulation (==0.9.2)
-Requires-Dist: pulser-pasqal (==0.9.2)
+Requires-Dist: pulser-core (==0.9.3)
+Requires-Dist: pulser-simulation (==0.9.3)
+Requires-Dist: pulser-pasqal (==0.9.3)
 
 # Pulser
 
 Pulser is a framework for composing, simulating and executing **pulse** sequences for neutral-atom quantum devices.
 
 **Documentation** for the [latest release](https://pypi.org/project/pulser/) of `pulser` is available at <https://pulser.readthedocs.io> (for the docs tracking the `develop` branch of this repository, visit <https://pulser.readthedocs.io/en/latest> instead).
```

