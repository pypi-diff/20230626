# Comparing `tmp/xiot-1.7.3.tar.gz` & `tmp/xiot-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xiot-1.7.3.tar", last modified: Sat Apr 29 16:50:47 2023, max compression
+gzip compressed data, was "dist/xiot-1.7.4.tar", last modified: Mon Jun 26 17:50:13 2023, max compression
```

## Comparing `xiot-1.7.3.tar` & `xiot-1.7.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-04-29 16:50:47.000000 xiot-1.7.3/
--rw-r--r--   0 Robin      (501) staff       (20)      242 2023-04-29 16:50:47.000000 xiot-1.7.3/PKG-INFO
-drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-04-29 16:50:47.000000 xiot-1.7.3/xiot.egg-info/
--rw-r--r--   0 Robin      (501) staff       (20)      242 2023-04-29 16:50:46.000000 xiot-1.7.3/xiot.egg-info/PKG-INFO
--rw-r--r--   0 Robin      (501) staff       (20)      168 2023-04-29 16:50:46.000000 xiot-1.7.3/xiot.egg-info/SOURCES.txt
--rw-r--r--   0 Robin      (501) staff       (20)       23 2023-04-29 16:50:46.000000 xiot-1.7.3/xiot.egg-info/requires.txt
--rw-r--r--   0 Robin      (501) staff       (20)       15 2023-04-29 16:50:46.000000 xiot-1.7.3/xiot.egg-info/top_level.txt
--rw-r--r--   0 Robin      (501) staff       (20)        1 2023-04-29 16:50:46.000000 xiot-1.7.3/xiot.egg-info/dependency_links.txt
--rw-r--r--   0 Robin      (501) staff       (20)     9597 2023-04-29 16:49:50.000000 xiot-1.7.3/xiot.py
--rw-r--r--   0 Robin      (501) staff       (20)      395 2020-02-10 15:11:28.000000 xiot-1.7.3/setup.py
--rw-r--r--   0 Robin      (501) staff       (20)       38 2023-04-29 16:50:47.000000 xiot-1.7.3/setup.cfg
--rw-r--r--   0 Robin      (501) staff       (20)    17265 2023-04-15 06:15:40.000000 xiot-1.7.3/xiotshell.py
+drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-06-26 17:50:13.000000 xiot-1.7.4/
+-rw-r--r--   0 Robin      (501) staff       (20)      242 2023-06-26 17:50:13.000000 xiot-1.7.4/PKG-INFO
+drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-06-26 17:50:13.000000 xiot-1.7.4/xiot.egg-info/
+-rw-r--r--   0 Robin      (501) staff       (20)      242 2023-06-26 17:50:12.000000 xiot-1.7.4/xiot.egg-info/PKG-INFO
+-rw-r--r--   0 Robin      (501) staff       (20)      168 2023-06-26 17:50:12.000000 xiot-1.7.4/xiot.egg-info/SOURCES.txt
+-rw-r--r--   0 Robin      (501) staff       (20)       23 2023-06-26 17:50:12.000000 xiot-1.7.4/xiot.egg-info/requires.txt
+-rw-r--r--   0 Robin      (501) staff       (20)       15 2023-06-26 17:50:12.000000 xiot-1.7.4/xiot.egg-info/top_level.txt
+-rw-r--r--   0 Robin      (501) staff       (20)        1 2023-06-26 17:50:12.000000 xiot-1.7.4/xiot.egg-info/dependency_links.txt
+-rw-r--r--   0 Robin      (501) staff       (20)     9597 2023-06-26 17:39:01.000000 xiot-1.7.4/xiot.py
+-rw-r--r--   0 Robin      (501) staff       (20)      395 2020-02-10 15:11:28.000000 xiot-1.7.4/setup.py
+-rw-r--r--   0 Robin      (501) staff       (20)       38 2023-06-26 17:50:13.000000 xiot-1.7.4/setup.cfg
+-rw-r--r--   0 Robin      (501) staff       (20)    17567 2023-06-26 17:49:35.000000 xiot-1.7.4/xiotshell.py
```

### Comparing `xiot-1.7.3/xiot.py` & `xiot-1.7.4/xiot.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 '''
 Created on 2018年11月23日
 
 @author: Robin
 '''
 from __future__ import print_function
 
-__version__ = '1.7.3'
+__version__ = '1.7.4'
 
 
 def md5(s):
     import hashlib
     m2 = hashlib.md5()
     m2.update(s.encode("utf8"))
     return m2.hexdigest()
```

### Comparing `xiot-1.7.3/xiotshell.py` & `xiot-1.7.4/xiotshell.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,14 +177,22 @@
         ]
 
     def __shell_run__(self):
         while True:
             dtu = None
             while self.running:
                 try:
+                    try:
+                        if dtu:
+                            print('stopping old dtu')
+                            dtu.stop()
+                            print('stopped old dtu ok')
+                            dtu = None
+                    except:
+                        pass
                     dtu = self.new_dtu()
                     self.dtu = dtu
                     define = self.runner.get_define()
                     attrs = define.get('attributes') or []
                     attrs += self.get_default_attributes() or []
                     if self.name:
                         define['name'] = self.name
```

