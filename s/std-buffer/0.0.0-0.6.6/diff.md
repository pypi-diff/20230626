# Comparing `tmp/std_buffer-0.0.0-py3-none-any.whl.zip` & `tmp/std_buffer-0.6.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 14569 bytes, number of entries: 17
+Zip file size: 14574 bytes, number of entries: 17
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-17 08:47 std_buffer/__init__.py
--rw-r--r--  2.0 unx     1247 b- defN 23-Jun-26 09:51 std_buffer/buffered_metadata_pb2.py
--rw-r--r--  2.0 unx     2794 b- defN 23-Jun-26 09:51 std_buffer/image_metadata_pb2.py
+-rw-r--r--  2.0 unx     1247 b- defN 23-Jun-26 12:33 std_buffer/buffered_metadata_pb2.py
+-rw-r--r--  2.0 unx     2794 b- defN 23-Jun-26 12:33 std_buffer/image_metadata_pb2.py
 -rw-r--r--  2.0 unx     3649 b- defN 23-Feb-06 08:47 std_buffer/stream_binary.py
--rw-r--r--  2.0 unx     2188 b- defN 23-Jun-26 09:51 std_buffer/writer_command_pb2.py
+-rw-r--r--  2.0 unx     2188 b- defN 23-Jun-26 12:33 std_buffer/writer_command_pb2.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-17 08:47 std_buffer/gigafrost/__init__.py
 -rw-r--r--  2.0 unx     6921 b- defN 23-Jan-26 14:47 std_buffer/gigafrost/data.py
 -rw-r--r--  2.0 unx     6761 b- defN 23-Apr-25 18:01 std_buffer/gigafrost/udp_sim_gf.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-17 08:47 std_buffer/jungfrau/__init__.py
 -rw-r--r--  2.0 unx     1887 b- defN 23-Jan-17 08:47 std_buffer/jungfrau/data.py
 -rw-r--r--  2.0 unx     2129 b- defN 23-Jan-17 08:47 std_buffer/jungfrau/extract_gains_and_pedestals_for_module.py
 -rw-r--r--  2.0 unx     3657 b- defN 23-Jun-06 09:12 std_buffer/jungfrau/stream_binary_jf_sim.py
 -rw-r--r--  2.0 unx     3966 b- defN 23-Jun-07 13:50 std_buffer/jungfrau/udp_sim_jf.py
--rw-r--r--  2.0 unx      277 b- defN 23-Jun-26 09:52 std_buffer-0.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 09:52 std_buffer-0.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-26 09:52 std_buffer-0.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1478 b- defN 23-Jun-26 09:52 std_buffer-0.0.0.dist-info/RECORD
-17 files, 37057 bytes uncompressed, 12101 bytes compressed:  67.3%
+-rw-r--r--  2.0 unx      277 b- defN 23-Jun-26 12:34 std_buffer-0.6.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 12:34 std_buffer-0.6.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-26 12:34 std_buffer-0.6.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1478 b- defN 23-Jun-26 12:34 std_buffer-0.6.6.dist-info/RECORD
+17 files, 37057 bytes uncompressed, 12106 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: std_buffer/jungfrau/stream_binary_jf_sim.py
 Comment: 
 
 Filename: std_buffer/jungfrau/udp_sim_jf.py
 Comment: 
 
-Filename: std_buffer-0.0.0.dist-info/METADATA
+Filename: std_buffer-0.6.6.dist-info/METADATA
 Comment: 
 
-Filename: std_buffer-0.0.0.dist-info/WHEEL
+Filename: std_buffer-0.6.6.dist-info/WHEEL
 Comment: 
 
-Filename: std_buffer-0.0.0.dist-info/top_level.txt
+Filename: std_buffer-0.6.6.dist-info/top_level.txt
 Comment: 
 
-Filename: std_buffer-0.0.0.dist-info/RECORD
+Filename: std_buffer-0.6.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `std_buffer-0.0.0.dist-info/RECORD` & `std_buffer-0.6.6.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 std_buffer/gigafrost/data.py,sha256=eRsggpkU6skhRE4ownz7yo-91ZxkBHOQQAXmI7f1nkQ,6921
 std_buffer/gigafrost/udp_sim_gf.py,sha256=PuBl3pD4Bq7opSJtgxgaZGePr0laQ63QklYL0mEZTp0,6761
 std_buffer/jungfrau/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 std_buffer/jungfrau/data.py,sha256=Q9YfiiU7i9DMR8KRm0TpG7y95pNO2ilXhVFsNcCyo8g,1887
 std_buffer/jungfrau/extract_gains_and_pedestals_for_module.py,sha256=D7dx6VFHOlG-Q0at9_2cQvHh9U_g_nW1ZRI5B6w0EyM,2129
 std_buffer/jungfrau/stream_binary_jf_sim.py,sha256=FibkwUgo7Yz5z5IUt4hRCDVh9Fan3CSxRb8TjS8m81E,3657
 std_buffer/jungfrau/udp_sim_jf.py,sha256=2ghli5dHCxCHGYtvnpjtvGV7sBH57119YoDKayTLEpI,3966
-std_buffer-0.0.0.dist-info/METADATA,sha256=-4Np8XJojmognScK0YsYRgLLcv9WqoT0uuGXTERYXDg,277
-std_buffer-0.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-std_buffer-0.0.0.dist-info/top_level.txt,sha256=HGlRsZdZHQhV_hF_Yc15cqbXUBj9o8phzwWh0fxAMQA,11
-std_buffer-0.0.0.dist-info/RECORD,,
+std_buffer-0.6.6.dist-info/METADATA,sha256=iIEjx4i6aDgsr3XcFAiucrkua_KrC3_VZqshCnzx0Zk,277
+std_buffer-0.6.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+std_buffer-0.6.6.dist-info/top_level.txt,sha256=HGlRsZdZHQhV_hF_Yc15cqbXUBj9o8phzwWh0fxAMQA,11
+std_buffer-0.6.6.dist-info/RECORD,,
```

