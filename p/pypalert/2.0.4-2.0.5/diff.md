# Comparing `tmp/pypalert-2.0.4.tar.gz` & `tmp/pypalert-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypalert-2.0.4.tar", last modified: Mon Jun 26 05:54:01 2023, max compression
+gzip compressed data, was "pypalert-2.0.5.tar", last modified: Mon Jun 26 08:47:34 2023, max compression
```

## Comparing `pypalert-2.0.4.tar` & `pypalert-2.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 05:54:01.653804 pypalert-2.0.4/
--rw-rw-rw-   0        0        0      420 2023-03-31 07:27:40.000000 pypalert-2.0.4/LICENSE.rst
--rw-rw-rw-   0        0        0      244 2023-06-26 05:54:01.653804 pypalert-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      115 2023-06-26 05:54:01.654804 pypalert-2.0.4/setup.cfg
--rw-rw-rw-   0        0        0      352 2023-06-26 05:53:52.000000 pypalert-2.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 05:54:01.621461 pypalert-2.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-26 05:54:01.639461 pypalert-2.0.4/src/pypalert/
--rw-rw-rw-   0        0        0        0 2023-03-24 06:06:44.000000 pypalert-2.0.4/src/pypalert/__init__.py
--rw-rw-rw-   0        0        0    13262 2023-06-26 05:53:40.000000 pypalert-2.0.4/src/pypalert/mode1.py
--rw-rw-rw-   0        0        0    11827 2023-06-26 02:21:04.000000 pypalert-2.0.4/src/pypalert/pypalert.py
-drwxrwxrwx   0        0        0        0 2023-06-26 05:54:01.653804 pypalert-2.0.4/src/pypalert.egg-info/
--rw-rw-rw-   0        0        0      244 2023-06-26 05:54:01.000000 pypalert-2.0.4/src/pypalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-06-26 05:54:01.000000 pypalert-2.0.4/src/pypalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 05:54:01.000000 pypalert-2.0.4/src/pypalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-26 05:54:01.000000 pypalert-2.0.4/src/pypalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 08:47:34.232540 pypalert-2.0.5/
+-rw-rw-rw-   0        0        0      420 2023-03-31 07:27:40.000000 pypalert-2.0.5/LICENSE.rst
+-rw-rw-rw-   0        0        0      244 2023-06-26 08:47:34.233542 pypalert-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      115 2023-06-26 08:47:34.234543 pypalert-2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      352 2023-06-26 08:47:21.000000 pypalert-2.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:47:34.203253 pypalert-2.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 08:47:34.217696 pypalert-2.0.5/src/pypalert/
+-rw-rw-rw-   0        0        0        0 2023-03-24 06:06:44.000000 pypalert-2.0.5/src/pypalert/__init__.py
+-rw-rw-rw-   0        0        0    14310 2023-06-26 08:47:12.000000 pypalert-2.0.5/src/pypalert/mode1.py
+-rw-rw-rw-   0        0        0    11827 2023-06-26 02:21:04.000000 pypalert-2.0.5/src/pypalert/pypalert.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:47:34.232540 pypalert-2.0.5/src/pypalert.egg-info/
+-rw-rw-rw-   0        0        0      244 2023-06-26 08:47:34.000000 pypalert-2.0.5/src/pypalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-06-26 08:47:34.000000 pypalert-2.0.5/src/pypalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 08:47:34.000000 pypalert-2.0.5/src/pypalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 08:47:34.000000 pypalert-2.0.5/src/pypalert.egg-info/top_level.txt
```

### Comparing `pypalert-2.0.4/src/pypalert/mode1.py` & `pypalert-2.0.5/src/pypalert/mode1.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,27 +79,61 @@
             Ehour =  int(data[46:48] + data[44:46] ,16) 
             Eminute = int(data[50:52] + data[48:50],16)
             Esecond = int(data[54:56],16)
             Emsecond = int(data[52:54],16)
             Etime = str(Eyear) + "-" + str(Emonth) + "-" + str(Eday) + "-" + str(Ehour) + "-" + str(Eminute) + "-" + str(Esecond) + "-" + str(Emsecond)
             #print(Etime)
             self.Etime = Etime
+
+            PGV_1s = int(data[58:60] + data[56:58] ,16)
+
+            PGA_10s = int(data[66:68] + data[64:66] ,16)
+
+            Pd_warning_threshold = int(data[82:84] + data[80:82] ,16)
+
+            PGA_warning_threshold = int(data[86:88] + data[84:86] ,16)
+
+            Pd_flag = int(data[94:96] + data[92:94] ,16) 
+
+            Pd_watch_threshold = int(data[98:100] + data[96:98] ,16)
+
+            PGA_warning_threshold = int(data[102:104] + data[100:102] ,16)
+
+            Intensity_now = int(data[106:108] + data[104:106] ,16)
+
+            Intensity_maximum = int(data[110:112] + data[108:110] ,16)
+
+            PGA_1s = int(data[114:116] + data[112:114] ,16)
+
+            tau_c = int(data[122:124] + data[120:122] ,16)
+
+            Trig_mode = int(data[126:128] + data[124:126] ,16)
+
+            Durations_WatchAndWarning = int(data[134:136] + data[132:134] ,16)
+
+            Firmware_version = int(data[138:140] + data[136:138] ,16)
+
+
+    
+
+
+            
             
             self.SPS = int(data[396:398] ,16)
 
             XYZdata = data[400:]
             xconnect, yconnect, zconnect, Pdconnect, Disconnect = data_cut(XYZdata)
             #print(len(xconnect)) --- 100
             self.X.extend(xconnect)
             self.Y.extend(yconnect)
             self.Z.extend(zconnect)
             self.Pd.extend(Pdconnect)
             self.Dis.extend(Disconnect)
             #print(len(self.X))
-            if(len(self.X)>1000):
+            if(len(self.X)>6000):
                 del self.X[:100]
                 del self.Y[:100]
                 del self.Z[:100]
                 del self.Pd[:100]
                 del self.Dis[:100]
                 del self.Stime[:1]
     
@@ -337,53 +371,56 @@
         #print(XYZhex)
 
         #儲存進XYZ的陣列
         if(flag == 0):
             hex_string = XYZhex  # 十六进制字符串
             unsigned_integer = int(hex_string, 16)  # 将十六进制字符串转换为无符号整数
             XYZdecimal = unsigned_integer if unsigned_integer < 32768 else unsigned_integer - 65536  # 转换为有符号整数
-            XYZdecimal = round(XYZdecimal/16.718,4)
+            XYZdecimal = XYZdecimal/16.718
             #print(XYZdecimal)
             xdata_cut.append(XYZdecimal)
             flag = flag +1
         elif(flag == 1):
             hex_string = XYZhex  # 十六进制字符串
             unsigned_integer = int(hex_string, 16)  # 将十六进制字符串转换为无符号整数
             XYZdecimal = unsigned_integer if unsigned_integer < 32768 else unsigned_integer - 65536
-            XYZdecimal = round(XYZdecimal/16.718,4)
+            XYZdecimal = XYZdecimal/16.718
             #print(XYZdecimal)
             ydata_cut.append(XYZdecimal)
             flag = flag +1
         elif(flag == 2):
             hex_string = XYZhex  # 十六进制字符串
             unsigned_integer = int(hex_string, 16)  # 将十六进制字符串转换为无符号整数
             XYZdecimal = unsigned_integer if unsigned_integer < 32768 else unsigned_integer - 65536
-            XYZdecimal = round(XYZdecimal/16.718,4)
+            XYZdecimal = XYZdecimal/16.718
             #print(XYZdecimal)
             zdata_cut.append(XYZdecimal)
             flag = flag +1
         elif(flag == 3):
             hex_string = int(XYZhex,16) 
+            #print(XYZhex)
             XYZdecimal = unsigned_integer if unsigned_integer < 32768 else unsigned_integer - 65536
+            XYZdecimal = XYZdecimal/1000
             PD_cut.append(XYZdecimal)
             flag = flag +1
         elif(flag == 4):
             hex_string = int(XYZhex,16) 
             XYZdecimal = unsigned_integer if unsigned_integer < 32768 else unsigned_integer - 65536
+            XYZdecimal = XYZdecimal/1000
             Dis_cut.append(XYZdecimal)
             flag = 0
 
     return xdata_cut, ydata_cut, zdata_cut, PD_cut, Dis_cut
 
 if __name__ == '__main__':
 
     XXXX = ModbusData('10.0.0.227',502)
     
     while True:
-        #bbbb = aaaa.get_Now_Channel1()
-        data = XXXX.get_Displacement()
-        print(data)
-        data = XXXX.get_Pd()
-        print(data)
+        Stime = XXXX.get_Now_Pd()
+        #print(Stime)
+        Stime = XXXX.get_Now_Channel1()
+        #print(Stime)
+
+    
         time.sleep(1)
-
```

### Comparing `pypalert-2.0.4/src/pypalert/pypalert.py` & `pypalert-2.0.5/src/pypalert/pypalert.py`

 * *Files identical despite different names*

