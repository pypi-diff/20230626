# Comparing `tmp/sui_brownie-1.0.8-py3-none-any.whl.zip` & `tmp/sui_brownie-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 28047 bytes, number of entries: 16
+Zip file size: 28137 bytes, number of entries: 16
 -rw-r--r--  2.0 unx       10 b- defN 22-Dec-02 09:41 sui_brownie/MANIFEST.in
 -rw-r--r--  2.0 unx      878 b- defN 23-Apr-01 13:03 sui_brownie/README.md
 -rw-r--r--  2.0 unx       38 b- defN 23-Apr-11 02:45 sui_brownie/__init__.py
 -rw-r--r--  2.0 unx     2514 b- defN 23-Apr-01 12:52 sui_brownie/account.py
--rw-r--r--  2.0 unx    12144 b- defN 23-Apr-21 09:58 sui_brownie/bcs.py
+-rw-r--r--  2.0 unx    12351 b- defN 23-Jun-26 10:12 sui_brownie/bcs.py
 -rw-r--r--  2.0 unx     4326 b- defN 23-Apr-01 12:53 sui_brownie/ed25519.py
 -rw-r--r--  2.0 unx    10047 b- defN 22-Dec-02 09:41 sui_brownie/parallelism.py
--rw-r--r--  2.0 unx    95775 b- defN 23-Jun-26 08:15 sui_brownie/sui_brownie.py
+-rw-r--r--  2.0 unx    96273 b- defN 23-Jun-26 10:12 sui_brownie/sui_brownie.py
 -rw-r--r--  2.0 unx    32439 b- defN 23-Apr-19 08:03 sui_brownie/sui_client.py
 -rw-r--r--  2.0 unx      140 b- defN 22-Dec-02 09:41 sui_brownie/sui_config.template.yaml
 -rw-r--r--  2.0 unx       19 b- defN 22-Dec-02 09:41 sui_brownie/sui_keystore.template.keystore
 -rw-r--r--  2.0 unx      866 b- defN 23-Apr-11 02:45 sui_brownie/utils.py
--rw-r--r--  2.0 unx     1002 b- defN 23-Jun-26 08:20 sui_brownie-1.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 08:20 sui_brownie-1.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-26 08:20 sui_brownie-1.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1297 b- defN 23-Jun-26 08:20 sui_brownie-1.0.8.dist-info/RECORD
-16 files, 161599 bytes uncompressed, 25913 bytes compressed:  84.0%
+-rw-r--r--  2.0 unx     1002 b- defN 23-Jun-26 10:12 sui_brownie-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 10:12 sui_brownie-1.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-26 10:12 sui_brownie-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1297 b- defN 23-Jun-26 10:12 sui_brownie-1.0.9.dist-info/RECORD
+16 files, 162304 bytes uncompressed, 26003 bytes compressed:  84.0%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: sui_brownie/sui_keystore.template.keystore
 Comment: 
 
 Filename: sui_brownie/utils.py
 Comment: 
 
-Filename: sui_brownie-1.0.8.dist-info/METADATA
+Filename: sui_brownie-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: sui_brownie-1.0.8.dist-info/WHEEL
+Filename: sui_brownie-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: sui_brownie-1.0.8.dist-info/top_level.txt
+Filename: sui_brownie-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: sui_brownie-1.0.8.dist-info/RECORD
+Filename: sui_brownie-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sui_brownie/bcs.py

```diff
@@ -99,14 +99,24 @@
     @property
     def encode(self) -> bytes:
         stream = io.BytesIO()
         stream.write(self.v0.to_bytes(8, "little", signed=False))
         return stream.getvalue()
 
 
+class String:
+    def __init__(self, v0: str):
+        assert isinstance(v0, str)
+        self.v0 = v0
+
+    @property
+    def encode(self) -> bytes:
+        return uleb128(len(self.v0)) + self.v0.encode()
+
+
 class U128:
     def __init__(self, v0: int):
         assert v0 <= MAX_U128
         assert isinstance(v0, int)
         self.v0 = v0
 
     @property
```

## sui_brownie/sui_brownie.py

```diff
@@ -413,29 +413,32 @@
     @classmethod
     def prepare_object_info(cls, call_arg, parameters):
         assert len(call_arg) == len(parameters)
         object_ids = []
         for i in range(len(call_arg)):
             param_type = parameters[i]
             if isinstance(param_type, dict):
+                if "Struct" in param_type and param_type["Struct"]["address"] == "0x1" and param_type["Struct"][
+                    "module"] == "string" and param_type["Struct"]["name"] == "String":
+                    continue
                 if ("Reference" in param_type or "MutableReference" in param_type or "Struct" in param_type) \
                         and isinstance(call_arg[i], str):
                     object_ids.append(call_arg[i])
                 if ("Reference" in param_type or "MutableReference" in param_type or "Struct" in param_type) \
                         and isinstance(call_arg[i], list):
                     object_ids.extend(call_arg[i])
                 elif "Vector" in param_type and "Struct" in param_type["Vector"]:
                     assert isinstance(call_arg[i], list)
                     object_ids.extend(call_arg[i])
 
         return cls.get_objects(object_ids)
 
     @classmethod
     def generate_pure_value(cls, param_type, data):
-        if param_type in ["Bool", "U8", "U64", "U128", "Address", "Signer", "U16", "U32", "U256"]:
+        if param_type in ["Bool", "U8", "U64", "U128", "Address", "Signer", "U16", "U32", "U256", "String"]:
             return getattr(bcs, param_type)(data)
         elif isinstance(param_type, dict) and "Vector" in param_type:
             output = []
             assert isinstance(data, list), f"{param_type}:{data}"
             for i in range(len(data)):
                 output.append(cls.generate_pure_value(param_type["Vector"], data[i]))
             return output
@@ -465,14 +468,18 @@
                                  ObjectID(data["objectId"]),
                                  SequenceNumber(int(data["version"])),
                                  ObjectDigest(data["digest"])
                              ))
 
     @classmethod
     def generate_call_arg(cls, param_type, data, object_infos):
+        if isinstance(param_type, dict) and "Struct" in param_type and param_type["Struct"]["address"] == "0x1" \
+                and param_type["Struct"]["module"] == "string" and param_type["Struct"]["name"] == "String":
+            param_type = "String"
+
         if isinstance(param_type, dict) and \
                 ("MutableReference" in param_type or
                  "Reference" in param_type or
                  "Struct" in param_type):
             if "Vector" in param_type.get("MutableReference", {}) or "Vector" in param_type.get("Reference",
                                                                                                 {}) or "Vector" in param_type.get(
                 "Struct", {}):
```

## Comparing `sui_brownie-1.0.8.dist-info/METADATA` & `sui_brownie-1.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sui-brownie
-Version: 1.0.8
+Version: 1.0.9
 Summary: Sui Package Tool
 Home-page: https://github.com/OmniBTC/DolaProtocol/blob/main/utils
 Author: DaiWei
 Author-email: dw1253464613@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

## Comparing `sui_brownie-1.0.8.dist-info/RECORD` & `sui_brownie-1.0.9.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 sui_brownie/MANIFEST.in,sha256=BzExY9sw9x0Pqk6SYHuMRRvYS-cm75AxBOBjsYGFfU4,10
 sui_brownie/README.md,sha256=-7DxT6cGHbWLr_VufOEwIzl4Vtojp5dZc_r89lwnK3o,878
 sui_brownie/__init__.py,sha256=ROrbn7qi0haZjB8FG5JqXpD5mQ6qQPDNOwe0-rPnKeM,38
 sui_brownie/account.py,sha256=suZRI__kDNhyuoCZ9_q4mIV673lJDz0jgj0HyEj_hsQ,2514
-sui_brownie/bcs.py,sha256=8LwJihqmjLGwtzq87XKAQhE7ZgxiRDUsUYRbK6yRy7s,12144
+sui_brownie/bcs.py,sha256=KZ-hx82tKH6MyMYXZqeh1JOSbrEBRHqDgWGOLJQxiXc,12351
 sui_brownie/ed25519.py,sha256=8hLHtC21og60B3MzXi4JmdQoOCbUutExyQIJhypJ9dg,4326
 sui_brownie/parallelism.py,sha256=Thh7TUrRU1fn47lNTF30RrcL5lBPBeMT2DX9A_swXDg,10047
-sui_brownie/sui_brownie.py,sha256=zMFLHNAOSoGArjL4J8AF4FbCE1ApzVZC5E6vrFFzHGs,95775
+sui_brownie/sui_brownie.py,sha256=xSpnsFpR6Hll6-UBRpHn2-LVwLN7YusX2D2GcoXeTYI,96273
 sui_brownie/sui_client.py,sha256=Epyu5pXAI6jl_L-lzBg4gnNLYQVjdQTZ8kR4YrJfnqk,32439
 sui_brownie/sui_config.template.yaml,sha256=Qa6n48nf4qeLDhZnpVNjZJIYDm8jYFs7dVLCyLjxMTs,140
 sui_brownie/sui_keystore.template.keystore,sha256=dIQsJL_H6FdnGlET9u5NYXSmjTc1-8dk8wZWKrzcLOM,19
 sui_brownie/utils.py,sha256=bttovGstKoozRoMvzYFOFs_z73aled7UFbNBDPxX9Uo,866
-sui_brownie-1.0.8.dist-info/METADATA,sha256=BBXH_UnYIESnQ9LOC_EaKTNLdtOy9VdowjIot7k30qo,1002
-sui_brownie-1.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-sui_brownie-1.0.8.dist-info/top_level.txt,sha256=Rh3-9xCv23H03EevKs1qJcZsUKCgFfOoxlhaDld3TdE,12
-sui_brownie-1.0.8.dist-info/RECORD,,
+sui_brownie-1.0.9.dist-info/METADATA,sha256=IvCQQyv1WZKkq-5KAIps2w9S-9r1uMQbJWwGtPo1UlE,1002
+sui_brownie-1.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+sui_brownie-1.0.9.dist-info/top_level.txt,sha256=Rh3-9xCv23H03EevKs1qJcZsUKCgFfOoxlhaDld3TdE,12
+sui_brownie-1.0.9.dist-info/RECORD,,
```

