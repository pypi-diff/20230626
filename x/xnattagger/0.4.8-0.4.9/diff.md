# Comparing `tmp/xnattagger-0.4.8-py2.py3-none-any.whl.zip` & `tmp/xnattagger-0.4.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6409 bytes, number of entries: 10
+Zip file size: 6410 bytes, number of entries: 10
 -rw-r--r--  2.0 unx    12743 b- defN 23-Jun-23 16:31 xnattagger/__init__.py
--rw-r--r--  2.0 unx      220 b- defN 23-Jun-23 17:44 xnattagger/__version__.py
+-rw-r--r--  2.0 unx      220 b- defN 23-Jun-23 17:45 xnattagger/__version__.py
 -rw-r--r--  2.0 unx      160 b- defN 23-Jun-23 16:36 xnattagger/config/__init__.py
 -rw-r--r--  2.0 unx     1449 b- defN 23-Jun-23 16:35 xnattagger/config/tagger.yaml
--rwxr-xr-x  2.0 unx     2281 b- defN 23-Jun-23 17:44 xnattagger-0.4.8.data/scripts/xnat_tagger.py
--rw-r--r--  2.0 unx     1541 b- defN 23-Jun-23 17:44 xnattagger-0.4.8.dist-info/LICENSE
--rw-r--r--  2.0 unx      310 b- defN 23-Jun-23 17:44 xnattagger-0.4.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-23 17:44 xnattagger-0.4.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-23 17:44 xnattagger-0.4.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      834 b- defN 23-Jun-23 17:44 xnattagger-0.4.8.dist-info/RECORD
-10 files, 19659 bytes uncompressed, 4981 bytes compressed:  74.7%
+-rwxr-xr-x  2.0 unx     2277 b- defN 23-Jun-23 17:46 xnattagger-0.4.9.data/scripts/xnat_tagger.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-Jun-23 17:46 xnattagger-0.4.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      310 b- defN 23-Jun-23 17:46 xnattagger-0.4.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-23 17:46 xnattagger-0.4.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-23 17:46 xnattagger-0.4.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      834 b- defN 23-Jun-23 17:46 xnattagger-0.4.9.dist-info/RECORD
+10 files, 19655 bytes uncompressed, 4982 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: xnattagger/config/__init__.py
 Comment: 
 
 Filename: xnattagger/config/tagger.yaml
 Comment: 
 
-Filename: xnattagger-0.4.8.data/scripts/xnat_tagger.py
+Filename: xnattagger-0.4.9.data/scripts/xnat_tagger.py
 Comment: 
 
-Filename: xnattagger-0.4.8.dist-info/LICENSE
+Filename: xnattagger-0.4.9.dist-info/LICENSE
 Comment: 
 
-Filename: xnattagger-0.4.8.dist-info/METADATA
+Filename: xnattagger-0.4.9.dist-info/METADATA
 Comment: 
 
-Filename: xnattagger-0.4.8.dist-info/WHEEL
+Filename: xnattagger-0.4.9.dist-info/WHEEL
 Comment: 
 
-Filename: xnattagger-0.4.8.dist-info/top_level.txt
+Filename: xnattagger-0.4.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xnattagger-0.4.8.dist-info/RECORD
+Filename: xnattagger-0.4.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xnattagger/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'xnattagger'
 __description__ = 'XNAT Tagger'
 __url__ = 'https://github.com/harvard-nrg/xnattagger'
-__version__ = '0.4.8'
+__version__ = '0.4.9'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## Comparing `xnattagger-0.4.8.data/scripts/xnat_tagger.py` & `xnattagger-0.4.9.data/scripts/xnat_tagger.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 yaml.add_representer(collections.defaultdict, Representer.represent_dict)
 
 
 def main():
     # Parse command line arguments
     parser = ap.ArgumentParser()
-    parser.add_argument('--xnat-alias', required=True,
+    parser.add_argument('-a', '--alias', required=True,
         help='XNAT alias')  # Set default value and provide help text for alias argument
     parser.add_argument('--project',
         help='XNAT project')  # Provide help text for project argument
     parser.add_argument('-c', '--cache', action='store_true',
         help='Speed up development by caching yaxil.scans output')  # Provide help text for cache argument
     parser.add_argument('-o', '--output-file',
         help='Output summary of updates')  # Provide help text for output-file argument
@@ -44,15 +44,15 @@
     parser.add_argument('--label', required=True,
         help='Label of XNAT MR Session')  # Require label argument
     args = parser.parse_args()
 
     with open(args.filters) as fo:
         filters = yaml.load(fo, Loader=yaml.SafeLoader)
 
-    tagger = Tagger(args.xnat-alias, filters, args.target, args.label)
+    tagger = Tagger(args.alias, filters, args.target, args.label)
     tagger.generate_updates()
 
     if args.output_file:
         with open(args.output_file, 'w') as fo:
             js = json.dumps(tagger.updates, indent=2)
             fo.write(js)
     if not args.dry_run:
```

## Comparing `xnattagger-0.4.8.dist-info/LICENSE` & `xnattagger-0.4.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xnattagger-0.4.8.dist-info/RECORD` & `xnattagger-0.4.9.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 xnattagger/__init__.py,sha256=Sxh2X6lBgvqEcJZx2BVuwW75k-EmXwxYv998zGyVHmA,12743
-xnattagger/__version__.py,sha256=z80lh9a2JYmRfdxVjVt9Zb1P50jzw-TmmiMOe0IAWTc,220
+xnattagger/__version__.py,sha256=ArvAPd-jJhlP-GQCKlW3TCRhwo0ntpfo4qaiPi1NRmE,220
 xnattagger/config/__init__.py,sha256=9NvVYPkoanrrNVRCljmYCAjjJZGq5kvF_oatEgVQDQo,160
 xnattagger/config/tagger.yaml,sha256=pg1jkPEr0wcv0Dz9SzwqCHuC8E_vztjM-OUkd4tt-Mo,1449
-xnattagger-0.4.8.data/scripts/xnat_tagger.py,sha256=iFxK2i4kuUzVe5wBf-aFwDNpI-5UyJ3QGOuYJ7rC-f8,2281
-xnattagger-0.4.8.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-xnattagger-0.4.8.dist-info/METADATA,sha256=NIB7Mzo4AfVfkt_-YrqUtq92eYxruihA0CEhCO14JNo,310
-xnattagger-0.4.8.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
-xnattagger-0.4.8.dist-info/top_level.txt,sha256=LdHhj5smL9uEh9HAguIPB8FH7EgYimhI-AODf4fl6tE,11
-xnattagger-0.4.8.dist-info/RECORD,,
+xnattagger-0.4.9.data/scripts/xnat_tagger.py,sha256=E_DInwnUfIQE5uGWOdWSKn44jSieloh28nq1Kf2jSG0,2277
+xnattagger-0.4.9.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+xnattagger-0.4.9.dist-info/METADATA,sha256=bkEDbd4Otg0HyO2dhXPRCci7LuXLodtU-W4NB7AplR4,310
+xnattagger-0.4.9.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
+xnattagger-0.4.9.dist-info/top_level.txt,sha256=LdHhj5smL9uEh9HAguIPB8FH7EgYimhI-AODf4fl6tE,11
+xnattagger-0.4.9.dist-info/RECORD,,
```

