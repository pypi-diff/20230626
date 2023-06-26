# Comparing `tmp/jcmutils-1.5.8.tar.gz` & `tmp/jcmutils-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcmutils-1.5.8.tar", last modified: Tue May 23 09:15:55 2023, max compression
+gzip compressed data, was "jcmutils-1.5.9.tar", last modified: Tue May 23 11:11:52 2023, max compression
```

## Comparing `jcmutils-1.5.8.tar` & `jcmutils-1.5.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-23 09:15:55.891628 jcmutils-1.5.8/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.5.8/LICENSE
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-23 09:15:55.891628 jcmutils-1.5.8/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-05-17 04:08:25.000000 jcmutils-1.5.8/README.md
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-23 09:15:55.891628 jcmutils-1.5.8/jcmutils/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-05-17 04:08:25.000000 jcmutils-1.5.8/jcmutils/__init__.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)    11551 2023-05-23 09:14:48.000000 jcmutils-1.5.8/jcmutils/dataset_utils.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.5.8/jcmutils/gen_sources.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-05-17 04:08:25.000000 jcmutils-1.5.8/jcmutils/logger.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-17 04:08:25.000000 jcmutils-1.5.8/jcmutils/solver.py
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-23 09:15:55.891628 jcmutils-1.5.8/jcmutils.egg-info/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-23 09:15:55.000000 jcmutils-1.5.8/jcmutils.egg-info/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-05-23 09:15:55.000000 jcmutils-1.5.8/jcmutils.egg-info/SOURCES.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-05-23 09:15:55.000000 jcmutils-1.5.8/jcmutils.egg-info/dependency_links.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-23 09:15:55.000000 jcmutils-1.5.8/jcmutils.egg-info/requires.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-05-23 09:15:55.000000 jcmutils-1.5.8/jcmutils.egg-info/top_level.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-23 09:15:55.891628 jcmutils-1.5.8/setup.cfg
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-05-23 09:15:45.000000 jcmutils-1.5.8/setup.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-23 11:11:51.999141 jcmutils-1.5.9/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.5.9/LICENSE
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-23 11:11:51.999141 jcmutils-1.5.9/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-05-17 04:08:25.000000 jcmutils-1.5.9/README.md
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-23 11:11:51.999141 jcmutils-1.5.9/jcmutils/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-05-17 04:08:25.000000 jcmutils-1.5.9/jcmutils/__init__.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)    13888 2023-05-23 11:11:08.000000 jcmutils-1.5.9/jcmutils/dataset_utils.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.5.9/jcmutils/gen_sources.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-05-17 04:08:25.000000 jcmutils-1.5.9/jcmutils/logger.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-17 04:08:25.000000 jcmutils-1.5.9/jcmutils/solver.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-23 11:11:51.999141 jcmutils-1.5.9/jcmutils.egg-info/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-23 11:11:51.000000 jcmutils-1.5.9/jcmutils.egg-info/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-05-23 11:11:51.000000 jcmutils-1.5.9/jcmutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-05-23 11:11:51.000000 jcmutils-1.5.9/jcmutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-23 11:11:51.000000 jcmutils-1.5.9/jcmutils.egg-info/requires.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-05-23 11:11:51.000000 jcmutils-1.5.9/jcmutils.egg-info/top_level.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-23 11:11:51.999141 jcmutils-1.5.9/setup.cfg
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-05-23 11:11:25.000000 jcmutils-1.5.9/setup.py
```

### Comparing `jcmutils-1.5.8/LICENSE` & `jcmutils-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.8/README.md` & `jcmutils-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.8/jcmutils/dataset_utils.py` & `jcmutils-1.5.9/jcmutils/dataset_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,65 @@
         if not os.path.exists(os.path.dirname(database_path)):
             raise Exception("exporting dataset but resultbag dosen't exist")
         self.resultbag = jcmwave.Resultbag(abs_resultbag_dir)
         logger.debug("datagen inited,no error reported")
         logger.debug(
             f"jcmp_path is {jcmp_path},database_path is {abs_resultbag_dir}")
 
+    def export_dataset_one(self, num_of_result, source_density, target_density,target_filename,phi0, vmax, is_light_intense=True, is_symmetry=False):
+        # 路径预处理
+        if not os.path.exists(os.path.dirname(target_filename)):
+            os.makedirs(os.path.dirname(target_filename))
+
+        # 提取无缺陷图像
+        ## 先确定total_result的形状
+        temp_result = self.resultbag.get_result(self.keys[0])
+        field = (temp_result[num_of_result]['field'][0].conj() *
+                 temp_result[num_of_result]['field'][0]).sum(axis=2).real
+        total_results = np.zeros(field.shape)
+        logger.debug(f"total_result shape defined as {total_results.shape}")
+
+        ## 开始逐个提取结果
+        for key in self.keys:
+            result = self.resultbag.get_result(key)
+            field = (result[num_of_result]['field'][0].conj() *
+                     result[num_of_result]['field'][0]).sum(axis=2).real
+            if is_light_intense:
+                field = np.power(field, 2)
+            total_results += field
+            if is_symmetry and not (key['thetaphi'][0] == 0 and key['thetaphi'][1] == 0):
+                field = np.rot90(field, 2)
+                total_results += field
+                logger.debug("key was rotated for symmetry")
+        
+        # 合并最终结果
+        vmaxa = np.max(total_results) if vmax is None else vmax
+        afield = (total_results/ vmaxa)*235
+        afield = np.rot90(afield)
+
+        label_name = target_filename + ".txt"
+        with open(label_name,"w") as f:
+            f.write("")
+
+        # 保存超分辨（原图）
+        cv2.imwrite(target_filename + "_origin.jpg",afield)
+
+        # 通过每个像素点代表的实际物理尺寸来计算缩放比比例
+        scale_factor =source_density*1.0/target_density
+        # 缩放电场/光强场到对应的大小
+        scaled_field = cv2.resize(output_image, None, fx=scale_factor,# type: ignore
+                                  fy=scale_factor, interpolation=cv2.INTER_LINEAR)  
+
+        # 绘图
+        logger.debug(f"printing max value of results:{np.max(total_results)}")
+        cv2.imwrite(target_filename + ".jpg",scaled_field)
+        logger.info("all target image saved completed!")
+
+
+
     def export_dataset(self, num_of_result, source_density, target_density,target_filename,phi0,defect_size, vmax, is_light_intense=True, is_symmetry=False):
         # 路径预处理
         if not os.path.exists(os.path.dirname(target_filename)):
             os.makedirs(os.path.dirname(target_filename))
         yamlpath =os.path.join(os.path.dirname(self.jcmp_path),"properties.yaml")
         
         # 解析YAML，准备必须的数据
@@ -118,21 +169,22 @@
         # diff_img = np.clip(diff_img, 0, 255).astype(np.uint8)
 
         gradX = cv2.Sobel(diff_img, ddepth=cv2.CV_32F, dx=1, dy=0, ksize=-1)
         gradY = cv2.Sobel(diff_img, ddepth=cv2.CV_32F, dx=0, dy=1, ksize=-1)
         
         # subtract the y-gradient from the x-gradient
         gradient = cv2.subtract(gradX, gradY)
-        gradient = cv2.convertScaleAbs(gradient)
+        gradient = cv2.convertScaleAbs(gradient)        
+        defect_lowborder = np.max(gradient) * 0.35
         blurred = cv2.blur(gradient, (5, 5),borderType=cv2.BORDER_REFLECT) 
-        (_, thresh) = cv2.threshold(blurred, 55 , 255, cv2.THRESH_BINARY)
+        (_, thresh) = cv2.threshold(blurred, defect_lowborder, 255, cv2.THRESH_BINARY)
         kernel = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (11, 11))
         closed = cv2.morphologyEx(thresh, cv2.MORPH_CLOSE, kernel,iterations=2,borderType=cv2.BORDER_ISOLATED)
-        closed = cv2.erode(closed, None, iterations=6)
-        closed = cv2.dilate(closed, None, iterations=7)
+        closed = cv2.erode(closed, None, iterations=4)
+        closed = cv2.dilate(closed, None, iterations=5)
 
         # 找距离图像中心点最近的一个封闭区域
         (cnts, _) = cv2.findContours(closed.copy(), cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
         # c = sorted(cnts, key=cv2.contourArea, reverse=True)[0]
         min_dist = -1
         c = cnts[0]
         for conners in cnts:
```

### Comparing `jcmutils-1.5.8/jcmutils/gen_sources.py` & `jcmutils-1.5.9/jcmutils/gen_sources.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.8/jcmutils/logger.py` & `jcmutils-1.5.9/jcmutils/logger.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.8/jcmutils/solver.py` & `jcmutils-1.5.9/jcmutils/solver.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.8/setup.py` & `jcmutils-1.5.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 
-VERSION = '1.5.8'
+VERSION = '1.5.9'
 DESCRIPTION = "A general utils for jcmsuite"
 
 setup(
     name="jcmutils",
     version=VERSION,
     author="crafter-z",
     author_email="crafterz@163.com",
```

