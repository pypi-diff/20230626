# Comparing `tmp/influxdb3-python-cli-0.1.1.tar.gz` & `tmp/influxdb3-python-cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxdb3-python-cli-0.1.1.tar", last modified: Mon Jun  5 17:39:02 2023, max compression
+gzip compressed data, was "influxdb3-python-cli-0.2.0.tar", last modified: Mon Jun 26 11:17:34 2023, max compression
```

## Comparing `influxdb3-python-cli-0.1.1.tar` & `influxdb3-python-cli-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:39:02.100865 influxdb3-python-cli-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 17:38:52.000000 influxdb3-python-cli-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-05 17:39:02.100865 influxdb3-python-cli-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-06-05 17:38:52.000000 influxdb3-python-cli-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:39:02.100865 influxdb3-python-cli-0.1.1/influxdb3_python_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-05 17:39:02.000000 influxdb3-python-cli-0.1.1/influxdb3_python_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-05 17:39:02.000000 influxdb3-python-cli-0.1.1/influxdb3_python_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:39:02.000000 influxdb3-python-cli-0.1.1/influxdb3_python_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-05 17:39:02.000000 influxdb3-python-cli-0.1.1/influxdb3_python_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-05 17:39:02.000000 influxdb3-python-cli-0.1.1/influxdb3_python_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 17:39:02.000000 influxdb3-python-cli-0.1.1/influxdb3_python_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:39:02.100865 influxdb3-python-cli-0.1.1/influxdb_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:38:52.000000 influxdb3-python-cli-0.1.1/influxdb_cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7599 2023-06-05 17:38:52.000000 influxdb3-python-cli-0.1.1/influxdb_cli/influx3.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 17:39:02.100865 influxdb3-python-cli-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-05 17:38:52.000000 influxdb3-python-cli-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:17:34.114022 influxdb3-python-cli-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-26 11:17:20.000000 influxdb3-python-cli-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-26 11:17:34.114022 influxdb3-python-cli-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-06-26 11:17:20.000000 influxdb3-python-cli-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:17:34.114022 influxdb3-python-cli-0.2.0/influxdb3_python_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-26 11:17:34.000000 influxdb3-python-cli-0.2.0/influxdb3_python_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-26 11:17:34.000000 influxdb3-python-cli-0.2.0/influxdb3_python_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 11:17:34.000000 influxdb3-python-cli-0.2.0/influxdb3_python_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-26 11:17:34.000000 influxdb3-python-cli-0.2.0/influxdb3_python_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 11:17:34.000000 influxdb3-python-cli-0.2.0/influxdb3_python_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 11:17:34.000000 influxdb3-python-cli-0.2.0/influxdb3_python_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:17:34.114022 influxdb3-python-cli-0.2.0/influxdb_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 11:17:20.000000 influxdb3-python-cli-0.2.0/influxdb_cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8351 2023-06-26 11:17:20.000000 influxdb3-python-cli-0.2.0/influxdb_cli/influx3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 11:17:34.114022 influxdb3-python-cli-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-26 11:17:20.000000 influxdb3-python-cli-0.2.0/setup.py
```

### Comparing `influxdb3-python-cli-0.1.1/LICENSE` & `influxdb3-python-cli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `influxdb3-python-cli-0.1.1/PKG-INFO` & `influxdb3-python-cli-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python-cli
-Version: 0.1.1
+Version: 0.2.0
 Summary: Community Python client for InfluxDB 3.0 (CLI)
 Home-page: https://github.com/InfluxCommunity/influxdb-python-cli
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.2.0 Summary:
 Community Python client for InfluxDB 3.0 (CLI) Home-page: https://github.com/
 InfluxCommunity/influxdb-python-cli Author: InfluxData Author-email:
 contact@influxdata.com Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `influxdb3-python-cli-0.1.1/README.md` & `influxdb3-python-cli-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `influxdb3-python-cli-0.1.1/influxdb3_python_cli.egg-info/PKG-INFO` & `influxdb3-python-cli-0.2.0/influxdb3_python_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python-cli
-Version: 0.1.1
+Version: 0.2.0
 Summary: Community Python client for InfluxDB 3.0 (CLI)
 Home-page: https://github.com/InfluxCommunity/influxdb-python-cli
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.2.0 Summary:
 Community Python client for InfluxDB 3.0 (CLI) Home-page: https://github.com/
 InfluxCommunity/influxdb-python-cli Author: InfluxData Author-email:
 contact@influxdata.com Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `influxdb3-python-cli-0.1.1/influxdb_cli/influx3.py` & `influxdb3-python-cli-0.2.0/influxdb_cli/influx3.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/usr/bin/env python3
 
 import cmd, ast
 import argparse
-from flightsql import FlightSQLClient
 import json
 from prompt_toolkit import PromptSession
 from prompt_toolkit.lexers import PygmentsLexer
 from pygments.lexers import SqlLexer
 from influxdb_client_3 import InfluxDBClient3
 import os
 
@@ -40,14 +39,24 @@
             return
         try: 
             table = self.influxdb_client.query(query=arg, language="sql")
             print(table.to_pandas().to_markdown())
         except Exception as e:
             print(e)
 
+    def do_influxql(self, arg):
+        if self._configurations == {}:
+            print("can't query, no active configs")
+            return
+        try: 
+            table = self.influxdb_client.query(query=arg, language="influxql")
+            print(table.to_pandas().to_markdown())
+        except Exception as e:
+            print(e)
+
     def do_write(self, arg):
         if self._configurations == {}:
             print("can't write, no active configs")
             return
         if arg == "":
             print("can't write, no line protocol supplied")
             return
@@ -86,14 +95,17 @@
         return self.do_exit(arg)
 
  
     def precmd(self, line):
         if line.strip() == 'sql':
             self._run_prompt_loop('(sql >) ', self.do_sql, 'SQL mode')
             return ''
+        if line.strip() == 'influxql':
+            self._run_prompt_loop('(influxql >) ', self.do_influxql, 'INFLUXQL mode')
+            return ''
         if line.strip() == 'write':
             self._run_prompt_loop('(write >) ', self.do_write, 'write mode')
             return ''
         return line
 
     def _run_prompt_loop(self, prompt, action, mode_name):
         prompt_session = self._sql_prompt_session if mode_name == 'SQL mode' else self._write_prompt_session
@@ -162,14 +174,16 @@
 def parse_args():
     parser = argparse.ArgumentParser(description= _description_string
                                      )
     subparsers = parser.add_subparsers(dest='command')
 
     sql_parser = subparsers.add_parser('sql', help='execute the given SQL query')
     sql_parser.add_argument('query', metavar='QUERY', nargs='*', action=StoreRemainingInput, help='the SQL query to execute')
+    influxql_parser = subparsers.add_parser('influxql', help='execute the given InfluxQL query')
+    influxql_parser.add_argument('query', metavar='QUERY', nargs='*', action=StoreRemainingInput, help='the INFLUXQL query to execute')
 
     write_parser = subparsers.add_parser('write', help='write line protocol to InfluxDB')
     write_parser.add_argument('line_protocol', metavar='LINE PROTOCOL',  nargs='*', action=StoreRemainingInput, help='the data to write')
 
     write_csv_parser = subparsers.add_parser('write_csv', help='write CSV data to InfluxDB')
     write_csv_parser.add_argument('--file', help='the CSV file to import', required=True)
     write_csv_parser.add_argument('--measurement', help='Define the name of the measurement', required=True)
@@ -189,14 +203,16 @@
 
 def main():
     args = parse_args()
     app = IOXCLI()
 
     if args.command == 'sql':
         app.do_sql(args.query)
+    if args.command == 'influxql':
+        app.do_influxql(args.query)
     if args.command == 'write':
         app.do_write(args.line_protocol)
     if args.command == 'write_csv':
         app.do_write_csv(args)
     if args.command == 'config':
         app.config(args)
     if args.command == 'help':
```

### Comparing `influxdb3-python-cli-0.1.1/setup.py` & `influxdb3-python-cli-0.2.0/setup.py`

 * *Files identical despite different names*

