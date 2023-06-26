# Comparing `tmp/py_dmidecode-0.1.1.tar.gz` & `tmp/py_dmidecode-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_dmidecode-0.1.1.tar", max compression
+gzip compressed data, was "py_dmidecode-0.1.2.tar", max compression
```

## Comparing `py_dmidecode-0.1.1.tar` & `py_dmidecode-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    11357 2019-10-06 18:35:46.000000 py_dmidecode-0.1.1/LICENSE
--rw-r--r--   0        0        0      945 2023-05-21 17:58:12.203993 py_dmidecode-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-21 17:58:12.204299 py_dmidecode-0.1.1/py_dmidecode/__init__.py
--rw-r--r--   0        0        0     7166 2023-05-21 17:58:12.211247 py_dmidecode-0.1.1/py_dmidecode/dmidecode.py
--rw-r--r--   0        0        0     1184 2023-05-21 17:59:04.926462 py_dmidecode-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2090 1970-01-01 00:00:00.000000 py_dmidecode-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2019-10-06 18:35:46.000000 py_dmidecode-0.1.2/LICENSE
+-rw-r--r--   0        0        0      927 2023-06-26 18:29:30.410688 py_dmidecode-0.1.2/README.md
+-rw-r--r--   0        0        0      141 2023-06-26 18:29:30.411072 py_dmidecode-0.1.2/dmidecode/__init__.py
+-rw-r--r--   0        0        0      700 2023-06-26 18:29:30.411267 py_dmidecode-0.1.2/dmidecode/decode.py
+-rw-r--r--   0        0        0     6484 2023-06-26 18:29:30.411490 py_dmidecode-0.1.2/dmidecode/parse.py
+-rw-r--r--   0        0        0     1181 2023-06-26 18:29:54.542658 py_dmidecode-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 py_dmidecode-0.1.2/PKG-INFO
```

### Comparing `py_dmidecode-0.1.1/LICENSE` & `py_dmidecode-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_dmidecode-0.1.1/README.md` & `py_dmidecode-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 Small tool that parses output of dmidecode command
 
 ## How to use
 
 ```python
 from dmidecode import DMIDecode
-import subprocess
 
 # create parsing instance by passing dmidecode output
 dmi = DMIDecode()
 
 # some of the pre-defined queries
 print('Manufacturer:\t', dmi.manufacturer())
 print('Model:\t\t', dmi.model())
```

### Comparing `py_dmidecode-0.1.1/py_dmidecode/dmidecode.py` & `py_dmidecode-0.1.2/dmidecode/parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import re
-import subprocess
 
 
 class DMIParse:
     """
     dmidecode information parsing object
     requires dmidecode output as input string
     """
@@ -120,15 +119,15 @@
             record_element = record.splitlines()
 
             #  Entries with less than 3 lines are incomplete / inactive
             #  skip them
             if len(record_element) < 3:
                 continue
 
-            handle_data = DMIDecode.handle_re.findall(record_element[0])
+            handle_data = self.handle_re.findall(record_element[0])
 
             if not handle_data:
                 continue
             handle_data = handle_data[0]
 
             dmi_handle = handle_data[0]
 
@@ -144,15 +143,15 @@
 
             #  Loop over the rest of the record, gathering values
             for i in range(2, len(record_element), 1):
                 if i >= len(record_element):
                     break
                 #  Check whether we are inside a \t\t block
                 if in_block_elemet != "":
-                    in_block_data = DMIDecode.in_block_re.findall(record_element[1])
+                    in_block_data = self.in_block_re.findall(record_element[1])
 
                     if in_block_data:
                         if not in_block_list:
                             in_block_list = in_block_data[0][0]
                         else:
                             in_block_list = in_block_list + "\t\t"
                             +in_block_data[0][1]
@@ -160,23 +159,23 @@
                         data[dmi_handle][in_block_elemet] = in_block_list
                         continue
                     else:
                         # We are out of the \t\t block; reset it again, and let
                         # the parsing continue
                         in_block_elemet = ""
 
-                record_data = DMIDecode.record_re.findall(record_element[i])
+                record_data = self.record_re.findall(record_element[i])
 
                 #  Is this the line containing handle identifier, type, size?
                 if record_data:
                     data[dmi_handle][record_data[0][0]] = record_data[0][1]
                     continue
 
                 #  Didn't findall regular entry, maybe an array of data?
-                record_data2 = DMIDecode.record2_re.findall(record_element[i])
+                record_data2 = self.record2_re.findall(record_element[i])
 
                 if record_data2:
                     #  This is an array of data - let the loop know we are
                     #  inside an array block
                     in_block_elemet = record_data2[0][0]
                     continue
         return data
@@ -190,25 +189,7 @@
             return 0
         if "MB" in value:
             return nb / 1024 if nb else 0
         elif "GB" in value:
             return nb
         else:
             return 0
-
-
-class DMIDecode(DMIParse):
-    """Wrapper over DMIParse which runs dmidecode locally"""
-
-    def __init__(self, command="dmidecode"):
-        self.dmidecode = command
-        raw = self._run()
-        super().__init__(raw)
-
-    def _run(self):
-        # let subprocess merge stderr with stdout
-        with subprocess.Popen(self.dmidecode, stderr=subprocess.STDOUT, stdout=subprocess.PIPE) as proc:
-            stdout, _ = proc.communicate()
-            if proc.returncode > 0:
-                raise RuntimeError("{} failed with an error:\n{}".format(self.dmidecode, stdout.decode()))
-            else:
-                return stdout.decode()
```

### Comparing `py_dmidecode-0.1.1/pyproject.toml` & `py_dmidecode-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,18 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 description = "python library to parse the output of dmidecode"
 homepage = "https://github.com/zaibon/py-dmidecode"
 keywords = ["system development"]
 name = "py-dmidecode"
-packages = [{include = "py_dmidecode"}]
+packages = [{include = "dmidecode"}]
 readme = "README.md"
 repository = "https://github.com/zaibon/py-dmidecode"
-version = "0.1.1"
+version = "0.1.2"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/zaibon/py-dmidecode/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
```

### Comparing `py_dmidecode-0.1.1/PKG-INFO` & `py_dmidecode-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 Metadata-Version: 2.1
 Name: py-dmidecode
-Version: 0.1.1
+Version: 0.1.2
 Summary: python library to parse the output of dmidecode
 Home-page: https://github.com/zaibon/py-dmidecode
 Keywords: system development
 Author: Christophe de Carvalho
 Author-email: christophe.dcpm@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Bug Tracker, https://github.com/zaibon/py-dmidecode/issues
 Project-URL: Repository, https://github.com/zaibon/py-dmidecode
 Description-Content-Type: text/markdown
 
 # py-dmidecode
 
 Small tool that parses output of dmidecode command
 
 ## How to use
 
 ```python
 from dmidecode import DMIDecode
-import subprocess
 
 # create parsing instance by passing dmidecode output
 dmi = DMIDecode()
 
 # some of the pre-defined queries
 print('Manufacturer:\t', dmi.manufacturer())
 print('Model:\t\t', dmi.model())
```

