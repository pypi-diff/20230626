# Comparing `tmp/gundi_core-1.0.4.tar.gz` & `tmp/gundi_core-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gundi_core-1.0.4.tar", max compression
+gzip compressed data, was "gundi_core-1.0.5.tar", max compression
```

## Comparing `gundi_core-1.0.4.tar` & `gundi_core-1.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       40 2023-06-14 17:07:47.722189 gundi_core-1.0.4/README.md
--rw-r--r--   0        0        0        0 2023-06-14 20:35:09.913772 gundi_core-1.0.4/gundi_core/__init__.py
--rw-r--r--   0        0        0      114 2023-06-14 18:33:55.875739 gundi_core-1.0.4/gundi_core/schemas/__init__.py
--rw-r--r--   0        0        0    13847 2023-06-14 19:41:05.310697 gundi_core-1.0.4/gundi_core/schemas/v1.py
--rw-r--r--   0        0        0    10689 2023-06-22 20:32:23.242615 gundi_core-1.0.4/gundi_core/schemas/v2.py
--rw-r--r--   0        0        0      329 2023-06-22 20:32:33.739034 gundi_core-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 gundi_core-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0       40 2023-06-14 17:07:47.722189 gundi_core-1.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 20:35:09.913772 gundi_core-1.0.5/gundi_core/__init__.py
+-rw-r--r--   0        0        0      114 2023-06-14 18:33:55.875739 gundi_core-1.0.5/gundi_core/schemas/__init__.py
+-rw-r--r--   0        0        0    13847 2023-06-14 19:41:05.310697 gundi_core-1.0.5/gundi_core/schemas/v1.py
+-rw-r--r--   0        0        0    11663 2023-06-26 12:53:21.708050 gundi_core-1.0.5/gundi_core/schemas/v2.py
+-rw-r--r--   0        0        0      329 2023-06-26 14:58:24.752760 gundi_core-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 gundi_core-1.0.5/PKG-INFO
```

### Comparing `gundi_core-1.0.4/gundi_core/schemas/v1.py` & `gundi_core-1.0.5/gundi_core/schemas/v1.py`

 * *Files identical despite different names*

### Comparing `gundi_core-1.0.4/gundi_core/schemas/v2.py` & `gundi_core-1.0.5/gundi_core/schemas/v2.py`

 * *Files 5% similar despite different names*

```diff
@@ -339,11 +339,44 @@
     status: Optional[Dict[str, Any]] = Field(  # ToDo: Review once Activity/Monitoring is implemented
         {},
         example="{}",
         description="A json object with detailed information about the integration health status",
     )
 
 
+# Earth Ranger Supported Actions & Configuration Schemas
+class EarthRangerActions(str, Enum):
+    AUTHENTICATE = "auth"
+    PUSH_EVENT = "push_event"
+    # ToDo. Add more as we support them
+
+
+class ERAuthActionConfig(BaseModel):
+    username: Optional[str] = Field(
+        "",
+        example="user@pamdas.org",
+        description="Username used to authenticate against Earth Ranger API",
+    )
+    password: Optional[str] = Field(
+        "",
+        example="passwd1234abc",
+        description="Password used to authenticate against Earth Ranger API",
+    )
+    token: Optional[str] = Field(
+        "",
+        example="1b4c1e9c-5ee0-44db-c7f1-177ede2f854a",
+        description="Token used to authenticate against Earth Ranger API",
+    )
+
+
+class ERPushEventActionConfig(BaseModel):
+    event_type: Optional[str] = Field(
+        "",
+        example="animal_sighting",
+        description="Event type to be applied to event sent to Earth Ranger (Optional).",
+    )
+
+
 models_by_stream_type = {
     StreamPrefixEnum.event: Event,
     StreamPrefixEnum.attachment: Attachment,
 }
```

### Comparing `gundi_core-1.0.4/PKG-INFO` & `gundi_core-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gundi-core
-Version: 1.0.4
+Version: 1.0.5
 Summary: 
 Author: Mariano M
 Author-email: marianom@earthranger.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

