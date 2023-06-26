# Comparing `tmp/sc_cc_ng_sdk_python-0.1.2.tar.gz` & `tmp/sc_cc_ng_sdk_python-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc_cc_ng_sdk_python-0.1.2.tar", max compression
+gzip compressed data, was "sc_cc_ng_sdk_python-0.1.3.tar", max compression
```

## Comparing `sc_cc_ng_sdk_python-0.1.2.tar` & `sc_cc_ng_sdk_python-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-26 13:45:09.675633 sc_cc_ng_sdk_python-0.1.2/README.md
--rw-r--r--   0        0        0      530 2023-06-26 15:49:36.490654 sc_cc_ng_sdk_python-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5110 2023-06-26 15:48:57.723020 sc_cc_ng_sdk_python-0.1.2/sc_cc_ng_sdk_python/__init__.py
--rw-r--r--   0        0        0      497 1970-01-01 00:00:00.000000 sc_cc_ng_sdk_python-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-26 13:45:09.675633 sc_cc_ng_sdk_python-0.1.3/README.md
+-rw-r--r--   0        0        0      530 2023-06-26 19:39:39.183266 sc_cc_ng_sdk_python-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6286 2023-06-26 19:37:08.166313 sc_cc_ng_sdk_python-0.1.3/sc_cc_ng_sdk_python/__init__.py
+-rw-r--r--   0        0        0      497 1970-01-01 00:00:00.000000 sc_cc_ng_sdk_python-0.1.3/PKG-INFO
```

### Comparing `sc_cc_ng_sdk_python-0.1.2/pyproject.toml` & `sc_cc_ng_sdk_python-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "sc-cc-ng-sdk-python"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Rikard Olsson <rikard@thryselius.se>"]
 readme = "README.md"
 packages = [{include = "sc_cc_ng_sdk_python"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-sc-cc-ng-models-python = "^0.1.2"
+sc-cc-ng-models-python = "^0.1.5"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.0.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `sc_cc_ng_sdk_python-0.1.2/sc_cc_ng_sdk_python/__init__.py` & `sc_cc_ng_sdk_python-0.1.3/sc_cc_ng_sdk_python/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,34 @@
 from dataclasses import dataclass, asdict
 from requests import post
 from sc_cc_ng_models_python import ContextFilter, BitVal
-from typing import List, Optional
+from typing import List, Optional, Any
 from enum import Enum
 
 @dataclass
-class DictResult:
+class Result:
 
     """
-        A result object, containing meta data if everything was ok else an error.
+        A result object, containing data if everything was ok else an error.
     """
 
-    data:   Optional[List[dict]]    = None
-    error:  Optional[str]           = None
+    data:   Optional[Any]   = None
+    error:  Optional[str]   = None
 
-@dataclass
-class ListResult:
-
-    """
-        A result object, containing meta data if everything was ok else an error.
-    """
-
-    data:   Optional[List[BitVal]]  = None
-    error:  Optional[str]           = None
 
 @dataclass
 class SCNG:
 
     url: str
 
-    def to_dict(
+    def to_dict_list(
         self, 
         tokens_list: List[List[str]],
         context_filter: Optional[ContextFilter] = None,
-    ) -> DictResult:
+    ) -> Result:
 
         """
             Converts lists of tokens to a list of dictionaries, containing
             all matching meta data to those tokens. If no meta data was found
             for a combination of tokens, the dictionary will be empty.
 
             :param tokens_list: A list of lists of tokens.
@@ -68,27 +59,27 @@
                         "contextFilter": context_filter.to_dict(),
                     }
                 },
             )
             if response.status_code == 200:
                 json = response.json()
                 if "errors" in json:
-                    return DictResult(error=json["errors"])
+                    return Result(error=json["errors"])
                 else:
-                    return DictResult(data=response.json()['data']['tokensListBasedContentAsDict'])
+                    return Result(data=response.json()['data']['tokensListBasedContentAsDict'])
             else:
-                return DictResult(error=response.text)
+                return Result(error=response.text)
         except Exception as e:
-            return DictResult(error=str(e))
+            return Result(error=str(e))
     
-    def to_list(
+    def to_bit_list(
         self,
         tokens_list: List[List[str]],
         context_filter: Optional[ContextFilter] = None,
-    ) -> ListResult:
+    ) -> Result:
 
         """
             Converts lists of tokens to a list of bit values, containing
             all matching meta data to those tokens. If no meta data was found
             for a combination of tokens, the list will be empty.
 
             :param tokens_list: A list of lists of tokens.
@@ -111,42 +102,84 @@
                         ) {
                             tokenListBasedContent(
                                 tokenList: $tokenList
                                 contextFilter: $contextFilter
                             ) {
                                 context
                                 value
+                                reason
                             }
                         }
                     """,
                     "variables": {
                         "tokenList": tokens_list,
                         "contextFilter": context_filter.to_dict(),
                     }
                 },
             )
             if response.status_code == 200:
                 json = response.json()
                 if "errors" in json:
-                    return ListResult(error=json["errors"])
+                    return Result(error=json["errors"])
                 else:
-                    return ListResult(
+                    return Result(
                         data=list(
                             map(
                                 lambda xs: list(
                                     map(
                                         lambda x: BitVal(
                                             context=x['context'],
                                             value=x['value'],
+                                            reason=x['reason'],
                                         ),
                                         xs
                                     )
                                 ),
                                 response.json()['data']['tokenListBasedContent']
                             )
                         )
                     )
             else:
-                return ListResult(error=response.text)
+                return Result(error=response.text)
         except Exception as e:
-            return ListResult(error=str(e))
+            return Result(error=str(e))
+
+    def to_string_list(
+        self, 
+        tokens_list: list,
+        context_filter: Optional[ContextFilter] = None,
+    ) -> Result:
+            
+        """
+            Converts lists of tokens to a list of strings, containing
+            all matching meta data to those tokens. If no meta data was found
+            for a combination of tokens, the list will be empty.
 
+            :param tokens_list: A list of lists of tokens.
+            :param context_filter: A context filter object.
+
+            :return: A result object.
+        """
+
+        try:
+            internal_result = self.to_bit_list(
+                tokens_list=tokens_list,
+                context_filter=context_filter,
+            )
+            if internal_result.error is None:
+                return Result(
+                    data=list(
+                        map(
+                            lambda xs: list(
+                                map(
+                                    lambda x: x.to_string(),
+                                    xs
+                                )
+                            ),
+                            internal_result.data
+                        )
+                    )
+                )
+            else:
+                return internal_result
+        except Exception as e:
+            return Result(error=str(e))
```

