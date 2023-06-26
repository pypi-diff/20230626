# Comparing `tmp/samna-0.9.38.0-py3-none-any.whl.zip` & `tmp/samna-0.9.39.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1678 bytes, number of entries: 5
--rw-r--r--  2.0 unx      977 b- defN 21-Nov-18 08:24 samna/__init__.py
--rw-r--r--  2.0 unx      227 b- defN 21-Nov-18 08:24 samna-0.9.38.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Nov-18 08:24 samna-0.9.38.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 21-Nov-18 08:24 samna-0.9.38.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      373 b- defN 21-Nov-18 08:24 samna-0.9.38.0.dist-info/RECORD
-5 files, 1675 bytes uncompressed, 978 bytes compressed:  41.6%
+Zip file size: 1675 bytes, number of entries: 5
+-rw-r--r--  2.0 unx      977 b- defN 21-Nov-18 14:48 samna/__init__.py
+-rw-r--r--  2.0 unx      227 b- defN 21-Nov-18 14:48 samna-0.9.39.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Nov-18 14:48 samna-0.9.39.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 21-Nov-18 14:48 samna-0.9.39.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      373 b- defN 21-Nov-18 14:48 samna-0.9.39.0.dist-info/RECORD
+5 files, 1675 bytes uncompressed, 975 bytes compressed:  41.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: samna/__init__.py
 Comment: 
 
-Filename: samna-0.9.38.0.dist-info/METADATA
+Filename: samna-0.9.39.0.dist-info/METADATA
 Comment: 
 
-Filename: samna-0.9.38.0.dist-info/WHEEL
+Filename: samna-0.9.39.0.dist-info/WHEEL
 Comment: 
 
-Filename: samna-0.9.38.0.dist-info/top_level.txt
+Filename: samna-0.9.39.0.dist-info/top_level.txt
 Comment: 
 
-Filename: samna-0.9.38.0.dist-info/RECORD
+Filename: samna-0.9.39.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## samna/__init__.py

```diff
@@ -1,14 +1,14 @@
 import subprocess
 import sys
 
 PYPI_SAMNA = True   # a mark to indicate it's pypi samna
 
 __gitlab_packages_index_url__ = 'https://gitlab.com/api/v4/projects/27423070/packages/pypi/simple'
-__version__ = '0.9.38.0'
+__version__ = '0.9.39.0'
 
 def __install_real_samna__(index_url, version):
     # Currently pypi samna is already installed, so old samna is already uninstalled, We just need to force reinstall samna to use real samna instead of pypi samna.
     subprocess.check_call([sys.executable, "-m", "pip", "install", '--force-reinstall', 'samna==%s' % version, '--index-url=%s' % index_url])
 
 def install_real_samna():
     __install_real_samna__(__gitlab_packages_index_url__, __version__)
```

