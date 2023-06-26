# Comparing `tmp/pypalert-2.0.3.tar.gz` & `tmp/pypalert-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypalert-2.0.3.tar", last modified: Mon Jun 26 03:34:02 2023, max compression
+gzip compressed data, was "pypalert-2.0.4.tar", last modified: Mon Jun 26 05:54:01 2023, max compression
```

## Comparing `pypalert-2.0.3.tar` & `pypalert-2.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 03:34:02.100974 pypalert-2.0.3/
--rw-rw-rw-   0        0        0      420 2023-03-31 07:27:40.000000 pypalert-2.0.3/LICENSE.rst
--rw-rw-rw-   0        0        0      244 2023-06-26 03:34:02.100974 pypalert-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      115 2023-06-26 03:34:02.100974 pypalert-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0      352 2023-06-26 03:33:41.000000 pypalert-2.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 03:34:02.085249 pypalert-2.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-26 03:34:02.087972 pypalert-2.0.3/src/pypalert/
--rw-rw-rw-   0        0        0        0 2023-03-24 06:06:44.000000 pypalert-2.0.3/src/pypalert/__init__.py
--rw-rw-rw-   0        0        0    13264 2023-06-26 03:33:23.000000 pypalert-2.0.3/src/pypalert/mode1.py
--rw-rw-rw-   0        0        0    11827 2023-06-26 02:21:04.000000 pypalert-2.0.3/src/pypalert/pypalert.py
-drwxrwxrwx   0        0        0        0 2023-06-26 03:34:02.099974 pypalert-2.0.3/src/pypalert.egg-info/
--rw-rw-rw-   0        0        0      244 2023-06-26 03:34:02.000000 pypalert-2.0.3/src/pypalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-06-26 03:34:02.000000 pypalert-2.0.3/src/pypalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 03:34:02.000000 pypalert-2.0.3/src/pypalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-26 03:34:02.000000 pypalert-2.0.3/src/pypalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 05:54:01.653804 pypalert-2.0.4/
+-rw-rw-rw-   0        0        0      420 2023-03-31 07:27:40.000000 pypalert-2.0.4/LICENSE.rst
+-rw-rw-rw-   0        0        0      244 2023-06-26 05:54:01.653804 pypalert-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      115 2023-06-26 05:54:01.654804 pypalert-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      352 2023-06-26 05:53:52.000000 pypalert-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 05:54:01.621461 pypalert-2.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 05:54:01.639461 pypalert-2.0.4/src/pypalert/
+-rw-rw-rw-   0        0        0        0 2023-03-24 06:06:44.000000 pypalert-2.0.4/src/pypalert/__init__.py
+-rw-rw-rw-   0        0        0    13262 2023-06-26 05:53:40.000000 pypalert-2.0.4/src/pypalert/mode1.py
+-rw-rw-rw-   0        0        0    11827 2023-06-26 02:21:04.000000 pypalert-2.0.4/src/pypalert/pypalert.py
+drwxrwxrwx   0        0        0        0 2023-06-26 05:54:01.653804 pypalert-2.0.4/src/pypalert.egg-info/
+-rw-rw-rw-   0        0        0      244 2023-06-26 05:54:01.000000 pypalert-2.0.4/src/pypalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-06-26 05:54:01.000000 pypalert-2.0.4/src/pypalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 05:54:01.000000 pypalert-2.0.4/src/pypalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 05:54:01.000000 pypalert-2.0.4/src/pypalert.egg-info/top_level.txt
```

### Comparing `pypalert-2.0.3/src/pypalert/mode1.py` & `pypalert-2.0.4/src/pypalert/mode1.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,39 +151,39 @@
         if(self.wait == False):
             time.sleep(2)
             self.wait = True
         try:
             return self.Z[-100:]          
         except :
             print("Connect Fail, so Nothing in list")
-    def get_Pd(self):
+    def get_Now_Pd(self):
         if(self.wait == False):
             time.sleep(2)
             self.wait = True
         try:
             return self.Pd[-100:]          
         except :
             print("Connect Fail, so Nothing in list")
-    def get_Displacement(self):
+    def get_Now_Displacement(self):
         if(self.wait == False):
             time.sleep(2)
             self.wait = True
         try:
             return self.Dis[-100:]          
         except :
             print("Connect Fail, so Nothing in list")
-    def get_Now_SystmeTime(self):
+    def get_Now_SystemTime(self):
         if(self.wait == False):
             time.sleep(2)
             self.wait = True
         try:
             return self.Stime[-1]
         except :
             print("Connect Fail, so Nothing in list")
-    def get_Now_EventTime(self):
+    def get_EventTime(self):
         if(self.wait == False):
             time.sleep(2)
             self.wait = True
         try:
             return self.Etime
         except :
             print("Connect Fail, so Nothing in list")
@@ -237,15 +237,15 @@
             return Yreturn, UTreturn
             
         except :
             if(self.connect_success == True):
                 print("Port Wrong, so Nothing in list")
             else:
                 print("Connect Fail, so Nothing in list")
-        
+  
     def get_NsecondChannel3Data(self,N):
         #print("len(Data)" + str(len(Data)))
         if(N == 0):
             print("Don't input 0, return now Data")
             N = 1
         elif(len(self.Stime)<N):
             print("Only have "+ str(len(self.Stime)) + " Second Data")
```

### Comparing `pypalert-2.0.3/src/pypalert/pypalert.py` & `pypalert-2.0.4/src/pypalert/pypalert.py`

 * *Files identical despite different names*

