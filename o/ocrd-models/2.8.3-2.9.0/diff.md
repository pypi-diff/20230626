# Comparing `tmp/ocrd_models-2.8.3.tar.gz` & `tmp/ocrd_models-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ocrd_models-2.8.3.tar", last modified: Mon Jun  8 16:56:34 2020, max compression
+gzip compressed data, was "dist/ocrd_models-2.9.0.tar", last modified: Tue Jun  9 17:33:31 2020, max compression
```

## Comparing `ocrd_models-2.8.3.tar` & `ocrd_models-2.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-08 16:56:34.000000 ocrd_models-2.8.3/
--rw-rw-r--   0 kba       (1000) kba       (1000)       38 2020-06-08 16:56:34.000000 ocrd_models-2.8.3/setup.cfg
--rw-rw-r--   0 kba       (1000) kba       (1000)      721 2020-05-12 11:01:01.000000 ocrd_models-2.8.3/setup.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     1865 2020-06-08 16:56:34.000000 ocrd_models-2.8.3/PKG-INFO
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-08 16:56:34.000000 ocrd_models-2.8.3/ocrd_models/
--rw-rw-r--   0 kba       (1000) kba       (1000)     3464 2020-05-12 11:01:01.000000 ocrd_models-2.8.3/ocrd_models/ocrd_agent.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     1218 2020-06-08 11:38:59.000000 ocrd_models-2.8.3/ocrd_models/mets-empty.xml
--rw-rw-r--   0 kba       (1000) kba       (1000)    14956 2020-06-07 19:05:48.000000 ocrd_models-2.8.3/ocrd_models/ocrd_mets.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     2655 2020-05-12 11:01:01.000000 ocrd_models-2.8.3/ocrd_models/ocrd_exif.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     1526 2020-05-12 11:01:01.000000 ocrd_models-2.8.3/ocrd_models/ocrd_xml_base.py
--rw-rw-r--   0 kba       (1000) kba       (1000)      242 2020-05-12 11:01:01.000000 ocrd_models-2.8.3/ocrd_models/__init__.py
--rw-rw-r--   0 kba       (1000) kba       (1000)   682689 2020-06-08 11:57:16.000000 ocrd_models-2.8.3/ocrd_models/ocrd_page_generateds.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     2185 2020-06-08 11:57:16.000000 ocrd_models-2.8.3/ocrd_models/constants.py
--rw-rw-r--   0 kba       (1000) kba       (1000)      557 2020-05-12 11:01:01.000000 ocrd_models-2.8.3/ocrd_models/utils.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     3068 2020-06-07 19:05:48.000000 ocrd_models-2.8.3/ocrd_models/ocrd_page.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     6205 2020-06-08 11:38:59.000000 ocrd_models-2.8.3/ocrd_models/ocrd_file.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     1141 2020-06-07 19:05:48.000000 ocrd_models-2.8.3/README.md
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-08 16:56:34.000000 ocrd_models-2.8.3/ocrd_models.egg-info/
--rw-rw-r--   0 kba       (1000) kba       (1000)      480 2020-06-08 16:56:34.000000 ocrd_models-2.8.3/ocrd_models.egg-info/SOURCES.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)       23 2020-06-08 16:56:34.000000 ocrd_models-2.8.3/ocrd_models.egg-info/requires.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)       12 2020-06-08 16:56:34.000000 ocrd_models-2.8.3/ocrd_models.egg-info/top_level.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)     1865 2020-06-08 16:56:34.000000 ocrd_models-2.8.3/ocrd_models.egg-info/PKG-INFO
--rw-rw-r--   0 kba       (1000) kba       (1000)        1 2020-06-08 16:56:34.000000 ocrd_models-2.8.3/ocrd_models.egg-info/dependency_links.txt
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-09 17:33:31.000000 ocrd_models-2.9.0/
+-rw-rw-r--   0 kba       (1000) kba       (1000)       38 2020-06-09 17:33:31.000000 ocrd_models-2.9.0/setup.cfg
+-rw-rw-r--   0 kba       (1000) kba       (1000)      721 2020-05-12 11:01:01.000000 ocrd_models-2.9.0/setup.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     1865 2020-06-09 17:33:31.000000 ocrd_models-2.9.0/PKG-INFO
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-09 17:33:31.000000 ocrd_models-2.9.0/ocrd_models/
+-rw-rw-r--   0 kba       (1000) kba       (1000)     3464 2020-05-12 11:01:01.000000 ocrd_models-2.9.0/ocrd_models/ocrd_agent.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     1218 2020-06-09 17:08:17.000000 ocrd_models-2.9.0/ocrd_models/mets-empty.xml
+-rw-rw-r--   0 kba       (1000) kba       (1000)    15092 2020-06-09 17:09:11.000000 ocrd_models-2.9.0/ocrd_models/ocrd_mets.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     2655 2020-05-12 11:01:01.000000 ocrd_models-2.9.0/ocrd_models/ocrd_exif.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     1526 2020-05-12 11:01:01.000000 ocrd_models-2.9.0/ocrd_models/ocrd_xml_base.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      242 2020-05-12 11:01:01.000000 ocrd_models-2.9.0/ocrd_models/__init__.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)   682689 2020-06-09 13:50:15.000000 ocrd_models-2.9.0/ocrd_models/ocrd_page_generateds.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     2264 2020-06-09 17:09:11.000000 ocrd_models-2.9.0/ocrd_models/constants.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      557 2020-05-12 11:01:01.000000 ocrd_models-2.9.0/ocrd_models/utils.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     3068 2020-06-09 13:50:15.000000 ocrd_models-2.9.0/ocrd_models/ocrd_page.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     6205 2020-06-09 17:08:17.000000 ocrd_models-2.9.0/ocrd_models/ocrd_file.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     1141 2020-06-09 13:50:15.000000 ocrd_models-2.9.0/README.md
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-09 17:33:31.000000 ocrd_models-2.9.0/ocrd_models.egg-info/
+-rw-rw-r--   0 kba       (1000) kba       (1000)      480 2020-06-09 17:33:30.000000 ocrd_models-2.9.0/ocrd_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)       23 2020-06-09 17:33:30.000000 ocrd_models-2.9.0/ocrd_models.egg-info/requires.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)       12 2020-06-09 17:33:30.000000 ocrd_models-2.9.0/ocrd_models.egg-info/top_level.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)     1865 2020-06-09 17:33:30.000000 ocrd_models-2.9.0/ocrd_models.egg-info/PKG-INFO
+-rw-rw-r--   0 kba       (1000) kba       (1000)        1 2020-06-09 17:33:30.000000 ocrd_models-2.9.0/ocrd_models.egg-info/dependency_links.txt
```

### Comparing `ocrd_models-2.8.3/setup.py` & `ocrd_models-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `ocrd_models-2.8.3/PKG-INFO` & `ocrd_models-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocrd_models
-Version: 2.8.3
+Version: 2.9.0
 Summary: OCR-D framework - file format APIs and schemas
 Home-page: https://github.com/OCR-D/core
 Author: Konstantin Baierer
 Author-email: unixprog@gmail.com
 License: Apache License 2.0
 Description: # ocrd_models
```

### Comparing `ocrd_models-2.8.3/ocrd_models/ocrd_agent.py` & `ocrd_models-2.9.0/ocrd_models/ocrd_agent.py`

 * *Files identical despite different names*

### Comparing `ocrd_models-2.8.3/ocrd_models/mets-empty.xml` & `ocrd_models-2.9.0/ocrd_models/mets-empty.xml`

 * *Files identical despite different names*

### Comparing `ocrd_models-2.8.3/ocrd_models/ocrd_mets.py` & `ocrd_models-2.9.0/ocrd_models/ocrd_mets.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     TAG_METS_FILESEC,
     TAG_METS_FPTR,
     TAG_METS_METSHDR,
     TAG_METS_STRUCTMAP,
     IDENTIFIER_PRIORITY,
     TAG_MODS_IDENTIFIER,
     METS_XML_EMPTY,
+    REGEX_FILE_ID
 )
 
 from .ocrd_xml_base import OcrdXmlDocument, ET
 from .ocrd_file import OcrdFile
 from .ocrd_agent import OcrdAgent
 
 log = getLogger('ocrd_models.ocrd_mets')
@@ -245,14 +246,16 @@
             pageId (string):
             force (boolean): Whether to add the file even if a ``mets:file`` with the same ``ID`` already exists.
             local_filename (string):
             mimetype (string):
         """
         if not ID:
             raise Exception("Must set ID of the mets:file")
+        elif not REGEX_FILE_ID.fullmatch(ID):
+            raise Exception("Invalid syntax for mets:file/@ID %s" % ID)
         el_fileGrp = self._tree.getroot().find(".//mets:fileGrp[@USE='%s']" % (fileGrp), NS)
         if el_fileGrp is None:
             el_fileGrp = self.add_file_group(fileGrp)
         if ID is not None and self.find_files(ID=ID) != []:
             if not force:
                 raise Exception("File with ID='%s' already exists" % ID)
             mets_file = self.find_files(ID=ID)[0]
```

### Comparing `ocrd_models-2.8.3/ocrd_models/ocrd_exif.py` & `ocrd_models-2.9.0/ocrd_models/ocrd_exif.py`

 * *Files identical despite different names*

### Comparing `ocrd_models-2.8.3/ocrd_models/ocrd_xml_base.py` & `ocrd_models-2.9.0/ocrd_models/ocrd_xml_base.py`

 * *Files identical despite different names*

### Comparing `ocrd_models-2.8.3/ocrd_models/ocrd_page_generateds.py` & `ocrd_models-2.9.0/ocrd_models/ocrd_page_generateds.py`

 * *Files identical despite different names*

### Comparing `ocrd_models-2.8.3/ocrd_models/constants.py` & `ocrd_models-2.9.0/ocrd_models/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Constants for ocrd_models.
 """
 from pkg_resources import resource_string
+import re
 
 __all__ = [
     'IDENTIFIER_PRIORITY',
     'METS_XML_EMPTY',
     'NAMESPACES',
     'TAG_METS_AGENT',
     'TAG_METS_DIV',
@@ -20,17 +21,20 @@
     'TAG_MODS_IDENTIFIER',
     'TAG_PAGE_ALTERNATIVEIMAGE',
     'TAG_PAGE_COORDS',
     'TAG_PAGE_READINGORDER',
     'TAG_PAGE_REGIONREFINDEXED',
     'TAG_PAGE_TEXTLINE',
     'TAG_PAGE_TEXTEQUIV',
-    'TAG_PAGE_TEXTREGION'
+    'TAG_PAGE_TEXTREGION',
+    'REGEX_FILE_ID',
 ]
 
+REGEX_FILE_ID = re.compile('^[A-Za-z][^:]*$')
+
 IDENTIFIER_PRIORITY = ['purl', 'urn', 'doi', 'url']
 
 METS_XML_EMPTY = resource_string(__name__, 'mets-empty.xml')
 
 NAMESPACES = {
     'mets': "http://www.loc.gov/METS/",
     'mods': "http://www.loc.gov/mods/v3",
```

### Comparing `ocrd_models-2.8.3/ocrd_models/utils.py` & `ocrd_models-2.9.0/ocrd_models/utils.py`

 * *Files identical despite different names*

### Comparing `ocrd_models-2.8.3/ocrd_models/ocrd_page.py` & `ocrd_models-2.9.0/ocrd_models/ocrd_page.py`

 * *Files identical despite different names*

### Comparing `ocrd_models-2.8.3/ocrd_models/ocrd_file.py` & `ocrd_models-2.9.0/ocrd_models/ocrd_file.py`

 * *Files identical despite different names*

### Comparing `ocrd_models-2.8.3/README.md` & `ocrd_models-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ocrd_models-2.8.3/ocrd_models.egg-info/PKG-INFO` & `ocrd_models-2.9.0/ocrd_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocrd-models
-Version: 2.8.3
+Version: 2.9.0
 Summary: OCR-D framework - file format APIs and schemas
 Home-page: https://github.com/OCR-D/core
 Author: Konstantin Baierer
 Author-email: unixprog@gmail.com
 License: Apache License 2.0
 Description: # ocrd_models
```

