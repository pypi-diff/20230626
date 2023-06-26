# Comparing `tmp/dwiqc-0.5.2-py2.py3-none-any.whl.zip` & `tmp/dwiqc-0.5.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 24773 bytes, number of entries: 22
+Zip file size: 24771 bytes, number of entries: 22
 -rw-r--r--  2.0 unx      225 b- defN 23-Jun-23 17:52 dwiqc/__init__.py
--rw-r--r--  2.0 unx      247 b- defN 23-Jun-26 14:27 dwiqc/__version__.py
+-rw-r--r--  2.0 unx      247 b- defN 23-Jun-26 14:46 dwiqc/__version__.py
 -rw-r--r--  2.0 unx     1352 b- defN 23-Jun-23 17:52 dwiqc/browser/__init__.py
 -rw-r--r--  2.0 unx       61 b- defN 23-Jun-23 17:52 dwiqc/cli/__init__.py
 -rw-r--r--  2.0 unx     6941 b- defN 23-Jun-26 11:29 dwiqc/cli/get.py
 -rw-r--r--  2.0 unx     6025 b- defN 23-Jun-23 17:52 dwiqc/cli/process.py
 -rw-r--r--  2.0 unx     4180 b- defN 23-Jun-26 11:29 dwiqc/cli/tandem.py
 -rw-r--r--  2.0 unx      160 b- defN 23-Jun-23 17:52 dwiqc/config/__init__.py
 -rw-r--r--  2.0 unx      274 b- defN 23-Jun-23 17:52 dwiqc/config/dwiqc.yaml
 -rw-r--r--  2.0 unx       98 b- defN 23-Jun-23 17:52 dwiqc/state/__init__.py
 -rw-r--r--  2.0 unx     1892 b- defN 23-Jun-23 17:52 dwiqc/tasks/__init__.py
 -rw-r--r--  2.0 unx    10118 b- defN 23-Jun-23 17:52 dwiqc/tasks/prequal.py
 -rw-r--r--  2.0 unx     4656 b- defN 23-Jun-23 17:52 dwiqc/tasks/prequal_EQ.py
 -rw-r--r--  2.0 unx     6165 b- defN 23-Jun-26 14:12 dwiqc/tasks/qsiprep.py
 -rw-r--r--  2.0 unx     3872 b- defN 23-Jun-23 17:52 dwiqc/tasks/qsiprep_EQ.py
 -rw-r--r--  2.0 unx    13136 b- defN 23-Jun-23 17:52 dwiqc/xnat/__init__.py
--rwxr-xr-x  2.0 unx     5783 b- defN 23-Jun-26 14:27 dwiqc-0.5.2.data/scripts/dwiQC.py
--rw-r--r--  2.0 unx     1541 b- defN 23-Jun-26 14:27 dwiqc-0.5.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      483 b- defN 23-Jun-26 14:27 dwiqc-0.5.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-26 14:27 dwiqc-0.5.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-26 14:27 dwiqc-0.5.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1718 b- defN 23-Jun-26 14:27 dwiqc-0.5.2.dist-info/RECORD
-22 files, 69043 bytes uncompressed, 22021 bytes compressed:  68.1%
+-rwxr-xr-x  2.0 unx     5783 b- defN 23-Jun-26 14:46 dwiqc-0.5.3.data/scripts/dwiQC.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-Jun-26 14:46 dwiqc-0.5.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      483 b- defN 23-Jun-26 14:46 dwiqc-0.5.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-26 14:46 dwiqc-0.5.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-26 14:46 dwiqc-0.5.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1718 b- defN 23-Jun-26 14:46 dwiqc-0.5.3.dist-info/RECORD
+22 files, 69043 bytes uncompressed, 22019 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -42,26 +42,26 @@
 
 Filename: dwiqc/tasks/qsiprep_EQ.py
 Comment: 
 
 Filename: dwiqc/xnat/__init__.py
 Comment: 
 
-Filename: dwiqc-0.5.2.data/scripts/dwiQC.py
+Filename: dwiqc-0.5.3.data/scripts/dwiQC.py
 Comment: 
 
-Filename: dwiqc-0.5.2.dist-info/LICENSE
+Filename: dwiqc-0.5.3.dist-info/LICENSE
 Comment: 
 
-Filename: dwiqc-0.5.2.dist-info/METADATA
+Filename: dwiqc-0.5.3.dist-info/METADATA
 Comment: 
 
-Filename: dwiqc-0.5.2.dist-info/WHEEL
+Filename: dwiqc-0.5.3.dist-info/WHEEL
 Comment: 
 
-Filename: dwiqc-0.5.2.dist-info/top_level.txt
+Filename: dwiqc-0.5.3.dist-info/top_level.txt
 Comment: 
 
-Filename: dwiqc-0.5.2.dist-info/RECORD
+Filename: dwiqc-0.5.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dwiqc/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'dwiqc'
 __description__ = 'Quality Assurance Pipeline for Diffusion MR Data'
 __url__ = 'https://github.com/harvard-nrg/dwiqc'
-__version__ = '0.5.2'
+__version__ = '0.5.3'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## Comparing `dwiqc-0.5.2.data/scripts/dwiQC.py` & `dwiqc-0.5.3.data/scripts/dwiQC.py`

 * *Files identical despite different names*

## Comparing `dwiqc-0.5.2.dist-info/LICENSE` & `dwiqc-0.5.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dwiqc-0.5.2.dist-info/RECORD` & `dwiqc-0.5.3.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 dwiqc/__init__.py,sha256=MZJhUZKhHHoZ2w_GeoFCITk1m_0ASdRw_ZaeDixFEPU,225
-dwiqc/__version__.py,sha256=HDDxuQ3kSNfpMpSHk9MvcRpvUVHQEZKkyvqP7x5dr_I,247
+dwiqc/__version__.py,sha256=n3RC7ktU4keK3BcfaVFnbsra2ftil5tzMOxUHpgdAz4,247
 dwiqc/browser/__init__.py,sha256=4lK-1-VH4l6ppP_5Ju6MeYIctiQmFQfGA7gclqh8euE,1352
 dwiqc/cli/__init__.py,sha256=1Y4dYEbkHH-jZ3cwbFnlb6TthH_K0t4xT_-IphRBu6k,61
 dwiqc/cli/get.py,sha256=w2jLbFA7unwfZ-DghKG-_3vPb1RhZPAYX-nXOEbC8wk,6941
 dwiqc/cli/process.py,sha256=CA2ythc83HISu41bpmWuf4cCr71ljlZHv_zkyy9cTB0,6025
 dwiqc/cli/tandem.py,sha256=18t_cn0VrXeAhohg8ukBnDydsR8ZiB8vM0_AZI1Ohkg,4180
 dwiqc/config/__init__.py,sha256=k_w5JzoJN_7R7eI_sIJxHA4FQQHs0_KGf-6jsbG4Xs8,160
 dwiqc/config/dwiqc.yaml,sha256=x8gKMFZyChdzvNX3GthRe0eWvyKDDL5itXo0kLWVfd0,274
 dwiqc/state/__init__.py,sha256=NaRifw26bI3F1J9BqeLa-KLSzEPq2m_UNhMbXdmPdh4,98
 dwiqc/tasks/__init__.py,sha256=LnlN7iYjpqiBic2ihFrM-_h7m8FD_N7Beh7UIwKyGZ8,1892
 dwiqc/tasks/prequal.py,sha256=WhQqExvDHEpUENseNLL2QHGfsJ9mjtufLU7QhiCGGl4,10118
 dwiqc/tasks/prequal_EQ.py,sha256=hvs6qjRNoJXuCzdvP-9BnaZc4xwvI9LHSgmueRobt1Q,4656
 dwiqc/tasks/qsiprep.py,sha256=6uxSezp3JGycLVTy-d_UuB9wfIQrihyzikL9_eF0_vw,6165
 dwiqc/tasks/qsiprep_EQ.py,sha256=oj9kJ4hRBlq8mT4Mp-ogakoOTVFbfJ2yUxcwoXPN4j8,3872
 dwiqc/xnat/__init__.py,sha256=mDXbGHAYEuTSe8Dg93ZKzgoYEP3EyfvqCWY8Ai7W1jE,13136
-dwiqc-0.5.2.data/scripts/dwiQC.py,sha256=9FvCPyuitQXOZOjcW3DQcyXL6jJ3-X9J9zxtkTSsYGw,5783
-dwiqc-0.5.2.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-dwiqc-0.5.2.dist-info/METADATA,sha256=2-hrOWGQyC6DI0HikQIf3b87USA3NJvEiUNMQfgFOj0,483
-dwiqc-0.5.2.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
-dwiqc-0.5.2.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
-dwiqc-0.5.2.dist-info/RECORD,,
+dwiqc-0.5.3.data/scripts/dwiQC.py,sha256=9FvCPyuitQXOZOjcW3DQcyXL6jJ3-X9J9zxtkTSsYGw,5783
+dwiqc-0.5.3.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+dwiqc-0.5.3.dist-info/METADATA,sha256=Rc9bSo_F9GFiNCkTdbkabOvQDqnOr5WLZmdXpK1Gb40,483
+dwiqc-0.5.3.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
+dwiqc-0.5.3.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
+dwiqc-0.5.3.dist-info/RECORD,,
```

