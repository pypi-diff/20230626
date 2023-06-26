# Comparing `tmp/libknot-3.2.7.tar.gz` & `tmp/libknot-3.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libknot-3.2.7.tar", last modified: Tue Jun  6 05:13:47 2023, max compression
+gzip compressed data, was "libknot-3.2.8.tar", last modified: Mon Jun 26 05:51:49 2023, max compression
```

## Comparing `libknot-3.2.7.tar` & `libknot-3.2.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 dsalzman  (1000) dsalzman  (1000)        0 2023-06-06 05:13:47.284194 libknot-3.2.7/
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     4489 2023-06-06 05:13:47.284194 libknot-3.2.7/PKG-INFO
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     3753 2022-12-12 06:51:42.000000 libknot-3.2.7/README.md
-drwxrwxr-x   0 dsalzman  (1000) dsalzman  (1000)        0 2023-06-06 05:13:47.284194 libknot-3.2.7/libknot/
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     2457 2023-06-06 05:13:15.000000 libknot-3.2.7/libknot/__init__.py
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)    10988 2022-10-03 08:30:42.000000 libknot-3.2.7/libknot/control.py
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     2088 2022-12-12 06:51:42.000000 libknot-3.2.7/libknot/dname.py
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     9802 2023-02-02 10:28:39.000000 libknot-3.2.7/libknot/probe.py
-drwxrwxr-x   0 dsalzman  (1000) dsalzman  (1000)        0 2023-06-06 05:13:47.284194 libknot-3.2.7/libknot.egg-info/
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     4489 2023-06-06 05:13:47.000000 libknot-3.2.7/libknot.egg-info/PKG-INFO
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)      215 2023-06-06 05:13:47.000000 libknot-3.2.7/libknot.egg-info/SOURCES.txt
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)        1 2023-06-06 05:13:47.000000 libknot-3.2.7/libknot.egg-info/dependency_links.txt
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)        8 2023-06-06 05:13:47.000000 libknot-3.2.7/libknot.egg-info/top_level.txt
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)       38 2023-06-06 05:13:47.284194 libknot-3.2.7/setup.cfg
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     1004 2023-06-06 05:13:15.000000 libknot-3.2.7/setup.py
+drwxrwxr-x   0 dsalzman  (1000) dsalzman  (1000)        0 2023-06-26 05:51:49.971862 libknot-3.2.8/
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     4876 2023-06-26 05:51:49.971862 libknot-3.2.8/PKG-INFO
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     4140 2023-06-26 05:51:16.000000 libknot-3.2.8/README.md
+drwxrwxr-x   0 dsalzman  (1000) dsalzman  (1000)        0 2023-06-26 05:51:49.971862 libknot-3.2.8/libknot/
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     2457 2023-06-26 05:51:37.000000 libknot-3.2.8/libknot/__init__.py
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)    10988 2022-10-03 08:30:42.000000 libknot-3.2.8/libknot/control.py
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     2862 2023-06-26 05:51:16.000000 libknot-3.2.8/libknot/dname.py
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     9802 2023-02-02 10:28:39.000000 libknot-3.2.8/libknot/probe.py
+drwxrwxr-x   0 dsalzman  (1000) dsalzman  (1000)        0 2023-06-26 05:51:49.971862 libknot-3.2.8/libknot.egg-info/
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     4876 2023-06-26 05:51:49.000000 libknot-3.2.8/libknot.egg-info/PKG-INFO
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)      215 2023-06-26 05:51:49.000000 libknot-3.2.8/libknot.egg-info/SOURCES.txt
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)        1 2023-06-26 05:51:49.000000 libknot-3.2.8/libknot.egg-info/dependency_links.txt
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)        8 2023-06-26 05:51:49.000000 libknot-3.2.8/libknot.egg-info/top_level.txt
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)       38 2023-06-26 05:51:49.971862 libknot-3.2.8/setup.cfg
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     1004 2023-06-26 05:51:37.000000 libknot-3.2.8/setup.py
```

### Comparing `libknot-3.2.7/PKG-INFO` & `libknot-3.2.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libknot
-Version: 3.2.7
+Version: 3.2.8
 Summary: Python bindings for libknot
 Home-page: https://gitlab.nic.cz/knot/knot-dns
 Author: Daniel Salzman
 Author-email: daniel.salzman@nic.cz
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -150,20 +150,24 @@
 Then the dname can be reformatted to wire format or back to textual format.
 
 ### Dname module example
 
 ```python3
 import libknot.dname
 
-dname = libknot.dname.KnotDname("e\\120ample.c\om.")
-print(dname.size()
-print(dname.str())
-print(dname.wire())
+dname1 = libknot.dname.KnotDname("knot-dns.cz")
+print("%s: wire: %s size: %u" % (dname1.str(), dname1.wire(), dname1.size()))
+
+dname2 = libknot.dname.KnotDname("e\\120ample.c\om.")
+print("%s: wire: %s size: %u" % (dname2.str(), dname2.wire(), dname2.size()))
+
+dname3 = libknot.dname.KnotDname(dname_wire=b'\x02cz\x00')
+print("%s: wire: %s size: %u" % (dname3.str(), dname3.wire(), dname3.size()))
 ```
 
 ```bash
-13
-example.com.
-b'\x07example\x03com\x00'
+knot-dns.cz.: wire: b'\x08knot-dns\x02cz\x00' size: 13
+example.com.: wire: b'\x07example\x03com\x00' size: 13
+cz.: wire: b'\x02cz\x00' size: 4
 ```
```

### Comparing `libknot-3.2.7/README.md` & `libknot-3.2.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -130,18 +130,22 @@
 Then the dname can be reformatted to wire format or back to textual format.
 
 ### Dname module example
 
 ```python3
 import libknot.dname
 
-dname = libknot.dname.KnotDname("e\\120ample.c\om.")
-print(dname.size()
-print(dname.str())
-print(dname.wire())
+dname1 = libknot.dname.KnotDname("knot-dns.cz")
+print("%s: wire: %s size: %u" % (dname1.str(), dname1.wire(), dname1.size()))
+
+dname2 = libknot.dname.KnotDname("e\\120ample.c\om.")
+print("%s: wire: %s size: %u" % (dname2.str(), dname2.wire(), dname2.size()))
+
+dname3 = libknot.dname.KnotDname(dname_wire=b'\x02cz\x00')
+print("%s: wire: %s size: %u" % (dname3.str(), dname3.wire(), dname3.size()))
 ```
 
 ```bash
-13
-example.com.
-b'\x07example\x03com\x00'
+knot-dns.cz.: wire: b'\x08knot-dns\x02cz\x00' size: 13
+example.com.: wire: b'\x07example\x03com\x00' size: 13
+cz.: wire: b'\x02cz\x00' size: 4
 ```
```

### Comparing `libknot-3.2.7/libknot/__init__.py` & `libknot-3.2.8/libknot/__init__.py`

 * *Files identical despite different names*

### Comparing `libknot-3.2.7/libknot/control.py` & `libknot-3.2.8/libknot/control.py`

 * *Files identical despite different names*

### Comparing `libknot-3.2.7/libknot/dname.py` & `libknot-3.2.8/libknot/dname.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,40 +10,55 @@
     CAPACITY = 255
     CAPACITY_TXT = 1004
 
     DnameStorage = ctypes.c_char * CAPACITY
     DnameTxtStorage = ctypes.c_char * CAPACITY_TXT
 
     SIZE = None
+    CHECK = None
     TO_STR = None
     FROM_STR = None
 
     data = None
 
-    def __init__(self, dname: str = None) -> None:
-        """Initializes a dname storage. Optionally initializes from a string."""
+    def __init__(self, dname_str: str = None, dname_wire: bytes = None) -> None:
+        """Initializes a dname storage. Optionally initializes from a string or wire."""
 
         if not KnotDname.SIZE:
             libknot.Knot()
 
             KnotDname.SIZE = libknot.Knot.LIBKNOT.knot_dname_size
             KnotDname.SIZE.restype = ctypes.c_size_t
             KnotDname.SIZE.argtypes = [KnotDname.DnameStorage]
 
+            KnotDname.CHECK = libknot.Knot.LIBKNOT.knot_dname_wire_check
+            KnotDname.CHECK.restype = ctypes.c_int
+            KnotDname.CHECK.argtypes = [ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p]
+
             KnotDname.TO_STR = libknot.Knot.LIBKNOT.knot_dname_to_str
             KnotDname.TO_STR.restype = ctypes.c_char_p
             KnotDname.TO_STR.argtypes = [KnotDname.DnameTxtStorage, KnotDname.DnameStorage, ctypes.c_size_t]
 
             KnotDname.FROM_STR = libknot.Knot.LIBKNOT.knot_dname_from_str
             KnotDname.FROM_STR.restype = ctypes.c_char_p
             KnotDname.FROM_STR.argtypes = [KnotDname.DnameStorage, ctypes.c_char_p, ctypes.c_size_t]
 
-        if dname:
+        if dname_str:
+            self.data = KnotDname.DnameStorage()
+            if not KnotDname.FROM_STR(self.data, dname_str.encode('utf-8'), KnotDname.CAPACITY):
+                raise ValueError
+        elif dname_wire:
+            size = len(dname_wire)
+            if size > KnotDname.CAPACITY:
+                raise ValueError
             self.data = KnotDname.DnameStorage()
-            if not KnotDname.FROM_STR(self.data, dname.encode('utf-8'), KnotDname.CAPACITY):
+            ctypes.memmove(self.data, dname_wire, size)
+            start = ctypes.cast(self.data, ctypes.POINTER(ctypes.c_char * size))[0]
+            end = ctypes.cast(self.data, ctypes.POINTER(ctypes.c_char * size))[1]
+            if KnotDname.CHECK(start, end, start) <= 0:
                 raise ValueError
 
     def size(self):
         """Returns size of the stored dname."""
 
         if self.data:
             return KnotDname.SIZE(self.data)
```

### Comparing `libknot-3.2.7/libknot/probe.py` & `libknot-3.2.8/libknot/probe.py`

 * *Files identical despite different names*

### Comparing `libknot-3.2.7/libknot.egg-info/PKG-INFO` & `libknot-3.2.8/libknot.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libknot
-Version: 3.2.7
+Version: 3.2.8
 Summary: Python bindings for libknot
 Home-page: https://gitlab.nic.cz/knot/knot-dns
 Author: Daniel Salzman
 Author-email: daniel.salzman@nic.cz
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -150,20 +150,24 @@
 Then the dname can be reformatted to wire format or back to textual format.
 
 ### Dname module example
 
 ```python3
 import libknot.dname
 
-dname = libknot.dname.KnotDname("e\\120ample.c\om.")
-print(dname.size()
-print(dname.str())
-print(dname.wire())
+dname1 = libknot.dname.KnotDname("knot-dns.cz")
+print("%s: wire: %s size: %u" % (dname1.str(), dname1.wire(), dname1.size()))
+
+dname2 = libknot.dname.KnotDname("e\\120ample.c\om.")
+print("%s: wire: %s size: %u" % (dname2.str(), dname2.wire(), dname2.size()))
+
+dname3 = libknot.dname.KnotDname(dname_wire=b'\x02cz\x00')
+print("%s: wire: %s size: %u" % (dname3.str(), dname3.wire(), dname3.size()))
 ```
 
 ```bash
-13
-example.com.
-b'\x07example\x03com\x00'
+knot-dns.cz.: wire: b'\x08knot-dns\x02cz\x00' size: 13
+example.com.: wire: b'\x07example\x03com\x00' size: 13
+cz.: wire: b'\x02cz\x00' size: 4
 ```
```

### Comparing `libknot-3.2.7/setup.py` & `libknot-3.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 p = pathlib.Path("README.md")
 if p.exists():
     long_description = p.read_text()
 
 setuptools.setup(
     name='libknot',
-    version='3.2.7',
+    version='3.2.8',
     description='Python bindings for libknot',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Daniel Salzman',
     author_email='daniel.salzman@nic.cz',
     url='https://gitlab.nic.cz/knot/knot-dns',
     license='GPL-3.0',
```

