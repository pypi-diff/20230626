# Comparing `tmp/dynapyt-0.3.0.tar.gz` & `tmp/dynapyt-0.3.1.tar.gz`

## Comparing `dynapyt-0.3.0.tar` & `dynapyt-0.3.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/__init__.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/run_all.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/run_analysis.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/run_instrumentation.py
--rw-r--r--   0        0        0    18071 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/runtime.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/BaseAnalysis.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/BranchCoverage.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/CallGraph.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/Demo.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/EventAnalysis.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/KeyInListAnalysis.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/LiteralAnalysis.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/MLMemoryAnalysis.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/ManipulateExec.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/MemoryAccessAnalysis.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/OnlyAddAnalysis.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/OperationAnalysis.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/SimpleTaintAnalysis.py
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/SimpleTestAnalysis.py
--rw-r--r--   0        0        0    34487 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/TraceAll.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/UnnecessaryDoubleDictQuery.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/__init__.py
--rw-r--r--   0        0        0    61731 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/instrument/CodeInstrumenter.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/instrument/IIDs.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/instrument/__init__.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/instrument/instrument.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/utils/AnalysisUtils.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/utils/__init__.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/utils/hierarchy.json
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/utils/hooks.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/utils/nodeLocator.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/nativetracer/__init__.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/nativetracer/instrument_tracer.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/nativetracer/trc.py
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 dynapyt-0.3.0/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 dynapyt-0.3.0/LICENSE
--rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 dynapyt-0.3.0/README.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 dynapyt-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6355 2020-02-02 00:00:00.000000 dynapyt-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/__init__.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/run_all.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/run_analysis.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/run_instrumentation.py
+-rw-r--r--   0        0        0    18071 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/runtime.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/analyses/BaseAnalysis.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/analyses/BranchCoverage.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/analyses/CallGraph.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/analyses/Demo.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/analyses/EventAnalysis.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/analyses/KeyInListAnalysis.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/analyses/LiteralAnalysis.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/analyses/MLMemoryAnalysis.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/analyses/ManipulateExec.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/analyses/MemoryAccessAnalysis.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/analyses/OnlyAddAnalysis.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/analyses/OperationAnalysis.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/analyses/SimpleTaintAnalysis.py
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/analyses/SimpleTestAnalysis.py
+-rw-r--r--   0        0        0    34487 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/analyses/TraceAll.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/analyses/UnnecessaryDoubleDictQuery.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/analyses/__init__.py
+-rw-r--r--   0        0        0    61731 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/instrument/CodeInstrumenter.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/instrument/IIDs.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/instrument/__init__.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/instrument/instrument.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/utils/AnalysisUtils.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/utils/__init__.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/utils/hierarchy.json
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/utils/hooks.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/dynapyt/utils/nodeLocator.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/nativetracer/__init__.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/nativetracer/instrument_tracer.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 dynapyt-0.3.1/src/nativetracer/trc.py
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 dynapyt-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 dynapyt-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 dynapyt-0.3.1/README.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 dynapyt-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6355 2020-02-02 00:00:00.000000 dynapyt-0.3.1/PKG-INFO
```

### Comparing `dynapyt-0.3.0/src/dynapyt/run_all.py` & `dynapyt-0.3.1/src/dynapyt/run_all.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/src/dynapyt/run_analysis.py` & `dynapyt-0.3.1/src/dynapyt/run_analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from os.path import abspath
 import sys
 import signal
 
 
 def run_analysis(entry: str, analysis: str, module: str = None, name: str = None):
     modulePath = "dynapyt.analyses"
-    if additional_module is not None:
-        modulePath = additional_module
+    if module is not None:
+        modulePath = module
     try:
         module = importlib.import_module(modulePath + "." + analysis)
     except TypeError as e:
         print(f"--module was used but no value specified {e}")
     except ImportError as e:
         print(f"module could not be imported {e}")
```

### Comparing `dynapyt-0.3.0/src/dynapyt/run_instrumentation.py` & `dynapyt-0.3.1/src/dynapyt/run_instrumentation.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/src/dynapyt/runtime.py` & `dynapyt-0.3.1/src/dynapyt/runtime.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/src/dynapyt/analyses/BaseAnalysis.py` & `dynapyt-0.3.1/src/dynapyt/analyses/BaseAnalysis.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/src/dynapyt/analyses/BranchCoverage.py` & `dynapyt-0.3.1/src/dynapyt/analyses/BranchCoverage.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/src/dynapyt/analyses/CallGraph.py` & `dynapyt-0.3.1/src/dynapyt/analyses/CallGraph.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/src/dynapyt/analyses/Demo.py` & `dynapyt-0.3.1/src/dynapyt/analyses/Demo.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/src/dynapyt/analyses/KeyInListAnalysis.py` & `dynapyt-0.3.1/src/dynapyt/analyses/KeyInListAnalysis.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/src/dynapyt/analyses/MLMemoryAnalysis.py` & `dynapyt-0.3.1/src/dynapyt/analyses/MLMemoryAnalysis.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/src/dynapyt/analyses/MemoryAccessAnalysis.py` & `dynapyt-0.3.1/src/dynapyt/analyses/MemoryAccessAnalysis.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/src/dynapyt/analyses/SimpleTaintAnalysis.py` & `dynapyt-0.3.1/src/dynapyt/analyses/SimpleTaintAnalysis.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/src/dynapyt/analyses/SimpleTestAnalysis.py` & `dynapyt-0.3.1/src/dynapyt/analyses/SimpleTestAnalysis.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/src/dynapyt/analyses/TraceAll.py` & `dynapyt-0.3.1/src/dynapyt/analyses/TraceAll.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/src/dynapyt/instrument/CodeInstrumenter.py` & `dynapyt-0.3.1/src/dynapyt/instrument/CodeInstrumenter.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/src/dynapyt/instrument/IIDs.py` & `dynapyt-0.3.1/src/dynapyt/instrument/IIDs.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/src/dynapyt/instrument/instrument.py` & `dynapyt-0.3.1/src/dynapyt/instrument/instrument.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/src/dynapyt/utils/AnalysisUtils.py` & `dynapyt-0.3.1/src/dynapyt/utils/AnalysisUtils.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/src/dynapyt/utils/hierarchy.json` & `dynapyt-0.3.1/src/dynapyt/utils/hierarchy.json`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/src/dynapyt/utils/hooks.py` & `dynapyt-0.3.1/src/dynapyt/utils/hooks.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/src/dynapyt/utils/nodeLocator.py` & `dynapyt-0.3.1/src/dynapyt/utils/nodeLocator.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/src/nativetracer/instrument_tracer.py` & `dynapyt-0.3.1/src/nativetracer/instrument_tracer.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/src/nativetracer/trc.py` & `dynapyt-0.3.1/src/nativetracer/trc.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/.gitignore` & `dynapyt-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/LICENSE` & `dynapyt-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/README.md` & `dynapyt-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/pyproject.toml` & `dynapyt-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dynapyt-0.3.0/PKG-INFO` & `dynapyt-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynapyt
-Version: 0.3.0
+Version: 0.3.1
 Summary: Dynamic analysis framework for Python
 Project-URL: Bug Tracker, https://github.com/sola-st/DynaPyt/issues
 Project-URL: Homepage, https://github.com/sola-st/DynaPyt
 Author-email: Aryaz Eghbali <aryaz.egh@gmail.com>, Michael Pradel <michael@binaervarianz.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

