# Comparing `tmp/ngdataenginterface-0.1.1.tar.gz` & `tmp/ngdataenginterface-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngdataenginterface-0.1.1.tar", max compression
+gzip compressed data, was "ngdataenginterface-0.1.2.tar", max compression
```

## Comparing `ngdataenginterface-0.1.1.tar` & `ngdataenginterface-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2934 2023-06-05 14:05:20.107219 ngdataenginterface-0.1.1/README.md
--rw-r--r--   0        0        0      348 2023-06-05 14:05:20.107219 ngdataenginterface-0.1.1/ngdataenginterface/__init__.py
--rw-r--r--   0        0        0     3778 2023-06-05 14:05:20.107219 ngdataenginterface-0.1.1/ngdataenginterface/analytical.py
--rw-r--r--   0        0        0     3392 2023-06-05 14:05:20.107219 ngdataenginterface-0.1.1/ngdataenginterface/aws_interface.py
--rw-r--r--   0        0        0     2704 2023-06-05 14:05:20.107219 ngdataenginterface-0.1.1/ngdataenginterface/process.py
--rw-r--r--   0        0        0      517 2023-06-05 14:05:20.107219 ngdataenginterface-0.1.1/ngdataenginterface/scripts/__init__.py
--rw-r--r--   0        0        0     2124 2023-06-05 14:05:20.107219 ngdataenginterface-0.1.1/ngdataenginterface/scripts/create_analytical_tables.py
--rw-r--r--   0        0        0     1516 2023-06-05 14:05:20.107219 ngdataenginterface-0.1.1/ngdataenginterface/scripts/landing_to_raw.py
--rw-r--r--   0        0        0     2015 2023-06-05 14:05:20.107219 ngdataenginterface-0.1.1/ngdataenginterface/scripts/raw_to_trusted.py
--rw-r--r--   0        0        0     1508 2023-06-05 14:05:20.108219 ngdataenginterface-0.1.1/ngdataenginterface/scripts/trusted_to_analytics.py
--rw-r--r--   0        0        0     1836 2023-06-05 14:05:20.108219 ngdataenginterface-0.1.1/ngdataenginterface/spark_manager.py
--rw-r--r--   0        0        0    13379 2023-06-05 14:05:20.108219 ngdataenginterface-0.1.1/ngdataenginterface/table.py
--rw-r--r--   0        0        0     2720 2023-06-05 14:05:20.108219 ngdataenginterface-0.1.1/ngdataenginterface/utils.py
--rw-r--r--   0        0        0      395 2023-06-05 14:05:20.108219 ngdataenginterface-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 ngdataenginterface-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2934 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/README.md
+-rw-r--r--   0        0        0      348 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/__init__.py
+-rw-r--r--   0        0        0     3778 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/analytical.py
+-rw-r--r--   0        0        0     3392 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/aws_interface.py
+-rw-r--r--   0        0        0     2704 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/process.py
+-rw-r--r--   0        0        0      517 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/scripts/__init__.py
+-rw-r--r--   0        0        0     2124 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/scripts/create_analytical_tables.py
+-rw-r--r--   0        0        0     1516 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/scripts/landing_to_raw.py
+-rw-r--r--   0        0        0     2015 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/scripts/raw_to_trusted.py
+-rw-r--r--   0        0        0     1508 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/scripts/trusted_to_analytics.py
+-rw-r--r--   0        0        0     1850 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/spark_manager.py
+-rw-r--r--   0        0        0    13389 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/table.py
+-rw-r--r--   0        0        0     2720 2023-06-26 16:53:29.874136 ngdataenginterface-0.1.2/ngdataenginterface/utils.py
+-rw-r--r--   0        0        0      395 2023-06-26 16:53:29.875136 ngdataenginterface-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 ngdataenginterface-0.1.2/PKG-INFO
```

### Comparing `ngdataenginterface-0.1.1/README.md` & `ngdataenginterface-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.1/ngdataenginterface/analytical.py` & `ngdataenginterface-0.1.2/ngdataenginterface/analytical.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.1/ngdataenginterface/aws_interface.py` & `ngdataenginterface-0.1.2/ngdataenginterface/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.1/ngdataenginterface/process.py` & `ngdataenginterface-0.1.2/ngdataenginterface/process.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.1/ngdataenginterface/scripts/__init__.py` & `ngdataenginterface-0.1.2/ngdataenginterface/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.1/ngdataenginterface/scripts/create_analytical_tables.py` & `ngdataenginterface-0.1.2/ngdataenginterface/scripts/create_analytical_tables.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.1/ngdataenginterface/scripts/landing_to_raw.py` & `ngdataenginterface-0.1.2/ngdataenginterface/scripts/landing_to_raw.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.1/ngdataenginterface/scripts/raw_to_trusted.py` & `ngdataenginterface-0.1.2/ngdataenginterface/scripts/raw_to_trusted.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.1/ngdataenginterface/scripts/trusted_to_analytics.py` & `ngdataenginterface-0.1.2/ngdataenginterface/scripts/trusted_to_analytics.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.1/ngdataenginterface/spark_manager.py` & `ngdataenginterface-0.1.2/ngdataenginterface/spark_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from pyspark import SQLContext
 from pyspark.sql import SparkSession
 from pyspark.conf import SparkConf
 
 
 class SparkManager:
-    def set_spark_config(self, name, aws_access_key_id=None, aws_secret_access_key=None):
+    def set_spark_config(
+        self, name, aws_access_key_id=None, aws_secret_access_key=None
+    ):
         # Create a SparkConf object and set the application name
         config = SparkConf().setAppName(name)
 
         # Set the Parquet datetimeRebaseModeInRead, datetimeRebaseModeInWrite, and int96RebaseModeInWrite to "LEGACY"
         config.set("spark.sql.parquet.datetimeRebaseModeInRead", "LEGACY")
         config.set("spark.sql.parquet.datetimeRebaseModeInWrite", "LEGACY")
         config.set("spark.sql.parquet.int96RebaseModeInWrite", "LEGACY")
```

### Comparing `ngdataenginterface-0.1.1/ngdataenginterface/table.py` & `ngdataenginterface-0.1.2/ngdataenginterface/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,24 +389,26 @@
         path = self.table_url()
         logging.debug("Table path: %s", path)
         # Get the file type
         file_type = self.path.file_type
         # Split the partition string into individual partitions
         partitions = self.path.partition.split("/")
 
+        # Write the schema
+        try:
+            self.write_schema(df)
+        except Exception as e:
+            raise ValueError("Error writing schema: {}".format(str(e)))
+
         # Check if the table should be saved partitioned
         if partitions != [""]:
             for part in partitions:
                 # Add the partition column in the table
                 df = df.withColumn(part, lit(PARTITION_MAP[part](self.meta.date)))
             # Write the table partitioned
             df.write.partitionBy(partitions).mode("append").format(file_type).save(path)
             # df.show()
         else:
             # Write the table without partition
             df.write.mode("append").format(file_type).save(path)
 
-        # Write the schema
-        try:
-            self.write_schema(df)
-        except Exception as e:
-            raise ValueError("Error writing schema: {}".format(str(e)))
+
```

### Comparing `ngdataenginterface-0.1.1/ngdataenginterface/utils.py` & `ngdataenginterface-0.1.2/ngdataenginterface/utils.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.1/PKG-INFO` & `ngdataenginterface-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngdataenginterface
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for facilitating the development of data engineering pipelines
 Author: NG.CASH
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

