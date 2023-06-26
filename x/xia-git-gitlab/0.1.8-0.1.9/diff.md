# Comparing `tmp/xia_git_gitlab-0.1.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_git_gitlab-0.1.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 187458 bytes, number of entries: 7
--rw-r--r--  2.0 unx       95 b- defN 23-Jun-25 16:43 xia_git_gitlab/__init__.py
--rw-r--r--  2.0 unx   529408 b- defN 23-Jun-25 16:46 xia_git_gitlab/git.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-25 16:46 xia_git_gitlab-0.1.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      700 b- defN 23-Jun-25 16:46 xia_git_gitlab-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-25 16:46 xia_git_gitlab-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-25 16:46 xia_git_gitlab-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      600 b- defN 23-Jun-25 16:46 xia_git_gitlab-0.1.8.dist-info/RECORD
-7 files, 531068 bytes uncompressed, 186382 bytes compressed:  64.9%
+Zip file size: 187457 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       95 b- defN 23-Jun-25 17:03 xia_git_gitlab/__init__.py
+-rw-r--r--  2.0 unx   529408 b- defN 23-Jun-25 17:07 xia_git_gitlab/git.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-25 17:07 xia_git_gitlab-0.1.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      700 b- defN 23-Jun-25 17:07 xia_git_gitlab-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-25 17:07 xia_git_gitlab-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-25 17:07 xia_git_gitlab-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      600 b- defN 23-Jun-25 17:07 xia_git_gitlab-0.1.9.dist-info/RECORD
+7 files, 531068 bytes uncompressed, 186381 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_git_gitlab/__init__.py
 Comment: 
 
 Filename: xia_git_gitlab/git.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_git_gitlab-0.1.8.dist-info/LICENSE.txt
+Filename: xia_git_gitlab-0.1.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_git_gitlab-0.1.8.dist-info/METADATA
+Filename: xia_git_gitlab-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_git_gitlab-0.1.8.dist-info/WHEEL
+Filename: xia_git_gitlab-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_git_gitlab-0.1.8.dist-info/top_level.txt
+Filename: xia_git_gitlab-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_git_gitlab-0.1.8.dist-info/RECORD
+Filename: xia_git_gitlab-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_git_gitlab/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_git_gitlab.git import GitlabGit
 
 __all__ = [
     "GitlabGit"
 ]
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

## Comparing `xia_git_gitlab-0.1.8.dist-info/METADATA` & `xia_git_gitlab-0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-git-gitlab
-Version: 0.1.8
+Version: 0.1.9
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-git-gitlab/0.1.8/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-git-gitlab/0.1.9/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_git_gitlab-0.1.8.dist-info/RECORD` & `xia_git_gitlab-0.1.9.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_git_gitlab/__init__.py,sha256=n6W-01Rvh0AdraOPXwLrZyV7Ex6sv9ASCTRJGUD6uKo,95
-xia_git_gitlab/git.cp39-win_amd64.pyd,sha256=2a8TtuOj6kqn6DpZmNXl_L300USARSbEfEwzzs9ADH8,529408
-xia_git_gitlab-0.1.8.dist-info/LICENSE.txt,sha256=gNAozHm4-2o3q0DsWBseQDOxAxNL0nSoJBA5UU4udf4,151
-xia_git_gitlab-0.1.8.dist-info/METADATA,sha256=TQ2JIQduYI9c-HbJkuANtOLhT8YJLdcZVIzCCjNX6UA,700
-xia_git_gitlab-0.1.8.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_git_gitlab-0.1.8.dist-info/top_level.txt,sha256=ACmFS4I_hBm4FPQPfnolgaIcTAxtHSabi8tlk73rHDU,15
-xia_git_gitlab-0.1.8.dist-info/RECORD,,
+xia_git_gitlab/__init__.py,sha256=97e7owsjcDWpEUm1ZkBhlMAUTXSeSaffObskIq_zEPk,95
+xia_git_gitlab/git.cp39-win_amd64.pyd,sha256=l9szgPHHH4Io2kJZ2qcJuAaPZBOletbxct_Zuwqqq0E,529408
+xia_git_gitlab-0.1.9.dist-info/LICENSE.txt,sha256=gNAozHm4-2o3q0DsWBseQDOxAxNL0nSoJBA5UU4udf4,151
+xia_git_gitlab-0.1.9.dist-info/METADATA,sha256=62QhMi4N-gNlVXUaZeG_-A9fFrYK5c5DyBM2c18jIKU,700
+xia_git_gitlab-0.1.9.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_git_gitlab-0.1.9.dist-info/top_level.txt,sha256=ACmFS4I_hBm4FPQPfnolgaIcTAxtHSabi8tlk73rHDU,15
+xia_git_gitlab-0.1.9.dist-info/RECORD,,
```

