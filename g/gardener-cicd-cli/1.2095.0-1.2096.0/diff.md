# Comparing `tmp/gardener-cicd-cli-1.2095.0.tar.gz` & `tmp/gardener-cicd-cli-1.2096.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-cli-1.2095.0.tar", last modified: Mon Jun 26 11:36:13 2023, max compression
+gzip compressed data, was "gardener-cicd-cli-1.2096.0.tar", last modified: Mon Jun 26 14:11:37 2023, max compression
```

## Comparing `gardener-cicd-cli-1.2095.0.tar` & `gardener-cicd-cli-1.2096.0.tar`

### file list

```diff
@@ -1,42 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:36:13.358093 gardener-cicd-cli-1.2095.0/
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-26 11:36:13.358093 gardener-cicd-cli-1.2095.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:36:13.354093 gardener-cicd-cli-1.2095.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)    11039 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/bin/component-cli
--rwxr-xr-x   0 root         (0) root         (0)      369 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/bin/helm
--rwxr-xr-x   0 root         (0) root         (0)     5611 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/bin/launch-dockerd.sh
--rwxr-xr-x   0 root         (0) root         (0)     3301 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/bin/purge_history
--rwxr-xr-x   0 root         (0) root         (0)      265 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/bin/yaml2json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:36:13.358093 gardener-cicd-cli-1.2095.0/gardener_ci/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3901 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/_cfg_mgmt.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/_clamav.py
--rw-r--r--   0 root         (0) root         (0)     6463 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/_concourse.py
--rw-r--r--   0 root         (0) root         (0)     8114 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/_oci.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/_osinfo.py
--rw-r--r--   0 root         (0) root         (0)      380 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/_slack.py
--rw-r--r--   0 root         (0) root         (0)    11329 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/bdba.py
--rw-r--r--   0 root         (0) root         (0)     8458 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/cd.py
--rw-r--r--   0 root         (0) root         (0)     1899 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/checkmarx_cli.py
--rwxr-xr-x   0 root         (0) root         (0)     9186 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/cli_gen.py
--rw-r--r--   0 root         (0) root         (0)     8141 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/compliance.py
--rw-r--r--   0 root         (0) root         (0)     3188 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/config.py
--rw-r--r--   0 root         (0) root         (0)      401 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/containerutil.py
--rw-r--r--   0 root         (0) root         (0)      886 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/docker.py
--rw-r--r--   0 root         (0) root         (0)     2415 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/elastic.py
--rw-r--r--   0 root         (0) root         (0)     3512 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/gh.py
--rw-r--r--   0 root         (0) root         (0)     4935 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/githubutil.py
--rw-r--r--   0 root         (0) root         (0)     3128 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/ocm.py
--rw-r--r--   0 root         (0) root         (0)    12219 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     2984 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/productutil_v2.py
--rw-r--r--   0 root         (0) root         (0)     2864 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/whdutil.py
--rwxr-xr-x   0 root         (0) root         (0)      265 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/gardener_ci/yaml2json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:36:13.358093 gardener-cicd-cli-1.2095.0/gardener_cicd_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-26 11:36:13.000000 gardener-cicd-cli-1.2095.0/gardener_cicd_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-26 11:36:13.000000 gardener-cicd-cli-1.2095.0/gardener_cicd_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 11:36:13.000000 gardener-cicd-cli-1.2095.0/gardener_cicd_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      130 2023-06-26 11:36:13.000000 gardener-cicd-cli-1.2095.0/gardener_cicd_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-26 11:36:13.000000 gardener-cicd-cli-1.2095.0/gardener_cicd_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-26 11:36:13.000000 gardener-cicd-cli-1.2095.0/gardener_cicd_cli.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 11:36:13.358093 gardener-cicd-cli-1.2095.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1514 2023-06-26 11:35:13.000000 gardener-cicd-cli-1.2095.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:11:37.406738 gardener-cicd-cli-1.2096.0/
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-26 14:11:37.406738 gardener-cicd-cli-1.2096.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:11:37.402738 gardener-cicd-cli-1.2096.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)    11039 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/bin/component-cli
+-rwxr-xr-x   0 root         (0) root         (0)      369 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/bin/helm
+-rwxr-xr-x   0 root         (0) root         (0)     5611 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/bin/launch-dockerd.sh
+-rwxr-xr-x   0 root         (0) root         (0)     3301 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/bin/purge_history
+-rwxr-xr-x   0 root         (0) root         (0)      265 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/bin/yaml2json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:11:37.402738 gardener-cicd-cli-1.2096.0/gardener_ci/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/gardener_ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3901 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/gardener_ci/_cfg_mgmt.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/gardener_ci/_clamav.py
+-rw-r--r--   0 root         (0) root         (0)     6463 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/gardener_ci/_concourse.py
+-rw-r--r--   0 root         (0) root         (0)     8114 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/gardener_ci/_oci.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/gardener_ci/_osinfo.py
+-rw-r--r--   0 root         (0) root         (0)      380 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/gardener_ci/_slack.py
+-rw-r--r--   0 root         (0) root         (0)    11329 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/gardener_ci/bdba.py
+-rw-r--r--   0 root         (0) root         (0)     8458 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/gardener_ci/cd.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/gardener_ci/checkmarx_cli.py
+-rwxr-xr-x   0 root         (0) root         (0)     9186 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/gardener_ci/cli_gen.py
+-rw-r--r--   0 root         (0) root         (0)     8141 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/gardener_ci/compliance.py
+-rw-r--r--   0 root         (0) root         (0)     3188 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/gardener_ci/config.py
+-rw-r--r--   0 root         (0) root         (0)      401 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/gardener_ci/containerutil.py
+-rw-r--r--   0 root         (0) root         (0)      886 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/gardener_ci/docker.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/gardener_ci/elastic.py
+-rw-r--r--   0 root         (0) root         (0)     3512 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/gardener_ci/gh.py
+-rw-r--r--   0 root         (0) root         (0)     4935 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/gardener_ci/githubutil.py
+-rw-r--r--   0 root         (0) root         (0)     3128 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/gardener_ci/ocm.py
+-rw-r--r--   0 root         (0) root         (0)    12219 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/gardener_ci/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     2984 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/gardener_ci/productutil_v2.py
+-rwxr-xr-x   0 root         (0) root         (0)      265 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/gardener_ci/yaml2json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:11:37.402738 gardener-cicd-cli-1.2096.0/gardener_cicd_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-26 14:11:37.000000 gardener-cicd-cli-1.2096.0/gardener_cicd_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      937 2023-06-26 14:11:37.000000 gardener-cicd-cli-1.2096.0/gardener_cicd_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 14:11:37.000000 gardener-cicd-cli-1.2096.0/gardener_cicd_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2023-06-26 14:11:37.000000 gardener-cicd-cli-1.2096.0/gardener_cicd_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-26 14:11:37.000000 gardener-cicd-cli-1.2096.0/gardener_cicd_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-26 14:11:37.000000 gardener-cicd-cli-1.2096.0/gardener_cicd_cli.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 14:11:37.406738 gardener-cicd-cli-1.2096.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1514 2023-06-26 14:06:25.000000 gardener-cicd-cli-1.2096.0/setup.py
```

### Comparing `gardener-cicd-cli-1.2095.0/bin/component-cli` & `gardener-cicd-cli-1.2096.0/bin/component-cli`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2095.0/bin/launch-dockerd.sh` & `gardener-cicd-cli-1.2096.0/bin/launch-dockerd.sh`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2095.0/bin/purge_history` & `gardener-cicd-cli-1.2096.0/bin/purge_history`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2095.0/gardener_ci/_cfg_mgmt.py` & `gardener-cicd-cli-1.2096.0/gardener_ci/_cfg_mgmt.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2095.0/gardener_ci/_clamav.py` & `gardener-cicd-cli-1.2096.0/gardener_ci/_clamav.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2095.0/gardener_ci/_concourse.py` & `gardener-cicd-cli-1.2096.0/gardener_ci/_concourse.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2095.0/gardener_ci/_oci.py` & `gardener-cicd-cli-1.2096.0/gardener_ci/_oci.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2095.0/gardener_ci/_osinfo.py` & `gardener-cicd-cli-1.2096.0/gardener_ci/_osinfo.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2095.0/gardener_ci/bdba.py` & `gardener-cicd-cli-1.2096.0/gardener_ci/bdba.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2095.0/gardener_ci/cd.py` & `gardener-cicd-cli-1.2096.0/gardener_ci/cd.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2095.0/gardener_ci/checkmarx_cli.py` & `gardener-cicd-cli-1.2096.0/gardener_ci/checkmarx_cli.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2095.0/gardener_ci/cli_gen.py` & `gardener-cicd-cli-1.2096.0/gardener_ci/cli_gen.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2095.0/gardener_ci/compliance.py` & `gardener-cicd-cli-1.2096.0/gardener_ci/compliance.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2095.0/gardener_ci/config.py` & `gardener-cicd-cli-1.2096.0/gardener_ci/config.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2095.0/gardener_ci/docker.py` & `gardener-cicd-cli-1.2096.0/gardener_ci/docker.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2095.0/gardener_ci/elastic.py` & `gardener-cicd-cli-1.2096.0/gardener_ci/elastic.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2095.0/gardener_ci/gh.py` & `gardener-cicd-cli-1.2096.0/gardener_ci/gh.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2095.0/gardener_ci/githubutil.py` & `gardener-cicd-cli-1.2096.0/gardener_ci/githubutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2095.0/gardener_ci/ocm.py` & `gardener-cicd-cli-1.2096.0/gardener_ci/ocm.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2095.0/gardener_ci/pipeline.py` & `gardener-cicd-cli-1.2096.0/gardener_ci/pipeline.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2095.0/gardener_ci/productutil_v2.py` & `gardener-cicd-cli-1.2096.0/gardener_ci/productutil_v2.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2095.0/gardener_cicd_cli.egg-info/SOURCES.txt` & `gardener-cicd-cli-1.2096.0/gardener_cicd_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 gardener_ci/docker.py
 gardener_ci/elastic.py
 gardener_ci/gh.py
 gardener_ci/githubutil.py
 gardener_ci/ocm.py
 gardener_ci/pipeline.py
 gardener_ci/productutil_v2.py
-gardener_ci/whdutil.py
 gardener_ci/yaml2json.py
 gardener_cicd_cli.egg-info/PKG-INFO
 gardener_cicd_cli.egg-info/SOURCES.txt
 gardener_cicd_cli.egg-info/dependency_links.txt
 gardener_cicd_cli.egg-info/entry_points.txt
 gardener_cicd_cli.egg-info/requires.txt
 gardener_cicd_cli.egg-info/top_level.txt
```

### Comparing `gardener-cicd-cli-1.2095.0/setup.py` & `gardener-cicd-cli-1.2096.0/setup.py`

 * *Files identical despite different names*

