# Comparing `tmp/dwiqc-0.4.8-py2.py3-none-any.whl.zip` & `tmp/dwiqc-0.4.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 24517 bytes, number of entries: 22
+Zip file size: 24515 bytes, number of entries: 22
 -rw-r--r--  2.0 unx      225 b- defN 23-Jun-08 18:05 dwiqc/__init__.py
--rw-r--r--  2.0 unx      247 b- defN 23-Jun-21 14:51 dwiqc/__version__.py
+-rw-r--r--  2.0 unx      247 b- defN 23-Jun-21 14:55 dwiqc/__version__.py
 -rw-r--r--  2.0 unx     1352 b- defN 23-Jun-08 18:05 dwiqc/browser/__init__.py
 -rw-r--r--  2.0 unx       61 b- defN 23-Jun-12 14:27 dwiqc/cli/__init__.py
 -rw-r--r--  2.0 unx     6651 b- defN 23-Jun-08 18:05 dwiqc/cli/get.py
 -rw-r--r--  2.0 unx     6025 b- defN 23-Jun-21 14:48 dwiqc/cli/process.py
 -rw-r--r--  2.0 unx     3801 b- defN 23-Jun-12 20:46 dwiqc/cli/tandem.py
 -rw-r--r--  2.0 unx      160 b- defN 23-Jun-08 18:05 dwiqc/config/__init__.py
 -rw-r--r--  2.0 unx      274 b- defN 23-Jun-08 18:05 dwiqc/config/dwiqc.yaml
 -rw-r--r--  2.0 unx       98 b- defN 23-Jun-08 18:05 dwiqc/state/__init__.py
 -rw-r--r--  2.0 unx     1892 b- defN 23-Jun-08 18:05 dwiqc/tasks/__init__.py
--rw-r--r--  2.0 unx    10122 b- defN 23-Jun-21 14:50 dwiqc/tasks/prequal.py
+-rw-r--r--  2.0 unx    10118 b- defN 23-Jun-21 14:54 dwiqc/tasks/prequal.py
 -rw-r--r--  2.0 unx     4656 b- defN 23-Jun-21 11:45 dwiqc/tasks/prequal_EQ.py
 -rw-r--r--  2.0 unx     6146 b- defN 23-Jun-08 18:05 dwiqc/tasks/qsiprep.py
 -rw-r--r--  2.0 unx     3872 b- defN 23-Jun-08 18:05 dwiqc/tasks/qsiprep_EQ.py
 -rw-r--r--  2.0 unx    13083 b- defN 23-Jun-08 18:05 dwiqc/xnat/__init__.py
--rwxr-xr-x  2.0 unx     5783 b- defN 23-Jun-21 14:52 dwiqc-0.4.8.data/scripts/dwiQC.py
--rw-r--r--  2.0 unx     1541 b- defN 23-Jun-21 14:52 dwiqc-0.4.8.dist-info/LICENSE
--rw-r--r--  2.0 unx      428 b- defN 23-Jun-21 14:52 dwiqc-0.4.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-21 14:52 dwiqc-0.4.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-21 14:52 dwiqc-0.4.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1718 b- defN 23-Jun-21 14:52 dwiqc-0.4.8.dist-info/RECORD
-22 files, 68251 bytes uncompressed, 21765 bytes compressed:  68.1%
+-rwxr-xr-x  2.0 unx     5783 b- defN 23-Jun-21 14:56 dwiqc-0.4.9.data/scripts/dwiQC.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-Jun-21 14:56 dwiqc-0.4.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      428 b- defN 23-Jun-21 14:56 dwiqc-0.4.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-21 14:56 dwiqc-0.4.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-21 14:56 dwiqc-0.4.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1718 b- defN 23-Jun-21 14:56 dwiqc-0.4.9.dist-info/RECORD
+22 files, 68247 bytes uncompressed, 21763 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -42,26 +42,26 @@
 
 Filename: dwiqc/tasks/qsiprep_EQ.py
 Comment: 
 
 Filename: dwiqc/xnat/__init__.py
 Comment: 
 
-Filename: dwiqc-0.4.8.data/scripts/dwiQC.py
+Filename: dwiqc-0.4.9.data/scripts/dwiQC.py
 Comment: 
 
-Filename: dwiqc-0.4.8.dist-info/LICENSE
+Filename: dwiqc-0.4.9.dist-info/LICENSE
 Comment: 
 
-Filename: dwiqc-0.4.8.dist-info/METADATA
+Filename: dwiqc-0.4.9.dist-info/METADATA
 Comment: 
 
-Filename: dwiqc-0.4.8.dist-info/WHEEL
+Filename: dwiqc-0.4.9.dist-info/WHEEL
 Comment: 
 
-Filename: dwiqc-0.4.8.dist-info/top_level.txt
+Filename: dwiqc-0.4.9.dist-info/top_level.txt
 Comment: 
 
-Filename: dwiqc-0.4.8.dist-info/RECORD
+Filename: dwiqc-0.4.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dwiqc/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'dwiqc'
 __description__ = 'Quality Assurance Pipeline for Diffusion MR Data'
 __url__ = 'https://github.com/harvard-nrg/dwiqc'
-__version__ = '0.4.8'
+__version__ = '0.4.9'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## dwiqc/tasks/prequal.py

```diff
@@ -32,15 +32,15 @@
 
 
 	# create an INPUTS dir next to the OUTPUTS dir
 	def copy_inputs(self, inputs_dir):
 		try:
 			os.makedirs(inputs_dir)
 		except FileExistsError:
-			continue
+			pass
 		#layout = BIDSLayout(self._bids) # load the data layout into pybids
 		all_files = self._layout.get(subject=self._sub, session=self._ses, run=self._run, return_type='filename') # get a list of all of the subject's files
 		# copy the all the subject's files into the INPUTS directory
 		for file in all_files:
 			basename = os.path.basename(file)
 			dest = os.path.join(inputs_dir, basename)
 			shutil.copy(file, dest)
```

## Comparing `dwiqc-0.4.8.data/scripts/dwiQC.py` & `dwiqc-0.4.9.data/scripts/dwiQC.py`

 * *Files identical despite different names*

## Comparing `dwiqc-0.4.8.dist-info/LICENSE` & `dwiqc-0.4.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dwiqc-0.4.8.dist-info/RECORD` & `dwiqc-0.4.9.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 dwiqc/__init__.py,sha256=MZJhUZKhHHoZ2w_GeoFCITk1m_0ASdRw_ZaeDixFEPU,225
-dwiqc/__version__.py,sha256=o-AM8zf4vhDFL54wcpTLLnVV9u2misZtwHqZZZlXYoM,247
+dwiqc/__version__.py,sha256=smBhAYAIcHmPC7g6Fv7CwwrQEPqq3T7cs1osfl48p0A,247
 dwiqc/browser/__init__.py,sha256=4lK-1-VH4l6ppP_5Ju6MeYIctiQmFQfGA7gclqh8euE,1352
 dwiqc/cli/__init__.py,sha256=1Y4dYEbkHH-jZ3cwbFnlb6TthH_K0t4xT_-IphRBu6k,61
 dwiqc/cli/get.py,sha256=6ixaBdwEgY_GXh8L-_3QDY4MEsNqSJgXle_mxW99mlk,6651
 dwiqc/cli/process.py,sha256=CA2ythc83HISu41bpmWuf4cCr71ljlZHv_zkyy9cTB0,6025
 dwiqc/cli/tandem.py,sha256=aB2uJN6X6aJWXT_JtL6U_Lj7ljItplFU8sVFnfpmrfA,3801
 dwiqc/config/__init__.py,sha256=k_w5JzoJN_7R7eI_sIJxHA4FQQHs0_KGf-6jsbG4Xs8,160
 dwiqc/config/dwiqc.yaml,sha256=x8gKMFZyChdzvNX3GthRe0eWvyKDDL5itXo0kLWVfd0,274
 dwiqc/state/__init__.py,sha256=NaRifw26bI3F1J9BqeLa-KLSzEPq2m_UNhMbXdmPdh4,98
 dwiqc/tasks/__init__.py,sha256=LnlN7iYjpqiBic2ihFrM-_h7m8FD_N7Beh7UIwKyGZ8,1892
-dwiqc/tasks/prequal.py,sha256=BF7xc6qb6TCApJuaSco6iJ0O2mOzMquegTS5r0LBnOo,10122
+dwiqc/tasks/prequal.py,sha256=WhQqExvDHEpUENseNLL2QHGfsJ9mjtufLU7QhiCGGl4,10118
 dwiqc/tasks/prequal_EQ.py,sha256=hvs6qjRNoJXuCzdvP-9BnaZc4xwvI9LHSgmueRobt1Q,4656
 dwiqc/tasks/qsiprep.py,sha256=CWalSV29PeSXhPANLR6MQiH6eAAFaaN6PxDITnTZ3Pw,6146
 dwiqc/tasks/qsiprep_EQ.py,sha256=oj9kJ4hRBlq8mT4Mp-ogakoOTVFbfJ2yUxcwoXPN4j8,3872
 dwiqc/xnat/__init__.py,sha256=HDjDNAQVSzr_e_ySPF_0vGHE5GjIWKXO7bv8ka4whm4,13083
-dwiqc-0.4.8.data/scripts/dwiQC.py,sha256=9FvCPyuitQXOZOjcW3DQcyXL6jJ3-X9J9zxtkTSsYGw,5783
-dwiqc-0.4.8.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-dwiqc-0.4.8.dist-info/METADATA,sha256=F_tmjM2Nk5RGugtMFDVmHR8dgB8eMbLqlXUj8FUNoAw,428
-dwiqc-0.4.8.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-dwiqc-0.4.8.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
-dwiqc-0.4.8.dist-info/RECORD,,
+dwiqc-0.4.9.data/scripts/dwiQC.py,sha256=9FvCPyuitQXOZOjcW3DQcyXL6jJ3-X9J9zxtkTSsYGw,5783
+dwiqc-0.4.9.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+dwiqc-0.4.9.dist-info/METADATA,sha256=WiIlKJWOS2v5R4VTwk88xBlvLkKd5niwctpja9qdiao,428
+dwiqc-0.4.9.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+dwiqc-0.4.9.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
+dwiqc-0.4.9.dist-info/RECORD,,
```

