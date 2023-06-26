# Comparing `tmp/pulser_pasqal-0.9.2-py3-none-any.whl.zip` & `tmp/pulser_pasqal-0.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9615 bytes, number of entries: 10
--rw-r--r--  2.0 unx      860 b- defN 23-Feb-16 16:52 pulser_pasqal/__init__.py
--rw-r--r--  2.0 unx       22 b- defN 23-Feb-16 16:52 pulser_pasqal/_version.py
--rw-r--r--  2.0 unx     2231 b- defN 23-Feb-16 16:52 pulser_pasqal/job_parameters.py
--rw-r--r--  2.0 unx     3983 b- defN 23-Feb-16 16:52 pulser_pasqal/pasqal_cloud.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-16 16:52 pulser_pasqal/py.typed
--rw-r--r--  2.0 unx    11358 b- defN 23-Feb-16 16:52 pulser_pasqal-0.9.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1171 b- defN 23-Feb-16 16:52 pulser_pasqal-0.9.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-16 16:52 pulser_pasqal-0.9.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Feb-16 16:52 pulser_pasqal-0.9.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      828 b- defN 23-Feb-16 16:52 pulser_pasqal-0.9.2.dist-info/RECORD
-10 files, 20559 bytes uncompressed, 8191 bytes compressed:  60.2%
+Zip file size: 9618 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      860 b- defN 23-Feb-24 14:04 pulser_pasqal/__init__.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Feb-24 14:04 pulser_pasqal/_version.py
+-rw-r--r--  2.0 unx     2231 b- defN 23-Feb-24 14:04 pulser_pasqal/job_parameters.py
+-rw-r--r--  2.0 unx     3983 b- defN 23-Feb-24 14:04 pulser_pasqal/pasqal_cloud.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-24 14:04 pulser_pasqal/py.typed
+-rw-r--r--  2.0 unx    11358 b- defN 23-Feb-24 14:04 pulser_pasqal-0.9.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1171 b- defN 23-Feb-24 14:04 pulser_pasqal-0.9.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Feb-24 14:04 pulser_pasqal-0.9.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Feb-24 14:04 pulser_pasqal-0.9.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      828 b- defN 23-Feb-24 14:04 pulser_pasqal-0.9.3.dist-info/RECORD
+10 files, 20559 bytes uncompressed, 8194 bytes compressed:  60.1%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: pulser_pasqal/pasqal_cloud.py
 Comment: 
 
 Filename: pulser_pasqal/py.typed
 Comment: 
 
-Filename: pulser_pasqal-0.9.2.dist-info/LICENSE
+Filename: pulser_pasqal-0.9.3.dist-info/LICENSE
 Comment: 
 
-Filename: pulser_pasqal-0.9.2.dist-info/METADATA
+Filename: pulser_pasqal-0.9.3.dist-info/METADATA
 Comment: 
 
-Filename: pulser_pasqal-0.9.2.dist-info/WHEEL
+Filename: pulser_pasqal-0.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: pulser_pasqal-0.9.2.dist-info/top_level.txt
+Filename: pulser_pasqal-0.9.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pulser_pasqal-0.9.2.dist-info/RECORD
+Filename: pulser_pasqal-0.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pulser_pasqal/_version.py

```diff
@@ -1 +1 @@
-__version__ = '0.9.2'
+__version__ = '0.9.3'
```

## Comparing `pulser_pasqal-0.9.2.dist-info/LICENSE` & `pulser_pasqal-0.9.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pulser_pasqal-0.9.2.dist-info/METADATA` & `pulser_pasqal-0.9.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pulser-pasqal
-Version: 0.9.2
+Version: 0.9.3
 Summary: A Pulser extension to execute pulse-level sequences on Pasqal backends.
 Home-page: https://github.com/pasqal-io/Pulser
 Author: Pulser Development Team
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pasqal-sdk (==0.1.6)
-Requires-Dist: pulser-core (==0.9.2)
+Requires-Dist: pulser-core (==0.9.3)
 
 # pulser-pasqal
 
 [Pulser](https://pypi.org/project/pulser/) is a framework for composing, simulating and executing **pulse** sequences for neutral-atom quantum devices.
 
 This is the `pulser-pasqal` extension, which provides the functionalities needed to execute `pulser` sequences on [Pasqal](https://pasqal.io/)'s backends.
```

## Comparing `pulser_pasqal-0.9.2.dist-info/RECORD` & `pulser_pasqal-0.9.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pulser_pasqal/__init__.py,sha256=cilp9AjiuGceJdJhqAcvNLSWlRnbswQ3WKfSpn4S96s,860
-pulser_pasqal/_version.py,sha256=HSMl6bLm3r1Ias1jHIPpJeQ0IYNuuSdlT38MTb79ewM,22
+pulser_pasqal/_version.py,sha256=83oJ8nCWXwQbno1uqIRolJfmli7BtUNqtuSvnzeSyxg,22
 pulser_pasqal/job_parameters.py,sha256=7uKHShs3rSs96ZfnrORbJTdbEGQ1_aH0eX8igY304qA,2231
 pulser_pasqal/pasqal_cloud.py,sha256=Ms5eVkoZl4A8pVbnD5Dm_-LdkzBljGh2wMoBvYHhNEI,3983
 pulser_pasqal/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pulser_pasqal-0.9.2.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-pulser_pasqal-0.9.2.dist-info/METADATA,sha256=cwwPd6_Acgder_0h1W6JAMXwvSt_4OKLBhx-HsymOpM,1171
-pulser_pasqal-0.9.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pulser_pasqal-0.9.2.dist-info/top_level.txt,sha256=tVH3lcJdmOaGbLttUuIOXOqrDSLoGyFtmLpe3lcUitE,14
-pulser_pasqal-0.9.2.dist-info/RECORD,,
+pulser_pasqal-0.9.3.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+pulser_pasqal-0.9.3.dist-info/METADATA,sha256=O7R1ocGjDjXPaWjxzYTYRQrw2FcSyPzKxE2QaHwWYF8,1171
+pulser_pasqal-0.9.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pulser_pasqal-0.9.3.dist-info/top_level.txt,sha256=tVH3lcJdmOaGbLttUuIOXOqrDSLoGyFtmLpe3lcUitE,14
+pulser_pasqal-0.9.3.dist-info/RECORD,,
```

