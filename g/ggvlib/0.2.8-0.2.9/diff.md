# Comparing `tmp/ggvlib-0.2.8.tar.gz` & `tmp/ggvlib-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ggvlib-0.2.8.tar", max compression
+gzip compressed data, was "ggvlib-0.2.9.tar", max compression
```

## Comparing `ggvlib-0.2.8.tar` & `ggvlib-0.2.9.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0       22 2022-12-20 12:38:48.235110 ggvlib-0.2.8/ggvlib/__init__.py
--rw-r--r--   0        0        0       95 2022-11-11 09:26:16.308184 ggvlib-0.2.8/ggvlib/config.py
--rw-r--r--   0        0        0        0 2022-11-11 09:26:16.308271 ggvlib-0.2.8/ggvlib/google/__init__.py
--rw-r--r--   0        0        0     2242 2022-11-11 09:26:16.308386 ggvlib-0.2.8/ggvlib/google/bigquery.py
--rw-r--r--   0        0        0     2229 2022-12-20 12:38:32.302199 ggvlib-0.2.8/ggvlib/google/drive.py
--rw-r--r--   0        0        0     4549 2022-11-11 09:50:27.879111 ggvlib-0.2.8/ggvlib/google/scheduler.py
--rw-r--r--   0        0        0      510 2022-11-11 09:50:27.879451 ggvlib-0.2.8/ggvlib/google/secrets.py
--rw-r--r--   0        0        0     5475 2022-11-11 09:26:16.308574 ggvlib-0.2.8/ggvlib/google/sheets.py
--rw-r--r--   0        0        0     2210 2022-11-11 09:26:16.308680 ggvlib-0.2.8/ggvlib/google/storage.py
--rw-r--r--   0        0        0       53 2022-12-20 12:37:58.934414 ggvlib-0.2.8/ggvlib/hubspot/__init__.py
--rw-r--r--   0        0        0    14617 2022-12-20 12:37:58.934533 ggvlib-0.2.8/ggvlib/hubspot/api.py
--rw-r--r--   0        0        0     1924 2022-12-20 12:37:58.934617 ggvlib-0.2.8/ggvlib/hubspot/schemas.py
--rw-r--r--   0        0        0        0 2022-11-11 09:26:16.308774 ggvlib-0.2.8/ggvlib/io/__init__.py
--rw-r--r--   0        0        0     3455 2022-12-20 12:37:58.934748 ggvlib-0.2.8/ggvlib/io/json.py
--rw-r--r--   0        0        0      132 2022-11-11 09:26:16.308986 ggvlib-0.2.8/ggvlib/io/yaml.py
--rw-r--r--   0        0        0      173 2022-11-11 09:26:16.309076 ggvlib-0.2.8/ggvlib/logging.py
--rw-r--r--   0        0        0        0 2022-11-11 09:26:16.309164 ggvlib-0.2.8/ggvlib/mixpanel/__init__.py
--rw-r--r--   0        0        0      888 2022-11-11 09:26:16.309250 ggvlib-0.2.8/ggvlib/mixpanel/api.py
--rw-r--r--   0        0        0     2000 2022-12-20 12:37:58.934857 ggvlib-0.2.8/ggvlib/parsing.py
--rw-r--r--   0        0        0        0 2022-11-11 09:26:16.309418 ggvlib-0.2.8/ggvlib/twilio/__init__.py
--rw-r--r--   0        0        0    10828 2022-11-11 09:26:16.309629 ggvlib-0.2.8/ggvlib/twilio/api.py
--rw-r--r--   0        0        0      108 2022-11-11 09:26:16.309706 ggvlib-0.2.8/ggvlib/twilio/parsing.py
--rw-r--r--   0        0        0      897 2022-12-20 12:38:48.229363 ggvlib-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1129 1970-01-01 00:00:00.000000 ggvlib-0.2.8/setup.py
--rw-r--r--   0        0        0     1014 1970-01-01 00:00:00.000000 ggvlib-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       22 2022-12-21 12:08:58.778246 ggvlib-0.2.9/ggvlib/__init__.py
+-rw-r--r--   0        0        0       95 2022-10-29 16:06:26.477874 ggvlib-0.2.9/ggvlib/config.py
+-rw-r--r--   0        0        0        0 2022-10-29 16:06:26.477874 ggvlib-0.2.9/ggvlib/google/__init__.py
+-rw-r--r--   0        0        0     2242 2022-10-30 05:21:01.178480 ggvlib-0.2.9/ggvlib/google/bigquery.py
+-rw-r--r--   0        0        0     2239 2022-12-20 08:03:31.578087 ggvlib-0.2.9/ggvlib/google/drive.py
+-rw-r--r--   0        0        0     4549 2022-11-15 05:29:51.022214 ggvlib-0.2.9/ggvlib/google/scheduler.py
+-rw-r--r--   0        0        0      510 2022-11-15 05:29:51.022214 ggvlib-0.2.9/ggvlib/google/secrets.py
+-rw-r--r--   0        0        0     5475 2022-10-30 06:31:41.927672 ggvlib-0.2.9/ggvlib/google/sheets.py
+-rw-r--r--   0        0        0     2210 2022-10-29 16:06:26.477874 ggvlib-0.2.9/ggvlib/google/storage.py
+-rw-r--r--   0        0        0     1721 2022-12-21 12:07:48.204737 ggvlib-0.2.9/ggvlib/google/utils.py
+-rw-r--r--   0        0        0       53 2022-11-22 09:11:24.787464 ggvlib-0.2.9/ggvlib/hubspot/__init__.py
+-rw-r--r--   0        0        0    18993 2022-12-21 09:37:06.112522 ggvlib-0.2.9/ggvlib/hubspot/api.py
+-rw-r--r--   0        0        0     1924 2022-11-25 04:40:13.545101 ggvlib-0.2.9/ggvlib/hubspot/schemas.py
+-rw-r--r--   0        0        0        0 2022-10-29 16:06:26.477874 ggvlib-0.2.9/ggvlib/io/__init__.py
+-rw-r--r--   0        0        0     3455 2022-12-21 03:49:30.875778 ggvlib-0.2.9/ggvlib/io/json.py
+-rw-r--r--   0        0        0      132 2022-10-31 08:31:01.058875 ggvlib-0.2.9/ggvlib/io/yaml.py
+-rw-r--r--   0        0        0      173 2022-10-29 16:06:26.477874 ggvlib-0.2.9/ggvlib/logging.py
+-rw-r--r--   0        0        0        0 2022-11-10 13:33:14.544404 ggvlib-0.2.9/ggvlib/mixpanel/__init__.py
+-rw-r--r--   0        0        0      888 2022-11-17 06:11:46.935561 ggvlib-0.2.9/ggvlib/mixpanel/api.py
+-rw-r--r--   0        0        0     2000 2022-11-24 10:32:30.330049 ggvlib-0.2.9/ggvlib/parsing.py
+-rw-r--r--   0        0        0        0 2022-10-29 16:06:26.477874 ggvlib-0.2.9/ggvlib/twilio/__init__.py
+-rw-r--r--   0        0        0    10828 2022-11-01 15:11:46.222157 ggvlib-0.2.9/ggvlib/twilio/api.py
+-rw-r--r--   0        0        0      108 2022-11-01 15:11:46.222157 ggvlib-0.2.9/ggvlib/twilio/parsing.py
+-rw-r--r--   0        0        0      929 2022-12-21 12:08:58.768251 ggvlib-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1168 1970-01-01 00:00:00.000000 ggvlib-0.2.9/setup.py
+-rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 ggvlib-0.2.9/PKG-INFO
```

### Comparing `ggvlib-0.2.8/ggvlib/google/bigquery.py` & `ggvlib-0.2.9/ggvlib/google/bigquery.py`

 * *Files identical despite different names*

### Comparing `ggvlib-0.2.8/ggvlib/google/drive.py` & `ggvlib-0.2.9/ggvlib/google/drive.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 def upload_file(
     name_on_drive: str,
     local_path: str,
     parent_id: str = None,
     mime_type="text/csv",
-    fields: str = "id",
+    fields: List["str"] = ["id"],
 ) -> Dict[str, str]:
     """Uploads a CSV from a local file
 
     Args:
         name_on_drive (str): What to name the CSV file on Google Drive
         local_path (str): The local path of the CSV file
         parent_id (str, optional): The parent id (ie folder) to use. Defaults to None.
```

### Comparing `ggvlib-0.2.8/ggvlib/google/scheduler.py` & `ggvlib-0.2.9/ggvlib/google/scheduler.py`

 * *Files identical despite different names*

### Comparing `ggvlib-0.2.8/ggvlib/google/sheets.py` & `ggvlib-0.2.9/ggvlib/google/sheets.py`

 * *Files identical despite different names*

### Comparing `ggvlib-0.2.8/ggvlib/google/storage.py` & `ggvlib-0.2.9/ggvlib/google/storage.py`

 * *Files identical despite different names*

### Comparing `ggvlib-0.2.8/ggvlib/hubspot/api.py` & `ggvlib-0.2.9/ggvlib/hubspot/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 
         Args:
             access_token (str): The access token for the private app
         """
         self.access_token = access_token
 
     @property
-    def auth_header(self) -> str:
+    def auth_header(self) -> dict:
         return {"Authorization": f"Bearer {self.access_token}"}
 
     @property
-    def json_header(self) -> str:
+    def json_header(self) -> dict:
         return {**self.auth_header, **{"Content-Type": "application/json"}}
 
     @classmethod
     def from_env(cls) -> "Client":
         if not os.getenv("HUBSPOT_ACCESS_TOKEN"):
             raise EnvironmentError(
                 "The environment variable 'HUBSPOT_ACCESS_TOKEN' has not been set"
@@ -76,14 +76,80 @@
                 has_more = response_data["has-more"]
                 offset = response_data[offset_key]
                 all_results.extend(response_data[response_key])
             else:
                 raise RuntimeError(response.status_code)
         return all_results
 
+    def _paginate_crm_list(
+        self, url: str, body_args: dict, method: str = "POST"
+    ) -> List[dict]:
+        """Paginate through a list of reponse pages
+
+        Args:
+            url (str): The url to send a get request to
+            body_args (dict): The body info to send along with the request
+
+        Returns:
+            List[dict]: A list of fetched responses
+        """
+        after = 0
+        failures = 0
+        results = []
+        while True:
+            body_args.update({"after": after})
+            if method == "POST":
+                response = requests.post(
+                    url,
+                    headers=self.json_header,
+                    data=json.dumps(body_args),
+                )
+            elif method == "GET":
+                response = requests.get(
+                    url,
+                    headers=self.json_header,
+                    params=body_args,
+                )
+            else:
+                raise ValueError("Method must be 'POST' or 'GET'")
+            if response.status_code == 200:
+                response_data = response.json()
+                if info := response_data.get("results"):
+                    results.extend(info)
+                else:
+                    results.append(response_data)
+                if paging := response_data.get("paging"):
+                    after = paging["next"]["after"]
+                else:
+                    break
+            else:
+                failures += 1
+                logger.error(response.json())
+                if failures > 3:
+                    break
+        return results
+
+    def _put(self, url: str) -> dict:
+        response = requests.put(url, headers=self.auth_header)
+        if response.status_code <= 400:
+            return response.json()
+        else:
+            raise RuntimeError(response.content)
+
+    def _post(self, url: str, body_args: dict) -> dict:
+        response = requests.post(
+            url,
+            headers=self.json_header,
+            data=json.dumps(body_args),
+        )
+        if response.status_code <= 400:
+            return response.json()
+        else:
+            raise RuntimeError(response.content)
+
     def get_object_properties(self, object_type: str) -> List[dict]:
         """List all properties for an object
 
         Args:
             object_type (str): The object to list properties for ie 'contacts'
 
         Returns:
@@ -153,14 +219,128 @@
         return self._paginate_list(
             request_url=f"{self.api_base_url}/contacts/v1/lists/",
             count=count,
             response_key="lists",
             offset_key="offset",
         )
 
+    def associate_custom_object(
+        self,
+        object_type: str,
+        object_id: str,
+        to_object_type: str,
+        to_object_id: str,
+        association_type: str,
+    ) -> dict:
+        """_summary_
+
+        Args:
+            object_type (str): _description_
+            object_id (str): _description_
+            to_object_type (str): _description_
+            to_object_id (str): _description_
+            association_type (str): _description_
+
+        Returns:
+            dict: _description_
+        """
+        return self._put(
+            url=(
+                f"{self.api_base_url}/crm/v3/objects/{object_type}/{object_id}/"
+                f"associations/{to_object_type}/{to_object_id}/{association_type}"
+            )
+        )
+
+    def create_custom_object_import(
+        self, file_path: str, import_request: dict
+    ) -> dict:
+        """_summary_
+
+        Args:
+            file_path (str): _description_
+            import_request (dict): _description_
+
+        Returns:
+            dict: _description_
+        """
+        file = {"file": open(file_path, "rb")}
+        body_args = {"import_request"}
+        response = requests.post(
+            f"{self.api_base_url}/crm/v3/imports",
+            headers=self.auth_header,
+            files=file,
+            data=body_args,
+        )
+
+    def create_custom_object_batch(
+        self, object_type: str, inputs: List[dict]
+    ) -> dict:
+        """_summary_
+
+        Args:
+            object_type (str): _description_
+            inputs (List[dict]): _description_
+
+        Returns:
+            dict: _description_
+        """
+        return self._post(
+            url=f"{self.api_base_url}/crm/v3/objects/{object_type}/batch/create",
+            body_args={"inputs": inputs},
+        )
+
+    def get_custom_object_batch(
+        self, object_type: str, inputs: List[dict], properties: List[str] = []
+    ) -> List[dict]:
+        """_summary_
+
+        Args:
+            object_type (str): _description_
+            inputs (List[dict]): _description_
+            properties (List[str], optional): _description_. Defaults to [].
+
+        Returns:
+            List[dict]: _description_
+        """
+        body_args = {"properties": properties, "inputs": inputs}
+        return self._paginate_crm_list(
+            url=f"{self.api_base_url}/crm/v3/objects/{object_type}/batch/read",
+            body_args=body_args,
+            method="POST",
+        )
+
+    def get_custom_object_schema(
+        self, object_type: str = None, properties: List[str] = []
+    ) -> List[dict]:
+        """Returns calls
+
+        Args:
+            filters (List[dict]): A list of filters
+            properties (List[str]): A list of properties to return
+
+        Returns:
+            List[dict]: A list of calls
+        """
+        body_args = {
+            "properties": properties,
+            "limit": 100,
+        }
+        if object_type:
+            return self._paginate_crm_list(
+                url=f"{self.api_base_url}/crm/v3/schemas/{object_type}",
+                body_args=body_args,
+                method="GET",
+            )
+        else:
+            return self._paginate_crm_list(
+                url=f"{self.api_base_url}/crm/v3/schemas/",
+                body_args=body_args,
+                method="GET",
+            )
+
     def get_contact_list(self, contact_list_id: int) -> dict:
         """Get information for a specific contact list by id
 
         Args:
             contact_list_id (int): The id of the contact list to fetch
 
         Raises:
@@ -324,48 +504,14 @@
             "limit": 100,
         }
         return self._paginate_crm_list(
             url=f"{self.api_base_url}/crm/v3/objects/calls/search",
             body_args=body_args,
         )
 
-    def _paginate_crm_list(self, url: str, body_args: dict) -> List[dict]:
-        """Paginate through a list of reponse pages
-
-        Args:
-            url (str): The url to send a get request to
-            body_args (dict): The body info to send along with the request
-
-        Returns:
-            List[dict]: A list of fetched responses
-        """
-        after = 0
-        failures = 0
-        results = []
-        while True:
-            body_args.update({"after": after})
-            response = requests.post(
-                url,
-                headers=self.json_header,
-                data=json.dumps(body_args),
-            )
-            if response.status_code == 200:
-                response_data = response.json()
-                results.extend(response_data["results"])
-                if paging := response_data.get("paging"):
-                    after = paging["next"]["after"]
-                else:
-                    break
-            else:
-                failures += 1
-                logger.error(response.json())
-                if failures > 3:
-                    break
-        return results
-
     def create_or_update_contact(self, contact: Contact) -> dict:
         """Create or update a Contact
 
         Args:
             contact (Contact): A Hubspot contacts
 
         Raises:
```

### Comparing `ggvlib-0.2.8/ggvlib/hubspot/schemas.py` & `ggvlib-0.2.9/ggvlib/hubspot/schemas.py`

 * *Files identical despite different names*

### Comparing `ggvlib-0.2.8/ggvlib/io/json.py` & `ggvlib-0.2.9/ggvlib/io/json.py`

 * *Files identical despite different names*

### Comparing `ggvlib-0.2.8/ggvlib/mixpanel/api.py` & `ggvlib-0.2.9/ggvlib/mixpanel/api.py`

 * *Files identical despite different names*

### Comparing `ggvlib-0.2.8/ggvlib/parsing.py` & `ggvlib-0.2.9/ggvlib/parsing.py`

 * *Files identical despite different names*

### Comparing `ggvlib-0.2.8/ggvlib/twilio/api.py` & `ggvlib-0.2.9/ggvlib/twilio/api.py`

 * *Files identical despite different names*

### Comparing `ggvlib-0.2.8/pyproject.toml` & `ggvlib-0.2.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ggvlib"
-version = "0.2.8"
+version = "0.2.9"
 description = ""
 authors = ["Adam Hoffstein <adam.hoffstein@gogox.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 google-cloud-bigquery = "^3.3.5"
 loguru = "0.5.0"
@@ -16,14 +16,15 @@
 google-api-python-client = "^2.65.0"
 pydantic = "^1.10.2"
 aiohttp = "^3.8.3"
 google-cloud-secret-manager = "^2.12.6"
 google-crc32c = "^1.5.0"
 google-cloud-scheduler = "^2.7.3"
 jsonschema = "^4.17.0"
+google-auth-oauthlib = "^0.8.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 black = "^22.10.0"
 Sphinx = "^5.3.0"
 sphinx-rtd-theme = "^1.0.0"
 sphinx-autoapi = "^2.0.0"
```

### Comparing `ggvlib-0.2.8/setup.py` & `ggvlib-0.2.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,29 +12,30 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8.3,<4.0.0',
  'db-dtypes>=1.0.4,<2.0.0',
  'google-api-python-client>=2.65.0,<3.0.0',
+ 'google-auth-oauthlib>=0.8.0,<0.9.0',
  'google-cloud-bigquery-storage>=2.16.2,<3.0.0',
  'google-cloud-bigquery>=3.3.5,<4.0.0',
  'google-cloud-scheduler>=2.7.3,<3.0.0',
  'google-cloud-secret-manager>=2.12.6,<3.0.0',
  'google-cloud-storage>=2.5.0,<3.0.0',
  'google-crc32c>=1.5.0,<2.0.0',
  'jsonschema>=4.17.0,<5.0.0',
  'loguru==0.5.0',
  'pandas>=1.5.1,<2.0.0',
  'pydantic>=1.10.2,<2.0.0',
  'pyyaml>=6.0,<7.0']
 
 setup_kwargs = {
     'name': 'ggvlib',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': '',
     'long_description': 'None',
     'author': 'Adam Hoffstein',
     'author_email': 'adam.hoffstein@gogox.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ggvlib-0.2.8/PKG-INFO` & `ggvlib-0.2.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ggvlib
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 Author: Adam Hoffstein
 Author-email: adam.hoffstein@gogox.com
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: db-dtypes (>=1.0.4,<2.0.0)
 Requires-Dist: google-api-python-client (>=2.65.0,<3.0.0)
+Requires-Dist: google-auth-oauthlib (>=0.8.0,<0.9.0)
 Requires-Dist: google-cloud-bigquery (>=3.3.5,<4.0.0)
 Requires-Dist: google-cloud-bigquery-storage (>=2.16.2,<3.0.0)
 Requires-Dist: google-cloud-scheduler (>=2.7.3,<3.0.0)
 Requires-Dist: google-cloud-secret-manager (>=2.12.6,<3.0.0)
 Requires-Dist: google-cloud-storage (>=2.5.0,<3.0.0)
 Requires-Dist: google-crc32c (>=1.5.0,<2.0.0)
 Requires-Dist: jsonschema (>=4.17.0,<5.0.0)
```

