# Comparing `tmp/pypalert-2.0.0.tar.gz` & `tmp/pypalert-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypalert-2.0.0.tar", last modified: Mon Jun 26 02:54:03 2023, max compression
+gzip compressed data, was "pypalert-2.0.1.tar", last modified: Mon Jun 26 03:09:04 2023, max compression
```

## Comparing `pypalert-2.0.0.tar` & `pypalert-2.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 02:54:03.691239 pypalert-2.0.0/
--rw-rw-rw-   0        0        0      420 2023-03-31 07:27:40.000000 pypalert-2.0.0/LICENSE.rst
--rw-rw-rw-   0        0        0      244 2023-06-26 02:54:03.691239 pypalert-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      115 2023-06-26 02:54:03.693240 pypalert-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      352 2023-06-26 02:53:07.000000 pypalert-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 02:54:03.676237 pypalert-2.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-26 02:54:03.679240 pypalert-2.0.0/src/pypalert/
--rw-rw-rw-   0        0        0        0 2023-03-24 06:06:44.000000 pypalert-2.0.0/src/pypalert/__init__.py
--rw-rw-rw-   0        0        0    10815 2023-06-26 02:53:15.000000 pypalert-2.0.0/src/pypalert/mode1.py
--rw-rw-rw-   0        0        0    11827 2023-06-26 02:21:04.000000 pypalert-2.0.0/src/pypalert/pypalert.py
-drwxrwxrwx   0        0        0        0 2023-06-26 02:54:03.691239 pypalert-2.0.0/src/pypalert.egg-info/
--rw-rw-rw-   0        0        0      244 2023-06-26 02:54:03.000000 pypalert-2.0.0/src/pypalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-06-26 02:54:03.000000 pypalert-2.0.0/src/pypalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 02:54:03.000000 pypalert-2.0.0/src/pypalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-26 02:54:03.000000 pypalert-2.0.0/src/pypalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 03:09:04.903064 pypalert-2.0.1/
+-rw-rw-rw-   0        0        0      420 2023-03-31 07:27:40.000000 pypalert-2.0.1/LICENSE.rst
+-rw-rw-rw-   0        0        0      244 2023-06-26 03:09:04.903064 pypalert-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      115 2023-06-26 03:09:04.905056 pypalert-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      352 2023-06-26 03:08:47.000000 pypalert-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 03:09:04.885045 pypalert-2.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 03:09:04.887761 pypalert-2.0.1/src/pypalert/
+-rw-rw-rw-   0        0        0        0 2023-03-24 06:06:44.000000 pypalert-2.0.1/src/pypalert/__init__.py
+-rw-rw-rw-   0        0        0    10786 2023-06-26 03:07:33.000000 pypalert-2.0.1/src/pypalert/mode1.py
+-rw-rw-rw-   0        0        0    11827 2023-06-26 02:21:04.000000 pypalert-2.0.1/src/pypalert/pypalert.py
+drwxrwxrwx   0        0        0        0 2023-06-26 03:09:04.903064 pypalert-2.0.1/src/pypalert.egg-info/
+-rw-rw-rw-   0        0        0      244 2023-06-26 03:09:04.000000 pypalert-2.0.1/src/pypalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-06-26 03:09:04.000000 pypalert-2.0.1/src/pypalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 03:09:04.000000 pypalert-2.0.1/src/pypalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 03:09:04.000000 pypalert-2.0.1/src/pypalert.egg-info/top_level.txt
```

### Comparing `pypalert-2.0.0/src/pypalert/mode1.py` & `pypalert-2.0.1/src/pypalert/mode1.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 
         while True:
             link1 = client.recv(2500)
             
             data = link1.hex()
             #print(data)
             if(data == "010200000006010600c00001"):
-                print("pp")
                 continue
             #print(len(data))
             header = data[:400]
             self.header = header
             #print(header)
             packet_type = data[2:4] + data[0:2]
             #print(packet_type)
```

### Comparing `pypalert-2.0.0/src/pypalert/pypalert.py` & `pypalert-2.0.1/src/pypalert/pypalert.py`

 * *Files identical despite different names*

