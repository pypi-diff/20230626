# Comparing `tmp/yaxil-0.9.5-py2.py3-none-any.whl.zip` & `tmp/yaxil-0.9.6-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 30391 bytes, number of entries: 19
--rw-r--r--  2.0 unx    46824 b- defN 23-Jun-20 13:33 yaxil/__init__.py
--rw-r--r--  2.0 unx      232 b- defN 23-Jun-20 13:33 yaxil/__version__.py
+Zip file size: 30410 bytes, number of entries: 19
+-rw-r--r--  2.0 unx    46800 b- defN 23-Jun-21 15:18 yaxil/__init__.py
+-rw-r--r--  2.0 unx      232 b- defN 23-Jun-26 17:34 yaxil/__version__.py
 -rw-r--r--  2.0 unx       84 b- defN 23-Jun-08 16:34 yaxil/assessments/__init__.py
 -rw-r--r--  2.0 unx    22420 b- defN 23-Jun-08 16:34 yaxil/assessments/neuroinfo/__init__.py
 -rw-r--r--  2.0 unx     7117 b- defN 23-Jun-08 16:34 yaxil/assessments/neuroinfo/legacy/__init__.py
 -rw-r--r--  2.0 unx      699 b- defN 23-Jun-08 16:34 yaxil/assessments/neuroinfo/session/__init__.py
 -rw-r--r--  2.0 unx    16280 b- defN 23-Jun-08 16:34 yaxil/bids/__init__.py
 -rw-r--r--  2.0 unx     2805 b- defN 23-Jun-08 16:34 yaxil/commons/__init__.py
 -rw-r--r--  2.0 unx     1656 b- defN 23-Jun-08 16:34 yaxil/dicom/__init__.py
 -rw-r--r--  2.0 unx      625 b- defN 23-Jun-08 16:34 yaxil/exceptions/__init__.py
 -rw-r--r--  2.0 unx      783 b- defN 23-Jun-08 16:34 yaxil/functools/__init__.py
 -rw-r--r--  2.0 unx     1477 b- defN 23-Jun-08 16:34 yaxil/session/__init__.py
--rwxr-xr-x  2.0 unx     9426 b- defN 23-Jun-20 13:36 yaxil-0.9.5.data/scripts/ArcGet.py
--rwxr-xr-x  2.0 unx     4114 b- defN 23-Jun-20 13:36 yaxil-0.9.5.data/scripts/xnat_auth
--rw-r--r--  2.0 unx     1541 b- defN 23-Jun-20 13:36 yaxil-0.9.5.dist-info/LICENSE
--rw-r--r--  2.0 unx      387 b- defN 23-Jun-20 13:36 yaxil-0.9.5.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-20 13:36 yaxil-0.9.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-20 13:36 yaxil-0.9.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1586 b- defN 23-Jun-20 13:36 yaxil-0.9.5.dist-info/RECORD
-19 files, 118172 bytes uncompressed, 27795 bytes compressed:  76.5%
+-rwxr-xr-x  2.0 unx     9426 b- defN 23-Jun-26 17:35 yaxil-0.9.6.data/scripts/ArcGet.py
+-rwxr-xr-x  2.0 unx     4114 b- defN 23-Jun-26 17:35 yaxil-0.9.6.data/scripts/xnat_auth
+-rw-r--r--  2.0 unx     1541 b- defN 23-Jun-26 17:35 yaxil-0.9.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx      387 b- defN 23-Jun-26 17:35 yaxil-0.9.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-26 17:35 yaxil-0.9.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-26 17:35 yaxil-0.9.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1586 b- defN 23-Jun-26 17:35 yaxil-0.9.6.dist-info/RECORD
+19 files, 118148 bytes uncompressed, 27814 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -30,29 +30,29 @@
 
 Filename: yaxil/functools/__init__.py
 Comment: 
 
 Filename: yaxil/session/__init__.py
 Comment: 
 
-Filename: yaxil-0.9.5.data/scripts/ArcGet.py
+Filename: yaxil-0.9.6.data/scripts/ArcGet.py
 Comment: 
 
-Filename: yaxil-0.9.5.data/scripts/xnat_auth
+Filename: yaxil-0.9.6.data/scripts/xnat_auth
 Comment: 
 
-Filename: yaxil-0.9.5.dist-info/LICENSE
+Filename: yaxil-0.9.6.dist-info/LICENSE
 Comment: 
 
-Filename: yaxil-0.9.5.dist-info/METADATA
+Filename: yaxil-0.9.6.dist-info/METADATA
 Comment: 
 
-Filename: yaxil-0.9.5.dist-info/WHEEL
+Filename: yaxil-0.9.6.dist-info/WHEEL
 Comment: 
 
-Filename: yaxil-0.9.5.dist-info/top_level.txt
+Filename: yaxil-0.9.6.dist-info/top_level.txt
 Comment: 
 
-Filename: yaxil-0.9.5.dist-info/RECORD
+Filename: yaxil-0.9.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yaxil/__init__.py

```diff
@@ -351,15 +351,16 @@
 Experiment = col.namedtuple('Experiment', [
     'uri',
     'label',
     'id',
     'project',
     'subject_id',
     'subject_label',
-    'archived_date'
+    'archived_date',
+    'note'
 ])
 '''
 Container to hold XNAT Experiment information. Fields include the Experiment URI
 ``uri``, Accession ID ``id``, Project ``project``, Label ``label``, Subject 
 Accession ID ``subject_id``, Subject label ``subject_label``, and archive date 
 ``archived_date``.
 '''
@@ -390,22 +391,22 @@
     :returns: Experiment object
     :rtype: :mod:`yaxil.Experiment`
     '''
     if subject and (label or project):
         raise ValueError('cannot provide subject with label or project')
     url = '{0}/data/experiments'.format(auth.url.rstrip('/'))
     logger.debug('issuing http request %s', url)
-    # compile query string
     columns = [
         'ID',
         'label',
         'project',
         'xnat:subjectassessordata/subject_id',
         'subject_label',
-        'insert_date'
+        'insert_date',
+        'note'
     ]
     payload = {
         'columns': ','.join(columns)
     }
     if label:
         payload['label'] = label
     if project:
@@ -433,21 +434,24 @@
         __quick_validate(results)
     except ResultSetError as e:
         raise ResultSetError('{0} from {1}'.format(e.message, r.url))
     results = results['ResultSet']
     if int(results['totalRecords']) == 0:
         raise NoExperimentsError('no records returned for {0}'.format(r.url))
     for item in results['Result']:
-        yield Experiment(uri=item['URI'],
-                         id=item['ID'],
-                         project=item['project'],
-                         label=item['label'],
-                         subject_id=item['subject_ID'],
-                         subject_label=item['subject_label'],
-                         archived_date=item['insert_date'])
+        yield Experiment(
+            uri=item['URI'],
+            id=item['ID'],
+            project=item['project'],
+            label=item['label'],
+            subject_id=item['subject_ID'],
+            subject_label=item['subject_label'],
+            archived_date=item['insert_date'],
+            note=item['note']
+        )
 
 @functools.lru_cache
 def accession(auth, label, project=None):
     '''
     Get the Accession ID for any Experiment.
 
     Example:
```

## yaxil/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'yaxil'
 __description__ = 'Yet another XNAT interface libary'
 __url__ = 'https://github.com/harvard-nrg/yaxil'
-__version__ = '0.9.5'
+__version__ = '0.9.6'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## Comparing `yaxil-0.9.5.data/scripts/ArcGet.py` & `yaxil-0.9.6.data/scripts/ArcGet.py`

 * *Files identical despite different names*

## Comparing `yaxil-0.9.5.data/scripts/xnat_auth` & `yaxil-0.9.6.data/scripts/xnat_auth`

 * *Files identical despite different names*

## Comparing `yaxil-0.9.5.dist-info/LICENSE` & `yaxil-0.9.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `yaxil-0.9.5.dist-info/RECORD` & `yaxil-0.9.6.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-yaxil/__init__.py,sha256=vsE9OWmDAN--A_L1kI2ItSQtKsIUyALpmSv_RvVzJxE,46824
-yaxil/__version__.py,sha256=2G_ll9DIQ1K74WbORKlDFlfaW9PqcQm9A9wJOQknqm8,232
+yaxil/__init__.py,sha256=ORVt8FrzAKC-vkG6-Nmne_ydZUgjnojDPgoAN3iXHsE,46800
+yaxil/__version__.py,sha256=0zVgEkhBwHX85OKt-YQ8cVmtB--owN0Iedwbh9iBVTc,232
 yaxil/assessments/__init__.py,sha256=TpcTgZ9L8FnHvBOwkeK07BDBnoqqHLV1hVaVG9-yXg8,84
 yaxil/assessments/neuroinfo/__init__.py,sha256=HLA6BTTUeUWDau6k-_yJnM1rDlXHOyTI5cEbACpsGK8,22420
 yaxil/assessments/neuroinfo/legacy/__init__.py,sha256=k7kzdPUCcFDE7CWYzLQj6KkgokcZPiAwa0Pp62-V2fY,7117
 yaxil/assessments/neuroinfo/session/__init__.py,sha256=W3COlgCEoyO0hth3idT1JP7IRhaFmT0CC7lNxVG0uRs,699
 yaxil/bids/__init__.py,sha256=I4VUikLW9gLwfPmEpw4SXJDSa_riBX7IOPryykxOFF8,16280
 yaxil/commons/__init__.py,sha256=lCdwSNdIavfJi5Wux0mZ5Ay_HgKU-FnG-X6vZclDq24,2805
 yaxil/dicom/__init__.py,sha256=hsrcXBZDMBJDrDtaGuVG-T8Btb-EDBSAf5PJbs-qht0,1656
 yaxil/exceptions/__init__.py,sha256=1xNTBxyCkWGevMNBe1kbESSMD5gH06bOG_3XUMYcUHQ,625
 yaxil/functools/__init__.py,sha256=P5yiAU1yotWAFPTi0_rs9SpKTxj1EH9NeBjVMHG3lGs,783
 yaxil/session/__init__.py,sha256=Tr9ALXprn6Xnx6smZHJgOcSBESMkgjB3dSnW_RnrZh8,1477
-yaxil-0.9.5.data/scripts/ArcGet.py,sha256=eNhHHTVeBgkkaZVu1fdLgiJv0ZHSGqNQU9aTRU-hIrU,9426
-yaxil-0.9.5.data/scripts/xnat_auth,sha256=wQ1aNeFxLjtarDu7LqdG-zEepMUShVjw0av_sT8uv3w,4114
-yaxil-0.9.5.dist-info/LICENSE,sha256=OeJg-nLVJUolsCpYxcm6T-P7HHtfoO7kwAC1IoZfjzA,1541
-yaxil-0.9.5.dist-info/METADATA,sha256=rMZ5LIe6gmhFTYyKpa8-habyMDKbI-Ri1sXct9_Z6GQ,387
-yaxil-0.9.5.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-yaxil-0.9.5.dist-info/top_level.txt,sha256=fJsV0xAAilNjfeNRzE2uEHQF-aNZy0K0CH9F6qhCXbU,6
-yaxil-0.9.5.dist-info/RECORD,,
+yaxil-0.9.6.data/scripts/ArcGet.py,sha256=eNhHHTVeBgkkaZVu1fdLgiJv0ZHSGqNQU9aTRU-hIrU,9426
+yaxil-0.9.6.data/scripts/xnat_auth,sha256=wQ1aNeFxLjtarDu7LqdG-zEepMUShVjw0av_sT8uv3w,4114
+yaxil-0.9.6.dist-info/LICENSE,sha256=OeJg-nLVJUolsCpYxcm6T-P7HHtfoO7kwAC1IoZfjzA,1541
+yaxil-0.9.6.dist-info/METADATA,sha256=1DlqDDSElq5h6oqB0WEwS3stiW9Kx8MPuKFq5kLRCJs,387
+yaxil-0.9.6.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+yaxil-0.9.6.dist-info/top_level.txt,sha256=fJsV0xAAilNjfeNRzE2uEHQF-aNZy0K0CH9F6qhCXbU,6
+yaxil-0.9.6.dist-info/RECORD,,
```

