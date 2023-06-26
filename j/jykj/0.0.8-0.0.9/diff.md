# Comparing `tmp/jykj-0.0.8.tar.gz` & `tmp/jykj-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jykj-0.0.8.tar", last modified: Sun Jun 25 07:36:41 2023, max compression
+gzip compressed data, was "jykj-0.0.9.tar", last modified: Mon Jun 26 09:54:01 2023, max compression
```

## Comparing `jykj-0.0.8.tar` & `jykj-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 07:36:41.707391 jykj-0.0.8/
--rw-rw-rw-   0        0        0     1088 2023-05-04 06:17:54.000000 jykj-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      348 2023-06-25 07:36:41.707391 jykj-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-25 07:36:41.673390 jykj-0.0.8/jykj/
--rw-rw-rw-   0        0        0        0 2023-05-15 03:16:59.000000 jykj-0.0.8/jykj/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 07:36:41.705406 jykj-0.0.8/jykj/business_model/
--rw-rw-rw-   0        0        0    17264 2023-06-25 06:46:54.000000 jykj-0.0.8/jykj/business_model/SHE.py
--rw-rw-rw-   0        0        0        0 2023-06-19 10:33:51.000000 jykj-0.0.8/jykj/business_model/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-19 10:33:15.000000 jykj-0.0.8/jykj/business_model/prevention.py
--rw-rw-rw-   0        0        0        0 2023-06-19 10:33:29.000000 jykj-0.0.8/jykj/business_model/production.py
--rw-rw-rw-   0        0        0    14683 2023-06-25 06:46:56.000000 jykj-0.0.8/jykj/business_model/security.py
--rw-rw-rw-   0        0        0    28571 2023-06-25 07:34:18.000000 jykj-0.0.8/jykj/business_model/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-25 07:36:41.693390 jykj-0.0.8/jykj.egg-info/
--rw-rw-rw-   0        0        0      348 2023-06-25 07:36:41.000000 jykj-0.0.8/jykj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-06-25 07:36:41.000000 jykj-0.0.8/jykj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 07:36:41.000000 jykj-0.0.8/jykj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-25 07:36:41.000000 jykj-0.0.8/jykj.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-25 07:36:41.000000 jykj-0.0.8/jykj.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 07:36:41.708391 jykj-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      569 2023-06-25 07:36:35.000000 jykj-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:54:01.696404 jykj-0.0.9/
+-rw-rw-rw-   0        0        0     1088 2023-05-04 06:17:54.000000 jykj-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      348 2023-06-26 09:54:01.695403 jykj-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-26 09:54:01.658404 jykj-0.0.9/jykj/
+-rw-rw-rw-   0        0        0        0 2023-05-15 03:16:59.000000 jykj-0.0.9/jykj/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:54:01.694419 jykj-0.0.9/jykj/business_model/
+-rw-rw-rw-   0        0        0    17686 2023-06-26 09:53:12.000000 jykj-0.0.9/jykj/business_model/SHE.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 10:33:51.000000 jykj-0.0.9/jykj/business_model/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 10:33:15.000000 jykj-0.0.9/jykj/business_model/prevention.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 10:33:29.000000 jykj-0.0.9/jykj/business_model/production.py
+-rw-rw-rw-   0        0        0    14683 2023-06-25 06:46:56.000000 jykj-0.0.9/jykj/business_model/security.py
+-rw-rw-rw-   0        0        0    28571 2023-06-26 09:53:23.000000 jykj-0.0.9/jykj/business_model/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:54:01.679406 jykj-0.0.9/jykj.egg-info/
+-rw-rw-rw-   0        0        0      348 2023-06-26 09:54:01.000000 jykj-0.0.9/jykj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-06-26 09:54:01.000000 jykj-0.0.9/jykj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 09:54:01.000000 jykj-0.0.9/jykj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-26 09:54:01.000000 jykj-0.0.9/jykj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-26 09:54:01.000000 jykj-0.0.9/jykj.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 09:54:01.696404 jykj-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      569 2023-06-26 09:53:50.000000 jykj-0.0.9/setup.py
```

### Comparing `jykj-0.0.8/LICENSE` & `jykj-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jykj-0.0.8/jykj/business_model/SHE.py` & `jykj-0.0.9/jykj/business_model/SHE.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,45 +39,60 @@
         persons_coords = [persons_coords]
     if np.array(areas).ndim == 2:
         areas = [areas]
 
     assert -0.5 <= h_offset <= 0.5
 
     # 判断是相对坐标还是绝对坐标(不严格)
-    abs_person = True if np.array(persons_coords).dtype == int else False
-    abs_area = True if np.array(areas[0]).dtype == int else False
+    if (np.array(persons_coords).dtype == float) and (np.array(persons_coords) <= 1).all():
+        abs_person = False
+    else:
+        abs_person = True
+
+    if (np.array(areas[0]).dtype == float) and (np.array(areas[0]) <= 1).all():
+        abs_area = False
+    else:
+        abs_area = True
 
     if abs_person != abs_area and not resolution:
         raise ValueError("未指定视频分辨率")
 
     # 如果坐标类型不一致就全部转为绝对坐标
     if abs_person == True and abs_area == False:
+        new_areas = []
         for area in areas:
-            area = rela_to_abs(area, resolution)
+            new_areas.append(rela_to_abs(area, resolution))
+        areas = new_areas
     elif abs_person == False and abs_area == True:
         persons_coords = rela_to_abs(persons_coords, resolution)
 
     # 宽度过滤
     if w_thresh != -1:
         assert 0 < w_thresh <= 1
         if abs_person:
             if not resolution:
                 raise ValueError("未指定视频分辨率")
             else:
                 w_thresh = int(w_thresh * resolution[0])
+        else:
+            if abs_area:
+                w_thresh = int(w_thresh * resolution[0])
         persons_coords = [p for p in persons_coords if p[2] <= w_thresh]
 
     # 高度过滤
     if h_thresh != -1:
         assert 0 < h_thresh <= 1
         if abs_person:
             if not resolution:
                 raise ValueError("未指定视频分辨率")
             else:
                 h_thresh = int(h_thresh * resolution[1])
+        else:
+            if abs_area:
+                h_thresh = int(h_thresh * resolution[1])
         persons_coords = [p for p in persons_coords if p[3] <= h_thresh]
 
     for p in persons_coords:
         cx = p[0]
         cy = p[1] + int(h_offset * p[3])
         for area in areas:
             if pnpoly(area, cx, cy):
```

### Comparing `jykj-0.0.8/jykj/business_model/security.py` & `jykj-0.0.9/jykj/business_model/security.py`

 * *Files identical despite different names*

### Comparing `jykj-0.0.8/jykj/business_model/utils.py` & `jykj-0.0.9/jykj/business_model/utils.py`

 * *Files identical despite different names*

### Comparing `jykj-0.0.8/setup.py` & `jykj-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="jykj",
-    version="0.0.8",
+    version="0.0.9",
     author="jykj",
     author_email="renshuai@jylink.com",
     description="",
     long_description="",
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

