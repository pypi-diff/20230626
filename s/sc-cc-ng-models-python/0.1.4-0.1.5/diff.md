# Comparing `tmp/sc_cc_ng_models_python-0.1.4.tar.gz` & `tmp/sc_cc_ng_models_python-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc_cc_ng_models_python-0.1.4.tar", max compression
+gzip compressed data, was "sc_cc_ng_models_python-0.1.5.tar", max compression
```

## Comparing `sc_cc_ng_models_python-0.1.4.tar` & `sc_cc_ng_models_python-0.1.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      576 2023-06-26 14:02:21.217632 sc_cc_ng_models_python-0.1.4/README.md
--rw-r--r--   0        0        0      425 2023-06-26 19:35:47.898773 sc_cc_ng_models_python-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    10569 2023-06-26 19:35:29.874303 sc_cc_ng_models_python-0.1.4/sc_cc_ng_models_python/__init__.py
--rw-r--r--   0        0        0      979 1970-01-01 00:00:00.000000 sc_cc_ng_models_python-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      576 2023-06-26 14:02:21.217632 sc_cc_ng_models_python-0.1.5/README.md
+-rw-r--r--   0        0        0      425 2023-06-26 19:37:49.115640 sc_cc_ng_models_python-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    10577 2023-06-26 19:37:35.495259 sc_cc_ng_models_python-0.1.5/sc_cc_ng_models_python/__init__.py
+-rw-r--r--   0        0        0      979 1970-01-01 00:00:00.000000 sc_cc_ng_models_python-0.1.5/PKG-INFO
```

### Comparing `sc_cc_ng_models_python-0.1.4/README.md` & `sc_cc_ng_models_python-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `sc_cc_ng_models_python-0.1.4/sc_cc_ng_models_python/__init__.py` & `sc_cc_ng_models_python-0.1.5/sc_cc_ng_models_python/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
     def to_dict(self) -> dict:
         return {
             "context": self.context,
             "value": self.value,
         }
 
     def to_string(self, join_on: str = ": ") -> str:
-        ctx_str = ", ".join(map(lambda ctx: " ".join(ctx.split("_")), self.context + self.reason))
+        ctx_str = ", ".join(map(lambda ctx: " ".join(ctx.lower().split("_")), self.context + self.reason))
         return f"{ctx_str}{join_on}{self.value}"
 
 class ContextRelation(Enum):
     ALL = "ALL"
     ANY = "ANY"
 
 @dataclass
```

### Comparing `sc_cc_ng_models_python-0.1.4/PKG-INFO` & `sc_cc_ng_models_python-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-cc-ng-models-python
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Rikard Olsson
 Author-email: rikard@thryselius.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

