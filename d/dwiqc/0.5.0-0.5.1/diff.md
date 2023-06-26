# Comparing `tmp/dwiqc-0.5.0-py2.py3-none-any.whl.zip` & `tmp/dwiqc-0.5.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 24749 bytes, number of entries: 22
+Zip file size: 24770 bytes, number of entries: 22
 -rw-r--r--  2.0 unx      225 b- defN 23-Jun-23 17:52 dwiqc/__init__.py
--rw-r--r--  2.0 unx      247 b- defN 23-Jun-26 11:30 dwiqc/__version__.py
+-rw-r--r--  2.0 unx      247 b- defN 23-Jun-26 14:13 dwiqc/__version__.py
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
--rw-r--r--  2.0 unx     6146 b- defN 23-Jun-23 17:52 dwiqc/tasks/qsiprep.py
+-rw-r--r--  2.0 unx     6165 b- defN 23-Jun-26 14:12 dwiqc/tasks/qsiprep.py
 -rw-r--r--  2.0 unx     3872 b- defN 23-Jun-23 17:52 dwiqc/tasks/qsiprep_EQ.py
 -rw-r--r--  2.0 unx    13136 b- defN 23-Jun-23 17:52 dwiqc/xnat/__init__.py
--rwxr-xr-x  2.0 unx     5783 b- defN 23-Jun-26 11:31 dwiqc-0.5.0.data/scripts/dwiQC.py
--rw-r--r--  2.0 unx     1541 b- defN 23-Jun-26 11:31 dwiqc-0.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      482 b- defN 23-Jun-26 11:31 dwiqc-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-26 11:31 dwiqc-0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-26 11:31 dwiqc-0.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1718 b- defN 23-Jun-26 11:31 dwiqc-0.5.0.dist-info/RECORD
-22 files, 69023 bytes uncompressed, 21997 bytes compressed:  68.1%
+-rwxr-xr-x  2.0 unx     5783 b- defN 23-Jun-26 14:15 dwiqc-0.5.1.data/scripts/dwiQC.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-Jun-26 14:15 dwiqc-0.5.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      482 b- defN 23-Jun-26 14:15 dwiqc-0.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-26 14:15 dwiqc-0.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-26 14:15 dwiqc-0.5.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1718 b- defN 23-Jun-26 14:15 dwiqc-0.5.1.dist-info/RECORD
+22 files, 69042 bytes uncompressed, 22018 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -42,26 +42,26 @@
 
 Filename: dwiqc/tasks/qsiprep_EQ.py
 Comment: 
 
 Filename: dwiqc/xnat/__init__.py
 Comment: 
 
-Filename: dwiqc-0.5.0.data/scripts/dwiQC.py
+Filename: dwiqc-0.5.1.data/scripts/dwiQC.py
 Comment: 
 
-Filename: dwiqc-0.5.0.dist-info/LICENSE
+Filename: dwiqc-0.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: dwiqc-0.5.0.dist-info/METADATA
+Filename: dwiqc-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: dwiqc-0.5.0.dist-info/WHEEL
+Filename: dwiqc-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: dwiqc-0.5.0.dist-info/top_level.txt
+Filename: dwiqc-0.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: dwiqc-0.5.0.dist-info/RECORD
+Filename: dwiqc-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dwiqc/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'dwiqc'
 __description__ = 'Quality Assurance Pipeline for Diffusion MR Data'
 __url__ = 'https://github.com/harvard-nrg/dwiqc'
-__version__ = '0.5.0'
+__version__ = '0.5.1'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## dwiqc/tasks/qsiprep.py

```diff
@@ -11,15 +11,15 @@
 import dwiqc.tasks as tasks
 sys.path.insert(0, os.path.join(os.environ['MODULESHOME'], "init"))
 from env_modules_python import module
 import shutil
 from executors.models import Job
 
 
-module('load', 'cuda/9.1.85-fasrc01')
+#module('load', 'cuda/9.1.85-fasrc01')
 
 
 logger = logging.getLogger(__name__)
 
 
 class Task(tasks.BaseTask):
 	def __init__(self, sub, ses, run, bids, outdir, output_resolution=None, tempdir=None, pipenv=None):
@@ -208,17 +208,17 @@
 		self._command = [
 			'selfie',
 			'--lock',
 			'--output-file', self._prov,
 			'singularity',
 			'run',
 			'--nv',
-			'-B',
-			'/n/sw/helmod-rocky8/apps/Core/cuda/9.1.85-fasrc01:/usr/local/cuda',
-			'/n/sw/ncf/apps/qsiprep/0.14.0/qsiprep.sif',			
+			#'-B',
+			#'/n/sw/helmod-rocky8/apps/Core/cuda/9.1.85-fasrc01:/usr/local/cuda',
+			'/n/sw/ncf/containers/hub.docker.io/pennbbl/qsiprep/0.18.0',			
 			self._bids,
 			self._outdir,
 			'participant',
 			'--output-resolution',
 			self._output_resolution,
 			'--separate-all-dwis',
 			'--output-space',
```

## Comparing `dwiqc-0.5.0.data/scripts/dwiQC.py` & `dwiqc-0.5.1.data/scripts/dwiQC.py`

 * *Files identical despite different names*

## Comparing `dwiqc-0.5.0.dist-info/LICENSE` & `dwiqc-0.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dwiqc-0.5.0.dist-info/RECORD` & `dwiqc-0.5.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 dwiqc/__init__.py,sha256=MZJhUZKhHHoZ2w_GeoFCITk1m_0ASdRw_ZaeDixFEPU,225
-dwiqc/__version__.py,sha256=Nsf3nhbOOM-pFa0xu0R8lPEZ3_rp89TauEZ9swKRn4A,247
+dwiqc/__version__.py,sha256=uWpDW7HeYHWfv7hZl66l_tNQnm7sZU0hf4o-E4YpXT8,247
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
-dwiqc/tasks/qsiprep.py,sha256=CWalSV29PeSXhPANLR6MQiH6eAAFaaN6PxDITnTZ3Pw,6146
+dwiqc/tasks/qsiprep.py,sha256=6uxSezp3JGycLVTy-d_UuB9wfIQrihyzikL9_eF0_vw,6165
 dwiqc/tasks/qsiprep_EQ.py,sha256=oj9kJ4hRBlq8mT4Mp-ogakoOTVFbfJ2yUxcwoXPN4j8,3872
 dwiqc/xnat/__init__.py,sha256=mDXbGHAYEuTSe8Dg93ZKzgoYEP3EyfvqCWY8Ai7W1jE,13136
-dwiqc-0.5.0.data/scripts/dwiQC.py,sha256=9FvCPyuitQXOZOjcW3DQcyXL6jJ3-X9J9zxtkTSsYGw,5783
-dwiqc-0.5.0.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-dwiqc-0.5.0.dist-info/METADATA,sha256=W3oYl7THbuIRYsKwrhmOtABkdsX495hcHYDAAp5jAe4,482
-dwiqc-0.5.0.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
-dwiqc-0.5.0.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
-dwiqc-0.5.0.dist-info/RECORD,,
+dwiqc-0.5.1.data/scripts/dwiQC.py,sha256=9FvCPyuitQXOZOjcW3DQcyXL6jJ3-X9J9zxtkTSsYGw,5783
+dwiqc-0.5.1.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+dwiqc-0.5.1.dist-info/METADATA,sha256=wZ_3ahYdghICmr6CWD9txEg-w_Hz4QalHPzi4Y73xLQ,482
+dwiqc-0.5.1.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
+dwiqc-0.5.1.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
+dwiqc-0.5.1.dist-info/RECORD,,
```

