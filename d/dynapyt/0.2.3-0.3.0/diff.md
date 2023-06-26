# Comparing `tmp/dynapyt-0.2.3.tar.gz` & `tmp/dynapyt-0.3.0.tar.gz`

## Comparing `dynapyt-0.2.3.tar` & `dynapyt-0.3.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/__init__.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/run_all.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/run_analysis.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/run_instrumentation.py
--rw-r--r--   0        0        0    17428 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/runtime.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/BaseAnalysis.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/BranchCoverage.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/CallGraph.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/Demo.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/EventAnalysis.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/KeyInListAnalysis.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/LiteralAnalysis.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/MLMemoryAnalysis.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/ManipulateExec.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/MemoryAccessAnalysis.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/OnlyAddAnalysis.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/OperationAnalysis.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/SimpleTaintAnalysis.py
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/SimpleTestAnalysis.py
--rw-r--r--   0        0        0    32544 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/TraceAll.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/UnnecessaryDoubleDictQuery.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/analyses/__init__.py
--rw-r--r--   0        0        0    47883 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/instrument/CodeInstrumenter.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/instrument/IIDs.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/instrument/__init__.py
--rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/instrument/instrument.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/utils/AnalysisUtils.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/utils/__init__.py
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/utils/hierarchy.json
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/utils/hooks.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/dynapyt/utils/nodeLocator.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/nativetracer/__init__.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/nativetracer/instrument_tracer.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 dynapyt-0.2.3/src/nativetracer/trc.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 dynapyt-0.2.3/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 dynapyt-0.2.3/LICENSE
--rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 dynapyt-0.2.3/README.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 dynapyt-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     6231 2020-02-02 00:00:00.000000 dynapyt-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/__init__.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/run_all.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/run_analysis.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/run_instrumentation.py
+-rw-r--r--   0        0        0    18071 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/runtime.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/BaseAnalysis.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/BranchCoverage.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/CallGraph.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/Demo.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/EventAnalysis.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/KeyInListAnalysis.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/LiteralAnalysis.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/MLMemoryAnalysis.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/ManipulateExec.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/MemoryAccessAnalysis.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/OnlyAddAnalysis.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/OperationAnalysis.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/SimpleTaintAnalysis.py
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/SimpleTestAnalysis.py
+-rw-r--r--   0        0        0    34487 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/TraceAll.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/UnnecessaryDoubleDictQuery.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/analyses/__init__.py
+-rw-r--r--   0        0        0    61731 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/instrument/CodeInstrumenter.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/instrument/IIDs.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/instrument/__init__.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/instrument/instrument.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/utils/AnalysisUtils.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/utils/__init__.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/utils/hierarchy.json
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/utils/hooks.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/dynapyt/utils/nodeLocator.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/nativetracer/__init__.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/nativetracer/instrument_tracer.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 dynapyt-0.3.0/src/nativetracer/trc.py
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 dynapyt-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 dynapyt-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 dynapyt-0.3.0/README.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 dynapyt-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6355 2020-02-02 00:00:00.000000 dynapyt-0.3.0/PKG-INFO
```

### Comparing `dynapyt-0.2.3/src/dynapyt/run_all.py` & `dynapyt-0.3.0/src/dynapyt/run_all.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.3/src/dynapyt/run_analysis.py` & `dynapyt-0.3.0/src/dynapyt/run_analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 import argparse
 import importlib
 from os.path import abspath
 import sys
 import signal
 
-parser = argparse.ArgumentParser()
-parser.add_argument(
-    "--entry", help="Entry file for execution")
-parser.add_argument(
-    "--analysis", help="Analysis class name")
-parser.add_argument(
-    "--module", help="Adds external module paths")
-parser.add_argument(
-    "--name", help="Associates a given name with current run"
-)
-
-import dynapyt.runtime as rt
 
-if __name__ == '__main__':
-    args = parser.parse_args()
-    additional_module = args.module
-    name = args.name
-    analysis = args.analysis
-    modulePath = 'dynapyt.analyses'
+def run_analysis(entry: str, analysis: str, module: str = None, name: str = None):
+    modulePath = "dynapyt.analyses"
     if additional_module is not None:
         modulePath = additional_module
     try:
-        module = importlib.import_module(modulePath + '.' + analysis)
+        module = importlib.import_module(modulePath + "." + analysis)
     except TypeError as e:
-        print(f'--module was used but no value specified {e}')
+        print(f"--module was used but no value specified {e}")
     except ImportError as e:
-        print(f'module could not be imported {e}')
+        print(f"module could not be imported {e}")
 
-    class_ = getattr(module, args.analysis)
+    class_ = getattr(module, analysis)
     my_analysis = class_()
     rt.set_analysis(my_analysis)
 
     def end_execution():
         try:
-            func = getattr(my_analysis, 'end_execution')
+            func = getattr(my_analysis, "end_execution")
             func()
         except AttributeError:
             pass
 
     # allow dynapyt to exit gracefully
     # Note: this will almost certainly not work on Windows
     signal.signal(signal.SIGINT, end_execution)
     signal.signal(signal.SIGTERM, end_execution)
 
     if not name is None:
-        getattr(my_analysis, 'add_metadata', lambda: None)({"name": name})
+        getattr(my_analysis, "add_metadata", lambda: None)({"name": name})
 
     try:
-        func = getattr(my_analysis, 'begin_execution')
+        func = getattr(my_analysis, "begin_execution")
         func()
     except AttributeError:
         pass
-    if args.entry.endswith('.py'):
-        sys.argv = [args.entry]
-        exec(open(abspath(args.entry)).read())
+    if entry.endswith(".py"):
+        sys.argv = [entry]
+        exec(open(abspath(entry)).read())
     else:
-        importlib.import_module(args.entry, '*')
-    end_execution()
+        importlib.import_module(entry, "*")
+    end_execution()
+
+
+parser = argparse.ArgumentParser()
+parser.add_argument("--entry", help="Entry file for execution")
+parser.add_argument("--analysis", help="Analysis class name")
+parser.add_argument("--module", help="Adds external module paths")
+parser.add_argument("--name", help="Associates a given name with current run")
+
+import dynapyt.runtime as rt
+
+if __name__ == "__main__":
+    args = parser.parse_args()
+    additional_module = args.module
+    name = args.name
+    analysis = args.analysis
+    run_analysis(args.entry, analysis, additional_module, name)
```

### Comparing `dynapyt-0.2.3/src/dynapyt/runtime.py` & `dynapyt-0.3.0/src/dynapyt/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -450,18 +450,31 @@
     value = var_arg()
     call_if_exists("memory_access", dyn_ast, iid, value)
     call_if_exists("read", dyn_ast, iid, value)
     result = call_if_exists("read_identifier", dyn_ast, iid, value)
     return result if result != None else value
 
 
-def _if_(dyn_ast, iid, val):
+def _if_expr_(dyn_ast, iid, condition, true_val, false_val):
     call_if_exists("runtime_event", dyn_ast, iid)
-    result = call_if_exists("_if", dyn_ast, iid, val)
-    return result if result != None else val
+    result_high = call_if_exists("enter_control_flow", dyn_ast, iid, condition)
+    result_low = call_if_exists("enter_if", dyn_ast, iid, condition)
+    final_condition = condition
+    if result_low is not None:
+        final_condition = result_low
+    elif result_high is not None:
+        final_condition = result_high
+    if final_condition:
+        res = true_val()
+    else:
+        res = false_val()
+    call_if_exists("runtime_event", dyn_ast, iid)
+    call_if_exists("exit_control_flow", dyn_ast, iid)
+    call_if_exists("exit_if", dyn_ast, iid)
+    return res
 
 
 def _func_entry_(dyn_ast, iid, args, name: str, is_lambda=False):
     call_if_exists("runtime_event", dyn_ast, iid)
     call_if_exists("function_enter", dyn_ast, iid, args, name, is_lambda)
 
 
@@ -473,29 +486,31 @@
 
 def _return_(dyn_ast, iid, function_iid, function_name, return_val=None):
     call_if_exists("runtime_event", dyn_ast, iid)
     result_high = call_if_exists(
         "function_exit", dyn_ast, function_iid, function_name, return_val
     )
     result_low = call_if_exists(
-        "_return", dyn_ast, iid, function_iid, return_val
+        "_return", dyn_ast, iid, function_iid, function_name, return_val
     )  # return needs both its own iid and the function iid
     if result_low != None:
         return result_low
     elif result_high != None:
         return result_high
     return return_val
 
 
 def _yield_(dyn_ast, iid, function_iid, function_name, return_val=None):
     call_if_exists("runtime_event", dyn_ast, iid)
     result_high = call_if_exists(
         "function_exit", dyn_ast, function_iid, function_name, return_val
     )
-    result_low = call_if_exists("_yield", dyn_ast, iid, function_iid, return_val)
+    result_low = call_if_exists(
+        "_yield", dyn_ast, iid, function_iid, function_name, return_val
+    )
     if result_low != None:
         return result_low
     elif result_high != None:
         return result_high
     return return_val
 
 
@@ -523,19 +538,20 @@
     return result if result != None else True
 
 
 def _enter_if_(dyn_ast, iid, condition):
     call_if_exists("runtime_event", dyn_ast, iid)
     result_high = call_if_exists("enter_control_flow", dyn_ast, iid, condition)
     result_low = call_if_exists("enter_if", dyn_ast, iid, condition)
+    final_condition = condition
     if result_low is not None:
-        return result_low
+        final_condition = result_low
     elif result_high is not None:
-        return result_high
-    return condition
+        final_condition = result_high
+    return final_condition
 
 
 def _exit_if_(dyn_ast, iid):
     call_if_exists("runtime_event", dyn_ast, iid)
     call_if_exists("exit_control_flow", dyn_ast, iid)
     call_if_exists("exit_if", dyn_ast, iid)
 
@@ -589,8 +605,9 @@
             result = _enter_for_(dyn_ast, iid, it, iterator)
             if result is not None:
                 yield result
             else:
                 yield it
         except StopIteration as e:
             _enter_for_(dyn_ast, iid, e, iterator)
+            _exit_for_(dyn_ast, iid)
             return
```

### Comparing `dynapyt-0.2.3/src/dynapyt/analyses/BaseAnalysis.py` & `dynapyt-0.3.0/src/dynapyt/analyses/BaseAnalysis.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.3/src/dynapyt/analyses/BranchCoverage.py` & `dynapyt-0.3.0/src/dynapyt/analyses/BranchCoverage.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.3/src/dynapyt/analyses/CallGraph.py` & `dynapyt-0.3.0/src/dynapyt/analyses/CallGraph.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.3/src/dynapyt/analyses/Demo.py` & `dynapyt-0.3.0/src/dynapyt/analyses/Demo.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.3/src/dynapyt/analyses/KeyInListAnalysis.py` & `dynapyt-0.3.0/src/dynapyt/analyses/KeyInListAnalysis.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.3/src/dynapyt/analyses/MLMemoryAnalysis.py` & `dynapyt-0.3.0/src/dynapyt/analyses/MLMemoryAnalysis.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.3/src/dynapyt/analyses/MemoryAccessAnalysis.py` & `dynapyt-0.3.0/src/dynapyt/analyses/MemoryAccessAnalysis.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.3/src/dynapyt/analyses/SimpleTaintAnalysis.py` & `dynapyt-0.3.0/src/dynapyt/analyses/SimpleTaintAnalysis.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.3/src/dynapyt/analyses/SimpleTestAnalysis.py` & `dynapyt-0.3.0/src/dynapyt/analyses/SimpleTestAnalysis.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.3/src/dynapyt/analyses/TraceAll.py` & `dynapyt-0.3.0/src/dynapyt/analyses/TraceAll.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 import libcst as cst
 import libcst.matchers as m
 from .BaseAnalysis import BaseAnalysis
 from ..utils.nodeLocator import get_node_by_location
 
 
 class TraceAll(BaseAnalysis):
+    """
+    .. include:: ../../../docs/hooks.md
+    """
+
     def __init__(self) -> None:
         super().__init__()
         root_logger = logging.getLogger()
         root_logger.setLevel(logging.INFO)
         handler = logging.FileHandler("output.log", "w", "utf-8")
         handler.setFormatter(logging.Formatter("%(message)s"))
         root_logger.addHandler(handler)
@@ -30,35 +34,40 @@
     def integer(self, dyn_ast: str, iid: int, val: Any) -> Any:
         """Hook for integer literals.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         val : Any
             The value of the integer literal.
 
         Returns
         -------
         Any
+
             If provided, overwrites the value of the integer literal.
         """
         self.log(iid, "    Integer", "value:", val)
 
     def _float(self, dyn_ast: str, iid: int, val: Any) -> Any:
         """Hook for floating point literals.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         val : Any
             The value of the floating point literal.
 
         Returns
         -------
         Any
             If provided, overwrites the value of the float literal.
@@ -68,35 +77,40 @@
     def imaginary(self, dyn_ast: str, iid: int, val: Any) -> Any:
         """Hook for imaginary number literals.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         val : Any
             The value of the imaginary number literal.
 
+
         Returns
         -------
         Any
             If provided, overwrites the value of the imaginary number literal.
         """
         self.log(iid, "    Imaginary", "value:", val)
 
     def string(self, dyn_ast: str, iid: int, val: Any) -> Any:
         """Hook for string literals.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         val : Any
             The value of the string literal.
 
         Returns
         -------
         Any
             If provided, overwrites the value of the string literal.
@@ -106,163 +120,204 @@
     def boolean(self, dyn_ast: str, iid: int, val: Any) -> Any:
         """Hook for boolean literals.
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         val : Any
             The value of the boolean literal.
 
+
         Returns
         -------
         Any
             If provided, overwrites the value of the boolean literal.
+
         """
         self.log(iid, "    Boolean", "value:", val)
 
     def literal(self, dyn_ast: str, iid: int, val: Any) -> Any:
         """Hook for all literals.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         val : Any
             The value of the literal.
 
+
         Returns
         -------
         Any
             If provided, overwrites the value of the literal.
+
         """
         self.log(iid, "Literal   ", "value:", val)
 
     def dictionary(self, dyn_ast: str, iid: int, items: List[Any], value: Dict) -> Dict:
         """Hook for a dictionary definition.
+
         E.g. `{'a': 1, 'b': 2}`
         or `{i: i for i in range(10)}`
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         items : List[Any]
             The lis of key-value pairs.
+
         value : Dict
             The dictionary itself.
 
+
         Returns
         -------
         Dict
             If provided, overwrites the value of the dictionary.
+
         """
         self.log(iid, "Dictionary", "items:", items)
 
     def _list(self, dyn_ast: str, iid: int, value: List) -> List:
         """Hook for a list definition.
+
         E.g. `[1, 2, 3]`
         or `[i for i in range(10)]`
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         value : List
             The list itself.
 
+
         Returns
         -------
         List
             If provided, overwrites the value of the list.
+
         """
         self.log(iid, "List", value)
 
     def _tuple(self, dyn_ast: str, iid: int, items: List[Any], value: tuple) -> tuple:
         """Hook for a tuple.
+
         E.g. `(1, 2, 3)`
         or `(i for i in range(10))`
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         items : List[Any]
             The lis of items in the tuple.
+
         value : tuple
             The tuple itself.
 
+
         Returns
         -------
         tuple
             If provided, overwrites the value of the tuple.
+
         """
         self.log(iid, "Tuple", "items:", items)
 
     # Operations
 
     def operation(
         self, dyn_ast: str, iid: int, operator: str, operands: List[Any], result: Any
     ) -> Any:
         """Hook for any operation.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         operator : str
             The operator of the operation.
+
         operands : List[Any]
             The operands of the operation.
+
         result : Any
             The result of the operation.
 
+
         Returns
         -------
         Any
             If provided, overwrites the result of the operation.
+
         """
         pass
 
     def binary_operation(
         self, dyn_ast: str, iid: int, op: str, left: Any, right: Any, result: Any
     ) -> Any:
         """Hook for any binary operation.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         op : str
             The operator of the operation.
+
         left : Any
             The left operand of the operation.
+
         right : Any
             The right operand of the operation.
+
         result : Any
             The result of the operation.
 
+
         Returns
         -------
         Any
             If provided, overwrites the result of the operation.
+
         """
         self.log(iid, "Binary Operation", left, op, right, "->", result)
 
     def add(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
         self.log(iid, "Binary Operation", left, right, "->", result)
 
     def bit_and(
@@ -324,31 +379,38 @@
         self.log(iid, "Binary Operation", left, right, "->", result)
 
     def unary_operation(
         self, dyn_ast: str, iid: int, opr: Any, arg: Any, result: Any
     ) -> Any:
         """Hook for any unary operation.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         opr : str
             The operator of the operation.
+
         arg : Any
             The operand of the operation.
+
         result : Any
             The result of the operation.
 
+
         Returns
         -------
         Any
             If provided, overwrites the result of the operation.
+
         """
         self.log(iid, "Unary Operation", arg, "->", result)
 
     def bit_invert(self, dyn_ast: str, iid: int, arg: Any, result: Any) -> Any:
         self.log(iid, "Unary Operation", arg, "->", result)
 
     def minus(self, dyn_ast: str, iid: int, arg: Any, result: Any) -> Any:
@@ -361,33 +423,41 @@
         self.log(iid, "Unary Operation", arg, "->", result)
 
     def comparison(
         self, dyn_ast: str, iid: int, op: str, left: Any, right: Any, result: Any
     ) -> Any:
         """Hook for the comparison operation.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         op : str
             The operator of the operation.
+
         left : Any
             The left operand of the operation.
+
         right : Any
             The right operand of the operation.
+
         result : Any
             The result of the operation.
 
+
         Returns
         -------
         Any
             If provided, overwrites the result of the operation.
+
         """
         self.log(iid, "Comparison", left, op, right, "->", result)
 
     def equal(self, dyn_ast: str, iid: int, left: Any, right: Any, result: Any) -> Any:
         self.log(iid, "Comparison", left, right, "->", result)
 
     def greater_than(
@@ -428,152 +498,188 @@
         self.log(iid, "Comparison", left, right, "->", result)
 
     # Memory access
 
     def memory_access(self, dyn_ast: str, iid: int, val: Any) -> Any:
         """Hook for any memory access, currently, except some write operations.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         val : Any
             The value accessed.
 
+
         Returns
         -------
         Any
             If provided, overwrites the returned value.
+
         """
         self.log(iid, "Accessing")
 
     def read(self, dyn_ast: str, iid: int, val: Any) -> Any:
         self.log(iid, " Reading")
 
     def read_identifier(self, dyn_ast: str, iid: int, val: Any) -> Any:
         self.log(iid, "    Reading")
 
     def write(
         self, dyn_ast: str, iid: int, old_vals: List[Callable], new_val: Any
     ) -> Any:
         """Hook for writes.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         old_vals : Any
             A list of old values before the write takes effect.
             It's a list to support multiple assignments.
             Each old value is wrapped into a lambda function, so that
             the analysis writer can decide if and when to evaluate it.
+
         new_val : Any
             The value after the write takes effect.
 
+
         Returns
         -------
         Any
             If provided, overwrites the returned value.
+
         """
         self.log(iid, "    Writing")
 
     def delete(self, dyn_ast: str, iid: int, val: Any) -> Optional[bool]:
         """Hook for deletes.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         val : Any
             The value deleted.
 
+
         Returns
         -------
         Any
             If True cancels the delete.
+
         """
         self.log(iid, "    Deleting")
 
     def read_attribute(
         self, dyn_ast: str, iid: int, base: Any, name: str, val: Any
     ) -> Any:
         """Hook for reading an object attribute.
+
         E.g. `obj.attr`
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         base : Any
             The object to which the attribute is attached.
+
         name : str
             The name of the attribute.
+
         val : Any
             The resulting value.
 
+
         Returns
         -------
         Any
             If provided, overwrites the returned value.
+
         """
         self.log(iid, "Attribute", name)
 
     def read_subscript(
         self, dyn_ast: str, iid: int, base: Any, sl: List[Union[int, Tuple]], val: Any
     ) -> Any:
         """Hook for reading a subscript, also known as a slice.
+
         E.g. `obj[1, 2]`
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         base : Any
             The object to which the subscript is attached.
+
         sl : List[Union[int, Tuple]]
             The subscript.
+
         val : Any
             The resulting value.
 
+
         Returns
         -------
         Any
             If provided, overwrites the returned value.
+
         """
         self.log(iid, "Slice", sl)
 
     # Instrumented function
 
     def function_enter(
-        self, dyn_ast: str, iid: int, name: str, args: List[Any], is_lambda: bool
+        self, dyn_ast: str, iid: int, args: List[Any], name: str, is_lambda: bool
     ) -> None:
         """Hook for when an instrumented function is entered.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         args : List[Any]
             The arguments passed to the function.
+
         name:
-            Name of the function called
+            Name of the function called.
+
         is_lambda : bool
             Whether the function is a lambda function.
+
         """
         tmp = self._get_ast(dyn_ast)
         if tmp is not None:
             ast, iids = tmp
         else:
             return
         if (not is_lambda) and (
@@ -583,146 +689,194 @@
             self.log(iid, "Entered function", danger_of_recursion=True)
 
     def function_exit(
         self, dyn_ast: str, function_iid: int, name: str, result: Any
     ) -> Any:
         """Hook for exiting an instrumented function.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         function_iid: int
-            ID unique to the current file, referring to the function
+            ID unique to the current file, referring to the function.
+
         name: str
-            Name of the function called
+            Name of the function called.
+
         result : Any
             The result of the function.
 
+
         Returns
         -------
         Any
             If provided, overwrites the returned value.
+
         """
         self.log(function_iid, "Exiting function")
 
-    def _return(self, dyn_ast: str, iid: int, function_iid: int, value: Any) -> Any:
+    def _return(
+        self, dyn_ast: str, iid: int, function_iid: int, function_name: str, value: Any
+    ) -> Any:
         """Hook for instrumented return statement.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid: int
-            ID unique to the current file, referring to the return statement
+            ID unique to the current file, referring to the return statement.
+
         function_iid: int
-            ID unique to the current file, referring to the function
+            ID unique to the current file, referring to the function.
+
+        function_name: str
+            Name of the function returning from.
+
         value : Any
             The value returned.
+
         """
         self.log(iid, "   Returning", value)
 
-    def _yield(self, dyn_ast: str, iid: int, function_iid: int, value: Any) -> Any:
+    def _yield(
+        self, dyn_ast: str, iid: int, function_iid: int, function_name: str, value: Any
+    ) -> Any:
         """Hook for instrumented yield statement.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid: int
-            ID unique to the current file, referring to the yield statement
+            ID unique to the current file, referring to the yield statement.
+
         function_iid: int
-            ID unique to the current file, referring to the function
+            ID unique to the current file, referring to the function.
+
+        function_name: str
+            Name of the function yielding from.
+
         value : Any
             The value yielded.
+
         """
         self.log(iid, "   Yielding", value)
 
     # Function Call
 
     def pre_call(
         self, dyn_ast: str, iid: int, function: Callable, pos_args: Tuple, kw_args: Dict
     ):
         """Hook called before a function call happens.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         function : str
-            Function which will be called
+            Function which will be called.
+
         pos_args : Tuple
             The positional arguments passed to the function.
+
         kw_args : Dict
             The keyword arguments passed to the function.
+
         """
         self.log(iid, "Before function call")
 
     def post_call(
         self,
         dyn_ast: str,
         iid: int,
         result: Any,
         call: Callable,
         pos_args: Tuple,
         kw_args: Dict,
     ) -> Any:
         """Hook called after a function call.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         val : Any
             The return value of the function.
+
         call: Callable
-            The function which was called
+            The function which was called.
+
         pos_args : Tuple
             The positional arguments passed to the function.
+
         kw_args : Dict
             The keyword arguments passed to the function.
 
+
         Returns
         -------
         Any
             If provided, overwrites the returned value.
+
         """
         self.log(iid, "After function call")
 
     # Statements
 
     def augmented_assignment(
         self, dyn_ast: str, iid: int, left: Any, op: str, right: Any
     ) -> Any:
         """Hook for any augmented assignment.
+
         E.g. `a += 1`
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         left : Any
             The left operand.
+
         op : str
             The operator.
+
         right : Any
             The right operand.
+
         val : Any
             The resulting value.
 
+
         Returns
         -------
         Any
             If provided, overwrites the result.
+
         """
         self.log(iid, "Augmented assignment", left, op, right)
 
     def add_assign(self, dyn_ast: str, iid: int, left: Any, right: Any) -> Any:
         self.log(iid, "Augmented assignment", left, right)
 
     def bit_and_assign(self, dyn_ast: str, iid: int, left: Any, right: Any) -> Any:
@@ -764,259 +918,381 @@
         self.log(iid, "Augmented assignment", left, right)
 
     def _raise(
         self, dyn_ast: str, iid: int, exc: Exception, cause: Any
     ) -> Optional[Exception]:
         """Hook for instrumented raise statement.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         exc : Exception
             The exception raised.
+
         cause : Any
             The cause of the exception.
 
+
         Returns
         -------
         Exception
             If provided, changes the exception raised.
+
         """
         self.log(iid, "Exception raised", exc, "because of", cause)
 
     def _assert(
         self, dyn_ast: str, iid: int, condition: bool, message: str
     ) -> Optional[bool]:
         """Hook for assert statement.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         condition : bool
             The condition to assert.
+
         message : str
             The message to display if the condition is false.
 
+
         Returns
         -------
         bool
             If provided, changes the condition of assert.
+
         """
         self.log(iid, "Asserting", condition, "with message", message)
 
     # Control flow
 
+    def control_flow_event(self, dyn_ast: str, iid: int) -> None:
+        """Hook called when a control flow event happens.
+
+        Parameters
+        ----------
+        dyn_ast : str
+            The path to the original code. Can be used to extract the syntax tree.
+
+        iid : int
+            Unique ID of the syntax tree node.
+        """
+        self.log(iid, "Control flow event")
+
     def enter_control_flow(
         self, dyn_ast: str, iid: int, cond_value: bool
     ) -> Optional[bool]:
         """Hook called when entering a control flow branch.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         cond_value : bool
             The value of the condition.
 
+
         Returns
         -------
         bool
             If provided, changes the condition of the control flow.
+
         """
         self.log(iid, "Control-flow enter", "with condition", cond_value)
 
     def exit_control_flow(self, dyn_ast: str, iid: int) -> None:
         """Hook called when exiting a control flow branch.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         """
         self.log(iid, "Control-flow exit")
 
     def enter_if(self, dyn_ast: str, iid: int, cond_value: bool) -> Optional[bool]:
-        """Hook called when entering an if conditional.
+        """Hook called when entering if.
+
 
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         cond_value : bool
             Whether the condition is true or false.
 
+
         Returns
         -------
         Optional[bool]
             If provided, overwrites the condition (which may change the branch outcome).
+
         """
         self.log(iid, "   If", cond_value)
 
+    def exit_if(self, dyn_ast, iid):
+        """Hook for exiting if.
+
+
+        Parameters
+        ----------
+        dyn_ast : str
+            The path to the original code. Can be used to extract the syntax tree.
+
+        iid : int
+            Unique ID of the syntax tree node.
+
+
+        """
+        self.log(iid, "If exit")
+
     def enter_for(
         self, dyn_ast: str, iid: int, next_value: Any, iterable: Iterable
     ) -> Optional[Any]:
         """Hook for entering a single iteration of a for loop.
 
+
         In most cases it should be ensured that the provided iterable is not consumed
         as the instrumented program will use it later on in the actual for loop.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         next_value : Any
             The next value of the iterator.
+
         iterable: Iterable
             Iterable used in the for loop.
 
+
         Returns
         -------
         Any
             If provided, overwrites the value of the iterator.
+
         """
         self.log(iid, "   For", next_value)
 
     def exit_for(self, dyn_ast, iid):
         """Hook for exiting a for loop.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
 
+
         """
         self.log(iid, "For exit")
 
     def enter_while(self, dyn_ast: str, iid: int, cond_value: bool) -> Optional[bool]:
         """Hook for entering the next iteration of a while loop.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         cond_value : bool
             The value of the condition (which may change the branch outcome).
 
+
         Returns
         -------
         bool
             If provided, overwrites the condition.
+
         """
         self.log(iid, "   While", cond_value)
 
+    def exit_while(self, dyn_ast, iid):
+        """Hook for exiting a while loop.
+
+
+        Parameters
+        ----------
+        dyn_ast : str
+            The path to the original code. Can be used to extract the syntax tree.
+
+        iid : int
+            Unique ID of the syntax tree node.
+
+
+        """
+        self.log(iid, "While exit")
+
     def _break(self, dyn_ast: str, iid: int) -> Optional[bool]:
         """Hook for break statement.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
 
+
         Returns
         -------
         bool
             If False, cancels the break.
+
         """
         self.log(iid, "Break")
 
     def _continue(self, dyn_ast: str, iid: int) -> Optional[bool]:
         """Hook for continue statement.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
 
+
         Returns
         -------
         bool
             If False, cancels continue.
+
         """
         self.log(iid, "Continue")
 
-    def _try(self, dyn_ast: str, iid: int) -> None:
+    def enter_try(self, dyn_ast: str, iid: int) -> None:
         """Hook for entering a try block.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         """
         self.log(iid, "Entered try")
 
+    def clean_exit_try(self, dyn_ast: str, iid: int) -> None:
+        """Hook for exiting a try block without an exception being raised.
+
+
+        Parameters
+        ----------
+        dyn_ast : str
+            The path to the original code. Can be used to extract the syntax tree.
+
+        iid: int
+            Unique ID of the syntax tree node.
+        """
+        self.log(iid, "Clean exit try")
+
     def exception(
         self, dyn_ast: str, iid: int, exceptions: List[Exception], caught: Exception
     ) -> Optional[Exception]:
         """Hook for entering an except block.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         exceptions : List[Exception]
             The exceptions to catch.
+
         caught : Exception
             The exception caught.
 
+
         Returns
         -------
         Exception
             If provided, overwrites the exception caught.
+
         """
         self.log(iid, "Caught", caught, "from", exceptions)
 
     # Top level
 
     def runtime_event(self, dyn_ast: str, iid: int) -> None:
         """Hook for any runtime event.
 
+
         Parameters
         ----------
         dyn_ast : str
             The path to the original code. Can be used to extract the syntax tree.
+
         iid : int
             Unique ID of the syntax tree node.
+
         """
         pass
 
     def uncaught_exception(self, exc: Exception, stack_trace: TracebackType) -> None:
         """Hook for any uncaught exceptions.
 
+
         Parameters
         ----------
         exc : Exception
             The exception raised.
+
         stack_trace : TracebackType
             The stack trace of the exception.
+
         """
         self.log(-1, "Uncaught exception", exc, stack_trace)
 
     def begin_execution(self) -> None:
         """Hook for the start of execution."""
         self.log(-1, "Execution started")
```

### Comparing `dynapyt-0.2.3/src/dynapyt/instrument/IIDs.py` & `dynapyt-0.3.0/src/dynapyt/instrument/IIDs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,55 @@
 from collections import namedtuple
 from os import path
 import json
 
 
-Location = namedtuple("Location", ["file", "start_line", "start_column", "end_line", "end_column"])
+Location = namedtuple(
+    "Location", ["file", "start_line", "start_column", "end_line", "end_column"]
+)
 
 
 class IIDs:
     def __init__(self, file_path):
-        if file_path.endswith('.py.orig'):
-            file_path = file_path[:-8] + '-dynapyt.json'
+        if file_path.endswith(".py.orig"):
+            file_path = file_path[:-8] + "-dynapyt.json"
         else:
-            file_path = file_path[:-3] + '-dynapyt.json'
+            file_path = file_path[:-3] + "-dynapyt.json"
         if not path.exists(file_path):
-            with open(file_path, 'w') as f:
-                json.dump({'next_iid': 0, 'iid_to_location': {}}, f)
+            with open(file_path, "w") as f:
+                json.dump({"next_iid": 0, "iid_to_location": {}}, f)
             self.next_iid = 0
             self.iid_to_location = {}
             self.location_to_iid = {}
         else:
-            with open(file_path, 'r') as file:
+            with open(file_path, "r") as file:
                 json_object = json.load(file)
-            self.next_iid = json_object['next_iid']
-            self.iid_to_location = {int(k): v for k, v in json_object['iid_to_location'].items()}
-            self.location_to_iid = {Location(*v): k for k, v in self.iid_to_location.items()}
+            self.next_iid = json_object["next_iid"]
+            self.iid_to_location = {
+                int(k): Location(**v) for k, v in json_object["iid_to_location"].items()
+            }
+            self.location_to_iid = {
+                Location(*v): k for k, v in self.iid_to_location.items()
+            }
         self.file_path = file_path
 
     def new(self, file, start_line, start_column, end_line, end_column):
         this_location = Location(file, start_line, start_column, end_line, end_column)
         if this_location in self.location_to_iid:
             return self.location_to_iid[this_location]
         self.iid_to_location[self.next_iid] = this_location
         self.next_iid += 1
         return self.next_iid - 1
 
     def store(self):
         all_data = {
             "next_iid": self.next_iid,
-            "iid_to_location": self.iid_to_location,
+            "iid_to_location": dict(
+                map(
+                    lambda item: (item[0], item[1]._asdict()),
+                    self.iid_to_location.items(),
+                )
+            ),
         }
         json_object = json.dumps(all_data, indent=2)
         with open(self.file_path, "w") as file:
-            file.write(json_object)
+            file.write(json_object)
```

### Comparing `dynapyt-0.2.3/src/dynapyt/instrument/instrument.py` & `dynapyt-0.3.0/src/dynapyt/instrument/instrument.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,87 +8,94 @@
 from .IIDs import IIDs
 import re
 from shutil import copyfile
 from dynapyt.utils.hooks import get_hooks_from_analysis
 
 parser = argparse.ArgumentParser()
 parser.add_argument(
-    "--files", help="Python files to instrument or .txt file with all file paths", nargs="+")
-parser.add_argument(
-    "--analysis", help="Analysis class name")
-parser.add_argument(
-    "--module", help="Adds external module paths")
+    "--files",
+    help="Python files to instrument or .txt file with all file paths",
+    nargs="+",
+)
+parser.add_argument("--analysis", help="Analysis class name")
+parser.add_argument("--module", help="Adds external module paths")
+
 
 def gather_files(files_arg):
-    if len(files_arg) == 1 and files_arg[0].endswith('.txt'):
+    if len(files_arg) == 1 and files_arg[0].endswith(".txt"):
         files = []
         with open(files_arg[0]) as fp:
             for line in fp.readlines():
                 files.append(line.rstrip())
     else:
         for f in files_arg:
-            if not f.endswith('.py'):
-                raise Exception(f'Incorrect argument, expected .py file: {f}')
+            if not f.endswith(".py"):
+                raise Exception(f"Incorrect argument, expected .py file: {f}")
         files = files_arg
     return files
 
 
 def instrument_code(src, file_path, iids, selected_hooks):
-    if 'DYNAPYT: DO NOT INSTRUMENT' in src:
-        print(f'{file_path} is already instrumented -- skipping it')
+    if "DYNAPYT: DO NOT INSTRUMENT" in src:
+        print(f"{file_path} is already instrumented -- skipping it")
         return None
 
     try:
         ast = cst.parse_module(src)
         ast_wrapper = cst.metadata.MetadataWrapper(ast)
 
         instrumented_code = CodeInstrumenter(src, file_path, iids, selected_hooks)
         instrumented_ast = ast_wrapper.visit(instrumented_code)
 
-        return '# DYNAPYT: DO NOT INSTRUMENT\n\n' + instrumented_ast.code
+        return "# DYNAPYT: DO NOT INSTRUMENT\n\n" + instrumented_ast.code
     except ParserSyntaxError:
-        print(f'Syntax error in {file_path} -- skipping it')
+        print(f"Syntax error in {file_path} -- skipping it")
         return None
 
+
 def instrument_file(file_path, selected_hooks):
-    with open(file_path, 'r') as file:
+    with open(file_path, "r") as file:
         src = file.read()
     iids = IIDs(file_path)
 
     instrumented_code = instrument_code(src, file_path, iids, selected_hooks)
     if instrumented_code is None:
         return
 
-    copied_file_path = re.sub(r'\.py$', '.py.orig', file_path)
+    copied_file_path = re.sub(r"\.py$", ".py.orig", file_path)
     copyfile(file_path, copied_file_path)
 
-    with open(file_path, 'w') as file:
+    with open(file_path, "w") as file:
         file.write(instrumented_code)
     iids.store()
-    print(f'Done with {file_path}')
+    print(f"Done with {file_path}")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     args = parser.parse_args()
     files = gather_files(args.files)
     additional_module = args.module
     analysis = args.analysis
-    modulePath = 'dynapyt.analyses'
+    modulePath = "dynapyt.analyses"
     if additional_module is not None:
         modulePath = additional_module
     try:
-        module = importlib.import_module(modulePath + '.' + analysis)
+        module = importlib.import_module(modulePath + "." + analysis)
     except TypeError as e:
-        print(f'--module was used but no value specified {e}')
+        print(f"--module was used but no value specified {e}")
     except ImportError as e:
-        print(f'module could not be imported {e}')
+        print(f"module could not be imported {e}")
 
     class_ = getattr(module, args.analysis)
     instance = class_()
-    method_list = [func for func in dir(instance) if callable(getattr(instance, func)) and not func.startswith("__")]
+    method_list = [
+        func
+        for func in dir(instance)
+        if callable(getattr(instance, func)) and not func.startswith("__")
+    ]
     selected_hooks = get_hooks_from_analysis(set(method_list))
     if len(files) < 2:
         for file_path in files:
             instrument_file(file_path, selected_hooks)
     else:
         arg_list = []
         for file_path in files:
```

### Comparing `dynapyt-0.2.3/src/dynapyt/utils/AnalysisUtils.py` & `dynapyt-0.3.0/src/dynapyt/utils/AnalysisUtils.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.3/src/dynapyt/utils/hierarchy.json` & `dynapyt-0.3.0/src/dynapyt/utils/hierarchy.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9402610964641039%*

 * *Differences: {"'runtime_event'": "{'literal': {'_float': OrderedDict(), '_list': OrderedDict(), '_tuple': "*

 * *                    "OrderedDict(), delete: ['float', 'list', 'tuple']}, 'operation': "*

 * *                    "{'binary_operation': {'augmented_assignment': OrderedDict([('add_assign', "*

 * *                    "OrderedDict()), ('bit_and_assign', OrderedDict()), ('bit_or_assign', "*

 * *                    "OrderedDict()), ('bit_xor_assign', OrderedDict()), ('divide_assign', "*

 * *                    "OrderedDict()), ('floor_div […]*

```diff
@@ -1,70 +1,62 @@
 {
     "runtime_event": {
         "begin_execution": {},
         "control_flow_event": {
-            "break": {},
-            "conditional_control_flow": {
-                "assert": {},
-                "enter_control_flow": {
-                    "enter_for": {},
-                    "enter_if": {},
-                    "enter_while": {}
-                },
-                "exit_control_flow": {
-                    "exit_for": {},
-                    "exit_if": {},
-                    "exit_while": {}
-                }
+            "_assert": {},
+            "_break": {},
+            "_continue": {},
+            "_raise": {},
+            "clean_exit_try": {},
+            "enter_control_flow": {
+                "enter_for": {},
+                "enter_if": {},
+                "enter_while": {}
             },
-            "continue": {},
+            "enter_try": {},
             "exception": {},
-            "function": {
-                "function_enter": {},
-                "function_exit": {
-                    "return": {},
-                    "yield": {}
-                }
-            },
-            "function_call": {
-                "post_call": {},
-                "pre_call": {}
-            },
-            "lambda": {},
-            "raise": {},
-            "try": {
-                "clean_exit_try": {},
-                "enter_try": {}
-            }
+            "exit_control_flow": {
+                "exit_for": {},
+                "exit_if": {},
+                "exit_while": {}
+            },
+            "function_enter": {},
+            "function_exit": {
+                "_return": {},
+                "_yield": {}
+            },
+            "post_call": {},
+            "pre_call": {}
         },
         "end_execution": {},
         "literal": {
+            "_float": {},
+            "_list": {},
+            "_tuple": {},
             "boolean": {},
             "dictionary": {},
-            "float": {},
             "imaginary": {},
             "integer": {},
-            "list": {},
-            "string": {},
-            "tuple": {}
+            "string": {}
         },
         "memory_access": {
             "delete": {},
             "read": {
                 "read_attribute": {},
                 "read_identifier": {},
                 "read_subscript": {}
             },
             "write": {}
         },
         "operation": {
             "binary_operation": {
+                "_and": {},
+                "_or": {},
                 "add": {},
-                "and": {},
-                "augmented_assign": {
+                "augmented_assignment": {
                     "add_assign": {},
                     "bit_and_assign": {},
                     "bit_or_assign": {},
                     "bit_xor_assign": {},
                     "divide_assign": {},
                     "floor_divide_assign": {},
                     "left_shift_assign": {},
@@ -80,34 +72,33 @@
                 "bit_xor": {},
                 "divide": {},
                 "floor_divide": {},
                 "left_shift": {},
                 "matrix_multiply": {},
                 "modulo": {},
                 "multiply": {},
-                "or": {},
                 "power": {},
                 "right_shift": {},
                 "subtract": {}
             },
             "comparison": {
+                "_in": {},
+                "_is": {},
                 "equal": {},
                 "greater_than": {},
                 "greater_than_equal": {},
-                "in": {},
-                "is": {},
                 "is_not": {},
                 "less_than": {},
                 "less_than_equal": {},
                 "not_equal": {},
                 "not_in": {}
             },
             "unary_operation": {
+                "_not": {},
                 "bit_invert": {},
                 "minus": {},
-                "not": {},
                 "plus": {}
             }
         },
         "uncaught_exception": {}
     }
 }
```

### Comparing `dynapyt-0.2.3/src/dynapyt/utils/hooks.py` & `dynapyt-0.3.0/src/dynapyt/utils/hooks.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.3/src/dynapyt/utils/nodeLocator.py` & `dynapyt-0.3.0/src/dynapyt/utils/nodeLocator.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.3/src/nativetracer/instrument_tracer.py` & `dynapyt-0.3.0/src/nativetracer/instrument_tracer.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.3/src/nativetracer/trc.py` & `dynapyt-0.3.0/src/nativetracer/trc.py`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.3/.gitignore` & `dynapyt-0.3.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -189,8 +189,12 @@
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 venvs/**
 !venvs
 under_test/**
 !under_test
-output.log
+output.log
+docs/dynapyt/
+docs/index.html
+docs/search.js
+docs/hooks.md
```

### Comparing `dynapyt-0.2.3/LICENSE` & `dynapyt-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.3/README.md` & `dynapyt-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,18 @@
 **Note:** The analysis name should either match the analysis name used for the instrumentation, or the analysis should have a subset of hooks used in the instrumentation analysis.
 
 Single command to instrument and run an analysis on a project:  
 ```
 python -m dynapyt.run_all --directory <directory of project> --entry <entry file (python)> --analysis <analysis name>
 ```
 
+## Available Hooks
+
+Check out [this auto-generated API reference](https://sola-st.github.io/DynaPyt/) for available hooks.
+
 --------------------
 
 ## Reproducing the Results in the Paper
 
 To reproduce results from the paper, follow these instructions:  
 We suggest running each experiment in a fresh Python environment.
```

### Comparing `dynapyt-0.2.3/pyproject.toml` & `dynapyt-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dynapyt-0.2.3/PKG-INFO` & `dynapyt-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynapyt
-Version: 0.2.3
+Version: 0.3.0
 Summary: Dynamic analysis framework for Python
 Project-URL: Bug Tracker, https://github.com/sola-st/DynaPyt/issues
 Project-URL: Homepage, https://github.com/sola-st/DynaPyt
 Author-email: Aryaz Eghbali <aryaz.egh@gmail.com>, Michael Pradel <michael@binaervarianz.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -82,14 +82,18 @@
 **Note:** The analysis name should either match the analysis name used for the instrumentation, or the analysis should have a subset of hooks used in the instrumentation analysis.
 
 Single command to instrument and run an analysis on a project:  
 ```
 python -m dynapyt.run_all --directory <directory of project> --entry <entry file (python)> --analysis <analysis name>
 ```
 
+## Available Hooks
+
+Check out [this auto-generated API reference](https://sola-st.github.io/DynaPyt/) for available hooks.
+
 --------------------
 
 ## Reproducing the Results in the Paper
 
 To reproduce results from the paper, follow these instructions:  
 We suggest running each experiment in a fresh Python environment.
```

