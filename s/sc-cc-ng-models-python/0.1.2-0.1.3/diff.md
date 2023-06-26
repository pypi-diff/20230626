# Comparing `tmp/sc_cc_ng_models_python-0.1.2.tar.gz` & `tmp/sc_cc_ng_models_python-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc_cc_ng_models_python-0.1.2.tar", max compression
+gzip compressed data, was "sc_cc_ng_models_python-0.1.3.tar", max compression
```

## Comparing `sc_cc_ng_models_python-0.1.2.tar` & `sc_cc_ng_models_python-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      576 2023-06-26 14:02:21.217632 sc_cc_ng_models_python-0.1.2/README.md
--rw-r--r--   0        0        0      425 2023-06-26 15:24:31.142183 sc_cc_ng_models_python-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    10285 2023-06-26 15:26:33.437183 sc_cc_ng_models_python-0.1.2/sc_cc_ng_models_python/__init__.py
--rw-r--r--   0        0        0      979 1970-01-01 00:00:00.000000 sc_cc_ng_models_python-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      576 2023-06-26 14:02:21.217632 sc_cc_ng_models_python-0.1.3/README.md
+-rw-r--r--   0        0        0      425 2023-06-26 19:27:26.044549 sc_cc_ng_models_python-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    10367 2023-06-26 19:26:32.794261 sc_cc_ng_models_python-0.1.3/sc_cc_ng_models_python/__init__.py
+-rw-r--r--   0        0        0      979 1970-01-01 00:00:00.000000 sc_cc_ng_models_python-0.1.3/PKG-INFO
```

### Comparing `sc_cc_ng_models_python-0.1.2/README.md` & `sc_cc_ng_models_python-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sc_cc_ng_models_python-0.1.2/sc_cc_ng_models_python/__init__.py` & `sc_cc_ng_models_python-0.1.3/sc_cc_ng_models_python/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,28 +156,29 @@
 	WLTP_SERVING_WEIGHT_MIN = "WLTP_SERVING_WEIGHT_MIN"
 	WLTP_TOTAL_WEIGHT_MAX = "WLTP_TOTAL_WEIGHT_MAX"
 	WLTP_TOTAL_WEIGHT_MIN = "WLTP_TOTAL_WEIGHT_MIN"
 
 
 @dataclass(frozen=True, eq=True)
 class BitVal:
-    context: List[str]
-    value: Union[str, float]
+    context:    List[str]
+    value:      Union[str, float]
+    reason:     List[str] = field(default_factory=lambda: [])
         
     def __hash__(self):
         return hash(self.as_string())
     
     def __eq__(self, other) -> bool:
         return self.__hash__() == other.__hash__()
     
     def sha256(self) -> str:
         return sha256(self.as_string().encode('utf8')).hexdigest()
     
     def as_string(self) -> str:
-        return "".join(self.context)+str(self.value)
+        return "".join(self.context+self.reason)+str(self.value)
 
     @staticmethod
     def from_dict(d: dict) -> "BitVal":
         return BitVal(
             context=d["context"],
             value=d["value"],
         )
```

### Comparing `sc_cc_ng_models_python-0.1.2/PKG-INFO` & `sc_cc_ng_models_python-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-cc-ng-models-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Rikard Olsson
 Author-email: rikard@thryselius.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

