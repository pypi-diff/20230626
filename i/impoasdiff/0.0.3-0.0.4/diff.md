# Comparing `tmp/impoasdiff-0.0.3.tar.gz` & `tmp/impoasdiff-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impoasdiff-0.0.3.tar", last modified: Thu Jun 22 06:11:56 2023, max compression
+gzip compressed data, was "impoasdiff-0.0.4.tar", last modified: Mon Jun 26 18:02:54 2023, max compression
```

## Comparing `impoasdiff-0.0.3.tar` & `impoasdiff-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-22 06:11:56.050035 impoasdiff-0.0.3/
--rw-r--r--   0 yash.thadani   (503) staff       (20)      701 2023-06-22 06:11:56.049832 impoasdiff-0.0.3/PKG-INFO
--rw-r--r--   0 yash.thadani   (503) staff       (20)      402 2023-06-22 06:11:47.000000 impoasdiff-0.0.3/README.md
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-22 06:11:56.046716 impoasdiff-0.0.3/impoasdiff/
--rw-r--r--   0 yash.thadani   (503) staff       (20)      489 2023-06-21 19:42:52.000000 impoasdiff-0.0.3/impoasdiff/__init__.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)      253 2023-06-21 19:34:04.000000 impoasdiff-0.0.3/impoasdiff/_version.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)      522 2023-06-21 18:05:33.000000 impoasdiff-0.0.3/impoasdiff/args_manager.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)    17977 2023-06-21 18:05:33.000000 impoasdiff-0.0.3/impoasdiff/diff_handler.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)     1218 2023-06-21 18:05:33.000000 impoasdiff-0.0.3/impoasdiff/file_handler.py
--rw-r--r--   0 yash.thadani   (503) staff       (20)     4777 2023-06-21 20:27:53.000000 impoasdiff-0.0.3/impoasdiff/generate_diff.py
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-22 06:11:56.049516 impoasdiff-0.0.3/impoasdiff/templates/
--rw-r--r--   0 yash.thadani   (503) staff       (20)    10919 2023-06-21 18:05:33.000000 impoasdiff-0.0.3/impoasdiff/templates/report_v3.html
--rw-r--r--   0 yash.thadani   (503) staff       (20)     1231 2023-06-21 18:05:33.000000 impoasdiff-0.0.3/impoasdiff/utils.py
-drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-22 06:11:56.049112 impoasdiff-0.0.3/impoasdiff.egg-info/
--rw-r--r--   0 yash.thadani   (503) staff       (20)      701 2023-06-22 06:11:56.000000 impoasdiff-0.0.3/impoasdiff.egg-info/PKG-INFO
--rw-r--r--   0 yash.thadani   (503) staff       (20)      435 2023-06-22 06:11:56.000000 impoasdiff-0.0.3/impoasdiff.egg-info/SOURCES.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)        1 2023-06-22 06:11:56.000000 impoasdiff-0.0.3/impoasdiff.egg-info/dependency_links.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)       61 2023-06-22 06:11:56.000000 impoasdiff-0.0.3/impoasdiff.egg-info/entry_points.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)      114 2023-06-22 06:11:56.000000 impoasdiff-0.0.3/impoasdiff.egg-info/requires.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)       70 2023-06-22 06:11:56.000000 impoasdiff-0.0.3/impoasdiff.egg-info/top_level.txt
--rw-r--r--   0 yash.thadani   (503) staff       (20)       38 2023-06-22 06:11:56.050085 impoasdiff-0.0.3/setup.cfg
--rw-r--r--   0 yash.thadani   (503) staff       (20)     1097 2023-06-22 06:11:08.000000 impoasdiff-0.0.3/setup.py
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-26 18:02:54.432041 impoasdiff-0.0.4/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      701 2023-06-26 18:02:54.431790 impoasdiff-0.0.4/PKG-INFO
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      402 2023-06-22 06:11:47.000000 impoasdiff-0.0.4/README.md
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-26 18:02:54.426393 impoasdiff-0.0.4/impoasdiff/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      489 2023-06-21 19:42:52.000000 impoasdiff-0.0.4/impoasdiff/__init__.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      253 2023-06-21 19:34:04.000000 impoasdiff-0.0.4/impoasdiff/_version.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      522 2023-06-21 18:05:33.000000 impoasdiff-0.0.4/impoasdiff/args_manager.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)    22246 2023-06-26 17:53:34.000000 impoasdiff-0.0.4/impoasdiff/diff_handler.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     1218 2023-06-21 18:05:33.000000 impoasdiff-0.0.4/impoasdiff/file_handler.py
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     4777 2023-06-21 20:27:53.000000 impoasdiff-0.0.4/impoasdiff/generate_diff.py
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-26 18:02:54.430378 impoasdiff-0.0.4/impoasdiff/templates/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)    10919 2023-06-21 18:05:33.000000 impoasdiff-0.0.4/impoasdiff/templates/report_v3.html
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     1231 2023-06-21 18:05:33.000000 impoasdiff-0.0.4/impoasdiff/utils.py
+drwxr-xr-x   0 yash.thadani   (503) staff       (20)        0 2023-06-26 18:02:54.429360 impoasdiff-0.0.4/impoasdiff.egg-info/
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      701 2023-06-26 18:02:54.000000 impoasdiff-0.0.4/impoasdiff.egg-info/PKG-INFO
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      435 2023-06-26 18:02:54.000000 impoasdiff-0.0.4/impoasdiff.egg-info/SOURCES.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)        1 2023-06-26 18:02:54.000000 impoasdiff-0.0.4/impoasdiff.egg-info/dependency_links.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)       61 2023-06-26 18:02:54.000000 impoasdiff-0.0.4/impoasdiff.egg-info/entry_points.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)      103 2023-06-26 18:02:54.000000 impoasdiff-0.0.4/impoasdiff.egg-info/requires.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)       70 2023-06-26 18:02:54.000000 impoasdiff-0.0.4/impoasdiff.egg-info/top_level.txt
+-rw-r--r--   0 yash.thadani   (503) staff       (20)       38 2023-06-26 18:02:54.432095 impoasdiff-0.0.4/setup.cfg
+-rw-r--r--   0 yash.thadani   (503) staff       (20)     1099 2023-06-26 18:01:06.000000 impoasdiff-0.0.4/setup.py
```

### Comparing `impoasdiff-0.0.3/PKG-INFO` & `impoasdiff-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impoasdiff
-Version: 0.0.3
+Version: 0.0.4
 Summary: Open API diff tool
 Author: Yash Thadani
 Author-email: yash.thadani@imperva.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `impoasdiff-0.0.3/impoasdiff/args_manager.py` & `impoasdiff-0.0.4/impoasdiff/args_manager.py`

 * *Files identical despite different names*

### Comparing `impoasdiff-0.0.3/impoasdiff/diff_handler.py` & `impoasdiff-0.0.4/impoasdiff/diff_handler.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pprint
 from abc import ABC, abstractmethod
 from file_handler import FileManager
 
 pp = pprint.PrettyPrinter(indent=2)
 
+ENABLE_BASEPATH = False
 class DiffAnalyser(ABC):
     def __init__(self, diff_analyser_type) :
         self.diff_analyser_type = diff_analyser_type
 
     @abstractmethod
     def find_diff(self):
         pass
@@ -51,43 +52,90 @@
 
 def _get_oas_type(spec):
         oas_ver = 2 if spec.get("swagger", None) else 3 if spec.get("openapi", None) else "Unknown"
         return oas_ver
 
 def _scan_paths_oas2(spec):
         paths = spec.get("paths")
+        basepath = spec.get("basePath", "")
         all_paths = paths.keys()
-        return all_paths
+        all_paths_with_basepath = []
+        for path in all_paths:
+            all_paths_with_basepath.append((basepath + path).replace('//','/'))
+        return all_paths_with_basepath, all_paths
+
+        # return basepath, all_paths
+
+def _get_oas3_server(spec):
+    server = ""
+    server_found= False
+    spec_paths = spec.get('paths')
+    for path, path_val in spec_paths.items():
+        for method, method_val in path_val.items():
+            
+            if not isinstance(spec_paths.get(path).get(method), dict):
+                continue
+            if spec_paths.get(path).get(method).get('servers'):
+                server = spec_paths.get(path).get(method).get('servers')[0].get('url')
+                if server:
+                    server_found =True
+                    break
+        if server_found:
+            break
+    return server
+
+def _get_oas3_basepath(spec):
+    from urllib.parse import urlparse
+    server = _get_oas3_server(spec)
+    parsed_url = urlparse(server)
+    return parsed_url.path
+
+
+
 
 def _scan_paths_oas3( spec):
     paths = spec.get("paths")
+    
     all_paths = paths.keys()
-    return all_paths
+    all_paths_with_basepath = []
+    basepath = _get_oas3_basepath(spec)
+    for path in all_paths:
+        all_paths_with_basepath.append((basepath + path).replace('//','/'))
+    return all_paths_with_basepath, all_paths
 
 
 def _generate_aggregated_paths(file_list):
     all_scans = []
+    all_scans_without_basepath = []
     for file in file_list:
         oas_spec = FileManager(file).load_json()
         if _get_oas_type(spec = oas_spec)==2:
-            spec_scan = _scan_paths_oas2(oas_spec)
+            spec_scan, spec_scan_without_basepath = _scan_paths_oas2(oas_spec)
         elif _get_oas_type(oas_spec)==3:
-            spec_scan = _scan_paths_oas3(oas_spec)
+            spec_scan, spec_scan_without_basepath = _scan_paths_oas3(oas_spec)
         spec_scan_meta = [[file, path] for path in spec_scan]
+        spec_scan_meta_without_basepath = [[file, path] for path in spec_scan_without_basepath]
         all_scans += spec_scan_meta
-    return all_scans, len(all_scans)
+        all_scans_without_basepath+= spec_scan_meta_without_basepath
+    return all_scans, len(all_scans),all_scans_without_basepath
 
 def scan_all_paths(src_files, tar_files):
-    paths_src, src_api_count = _generate_aggregated_paths(src_files)
-    paths_tar, tar_api_count = _generate_aggregated_paths(tar_files)
+    paths_src, src_api_count, paths_src_without_basepath = _generate_aggregated_paths(src_files)
+    paths_tar, tar_api_count, paths_tar_without_basepath = _generate_aggregated_paths(tar_files)
     paths_src_dict  = {x[1]:x[0] for x in paths_src }
-    
     paths_tar_dict = {x[1]:x[0] for x in paths_tar}
     paths_src_list = [x[1] for x in paths_src]
     paths_tar_list = [x[1] for x in paths_tar]
+    paths_src_dict_without_basepath  = {x[1]:x[0] for x in paths_src_without_basepath }
+    paths_tar_dict_without_basepath  = {x[1]:x[0] for x in paths_tar_without_basepath }
+    paths_src_list_without_basepath = [x[1] for x in paths_src_without_basepath]
+    paths_tar_list_without_basepath = [x[1] for x in paths_tar_without_basepath]
+    paths_diff1_without_basepath  = list(set(paths_src_list_without_basepath)-set(paths_tar_list_without_basepath)) 
+    paths_diff2_without_basepath = list(set(paths_tar_list_without_basepath)- set(paths_src_list_without_basepath))
+    paths_common_without_basepath = list(set(paths_src_list_without_basepath).intersection(paths_tar_list_without_basepath))
 
     paths_diff1  = list(set(paths_src_list)-set(paths_tar_list)) 
     paths_diff2 = list(set(paths_tar_list)- set(paths_src_list))
     paths_common = list(set(paths_src_list).intersection(paths_tar_list))
 
     paths_diff1_with_file = [[paths_src_dict.get(x), x] for x in paths_diff1]
     paths_diff2_with_file = [[paths_tar_dict.get(x), x] for x in paths_diff2]
@@ -103,14 +151,16 @@
             paths_tar_dict_transpose[path_tar[0]].append(path_tar[1])
         else:
             paths_tar_dict_transpose[path_tar[0]] = [path_tar[1]]
     return [paths_diff1_with_file, paths_diff2_with_file, \
             src_api_count,tar_api_count, paths_src_dict_transpose,\
             paths_tar_dict_transpose, paths_common, \
             paths_src_dict,paths_tar_dict
+            , paths_src_dict_without_basepath,paths_tar_dict_without_basepath,
+            paths_common_without_basepath
             ]
 
 def is_hashable(value):
     try:
         hash(value)
         return True
     except TypeError:
@@ -137,20 +187,22 @@
 
 
 def _summary(src_files, tar_files):
     summary = {}
     summary['whats_new'], summary['whats_missing'],\
         summary['count_api_src_files'],summary['count_api_tar_files'],\
             summary['paths_src_dict_transpose'],summary['paths_tar_dict_transpose'],\
-                  paths_common, paths_src_dict, paths_tar_dict  = scan_all_paths(src_files, tar_files)
+                  paths_common, paths_src_dict, paths_tar_dict,\
+                      paths_src_dict_without_basepath,paths_tar_dict_without_basepath,\
+                         paths_common_without_basepath = scan_all_paths(src_files, tar_files)
     summary['count_src_files'] = len(src_files)
     summary['count_tar_files'] = len(tar_files)
     summary['count_whats_new'] = len(summary['whats_new'])
     summary['count_whats_missing'] = len(summary['whats_missing'])
-    diff_paths_methods,src_methods_dict,tar_methods_dict, src_methods_metadata_list,tar_methods_metadata_list = extract_metadata_endpoints(paths_common, paths_src_dict, paths_tar_dict)
+    diff_paths_methods,src_methods_dict,tar_methods_dict, src_methods_metadata_list,tar_methods_metadata_list = extract_metadata_endpoints(paths_common, paths_src_dict, paths_tar_dict,paths_common_without_basepath,paths_src_dict_without_basepath,paths_tar_dict_without_basepath)
     summary['diff_paths_methods'] = diff_paths_methods
     summary['tar_methods_dict'] = tar_methods_dict
     summary['src_methods_dict'] = src_methods_dict
     summary['src_methods_metadata_list'] = src_methods_metadata_list
     summary['tar_methods_metadata_list'] = tar_methods_metadata_list
     src_methods_metadata_dict = get_methods_metadata_dict(src_methods_metadata_list)
     tar_methods_metadata_dict = get_methods_metadata_dict(tar_methods_metadata_list)
@@ -252,21 +304,21 @@
                                 to_scan.append(v1)
     except Exception as e:
         pass
         # print(e)
         # print(v)
     return data_types
     
-def extract_metadata_endpoints(paths, src_file_map, tar_file_map ):
+def extract_metadata_endpoints(paths, src_file_map, tar_file_map,paths_common_without_basepath,paths_src_dict_without_basepath,paths_tar_dict_without_basepath ):
     diff_paths_methods = []
     src_methods_dict = {}
     tar_methods_dict = {}
     src_methods_metadata_list = []
     tar_methods_metadata_list = []
-    for path in paths:
+    for path in paths_common_without_basepath:
         src_file = src_file_map.get(path) 
         tar_file = tar_file_map.get(path)
         if src_file and tar_file:
             if not src_methods_dict.get(src_file):
                 src_methods_dict[src_file] = {}
             if not tar_methods_dict.get(tar_file):
                 tar_methods_dict[tar_file] = {}
@@ -293,26 +345,24 @@
                             temp_list.append([parameter, v])
                         elif k== 'schema':
                             data_types = resolve_definitions(file_path,v, path, method)
                             temp_list += data_types
                         if _get_oas_type(oas_spec) == 3:
                             data_types = resolve_definitions(file_path,v, path, method)
                             temp_list += data_types
-
             src_methods_metadata_list.append(temp_list)
 
     for file_path, file_value in tar_methods_dict.items():
         oas_spec = FileManager(file_path).load_json()
         for path, path_value in file_value.items():
             for method, method_value in path_value.items():
                 temp_list = [path,method]
                 if _get_oas_type(oas_spec) == 3:
                     data_types = resolve_definitions(file_path,{}, path, method)
                     temp_list += data_types
-
                 for parameter,param_val in method_value.items():
                     for k,v in param_val.items():
                         if k=='type':
                             temp_list.append([parameter,v])   
                 tar_methods_metadata_list.append(temp_list)
     return diff_paths_methods,src_methods_dict, tar_methods_dict, src_methods_metadata_list, tar_methods_metadata_list
 
@@ -325,16 +375,14 @@
         if not isinstance(method_value, dict):
             return methods_dict
         parameters = method_value.get('parameters', [])
         if spec_type == 2:
             for parameter in parameters:
                 parameter_name = parameter['name']
                 in_header = parameter['in']
-    #             # if parameter_name == 'body' and in_header == 'body':
-    #             #     continue
                 required = parameter.get('required', False)
                 if parameter.get('type'):
                     parameter_type = parameter['type']
                     methods_dict[method][parameter_name] = {
                         'in': in_header,
                         'required': required,
                         'type': parameter_type
@@ -358,22 +406,67 @@
                         'in': in_header,
                         'required': required,
                         'type': parameter_type
                     }
     return methods, methods_dict
 
 
+def _get_paths_oas2_dict(spec,path):
+    paths = spec.get("paths")
+    basepath = spec.get("basePath", "")
+    all_paths = paths.keys()
+    all_paths_with_basepath_dict = {}
+    return paths.get((basepath + path).replace('//','/'))
+    # for path in all_paths:
+    #     all_paths_with_basepath_dict[(basepath + path).replace('//','/')] = paths.get(path)
+    # return all_paths_with_basepath_dict, all_paths
+
+def _get_paths_oas3_dict(spec, path):
+    paths = spec.get("paths")
+    
+    all_paths = paths.keys()
+    all_paths_with_basepath = []
+    basepath = _get_oas3_basepath(spec)
+    return paths.get((basepath + path).replace('//','/'))
+    # all_paths_with_basepath_dict = {}
+    # for path in all_paths:
+    #     all_paths_with_basepath_dict[(basepath + path).replace('//','/')] = paths.get(path)
+    # return all_paths_with_basepath_dict, all_paths
+
+
+
+    return all_paths_with_basepath, all_paths
+
 def _get_path_from_spec(spec, path):
     spec_type = _get_oas_type(spec = spec)
     if spec_type== 2:
-        return spec.get('paths').get(path), spec_type
+        all_paths_with_basepath = _get_paths_oas2_dict(spec,path)
+        return all_paths_with_basepath, spec_type
     elif spec_type == 3:
-        return spec.get('paths').get(path), spec_type
+        all_paths_with_basepath = _get_paths_oas3_dict(spec,path)
+        return all_paths_with_basepath, spec_type
+
+# def _get_path_from_spec(spec, path):
+#     spec_type = _get_oas_type(spec = spec)
+#     if spec_type== 2:
+#         return spec.get('paths').get(path), spec_type
+#     elif spec_type == 3:
+#         return spec.get('paths').get(path), spec_type
+    
+def _scan_paths_oas3( spec):
+    paths = spec.get("paths")
+    
+    all_paths = paths.keys()
+    all_paths_with_basepath = []
+    basepath = _get_oas3_basepath(spec)
+    for path in all_paths:
+        all_paths_with_basepath.append((basepath + path).replace('//','/'))
 
 
+    return all_paths_with_basepath, all_paths
 def deep_compare(obj1, obj2):
     if type(obj1) != type(obj2):
         return False
     
     if isinstance(obj1, dict):
         if obj1.keys()  != obj2.keys():
             return False
```

### Comparing `impoasdiff-0.0.3/impoasdiff/file_handler.py` & `impoasdiff-0.0.4/impoasdiff/file_handler.py`

 * *Files identical despite different names*

### Comparing `impoasdiff-0.0.3/impoasdiff/generate_diff.py` & `impoasdiff-0.0.4/impoasdiff/generate_diff.py`

 * *Files identical despite different names*

### Comparing `impoasdiff-0.0.3/impoasdiff/templates/report_v3.html` & `impoasdiff-0.0.4/impoasdiff/templates/report_v3.html`

 * *Files identical despite different names*

### Comparing `impoasdiff-0.0.3/impoasdiff/utils.py` & `impoasdiff-0.0.4/impoasdiff/utils.py`

 * *Files identical despite different names*

### Comparing `impoasdiff-0.0.3/impoasdiff.egg-info/PKG-INFO` & `impoasdiff-0.0.4/impoasdiff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impoasdiff
-Version: 0.0.3
+Version: 0.0.4
 Summary: Open API diff tool
 Author: Yash Thadani
 Author-email: yash.thadani@imperva.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `impoasdiff-0.0.3/setup.py` & `impoasdiff-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="impoasdiff",
-    version=os.environ.get("VER", "0.0.3"),
+    version=os.environ.get("VER", "0.0.4"),
     author="Yash Thadani",
     author_email="yash.thadani@imperva.com",
     description="Open API diff tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     py_modules=["generate_diff", "file_handler", "diff_handler", "args_manager", "utils"], 
@@ -20,15 +20,15 @@
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3',
     entry_points = {'console_scripts': ['impoasdiff = impoasdiff.generate_diff:main']},
 
      install_requires = [
-        "idna==2.10",
+        # "idna==2.10",
         "Jinja2==3.1.2",
         "macholib==1.16.2",
         "MarkupSafe==2.1.3",
         "pyinstaller==5.12.0",
         "pyinstaller-hooks-contrib==2023.3",
     ],
     include_package_data=True,
```

