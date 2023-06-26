# Comparing `tmp/cantools-9.1.0.tar.gz` & `tmp/cantools-9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cantools-9.1.0.tar", last modified: Fri Sep  1 19:30:42 2017, max compression
+gzip compressed data, was "dist/cantools-9.1.1.tar", last modified: Sat Sep  2 06:05:10 2017, max compression
```

## Comparing `cantools-9.1.0.tar` & `cantools-9.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2017-09-01 19:30:42.000000 cantools-9.1.0/
--rw-rw-r--   0 erik      (1000) erik      (1000)     3745 2017-08-30 18:11:53.000000 cantools-9.1.0/README.rst
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2017-09-01 19:30:41.000000 cantools-9.1.0/cantools/
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2017-09-01 19:30:41.000000 cantools-9.1.0/cantools/db/
--rw-rw-r--   0 erik      (1000) erik      (1000)      612 2017-07-28 10:59:57.000000 cantools-9.1.0/cantools/db/bus.py
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2017-09-01 19:30:41.000000 cantools-9.1.0/cantools/db/formats/
--rw-rw-r--   0 erik      (1000) erik      (1000)    20831 2017-08-16 16:46:06.000000 cantools-9.1.0/cantools/db/formats/dbc.py
--rw-rw-r--   0 erik      (1000) erik      (1000)     4683 2017-07-28 10:59:57.000000 cantools-9.1.0/cantools/db/formats/kcd.py
--rw-rw-r--   0 erik      (1000) erik      (1000)        0 2017-07-25 13:10:24.000000 cantools-9.1.0/cantools/db/formats/__init__.py
--rw-rw-r--   0 erik      (1000) erik      (1000)      283 2017-07-27 10:39:48.000000 cantools-9.1.0/cantools/db/formats/utils.py
--rw-rw-r--   0 erik      (1000) erik      (1000)      644 2017-07-28 10:59:57.000000 cantools-9.1.0/cantools/db/node.py
--rw-rw-r--   0 erik      (1000) erik      (1000)     4106 2017-07-28 10:59:57.000000 cantools-9.1.0/cantools/db/signal.py
--rw-rw-r--   0 erik      (1000) erik      (1000)     1628 2017-07-28 10:59:57.000000 cantools-9.1.0/cantools/db/__init__.py
--rw-rw-r--   0 erik      (1000) erik      (1000)    10555 2017-09-01 19:04:27.000000 cantools-9.1.0/cantools/db/message.py
--rw-rw-r--   0 erik      (1000) erik      (1000)     6553 2017-09-01 19:04:06.000000 cantools-9.1.0/cantools/db/file.py
--rw-rw-r--   0 erik      (1000) erik      (1000)      479 2017-07-28 10:59:57.000000 cantools-9.1.0/cantools/db/database.py
--rw-rw-r--   0 erik      (1000) erik      (1000)     3458 2017-09-01 19:20:04.000000 cantools-9.1.0/cantools/__init__.py
--rw-rw-r--   0 erik      (1000) erik      (1000)     1080 2016-08-27 21:17:08.000000 cantools-9.1.0/LICENSE
--rw-rw-r--   0 erik      (1000) erik      (1000)       38 2017-09-01 19:30:42.000000 cantools-9.1.0/setup.cfg
--rw-rw-r--   0 erik      (1000) erik      (1000)     5119 2017-09-01 19:30:42.000000 cantools-9.1.0/PKG-INFO
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2017-09-01 19:30:41.000000 cantools-9.1.0/cantools.egg-info/
--rw-rw-r--   0 erik      (1000) erik      (1000)        9 2017-09-01 19:30:41.000000 cantools-9.1.0/cantools.egg-info/top_level.txt
--rw-rw-r--   0 erik      (1000) erik      (1000)     5119 2017-09-01 19:30:41.000000 cantools-9.1.0/cantools.egg-info/PKG-INFO
--rw-rw-r--   0 erik      (1000) erik      (1000)       54 2017-09-01 19:30:41.000000 cantools-9.1.0/cantools.egg-info/entry_points.txt
--rw-rw-r--   0 erik      (1000) erik      (1000)      727 2017-09-01 19:30:41.000000 cantools-9.1.0/cantools.egg-info/SOURCES.txt
--rw-rw-r--   0 erik      (1000) erik      (1000)        1 2017-09-01 19:30:41.000000 cantools-9.1.0/cantools.egg-info/dependency_links.txt
--rw-rw-r--   0 erik      (1000) erik      (1000)       34 2017-09-01 19:30:41.000000 cantools-9.1.0/cantools.egg-info/requires.txt
--rwxrwxr-x   0 erik      (1000) erik      (1000)      882 2017-07-28 10:59:57.000000 cantools-9.1.0/setup.py
--rw-rw-r--   0 erik      (1000) erik      (1000)       68 2017-06-06 10:05:18.000000 cantools-9.1.0/MANIFEST.in
--rw-rw-r--   0 erik      (1000) erik      (1000)      180 2017-08-19 19:40:06.000000 cantools-9.1.0/Makefile
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2017-09-01 19:30:41.000000 cantools-9.1.0/tests/
--rw-rw-r--   0 erik      (1000) erik      (1000)        0 2016-08-27 21:17:08.000000 cantools-9.1.0/tests/__init__.py
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2017-09-01 19:30:42.000000 cantools-9.1.0/tests/files/
--rw-rw-r--   0 erik      (1000) erik      (1000)    70458 2017-06-06 10:05:18.000000 cantools-9.1.0/tests/files/vehicle.dbc
--rw-rw-r--   0 erik      (1000) erik      (1000)     1970 2017-06-28 20:16:11.000000 cantools-9.1.0/tests/files/emc32.dbc
--rw-rw-r--   0 erik      (1000) erik      (1000)      925 2017-08-16 16:46:06.000000 cantools-9.1.0/tests/files/foobar.dbc
--rwxrwxr-x   0 erik      (1000) erik      (1000)      634 2017-08-19 19:35:49.000000 cantools-9.1.0/tests/files/padding_bit_order.dbc
--rw-rw-r--   0 erik      (1000) erik      (1000)      734 2017-08-16 16:46:06.000000 cantools-9.1.0/tests/files/motohawk.dbc
--rw-rw-r--   0 erik      (1000) erik      (1000)     2641 2017-07-26 10:31:07.000000 cantools-9.1.0/tests/files/socialledge.dbc
--rw-rw-r--   0 erik      (1000) erik      (1000)    19776 2017-09-01 19:15:17.000000 cantools-9.1.0/tests/test_cantools.py
+drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2017-09-02 06:05:10.000000 cantools-9.1.1/
+-rw-rw-r--   0 erik      (1000) erik      (1000)       38 2017-09-02 06:05:10.000000 cantools-9.1.1/setup.cfg
+drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2017-09-02 06:05:10.000000 cantools-9.1.1/tests/
+-rw-rw-r--   0 erik      (1000) erik      (1000)    20360 2017-09-02 05:59:53.000000 cantools-9.1.1/tests/test_cantools.py
+drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2017-09-02 06:05:10.000000 cantools-9.1.1/tests/files/
+-rw-rw-r--   0 erik      (1000) erik      (1000)      734 2017-08-20 19:41:13.000000 cantools-9.1.1/tests/files/motohawk.dbc
+-rw-rw-r--   0 erik      (1000) erik      (1000)    70458 2017-06-06 05:29:08.000000 cantools-9.1.1/tests/files/vehicle.dbc
+-rw-rw-r--   0 erik      (1000) erik      (1000)     2641 2017-07-26 21:40:40.000000 cantools-9.1.1/tests/files/socialledge.dbc
+-rwxrwxr-x   0 erik      (1000) erik      (1000)      634 2017-08-20 19:41:13.000000 cantools-9.1.1/tests/files/padding_bit_order.dbc
+-rw-rw-r--   0 erik      (1000) erik      (1000)      925 2017-08-20 19:41:13.000000 cantools-9.1.1/tests/files/foobar.dbc
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1970 2017-06-17 06:57:15.000000 cantools-9.1.1/tests/files/emc32.dbc
+-rw-rw-r--   0 erik      (1000) erik      (1000)        0 2015-12-28 18:41:35.000000 cantools-9.1.1/tests/__init__.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)     3745 2017-09-02 05:40:05.000000 cantools-9.1.1/README.rst
+drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2017-09-02 06:05:10.000000 cantools-9.1.1/cantools.egg-info/
+-rw-rw-r--   0 erik      (1000) erik      (1000)       34 2017-09-02 06:05:10.000000 cantools-9.1.1/cantools.egg-info/requires.txt
+-rw-rw-r--   0 erik      (1000) erik      (1000)       54 2017-09-02 06:05:10.000000 cantools-9.1.1/cantools.egg-info/entry_points.txt
+-rw-rw-r--   0 erik      (1000) erik      (1000)        9 2017-09-02 06:05:10.000000 cantools-9.1.1/cantools.egg-info/top_level.txt
+-rw-rw-r--   0 erik      (1000) erik      (1000)      727 2017-09-02 06:05:10.000000 cantools-9.1.1/cantools.egg-info/SOURCES.txt
+-rw-rw-r--   0 erik      (1000) erik      (1000)        1 2017-09-02 06:05:10.000000 cantools-9.1.1/cantools.egg-info/dependency_links.txt
+-rw-rw-r--   0 erik      (1000) erik      (1000)     5119 2017-09-02 06:05:10.000000 cantools-9.1.1/cantools.egg-info/PKG-INFO
+-rw-rw-r--   0 erik      (1000) erik      (1000)      180 2017-08-20 19:41:13.000000 cantools-9.1.1/Makefile
+drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2017-09-02 06:05:10.000000 cantools-9.1.1/cantools/
+-rw-rw-r--   0 erik      (1000) erik      (1000)     3458 2017-09-02 05:50:42.000000 cantools-9.1.1/cantools/__init__.py
+drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2017-09-02 06:05:10.000000 cantools-9.1.1/cantools/db/
+-rw-rw-r--   0 erik      (1000) erik      (1000)     4106 2017-07-28 07:06:34.000000 cantools-9.1.1/cantools/db/signal.py
+drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2017-09-02 06:05:10.000000 cantools-9.1.1/cantools/db/formats/
+-rw-rw-r--   0 erik      (1000) erik      (1000)     4683 2017-07-28 06:56:46.000000 cantools-9.1.1/cantools/db/formats/kcd.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)      283 2017-07-27 21:29:08.000000 cantools-9.1.1/cantools/db/formats/utils.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)        0 2017-07-20 09:18:16.000000 cantools-9.1.1/cantools/db/formats/__init__.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)    20831 2017-08-20 19:41:13.000000 cantools-9.1.1/cantools/db/formats/dbc.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)      644 2017-07-28 07:05:09.000000 cantools-9.1.1/cantools/db/node.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)      612 2017-07-28 07:04:07.000000 cantools-9.1.1/cantools/db/bus.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1628 2017-07-28 06:55:21.000000 cantools-9.1.1/cantools/db/__init__.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)    10624 2017-09-02 06:00:50.000000 cantools-9.1.1/cantools/db/message.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)      479 2017-07-28 05:31:49.000000 cantools-9.1.1/cantools/db/database.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)     6553 2017-09-02 05:40:05.000000 cantools-9.1.1/cantools/db/file.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1080 2015-12-28 18:41:35.000000 cantools-9.1.1/LICENSE
+-rw-rw-r--   0 erik      (1000) erik      (1000)     5119 2017-09-02 06:05:10.000000 cantools-9.1.1/PKG-INFO
+-rwxrwxr-x   0 erik      (1000) erik      (1000)      882 2017-08-20 19:41:13.000000 cantools-9.1.1/setup.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)       68 2017-06-06 05:29:08.000000 cantools-9.1.1/MANIFEST.in
```

### Comparing `cantools-9.1.0/README.rst` & `cantools-9.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `cantools-9.1.0/cantools/db/bus.py` & `cantools-9.1.1/cantools/db/bus.py`

 * *Files identical despite different names*

### Comparing `cantools-9.1.0/cantools/db/formats/dbc.py` & `cantools-9.1.1/cantools/db/formats/dbc.py`

 * *Files identical despite different names*

### Comparing `cantools-9.1.0/cantools/db/formats/kcd.py` & `cantools-9.1.1/cantools/db/formats/kcd.py`

 * *Files identical despite different names*

### Comparing `cantools-9.1.0/cantools/db/node.py` & `cantools-9.1.1/cantools/db/node.py`

 * *Files identical despite different names*

### Comparing `cantools-9.1.0/cantools/db/signal.py` & `cantools-9.1.1/cantools/db/signal.py`

 * *Files identical despite different names*

### Comparing `cantools-9.1.0/cantools/db/__init__.py` & `cantools-9.1.1/cantools/db/__init__.py`

 * *Files identical despite different names*

### Comparing `cantools-9.1.0/cantools/db/message.py` & `cantools-9.1.1/cantools/db/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,27 @@
             if choice_string == scaled_value:
                 scaled_value = choice_number
                 break
 
     return int((scaled_value - signal.offset) / signal.scale)
 
 
+def _decode_signal(signal, value, decode_choices):
+    scaled_value = (signal.scale * value + signal.offset)
+
+    if decode_choices:
+        try:
+            decoded_signal = signal.choices[scaled_value]
+        except (KeyError, TypeError):
+            decoded_signal = scaled_value
+    else:
+        decoded_signal = scaled_value
+
+    return decoded_signal
+
 
 def _encode_data(data, signals, formats):
     big_decoded_data = []
     little_decoded_data = []
 
     for signal in signals:
         if signal.byte_order == 'little_endian':
@@ -31,61 +44,44 @@
         if signal.byte_order == 'big_endian':
             continue
 
         little_decoded_data.append(_unscale_value(signal, data))
 
     big_packed = bitstruct.pack(formats[0], *big_decoded_data)
     little_packed = bitstruct.pack(formats[1], *little_decoded_data)[::-1]
-    packed_union = (struct.unpack('>Q', big_packed)[0]
-                    | struct.unpack('>Q', little_packed)[0])
+    packed_union = struct.unpack('>Q', big_packed)[0]
+    packed_union |= struct.unpack('>Q', little_packed)[0]
 
     return struct.pack('>Q', packed_union)
 
 
 def _decode_data(data, signals, formats, decode_choices):
     decoded_signals = {}
 
     # Big endian signals.
-    big_unpacked = bitstruct.unpack(formats[0], data)
-    i = 0
+    big_unpacked = list(bitstruct.unpack(formats[0], data))
 
     for signal in signals:
         if signal.byte_order == 'little_endian':
             continue
 
-        value = big_unpacked[i]
-        scaled_value = (signal.scale * value + signal.offset)
-
-        if decode_choices:
-            try:
-                decoded_signals[signal.name] = signal.choices[scaled_value]
-            except (KeyError, TypeError):
-                decoded_signals[signal.name] = scaled_value
-        else:
-            decoded_signals[signal.name] = scaled_value
-
-        i += 1
+        decoded_signals[signal.name] = _decode_signal(signal,
+                                                      big_unpacked.pop(0),
+                                                      decode_choices)
 
     # Little endian signals.
-    little_unpacked = bitstruct.unpack(formats[1], data[::-1])[::-1]
-    i = 0
+    little_unpacked = list(bitstruct.unpack(formats[1], data[::-1])[::-1])
 
     for signal in signals:
         if signal.byte_order == 'big_endian':
             continue
 
-        value = little_unpacked[i]
-        scaled_value = (signal.scale * value + signal.offset)
-
-        try:
-            decoded_signals[signal.name] = signal.choices[scaled_value]
-        except (KeyError, TypeError):
-            decoded_signals[signal.name] = scaled_value
-
-        i += 1
+        decoded_signals[signal.name] = _decode_signal(signal,
+                                                      little_unpacked.pop(0),
+                                                      decode_choices)
 
     return decoded_signals
 
 
 def _create_message_encode_decode_formats(signals):
     # Big endian byte order format.
     big_fmt = ''
```

### Comparing `cantools-9.1.0/cantools/db/file.py` & `cantools-9.1.1/cantools/db/file.py`

 * *Files identical despite different names*

### Comparing `cantools-9.1.0/cantools/__init__.py` & `cantools-9.1.1/cantools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import argparse
 import re
 import binascii
 import struct
 from . import db
 
 __author__ = 'Erik Moqvist'
-__version__ = '9.1.0'
+__version__ = '9.1.1'
 
 
 # Matches 'candump' output, i.e. "vcan0  1F0   [8]  00 00 00 00 00 00 1B C1".
 RE_CANDUMP = re.compile(r'^.*  ([0-9A-F]+)   \[\d\]\s*([0-9A-F ]*)$')
 
 
 def _do_decode(args):
```

### Comparing `cantools-9.1.0/LICENSE` & `cantools-9.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cantools-9.1.0/PKG-INFO` & `cantools-9.1.1/cantools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cantools
-Version: 9.1.0
+Version: 9.1.1
 Summary: CAN BUS tools.
 Home-page: https://github.com/eerimoq/cantools
 Author: Erik Moqvist
 Author-email: erik.moqvist@gmail.com
 License: MIT
 Description: |buildstatus|_
         |coverage|_
```

### Comparing `cantools-9.1.0/cantools.egg-info/PKG-INFO` & `cantools-9.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cantools
-Version: 9.1.0
+Version: 9.1.1
 Summary: CAN BUS tools.
 Home-page: https://github.com/eerimoq/cantools
 Author: Erik Moqvist
 Author-email: erik.moqvist@gmail.com
 License: MIT
 Description: |buildstatus|_
         |coverage|_
```

### Comparing `cantools-9.1.0/cantools.egg-info/SOURCES.txt` & `cantools-9.1.1/cantools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cantools-9.1.0/setup.py` & `cantools-9.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `cantools-9.1.0/tests/files/vehicle.dbc` & `cantools-9.1.1/tests/files/vehicle.dbc`

 * *Files identical despite different names*

### Comparing `cantools-9.1.0/tests/files/emc32.dbc` & `cantools-9.1.1/tests/files/emc32.dbc`

 * *Files identical despite different names*

### Comparing `cantools-9.1.0/tests/files/foobar.dbc` & `cantools-9.1.1/tests/files/foobar.dbc`

 * *Files identical despite different names*

### Comparing `cantools-9.1.0/tests/files/padding_bit_order.dbc` & `cantools-9.1.1/tests/files/padding_bit_order.dbc`

 * *Files identical despite different names*

### Comparing `cantools-9.1.0/tests/files/motohawk.dbc` & `cantools-9.1.1/tests/files/motohawk.dbc`

 * *Files identical despite different names*

### Comparing `cantools-9.1.0/tests/files/socialledge.dbc` & `cantools-9.1.1/tests/files/socialledge.dbc`

 * *Files identical despite different names*

### Comparing `cantools-9.1.0/tests/test_cantools.py` & `cantools-9.1.1/tests/test_cantools.py`

 * *Files 3% similar despite different names*

```diff
@@ -213,39 +213,60 @@
 
         encoded = db.encode_message(example_message_frame_id, data)
         self.assertEqual(encoded, b'\xc0\x06\xe0\x00\x00\x00\x00\x00')
 
         decoded = db.decode_message(example_message_frame_id, encoded)
         self.assertEqual(decoded, data)
 
-    def test_motohawk_encode_decode_no_decode_choices(self):
-        """Encode and decode the signals in a ExampleMessage frame with
-        `decode_choices` set to False.
+    def test_big_endian_no_decode_choices(self):
+        """Decode a big endian signal with `decode_choices` set to False.
 
         """
 
         db = cantools.db.File()
         filename = os.path.join('tests', 'files', 'motohawk.dbc')
         db.add_dbc_file(filename)
 
-        example_message_frame_id = 496
-
         data = {
             'Temperature': 250.55,
             'AverageRadius': 3.2,
             'Enable': 1
         }
 
-        encoded = db.encode_message(example_message_frame_id, data)
-        self.assertEqual(encoded, b'\xc0\x06\xe0\x00\x00\x00\x00\x00')
-        decoded = db.decode_message(example_message_frame_id,
-                                    encoded,
+        decoded = db.decode_message(496,
+                                    b'\xc0\x06\xe0\x00\x00\x00\x00\x00',
                                     decode_choices=False)
         self.assertEqual(decoded, data)
 
+    def test_little_endian_no_decode_choices(self):
+        """Decode a little endian signal with `decode_choices` set to False.
+
+        """
+
+        db = cantools.db.File()
+        filename = os.path.join('tests', 'files', 'socialledge.dbc')
+        db.add_dbc_file(filename)
+
+        data = {
+            'DRIVER_HEARTBEAT_cmd': 1
+        }
+
+        decoded = db.decode_message(100,
+                                    b'\x01\x00\x00\x00\x00\x00\x00\x00',
+                                    decode_choices=False)
+        self.assertEqual(decoded, data)
+
+        data = {
+            'DRIVER_HEARTBEAT_cmd': 'DRIVER_HEARTBEAT_cmd_SYNC'
+        }
+
+        decoded = db.decode_message(100,
+                                    b'\x01\x00\x00\x00\x00\x00\x00\x00')
+        self.assertEqual(decoded, data)
+
     def test_socialledge(self):
         db = cantools.db.File()
         filename = os.path.join('tests', 'files', 'socialledge.dbc')
         db.add_dbc_file(filename)
 
         # Verify nodes.
         self.assertEqual(len(db.nodes), 5)
```

