# Comparing `tmp/nucleus_driver-1.5.2.tar.gz` & `tmp/nucleus_driver-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nucleus_driver-1.5.2.tar", last modified: Mon Jun 19 11:29:18 2023, max compression
+gzip compressed data, was "nucleus_driver-1.5.3.tar", last modified: Mon Jun 26 12:45:09 2023, max compression
```

## Comparing `nucleus_driver-1.5.2.tar` & `nucleus_driver-1.5.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 11:29:18.297179 nucleus_driver-1.5.2/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1063 2023-03-27 14:20:11.000000 nucleus_driver-1.5.2/LICENSE.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-06-19 11:29:18.297179 nucleus_driver-1.5.2/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     8987 2023-03-27 14:20:11.000000 nucleus_driver-1.5.2/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)      105 2023-03-27 14:20:11.000000 nucleus_driver-1.5.2/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)      737 2023-06-19 11:29:18.297179 nucleus_driver-1.5.2/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 11:29:18.297179 nucleus_driver-1.5.2/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 11:29:18.297179 nucleus_driver-1.5.2/src/nucleus_driver/
--rw-rw-r--   0 martin    (1000) martin    (1000)       71 2023-03-27 14:20:11.000000 nucleus_driver-1.5.2/src/nucleus_driver/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2203 2023-03-27 14:20:11.000000 nucleus_driver-1.5.2/src/nucleus_driver/_assert.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    50233 2023-06-19 08:02:36.000000 nucleus_driver-1.5.2/src/nucleus_driver/_commands.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    17554 2023-06-19 11:22:50.000000 nucleus_driver-1.5.2/src/nucleus_driver/_connection.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    25406 2023-06-19 11:22:47.000000 nucleus_driver-1.5.2/src/nucleus_driver/_download.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    16602 2023-06-15 06:32:32.000000 nucleus_driver-1.5.2/src/nucleus_driver/_flash.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10853 2023-06-08 13:16:41.000000 nucleus_driver-1.5.2/src/nucleus_driver/_logger.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      470 2023-03-27 14:20:11.000000 nucleus_driver-1.5.2/src/nucleus_driver/_messages.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    39751 2023-06-08 13:16:41.000000 nucleus_driver-1.5.2/src/nucleus_driver/_parser.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2523 2023-03-27 14:20:11.000000 nucleus_driver-1.5.2/src/nucleus_driver/_syslog.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    19319 2023-06-15 09:06:07.000000 nucleus_driver-1.5.2/src/nucleus_driver/app.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    11259 2023-06-08 13:16:41.000000 nucleus_driver-1.5.2/src/nucleus_driver/nucleus_driver.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 11:29:18.297179 nucleus_driver-1.5.2/src/nucleus_driver.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-06-19 11:29:18.000000 nucleus_driver-1.5.2/src/nucleus_driver.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      673 2023-06-19 11:29:18.000000 nucleus_driver-1.5.2/src/nucleus_driver.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-06-19 11:29:18.000000 nucleus_driver-1.5.2/src/nucleus_driver.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       77 2023-06-19 11:29:18.000000 nucleus_driver-1.5.2/src/nucleus_driver.egg-info/entry_points.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       26 2023-06-19 11:29:18.000000 nucleus_driver-1.5.2/src/nucleus_driver.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       15 2023-06-19 11:29:18.000000 nucleus_driver-1.5.2/src/nucleus_driver.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-26 12:45:09.485389 nucleus_driver-1.5.3/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1063 2023-03-27 14:20:11.000000 nucleus_driver-1.5.3/LICENSE.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-06-26 12:45:09.485389 nucleus_driver-1.5.3/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8987 2023-03-27 14:20:11.000000 nucleus_driver-1.5.3/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)      105 2023-03-27 14:20:11.000000 nucleus_driver-1.5.3/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)      737 2023-06-26 12:45:09.485389 nucleus_driver-1.5.3/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-26 12:45:09.481389 nucleus_driver-1.5.3/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-26 12:45:09.481389 nucleus_driver-1.5.3/src/nucleus_driver/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       71 2023-03-27 14:20:11.000000 nucleus_driver-1.5.3/src/nucleus_driver/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2203 2023-03-27 14:20:11.000000 nucleus_driver-1.5.3/src/nucleus_driver/_assert.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    50233 2023-06-26 12:27:28.000000 nucleus_driver-1.5.3/src/nucleus_driver/_commands.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    17098 2023-06-26 12:37:00.000000 nucleus_driver-1.5.3/src/nucleus_driver/_connection.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    25406 2023-06-20 07:42:44.000000 nucleus_driver-1.5.3/src/nucleus_driver/_download.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    16602 2023-06-20 07:42:44.000000 nucleus_driver-1.5.3/src/nucleus_driver/_flash.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10853 2023-06-20 07:42:44.000000 nucleus_driver-1.5.3/src/nucleus_driver/_logger.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      470 2023-03-27 14:20:11.000000 nucleus_driver-1.5.3/src/nucleus_driver/_messages.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    39751 2023-06-22 06:43:20.000000 nucleus_driver-1.5.3/src/nucleus_driver/_parser.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2523 2023-03-27 14:20:11.000000 nucleus_driver-1.5.3/src/nucleus_driver/_syslog.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    19319 2023-06-20 07:42:44.000000 nucleus_driver-1.5.3/src/nucleus_driver/app.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    11259 2023-06-20 07:42:44.000000 nucleus_driver-1.5.3/src/nucleus_driver/nucleus_driver.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-26 12:45:09.485389 nucleus_driver-1.5.3/src/nucleus_driver.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-06-26 12:45:09.000000 nucleus_driver-1.5.3/src/nucleus_driver.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      673 2023-06-26 12:45:09.000000 nucleus_driver-1.5.3/src/nucleus_driver.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-06-26 12:45:09.000000 nucleus_driver-1.5.3/src/nucleus_driver.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       77 2023-06-26 12:45:09.000000 nucleus_driver-1.5.3/src/nucleus_driver.egg-info/entry_points.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       26 2023-06-26 12:45:09.000000 nucleus_driver-1.5.3/src/nucleus_driver.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       15 2023-06-26 12:45:09.000000 nucleus_driver-1.5.3/src/nucleus_driver.egg-info/top_level.txt
```

### Comparing `nucleus_driver-1.5.2/LICENSE.txt` & `nucleus_driver-1.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.2/PKG-INFO` & `nucleus_driver-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucleus_driver
-Version: 1.5.2
+Version: 1.5.3
 Summary: driver for the Nortek Nucleus
 Home-page: https://github.com/nortekgroup/nucleus_driver
 Author: Martin Bergene Johansen
 Author-email: martin.johansen@nortekgroup.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nucleus_driver-1.5.2/README.md` & `nucleus_driver-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.2/setup.cfg` & `nucleus_driver-1.5.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nucleus_driver
-version = 1.5.2
+version = 1.5.3
 author = Martin Bergene Johansen
 author_email = martin.johansen@nortekgroup.com
 description = driver for the Nortek Nucleus
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nortekgroup/nucleus_driver
 classifiers =
```

### Comparing `nucleus_driver-1.5.2/src/nucleus_driver/_assert.py` & `nucleus_driver-1.5.3/src/nucleus_driver/_assert.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.2/src/nucleus_driver/_commands.py` & `nucleus_driver-1.5.3/src/nucleus_driver/_commands.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.2/src/nucleus_driver/_connection.py` & `nucleus_driver-1.5.3/src/nucleus_driver/_connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         self.serial = serial.Serial()
         self.tcp = socket.socket()
 
         self.serial_configuration = self.SerialConfiguration()
         self.tcp_configuration = self.TcpConfiguration()
         self.timeout = 1
 
-        self.tcp_buffer = b''
+        self.buffer = b''
 
         self.nucleus_id = None
         self.firmware_version = None
         self.get_all = None
 
     def get_connection_type(self) -> str:
 
@@ -422,117 +422,123 @@
             sending_successful = _send_serial_command()
 
         if self.get_connection_type() == 'tcp':
             sending_successful = _send_tcp_command()
 
         return sending_successful
 
-    def read(self, size=None, terminator: bytes = None, timeout: int = 1) -> bytes:
-
-        read_data = b''
-
-        def _serial_read() -> bytes:
-            serial_data = b''
+    def _read(self) -> bytes:
+        
+        data = b''
 
+        if self.get_connection_type() == 'tcp':
             try:
-                if terminator is not None:
-                    init_time = datetime.now()
-                    while (datetime.now() - init_time).seconds < timeout:
-                        serial_data += self.serial.read_until(terminator, size)
-                        if terminator in serial_data or b'ERROR\r\n' in serial_data:
-                            break
-
-                elif size is not None:
-                    init_time = datetime.now()
-                    while (datetime.now() - init_time).seconds < timeout:
-                        serial_data += self.serial.read(size=max(0, size - len(serial_data)))
-                        if len(serial_data) >= size:
-                            break
-
-                else:
-                    if self.serial.in_waiting:
-                        serial_data += self.serial.read(self.serial.in_waiting)
-
+                data = self.tcp.recv(4096)
+            except socket.timeout:
+                data = b''
             except Exception as exception:
-                self.messages.write_exception(message='Failed to read serial data from Nucleus: {}'.format(exception))
+                self.messages.write_exception(message='Failed to read tcp data from Nucleus: {}'.format(exception))
+                return None
+            
+        if self.get_connection_type() == 'serial':
+            data = self.serial.read(size=self.serial.in_waiting)
+        
+        return data
 
-            return serial_data
+    def read(self, size=None, terminator: bytes = None, timeout: int = 1) -> bytes:
 
-        def _tcp_read() -> bytes:
+        data = b''
+        size_satisfied = False
+        terminator_satisfied = False
+
+        if timeout is None:
+
+            read_data = self._read()
+
+            if read_data is not None:
+                data = read_data
+
+            return data
+
+        init_time = datetime.now()
+        while (datetime.now() - init_time).total_seconds() <= timeout:
+            
+            read_data = self._read()
+            
+            if read_data is None:
+                break
+
+            self.buffer += read_data
+            
+            if size is not None and len(self.buffer) >= size:
+                size_satisfied = True
+
+            if terminator is not None and terminator in self.buffer:
+                terminator_satisfied = True
+
+            if b'ERROR\r\n' in self.buffer:
+                
+                if terminator_satisfied:
+                    if self.buffer.find(b'ERROR\r\n') < self.buffer.find(terminator):
+                        terminator = b'ERROR\r\n'
+                else:
+                    terminator_satisfied = True
+                    terminator = b'ERROR\r\n'
 
-            def _read() -> bool:
-                try:
-                    self.tcp_buffer += self.tcp.recv(4096)
-                    return True
-                except socket.timeout:
-                    return True
-                except Exception as exception:
-                    if self.get_connection_status():
-                        self.messages.write_exception(message='Failed to read tcp data from Nucleus: {}'.format(exception))
+            if size_satisfied and terminator_satisfied:
 
-                    return False
+                line, separator, self.buffer = self.buffer.partition(terminator)
+                data = line + separator
 
-            if terminator is not None:
+                if len(data) > size:
 
-                init_time = datetime.now()
-                while (datetime.now() - init_time).seconds < timeout:
-                    if terminator in self.tcp_buffer:
-                        break
-                    else:
-                        if not _read():
-                            break
-
-                line, separator, self.tcp_buffer = self.tcp_buffer.partition(terminator)
-                tcp_data = line + separator
-
-            elif size is not None:
-
-                init_time = datetime.now()
-                while (datetime.now() - init_time).seconds < timeout:
-                    if len(self.tcp_buffer) >= size:
-                        break
-                    else:
-                        if not _read():
-                            break
+                    data = data[:size]
+                    self.buffer = data[size:] + self.buffer
 
-                tcp_data = self.tcp_buffer[:size]
-                self.tcp_buffer = self.tcp_buffer[size:]
+                break
 
-            else:
-                _read()
-                tcp_data = self.tcp_buffer
-                self.tcp_buffer = b''
+            elif size_satisfied:
 
-            return tcp_data
+                data = self.buffer[:size]
+                self.buffer = self.buffer[size:]
 
-        if self.get_connection_type() == 'serial':
-            read_data = _serial_read()
+                break
 
-        if self.get_connection_type() == 'tcp':
-            read_data = _tcp_read()
+            elif terminator_satisfied:
+                
+                line, separator, self.buffer = self.buffer.partition(terminator)
+                data = line + separator
 
-        return read_data
+                break
 
+        else:
+            data = self.buffer
+            self.buffer = b''
+
+        return data
+    
     def readline(self, timeout: int = 1) -> bytes:
 
         return self.read(terminator=b'\r\n', timeout=timeout)
 
     def reset_buffers(self):
+        
+        self.buffer = b''
 
         if self.get_connection_type() == 'serial':
             self.serial.reset_output_buffer()
             self.serial.reset_input_buffer()
             time.sleep(0.01)  # Double reset with delay since serial buffer reset is buggy
             self.serial.reset_output_buffer()
             self.serial.reset_input_buffer()
 
         elif self.get_connection_type() == 'tcp':
-            self.tcp_buffer = b''
-            for i in range(100):
+            
+            for _ in range(5):
                 try:
                     self.tcp.recv(4096)
                 except socket.timeout as e:
                     break
                 except Exception as e:
                     self.messages.write_warning('Got an unexpected exception when resetting TCP buffers: {}'.format(e))
                     break
-
+
```

### Comparing `nucleus_driver-1.5.2/src/nucleus_driver/_download.py` & `nucleus_driver-1.5.3/src/nucleus_driver/_download.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.2/src/nucleus_driver/_flash.py` & `nucleus_driver-1.5.3/src/nucleus_driver/_flash.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.2/src/nucleus_driver/_logger.py` & `nucleus_driver-1.5.3/src/nucleus_driver/_logger.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.2/src/nucleus_driver/_parser.py` & `nucleus_driver-1.5.3/src/nucleus_driver/_parser.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.2/src/nucleus_driver/_syslog.py` & `nucleus_driver-1.5.3/src/nucleus_driver/_syslog.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.2/src/nucleus_driver/app.py` & `nucleus_driver-1.5.3/src/nucleus_driver/app.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.2/src/nucleus_driver/nucleus_driver.py` & `nucleus_driver-1.5.3/src/nucleus_driver/nucleus_driver.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.2/src/nucleus_driver.egg-info/PKG-INFO` & `nucleus_driver-1.5.3/src/nucleus_driver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucleus-driver
-Version: 1.5.2
+Version: 1.5.3
 Summary: driver for the Nortek Nucleus
 Home-page: https://github.com/nortekgroup/nucleus_driver
 Author: Martin Bergene Johansen
 Author-email: martin.johansen@nortekgroup.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nucleus_driver-1.5.2/src/nucleus_driver.egg-info/SOURCES.txt` & `nucleus_driver-1.5.3/src/nucleus_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

