# Comparing `tmp/tibis-1.0.6.tar.gz` & `tmp/tibis-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tibis-1.0.6.tar", max compression
+gzip compressed data, was "tibis-1.0.7.tar", max compression
```

## Comparing `tibis-1.0.6.tar` & `tibis-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1317 2022-05-04 07:11:06.352528 tibis-1.0.6/LICENSE
--rw-r--r--   0        0        0     3298 2023-03-07 15:28:13.653463 tibis-1.0.6/README.md
--rw-r--r--   0        0        0      499 2023-05-30 15:54:32.843837 tibis-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     1602 2022-05-04 07:11:06.355861 tibis-1.0.6/tibis/lib/args_parser.py
--rw-r--r--   0        0        0     4972 2023-03-06 20:46:55.708576 tibis-1.0.6/tibis/lib/common.py
--rw-r--r--   0        0        0      366 2022-11-15 15:00:51.186221 tibis-1.0.6/tibis/lib/config.py
--rw-r--r--   0        0        0     2956 2022-11-15 15:00:41.092868 tibis-1.0.6/tibis/lib/create.py
--rw-r--r--   0        0        0      935 2022-05-04 07:11:06.355861 tibis-1.0.6/tibis/lib/delete.py
--rw-r--r--   0        0        0     1267 2022-05-04 07:40:49.614937 tibis-1.0.6/tibis/lib/first_time.py
--rw-r--r--   0        0        0      562 2022-05-04 07:11:06.355861 tibis-1.0.6/tibis/lib/list.py
--rw-r--r--   0        0        0     1054 2022-05-04 08:17:44.853283 tibis-1.0.6/tibis/lib/lock.py
--rw-r--r--   0        0        0      540 2022-05-04 07:11:06.355861 tibis-1.0.6/tibis/lib/logger.py
--rw-r--r--   0        0        0     1180 2023-05-30 15:54:51.797261 tibis-1.0.6/tibis/lib/static.py
--rw-r--r--   0        0        0     1643 2023-03-07 09:14:53.679647 tibis-1.0.6/tibis/lib/unlock.py
--rw-r--r--   0        0        0      729 2022-05-04 07:28:38.614261 tibis-1.0.6/tibis/tibis.py
--rw-r--r--   0        0        0     4055 1970-01-01 00:00:00.000000 tibis-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1317 2022-05-04 07:11:06.352528 tibis-1.0.7/LICENSE
+-rw-r--r--   0        0        0     3298 2023-03-07 15:28:13.653463 tibis-1.0.7/README.md
+-rw-r--r--   0        0        0      517 2023-06-26 08:40:39.216624 tibis-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1582 2023-06-26 08:37:09.179153 tibis-1.0.7/tibis/lib/args_parser.py
+-rw-r--r--   0        0        0     7881 2023-06-07 17:23:03.849883 tibis-1.0.7/tibis/lib/common.py
+-rw-r--r--   0        0        0      542 2023-06-05 05:21:48.691631 tibis-1.0.7/tibis/lib/config.py
+-rw-r--r--   0        0        0     2956 2022-11-15 15:00:41.092868 tibis-1.0.7/tibis/lib/create.py
+-rw-r--r--   0        0        0      935 2022-05-04 07:11:06.355861 tibis-1.0.7/tibis/lib/delete.py
+-rw-r--r--   0        0        0     1267 2022-05-04 07:40:49.614937 tibis-1.0.7/tibis/lib/first_time.py
+-rw-r--r--   0        0        0      562 2022-05-04 07:11:06.355861 tibis-1.0.7/tibis/lib/list.py
+-rw-r--r--   0        0        0     1431 2023-06-05 07:02:14.055365 tibis-1.0.7/tibis/lib/lock.py
+-rw-r--r--   0        0        0      540 2022-05-04 07:11:06.355861 tibis-1.0.7/tibis/lib/logger.py
+-rw-r--r--   0        0        0     1203 2023-06-26 08:40:28.923238 tibis-1.0.7/tibis/lib/static.py
+-rw-r--r--   0        0        0     1643 2023-03-07 09:14:53.679647 tibis-1.0.7/tibis/lib/unlock.py
+-rw-r--r--   0        0        0      729 2022-05-04 07:28:38.614261 tibis-1.0.7/tibis/tibis.py
+-rw-r--r--   0        0        0     4094 1970-01-01 00:00:00.000000 tibis-1.0.7/PKG-INFO
```

### Comparing `tibis-1.0.6/LICENSE` & `tibis-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tibis-1.0.6/README.md` & `tibis-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `tibis-1.0.6/tibis/lib/args_parser.py` & `tibis-1.0.7/tibis/lib/args_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from tibis.lib.list import list
 from tibis.lib.delete import delete
 from tibis.lib.static import version,codename
 import tibis.lib.logger as log
 
 def args_parser():
 
-	parser = argparse.ArgumentParser(exit_on_error=False,description=f"""
+	parser = argparse.ArgumentParser(description=f"""
 		   _   _   _   _   _  
 		  / \ / \ / \ / \ / \ 
 		 ( t | i | b | i | s )
 		  \_/ \_/ \_/ \_/ \_/	
 
 	A cool tool to manage encrypted directory
     Version : {version} Codename : {codename}""",
```

### Comparing `tibis-1.0.6/tibis/lib/create.py` & `tibis-1.0.7/tibis/lib/create.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.6/tibis/lib/delete.py` & `tibis-1.0.7/tibis/lib/delete.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.6/tibis/lib/first_time.py` & `tibis-1.0.7/tibis/lib/first_time.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.6/tibis/lib/list.py` & `tibis-1.0.7/tibis/lib/list.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.6/tibis/lib/logger.py` & `tibis-1.0.7/tibis/lib/logger.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.6/tibis/lib/static.py` & `tibis-1.0.7/tibis/lib/static.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-version  = '1.0.6'
+version  = '1.0.7'
 codename = "Ibis is born"
 
 tibis_config_file="config.yml"
 tibis_config_location=str(Path.home())+"/.config/tibis/"
 tibis_full_config_location=tibis_config_location+tibis_config_file
 
 tibis_keys_location=tibis_config_location+"keys"
@@ -23,9 +23,9 @@
 tibis_database_insert=""" INSERT INTO tibis(name,private_key_path,public_key_path,status,mount_point) VALUES(?,?,?,?,?) """
 tibis_database_list_all="""SELECT name,private_key_path,public_key_path,status,mount_point FROM tibis"""
 
 tibis_empty_dir="/tmp/tempate_tibis_empty_dir"
 tibis_storage_path="/tmp/storage"
 tibis_tmp_dir="/tmp/tibis_tmp"
 
-default_config={'storage_path':tibis_storage_path,'keys_location':tibis_keys_location,'pgp_infos':{'email':'tibis@localhost.org','comment':'Tibis Key','name':'Tibis'}}
+default_config={'storage_path':tibis_storage_path,'keys_location':tibis_keys_location,'pgp_infos':{'email':'tibis@localhost.org','comment':'Tibis Key','name':'Tibis'},'check_integrity':True}
```

### Comparing `tibis-1.0.6/tibis/lib/unlock.py` & `tibis-1.0.7/tibis/lib/unlock.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.6/tibis/tibis.py` & `tibis-1.0.7/tibis/tibis.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.6/PKG-INFO` & `tibis-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: tibis
-Version: 1.0.6
+Version: 1.0.7
 Summary: Tibis is a secure storage manager
 Home-page: https://github.com/shoxxdj/tibis
 Author: shoxxdj
 Author-email: shoxx@shoxxdj.fr
 Requires-Python: >=3.6
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PGPy (>=0.6.0,<0.7.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: pyspin (>=1.1.1,<2.0.0)
 Requires-Dist: simple-chalk (>=0.1.0,<0.2.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Tibis
 
 ![image](https://user-images.githubusercontent.com/5250807/166554591-47e85ac2-2f59-4e33-ba95-a76f2ea41818.png)
```

