# Comparing `tmp/delphai_fastapi-0.1.1.tar.gz` & `tmp/delphai_fastapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delphai_fastapi-0.1.1.tar", max compression
+gzip compressed data, was "delphai_fastapi-0.1.2.tar", max compression
```

## Comparing `delphai_fastapi-0.1.1.tar` & `delphai_fastapi-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-06-19 14:48:28.928465 delphai_fastapi-0.1.1/delphai_fastapi/__init__.py
--rw-r--r--   0        0        0     2521 2023-06-19 14:48:28.928465 delphai_fastapi-0.1.1/delphai_fastapi/app.py
--rw-r--r--   0        0        0     3173 2023-06-19 14:48:28.928465 delphai_fastapi-0.1.1/delphai_fastapi/auth.py
--rw-r--r--   0        0        0        0 2023-06-19 14:48:28.928465 delphai_fastapi-0.1.1/delphai_fastapi/companies/__init__.py
--rw-r--r--   0        0        0     2915 2023-06-19 14:48:28.928465 delphai_fastapi-0.1.1/delphai_fastapi/companies/models.py
--rw-r--r--   0        0        0      375 2023-06-19 14:48:28.928465 delphai_fastapi-0.1.1/delphai_fastapi/decorators.py
--rw-r--r--   0        0        0      821 2023-06-19 14:48:28.928465 delphai_fastapi-0.1.1/delphai_fastapi/models.py
--rw-r--r--   0        0        0     1342 2023-06-19 14:48:28.928465 delphai_fastapi-0.1.1/delphai_fastapi/types.py
--rw-r--r--   0        0        0      476 2023-06-19 14:49:08.581241 delphai_fastapi-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      755 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.1/setup.py
--rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-26 08:29:07.579788 delphai_fastapi-0.1.2/delphai_fastapi/__init__.py
+-rw-r--r--   0        0        0     2521 2023-06-26 08:29:07.579788 delphai_fastapi-0.1.2/delphai_fastapi/app.py
+-rw-r--r--   0        0        0     3173 2023-06-26 08:29:07.579788 delphai_fastapi-0.1.2/delphai_fastapi/auth.py
+-rw-r--r--   0        0        0        0 2023-06-26 08:29:07.579788 delphai_fastapi-0.1.2/delphai_fastapi/companies/__init__.py
+-rw-r--r--   0        0        0     3266 2023-06-26 08:29:07.579788 delphai_fastapi-0.1.2/delphai_fastapi/companies/models.py
+-rw-r--r--   0        0        0      375 2023-06-26 08:29:07.579788 delphai_fastapi-0.1.2/delphai_fastapi/decorators.py
+-rw-r--r--   0        0        0     1619 2023-06-26 08:29:07.579788 delphai_fastapi-0.1.2/delphai_fastapi/models.py
+-rw-r--r--   0        0        0     1342 2023-06-26 08:29:07.579788 delphai_fastapi-0.1.2/delphai_fastapi/types.py
+-rw-r--r--   0        0        0      476 2023-06-26 08:29:49.876780 delphai_fastapi-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      755 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.2/setup.py
+-rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.2/PKG-INFO
```

### Comparing `delphai_fastapi-0.1.1/delphai_fastapi/app.py` & `delphai_fastapi-0.1.2/delphai_fastapi/app.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.1/delphai_fastapi/auth.py` & `delphai_fastapi-0.1.2/delphai_fastapi/auth.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.1/delphai_fastapi/companies/models.py` & `delphai_fastapi-0.1.2/delphai_fastapi/companies/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict, List, Optional
 
 from fastapi_camelcase import CamelModel
 from pydantic import Field
 
 from ..types import ObjectId
-from ..models import Location
+from ..models import Location, Source
 
 
 class EmployeeCount(CamelModel):
     min: Optional[int] = Field(
         description="Bottom range of the employee count interval", example=11
     )
     max: Optional[int] = Field(
@@ -36,14 +36,16 @@
 class CompanyRevenue(CamelModel):
     currency: Optional[str] = Field(
         description="Currency of revenue number", example="EUR"
     )
     annual: Optional[int] = Field(
         description="Annual revenue number for specified year", example=5000000
     )
+    year: Optional[int] = Field(description="Year of revenue number", example=2022)
+    source: Source
 
 
 class Company(CamelModel):
     id: ObjectId = Field(..., description="Internal company ID")
     name: Optional[str] = Field(description="Name of the company", example="delphai")
     url: str = Field(..., description="Webpage of the company", example="delphai.com")
     descriptions: Optional[Dict[str, CompanyDescription]]
@@ -57,14 +59,20 @@
         description="Company revenue with currency"
     )
     products: Optional[List[str]] = Field(
         description="List of company products", example=["Software"]
     )
 
 
+class ProjectsCompany(CamelModel):
+    company: Company
+    custom_labels: Optional[List[str]] = Field(description="Custom labels assigned by user")
+    assigned_by: str = Field(description="By whom the company was added to the project")
+
+
 class CompaniesSearchResult(CamelModel):
     company: Company
     score: float = Field(default=0, description="Search score", example="202.35745")
     snippets: List[str] = Field(
         default=[],
         description="Snippets containing query keywords",
         example=[
```

### Comparing `delphai_fastapi-0.1.1/delphai_fastapi/types.py` & `delphai_fastapi-0.1.2/delphai_fastapi/types.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.1/setup.py` & `delphai_fastapi-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['bson>=0.5.10,<0.6.0',
  'delphai-utils[config]>=3,<4',
  'fastapi-camelcase>=1.0.5,<2.0.0',
  'fastapi>=0.95,<0.96']
 
 setup_kwargs = {
     'name': 'delphai-fastapi',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Package for fastAPI models',
     'long_description': 'None',
     'author': 'Berinike Tech',
     'author_email': 'berinike@delphai.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `delphai_fastapi-0.1.1/PKG-INFO` & `delphai_fastapi-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delphai-fastapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Package for fastAPI models
 Author: Berinike Tech
 Author-email: berinike@delphai.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

