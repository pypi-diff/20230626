# Comparing `tmp/pypalert-1.3.1.tar.gz` & `tmp/pypalert-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypalert-1.3.1.tar", last modified: Fri Apr  7 03:46:51 2023, max compression
+gzip compressed data, was "pypalert-2.0.0.tar", last modified: Mon Jun 26 02:54:03 2023, max compression
```

## Comparing `pypalert-1.3.1.tar` & `pypalert-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 03:46:51.866446 pypalert-1.3.1/
--rw-rw-rw-   0        0        0      420 2023-03-31 07:27:40.000000 pypalert-1.3.1/LICENSE.rst
--rw-rw-rw-   0        0        0      235 2023-04-07 03:46:51.866446 pypalert-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      115 2023-04-07 03:46:51.867361 pypalert-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      343 2023-04-07 03:46:32.000000 pypalert-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 03:46:51.838753 pypalert-1.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-07 03:46:51.853458 pypalert-1.3.1/src/pypalert/
--rw-rw-rw-   0        0        0        0 2023-03-24 06:06:44.000000 pypalert-1.3.1/src/pypalert/__init__.py
--rw-rw-rw-   0        0        0    11846 2023-04-07 01:30:08.000000 pypalert-1.3.1/src/pypalert/pypalert.py
-drwxrwxrwx   0        0        0        0 2023-04-07 03:46:51.865428 pypalert-1.3.1/src/pypalert.egg-info/
--rw-rw-rw-   0        0        0      235 2023-04-07 03:46:51.000000 pypalert-1.3.1/src/pypalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-04-07 03:46:51.000000 pypalert-1.3.1/src/pypalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 03:46:51.000000 pypalert-1.3.1/src/pypalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-07 03:46:51.000000 pypalert-1.3.1/src/pypalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 02:54:03.691239 pypalert-2.0.0/
+-rw-rw-rw-   0        0        0      420 2023-03-31 07:27:40.000000 pypalert-2.0.0/LICENSE.rst
+-rw-rw-rw-   0        0        0      244 2023-06-26 02:54:03.691239 pypalert-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      115 2023-06-26 02:54:03.693240 pypalert-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      352 2023-06-26 02:53:07.000000 pypalert-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 02:54:03.676237 pypalert-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 02:54:03.679240 pypalert-2.0.0/src/pypalert/
+-rw-rw-rw-   0        0        0        0 2023-03-24 06:06:44.000000 pypalert-2.0.0/src/pypalert/__init__.py
+-rw-rw-rw-   0        0        0    10815 2023-06-26 02:53:15.000000 pypalert-2.0.0/src/pypalert/mode1.py
+-rw-rw-rw-   0        0        0    11827 2023-06-26 02:21:04.000000 pypalert-2.0.0/src/pypalert/pypalert.py
+drwxrwxrwx   0        0        0        0 2023-06-26 02:54:03.691239 pypalert-2.0.0/src/pypalert.egg-info/
+-rw-rw-rw-   0        0        0      244 2023-06-26 02:54:03.000000 pypalert-2.0.0/src/pypalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-06-26 02:54:03.000000 pypalert-2.0.0/src/pypalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 02:54:03.000000 pypalert-2.0.0/src/pypalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 02:54:03.000000 pypalert-2.0.0/src/pypalert.egg-info/top_level.txt
```

### Comparing `pypalert-1.3.1/src/pypalert/pypalert.py` & `pypalert-2.0.0/src/pypalert/pypalert.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,39 +47,38 @@
 
         client.send(link)
 
         while True:
             link1 = client.recv(24080)
             
             string = link1.hex()
-            #print(string)
+            print(string)
 
             #第一個    
             if('53594e43' in string):
                 tmp=''
                 #print(string)
                 tmp = tmp + string
                 #print("-----T="+str(len(tmp)))  
                 #XYZstorage(string[70:])
-                CRC16 = tmp[-4:]
+                CRC16 = tmp[-4:]    
                 #print(len(tmp))
                 
                 tmp_header = int(tmp[12:14], 16)
                 tmp_header = (tmp_header + 11) * 2
                 #header
                 header =tmp[:tmp_header]
                 UTime = header[30:32] + header[28:30] + header[26:28] + header[24:26] + header[22:24]  
                 UTime = int(UTime, base=16)
                 #print(UTime)
                 SPS = header[48:50] + header [46:48]
                 SPS = int(SPS, base=16)
                 
                 scale = header [44:46] + header[42:44] + header [40:42] + header[38:40] 
                 
-                
                 binary_number = bytes.fromhex(scale)
                 
                 scale = struct.unpack('!f', binary_number)[0]
                 scale = format(scale,'.2f')
                 #print("scale" + str(scale))
 
                 #print(CRC16)
@@ -358,13 +357,13 @@
     print(len(x))
     print(len(n))
     """
     
     while True:
         #bbbb = aaaa.get_Now_Channel1()
         #data = XXXX.get_Now_Channel1()
-        print(len(aaaa.get_Now_Channel4()))
-        print(len(XXXX.get_Now_Channel4()))
+        print(aaaa.get_Now_UnixTime())
+        #print(len(XXXX.get_Now_Channel4()))
         #print("Current data:", len(my_obj.get_Now_UnixTime()))
         time.sleep(1)
```

