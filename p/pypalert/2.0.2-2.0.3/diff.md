# Comparing `tmp/pypalert-2.0.2.tar.gz` & `tmp/pypalert-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypalert-2.0.2.tar", last modified: Mon Jun 26 03:29:38 2023, max compression
+gzip compressed data, was "pypalert-2.0.3.tar", last modified: Mon Jun 26 03:34:02 2023, max compression
```

## Comparing `pypalert-2.0.2.tar` & `pypalert-2.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 03:29:38.569153 pypalert-2.0.2/
--rw-rw-rw-   0        0        0      420 2023-03-31 07:27:40.000000 pypalert-2.0.2/LICENSE.rst
--rw-rw-rw-   0        0        0      244 2023-06-26 03:29:38.569153 pypalert-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      115 2023-06-26 03:29:38.570157 pypalert-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0      352 2023-06-26 03:29:21.000000 pypalert-2.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 03:29:38.560156 pypalert-2.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-26 03:29:38.563175 pypalert-2.0.2/src/pypalert/
--rw-rw-rw-   0        0        0        0 2023-03-24 06:06:44.000000 pypalert-2.0.2/src/pypalert/__init__.py
--rw-rw-rw-   0        0        0    11638 2023-06-26 03:29:02.000000 pypalert-2.0.2/src/pypalert/mode1.py
--rw-rw-rw-   0        0        0    11827 2023-06-26 02:21:04.000000 pypalert-2.0.2/src/pypalert/pypalert.py
-drwxrwxrwx   0        0        0        0 2023-06-26 03:29:38.569153 pypalert-2.0.2/src/pypalert.egg-info/
--rw-rw-rw-   0        0        0      244 2023-06-26 03:29:38.000000 pypalert-2.0.2/src/pypalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-06-26 03:29:38.000000 pypalert-2.0.2/src/pypalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 03:29:38.000000 pypalert-2.0.2/src/pypalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-26 03:29:38.000000 pypalert-2.0.2/src/pypalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 03:34:02.100974 pypalert-2.0.3/
+-rw-rw-rw-   0        0        0      420 2023-03-31 07:27:40.000000 pypalert-2.0.3/LICENSE.rst
+-rw-rw-rw-   0        0        0      244 2023-06-26 03:34:02.100974 pypalert-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      115 2023-06-26 03:34:02.100974 pypalert-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      352 2023-06-26 03:33:41.000000 pypalert-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 03:34:02.085249 pypalert-2.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 03:34:02.087972 pypalert-2.0.3/src/pypalert/
+-rw-rw-rw-   0        0        0        0 2023-03-24 06:06:44.000000 pypalert-2.0.3/src/pypalert/__init__.py
+-rw-rw-rw-   0        0        0    13264 2023-06-26 03:33:23.000000 pypalert-2.0.3/src/pypalert/mode1.py
+-rw-rw-rw-   0        0        0    11827 2023-06-26 02:21:04.000000 pypalert-2.0.3/src/pypalert/pypalert.py
+drwxrwxrwx   0        0        0        0 2023-06-26 03:34:02.099974 pypalert-2.0.3/src/pypalert.egg-info/
+-rw-rw-rw-   0        0        0      244 2023-06-26 03:34:02.000000 pypalert-2.0.3/src/pypalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-06-26 03:34:02.000000 pypalert-2.0.3/src/pypalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 03:34:02.000000 pypalert-2.0.3/src/pypalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 03:34:02.000000 pypalert-2.0.3/src/pypalert.egg-info/top_level.txt
```

### Comparing `pypalert-2.0.2/src/pypalert/mode1.py` & `pypalert-2.0.3/src/pypalert/pypalert.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 import time
 import sys
 import datetime
 class ModbusData:
     def __init__(self,IP,port):
         self.IP = IP
         self.port = port
-        self.header = ''
         self.X = []
         self.Y = []
         self.Z = []
-        self.Pd = []
-        self.Dis = []
-        self.Stime = []
-        self.Etime = ''
+        self.F = []
+        self.UT = []
         self.SPS = 0
+        self.scale = 0
         self.connect_success=False
         self.wait=False
+        self.S303_3Axis=True
 
         self.lock = threading.Lock()
         self.background_thread = threading.Thread(target=self.connect, args=(IP,port), daemon=True)
         self.background_thread.start()
 
     def connect(self,IP,port):
-        arr = [0x01, 0x02, 0x00, 0x00, 0x00, 0x06, 0x01, 0x06, 0x00, 0xc0, 0x00, 0x01]
+        arr = [0x01, 0x02, 0x00, 0x00, 0x00, 0x06, 0x01, 0x06, 0x00, 0xc0, 0x00, 0x10]
         link=struct.pack("%dB"%(len(arr)),*arr)
 
         try: 
             client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         except socket.error as e: 
             print ("Error creating socket: %s" % e) 
             sys.exit(1) 
@@ -45,68 +44,77 @@
             print ("FAIL") 
             sys.exit(1) 
         
 
         client.send(link)
 
         while True:
-            link1 = client.recv(2500)
+            link1 = client.recv(24080)
             
-            data = link1.hex()
-            #print(data)
-            if(data == "010200000006010600c00001"):
-                continue
-            #print(len(data))
-            header = data[:400]
-            self.header = header
-            #print(header)
-            packet_type = data[2:4] + data[0:2]
-            #print(packet_type)
-            event_flag = data[6:8] + data[4:6]
-            #print(event_flag)
-            Syear =  int(data[10:12] + data[8:10] ,16)
-            Smonth =  int(data[14:16] + data[12:14] ,16)
-            Sday =  int(data[18:20] + data[16:18] ,16)
-            Shour =  int(data[22:24] + data[20:22] ,16) 
-            Sminute = int(data[26:28] + data[24:26],16)
-            Ssecond = int(data[30:32],16)
-            Smsecond = int(data[28:30],16)
-            Stime = str(Syear) + "-" + str(Smonth) + "-" + str(Sday) + "-" + str(Shour) + "-" + str(Sminute) + "-" + str(Ssecond) + "-" + str(Smsecond)
-            #print(Stime)
-            self.Stime.append(Stime)
-            Eyear =  int(data[34:36] + data[32:34] ,16)
-            Emonth =  int(data[38:40] + data[36:38] ,16)
-            Eday =  int(data[42:44] + data[40:42] ,16)
-            Ehour =  int(data[46:48] + data[44:46] ,16) 
-            Eminute = int(data[50:52] + data[48:50],16)
-            Esecond = int(data[54:56],16)
-            Emsecond = int(data[52:54],16)
-            Etime = str(Eyear) + "-" + str(Emonth) + "-" + str(Eday) + "-" + str(Ehour) + "-" + str(Eminute) + "-" + str(Esecond) + "-" + str(Emsecond)
-            #print(Etime)
-            self.Etime = Etime
-            
-            self.SPS = int(data[396:398] ,16)
+            string = link1.hex()
+            print(string)
 
-            XYZdata = data[400:]
-            xconnect, yconnect, zconnect, Pdconnect, Disconnect = data_cut(XYZdata)
-            #print(len(xconnect)) --- 100
-            self.X.extend(xconnect)
-            self.Y.extend(yconnect)
-            self.Z.extend(zconnect)
-            self.Pd.extend(Pdconnect)
-            self.Dis.extend(Disconnect)
-            #print(len(self.X))
-            if(len(self.X)>1000):
-                del self.X[:100]
-                del self.Y[:100]
-                del self.Z[:100]
-                del self.Pd[:100]
-                del self.Dis[:100]
-                del self.Stime[:1]
-    
+            #第一個    
+            if('53594e43' in string):
+                tmp=''
+                #print(string)
+                tmp = tmp + string
+                #print("-----T="+str(len(tmp)))  
+                #XYZstorage(string[70:])
+                CRC16 = tmp[-4:]    
+                #print(len(tmp))
+                
+                tmp_header = int(tmp[12:14], 16)
+                tmp_header = (tmp_header + 11) * 2
+                #header
+                header =tmp[:tmp_header]
+                UTime = header[30:32] + header[28:30] + header[26:28] + header[24:26] + header[22:24]  
+                UTime = int(UTime, base=16)
+                #print(UTime)
+                SPS = header[48:50] + header [46:48]
+                SPS = int(SPS, base=16)
+                
+                scale = header [44:46] + header[42:44] + header [40:42] + header[38:40] 
+                
+                binary_number = bytes.fromhex(scale)
+                
+                scale = struct.unpack('!f', binary_number)[0]
+                scale = format(scale,'.2f')
+                #print("scale" + str(scale))
+
+                #print(CRC16)
+                XYZdata = tmp[tmp_header:-4]
+                #print(header[52:54])
+                if(header[52:54] == '03'):
+                    self.S303_3Axis = True
+                elif(header[52:54] == '04'):
+                    self.S303_3Axis = False
+                
+                self.UT.append(UTime)
+                self.SPS = SPS
+                self.scale = scale
+
+                if(self.S303_3Axis):
+                    xconnect, yconnect, zconnect = data_cut(XYZdata,self.S303_3Axis)
+                    self.X.extend(xconnect)
+                    self.Y.extend(yconnect)
+                    self.Z.extend(zconnect)
+                else:
+                    xconnect, yconnect, zconnect, fconnect = data_cut(XYZdata,self.S303_3Axis)
+                    self.X.extend(xconnect)
+                    self.Y.extend(yconnect)
+                    self.Z.extend(zconnect)
+                    self.F.extend(fconnect)
+
+                if(len(self.X)>60000):
+                    del self.X[:1000]
+                    del self.Y[:1000]
+                    del self.Z[:1000]
+                    del self.F[:1000]
+                    del self.UT[:1]
 
     def get_IP(self):
         if(self.wait == False):
             time.sleep(2)
             self.wait = True
         try:
             return self.IP
@@ -118,224 +126,244 @@
             time.sleep(2)
             self.wait = True
         try:
             return self.port
         except :
             print("Connect Fail, so Nothing in list")
 
-    def get_Header(self):
-        if(self.wait == False):
-            time.sleep(2)
-            self.wait = True
-        try:
-            return self.header
-        except :
-            print("Connect Fail, so Nothing in list")
-
     def get_Now_Channel1(self):
         if(self.wait == False):
             time.sleep(2)
             self.wait = True
         try:
-            return self.X[-100:]
+            return self.X[-1000:]
         except :
             print("Connect Fail, so Nothing in list")
     def get_Now_Channel2(self):
         if(self.wait == False):
             time.sleep(2)
             self.wait = True
         try:
-            return self.Y[-100:]                  
+            return self.Y[-1000:]                  
         except :
             print("Connect Fail, so Nothing in list")
     def get_Now_Channel3(self):
         if(self.wait == False):
             time.sleep(2)
             self.wait = True
         try:
-            return self.Z[-100:]          
+            return self.Z[-1000:]          
         except :
             print("Connect Fail, so Nothing in list")
-    def get_Pd(self):
+    def get_Now_Channel4(self):
         if(self.wait == False):
             time.sleep(2)
             self.wait = True
         try:
-            return self.Pd[-100:]          
+            return self.F[-1000:]                
         except :
-            print("Connect Fail, so Nothing in list")
-    def get_Displacement(self):
+            print("Connect Fail, so Nothing in list")    
+    def get_Now_UnixTime(self):
         if(self.wait == False):
             time.sleep(2)
             self.wait = True
         try:
-            return self.Dis[-100:]          
+            return self.UT[-1]
         except :
             print("Connect Fail, so Nothing in list")
-    def get_Now_SystmeTime(self):
-        if(self.wait == False):
-            time.sleep(2)
-            self.wait = True
-        try:
-            return self.Stime[-1]
-        except :
-            print("Connect Fail, so Nothing in list")
-    def get_Now_EventTime(self):
+    def get_SPS(self):
         if(self.wait == False):
             time.sleep(2)
             self.wait = True
         try:
-            return self.Etime
+            return self.SPS
         except :
             print("Connect Fail, so Nothing in list")
-    def get_SPS(self):
+    def get_Scale(self):
         if(self.wait == False):
             time.sleep(2)
             self.wait = True
         try:
-            return self.SPS
+            return self.scale
         except :
             print("Connect Fail, so Nothing in list")
+
     def get_NsecondChannel1Data(self,N):
         #print("len(Data)" + str(len(Data)))
         if(N == 0):
             print("Don't input 0, return now Data")
             N = 1
-        elif(len(self.Stime)<N):
-            print("Only have "+ str(len(self.Stime)) + " Second Data")
-            N = len(self.Stime)
+        elif(len(self.UT)<N):
+            print("Only have "+ str(len(self.UT)) + " Second Data")
+            N = len(self.UT)
         elif(N >60):
             print("We only store 60s Data")    
-        N1000 = N*100
+        N1000 = N*1000
         Xreturn = []
         UTreturn = []
         try:
             Xreturn.extend(self.X[-N1000:])
-            UTreturn.extend(self.Stime[-N:])
+            UTreturn.extend(self.UT[-N:])
             return Xreturn, UTreturn
             
         except :
             if(self.connect_success == True):
                 print("Port Wrong, so Nothing in list")
             else:
                 print("Connect Fail, so Nothing in list")
     def get_NsecondChannel2Data(self,N):
         #print("len(Data)" + str(len(Data)))
         if(N == 0):
             print("Don't input 0, return now Data")
             N = 1
-        elif(len(self.Stime)<N):
-            print("Only have "+ str(len(self.Stime)) + " Second Data")
-            N = len(self.Stime)
+        elif(len(self.UT)<N):
+            print("Only have "+ str(len(self.UT)) + " Second Data")
+            N = len(self.UT)
         elif(N >60):
             print("We only store 60s Data")    
-        N1000 = N*100
+        N1000 = N*1000
         Yreturn = []
         UTreturn = []
         try:
             Yreturn.extend(self.Y[-N1000:])
-            UTreturn.extend(self.Stime[-N:])
+            UTreturn.extend(self.UT[-N:])
             return Yreturn, UTreturn
             
         except :
             if(self.connect_success == True):
                 print("Port Wrong, so Nothing in list")
             else:
                 print("Connect Fail, so Nothing in list")
         
     def get_NsecondChannel3Data(self,N):
         #print("len(Data)" + str(len(Data)))
         if(N == 0):
             print("Don't input 0, return now Data")
             N = 1
-        elif(len(self.Stime)<N):
-            print("Only have "+ str(len(self.Stime)) + " Second Data")
-            N = len(self.Stime)
+        elif(len(self.UT)<N):
+            print("Only have "+ str(len(self.UT)) + " Second Data")
+            N = len(self.UT)
         elif(N >60):
             print("We only store 60s Data")    
-        N1000 = N*100
+        N1000 = N*1000
         Zreturn = []
         UTreturn = []
         try:
             Zreturn.extend(self.Z[-N1000:])
-            UTreturn.extend(self.Stime[-N:])
+            UTreturn.extend(self.UT[-N:])
             return Zreturn, UTreturn
             
         except :
             if(self.connect_success == True):
                 print("Port Wrong, so Nothing in list")
             else:
                 print("Connect Fail, so Nothing in list")
-
-            
-def data_cut(XYZstr):
     
+    def get_NsecondChannel4Data(self,N):
+        #print("len(Data)" + str(len(Data)))
+        if(self.S303_3Axis==True):
+            print("You don't have Channel 4")
+            return 
+        if(N == 0):
+            print("Don't input 0, return now Data")
+            N = 1
+        elif(len(self.UT)<N):
+            print("Only have "+ str(len(self.UT)) + " Second Data")
+            N = len(self.UT)
+        elif(N >60):
+            print("We only store 60s Data")    
+        N1000 = N*1000
+        Freturn = []
+        UTreturn = []
+        try:
+            Freturn.extend(self.F[-N1000:])
+            UTreturn.extend(self.UT[-N:])
+            return Freturn, UTreturn
+            
+        except :
+            if(self.connect_success == True):
+                print("Port Wrong, so Nothing in list")
+            else:
+                print("Connect Fail, so Nothing in list")
+
+
+def data_cut(XYZstr,S303_3Axis):
+    #print(S303_3Axis)
     xdata_cut = []
     ydata_cut = []
     zdata_cut = []
-    PD_cut = []
-    Dis_cut = []
+    fdata_cut = []
     flag = 0
     #Little Endian 轉回正常
     XYZhex = ''
     #print(len(XYZstr))
     
     #每4個byte為一組處理
-    for i in range(0, len(XYZstr), 4):
+    for i in range(0, len(XYZstr), 8):
         XYZdecimal=0
         a = XYZstr[i:i+2]
         b = XYZstr[i+2:i+4]
-        XYZhex = b+a
+        c = XYZstr[i+4:i+6]
+        d = XYZstr[i+6:i+8]
+        XYZhex = d+c+b+a
         #hex to decimal 
+        if(len(XYZhex)==8):
+            XYZdecimal=struct.unpack('>f',bytes.fromhex(XYZhex))[0]
+        #print(type(XYZdecimal))
         #print(XYZhex)
-
+        #print(XYZdecimal)
+        
         #儲存進XYZ的陣列
-        if(flag == 0):
-            hex_string = XYZhex  # 十六进制字符串
-            unsigned_integer = int(hex_string, 16)  # 将十六进制字符串转换为无符号整数
-            XYZdecimal = unsigned_integer if unsigned_integer < 32768 else unsigned_integer - 65536  # 转换为有符号整数
-            XYZdecimal = round(XYZdecimal/16.718,4)
-            #print(XYZdecimal)
-            xdata_cut.append(XYZdecimal)
-            flag = flag +1
-        elif(flag == 1):
-            hex_string = XYZhex  # 十六进制字符串
-            unsigned_integer = int(hex_string, 16)  # 将十六进制字符串转换为无符号整数
-            XYZdecimal = unsigned_integer if unsigned_integer < 32768 else unsigned_integer - 65536
-            XYZdecimal = round(XYZdecimal/16.718,4)
-            #print(XYZdecimal)
-            ydata_cut.append(XYZdecimal)
-            flag = flag +1
-        elif(flag == 2):
-            hex_string = XYZhex  # 十六进制字符串
-            unsigned_integer = int(hex_string, 16)  # 将十六进制字符串转换为无符号整数
-            XYZdecimal = unsigned_integer if unsigned_integer < 32768 else unsigned_integer - 65536
-            XYZdecimal = round(XYZdecimal/16.718,4)
-            #print(XYZdecimal)
-            zdata_cut.append(XYZdecimal)
-            flag = flag +1
-        elif(flag == 3):
-            hex_string = int(XYZhex,16) 
-            XYZdecimal = unsigned_integer if unsigned_integer < 32768 else unsigned_integer - 65536
-            PD_cut.append(XYZdecimal)
-            flag = flag +1
-        elif(flag == 4):
-            hex_string = int(XYZhex,16) 
-            XYZdecimal = unsigned_integer if unsigned_integer < 32768 else unsigned_integer - 65536
-            Dis_cut.append(XYZdecimal)
-            flag = 0
+        if(S303_3Axis):
+            if(flag == 0):
+                xdata_cut.append(XYZdecimal)
+                flag = flag +1
+            elif(flag == 1):
+                ydata_cut.append(XYZdecimal)
+                flag = flag +1
+            elif(flag == 2):
+                zdata_cut.append(XYZdecimal)
+                flag = 0
+        else:
+            if(flag == 0):
+                xdata_cut.append(XYZdecimal)
+                flag = flag +1
+            elif(flag == 1):
+                ydata_cut.append(XYZdecimal)
+                flag = flag +1
+            elif(flag == 2):
+                zdata_cut.append(XYZdecimal)
+                flag = flag +1
+            elif(flag == 3):
+                fdata_cut.append(XYZdecimal)
+                flag = 0
+    
+    
+    #print("XYZstr: " + str(len(XYZstr)))
+    if(S303_3Axis):
+        return xdata_cut, ydata_cut, zdata_cut
+    else:
+        return xdata_cut, ydata_cut, zdata_cut, fdata_cut
 
-    return xdata_cut, ydata_cut, zdata_cut, PD_cut, Dis_cut
 
-if __name__ == '__main__':
 
-    XXXX = ModbusData('10.0.0.227',502)
+if __name__ == '__main__':
+    XXXX = ModbusData('10.0.0.50',502)
+    aaaa = ModbusData('10.0.0.68',502)
+    """aaaa = ModbusData('10.0.0.180',502)    
+    print('XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX' + str(datetime.datetime.now()))
+
+    time.sleep(2)
+    x, n= XXXX.get_NsecondChannel3Data(10)
+    print(len(x))
+    print(len(n))
+    """
     
     while True:
         #bbbb = aaaa.get_Now_Channel1()
-        data = XXXX.get_Displacement()
-        print(data)
-        data = XXXX.get_Pd()
-        print(data)
+        #data = XXXX.get_Now_Channel1()
+        print(aaaa.get_Now_UnixTime())
+        #print(len(XXXX.get_Now_Channel4()))
+        #print("Current data:", len(my_obj.get_Now_UnixTime()))
         time.sleep(1)
-       
+
```

