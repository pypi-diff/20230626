# Comparing `tmp/fme_packager-1.4.3-py3-none-any.whl.zip` & `tmp/fme_packager-1.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 21620 bytes, number of entries: 18
--rw-rw-rw-  2.0 fat       23 b- defN 23-May-12 21:44 fme_packager/__init__.py
+Zip file size: 21642 bytes, number of entries: 18
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-23 23:54 fme_packager/__init__.py
 -rw-rw-rw-  2.0 fat       90 b- defN 22-Nov-29 23:42 fme_packager/__main__.py
 -rw-rw-rw-  2.0 fat     4445 b- defN 23-May-02 17:25 fme_packager/cli.py
 -rw-rw-rw-  2.0 fat      647 b- defN 22-Nov-29 23:42 fme_packager/exception.py
 -rw-rw-rw-  2.0 fat      543 b- defN 22-Nov-29 23:42 fme_packager/fme_env.py
--rw-rw-rw-  2.0 fat     9683 b- defN 23-May-12 21:44 fme_packager/help.py
+-rw-rw-rw-  2.0 fat     9749 b- defN 23-Jun-23 23:55 fme_packager/help.py
 -rw-rw-rw-  2.0 fat     3356 b- defN 22-Nov-29 23:42 fme_packager/metadata.py
 -rw-rw-rw-  2.0 fat     2457 b- defN 23-Jan-31 23:37 fme_packager/operations.py
 -rw-rw-rw-  2.0 fat    22830 b- defN 23-May-12 21:44 fme_packager/packager.py
 -rw-rw-rw-  2.0 fat     4692 b- defN 23-Jan-12 22:04 fme_packager/spec.json
 -rw-rw-rw-  2.0 fat     6158 b- defN 23-Jan-12 22:04 fme_packager/transformer.py
 -rw-rw-rw-  2.0 fat     1796 b- defN 23-May-12 21:44 fme_packager/verifier.py
--rw-rw-rw-  2.0 fat     1307 b- defN 23-May-12 21:50 fme_packager-1.4.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3748 b- defN 23-May-12 21:50 fme_packager-1.4.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-12 21:50 fme_packager-1.4.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       54 b- defN 23-May-12 21:49 fme_packager-1.4.3.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       13 b- defN 23-May-12 21:49 fme_packager-1.4.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1472 b- defN 23-May-12 21:50 fme_packager-1.4.3.dist-info/RECORD
-18 files, 63406 bytes uncompressed, 19208 bytes compressed:  69.7%
+-rw-rw-rw-  2.0 fat     1307 b- defN 23-Jun-23 23:55 fme_packager-1.4.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3748 b- defN 23-Jun-23 23:55 fme_packager-1.4.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-23 23:55 fme_packager-1.4.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       54 b- defN 23-Jun-23 23:55 fme_packager-1.4.4.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Jun-23 23:55 fme_packager-1.4.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1472 b- defN 23-Jun-23 23:55 fme_packager-1.4.4.dist-info/RECORD
+18 files, 63472 bytes uncompressed, 19230 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: fme_packager/transformer.py
 Comment: 
 
 Filename: fme_packager/verifier.py
 Comment: 
 
-Filename: fme_packager-1.4.3.dist-info/LICENSE
+Filename: fme_packager-1.4.4.dist-info/LICENSE
 Comment: 
 
-Filename: fme_packager-1.4.3.dist-info/METADATA
+Filename: fme_packager-1.4.4.dist-info/METADATA
 Comment: 
 
-Filename: fme_packager-1.4.3.dist-info/WHEEL
+Filename: fme_packager-1.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: fme_packager-1.4.3.dist-info/entry_points.txt
+Filename: fme_packager-1.4.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: fme_packager-1.4.3.dist-info/top_level.txt
+Filename: fme_packager-1.4.4.dist-info/top_level.txt
 Comment: 
 
-Filename: fme_packager-1.4.3.dist-info/RECORD
+Filename: fme_packager-1.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fme_packager/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.4.3"
+__version__ = "1.4.4"
```

## fme_packager/help.py

```diff
@@ -116,21 +116,22 @@
     to its corresponding page of documentation.
     The names of the expected HTML files follow a naming convention based on the help context.
     """
     # /foundation/ui/core/include/ui/core/helpkeywords.h
     index = {}
     if not format_directions:
         format_directions = {}
-    # dashes in the UIDs get turned to underscores
-    fpkg_ident = f"{fpkg_metadata.publisher_uid}_{fpkg_metadata.uid}".replace("-", "_")
+    fpkg_ident = f"{fpkg_metadata.publisher_uid}_{fpkg_metadata.uid}"
     # Each transformer has only one topic.
     for xformer in fpkg_metadata.transformers:
         index[f"fmx_{fpkg_ident}_{xformer.name}"] = f"/{xformer.name}.htm"
     # Each format has many topics.
     for fmt in fpkg_metadata.formats:
+        # dashes in the UIDs get turned to underscores when looking for format help
+        fpkg_ident = fpkg_ident.replace("-", "_")
         fmt_ident = f"{fpkg_ident}_{fmt.name}".lower()
         directions = format_directions.get(fmt.name, "rw")
         # Format prefix is "rw" even when read-only or write-only
         index[f"rw_{fmt_ident}_index"] = f"/{fmt.name}.htm"
         index[f"rw_{fmt_ident}_feature_rep"] = f"/{fmt.name}_feature_rep.htm"
         for direction in directions:
             index[f"param_{fmt_ident}_{direction}"] = f"/{fmt.name}_param_{direction}.htm"
```

## Comparing `fme_packager-1.4.3.dist-info/LICENSE` & `fme_packager-1.4.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fme_packager-1.4.3.dist-info/METADATA` & `fme_packager-1.4.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fme-packager
-Version: 1.4.3
+Version: 1.4.4
 Summary: Tool for creating FME Packages.
 Home-page: https://github.com/safesoftware/fme-packager
 Author: Safe Software Inc.
 License: BSD
 Keywords: FME fmeobjects
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

