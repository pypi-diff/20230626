# Comparing `tmp/plottah-0.1.3.tar.gz` & `tmp/plottah-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plottah-0.1.3.tar", max compression
+gzip compressed data, was "plottah-0.1.5.tar", max compression
```

## Comparing `plottah-0.1.3.tar` & `plottah-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      835 2023-06-22 12:52:22.561511 plottah-0.1.3/README.md
--rw-r--r--   0        0        0       22 2023-06-22 11:30:53.499061 plottah-0.1.3/plottah/__init__.py
--rw-r--r--   0        0        0     1012 2023-06-22 12:44:11.607614 plottah-0.1.3/plottah/__main__.py
--rw-r--r--   0        0        0     1339 2023-06-19 19:34:19.357898 plottah-0.1.3/plottah/colors.py
--rw-r--r--   0        0        0     3056 2023-06-22 09:19:12.089888 plottah-0.1.3/plottah/config.py
--rw-r--r--   0        0        0      988 2023-06-22 09:55:14.056657 plottah-0.1.3/plottah/main.py
--rw-r--r--   0        0        0       24 2023-06-20 17:12:04.651705 plottah-0.1.3/plottah/plot_builder/__init__.py
--rw-r--r--   0        0        0     2684 2023-06-22 12:58:33.986776 plottah-0.1.3/plottah/plot_builder/builders.py
--rw-r--r--   0        0        0     7488 2023-06-22 12:44:18.976051 plottah-0.1.3/plottah/plot_handler/PlotHandler.py
--rw-r--r--   0        0        0       37 2023-06-20 17:27:02.673177 plottah-0.1.3/plottah/plot_handler/__init__.py
--rw-r--r--   0        0        0     7530 2023-06-22 12:44:22.633547 plottah-0.1.3/plottah/plots/BinEventRatePlot.py
--rw-r--r--   0        0        0     3987 2023-06-22 12:44:23.133501 plottah-0.1.3/plottah/plots/DistPlot.py
--rw-r--r--   0        0        0     1927 2023-06-22 07:41:05.603043 plottah-0.1.3/plottah/plots/PlotProtocol.py
--rw-r--r--   0        0        0     3578 2023-06-22 12:44:24.105798 plottah-0.1.3/plottah/plots/RocCurvePlot.py
--rw-r--r--   0        0        0      117 2023-06-16 12:50:48.680563 plottah-0.1.3/plottah/plots/__init__.py
--rw-r--r--   0        0        0     4050 2023-06-16 12:25:45.788578 plottah-0.1.3/plottah/utils.py
--rw-r--r--   0        0        0      505 2023-06-26 11:25:35.065446 plottah-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1824 1970-01-01 00:00:00.000000 plottah-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      835 2023-06-26 14:13:16.672074 plottah-0.1.5/README.md
+-rw-r--r--   0        0        0       22 2023-06-26 14:13:18.148086 plottah-0.1.5/plottah/__init__.py
+-rw-r--r--   0        0        0     1012 2023-06-26 14:13:18.148086 plottah-0.1.5/plottah/__main__.py
+-rw-r--r--   0        0        0     1339 2023-06-26 14:13:18.148086 plottah-0.1.5/plottah/colors.py
+-rw-r--r--   0        0        0     3124 2023-06-26 14:13:18.148086 plottah-0.1.5/plottah/config.py
+-rw-r--r--   0        0        0      988 2023-06-26 14:13:18.148086 plottah-0.1.5/plottah/main.py
+-rw-r--r--   0        0        0       24 2023-06-26 14:13:18.148086 plottah-0.1.5/plottah/plot_builder/__init__.py
+-rw-r--r--   0        0        0     2684 2023-06-26 14:13:18.148086 plottah-0.1.5/plottah/plot_builder/builders.py
+-rw-r--r--   0        0        0     7487 2023-06-26 14:13:18.148086 plottah-0.1.5/plottah/plot_handler/PlotHandler.py
+-rw-r--r--   0        0        0       37 2023-06-26 14:13:18.148086 plottah-0.1.5/plottah/plot_handler/__init__.py
+-rw-r--r--   0        0        0     7584 2023-06-26 14:13:18.152086 plottah-0.1.5/plottah/plots/BinEventRatePlot.py
+-rw-r--r--   0        0        0     3987 2023-06-26 14:13:18.152086 plottah-0.1.5/plottah/plots/DistPlot.py
+-rw-r--r--   0        0        0     1927 2023-06-26 14:13:18.152086 plottah-0.1.5/plottah/plots/PlotProtocol.py
+-rw-r--r--   0        0        0     3578 2023-06-26 14:13:18.152086 plottah-0.1.5/plottah/plots/RocCurvePlot.py
+-rw-r--r--   0        0        0      117 2023-06-26 14:13:18.152086 plottah-0.1.5/plottah/plots/__init__.py
+-rw-r--r--   0        0        0     4200 2023-06-26 14:13:18.152086 plottah-0.1.5/plottah/utils.py
+-rw-r--r--   0        0        0      505 2023-06-26 14:13:56.280349 plottah-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1824 1970-01-01 00:00:00.000000 plottah-0.1.5/PKG-INFO
```

### Comparing `plottah-0.1.3/README.md` & `plottah-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `plottah-0.1.3/plottah/__main__.py` & `plottah-0.1.5/plottah/__main__.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.3/plottah/colors.py` & `plottah-0.1.5/plottah/colors.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.3/plottah/config.py` & `plottah-0.1.5/plottah/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,15 +91,16 @@
         if v not in sample_df.columns:
             raise ValueError(
                 f"Column: {v} does not exist is dataframe \n Please ensure the config.yaml contains only valid columns"
             )
         return v
 
 
+# config = parse_from_yaml(str(ROOT_DIR / "config_bank.yaml"))
 config = parse_from_yaml(str(ROOT_DIR / "config.yaml"))
 settings = Settings(**config)
 
 if __name__ == "__main__":
-    config = parse_from_yaml(str(ROOT_DIR / "config.yaml"))
+    config = parse_from_yaml(str(ROOT_DIR / "config_bank.yaml"))
     print(config)
     settings = Settings(**config)
     print(settings)
```

### Comparing `plottah-0.1.3/plottah/main.py` & `plottah-0.1.5/plottah/main.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.3/plottah/plot_builder/builders.py` & `plottah-0.1.5/plottah/plot_builder/builders.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.3/plottah/plot_handler/PlotHandler.py` & `plottah-0.1.5/plottah/plot_handler/PlotHandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             ),
             margin=dict(t=40),
             title_x=0.5,
             width=1000,
             height=800,
             legend=dict(
                 # the below if through experimentation
-                x=0.94,
+                x=1.1,
                 y=0.36 + (1 - self.legend_xref) * 0.57,
                 xanchor="right",
                 yanchor="bottom",
             ),
         )
 
     def build_subplot(self, subplot: PlotProtocol, row: int, col: int):
```

### Comparing `plottah-0.1.3/plottah/plots/BinEventRatePlot.py` & `plottah-0.1.5/plottah/plots/BinEventRatePlot.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
                 self.target_col,
                 min_val_adj,
                 max_val_adj,
                 n_bins=self.n_bins,
                 method=method,
             )
         )
+        print(self.bins)
         # convert type to list
         self.bins = list(self.bins)
 
         # set first and last value back to min and max before imputing
         self.bins[0] = min_val
         self.bins[self.n_bins - 1] = max_val
 
@@ -93,14 +94,15 @@
                 )
             )
         except Exception as e:
             raise ValueError("{self.feature_col} cannot be binned")
 
         # Create plot labels: [(4, 6), (6, 10), ...]
         self.labels = get_labels_from_bins(self.bins)
+        print(self.labels)
 
         ## CLIPPING
 
         # Clip values according to min/max values
         df[feature_col].clip(lower=min_val, upper=max_val, inplace=True)
 
         # Ensure clipping values does not remove all but a single value
@@ -209,15 +211,15 @@
             tickangle=22.5,
         )
 
     def get_y_axes_layout(self, row, col):
         return dict(
             title_text=f"Fraction of Observations",
             title_font={"size": 12},
-            range=[0, 1.2 * self.df_binned[f"{self.feature_col}_len"].max()],
+            # range=[0, 1.2 * self.df_binned[f"{self.feature_col}_len"].max()],
             row=row,
             col=col,
             title_standoff=5,  # decrease space between title and plot
         )
 
     def get_secondary_y_axis_title(self):
         return "Event Rate"
```

### Comparing `plottah-0.1.3/plottah/plots/DistPlot.py` & `plottah-0.1.5/plottah/plots/DistPlot.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.3/plottah/plots/PlotProtocol.py` & `plottah-0.1.5/plottah/plots/PlotProtocol.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.3/plottah/plots/RocCurvePlot.py` & `plottah-0.1.5/plottah/plots/RocCurvePlot.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.3/plottah/utils.py` & `plottah-0.1.5/plottah/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,12 +136,17 @@
 
 def get_labels_from_bins(bins: list) -> list:
     """
     generate labels from bins
 
     example: [0, 1, 2] -> ['(0.00, 1.00]', '(1.00, 2.00]']
     """
+
+    precision = 2
+    while len(bins) > len(np.unique(np.round(bins, precision))):
+        precision += 1
+
     labels = [
-        f'({"{:,.2f}".format(bins[i])}, {"{:,.2f}".format(bins[i+1])}]'
+        f'({"{:,.{prec}f}".format(bins[i], prec=precision)}, {"{:,.{prec}f}".format(bins[i+1], prec=precision)}]'
         for i in range(len(bins) - 1)
     ]
     return labels
```

### Comparing `plottah-0.1.3/PKG-INFO` & `plottah-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plottah
-Version: 0.1.3
+Version: 0.1.5
 Summary: 
 Author: Niels Ota
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

