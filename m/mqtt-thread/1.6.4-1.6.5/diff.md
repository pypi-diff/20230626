# Comparing `tmp/mqtt_thread-1.6.4.tar.gz` & `tmp/mqtt_thread-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqtt_thread-1.6.4.tar", last modified: Mon May 15 13:47:32 2023, max compression
+gzip compressed data, was "mqtt_thread-1.6.5.tar", last modified: Mon Jun 26 16:27:22 2023, max compression
```

## Comparing `mqtt_thread-1.6.4.tar` & `mqtt_thread-1.6.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 13:47:32.123537 mqtt_thread-1.6.4/
--rw-rw-rw-   0        0        0     1088 2021-02-01 10:36:06.000000 mqtt_thread-1.6.4/LICENCE
--rw-rw-rw-   0        0        0     3720 2023-05-15 13:47:32.123537 mqtt_thread-1.6.4/PKG-INFO
--rw-rw-rw-   0        0        0     3320 2023-02-25 23:15:51.000000 mqtt_thread-1.6.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 13:47:32.108567 mqtt_thread-1.6.4/mqtt_thread/
--rw-rw-rw-   0        0        0     8032 2023-05-15 13:44:49.000000 mqtt_thread-1.6.4/mqtt_thread/MQTT_Thread.py
--rw-rw-rw-   0        0        0     5772 2023-02-22 15:29:07.000000 mqtt_thread-1.6.4/mqtt_thread/MQTT_Thread_bak.py
--rw-rw-rw-   0        0        0       51 2021-02-01 20:48:52.000000 mqtt_thread-1.6.4/mqtt_thread/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 13:47:32.123537 mqtt_thread-1.6.4/mqtt_thread.egg-info/
--rw-rw-rw-   0        0        0     3720 2023-05-15 13:47:32.000000 mqtt_thread-1.6.4/mqtt_thread.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-05-15 13:47:32.000000 mqtt_thread-1.6.4/mqtt_thread.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 13:47:32.000000 mqtt_thread-1.6.4/mqtt_thread.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-15 13:47:32.000000 mqtt_thread-1.6.4/mqtt_thread.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-15 13:47:32.000000 mqtt_thread-1.6.4/mqtt_thread.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 13:47:32.123537 mqtt_thread-1.6.4/setup.cfg
--rw-rw-rw-   0        0        0      764 2023-05-15 13:46:32.000000 mqtt_thread-1.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 16:27:22.211487 mqtt_thread-1.6.5/
+-rw-rw-rw-   0        0        0     1088 2021-02-01 10:36:06.000000 mqtt_thread-1.6.5/LICENCE
+-rw-rw-rw-   0        0        0     3720 2023-06-26 16:27:22.211487 mqtt_thread-1.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3320 2023-02-25 23:15:51.000000 mqtt_thread-1.6.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 16:27:22.200171 mqtt_thread-1.6.5/mqtt_thread/
+-rw-rw-rw-   0        0        0     8039 2023-06-26 16:26:23.000000 mqtt_thread-1.6.5/mqtt_thread/MQTT_Thread.py
+-rw-rw-rw-   0        0        0     5772 2023-02-22 15:29:07.000000 mqtt_thread-1.6.5/mqtt_thread/MQTT_Thread_bak.py
+-rw-rw-rw-   0        0        0       51 2021-02-01 20:48:52.000000 mqtt_thread-1.6.5/mqtt_thread/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 16:27:22.211487 mqtt_thread-1.6.5/mqtt_thread.egg-info/
+-rw-rw-rw-   0        0        0     3720 2023-06-26 16:27:22.000000 mqtt_thread-1.6.5/mqtt_thread.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-06-26 16:27:22.000000 mqtt_thread-1.6.5/mqtt_thread.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 16:27:22.000000 mqtt_thread-1.6.5/mqtt_thread.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-26 16:27:22.000000 mqtt_thread-1.6.5/mqtt_thread.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-26 16:27:22.000000 mqtt_thread-1.6.5/mqtt_thread.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 16:27:22.225494 mqtt_thread-1.6.5/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-06-26 16:25:33.000000 mqtt_thread-1.6.5/setup.py
```

### Comparing `mqtt_thread-1.6.4/LICENCE` & `mqtt_thread-1.6.5/LICENCE`

 * *Files identical despite different names*

### Comparing `mqtt_thread-1.6.4/PKG-INFO` & `mqtt_thread-1.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt_thread
-Version: 1.6.4
+Version: 1.6.5
 Summary: Connection MQTT with thread
 Author: Didier Orlandi
 Author-email: didier.orlandi@wanadoo.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `mqtt_thread-1.6.4/README.md` & `mqtt_thread-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `mqtt_thread-1.6.4/mqtt_thread/MQTT_Thread.py` & `mqtt_thread-1.6.5/mqtt_thread/MQTT_Thread.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                 for j in range(0,len(key[0])):
                     champs.append(key[0][j])
                 champs.append("tps-secondes")
                 writer.writerow(champs)
     else:
         for i in range(0,len(key)):
             if (not os.path.exists(nomFichier + "_" + str(i)+ ".csv") or erase):
-                with open(nomFichier + str(i)+ "csv", 'w', newline='') as file:
+                with open(nomFichier + "_" + str(i)+ ".csv", 'w', newline='') as file:
                     writer = csv.writer(file, delimiter=';',quotechar='"', quoting=csv.QUOTE_NONNUMERIC)
                     #date = [datetime.datetime.now()]
                     champs = ["date"]
                     for j in range(0,len(key[i])):
                         champs.append(key[i][j])
                     champs.append("tps-secondes")
                     writer.writerow(champs)
```

### Comparing `mqtt_thread-1.6.4/mqtt_thread/MQTT_Thread_bak.py` & `mqtt_thread-1.6.5/mqtt_thread/MQTT_Thread_bak.py`

 * *Files identical despite different names*

### Comparing `mqtt_thread-1.6.4/mqtt_thread.egg-info/PKG-INFO` & `mqtt_thread-1.6.5/mqtt_thread.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt-thread
-Version: 1.6.4
+Version: 1.6.5
 Summary: Connection MQTT with thread
 Author: Didier Orlandi
 Author-email: didier.orlandi@wanadoo.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `mqtt_thread-1.6.4/setup.py` & `mqtt_thread-1.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mqtt_thread", # Replace with your own username
-    version="1.6.4",
+    version="1.6.5",
     author="Didier Orlandi",
     author_email="didier.orlandi@wanadoo.fr",
     description="Connection MQTT with thread",
     long_description=long_description,
     long_description_content_type="text/markdown",
     #url="https://github.com/",
     packages=setuptools.find_packages(),
```

