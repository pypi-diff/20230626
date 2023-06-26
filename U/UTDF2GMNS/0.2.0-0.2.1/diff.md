# Comparing `tmp/UTDF2GMNS-0.2.0.tar.gz` & `tmp/UTDF2GMNS-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UTDF2GMNS-0.2.0.tar", last modified: Mon Jun 26 02:12:51 2023, max compression
+gzip compressed data, was "UTDF2GMNS-0.2.1.tar", last modified: Mon Jun 26 02:28:34 2023, max compression
```

## Comparing `UTDF2GMNS-0.2.0.tar` & `UTDF2GMNS-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 02:12:51.739970 UTDF2GMNS-0.2.0/
--rw-rw-rw-   0        0        0    11558 2022-12-19 22:02:10.000000 UTDF2GMNS-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     2188 2023-06-26 02:12:51.739970 UTDF2GMNS-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1665 2023-06-24 00:38:11.000000 UTDF2GMNS-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 02:12:51.711717 UTDF2GMNS-0.2.0/UTDF2GMNS.egg-info/
--rw-rw-rw-   0        0        0     2188 2023-06-26 02:12:51.000000 UTDF2GMNS-0.2.0/UTDF2GMNS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-06-26 02:12:51.000000 UTDF2GMNS-0.2.0/UTDF2GMNS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 02:12:51.000000 UTDF2GMNS-0.2.0/UTDF2GMNS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-26 02:12:51.000000 UTDF2GMNS-0.2.0/UTDF2GMNS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-26 02:12:51.000000 UTDF2GMNS-0.2.0/UTDF2GMNS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 02:12:51.739970 UTDF2GMNS-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1489 2023-06-26 02:12:27.000000 UTDF2GMNS-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 02:12:51.715711 UTDF2GMNS-0.2.0/utdf2gmns/
--rw-rw-rw-   0        0        0     1155 2023-06-26 02:12:41.000000 UTDF2GMNS-0.2.0/utdf2gmns/__init__.py
--rw-rw-rw-   0        0        0     9196 2023-06-26 02:03:52.000000 UTDF2GMNS-0.2.0/utdf2gmns/__utdf2gmns.py
-drwxrwxrwx   0        0        0        0 2023-06-26 02:12:51.728902 UTDF2GMNS-0.2.0/utdf2gmns/func_lib/
--rw-rw-rw-   0        0        0      277 2023-06-24 00:46:51.000000 UTDF2GMNS-0.2.0/utdf2gmns/func_lib/__init__.py
--rw-rw-rw-   0        0        0     6269 2023-06-26 01:17:25.000000 UTDF2GMNS-0.2.0/utdf2gmns/func_lib/geocoding_intersection.py
--rw-rw-rw-   0        0        0     7397 2023-06-26 01:52:21.000000 UTDF2GMNS-0.2.0/utdf2gmns/func_lib/match_node_intersection_movement_utdf.py
--rw-rw-rw-   0        0        0    11276 2023-06-26 02:07:54.000000 UTDF2GMNS-0.2.0/utdf2gmns/func_lib/read_utdf.py
-drwxrwxrwx   0        0        0        0 2023-06-26 02:12:51.738909 UTDF2GMNS-0.2.0/utdf2gmns/utils_lib/
--rw-rw-rw-   0        0        0      278 2023-03-07 10:13:11.000000 UTDF2GMNS-0.2.0/utdf2gmns/utils_lib/__init__.py
--rw-rw-rw-   0        0        0     3356 2023-06-26 02:02:58.000000 UTDF2GMNS-0.2.0/utdf2gmns/utils_lib/package_settings.py
--rw-rw-rw-   0        0        0     5794 2023-03-14 01:43:28.000000 UTDF2GMNS-0.2.0/utdf2gmns/utils_lib/utility_lib.py
+drwxrwxrwx   0        0        0        0 2023-06-26 02:28:34.045524 UTDF2GMNS-0.2.1/
+-rw-rw-rw-   0        0        0    11558 2022-12-19 22:02:10.000000 UTDF2GMNS-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2238 2023-06-26 02:28:34.043490 UTDF2GMNS-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1715 2023-06-26 02:26:35.000000 UTDF2GMNS-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 02:28:34.012340 UTDF2GMNS-0.2.1/UTDF2GMNS.egg-info/
+-rw-rw-rw-   0        0        0     2238 2023-06-26 02:28:33.000000 UTDF2GMNS-0.2.1/UTDF2GMNS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-06-26 02:28:33.000000 UTDF2GMNS-0.2.1/UTDF2GMNS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 02:28:33.000000 UTDF2GMNS-0.2.1/UTDF2GMNS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-26 02:28:33.000000 UTDF2GMNS-0.2.1/UTDF2GMNS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-26 02:28:33.000000 UTDF2GMNS-0.2.1/UTDF2GMNS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 02:28:34.046495 UTDF2GMNS-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1489 2023-06-26 02:28:05.000000 UTDF2GMNS-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 02:28:34.020378 UTDF2GMNS-0.2.1/utdf2gmns/
+-rw-rw-rw-   0        0        0     1155 2023-06-26 02:28:18.000000 UTDF2GMNS-0.2.1/utdf2gmns/__init__.py
+-rw-rw-rw-   0        0        0     9196 2023-06-26 02:03:52.000000 UTDF2GMNS-0.2.1/utdf2gmns/__utdf2gmns.py
+drwxrwxrwx   0        0        0        0 2023-06-26 02:28:34.033703 UTDF2GMNS-0.2.1/utdf2gmns/func_lib/
+-rw-rw-rw-   0        0        0      277 2023-06-24 00:46:51.000000 UTDF2GMNS-0.2.1/utdf2gmns/func_lib/__init__.py
+-rw-rw-rw-   0        0        0     6379 2023-06-26 02:22:27.000000 UTDF2GMNS-0.2.1/utdf2gmns/func_lib/geocoding_intersection.py
+-rw-rw-rw-   0        0        0     7462 2023-06-26 02:25:19.000000 UTDF2GMNS-0.2.1/utdf2gmns/func_lib/match_node_intersection_movement_utdf.py
+-rw-rw-rw-   0        0        0    11276 2023-06-26 02:07:54.000000 UTDF2GMNS-0.2.1/utdf2gmns/func_lib/read_utdf.py
+drwxrwxrwx   0        0        0        0 2023-06-26 02:28:34.041492 UTDF2GMNS-0.2.1/utdf2gmns/utils_lib/
+-rw-rw-rw-   0        0        0      278 2023-03-07 10:13:11.000000 UTDF2GMNS-0.2.1/utdf2gmns/utils_lib/__init__.py
+-rw-rw-rw-   0        0        0     3356 2023-06-26 02:02:58.000000 UTDF2GMNS-0.2.1/utdf2gmns/utils_lib/package_settings.py
+-rw-rw-rw-   0        0        0     5794 2023-03-14 01:43:28.000000 UTDF2GMNS-0.2.1/utdf2gmns/utils_lib/utility_lib.py
```

### Comparing `UTDF2GMNS-0.2.0/LICENSE` & `UTDF2GMNS-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `UTDF2GMNS-0.2.0/PKG-INFO` & `UTDF2GMNS-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UTDF2GMNS
-Version: 0.2.0
+Version: 0.2.1
 Summary: This open-source package is a tool to convert utdf file to GMNS format.
 Home-page: https://github.com/asu-trans-ai-lab/utdf2gmns
 Author: Xiangyong Luo, Dr.Xuesong (Simon) Zhou
 Author-email: luoxiangyong01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -44,26 +44,21 @@
 ## Data Conversion Steps:
 
 * Step 1: Read UTDF.csv file and perform geocoding, then produce utdf_geo, utdf_lane, and utdf_phase_timeplans.
 * Step 2: Match four files (utdf_geo, node, utdf_lane, utdf_pahse_timeplans, movement) to produce movement_utdf
 
 ## TODO LIST
 
-Print out how many intersections being geocoded.
+* [X] Print out how many intersections being geocoded.
+* [ ] Print out how many movements being matched or not matched for signalized intersecton nodes in osm2gmns files.
 
-Print out how many movements being matched or not matched for signalized intersecton nodes in osm2gmns files.
+* [ ] Add cycle length and green time for each movement.
+* [ ] Check reasonable capacity.
 
-Add cycle length and green time for each movement.
+* [ ] Check each movement is reasonable (like 15s of green time...). other attributes.
+* [ ] Check number of lanes correctness between osm2gmns file and synchro file per movements.
 
-Check reasonable capacity.
+* [X] Print out check log.
+* [X] Number of lanes of the movements from synchro file.
 
-Check each movement is reasonable (like 15s of green time...). other attributes.
-
-Check number of lanes correctness between osm2gmns file and synchro file per movements.
-
-Print out check log.
-
-Number of lanes of the movements from synchro file.
-
-Add signal info to micre-link.csv
-
-Add function to verify whether geocoded for utdf_geo
+* [ ] Add signal info to micre-link.csv
+* [X] Add function to verify whether geocoded for utdf_geo
```

### Comparing `UTDF2GMNS-0.2.0/README.md` & `UTDF2GMNS-0.2.1/UTDF2GMNS.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: UTDF2GMNS
+Version: 0.2.1
+Summary: This open-source package is a tool to convert utdf file to GMNS format.
+Home-page: https://github.com/asu-trans-ai-lab/utdf2gmns
+Author: Xiangyong Luo, Dr.Xuesong (Simon) Zhou
+Author-email: luoxiangyong01@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## utdf2gmns: Introduction
 
 This open-source package is a tool to convert utdf file to GMNS format.
 
 ## Required Data Input Files:
 
 * [X] UTDF.csv
@@ -30,26 +44,21 @@
 ## Data Conversion Steps:
 
 * Step 1: Read UTDF.csv file and perform geocoding, then produce utdf_geo, utdf_lane, and utdf_phase_timeplans.
 * Step 2: Match four files (utdf_geo, node, utdf_lane, utdf_pahse_timeplans, movement) to produce movement_utdf
 
 ## TODO LIST
 
-Print out how many intersections being geocoded.
-
-Print out how many movements being matched or not matched for signalized intersecton nodes in osm2gmns files.
-
-Add cycle length and green time for each movement.
-
-Check reasonable capacity.
-
-Check each movement is reasonable (like 15s of green time...). other attributes.
-
-Check number of lanes correctness between osm2gmns file and synchro file per movements.
+* [X] Print out how many intersections being geocoded.
+* [ ] Print out how many movements being matched or not matched for signalized intersecton nodes in osm2gmns files.
 
-Print out check log.
+* [ ] Add cycle length and green time for each movement.
+* [ ] Check reasonable capacity.
 
-Number of lanes of the movements from synchro file.
+* [ ] Check each movement is reasonable (like 15s of green time...). other attributes.
+* [ ] Check number of lanes correctness between osm2gmns file and synchro file per movements.
 
-Add signal info to micre-link.csv
+* [X] Print out check log.
+* [X] Number of lanes of the movements from synchro file.
 
-Add function to verify whether geocoded for utdf_geo
+* [ ] Add signal info to micre-link.csv
+* [X] Add function to verify whether geocoded for utdf_geo
```

### Comparing `UTDF2GMNS-0.2.0/UTDF2GMNS.egg-info/PKG-INFO` & `UTDF2GMNS-0.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: UTDF2GMNS
-Version: 0.2.0
-Summary: This open-source package is a tool to convert utdf file to GMNS format.
-Home-page: https://github.com/asu-trans-ai-lab/utdf2gmns
-Author: Xiangyong Luo, Dr.Xuesong (Simon) Zhou
-Author-email: luoxiangyong01@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## utdf2gmns: Introduction
 
 This open-source package is a tool to convert utdf file to GMNS format.
 
 ## Required Data Input Files:
 
 * [X] UTDF.csv
@@ -44,26 +30,21 @@
 ## Data Conversion Steps:
 
 * Step 1: Read UTDF.csv file and perform geocoding, then produce utdf_geo, utdf_lane, and utdf_phase_timeplans.
 * Step 2: Match four files (utdf_geo, node, utdf_lane, utdf_pahse_timeplans, movement) to produce movement_utdf
 
 ## TODO LIST
 
-Print out how many intersections being geocoded.
-
-Print out how many movements being matched or not matched for signalized intersecton nodes in osm2gmns files.
-
-Add cycle length and green time for each movement.
-
-Check reasonable capacity.
-
-Check each movement is reasonable (like 15s of green time...). other attributes.
-
-Check number of lanes correctness between osm2gmns file and synchro file per movements.
+* [X] Print out how many intersections being geocoded.
+* [ ] Print out how many movements being matched or not matched for signalized intersecton nodes in osm2gmns files.
 
-Print out check log.
+* [ ] Add cycle length and green time for each movement.
+* [ ] Check reasonable capacity.
 
-Number of lanes of the movements from synchro file.
+* [ ] Check each movement is reasonable (like 15s of green time...). other attributes.
+* [ ] Check number of lanes correctness between osm2gmns file and synchro file per movements.
 
-Add signal info to micre-link.csv
+* [X] Print out check log.
+* [X] Number of lanes of the movements from synchro file.
 
-Add function to verify whether geocoded for utdf_geo
+* [ ] Add signal info to micre-link.csv
+* [X] Add function to verify whether geocoded for utdf_geo
```

### Comparing `UTDF2GMNS-0.2.0/UTDF2GMNS.egg-info/SOURCES.txt` & `UTDF2GMNS-0.2.1/UTDF2GMNS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UTDF2GMNS-0.2.0/setup.py` & `UTDF2GMNS-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     with open("requirements.txt", "r", encoding="utf-8") as f:
         modules_needed = [i.strip() for i in f.readlines()]
 except Exception:
     modules_needed = []
 
 setuptools.setup(
     name="UTDF2GMNS",  # Replace with your own username
-    version="0.2.0",
+    version="0.2.1",
     author="Xiangyong Luo, Dr.Xuesong (Simon) Zhou",
     author_email="luoxiangyong01@gmail.com",
     description="This open-source package is a tool to convert utdf file to GMNS format.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/asu-trans-ai-lab/utdf2gmns",
```

### Comparing `UTDF2GMNS-0.2.0/utdf2gmns/__init__.py` & `UTDF2GMNS-0.2.1/utdf2gmns/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
            'match_intersection_node',
            'match_movement_and_intersection_node',
            'match_movement_utdf_lane',
            'match_movement_utdf_phase_timeplans',
            'package_settings'
            ]
 
-print("UTDF2GMNS Version: ", "0.2.0")
+print("UTDF2GMNS Version: ", "0.2.1")
```

### Comparing `UTDF2GMNS-0.2.0/utdf2gmns/__utdf2gmns.py` & `UTDF2GMNS-0.2.1/utdf2gmns/__utdf2gmns.py`

 * *Files identical despite different names*

### Comparing `UTDF2GMNS-0.2.0/utdf2gmns/func_lib/geocoding_intersection.py` & `UTDF2GMNS-0.2.1/utdf2gmns/func_lib/geocoding_intersection.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,17 @@
 
     created_column_names = ["reversed_intersection_name", "full_name_intersection",
                             "full_name_intersection_reversed", "distance_from_full_name"]
     df_final = df.loc[:, ~df.columns.isin(created_column_names)]
 
     # print summary information
     print(
-        f"There are {df_final['coord_x'].isna().sum()} / {len(df_final)} intersections are not able to geocode.")
+        f" {len(df_final) - df_final['coord_x'].isna().sum()} / {len(df_final)} intersections geocoded.")
+    print(
+        f" {df_final['coord_x'].isna().sum()} / {len(df_final)} intersections are not able to geocode.")
 
     return df_final
 
 
 if __name__ == "__main__":
     """
     We provided three geocoding methods: googlemaps, geopy and geocoder
```

### Comparing `UTDF2GMNS-0.2.0/utdf2gmns/func_lib/match_node_intersection_movement_utdf.py` & `UTDF2GMNS-0.2.1/utdf2gmns/func_lib/match_node_intersection_movement_utdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,15 @@
     return df_movement_intersection
 
 
 @func_running_time
 def match_movement_utdf_lane(df_movement_intersection: pd.DataFrame, utdf_dict_data: dict) -> pd.DataFrame:
     # Add Synchro/utdf data to movement_intersection_node
     df_utdf_lanes = utdf_dict_data.get("Lanes")
+    print(f"  : There are {df_utdf_lanes.shape[0]} utdf lanes")
 
     intersection_id_list = [value for value in list(
         df_movement_intersection["synchro_INTID"].unique()) if value is not None]
 
     # get movement_intersection dataframe with and without id list
     df_with_id = df_movement_intersection[df_movement_intersection["synchro_INTID"].isin(
         intersection_id_list)]
```

### Comparing `UTDF2GMNS-0.2.0/utdf2gmns/func_lib/read_utdf.py` & `UTDF2GMNS-0.2.1/utdf2gmns/func_lib/read_utdf.py`

 * *Files identical despite different names*

### Comparing `UTDF2GMNS-0.2.0/utdf2gmns/utils_lib/package_settings.py` & `UTDF2GMNS-0.2.1/utdf2gmns/utils_lib/package_settings.py`

 * *Files identical despite different names*

### Comparing `UTDF2GMNS-0.2.0/utdf2gmns/utils_lib/utility_lib.py` & `UTDF2GMNS-0.2.1/utdf2gmns/utils_lib/utility_lib.py`

 * *Files identical despite different names*

