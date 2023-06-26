# Comparing `tmp/ocrd_validators-2.8.3.tar.gz` & `tmp/ocrd_validators-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ocrd_validators-2.8.3.tar", last modified: Mon Jun  8 16:56:37 2020, max compression
+gzip compressed data, was "dist/ocrd_validators-2.9.0.tar", last modified: Tue Jun  9 17:33:34 2020, max compression
```

## Comparing `ocrd_validators-2.8.3.tar` & `ocrd_validators-2.9.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-08 16:56:37.000000 ocrd_validators-2.8.3/
--rw-rw-r--   0 kba       (1000) kba       (1000)       38 2020-06-08 16:56:37.000000 ocrd_validators-2.8.3/setup.cfg
--rw-rw-r--   0 kba       (1000) kba       (1000)      844 2020-06-07 20:54:07.000000 ocrd_validators-2.8.3/setup.py
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-08 16:56:37.000000 ocrd_validators-2.8.3/ocrd_validators.egg-info/
--rw-rw-r--   0 kba       (1000) kba       (1000)      518 2020-06-08 16:56:37.000000 ocrd_validators-2.8.3/ocrd_validators.egg-info/SOURCES.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)      131 2020-06-08 16:56:37.000000 ocrd_validators-2.8.3/ocrd_validators.egg-info/requires.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)       16 2020-06-08 16:56:37.000000 ocrd_validators-2.8.3/ocrd_validators.egg-info/top_level.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)      449 2020-06-08 16:56:37.000000 ocrd_validators-2.8.3/ocrd_validators.egg-info/PKG-INFO
--rw-rw-r--   0 kba       (1000) kba       (1000)        1 2020-06-08 16:56:37.000000 ocrd_validators-2.8.3/ocrd_validators.egg-info/dependency_links.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)      449 2020-06-08 16:56:37.000000 ocrd_validators-2.8.3/PKG-INFO
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-08 16:56:37.000000 ocrd_validators-2.8.3/ocrd_validators/
--rw-rw-r--   0 kba       (1000) kba       (1000)     2218 2020-05-12 11:01:01.000000 ocrd_validators-2.8.3/ocrd_validators/json_validator.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     2026 2020-05-12 11:01:01.000000 ocrd_validators-2.8.3/ocrd_validators/report.py
--rw-rw-r--   0 kba       (1000) kba       (1000)    22815 2020-06-07 19:05:48.000000 ocrd_validators-2.8.3/ocrd_validators/page_validator.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     3663 2020-05-12 11:01:01.000000 ocrd_validators-2.8.3/ocrd_validators/ocrd_zip_validator.py
--rw-rw-r--   0 kba       (1000) kba       (1000)      505 2020-06-07 20:54:07.000000 ocrd_validators-2.8.3/ocrd_validators/__init__.py
--rw-rw-r--   0 kba       (1000) kba       (1000)      548 2020-05-12 11:01:01.000000 ocrd_validators-2.8.3/ocrd_validators/ocrd_tool_validator.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     1405 2020-05-12 11:01:01.000000 ocrd_validators-2.8.3/ocrd_validators/parameter_validator.py
--rw-rw-r--   0 kba       (1000) kba       (1000)      524 2020-06-08 16:36:05.000000 ocrd_validators-2.8.3/ocrd_validators/constants.py
--rw-rw-r--   0 kba       (1000) kba       (1000)    12176 2020-06-08 11:57:16.000000 ocrd_validators-2.8.3/ocrd_validators/workspace_validator.py
--rw-rw-r--   0 kba       (1000) kba       (1000)       86 2020-05-12 11:01:01.000000 ocrd_validators-2.8.3/README.md
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-09 17:33:34.000000 ocrd_validators-2.9.0/
+-rw-rw-r--   0 kba       (1000) kba       (1000)       38 2020-06-09 17:33:34.000000 ocrd_validators-2.9.0/setup.cfg
+-rw-rw-r--   0 kba       (1000) kba       (1000)      853 2020-06-09 17:08:17.000000 ocrd_validators-2.9.0/setup.py
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-09 17:33:34.000000 ocrd_validators-2.9.0/ocrd_validators.egg-info/
+-rw-rw-r--   0 kba       (1000) kba       (1000)      627 2020-06-09 17:33:34.000000 ocrd_validators-2.9.0/ocrd_validators.egg-info/SOURCES.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)      131 2020-06-09 17:33:34.000000 ocrd_validators-2.9.0/ocrd_validators.egg-info/requires.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)       16 2020-06-09 17:33:34.000000 ocrd_validators-2.9.0/ocrd_validators.egg-info/top_level.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)      449 2020-06-09 17:33:34.000000 ocrd_validators-2.9.0/ocrd_validators.egg-info/PKG-INFO
+-rw-rw-r--   0 kba       (1000) kba       (1000)        1 2020-06-09 17:33:34.000000 ocrd_validators-2.9.0/ocrd_validators.egg-info/dependency_links.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)      449 2020-06-09 17:33:34.000000 ocrd_validators-2.9.0/PKG-INFO
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-09 17:33:34.000000 ocrd_validators-2.9.0/ocrd_validators/
+-rw-rw-r--   0 kba       (1000) kba       (1000)     2218 2020-05-12 11:01:01.000000 ocrd_validators-2.9.0/ocrd_validators/json_validator.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     2026 2020-05-12 11:01:01.000000 ocrd_validators-2.9.0/ocrd_validators/report.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)    22815 2020-06-09 13:50:15.000000 ocrd_validators-2.9.0/ocrd_validators/page_validator.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      467 2020-06-09 17:08:17.000000 ocrd_validators-2.9.0/ocrd_validators/xsd_mets_validator.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     2087 2020-06-09 17:08:17.000000 ocrd_validators-2.9.0/ocrd_validators/xsd_validator.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     3663 2020-05-12 11:01:01.000000 ocrd_validators-2.9.0/ocrd_validators/ocrd_zip_validator.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      712 2020-06-09 17:08:17.000000 ocrd_validators-2.9.0/ocrd_validators/__init__.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      548 2020-05-12 11:01:01.000000 ocrd_validators-2.9.0/ocrd_validators/ocrd_tool_validator.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     1405 2020-05-12 11:01:01.000000 ocrd_validators-2.9.0/ocrd_validators/parameter_validator.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      467 2020-06-09 17:08:17.000000 ocrd_validators-2.9.0/ocrd_validators/xsd_page_validator.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      860 2020-06-09 17:08:17.000000 ocrd_validators-2.9.0/ocrd_validators/constants.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)    13452 2020-06-09 17:08:17.000000 ocrd_validators-2.9.0/ocrd_validators/workspace_validator.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)       86 2020-05-12 11:01:01.000000 ocrd_validators-2.9.0/README.md
```

### Comparing `ocrd_validators-2.8.3/setup.py` & `ocrd_validators-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,10 +17,10 @@
     author='Konstantin Baierer',
     author_email='unixprog@gmail.com',
     url='https://github.com/OCR-D/core',
     license='Apache License 2.0',
     install_requires=install_requires,
     packages=['ocrd_validators'],
     include_package_data=True,
-    package_data={'': ['*.yml']},
+    package_data={'': ['*.yml', '*.xsd']},
     keywords=['OCR', 'OCR-D']
 )
```

### Comparing `ocrd_validators-2.8.3/ocrd_validators.egg-info/SOURCES.txt` & `ocrd_validators-2.9.0/ocrd_validators.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -5,12 +5,15 @@
 ocrd_validators/json_validator.py
 ocrd_validators/ocrd_tool_validator.py
 ocrd_validators/ocrd_zip_validator.py
 ocrd_validators/page_validator.py
 ocrd_validators/parameter_validator.py
 ocrd_validators/report.py
 ocrd_validators/workspace_validator.py
+ocrd_validators/xsd_mets_validator.py
+ocrd_validators/xsd_page_validator.py
+ocrd_validators/xsd_validator.py
 ocrd_validators.egg-info/PKG-INFO
 ocrd_validators.egg-info/SOURCES.txt
 ocrd_validators.egg-info/dependency_links.txt
 ocrd_validators.egg-info/requires.txt
 ocrd_validators.egg-info/top_level.txt
```

### Comparing `ocrd_validators-2.8.3/ocrd_validators/json_validator.py` & `ocrd_validators-2.9.0/ocrd_validators/json_validator.py`

 * *Files identical despite different names*

### Comparing `ocrd_validators-2.8.3/ocrd_validators/report.py` & `ocrd_validators-2.9.0/ocrd_validators/report.py`

 * *Files identical despite different names*

### Comparing `ocrd_validators-2.8.3/ocrd_validators/page_validator.py` & `ocrd_validators-2.9.0/ocrd_validators/page_validator.py`

 * *Files identical despite different names*

### Comparing `ocrd_validators-2.8.3/ocrd_validators/ocrd_zip_validator.py` & `ocrd_validators-2.9.0/ocrd_validators/ocrd_zip_validator.py`

 * *Files identical despite different names*

### Comparing `ocrd_validators-2.8.3/ocrd_validators/ocrd_tool_validator.py` & `ocrd_validators-2.9.0/ocrd_validators/ocrd_tool_validator.py`

 * *Files identical despite different names*

### Comparing `ocrd_validators-2.8.3/ocrd_validators/parameter_validator.py` & `ocrd_validators-2.9.0/ocrd_validators/parameter_validator.py`

 * *Files identical despite different names*

### Comparing `ocrd_validators-2.8.3/ocrd_validators/workspace_validator.py` & `ocrd_validators-2.9.0/ocrd_validators/workspace_validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 from ocrd_utils import getLogger, MIMETYPE_PAGE, pushd_popd, is_local_filename
 from ocrd_modelfactory import page_from_file
 
 from .constants import FILE_GROUP_CATEGORIES, FILE_GROUP_PREFIX
 from .report import ValidationReport
 from .page_validator import PageValidator
+from .xsd_page_validator import XsdPageValidator
+from .xsd_mets_validator import XsdMetsValidator
 
 log = getLogger('ocrd.workspace_validator')
 
 #
 # -------------------------------------------------
 #
 
@@ -119,15 +121,19 @@
                     self._validate_multipage()
                 if 'dimension' not in self.skip:
                     self._validate_dimension()
                 if 'imagefilename' not in self.skip:
                     self._validate_imagefilename()
                 if 'page' not in self.skip:
                     self._validate_page()
-            except Exception:
+                if 'page_xsd' not in self.skip:
+                    self._validate_page_xsd()
+                if 'mets_xsd' not in self.skip:
+                    self._validate_mets_xsd()
+            except Exception: # pylint: disable=broad-except
                 self.report.add_error("Validation aborted with exception: %s" % format_exc())
         return self.report
 
     def _resolve_workspace(self):
         """
         Clone workspace from mets_url unless workspace was provided.
         """
@@ -260,7 +266,27 @@
                                                  page_textequiv_consistency=self.page_strictness,
                                                  check_coords=self.page_coordinate_consistency in ['poly', 'both'],
                                                  check_baseline=self.page_coordinate_consistency in ['baseline', 'both'])
             pg = page_from_file(ocrd_file)
             if pg.pcGtsId != ocrd_file.ID:
                 page_report.add_warning('pc:PcGts/@pcGtsId differs from mets:file/@ID: "%s" !== "%s"' % (pg.pcGtsId or '', ocrd_file.ID or ''))
             self.report.merge_report(page_report)
+
+    def _validate_page_xsd(self):
+        """
+        Validate all PAGE-XML files against PAGE XSD schema
+        """
+        log.info("Validating all PAGE-XML files against XSD")
+        for ocrd_file in self.mets.find_files(mimetype=MIMETYPE_PAGE, local_only=True):
+            self.workspace.download_file(ocrd_file)
+            for err in XsdPageValidator.validate(Path(ocrd_file.local_filename)).errors:
+                self.report.add_error("%s: %s" % (ocrd_file.ID, err))
+        log.info("Finished alidating all PAGE-XML files against XSD")
+
+    def _validate_mets_xsd(self):
+        """
+        Validate METS against METS XSD schema
+        """
+        log.info("Validating METS %s against XSD" % self.workspace.mets_target)
+        for err in XsdMetsValidator.validate(Path(self.workspace.mets_target)).errors:
+            self.report.add_error("%s: %s" % (self.workspace.mets_target, err))
+        log.info("Finished Validating METS against XSD")
```

