# Comparing `tmp/cryptol-2.13.0.tar.gz` & `tmp/cryptol-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptol-2.13.0.tar", last modified: Tue May 17 12:53:16 2022, max compression
+gzip compressed data, was "cryptol-3.0.0.tar", max compression
```

## Comparing `cryptol-2.13.0.tar` & `cryptol-3.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1504 2022-03-17 13:58:42.893837 cryptol-2.13.0/LICENSE
--rw-r--r--   0        0        0     6974 2022-03-17 13:58:42.893837 cryptol-2.13.0/README.md
--rw-r--r--   0        0        0     1242 2022-03-17 13:58:42.893837 cryptol-2.13.0/cryptol/__init__.py
--rw-r--r--   0        0        0    21302 2022-03-17 13:58:42.893837 cryptol-2.13.0/cryptol/bitvector.py
--rw-r--r--   0        0        0    11470 2022-03-17 13:58:42.893837 cryptol-2.13.0/cryptol/commands.py
--rw-r--r--   0        0        0    25447 2022-03-17 13:58:42.893837 cryptol-2.13.0/cryptol/connection.py
--rw-r--r--   0        0        0    15913 2022-03-17 13:58:42.897837 cryptol-2.13.0/cryptol/cryptoltypes.py
--rw-r--r--   0        0        0     4476 2022-03-17 13:58:42.897837 cryptol-2.13.0/cryptol/custom_fstring.py
--rw-r--r--   0        0        0      561 2022-03-17 13:58:42.897837 cryptol-2.13.0/cryptol/opaque.py
--rw-r--r--   0        0        0        0 2022-03-17 13:58:42.897837 cryptol-2.13.0/cryptol/py.typed
--rw-r--r--   0        0        0     3900 2022-03-17 13:58:42.897837 cryptol-2.13.0/cryptol/quoting.py
--rw-r--r--   0        0        0    11778 2022-03-17 13:58:42.897837 cryptol-2.13.0/cryptol/single_connection.py
--rw-r--r--   0        0        0     3018 2022-03-17 13:58:42.897837 cryptol-2.13.0/cryptol/solver.py
--rw-r--r--   0        0        0    18684 2022-03-17 13:58:42.897837 cryptol-2.13.0/cryptol/synchronous.py
--rw-r--r--   0        0        0      228 2022-03-17 13:58:42.897837 cryptol-2.13.0/mypy.ini
--rw-r--r--   0        0        0      560 2022-05-16 13:16:55.971212 cryptol-2.13.0/pyproject.toml
--rw-r--r--   0        0        0     7902 2022-05-17 12:53:16.626243 cryptol-2.13.0/setup.py
--rw-r--r--   0        0        0     7687 2022-05-17 12:53:16.626960 cryptol-2.13.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2022-03-17 13:58:42.893837 cryptol-3.0.0/LICENSE
+-rw-r--r--   0        0        0     6969 2023-06-22 14:12:12.001591 cryptol-3.0.0/README.md
+-rw-r--r--   0        0        0     1242 2022-05-18 13:09:19.916614 cryptol-3.0.0/cryptol/__init__.py
+-rw-r--r--   0        0        0    21302 2022-05-18 13:09:19.916614 cryptol-3.0.0/cryptol/bitvector.py
+-rw-r--r--   0        0        0    12494 2023-06-22 14:12:12.001591 cryptol-3.0.0/cryptol/commands.py
+-rw-r--r--   0        0        0    26865 2023-06-22 14:12:12.001591 cryptol-3.0.0/cryptol/connection.py
+-rw-r--r--   0        0        0    18605 2023-06-22 14:12:12.001591 cryptol-3.0.0/cryptol/cryptoltypes.py
+-rw-r--r--   0        0        0     4476 2022-05-18 13:09:19.916614 cryptol-3.0.0/cryptol/custom_fstring.py
+-rw-r--r--   0        0        0      355 2023-06-22 14:12:12.001591 cryptol-3.0.0/cryptol/file_deps.py
+-rw-r--r--   0        0        0      561 2022-05-18 13:09:19.916614 cryptol-3.0.0/cryptol/opaque.py
+-rw-r--r--   0        0        0        0 2022-03-17 13:58:42.897837 cryptol-3.0.0/cryptol/py.typed
+-rw-r--r--   0        0        0     3900 2022-05-18 13:09:19.916614 cryptol-3.0.0/cryptol/quoting.py
+-rw-r--r--   0        0        0    12665 2023-06-22 14:12:12.001591 cryptol-3.0.0/cryptol/single_connection.py
+-rw-r--r--   0        0        0     3178 2023-06-22 14:12:12.005591 cryptol-3.0.0/cryptol/solver.py
+-rw-r--r--   0        0        0    19875 2023-06-22 14:12:12.005591 cryptol-3.0.0/cryptol/synchronous.py
+-rw-r--r--   0        0        0      228 2022-03-17 13:58:42.897837 cryptol-3.0.0/mypy.ini
+-rw-r--r--   0        0        0      584 2023-06-26 17:51:42.962079 cryptol-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7733 1970-01-01 00:00:00.000000 cryptol-3.0.0/PKG-INFO
```

### Comparing `cryptol-2.13.0/LICENSE` & `cryptol-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptol-2.13.0/README.md` & `cryptol-3.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,15 @@
 
 Or a server URL can be specified directly in the script, e.g.:
 
 ```
 cryptol.connect(url=URL)
 ```
 
-where `URL` is a URL for a running Cryptol server in HTTP mode.
+There is a step-by-step example [here](GettingStarted.md).
 
 ## Running Cryptol Scripts from a clean server state
 
 To ensure any previous server state is cleared when running a Cryptol Python script
 against a persistent server (e.g., one running in HTTP mode in a different process),
 the `reset_server` keyword can be passed to `cryptol.connect()`. E.g.,
```

### Comparing `cryptol-2.13.0/cryptol/__init__.py` & `cryptol-3.0.0/cryptol/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptol-2.13.0/cryptol/bitvector.py` & `cryptol-3.0.0/cryptol/bitvector.py`

 * *Files identical despite different names*

### Comparing `cryptol-2.13.0/cryptol/commands.py` & `cryptol-3.0.0/cryptol/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,22 +71,39 @@
 class CryptolLoadFile(argo.Command):
     def __init__(self, connection : HasProtocolState, filename : str, timeout: Optional[float]) -> None:
         super(CryptolLoadFile, self).__init__('load file', {'file': filename}, connection, timeout=timeout)
 
     def process_result(self, res : Any) -> Any:
         return res
 
+class CryptolFileDeps(argo.Command):
+  def __init__( self
+              , connection : HasProtocolState
+              , name : str, isFile : bool
+              , timeout: Optional[float]
+              ) -> None:
+    super(CryptolFileDeps, self).__init__('file-deps'
+                                         , {'name': name, 'is-file': isFile }
+                                         , connection
+                                         , timeout=timeout
+                                         )
+
+  def process_result(self, res : Any) -> Any:
+      return res
+
 class CryptolExtendSearchPath(argo.Command):
     def __init__(self, connection : HasProtocolState, dirs : List[str], timeout: Optional[float]) -> None:
         super(CryptolExtendSearchPath, self).__init__('extend search path', {'paths': dirs}, connection, timeout=timeout)
 
     def process_result(self, res : Any) -> Any:
         return res
 
 
+
+
 class CryptolEvalExprRaw(argo.Command):
     def __init__(self, connection : HasProtocolState, expr : Any, timeout: Optional[float]) -> None:
         super(CryptolEvalExprRaw, self).__init__(
             'evaluate expression',
             {'expression': expr},
             connection,
             timeout=timeout
@@ -266,14 +283,24 @@
 class CryptolNames(argo.Command):
     def __init__(self, connection : HasProtocolState, timeout: Optional[float]) -> None:
         super(CryptolNames, self).__init__('visible names', {}, connection, timeout=timeout)
 
     def process_result(self, res : Any) -> Any:
         return res
 
+class CryptolParameterNames(CryptolNames):
+    def process_result(self, res : Any) -> Any:
+        res = super(CryptolParameterNames, self).process_result(res)
+        return [ n for n in res if "parameter" in n ]
+
+class CryptolPropertyNames(CryptolNames):
+    def process_result(self, res : Any) -> Any:
+        res = super(CryptolPropertyNames, self).process_result(res)
+        return [ n for n in res if "pragmas" in n and "property" in n["pragmas"] ]
+
 
 class CryptolFocusedModule(argo.Command):
     def __init__(self, connection : HasProtocolState, timeout: Optional[float]) -> None:
         super(CryptolFocusedModule, self).__init__(
             'focused module',
             {},
             connection,
```

### Comparing `cryptol-2.13.0/cryptol/connection.py` & `cryptol-3.0.0/cryptol/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,14 +209,23 @@
 
         :param timeout: Optional timeout for this request (in seconds).
         """
         timeout = timeout if timeout is not None else self.timeout
         self.most_recent_result = CryptolLoadModule(self, module_name, timeout)
         return self.most_recent_result
 
+    def file_deps(self, name : str, isFile : bool, *, timeout:Optional[float] = None) -> argo.Command:
+        """Get information about a module or a file.
+
+        :param timeout: Optional timeout for this request (in seconds).
+        """
+        timeout = timeout if timeout is not None else self.timeout
+        self.most_recent_result = CryptolFileDeps(self, name, isFile, timeout)
+        return self.most_recent_result
+
     def eval_raw(self, expression : Any, *, timeout:Optional[float] = None) -> argo.Command:
         """Like the member method ``eval``, but does not call
         ``from_cryptol_arg`` on the ``.result()``.
 
         :param timeout: Optional timeout for this request (in seconds).
         """
         if hasattr(expression, '__to_cryptol__'):
@@ -375,21 +384,39 @@
         :param timeout: Optional timeout for this request (in seconds).
         """
         timeout = timeout if timeout is not None else self.timeout
         self.most_recent_result = CryptolSafe(self, expr, solver, timeout)
         return self.most_recent_result
 
     def names(self, *, timeout:Optional[float] = None) -> argo.Command:
-        """Discover the list of names currently in scope in the current context.
+        """Discover the list of term names currently in scope in the current context.
 
         :param timeout: Optional timeout for this request (in seconds)."""
         timeout = timeout if timeout is not None else self.timeout
         self.most_recent_result = CryptolNames(self, timeout)
         return self.most_recent_result
 
+    def parameter_names(self, *, timeout:Optional[float] = None) -> argo.Command:
+        """Discover the list of module parameter names currently in scope in the current context.
+        The result is a subset of the list returned by `names`.
+
+        :param timeout: Optional timeout for this request (in seconds)."""
+        timeout = timeout if timeout is not None else self.timeout
+        self.most_recent_result = CryptolParameterNames(self, timeout)
+        return self.most_recent_result
+
+    def property_names(self, *, timeout:Optional[float] = None) -> argo.Command:
+        """Discover the list of property names currently in scope in the current context.
+        The result is a subset of the list returned by `names`.
+
+        :param timeout: Optional timeout for this request (in seconds)."""
+        timeout = timeout if timeout is not None else self.timeout
+        self.most_recent_result = CryptolPropertyNames(self, timeout)
+        return self.most_recent_result
+
     def focused_module(self, *, timeout:Optional[float] = None) -> argo.Command:
         """Return the name of the currently-focused module.
 
         :param timeout: Optional timeout for this request (in seconds)."""
         timeout = timeout if timeout is not None else self.timeout
         self.most_recent_result = CryptolFocusedModule(self, timeout)
         return self.most_recent_result
```

### Comparing `cryptol-2.13.0/cryptol/cryptoltypes.py` & `cryptol-3.0.0/cryptol/cryptoltypes.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import BitVector #type: ignore
 from .bitvector import BV
 from .opaque import OpaqueValue
 
 import typing
 from typing import cast, Any, Dict, Iterable, List, NoReturn, Optional, TypeVar, Union
 import typing_extensions
-from typing_extensions import Protocol, runtime_checkable
+from typing_extensions import Protocol, runtime_checkable, TypedDict, NotRequired
 
 A = TypeVar('A')
 
 
 # -----------------------------------------------------------
 # CryptolJSON and CryptolCode
 # -----------------------------------------------------------
@@ -472,7 +472,74 @@
         return argument_types(obj.body)
     elif isinstance(obj, Function):
         arg1 = obj.domain
         args = argument_types(obj.range)
         return [arg1] + args
     else:
         return []
+
+
+# -----------------------------------------------------------
+# Cryptol Name Info
+# -----------------------------------------------------------
+
+CryptolInfixInfo = TypedDict("CryptolInfixInfo",
+    { "associativity": Union[typing_extensions.Literal["left-associative"],
+                             typing_extensions.Literal["right-associative"],
+                             typing_extensions.Literal["non-associative"]]
+    , "level": int
+    })
+
+CryptolNameInfo = TypedDict("CryptolNameInfo",
+    { "module": str
+    , "name": str
+    , "type": CryptolTypeSchema
+    , "type string": str
+    , "documentation": NotRequired[str]
+    , "pragmas": NotRequired[List[str]]
+    , "parameter": NotRequired[typing.Tuple[()]]
+    , "infix": NotRequired[CryptolInfixInfo]
+    })
+
+def check_dict(d : Any, required_keys : Dict[str, Any], optional_keys : Dict[str, Any] = {}) -> bool:
+    return isinstance(d, dict) and all(k in d for k in required_keys) and \
+           all(k in required_keys and isinstance(d[k], required_keys[k]) or
+               k in optional_keys and isinstance(d[k], optional_keys[k]) for k in d)
+
+def to_cryptol_name_info(d : Any) -> CryptolNameInfo:
+    req_keys = {"module": str, "name": str, "type": Dict, "type string": str}
+    opt_keys = {"documentation": str, "pragmas": List, "parameter": List, "infix": Dict}
+    infix_req_keys = {"associativity": str, "level": int}
+    if check_dict(d, req_keys, opt_keys) and ("infix" not in d or check_dict(d["infix"], infix_req_keys)):
+        d["type"] = to_schema(d["type"])
+        if "parameter" in d: d["parameter"] = ()
+        # the calls to check_dict and the above ensure this cast is OK
+        return cast(CryptolNameInfo, d)
+    else:
+        raise ValueError("Cryptol name info is malformed: " + str(d))
+
+
+# -----------------------------------------------------------
+# Cryptol Module Info
+# -----------------------------------------------------------
+
+CryptolFocusedModuleInfo = TypedDict("CryptolFocusedModuleInfo",
+    { "module": str
+    , "parameterized": bool
+    })
+
+CryptolNoModuleInfo = TypedDict("CryptolNoModuleInfo",
+    { "module": None
+    })
+
+CryptolModuleInfo = Union[CryptolFocusedModuleInfo, CryptolNoModuleInfo]
+
+def to_cryptol_module_info(d : Any) -> CryptolModuleInfo:
+    if check_dict(d, {"module": str, "parameterized": bool}):
+        # the call to check_dict ensures this cast is OK
+        return cast(CryptolFocusedModuleInfo, d)
+    elif check_dict(d, {"module": type(None)}):
+        # the call to check_dict ensures this cast is OK
+        return cast(CryptolNoModuleInfo, d)
+    else:
+        raise ValueError("Cryptol module info is malformed: " + str(d))
+
```

### Comparing `cryptol-2.13.0/cryptol/custom_fstring.py` & `cryptol-3.0.0/cryptol/custom_fstring.py`

 * *Files identical despite different names*

### Comparing `cryptol-2.13.0/cryptol/opaque.py` & `cryptol-3.0.0/cryptol/opaque.py`

 * *Files identical despite different names*

### Comparing `cryptol-2.13.0/cryptol/quoting.py` & `cryptol-3.0.0/cryptol/quoting.py`

 * *Files identical despite different names*

### Comparing `cryptol-2.13.0/cryptol/single_connection.py` & `cryptol-3.0.0/cryptol/single_connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -214,19 +214,29 @@
 
 def safe(expr : Any, solver : Solver = Z3, *, timeout:Optional[float] = None) -> Union[Safe, Counterexample, OfflineSmtQuery]:
     """Check via an external SMT solver that the given term is safe for all inputs,
     which means it cannot encounter a run-time error.
     """
     return __get_designated_connection().safe(expr, solver, timeout=timeout)
 
-def names(*, timeout:Optional[float] = None) -> List[Dict[str,Any]]:
-    """Discover the list of names currently in scope in the current context."""
+def names(*, timeout:Optional[float] = None) -> List[cryptoltypes.CryptolNameInfo]:
+    """Discover the list of term names currently in scope in the current context."""
     return __get_designated_connection().names(timeout=timeout)
 
-def focused_module(*, timeout:Optional[float] = None) -> Dict[str,Any]:
+def parameter_names(*, timeout:Optional[float] = None) -> List[cryptoltypes.CryptolNameInfo]:
+    """Discover the list of module parameter names currently in scope in the current context.
+    The result is a subset of the list returned by `names`."""
+    return __get_designated_connection().parameter_names(timeout=timeout)
+
+def property_names(*, timeout:Optional[float] = None) -> List[cryptoltypes.CryptolNameInfo]:
+    """Discover the list of property names currently in scope in the current context.
+    The result is a subset of the list returned by `names`."""
+    return __get_designated_connection().property_names(timeout=timeout)
+
+def focused_module(*, timeout:Optional[float] = None) -> cryptoltypes.CryptolModuleInfo:
     """Returns the name and other information about the currently-focused module."""
     return __get_designated_connection().focused_module(timeout=timeout)
 
 def reset() -> None:
     """Resets the connection, causing its unique state on the server to be freed (if applicable).
     After a reset a connection may be treated as if it were a fresh connection with the server if desired."""
     __get_designated_connection().reset()
@@ -238,7 +248,13 @@
 def interrupt() -> None:
     """Interrupt the Cryptol server, cancelling any in-progress requests."""
     __get_designated_connection().interrupt()
 
 def logging(on : bool, *, dest : TextIO = sys.stderr) -> None:
     """Whether to log received and transmitted JSON."""
     __get_designated_connection().logging(on=on,dest=dest)
+
+def file_deps(m : str, isFile:bool, timeout:Optional[float] = None) -> Any:
+    """Get information about a module or a file."""
+    return __get_designated_connection().file_deps(m,isFile,timeout=timeout)
+
+
```

### Comparing `cryptol-2.13.0/cryptol/solver.py` & `cryptol-3.0.0/cryptol/solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,29 +48,32 @@
 class OfflineSolver(Solver):
   def without_hash_consing(self) -> 'OfflineSolver':
     return OfflineSolver(name=self.name(), hash_consing=False)
 
 # Cryptol-supported SMT configurations/solvers
 # (see Cryptol.Symbolic.SBV Haskell module)
 CVC4: OnlineSolver          = OnlineSolver("cvc4")
+CVC5: OnlineSolver          = OnlineSolver("cvc5")
 YICES: OnlineSolver         = OnlineSolver("yices")
 Z3: OnlineSolver            = OnlineSolver("z3")
 BOOLECTOR: OnlineSolver     = OnlineSolver("boolector")
 MATHSAT: OnlineSolver       = OnlineSolver("mathsat")
 ABC: OnlineSolver           = OnlineSolver("abc")
 OFFLINE: OfflineSolver      = OfflineSolver("offline")
 ANY: OnlineSolver           = OnlineSolver("any")
 SBV_CVC4: OnlineSolver      = OnlineSolver("sbv-cvc4")
+SBV_CVC5: OnlineSolver      = OnlineSolver("sbv-cvc5")
 SBV_YICES: OnlineSolver     = OnlineSolver("sbv-yices")
 SBV_Z3: OnlineSolver        = OnlineSolver("sbv-z3")
 SBV_BOOLECTOR: OnlineSolver = OnlineSolver("sbv-boolector")
 SBV_MATHSAT: OnlineSolver   = OnlineSolver("sbv-mathsat")
 SBV_ABC: OnlineSolver       = OnlineSolver("sbv-abc")
 SBV_OFFLINE: OfflineSolver  = OfflineSolver("sbv-offline")
 SBV_ANY: OnlineSolver       = OnlineSolver("sbv-any")
 W4_CVC4: OnlineSolver       = OnlineSolver("w4-cvc4")
+W4_CVC5: OnlineSolver       = OnlineSolver("w4-cvc5")
 W4_YICES: OnlineSolver      = OnlineSolver("w4-yices")
 W4_Z3: OnlineSolver         = OnlineSolver("w4-z3")
 W4_BOOLECTOR: OnlineSolver  = OnlineSolver("w4-boolector")
 W4_OFFLINE: OfflineSolver   = OfflineSolver("w4-offline")
 W4_ABC: OnlineSolver        = OnlineSolver("w4-abc")
 W4_ANY: OnlineSolver        = OnlineSolver("w4-any")
```

### Comparing `cryptol-2.13.0/cryptol/synchronous.py` & `cryptol-3.0.0/cryptol/synchronous.py`

 * *Files 4% similar despite different names*

```diff
@@ -343,29 +343,43 @@
             elif res['result'] == 'invalid':
                 return Counterexample(res['counterexample type'], [from_cryptol_arg(arg['expr']) for arg in res['counterexample']])
             else:
                 raise ValueError("Unexpected 'safe' SMT result: " + str(res))
         else:
             raise ValueError("Unknown solver type: " + str(solver))
 
-    def names(self, *, timeout:Optional[float] = None) -> List[Dict[str,Any]]:
-        """Discover the list of names currently in scope in the current context."""
+    def names(self, *, timeout:Optional[float] = None) -> List[cryptoltypes.CryptolNameInfo]:
+        """Discover the list of term names currently in scope in the current context."""
         res = self.connection.names(timeout=timeout).result()
-        if isinstance(res, list) and all(isinstance(d, dict) and all(isinstance(k, str) for k in d.keys()) for d in res):
-            return res
+        if isinstance(res, list):
+            return [ cryptoltypes.to_cryptol_name_info(entry) for entry in res ]
         else:
-            raise ValueError("Panic! Result of `names()` is malformed: " + str(res))
+            raise ValueError("Result of `names()` is not a list: " + str(res))
 
-    def focused_module(self, *, timeout:Optional[float] = None) -> Dict[str,Any]:
-        """Returns the name and other information about the currently-focused module."""
-        res = self.connection.focused_module(timeout=timeout).result()
-        if isinstance(res, dict) and all(isinstance(k, str) for k in res.keys()):
-            return res
+    def parameter_names(self, *, timeout:Optional[float] = None) -> List[cryptoltypes.CryptolNameInfo]:
+        """Discover the list of module parameter names currently in scope in the current context.
+        The result is a subset of the list returned by `names`."""
+        res = self.connection.parameter_names(timeout=timeout).result()
+        if isinstance(res, list):
+            return [ cryptoltypes.to_cryptol_name_info(entry) for entry in res ]
+        else:
+            raise ValueError("Result of `parameter_names()` is not a list: " + str(res))
+
+    def property_names(self, *, timeout:Optional[float] = None) -> List[cryptoltypes.CryptolNameInfo]:
+        """Discover the list of property names currently in scope in the current context.
+        The result is a subset of the list returned by `names`."""
+        res = self.connection.property_names(timeout=timeout).result()
+        if isinstance(res, list):
+            return [ cryptoltypes.to_cryptol_name_info(entry) for entry in res ]
         else:
-            raise ValueError("Panic! Result of `focused_module()` is malformed: " + str(res))
+            raise ValueError("Result of `property_names()` is not a list: " + str(res))
+
+    def focused_module(self, *, timeout:Optional[float] = None) -> cryptoltypes.CryptolModuleInfo:
+        """Returns the name and other information about the currently-focused module."""
+        return cryptoltypes.to_cryptol_module_info(self.connection.focused_module(timeout=timeout).result())
 
     def reset(self) -> None:
         """Resets the connection, causing its unique state on the server to be freed (if applicable).
         After a reset a connection may be treated as if it were a fresh connection with the server if desired."""
         self.connection.reset()
 
     def reset_server(self) -> None:
@@ -375,7 +389,13 @@
     def interrupt(self) -> None:
         """Interrupt the Cryptol server, cancelling any in-progress requests."""
         self.connection.interrupt()
 
     def logging(self, on : bool, *, dest : TextIO = sys.stderr) -> None:
         """Whether to log received and transmitted JSON."""
         self.connection.server_connection.logging(on=on,dest=dest)
+
+    def file_deps( self
+                 , m : str, isFile:bool
+                 , timeout:Optional[float] = None) -> Any:
+        """Get information about a module or a file."""
+        return self.connection.file_deps(m,isFile,timeout=timeout).result()
```

### Comparing `cryptol-2.13.0/pyproject.toml` & `cryptol-3.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "cryptol"
-version = "2.13.0"
+version = "3.0.0"
 readme = "README.md"
 keywords = ["cryptography", "verification"]
-description = "Cryptol client for the Cryptol 2.12 RPC server"
+description = "Cryptol client for the Cryptol 2.13 RPC server"
 authors = ["Galois, Inc. <cryptol-team@galois.com>"]
 
 license = "BSD License"
 include = [
     "LICENSE",
     "mypy.ini",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7.0,<4"
-requests = "^2.25.1"
+python = ">=3.8.0,<4"
+requests = "^2.31.0"
 BitVector = "^3.4.9"
-argo-client = "0.0.10"
+argo-client = "0.0.11"
 typing-extensions = "^4.1.1"
 
 [tool.poetry.dev-dependencies]
-mypy = "^0.812"
+mypy = "^0.991"
 
 [build-system]
-requires = ["poetry>=1.1.4", "setuptools>=40.8.0"]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `cryptol-2.13.0/setup.py` & `cryptol-3.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,218 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: cryptol
+Version: 3.0.0
+Summary: Cryptol client for the Cryptol 2.13 RPC server
+License: BSD License
+Keywords: cryptography,verification
+Author: Galois, Inc.
+Author-email: cryptol-team@galois.com
+Requires-Python: >=3.8.0,<4
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: BitVector (>=3.4.9,<4.0.0)
+Requires-Dist: argo-client (==0.0.11)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: typing-extensions (>=4.1.1,<5.0.0)
+Description-Content-Type: text/markdown
+
+# Cryptol Python Client
+
+In-development Python client for Cryptol. Currently tested on Linux and MacOS --
+at present there may be some minor issues running the Python Client in a Windows
+environment that need to be addressed (e.g., some Python process management methods
+are not cross-OS-compatible).
+
+This Cryptol client depends on the
+[cryptol-remote-api](https://github.com/GaloisInc/cryptol/tree/master/cryptol-remote-api)
+server.
+
+# TL;DR Steps to running Cryptol Python scripts
+
+1. Clone the repo 
+```
+git clone https://github.com/GaloisInc/cryptol.git
+```
+2. Enter the repo
+```
+cd cryptol
+```
+3. Initialize git submodules 
+```
+git submodule update --init
+```
+4. Navigate to the python client
+```
+cd cryptol-remote-api/python
+```
+5. Install and setup some version of the `cryptol-remote-api` server and update any
+   relevant environment variables as needed (see `cryptol.connect()` documentation
+   for the various ways a server can be connected to).
+   E.g., here is how the docker image of the server might be used:
+```
+$ docker run --name=cryptol-remote-api -d \
+  -v $PWD/tests/cryptol/test-files:/home/cryptol/tests/cryptol/test-files \
+  -p 8080:8080 \
+  ghcr.io/galoisinc/cryptol-remote-api:nightly-portable
+$ export CRYPTOL_SERVER_URL="http://localhost:8080/"
+```
+6. Install the Python client (requires Python v3.7 or newer -- we recommend using [`poetry`](https://python-poetry.org/docs/#installation) to install the package):
+```
+$ poetry install 
+```
+7. Run tests or individual scripts:
+```
+$ poetry run python -m unittest discover tests/cryptol
+$ poetry run python tests/cryptol/test_salsa20.py
+```
+
+# Python Client Installation (via Poetry)
+
+First, clone the repository and submodules.
+
+```
+$ git clone https://github.com/GaloisInc/cryptol.git
+$ cd cryptol
+$ git submodule update --init
+```
+
+Then, use [`poetry`](https://python-poetry.org/docs/#installation) to install
+the python client from the `cryptol-remote-api/python` directory:
+
+```
+$ cd cryptol-remote-api/python
+$ poetry install
+```
+
+# Cryptol server
+
+To run the verification scripts a `cryptol-remote-api` server must be available,
+either as a local executable or running in docker image listening on a port.
+
+## Connecting with a server in a script
+
+Connecting to a server in a Python script is accomplished via the `cryptol.connect`
+method. Its accompanying Python doc strings describe the various ways it can be
+used. Below is a brief summary:
+
+`cryptol.connect()`, when provided no arguments, will attempt the following in order:
+
+1. If the environment variable ``CRYPTOL_SERVER`` is set and refers to an
+   executable, it is assumed to be a `cryptol-remote-api` executable and will be
+   used for the duration of the script.
+2. If the environment variable ``CRYPTOL_SERVER_URL`` is set, it is assumed to be
+   the URL for a running Cryptol server in ``http`` mode and will be connected to.
+   (N.B., this can be a local server or a server running in a docker image.)
+3. If an executable ``cryptol-remote-api`` is available on the ``PATH`` it is
+    assumed to be a Cryptol server and will be used for the duration of the script.
+
+Additional arguments and options are documented with the function.
+
+Notably, the `reset_server` keyword can be used to connect to a running server
+and reset it, ensuring states from previous scripts have been cleared. E.g.,
+`cryptol.connect(reset_server=True)`.
+
+
+## Acquiring a Cryptol Server
+
+There are several ways a server executable can be obtained.
+
+### Server executables
+
+An executable of the server is now included in each release of Cryptol.
+
+Nightly server builds can be found as `Artifacts` of the [Nightly
+Builds](https://github.com/GaloisInc/saw-script/actions/workflows/nightly.yml)
+github action. I.e., go to the `Nightly Builds` Github Action, click on a
+successful build, scroll to the bottom and under `Artifacts` a Linux, Windows,
+and MacOS tarball will be listed.
+
+Nightly Docker images of the server can be found under the
+[Packages](https://github.com/orgs/GaloisInc/packages?repo_name=cryptol) section
+of the Cryptol github repository.
+
+### Server docker images
+
+Release docker images for the Cryptol server are distributed with Cryptol
+releases; nightly Cryptol servers are available under the
+[Packages](https://github.com/orgs/GaloisInc/packages) section of the Cryptol repository.
+
+These images are set up to run as HTTP `cryptol-remote-api` servers, e.g.:
+
+```
+docker run --name=cryptol-remote-api -d \
+  -p 8080:8080 \
+  ghcr.io/galoisinc/cryptol-remote-api:nightly-portable
+```
+
+The `-v` option to `docker run` can be used to load files into the docker
+server's working directory so they can be loaded into the server at the request
+of python scripts. E.g., `-v PATH_TO_FILES:/home/cryptol/files/` will upload the
+contents of the host machine's directory `PATH_TO_FILES` to the
+`/home/cryptol/files/` directory in the docker container, which corresponds to the
+relative path `files/` for the Cryptol server. (If desired, it can be useful to
+place files in a location in the Docker container such that the same relative
+paths in scripts refer to the same files in the host machine and docker
+container.)
+
+### Building from Source
+
+If this repository is checked out and the build directions are successfully run,
+`cabal v2-exec which cryptol-remote-api` should indicate where the server executable has
+been stored by `cabal`.
+
+Alternatively `cabal v2-install cryptol-remote-api` should install the server
+executable into the user's `~/.cabal/bin` directory (or similar), which (if
+configured properly) should then appear as `cryptol-remote-api` in a user's `PATH`.
+
+
+# Running Python Cryptol scripts
+
+Once the server is setup and any path variables are setup as desired, the
+Python (>= v3.7) client can be installed using
+[`poetry`](https://python-poetry.org/docs/#installation) as follows:
+
+```
+$ cd cryptol-remote-api/python
+$ poetry install
+```
+
+Then the tests or individual scripts can be run as follows:
+```
+$ poetry run python -m unittest discover tests/cryptol
+$ poetry run python tests/cryptol/test_cryptol_api.py
+```
+
+If leveraging environment variables is undesirable, the scripts themselves can
+specify a command to launch the server, e.g.:
+
+```
+cryptol.connect(COMMAND)
+```
+
+where `COMMAND` is a command to launch a new Cryptol server in socket mode.
+
+Or a server URL can be specified directly in the script, e.g.:
+
+```
+cryptol.connect(url=URL)
+```
+
+There is a step-by-step example [here](GettingStarted.md).
+
+## Running Cryptol Scripts from a clean server state
+
+To ensure any previous server state is cleared when running a Cryptol Python script
+against a persistent server (e.g., one running in HTTP mode in a different process),
+the `reset_server` keyword can be passed to `cryptol.connect()`. E.g.,
+
+```
+cryptol.connect(url="http://localhost:8080/", reset_server=True)
+```
 
-packages = \
-['cryptol']
+will connect to a Cryptol server running at `http://localhost:8080/` and will
+guarantee any previous state on the server is cleared.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['BitVector>=3.4.9,<4.0.0',
- 'argo-client==0.0.10',
- 'requests>=2.25.1,<3.0.0',
- 'typing-extensions>=4.1.1,<5.0.0']
-
-setup_kwargs = {
-    'name': 'cryptol',
-    'version': '2.13.0',
-    'description': 'Cryptol client for the Cryptol 2.12 RPC server',
-    'long_description': '# Cryptol Python Client\n\nIn-development Python client for Cryptol. Currently tested on Linux and MacOS --\nat present there may be some minor issues running the Python Client in a Windows\nenvironment that need to be addressed (e.g., some Python process management methods\nare not cross-OS-compatible).\n\nThis Cryptol client depends on the\n[cryptol-remote-api](https://github.com/GaloisInc/cryptol/tree/master/cryptol-remote-api)\nserver.\n\n# TL;DR Steps to running Cryptol Python scripts\n\n1. Clone the repo \n```\ngit clone https://github.com/GaloisInc/cryptol.git\n```\n2. Enter the repo\n```\ncd cryptol\n```\n3. Initialize git submodules \n```\ngit submodule update --init\n```\n4. Navigate to the python client\n```\ncd cryptol-remote-api/python\n```\n5. Install and setup some version of the `cryptol-remote-api` server and update any\n   relevant environment variables as needed (see `cryptol.connect()` documentation\n   for the various ways a server can be connected to).\n   E.g., here is how the docker image of the server might be used:\n```\n$ docker run --name=cryptol-remote-api -d \\\n  -v $PWD/tests/cryptol/test-files:/home/cryptol/tests/cryptol/test-files \\\n  -p 8080:8080 \\\n  ghcr.io/galoisinc/cryptol-remote-api:nightly-portable\n$ export CRYPTOL_SERVER_URL="http://localhost:8080/"\n```\n6. Install the Python client (requires Python v3.7 or newer -- we recommend using [`poetry`](https://python-poetry.org/docs/#installation) to install the package):\n```\n$ poetry install \n```\n7. Run tests or individual scripts:\n```\n$ poetry run python -m unittest discover tests/cryptol\n$ poetry run python tests/cryptol/test_salsa20.py\n```\n\n# Python Client Installation (via Poetry)\n\nFirst, clone the repository and submodules.\n\n```\n$ git clone https://github.com/GaloisInc/cryptol.git\n$ cd cryptol\n$ git submodule update --init\n```\n\nThen, use [`poetry`](https://python-poetry.org/docs/#installation) to install\nthe python client from the `cryptol-remote-api/python` directory:\n\n```\n$ cd cryptol-remote-api/python\n$ poetry install\n```\n\n# Cryptol server\n\nTo run the verification scripts a `cryptol-remote-api` server must be available,\neither as a local executable or running in docker image listening on a port.\n\n## Connecting with a server in a script\n\nConnecting to a server in a Python script is accomplished via the `cryptol.connect`\nmethod. Its accompanying Python doc strings describe the various ways it can be\nused. Below is a brief summary:\n\n`cryptol.connect()`, when provided no arguments, will attempt the following in order:\n\n1. If the environment variable ``CRYPTOL_SERVER`` is set and refers to an\n   executable, it is assumed to be a `cryptol-remote-api` executable and will be\n   used for the duration of the script.\n2. If the environment variable ``CRYPTOL_SERVER_URL`` is set, it is assumed to be\n   the URL for a running Cryptol server in ``http`` mode and will be connected to.\n   (N.B., this can be a local server or a server running in a docker image.)\n3. If an executable ``cryptol-remote-api`` is available on the ``PATH`` it is\n    assumed to be a Cryptol server and will be used for the duration of the script.\n\nAdditional arguments and options are documented with the function.\n\nNotably, the `reset_server` keyword can be used to connect to a running server\nand reset it, ensuring states from previous scripts have been cleared. E.g.,\n`cryptol.connect(reset_server=True)`.\n\n\n## Acquiring a Cryptol Server\n\nThere are several ways a server executable can be obtained.\n\n### Server executables\n\nAn executable of the server is now included in each release of Cryptol.\n\nNightly server builds can be found as `Artifacts` of the [Nightly\nBuilds](https://github.com/GaloisInc/saw-script/actions/workflows/nightly.yml)\ngithub action. I.e., go to the `Nightly Builds` Github Action, click on a\nsuccessful build, scroll to the bottom and under `Artifacts` a Linux, Windows,\nand MacOS tarball will be listed.\n\nNightly Docker images of the server can be found under the\n[Packages](https://github.com/orgs/GaloisInc/packages?repo_name=cryptol) section\nof the Cryptol github repository.\n\n### Server docker images\n\nRelease docker images for the Cryptol server are distributed with Cryptol\nreleases; nightly Cryptol servers are available under the\n[Packages](https://github.com/orgs/GaloisInc/packages) section of the Cryptol repository.\n\nThese images are set up to run as HTTP `cryptol-remote-api` servers, e.g.:\n\n```\ndocker run --name=cryptol-remote-api -d \\\n  -p 8080:8080 \\\n  ghcr.io/galoisinc/cryptol-remote-api:nightly-portable\n```\n\nThe `-v` option to `docker run` can be used to load files into the docker\nserver\'s working directory so they can be loaded into the server at the request\nof python scripts. E.g., `-v PATH_TO_FILES:/home/cryptol/files/` will upload the\ncontents of the host machine\'s directory `PATH_TO_FILES` to the\n`/home/cryptol/files/` directory in the docker container, which corresponds to the\nrelative path `files/` for the Cryptol server. (If desired, it can be useful to\nplace files in a location in the Docker container such that the same relative\npaths in scripts refer to the same files in the host machine and docker\ncontainer.)\n\n### Building from Source\n\nIf this repository is checked out and the build directions are successfully run,\n`cabal v2-exec which cryptol-remote-api` should indicate where the server executable has\nbeen stored by `cabal`.\n\nAlternatively `cabal v2-install cryptol-remote-api` should install the server\nexecutable into the user\'s `~/.cabal/bin` directory (or similar), which (if\nconfigured properly) should then appear as `cryptol-remote-api` in a user\'s `PATH`.\n\n\n# Running Python Cryptol scripts\n\nOnce the server is setup and any path variables are setup as desired, the\nPython (>= v3.7) client can be installed using\n[`poetry`](https://python-poetry.org/docs/#installation) as follows:\n\n```\n$ cd cryptol-remote-api/python\n$ poetry install\n```\n\nThen the tests or individual scripts can be run as follows:\n```\n$ poetry run python -m unittest discover tests/cryptol\n$ poetry run python tests/cryptol/test_cryptol_api.py\n```\n\nIf leveraging environment variables is undesirable, the scripts themselves can\nspecify a command to launch the server, e.g.:\n\n```\ncryptol.connect(COMMAND)\n```\n\nwhere `COMMAND` is a command to launch a new Cryptol server in socket mode.\n\nOr a server URL can be specified directly in the script, e.g.:\n\n```\ncryptol.connect(url=URL)\n```\n\nwhere `URL` is a URL for a running Cryptol server in HTTP mode.\n\n## Running Cryptol Scripts from a clean server state\n\nTo ensure any previous server state is cleared when running a Cryptol Python script\nagainst a persistent server (e.g., one running in HTTP mode in a different process),\nthe `reset_server` keyword can be passed to `cryptol.connect()`. E.g.,\n\n```\ncryptol.connect(url="http://localhost:8080/", reset_server=True)\n```\n\nwill connect to a Cryptol server running at `http://localhost:8080/` and will\nguarantee any previous state on the server is cleared.\n',
-    'author': 'Galois, Inc.',
-    'author_email': 'cryptol-team@galois.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.0,<4',
-}
-
-
-setup(**setup_kwargs)
```

