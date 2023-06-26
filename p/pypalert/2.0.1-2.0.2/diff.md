# Comparing `tmp/pypalert-2.0.1.tar.gz` & `tmp/pypalert-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypalert-2.0.1.tar", last modified: Mon Jun 26 03:09:04 2023, max compression
+gzip compressed data, was "pypalert-2.0.2.tar", last modified: Mon Jun 26 03:29:38 2023, max compression
```

## Comparing `pypalert-2.0.1.tar` & `pypalert-2.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 03:09:04.903064 pypalert-2.0.1/
--rw-rw-rw-   0        0        0      420 2023-03-31 07:27:40.000000 pypalert-2.0.1/LICENSE.rst
--rw-rw-rw-   0        0        0      244 2023-06-26 03:09:04.903064 pypalert-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      115 2023-06-26 03:09:04.905056 pypalert-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      352 2023-06-26 03:08:47.000000 pypalert-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 03:09:04.885045 pypalert-2.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-26 03:09:04.887761 pypalert-2.0.1/src/pypalert/
--rw-rw-rw-   0        0        0        0 2023-03-24 06:06:44.000000 pypalert-2.0.1/src/pypalert/__init__.py
--rw-rw-rw-   0        0        0    10786 2023-06-26 03:07:33.000000 pypalert-2.0.1/src/pypalert/mode1.py
--rw-rw-rw-   0        0        0    11827 2023-06-26 02:21:04.000000 pypalert-2.0.1/src/pypalert/pypalert.py
-drwxrwxrwx   0        0        0        0 2023-06-26 03:09:04.903064 pypalert-2.0.1/src/pypalert.egg-info/
--rw-rw-rw-   0        0        0      244 2023-06-26 03:09:04.000000 pypalert-2.0.1/src/pypalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-06-26 03:09:04.000000 pypalert-2.0.1/src/pypalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 03:09:04.000000 pypalert-2.0.1/src/pypalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-26 03:09:04.000000 pypalert-2.0.1/src/pypalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 03:29:38.569153 pypalert-2.0.2/
+-rw-rw-rw-   0        0        0      420 2023-03-31 07:27:40.000000 pypalert-2.0.2/LICENSE.rst
+-rw-rw-rw-   0        0        0      244 2023-06-26 03:29:38.569153 pypalert-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      115 2023-06-26 03:29:38.570157 pypalert-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      352 2023-06-26 03:29:21.000000 pypalert-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 03:29:38.560156 pypalert-2.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 03:29:38.563175 pypalert-2.0.2/src/pypalert/
+-rw-rw-rw-   0        0        0        0 2023-03-24 06:06:44.000000 pypalert-2.0.2/src/pypalert/__init__.py
+-rw-rw-rw-   0        0        0    11638 2023-06-26 03:29:02.000000 pypalert-2.0.2/src/pypalert/mode1.py
+-rw-rw-rw-   0        0        0    11827 2023-06-26 02:21:04.000000 pypalert-2.0.2/src/pypalert/pypalert.py
+drwxrwxrwx   0        0        0        0 2023-06-26 03:29:38.569153 pypalert-2.0.2/src/pypalert.egg-info/
+-rw-rw-rw-   0        0        0      244 2023-06-26 03:29:38.000000 pypalert-2.0.2/src/pypalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-06-26 03:29:38.000000 pypalert-2.0.2/src/pypalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 03:29:38.000000 pypalert-2.0.2/src/pypalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 03:29:38.000000 pypalert-2.0.2/src/pypalert.egg-info/top_level.txt
```

### Comparing `pypalert-2.0.1/src/pypalert/mode1.py` & `pypalert-2.0.2/src/pypalert/mode1.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,14 +151,30 @@
         if(self.wait == False):
             time.sleep(2)
             self.wait = True
         try:
             return self.Z[-100:]          
         except :
             print("Connect Fail, so Nothing in list")
+    def get_Pd(self):
+        if(self.wait == False):
+            time.sleep(2)
+            self.wait = True
+        try:
+            return self.Pd[-100:]          
+        except :
+            print("Connect Fail, so Nothing in list")
+    def get_Displacement(self):
+        if(self.wait == False):
+            time.sleep(2)
+            self.wait = True
+        try:
+            return self.Dis[-100:]          
+        except :
+            print("Connect Fail, so Nothing in list")
     def get_Now_SystmeTime(self):
         if(self.wait == False):
             time.sleep(2)
             self.wait = True
         try:
             return self.Stime[-1]
         except :
@@ -294,26 +310,32 @@
             unsigned_integer = int(hex_string, 16)  # 将十六进制字符串转换为无符号整数
             XYZdecimal = unsigned_integer if unsigned_integer < 32768 else unsigned_integer - 65536
             XYZdecimal = round(XYZdecimal/16.718,4)
             #print(XYZdecimal)
             zdata_cut.append(XYZdecimal)
             flag = flag +1
         elif(flag == 3):
-            PD_cut.append(XYZhex)
+            hex_string = int(XYZhex,16) 
+            XYZdecimal = unsigned_integer if unsigned_integer < 32768 else unsigned_integer - 65536
+            PD_cut.append(XYZdecimal)
             flag = flag +1
         elif(flag == 4):
-            Dis_cut.append(XYZhex)
+            hex_string = int(XYZhex,16) 
+            XYZdecimal = unsigned_integer if unsigned_integer < 32768 else unsigned_integer - 65536
+            Dis_cut.append(XYZdecimal)
             flag = 0
 
     return xdata_cut, ydata_cut, zdata_cut, PD_cut, Dis_cut
 
 if __name__ == '__main__':
 
     XXXX = ModbusData('10.0.0.227',502)
     
     while True:
         #bbbb = aaaa.get_Now_Channel1()
-        data = XXXX.get_Header()
+        data = XXXX.get_Displacement()
+        print(data)
+        data = XXXX.get_Pd()
         print(data)
         time.sleep(1)
```

### Comparing `pypalert-2.0.1/src/pypalert/pypalert.py` & `pypalert-2.0.2/src/pypalert/pypalert.py`

 * *Files identical despite different names*

