# Comparing `tmp/midas-data-util-0.2.3.tar.gz` & `tmp/midas-data-util-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midas-data-util-0.2.3.tar", last modified: Wed Apr 12 12:05:58 2023, max compression
+gzip compressed data, was "midas-data-util-0.2.4.tar", last modified: Sun Jun 25 23:44:11 2023, max compression
```

## Comparing `midas-data-util-0.2.3.tar` & `midas-data-util-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 12:05:58.192146 midas-data-util-0.2.3/
--rw-rw-rw-   0        0        0    11558 2023-04-07 08:14:57.000000 midas-data-util-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      520 2023-04-12 12:05:58.191078 midas-data-util-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-04-07 08:58:48.000000 midas-data-util-0.2.3/README.md
--rw-rw-rw-   0        0        0      623 2023-04-12 12:05:24.000000 midas-data-util-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 12:05:58.192146 midas-data-util-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-12 12:05:58.082965 midas-data-util-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 12:05:58.140814 midas-data-util-0.2.3/src/midas/
--rw-rw-rw-   0        0        0     2631 2023-04-12 07:17:33.000000 midas-data-util-0.2.3/src/midas/__init__.py
--rw-rw-rw-   0        0        0     5845 2023-04-12 07:16:48.000000 midas-data-util-0.2.3/src/midas/data_encoder.py
--rw-rw-rw-   0        0        0    11528 2023-04-12 11:59:47.000000 midas-data-util-0.2.3/src/midas/event.py
--rw-rw-rw-   0        0        0     9405 2023-04-12 06:08:18.000000 midas-data-util-0.2.3/src/midas/playfab.py
--rw-rw-rw-   0        0        0     4327 2023-04-12 12:04:40.000000 midas-data-util-0.2.3/src/midas/session.py
--rw-rw-rw-   0        0        0     3448 2023-04-12 12:05:02.000000 midas-data-util-0.2.3/src/midas/user.py
-drwxrwxrwx   0        0        0        0 2023-04-12 12:05:58.189085 midas-data-util-0.2.3/src/midas_data_util.egg-info/
--rw-rw-rw-   0        0        0      520 2023-04-12 12:05:58.000000 midas-data-util-0.2.3/src/midas_data_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-04-12 12:05:58.000000 midas-data-util-0.2.3/src/midas_data_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 12:05:58.000000 midas-data-util-0.2.3/src/midas_data_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-04-12 12:05:58.000000 midas-data-util-0.2.3/src/midas_data_util.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-12 12:05:58.000000 midas-data-util-0.2.3/src/midas_data_util.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 23:44:11.251139 midas-data-util-0.2.4/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 08:14:57.000000 midas-data-util-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      520 2023-06-25 23:44:11.250163 midas-data-util-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2023-04-07 08:58:48.000000 midas-data-util-0.2.4/README.md
+-rw-rw-rw-   0        0        0      623 2023-06-25 23:37:18.000000 midas-data-util-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-25 23:44:11.251139 midas-data-util-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-25 23:44:11.202105 midas-data-util-0.2.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 23:44:11.217639 midas-data-util-0.2.4/src/midas/
+-rw-rw-rw-   0        0        0     2631 2023-04-12 07:17:33.000000 midas-data-util-0.2.4/src/midas/__init__.py
+-rw-rw-rw-   0        0        0     5845 2023-04-12 07:16:48.000000 midas-data-util-0.2.4/src/midas/data_encoder.py
+-rw-rw-rw-   0        0        0    11528 2023-04-12 11:59:47.000000 midas-data-util-0.2.4/src/midas/event.py
+-rw-rw-rw-   0        0        0     9478 2023-06-25 23:37:04.000000 midas-data-util-0.2.4/src/midas/playfab.py
+-rw-rw-rw-   0        0        0     4327 2023-04-12 12:04:40.000000 midas-data-util-0.2.4/src/midas/session.py
+-rw-rw-rw-   0        0        0     3448 2023-04-12 12:05:02.000000 midas-data-util-0.2.4/src/midas/user.py
+drwxrwxrwx   0        0        0        0 2023-06-25 23:44:11.248155 midas-data-util-0.2.4/src/midas_data_util.egg-info/
+-rw-rw-rw-   0        0        0      520 2023-06-25 23:44:11.000000 midas-data-util-0.2.4/src/midas_data_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-06-25 23:44:11.000000 midas-data-util-0.2.4/src/midas_data_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 23:44:11.000000 midas-data-util-0.2.4/src/midas_data_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-06-25 23:44:11.000000 midas-data-util-0.2.4/src/midas_data_util.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-25 23:44:11.000000 midas-data-util-0.2.4/src/midas_data_util.egg-info/top_level.txt
```

### Comparing `midas-data-util-0.2.3/LICENSE` & `midas-data-util-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.2.3/PKG-INFO` & `midas-data-util-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas-data-util
-Version: 0.2.3
+Version: 0.2.4
 Summary: a package with useful functions for downloading and working with midas generated analytics data
 Author-email: nightcycle <coyer@nightcycle.us>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `midas-data-util-0.2.3/pyproject.toml` & `midas-data-util-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "midas-data-util"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"lxml~=4.9.2", 
 	"pandas~=2.0.0",
 	"adal~=1.2.7",
```

### Comparing `midas-data-util-0.2.3/src/midas/__init__.py` & `midas-data-util-0.2.4/src/midas/__init__.py`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.2.3/src/midas/data_encoder.py` & `midas-data-util-0.2.4/src/midas/data_encoder.py`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.2.3/src/midas/event.py` & `midas-data-util-0.2.4/src/midas/event.py`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.2.3/src/midas/playfab.py` & `midas-data-util-0.2.4/src/midas/playfab.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,21 +86,24 @@
 		self.client = KustoClient(kcsb)
 		self.client._query_endpoint = CLUSTER + "/v1/rest/query"
 
 		crp = ClientRequestProperties()
 		crp.application = "KustoPythonSDK"
 
 	def query(self, query=DEFAULT_QUERY):
-		response = self.client.execute(self.title_id, query)
+		try:
+			response = self.client.execute(self.title_id, query)
 
-		# Response processing
-		result = str(response[0])
-		df = pd.DataFrame(json.loads(result)["data"])
+			# Response processing
+			result = str(response[0])
+			df = pd.DataFrame(json.loads(result)["data"])
 
-		return df.to_dict(orient='records')
+			return df.to_dict(orient='records')
+		except:
+			raise ValueError("query failed: \n\n"+query)
 
 	def query_user_data_list(self, user_join_floor: datetime, join_window_in_days: int, user_limit=100000) -> list[UserData]:
 		query = f"""let title_id = "{self.title_id}";
 let filter_users_who_joined_before= datetime("{get_playfab_str_from_datetime(user_join_floor)}");
 let join_window_in_days = {join_window_in_days};
 let user_limit = {user_limit+1};
 let filter_users_who_joined_after = datetime_add("day", join_window_in_days, filter_users_who_joined_before);
```

### Comparing `midas-data-util-0.2.3/src/midas/session.py` & `midas-data-util-0.2.4/src/midas/session.py`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.2.3/src/midas/user.py` & `midas-data-util-0.2.4/src/midas/user.py`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.2.3/src/midas_data_util.egg-info/PKG-INFO` & `midas-data-util-0.2.4/src/midas_data_util.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas-data-util
-Version: 0.2.3
+Version: 0.2.4
 Summary: a package with useful functions for downloading and working with midas generated analytics data
 Author-email: nightcycle <coyer@nightcycle.us>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

