# Comparing `tmp/gitlab_arc_fs-0.0.8.dev1.tar.gz` & `tmp/gitlab_arc_fs-0.0.9.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_arc_fs-0.0.8.dev1.tar", last modified: Mon Jun  5 08:34:51 2023, max compression
+gzip compressed data, was "gitlab_arc_fs-0.0.9.dev1.tar", last modified: Mon Jun  5 11:41:23 2023, max compression
```

## Comparing `gitlab_arc_fs-0.0.8.dev1.tar` & `gitlab_arc_fs-0.0.9.dev1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-06-05 08:34:51.879120 gitlab_arc_fs-0.0.8.dev1/
--rw-rw-r--   0 julian    (1000) julian    (1000)      336 2023-06-05 08:34:51.879120 gitlab_arc_fs-0.0.8.dev1/PKG-INFO
--rw-rw-r--   0 julian    (1000) julian    (1000)      185 2023-02-27 10:58:22.000000 gitlab_arc_fs-0.0.8.dev1/README.md
-drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-06-05 08:34:51.879120 gitlab_arc_fs-0.0.8.dev1/gitlab_arc_fs.egg-info/
--rw-rw-r--   0 julian    (1000) julian    (1000)      336 2023-06-05 08:34:51.000000 gitlab_arc_fs-0.0.8.dev1/gitlab_arc_fs.egg-info/PKG-INFO
--rw-rw-r--   0 julian    (1000) julian    (1000)      424 2023-06-05 08:34:51.000000 gitlab_arc_fs-0.0.8.dev1/gitlab_arc_fs.egg-info/SOURCES.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)        1 2023-06-05 08:34:51.000000 gitlab_arc_fs-0.0.8.dev1/gitlab_arc_fs.egg-info/dependency_links.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)       53 2023-06-05 08:34:51.000000 gitlab_arc_fs-0.0.8.dev1/gitlab_arc_fs.egg-info/entry_points.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)       60 2023-06-05 08:34:51.000000 gitlab_arc_fs-0.0.8.dev1/gitlab_arc_fs.egg-info/requires.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)       14 2023-06-05 08:34:51.000000 gitlab_arc_fs-0.0.8.dev1/gitlab_arc_fs.egg-info/top_level.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)       38 2023-06-05 08:34:51.879120 gitlab_arc_fs-0.0.8.dev1/setup.cfg
--rw-rw-r--   0 julian    (1000) julian    (1000)      768 2023-06-05 08:29:53.000000 gitlab_arc_fs-0.0.8.dev1/setup.py
-drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-06-05 08:34:51.879120 gitlab_arc_fs-0.0.8.dev1/src/
-drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-06-05 08:34:51.879120 gitlab_arc_fs-0.0.8.dev1/src/gitlab_arc_fs/
--rw-rw-r--   0 julian    (1000) julian    (1000)       72 2023-05-31 06:59:25.000000 gitlab_arc_fs-0.0.8.dev1/src/gitlab_arc_fs/__init__.py
--rw-rw-r--   0 julian    (1000) julian    (1000)     8611 2023-06-01 11:10:56.000000 gitlab_arc_fs-0.0.8.dev1/src/gitlab_arc_fs/gitlab_filestream.py
--rw-rw-r--   0 julian    (1000) julian    (1000)    28274 2023-06-05 08:10:53.000000 gitlab_arc_fs-0.0.8.dev1/src/gitlab_arc_fs/gitlab_fs.py
--rw-rw-r--   0 julian    (1000) julian    (1000)    11337 2023-06-05 08:08:08.000000 gitlab_arc_fs-0.0.8.dev1/src/gitlab_arc_fs/lfs_file.py
--rw-rw-r--   0 julian    (1000) julian    (1000)     1046 2023-05-31 07:00:16.000000 gitlab_arc_fs-0.0.8.dev1/src/gitlab_arc_fs/opener.py
-drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-06-05 08:34:51.879120 gitlab_arc_fs-0.0.8.dev1/tests/
--rw-rw-r--   0 julian    (1000) julian    (1000)    10257 2023-05-30 12:58:02.000000 gitlab_arc_fs-0.0.8.dev1/tests/test_gitlab_fs.py
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-06-05 11:41:23.387792 gitlab_arc_fs-0.0.9.dev1/
+-rw-rw-r--   0 julian    (1000) julian    (1000)      336 2023-06-05 11:41:23.387792 gitlab_arc_fs-0.0.9.dev1/PKG-INFO
+-rw-rw-r--   0 julian    (1000) julian    (1000)      185 2023-02-27 10:58:22.000000 gitlab_arc_fs-0.0.9.dev1/README.md
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-06-05 11:41:23.387792 gitlab_arc_fs-0.0.9.dev1/gitlab_arc_fs.egg-info/
+-rw-rw-r--   0 julian    (1000) julian    (1000)      336 2023-06-05 11:41:23.000000 gitlab_arc_fs-0.0.9.dev1/gitlab_arc_fs.egg-info/PKG-INFO
+-rw-rw-r--   0 julian    (1000) julian    (1000)      424 2023-06-05 11:41:23.000000 gitlab_arc_fs-0.0.9.dev1/gitlab_arc_fs.egg-info/SOURCES.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)        1 2023-06-05 11:41:23.000000 gitlab_arc_fs-0.0.9.dev1/gitlab_arc_fs.egg-info/dependency_links.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)       53 2023-06-05 11:41:23.000000 gitlab_arc_fs-0.0.9.dev1/gitlab_arc_fs.egg-info/entry_points.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)       60 2023-06-05 11:41:23.000000 gitlab_arc_fs-0.0.9.dev1/gitlab_arc_fs.egg-info/requires.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)       14 2023-06-05 11:41:23.000000 gitlab_arc_fs-0.0.9.dev1/gitlab_arc_fs.egg-info/top_level.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)       38 2023-06-05 11:41:23.391793 gitlab_arc_fs-0.0.9.dev1/setup.cfg
+-rw-rw-r--   0 julian    (1000) julian    (1000)      768 2023-06-05 11:41:03.000000 gitlab_arc_fs-0.0.9.dev1/setup.py
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-06-05 11:41:23.387792 gitlab_arc_fs-0.0.9.dev1/src/
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-06-05 11:41:23.387792 gitlab_arc_fs-0.0.9.dev1/src/gitlab_arc_fs/
+-rw-rw-r--   0 julian    (1000) julian    (1000)       72 2023-05-31 06:59:25.000000 gitlab_arc_fs-0.0.9.dev1/src/gitlab_arc_fs/__init__.py
+-rw-rw-r--   0 julian    (1000) julian    (1000)     8611 2023-06-01 11:10:56.000000 gitlab_arc_fs-0.0.9.dev1/src/gitlab_arc_fs/gitlab_filestream.py
+-rw-rw-r--   0 julian    (1000) julian    (1000)    28602 2023-06-05 11:11:56.000000 gitlab_arc_fs-0.0.9.dev1/src/gitlab_arc_fs/gitlab_fs.py
+-rw-rw-r--   0 julian    (1000) julian    (1000)    11325 2023-06-05 09:56:21.000000 gitlab_arc_fs-0.0.9.dev1/src/gitlab_arc_fs/lfs_file.py
+-rw-rw-r--   0 julian    (1000) julian    (1000)     1046 2023-05-31 07:00:16.000000 gitlab_arc_fs-0.0.9.dev1/src/gitlab_arc_fs/opener.py
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-06-05 11:41:23.387792 gitlab_arc_fs-0.0.9.dev1/tests/
+-rw-rw-r--   0 julian    (1000) julian    (1000)    10257 2023-05-30 12:58:02.000000 gitlab_arc_fs-0.0.9.dev1/tests/test_gitlab_fs.py
```

### Comparing `gitlab_arc_fs-0.0.8.dev1/setup.py` & `gitlab_arc_fs-0.0.9.dev1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,11 +15,11 @@
         'fs.opener': [
             'gitlab = gitlab_fs.opener:GitlabFSOpener',
         ]
     },
     license="MY LICENSE",
     packages=['gitlab_arc_fs'],
     package_dir={'gitlab_arc_fs': 'src/gitlab_arc_fs'},
-    version="0.0.8.dev1",
+    version="0.0.9.dev1",
     url="https://git.bwcloud.uni-freiburg.de/julian.weidhase/GitlabFS",
     python_requires='>=3.8'
 )
```

### Comparing `gitlab_arc_fs-0.0.8.dev1/src/gitlab_arc_fs/gitlab_filestream.py` & `gitlab_arc_fs-0.0.9.dev1/src/gitlab_arc_fs/gitlab_filestream.py`

 * *Files identical despite different names*

### Comparing `gitlab_arc_fs-0.0.8.dev1/src/gitlab_arc_fs/gitlab_fs.py` & `gitlab_arc_fs-0.0.9.dev1/src/gitlab_arc_fs/gitlab_fs.py`

 * *Files 1% similar despite different names*

```diff
@@ -708,15 +708,23 @@
                 (repo_id, repo_path) = self._get_repo_id_path(str(path))
                 r = self.fstream.get_file_stream(path, repo_id, repo_path)
                 return r.raw
             if parsedMode.exclusive or parsedMode.writing or parsedMode.create:
                 repo_id, repo_path = self._get_repo_id_path(str(path))
                 namespace = self._get_namespace(repo_path)
                 path = "/".join(part for part in Path(path).parts[1:])
-                file = LFSFile(path, self.token,
+                path = Path(path)
+                if len(path.suffixes) > 1:
+                    if path.suffixes[0] == path.suffixes[1]:
+                        suffix = path.suffixes[1]
+                        path = Path(path.stem)
+                        path = path.with_suffix(suffix)
+
+                file = LFSFile(str(path),
+                               self.token,
                                self.hostname,
                                namespace,
                                repo_id)
                 return file
             else:
                 raise Unsupported
```

### Comparing `gitlab_arc_fs-0.0.8.dev1/src/gitlab_arc_fs/lfs_file.py` & `gitlab_arc_fs-0.0.9.dev1/src/gitlab_arc_fs/lfs_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
                  repo_id: str,
                  local_path: str = None,
                  ref: str = None):
         """
         Constructor for the LSF file class.
 
         Args:
-            path (str):         The path to the ressource (namespace) on
-                                Gitlab inside a repository.
+            path (str):         The path to the ressource on Gitlab inside a
+                                repository.
             token (str):        A Gitlab access token with the scope "api".
             host (str):         Hostname of the GitLab serer
             namespace (str):    The "path" to the repository on GitLab
             repo_id (str):      The id of the repository on GitLab
             local_path:         Path of a local file to be uploaded.
             (str, optional)     Defaults to None.
             ref:                The commit-sha / branch name / tag of the
```

### Comparing `gitlab_arc_fs-0.0.8.dev1/src/gitlab_arc_fs/opener.py` & `gitlab_arc_fs-0.0.9.dev1/src/gitlab_arc_fs/opener.py`

 * *Files identical despite different names*

### Comparing `gitlab_arc_fs-0.0.8.dev1/tests/test_gitlab_fs.py` & `gitlab_arc_fs-0.0.9.dev1/tests/test_gitlab_fs.py`

 * *Files identical despite different names*

