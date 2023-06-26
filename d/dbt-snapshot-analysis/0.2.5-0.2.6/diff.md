# Comparing `tmp/dbt_snapshot_analysis-0.2.5.tar.gz` & `tmp/dbt_snapshot_analysis-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_snapshot_analysis-0.2.5.tar", last modified: Fri Jun 23 16:07:11 2023, max compression
+gzip compressed data, was "dbt_snapshot_analysis-0.2.6.tar", last modified: Mon Jun 26 15:35:46 2023, max compression
```

## Comparing `dbt_snapshot_analysis-0.2.5.tar` & `dbt_snapshot_analysis-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 16:07:11.503872 dbt_snapshot_analysis-0.2.5/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     1347 2023-06-23 16:07:11.503744 dbt_snapshot_analysis-0.2.5/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      928 2023-06-23 13:57:34.000000 dbt_snapshot_analysis-0.2.5/README.md
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 16:07:11.502762 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis/
--rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:17:16.000000 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis/__init__.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      873 2023-06-21 15:26:08.000000 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis/data_validation.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)     5917 2023-06-23 16:05:25.000000 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis/dbt_snapshot_analysis.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)     1449 2023-06-23 15:03:50.000000 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis/snapshot_utils.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      372 2023-06-23 13:21:59.000000 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis/streamlit_entry_point.py
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 16:07:11.503555 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis.egg-info/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     1347 2023-06-23 16:07:11.000000 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis.egg-info/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      499 2023-06-23 16:07:11.000000 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-06-23 16:07:11.000000 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       91 2023-06-23 16:07:11.000000 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis.egg-info/entry_points.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       24 2023-06-23 16:07:11.000000 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis.egg-info/requires.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       22 2023-06-23 16:07:11.000000 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis.egg-info/top_level.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-06-23 16:07:11.503920 dbt_snapshot_analysis-0.2.5/setup.cfg
--rw-r--r--   0 sammyteillet   (501) staff       (20)      847 2023-06-23 16:06:39.000000 dbt_snapshot_analysis-0.2.5/setup.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-26 15:35:46.691938 dbt_snapshot_analysis-0.2.6/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     1355 2023-06-26 15:35:46.691810 dbt_snapshot_analysis-0.2.6/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      936 2023-06-26 08:26:25.000000 dbt_snapshot_analysis-0.2.6/README.md
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-26 15:35:46.690692 dbt_snapshot_analysis-0.2.6/dbt_snapshot_analysis/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:17:16.000000 dbt_snapshot_analysis-0.2.6/dbt_snapshot_analysis/__init__.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      873 2023-06-21 15:26:08.000000 dbt_snapshot_analysis-0.2.6/dbt_snapshot_analysis/data_validation.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     9807 2023-06-26 15:35:00.000000 dbt_snapshot_analysis-0.2.6/dbt_snapshot_analysis/dbt_snapshot_analysis.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     2025 2023-06-26 15:24:40.000000 dbt_snapshot_analysis-0.2.6/dbt_snapshot_analysis/snapshot_utils.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      372 2023-06-23 13:21:59.000000 dbt_snapshot_analysis-0.2.6/dbt_snapshot_analysis/streamlit_entry_point.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-26 15:35:46.691603 dbt_snapshot_analysis-0.2.6/dbt_snapshot_analysis.egg-info/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     1355 2023-06-26 15:35:46.000000 dbt_snapshot_analysis-0.2.6/dbt_snapshot_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      499 2023-06-26 15:35:46.000000 dbt_snapshot_analysis-0.2.6/dbt_snapshot_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-06-26 15:35:46.000000 dbt_snapshot_analysis-0.2.6/dbt_snapshot_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       91 2023-06-26 15:35:46.000000 dbt_snapshot_analysis-0.2.6/dbt_snapshot_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       24 2023-06-26 15:35:46.000000 dbt_snapshot_analysis-0.2.6/dbt_snapshot_analysis.egg-info/requires.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       22 2023-06-26 15:35:46.000000 dbt_snapshot_analysis-0.2.6/dbt_snapshot_analysis.egg-info/top_level.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-06-26 15:35:46.691982 dbt_snapshot_analysis-0.2.6/setup.cfg
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      847 2023-06-26 15:35:43.000000 dbt_snapshot_analysis-0.2.6/setup.py
```

### Comparing `dbt_snapshot_analysis-0.2.5/PKG-INFO` & `dbt_snapshot_analysis-0.2.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt_snapshot_analysis
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package for analyzing snapshots
 Home-page: https://github.com/data-drift/dbt-snapshot-analytics
 Author: Sammy Teillet
 Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,15 @@
 
 This project is developped by the DataDrift team.
 
 DBT Snapshot Analysis is a Python package for analyzing snapshots. It provides a set of tools for visualizing and exploring data in a variety of ways.
 
 ## Installation
 
-You can install Plot Analysis using `pip`:
+You can install DBT Snapshot Analysis using `pip`:
 
 ```sh
 pip install dbt-snapshot-analysis
 ```
 
 ## Usage
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_s0gvmt88_/tmpn8l276xj_TarContainer/0/1", line 21, column 2: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_s0gvmt88_/tmpn8l276xj_TarContainer/0/1", line 21, column 2: Levels of opening and closing headings don't match*

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: dbt_snapshot_analysis Version: 0.2.5 Summary: A
+Metadata-Version: 2.1 Name: dbt_snapshot_analysis Version: 0.2.6 Summary: A
 package for analyzing snapshots Home-page: https://github.com/data-drift/dbt-
 snapshot-analytics Author: Sammy Teillet Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
                                [DataDrift_logo]
                        ***** A Changelog for Data *****
                       Git-Based. Data-Consumer-Friendly.
                                 Website Â· Blog
 # DBT Snapshot Analysis [![PyPI version](https://badge.fury.io/py/dbt-snapshot-
 analysis.svg)](https://badge.fury.io/py/dbt-snapshot-analysis) This project is
 developped by the DataDrift team. DBT Snapshot Analysis is a Python package for
 analyzing snapshots. It provides a set of tools for visualizing and exploring
-data in a variety of ways. ## Installation You can install Plot Analysis using
-`pip`: ```sh pip install dbt-snapshot-analysis ``` ## Usage ```sh
-dbt_snapshot_analysis ```
+data in a variety of ways. ## Installation You can install DBT Snapshot
+Analysis using `pip`: ```sh pip install dbt-snapshot-analysis ``` ## Usage
+```sh dbt_snapshot_analysis ```
```

### Comparing `dbt_snapshot_analysis-0.2.5/README.md` & `dbt_snapshot_analysis-0.2.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 This project is developped by the DataDrift team.
 
 DBT Snapshot Analysis is a Python package for analyzing snapshots. It provides a set of tools for visualizing and exploring data in a variety of ways.
 
 ## Installation
 
-You can install Plot Analysis using `pip`:
+You can install DBT Snapshot Analysis using `pip`:
 
 ```sh
 pip install dbt-snapshot-analysis
 ```
 
 ## Usage
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_s0gvmt88_/tmpn8l276xj_TarContainer/0/2.md", line 9, column 2: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_s0gvmt88_/tmpn8l276xj_TarContainer/0/2.md", line 9, column 2: Levels of opening and closing headings don't match*

```diff
@@ -2,10 +2,10 @@
                        ***** A Changelog for Data *****
                       Git-Based. Data-Consumer-Friendly.
                                 Website Â· Blog
 # DBT Snapshot Analysis [![PyPI version](https://badge.fury.io/py/dbt-snapshot-
 analysis.svg)](https://badge.fury.io/py/dbt-snapshot-analysis) This project is
 developped by the DataDrift team. DBT Snapshot Analysis is a Python package for
 analyzing snapshots. It provides a set of tools for visualizing and exploring
-data in a variety of ways. ## Installation You can install Plot Analysis using
-`pip`: ```sh pip install dbt-snapshot-analysis ``` ## Usage ```sh
-dbt_snapshot_analysis ```
+data in a variety of ways. ## Installation You can install DBT Snapshot
+Analysis using `pip`: ```sh pip install dbt-snapshot-analysis ``` ## Usage
+```sh dbt_snapshot_analysis ```
```

### Comparing `dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis/data_validation.py` & `dbt_snapshot_analysis-0.2.6/dbt_snapshot_analysis/data_validation.py`

 * *Files identical despite different names*

### Comparing `dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis/dbt_snapshot_analysis.py` & `dbt_snapshot_analysis-0.2.6/dbt_snapshot_analysis/dbt_snapshot_analysis.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 import pandas as pd
 import streamlit as st
 from typing import List
 from datetime import datetime
 import plotly.express as px
 import plotly.graph_objects as go
+import numpy as np
 
 
-from snapshot_utils import (
-    get_metric_by_month,
-    get_snapshot_as_of_date,
-)
+from snapshot_utils import get_metric_by_month, get_snapshot_as_of_date, determine_type
 
 
 @st.cache_data()
-def compute_all_metric_day_by_day(df: pd.DataFrame, date_range: List[str]):
+def compute_all_metric_day_by_day(local_df: pd.DataFrame, date_range: List[str]):
     print("Computing metric day by day...")
-    all_results = pd.DataFrame()
+    all_monthly_metrics = pd.DataFrame()
     progress_text = "Operation in progress. Please wait."
     my_bar = st.progress(0, text=progress_text)
     index = 0
     for day in date_range:
         index += 1
         day_date = datetime.strptime(day, "%Y-%m-%d")
-        current_df = get_snapshot_as_of_date(df, day_date)
+        current_df = get_snapshot_as_of_date(local_df, day_date)
+        if current_df.empty:
+            continue
         metric_by_month = get_metric_by_month(
             current_df, "metric_value", "metric_date", "%Y-%m"
         )
         metric_by_month["computation_day"] = day_date.date()
-        all_results = pd.concat([all_results, metric_by_month], ignore_index=True)
+        all_monthly_metrics = pd.concat(
+            [all_monthly_metrics, metric_by_month], ignore_index=True
+        )
         progress = index / date_range.__len__()
         my_bar.progress(progress, text=progress_text)
 
     my_bar.empty()
-    return all_results
+
+    return all_monthly_metrics
 
 
 def is_numeric_column(df, column_name):
     try:
         pd.to_numeric(df[column_name])
         return True
     except ValueError:
@@ -48,129 +51,233 @@
         pd.to_datetime(df[column_name])
         return True
     except ValueError:
         return False
 
 
 @st.cache_data()
-def parse_uploaded_file(uploaded_file):
+def parse_csv_file(uploaded_file):
+    if uploaded_file is None:
+        return pd.DataFrame()
     print("Parsing uploaded file...")
-    df = pd.read_csv(uploaded_file, low_memory=False)
+    local_df = pd.read_csv(uploaded_file, low_memory=False)
 
+    print(type(local_df["dbt_valid_from"].iloc[0]))
+    datetime_format = determine_type(local_df["dbt_valid_from"].iloc[0])
+    print(f"Date format: {datetime_format}")
     # format dates
     try:
-        df["dbt_valid_from"] = pd.to_datetime(df["dbt_valid_from"], unit="s")
-        now = pd.Timestamp.now().timestamp()
-        df["dbt_valid_to"] = df["dbt_valid_to"].fillna(now)
-        df["dbt_valid_to"] = pd.to_datetime(df["dbt_valid_to"], unit="s")
+        if datetime_format == "timestamp":
+            local_df["is_current_version"] = local_df["dbt_valid_to"].isnull()
+            local_df["dbt_valid_from"] = pd.to_datetime(
+                local_df["dbt_valid_from"], unit="s"
+            )
+            now = pd.Timestamp.now().timestamp()
+            local_df["dbt_valid_to"] = local_df["dbt_valid_to"].fillna(now)
+            local_df["dbt_valid_to"] = pd.to_datetime(
+                local_df["dbt_valid_to"], unit="s"
+            )
+        else:
+            local_df["is_current_version"] = local_df["dbt_valid_to"].isnull()
+            local_df["dbt_valid_from"] = pd.to_datetime(local_df["dbt_valid_from"])
+            now = pd.Timestamp.now().strftime("%Y-%m-%dT%H:%M:%S.%f")
+            local_df["dbt_valid_to"] = local_df["dbt_valid_to"].fillna(now)
+            local_df["dbt_valid_to"] = pd.to_datetime(local_df["dbt_valid_to"])
     except ValueError as e:
         invalid_row_index = int(str(e).split(" ")[-1])
         print(f"Invalid row index: {invalid_row_index}")
 
-    print(f"Number of rows: {df.shape[0]}")
-    print(f"Number of columns: {df.shape[1]}")
-    return df
+    print(f"Number of rows: {local_df.shape[0]}")
+    print(f"Number of columns: {local_df.shape[1]}")
+    return local_df
 
 
 @st.cache_data()
-def get_metric_value_and_date(df, metric_column, date_column):
-    is_numeric_column_valid = is_numeric_column(df, metric_column)
-    is_date_column_valid = is_date_column(df, date_column)
+def get_metric_value_and_date(local_df, metric_column, date_column):
+    is_numeric_column_valid = is_numeric_column(local_df, metric_column)
+    is_date_column_valid = is_date_column(local_df, date_column)
     if is_numeric_column_valid and is_date_column_valid:
-        df["metric_value"] = df[metric_column]
-        df["metric_date"] = df[date_column]
+        local_df["metric_value"] = local_df[metric_column]
+        local_df["metric_date"] = local_df[date_column]
 
-        df = df[(df["metric_date"].notnull()) & (df["metric_value"].notnull())]
+        local_df = local_df[
+            (local_df["metric_date"].notnull()) & (local_df["metric_value"].notnull())
+        ]
     else:
         st.write("Please select a valid metric column and a date column")
-    return df
+    return local_df
 
 
 def run():
-    uploaded_file = st.file_uploader("Choose a file")
-    if uploaded_file is not None:
-        df = parse_uploaded_file(uploaded_file)
-        col1, col2 = st.columns(2)
-        with col1:
-            metric_column = st.selectbox("Select metric column", df.columns)
-            is_numeric_column_valid = is_numeric_column(df, metric_column)
-            if not is_numeric_column_valid:
-                st.warning(
-                    "Please select a valid metric column, it should be a numeric column."
-                )
-
-        with col2:
-            date_column = st.selectbox("Select metric date column", df.columns)
-            is_date_column_valid = is_date_column(df, date_column)
-            if not is_date_column_valid:
-                st.warning(
-                    "Please select a valid date column, it should be supported by pandas.to_datetime."
-                )
+    firstCol1, firstCol2 = st.columns(2)
+    df = pd.DataFrame()
+    with firstCol1:
+        uploaded_file = st.file_uploader("Choose a file")
+
+    with firstCol2:
+        if uploaded_file is not None:
+            df = parse_csv_file(uploaded_file)
+            unique_id_column = st.selectbox("Select unique id column", df.columns)
 
+    if not df.empty:
         tab1, tab2, tab3 = st.tabs(["Version", "Lifespan", "Data"])
         with tab1:
             st.markdown("## Distribution of versions per ID")
             st.header("Version distribution")
-            unique_ids = df.groupby("id").size()
+            unique_ids = df.groupby(unique_id_column).size()
             print(f"Number of unique ids: {unique_ids.shape[0]}")
-            versions_per_id = df.groupby("id").size().reset_index(name="num_versions")
-            versions_count = versions_per_id["num_versions"].value_counts().sort_index()
+            versions_per_id = (
+                df.groupby(unique_id_column).size().reset_index(name="version per id")
+            )
+            versions_count = (
+                versions_per_id["version per id"].value_counts().sort_index()
+            )
 
             st.bar_chart(versions_count)
 
         with tab2:
             lifespandf = df.copy()
             lifespandf["lifespan"] = (
                 lifespandf["dbt_valid_to"] - lifespandf["dbt_valid_from"]
             )
             print(lifespandf["lifespan"].describe())
             lifespandf["lifespan_numeric"] = pd.to_numeric(
                 lifespandf["lifespan"], errors="coerce"
             )
-            lifespandf["lifespan_days"] = lifespandf["lifespan_numeric"] / 86400
-            fig = px.histogram(lifespandf["lifespan_days"], nbins=20)
+            lifespandf["lifespan (days)"] = lifespandf["lifespan"].dt.days
+            print(lifespandf["lifespan (days)"].describe())
+
+            all_versions = lifespandf["lifespan (days)"]
+            dead_versions = lifespandf[lifespandf["is_current_version"] == False][
+                "lifespan (days)"
+            ]
+
+            lifespan_df_with_alive = pd.DataFrame(
+                dict(
+                    series=np.concatenate(
+                        (
+                            ["lifespan all rows (days)"] * len(all_versions),
+                            ["lifespan without active (days)"] * len(dead_versions),
+                        )
+                    ),
+                    data=np.concatenate((all_versions, dead_versions)),
+                )
+            )
+
+            fig = px.histogram(
+                lifespan_df_with_alive,
+                x="data",
+                color="series",
+                barmode="overlay",
+                nbins=50,
+            )
 
             st.plotly_chart(fig, use_container_width=True)
 
         with tab3:
             st.header("Dataframe")
             st.write(df)
 
         min_date = df["dbt_valid_from"].min()
         max_date = df["dbt_valid_from"].max()
         date_range = pd.date_range(start=min_date, end=max_date)
         date_range_str = date_range.strftime("%Y-%m-%d").tolist()
 
+        metric_distribution_df = df.copy()
+
+        col1, col2, col3 = st.columns(3)
+
+        with col1:
+            is_metric_or_count = st.radio("Metric", ["Count", "Sum"])
+
+        with col2:
+            date_column = st.selectbox(
+                "Select metric date column", metric_distribution_df.columns
+            )
+            is_date_column_valid = is_date_column(metric_distribution_df, date_column)
+            if not is_date_column_valid:
+                st.warning(
+                    "Please select a valid date column, it should be supported by pandas.to_datetime."
+                )
+
+        with col3:
+            is_numeric_column_valid = False
+            if is_metric_or_count == "Sum":
+                metric_column = st.selectbox(
+                    "Select metric column to sum", metric_distribution_df.columns
+                )
+                is_numeric_column_valid = is_numeric_column(
+                    metric_distribution_df, metric_column
+                )
+                if not is_numeric_column_valid:
+                    st.warning(
+                        "Please select a valid metric column, it should be a numeric column."
+                    )
+            else:
+                metric_distribution_df["count"] = 1
+                metric_column = "count"
+                is_numeric_column_valid = True
+
         if is_numeric_column_valid and is_date_column_valid:
-            df = get_metric_value_and_date(df, metric_column, date_column)
+            metric_distribution_df_with_formated_date = get_metric_value_and_date(
+                metric_distribution_df, metric_column, date_column
+            )
 
-            all_results = compute_all_metric_day_by_day(df, date_range_str)
+            all_results = compute_all_metric_day_by_day(
+                metric_distribution_df_with_formated_date, date_range_str
+            )
+
+            all_results = all_results[all_results["metric_value"] > 0]
+
+            all_results["latest_value"] = (
+                all_results.sort_values(
+                    ["metric_date", "computation_day"], ascending=[True, False]
+                )
+                .groupby("metric_date")["metric_value"]
+                .transform("first")
+            )
+
+            all_results["relative_value"] = (
+                all_results["metric_value"] / all_results["latest_value"]
+            )
+
+            all_monthly_volatility = (
+                all_results[all_results["metric_value"] > 0]
+                .groupby("metric_date")["relative_value"]
+                .std()
+            )
+
+            print("all_monthly_volatility", all_monthly_volatility)
 
             grouped_df = all_results.groupby("metric_date")
 
             st.set_option("deprecation.showPyplotGlobalUse", False)
             fig = go.Figure()
 
             for metric_name, group in grouped_df:
                 fig.add_trace(
                     go.Scatter(
                         x=group["computation_day"],
-                        y=group["metric_value"],
+                        y=group["relative_value"],
                         name=metric_name,
                     )
                 )
 
             fig.update_layout(
                 title="Metric Value Over Time",
                 xaxis_title="Computation Day",
                 yaxis_title="Metric Value",
                 showlegend=True,
             )
             st.plotly_chart(fig)
 
+            st.subheader("Monthly volatility")
+
+            st.dataframe(all_monthly_volatility)
+
 
 def main():
     run()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis/snapshot_utils.py` & `dbt_snapshot_analysis-0.2.6/dbt_snapshot_analysis/snapshot_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pandas as pd
+import numpy as np
 
 
 def get_snapshot_as_of_date(df: pd.DataFrame, current_day: pd.Timestamp):
     """
     Returns a snapshot of the DataFrame as of a given date.
 
     Parameters:
@@ -16,15 +17,23 @@
     valid_df = df[
         (df["dbt_valid_from"] <= current_day) & (current_day < df["dbt_valid_to"])
     ]
 
     return valid_df
 
 
-import pandas as pd
+def determine_type(input_str):
+    if isinstance(input_str, np.int64):
+        return "timestamp"
+    if isinstance(input_str, np.float64):
+        return "timestamp"
+    if isinstance(input_str, np.float32):
+        return "timestamp"
+    else:
+        return "datetime"
 
 
 def get_metric_by_month(
     df: pd.DataFrame, metric_value_col: str, metric_date_col: str, date_format="%Y-%m"
 ) -> pd.DataFrame:
     """
     Returns a DataFrame with the monthly sum of a metric value column.
@@ -34,11 +43,17 @@
     metric_value_col (str): The name of the column containing the metric values.
     metric_date_col (str): The name of the column containing the metric dates.
 
     Returns:
     pandas.DataFrame: A DataFrame with the monthly sum of the metric value column.
     """
     df_copy = df.copy()
-    df_copy[metric_date_col] = pd.to_datetime(df_copy[metric_date_col], unit="s")
+    df_copy = df_copy[df_copy[metric_value_col].notnull()]
+    df_copy = df_copy[df_copy[metric_date_col].notnull()]
+    date_type = determine_type(df_copy[metric_date_col].iloc[0])
+    if date_type == "timestamp":
+        df_copy[metric_date_col] = pd.to_datetime(df_copy[metric_date_col], unit="s")
+    else:
+        df_copy[metric_date_col] = pd.to_datetime(df_copy[metric_date_col])
     df_copy["metric_date"] = df_copy[metric_date_col].dt.strftime(date_format)
     monthly_sum = df_copy.groupby("metric_date")[metric_value_col].sum().reset_index()
     return monthly_sum
```

### Comparing `dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis.egg-info/PKG-INFO` & `dbt_snapshot_analysis-0.2.6/dbt_snapshot_analysis.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-snapshot-analysis
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package for analyzing snapshots
 Home-page: https://github.com/data-drift/dbt-snapshot-analytics
 Author: Sammy Teillet
 Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,15 @@
 
 This project is developped by the DataDrift team.
 
 DBT Snapshot Analysis is a Python package for analyzing snapshots. It provides a set of tools for visualizing and exploring data in a variety of ways.
 
 ## Installation
 
-You can install Plot Analysis using `pip`:
+You can install DBT Snapshot Analysis using `pip`:
 
 ```sh
 pip install dbt-snapshot-analysis
 ```
 
 ## Usage
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_s0gvmt88_/tmpn8l276xj_TarContainer/0/10", line 21, column 2: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_s0gvmt88_/tmpn8l276xj_TarContainer/0/10", line 21, column 2: Levels of opening and closing headings don't match*

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: dbt-snapshot-analysis Version: 0.2.5 Summary: A
+Metadata-Version: 2.1 Name: dbt-snapshot-analysis Version: 0.2.6 Summary: A
 package for analyzing snapshots Home-page: https://github.com/data-drift/dbt-
 snapshot-analytics Author: Sammy Teillet Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
                                [DataDrift_logo]
                        ***** A Changelog for Data *****
                       Git-Based. Data-Consumer-Friendly.
                                 Website Â· Blog
 # DBT Snapshot Analysis [![PyPI version](https://badge.fury.io/py/dbt-snapshot-
 analysis.svg)](https://badge.fury.io/py/dbt-snapshot-analysis) This project is
 developped by the DataDrift team. DBT Snapshot Analysis is a Python package for
 analyzing snapshots. It provides a set of tools for visualizing and exploring
-data in a variety of ways. ## Installation You can install Plot Analysis using
-`pip`: ```sh pip install dbt-snapshot-analysis ``` ## Usage ```sh
-dbt_snapshot_analysis ```
+data in a variety of ways. ## Installation You can install DBT Snapshot
+Analysis using `pip`: ```sh pip install dbt-snapshot-analysis ``` ## Usage
+```sh dbt_snapshot_analysis ```
```

### Comparing `dbt_snapshot_analysis-0.2.5/setup.py` & `dbt_snapshot_analysis-0.2.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dbt_snapshot_analysis",
-    version="0.2.5",
+    version="0.2.6",
     packages=find_packages(),
     py_modules=["dbt_snapshot_analysis"],
     install_requires=["pandas", "plotly", "streamlit"],
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     entry_points={
         "console_scripts": [
```

