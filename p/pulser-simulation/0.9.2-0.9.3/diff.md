# Comparing `tmp/pulser_simulation-0.9.2-py3-none-any.whl.zip` & `tmp/pulser_simulation-0.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 26102 bytes, number of entries: 11
--rw-r--r--  2.0 unx      793 b- defN 23-Feb-16 16:52 pulser_simulation/__init__.py
--rw-r--r--  2.0 unx       22 b- defN 23-Feb-16 16:52 pulser_simulation/_version.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-16 16:52 pulser_simulation/py.typed
--rw-r--r--  2.0 unx     6845 b- defN 23-Feb-16 16:52 pulser_simulation/simconfig.py
--rw-r--r--  2.0 unx    24141 b- defN 23-Feb-16 16:52 pulser_simulation/simresults.py
--rw-r--r--  2.0 unx    39615 b- defN 23-Feb-16 16:52 pulser_simulation/simulation.py
--rw-r--r--  2.0 unx    11358 b- defN 23-Feb-16 16:52 pulser_simulation-0.9.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1192 b- defN 23-Feb-16 16:52 pulser_simulation-0.9.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-16 16:52 pulser_simulation-0.9.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Feb-16 16:52 pulser_simulation-0.9.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      951 b- defN 23-Feb-16 16:52 pulser_simulation-0.9.2.dist-info/RECORD
-11 files, 85027 bytes uncompressed, 24474 bytes compressed:  71.2%
+Zip file size: 26103 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      793 b- defN 23-Feb-24 14:04 pulser_simulation/__init__.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Feb-24 14:04 pulser_simulation/_version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-24 14:04 pulser_simulation/py.typed
+-rw-r--r--  2.0 unx     6845 b- defN 23-Feb-24 14:04 pulser_simulation/simconfig.py
+-rw-r--r--  2.0 unx    24141 b- defN 23-Feb-24 14:04 pulser_simulation/simresults.py
+-rw-r--r--  2.0 unx    39615 b- defN 23-Feb-24 14:04 pulser_simulation/simulation.py
+-rw-r--r--  2.0 unx    11358 b- defN 23-Feb-24 14:04 pulser_simulation-0.9.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1192 b- defN 23-Feb-24 14:04 pulser_simulation-0.9.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Feb-24 14:04 pulser_simulation-0.9.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Feb-24 14:04 pulser_simulation-0.9.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      951 b- defN 23-Feb-24 14:04 pulser_simulation-0.9.3.dist-info/RECORD
+11 files, 85027 bytes uncompressed, 24475 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: pulser_simulation/simresults.py
 Comment: 
 
 Filename: pulser_simulation/simulation.py
 Comment: 
 
-Filename: pulser_simulation-0.9.2.dist-info/LICENSE
+Filename: pulser_simulation-0.9.3.dist-info/LICENSE
 Comment: 
 
-Filename: pulser_simulation-0.9.2.dist-info/METADATA
+Filename: pulser_simulation-0.9.3.dist-info/METADATA
 Comment: 
 
-Filename: pulser_simulation-0.9.2.dist-info/WHEEL
+Filename: pulser_simulation-0.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: pulser_simulation-0.9.2.dist-info/top_level.txt
+Filename: pulser_simulation-0.9.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pulser_simulation-0.9.2.dist-info/RECORD
+Filename: pulser_simulation-0.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pulser_simulation/_version.py

```diff
@@ -1 +1 @@
-__version__ = '0.9.2'
+__version__ = '0.9.3'
```

## Comparing `pulser_simulation-0.9.2.dist-info/LICENSE` & `pulser_simulation-0.9.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pulser_simulation-0.9.2.dist-info/METADATA` & `pulser_simulation-0.9.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pulser-simulation
-Version: 0.9.2
+Version: 0.9.3
 Summary: An emulator of pulse-level sequences created with Pulser.
 Home-page: https://github.com/pasqal-io/Pulser
 Author: Pulser Development Team
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: qutip (>=4.7.1)
-Requires-Dist: pulser-core (==0.9.2)
+Requires-Dist: pulser-core (==0.9.3)
 Requires-Dist: typing-extensions ; python_version == "3.7"
 
 # pulser-simulation
 
 [Pulser](https://pypi.org/project/pulser/) is a framework for composing, simulating and executing **pulse** sequences for neutral-atom quantum devices.
 
 This is the `pulser-simulation` extension, which provides the functionalities needed to emulate `pulser` sequences.
```

## Comparing `pulser_simulation-0.9.2.dist-info/RECORD` & `pulser_simulation-0.9.3.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 pulser_simulation/__init__.py,sha256=kwq41SK6HTPJBT_OeZSWhA_-CPDqSSDw118jsY-aQfU,793
-pulser_simulation/_version.py,sha256=HSMl6bLm3r1Ias1jHIPpJeQ0IYNuuSdlT38MTb79ewM,22
+pulser_simulation/_version.py,sha256=83oJ8nCWXwQbno1uqIRolJfmli7BtUNqtuSvnzeSyxg,22
 pulser_simulation/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pulser_simulation/simconfig.py,sha256=w21JrnSzU56AGgBgvxCwXk5XWfGlWDnWSrHcL67A09g,6845
 pulser_simulation/simresults.py,sha256=iMWrjs-iD-asf010YaX21leIWYoPXvMnztftG84fd-o,24141
 pulser_simulation/simulation.py,sha256=Z0sNlGLTtRAI0x-zZhBwbNk1umA_i0yYWc5YcC9my1w,39615
-pulser_simulation-0.9.2.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-pulser_simulation-0.9.2.dist-info/METADATA,sha256=Ai-IY7pg38VHFrUx-hSAgN1GCLDqCu3n0IERIwWGmhM,1192
-pulser_simulation-0.9.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pulser_simulation-0.9.2.dist-info/top_level.txt,sha256=MHIiIdwiVT67DI6mJQCsj7XDwNJse1Oeugyu_9424No,18
-pulser_simulation-0.9.2.dist-info/RECORD,,
+pulser_simulation-0.9.3.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+pulser_simulation-0.9.3.dist-info/METADATA,sha256=nBv8fPGDmS-7rl-wqSUJmoMn0ZVGkHJt7gP-MLj2vdQ,1192
+pulser_simulation-0.9.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pulser_simulation-0.9.3.dist-info/top_level.txt,sha256=MHIiIdwiVT67DI6mJQCsj7XDwNJse1Oeugyu_9424No,18
+pulser_simulation-0.9.3.dist-info/RECORD,,
```

