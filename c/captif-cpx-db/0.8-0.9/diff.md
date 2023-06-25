# Comparing `tmp/captif_cpx_db-0.8.tar.gz` & `tmp/captif_cpx_db-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captif_cpx_db-0.8.tar", max compression
+gzip compressed data, was "captif_cpx_db-0.9.tar", max compression
```

## Comparing `captif_cpx_db-0.8.tar` & `captif_cpx_db-0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1084 2023-06-21 21:39:41.054948 captif_cpx_db-0.8/LICENSE
--rw-r--r--   0        0        0       16 2023-06-21 21:39:41.054948 captif_cpx_db-0.8/README.md
--rw-r--r--   0        0        0       20 2023-06-21 21:39:41.054948 captif_cpx_db-0.8/captif_cpx_db/__init__.py
--rw-r--r--   0        0        0    27030 2023-06-21 21:39:41.058948 captif_cpx_db-0.8/captif_cpx_db/models.py
--rw-r--r--   0        0        0      504 2023-06-21 21:39:41.058948 captif_cpx_db-0.8/pyproject.toml
--rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 captif_cpx_db-0.8/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-22 23:21:17.142681 captif_cpx_db-0.9/LICENSE
+-rw-r--r--   0        0        0       16 2023-06-22 23:21:17.142681 captif_cpx_db-0.9/README.md
+-rw-r--r--   0        0        0      334 2023-06-22 23:21:17.142681 captif_cpx_db-0.9/captif_cpx_db/__init__.py
+-rw-r--r--   0        0        0    27546 2023-06-22 23:21:17.142681 captif_cpx_db-0.9/captif_cpx_db/models.py
+-rw-r--r--   0        0        0      523 2023-06-22 23:21:17.142681 captif_cpx_db-0.9/pyproject.toml
+-rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 captif_cpx_db-0.9/PKG-INFO
```

### Comparing `captif_cpx_db-0.8/LICENSE` & `captif_cpx_db-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `captif_cpx_db-0.8/captif_cpx_db/models.py` & `captif_cpx_db-0.9/captif_cpx_db/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from datetime import date as date_
 from pydantic import condecimal, validator
+from shapely.wkt import loads
 from sqlalchemy import ForeignKeyConstraint as ForeignKeyConstraint_
 from sqlmodel import Field, SQLModel, Relationship
 from typing import List, Optional
 
 
 def ForeignKeyConstraint(*args, **kwargs):
     return ForeignKeyConstraint_(
@@ -575,21 +576,35 @@
     valid: bool = Field(
         nullable=False,
         description=(
             "indicates whether the road segment results are valid or not, "
             "based on the speed and any event flags"
         ),
     )
+    geometry: str = Field(
+        nullable=False,
+        description="RAMM centreline geometry of the road segment",
+    )
 
     wheel_bay_details: List["SegmentWheelBayDetails"] = Relationship()
 
     @validator("start_m", "end_m", "length_m", pre=True)
     def round_1(cls, v):
         return round(v, 1) if v is not None else None
 
+    @validator("geometry")
+    def validate_linestring(cls, v):
+        try:
+            linestring = loads(v)
+            if not linestring.is_valid or linestring.geom_type != "LineString":
+                raise ValueError("Invalid WKT LINESTRING")
+        except Exception as e:
+            raise ValueError("Invalid WKT LINESTRING") from e
+        return v
+
 
 class SegmentWheelBayDetails(SQLModel, table=True):
     """
     Segment-level (results set) wheel bay details.
     """
 
     __tablename__ = "segment_wheel_bay_details"
```

