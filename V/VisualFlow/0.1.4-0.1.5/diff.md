# Comparing `tmp/VisualFlow-0.1.4.tar.gz` & `tmp/VisualFlow-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VisualFlow-0.1.4.tar", last modified: Mon Jun 26 02:46:50 2023, max compression
+gzip compressed data, was "VisualFlow-0.1.5.tar", last modified: Mon Jun 26 03:19:11 2023, max compression
```

## Comparing `VisualFlow-0.1.4.tar` & `VisualFlow-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 02:46:50.195799 VisualFlow-0.1.4/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4134 2023-06-26 02:46:50.195799 VisualFlow-0.1.4/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2651 2023-06-25 22:23:46.000000 VisualFlow-0.1.4/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 02:46:50.195799 VisualFlow-0.1.4/VisualFlow/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       35 2023-06-26 02:45:48.000000 VisualFlow-0.1.4/VisualFlow/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18981 2023-06-25 22:23:46.000000 VisualFlow-0.1.4/VisualFlow/visualflow.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 02:46:50.195799 VisualFlow-0.1.4/VisualFlow.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4134 2023-06-26 02:46:50.000000 VisualFlow-0.1.4/VisualFlow.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      235 2023-06-26 02:46:50.000000 VisualFlow-0.1.4/VisualFlow.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-26 02:46:50.000000 VisualFlow-0.1.4/VisualFlow.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-06-26 02:46:50.000000 VisualFlow-0.1.4/VisualFlow.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-06-26 02:46:50.000000 VisualFlow-0.1.4/VisualFlow.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-26 02:46:50.195799 VisualFlow-0.1.4/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1011 2023-06-26 02:46:12.000000 VisualFlow-0.1.4/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 03:19:11.490939 VisualFlow-0.1.5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4405 2023-06-26 03:19:11.490939 VisualFlow-0.1.5/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2890 2023-06-26 03:10:07.000000 VisualFlow-0.1.5/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 03:19:11.486938 VisualFlow-0.1.5/VisualFlow/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       35 2023-06-26 02:45:48.000000 VisualFlow-0.1.5/VisualFlow/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18762 2023-06-26 03:15:28.000000 VisualFlow-0.1.5/VisualFlow/visualflow.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 03:19:11.490939 VisualFlow-0.1.5/VisualFlow.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4405 2023-06-26 03:19:11.000000 VisualFlow-0.1.5/VisualFlow.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      235 2023-06-26 03:19:11.000000 VisualFlow-0.1.5/VisualFlow.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-26 03:19:11.000000 VisualFlow-0.1.5/VisualFlow.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-06-26 03:19:11.000000 VisualFlow-0.1.5/VisualFlow.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-06-26 03:19:11.000000 VisualFlow-0.1.5/VisualFlow.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-26 03:19:11.490939 VisualFlow-0.1.5/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1011 2023-06-26 03:17:18.000000 VisualFlow-0.1.5/setup.py
```

### Comparing `VisualFlow-0.1.4/PKG-INFO` & `VisualFlow-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: VisualFlow
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python library for object detection format conversion
 Home-page: https://github.com/Ojas-Sharma/VisualFlow
 Author: Ojas Sharma
 Author-email: ojassharma1607@gmail.com
 License: UNKNOWN
 Description: # VisualFlow
         
         VisualFlow is a Python library for object detection that provides conversion functions between Pascal VOC, YOLO, and COCO formats. It aims to simplify the process of converting annotated datasets between these popular object detection formats.
         
+        We have started this library with the vision of providing end to end object detection, from formatting all the way to inferencing multiple types of object detection models.
+        
+        Our initial version of VisualFlow allows format conversions between PASCAL VOC, COCO and YOLO. Stay tuned for future updates!
+        
         ## Installation
         
         You can install VisualFlow using pip:
         
         ```bash
         pip install visualflow
         ```
@@ -22,74 +26,74 @@
         VisualFlow provides three main conversion functions: to_voc(), to_yolo(), and to_coco(). Here's how you can use them:
         
         ### Conversion to YOLO Format
         To convert from PASCAL VOC or COCO format to YOLO format, use the to_yolo() function.
         
         For VOC to YOLO:
         ```python
-        import visualflow as vf
+        import VisualFlow as vf
         
-        vf.to_yolo(input_type='voc',
-               image_folder='path/to/images',
-               ann_folder='path/to/annotations',
-               output_folder='path/to/output')
+        vf.to_yolo(in_format='voc',
+               images='path/to/images',
+               annotations='path/to/annotations',
+               out_dir='path/to/output')
         ```
         For COCO to YOLO:
         ```python
-        import visualflow as vf
+        import VisualFlow as vf
         
-        vf.to_yolo(input_type='coco',
-               image_folder='path/to/images',
-               output_folder='path/to/output',
+        vf.to_yolo(in_format='coco',
+               images='path/to/images',
+               out_dir='path/to/output',
                json_file='path/to/annotations.json')
         ```
         
         ### Conversion to Pascal VOC Format
         To convert from COCO or YOLO format to Pascal VOC format, use the to_voc() function.
         
         For COCO to VOC:
         ```python
-        import visualflow as vf
+        import VisualFlow as vf
         
-        vf.to_voc(input_type='coco',
-               image_folder='path/to/images',
-               output_folder='path/to/output',
+        vf.to_voc(in_format='coco',
+               images='path/to/images',
+               out_dir='path/to/output',
                json_file='path/to/annotations.json')
         ```
         For YOLO to VOC:
         ```python
-        import visualflow as vf
+        import VisualFlow as vf
         
-        vf.to_voc(input_type='yolo',
-               image_folder='path/to/images',
-               ann_folder='path/to/annotations',
+        vf.to_voc(in_format='yolo',
+               images='path/to/images',
+               annotations='path/to/annotations',
                class_file='path/to/classes.txt',
-               output_folder='path/to/output')
+               out_dir='path/to/output')
         ```
         
         ### Conversion to COCO Format
         To convert from PASCAL VOC or YOLO format to COCO format, use the to_coco() function.
         
         For VOC to COCO:
         ```python
-        import visualflow as vf
+        import VisualFlow as vf
         
-        vf.to_coco(input_type='voc',
-               image_folder='path/to/images',
-               ann_folder='path/to/annotations',
+        vf.to_coco(in_format='voc',
+               images='path/to/images',
+               annotations='path/to/annotations',
                class_file='path/to/classes.txt',
                output_file_path='path/to/output.json')
         ```
         For YOLO to COCO:
         ```python
-        import visualflow as vf
+        import VisualFlow as vf
         
-        vf.to_coco(input_type='yolo',
-               image_folder='path/to/images',
-               ann_folder='path/to/annotations',
+        vf.to_coco(in_format='yolo',
+               images='path/to/images',
+               annotations='path/to/annotations',
                class_file='path/to/classes.txt',
                output_file_path='path/to/output.json')
         ```
         
         Make sure to replace 'path/to/images', 'path/to/annotations', 'path/to/classes.txt', and 'path/to/output' with the actual paths to your dataset files and folders.
         
         ## Contributing
```

### Comparing `VisualFlow-0.1.4/VisualFlow/visualflow.py` & `VisualFlow-0.1.5/VisualFlow/visualflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,42 +40,42 @@
     return [xmin,ymin, w, h]
 
 def coco2yolo(xmin, ymin, w, h, image_w, image_h):
     x_center = ((2*xmin + w)/(2*image_w))
     y_center = ((2*ymin + h)/(2*image_h))
     return [x_center , y_center, w/image_w, h/image_h]
 
-def to_voc(input_type=None, image_folder=None, ann_folder=None, class_file=None, output_folder=None, json_file=None):
-    if input_type is None:
+def to_voc(in_format=None, images=None, annotations=None, class_file=None, out_dir=None, json_file=None):
+    if in_format is None:
         raise ValueError("Missing input argument: Please provide input type ('yolo' or 'coco')")
-    if output_folder is None:
-        raise ValueError("Missing argument: output_folder")
-    if image_folder is None:
-        raise ValueError("Missing argument: image_folder")
-    if not os.path.isdir(os.path.join(output_folder, "xmls")):
-        os.mkdir(os.path.join(output_folder, "xmls"))
-    if input_type == "yolo":
+    if out_dir is None:
+        raise ValueError("Missing argument: out_dir")
+    if images is None:
+        raise ValueError("Missing argument: images")
+    if not os.path.isdir(os.path.join(out_dir, "xmls")):
+        os.mkdir(os.path.join(out_dir, "xmls"))
+    if in_format == "yolo":
         if class_file is None:
             raise ValueError("Please provide path to classes.txt")
-        if ann_folder is None:
-            raise ValueError("Missing argument: ann_folder")
+        if annotations is None:
+            raise ValueError("Missing argument: annotations")
         else:
             class_dict = {}
             with open(class_file, 'r') as file:
                 for line_num, name in enumerate(file):
                     name = name.strip()
                     class_dict[line_num] = name
 
             image_info = []
-            image_files = [filename for filename in os.listdir(image_folder) if filename.endswith(('.png', '.jpg', '.jpeg', '.webp'))]
+            image_files = [filename for filename in os.listdir(images) if filename.endswith(('.png', '.jpg', '.jpeg', '.webp'))]
             with tqdm(total=len(image_files), desc="Converting...") as pbar:
-                for filename in os.listdir(image_folder):
+                for filename in os.listdir(images):
                     if filename.endswith(('.png', '.jpg', '.jpeg', '.webp')):
-                        image_path = os.path.join(image_folder, filename)
-                        label_path = os.path.join(ann_folder, filename.rsplit(".", 1)[0] + ".txt")
+                        image_path = os.path.join(images, filename)
+                        label_path = os.path.join(annotations, filename.rsplit(".", 1)[0] + ".txt")
                         try:
                             image_width, image_height = 0, 0
                             with Image.open(image_path) as img:
                                 image_width, image_height = img.size
                             with open(label_path, 'r') as label:
                                 bboxes = []
                                 for line in label:
@@ -94,15 +94,15 @@
                                 writer.save(os.path.join(output, "xmls", filename.rsplit(".", 1)[0] + ".xml"))
                         except OSError:
                             print(image_path + " skipped")
                             pass
                         pbar.update(1)
             print("Completed!")
 
-    if input_type == "coco":
+    if in_format == "coco":
         if json_file is None:
             raise ValueError("Missing argument: json_file. Please provide path to json file")
         else:
             print("starting")
             bbox_mapping = {}
             class_mapping = {}
             coco = json.load(open(json_file, 'r'))
@@ -118,46 +118,46 @@
                 w = ann['bbox'][2]
                 h = ann['bbox'][3]
                 bbox_mapping[image_id].append([ann["category_id"] - 1, xmin, ymin, w, h])
             with tqdm(total=len(coco['images']), desc="Converting...") as pbar:
                 for im in coco['images']:
                     result = []
                     bboxes = bbox_mapping[im["id"]]
-                    image_path = os.path.join(image_folder, os.path.basename(im["file_name"]))
+                    image_path = os.path.join(images, os.path.basename(im["file_name"]))
                     writer = Writer(image_path, im["width"], im["height"])
                     for bbox in bboxes:
                         voc_bbox = coco2pascalvoc(bbox[1], bbox[2], bbox[3], bbox[4])
                         writer.addObject(class_mapping[bbox[0]], voc_bbox[0], voc_bbox[1], voc_bbox[2], voc_bbox[3])
                     xml_filename = os.path.basename(im["file_name"]).rsplit(".", 1)[0]
-                    writer.save(os.path.join(output_folder, "xmls", xml_filename + ".xml"))
+                    writer.save(os.path.join(out_dir, "xmls", xml_filename + ".xml"))
                     pbar.update(1)
             print("Completed!")
 
 
-def to_yolo(input_type=None, image_folder=None, ann_folder=None, output_folder=None, json_file=None):
-    if input_type is None:
+def to_yolo(in_format=None, images=None, annotations=None, out_dir=None, json_file=None):
+    if in_format is None:
         raise ValueError("Missing input argument: Please provide input type ('voc' or 'coco')")
-    if output_folder is None:
-        raise ValueError("Missing argument: output_folder")
-    if image_folder is None:
-        raise ValueError("Missing argument: image_folder")
-    if not os.path.isdir(os.path.join(output_folder, "labels")):
-        os.mkdir(os.path.join(output_folder, "labels"))
-    if input_type == "voc":
-        if ann_folder is None:
-            raise ValueError("Missing argument: ann_folder")
+    if out_dir is None:
+        raise ValueError("Missing argument: out_dir")
+    if images is None:
+        raise ValueError("Missing argument: images")
+    if not os.path.isdir(os.path.join(out_dir, "labels")):
+        os.mkdir(os.path.join(out_dir, "labels"))
+    if in_format == "voc":
+        if annotations is None:
+            raise ValueError("Missing argument: annotations")
         else:
             class_lst = []
-            class_path = os.path.join(output_folder, "classes.txt")
-            image_files = [filename for filename in os.listdir(image_folder) if filename.endswith(('.png', '.jpg', '.jpeg', '.webp'))]
+            class_path = os.path.join(out_dir, "classes.txt")
+            image_files = [filename for filename in os.listdir(images) if filename.endswith(('.png', '.jpg', '.jpeg', '.webp'))]
             with tqdm(total=len(image_files), desc="Converting...") as pbar:
-                for filename in os.listdir(image_folder):
+                for filename in os.listdir(images):
                     if filename.endswith(('.png', '.jpg', '.jpeg', '.webp')):
-                        image_path = os.path.join(image_folder, filename)
-                        label_path = os.path.join(ann_folder, filename.rsplit(".", 1)[0] + ".xml")
+                        image_path = os.path.join(images, filename)
+                        label_path = os.path.join(annotations, filename.rsplit(".", 1)[0] + ".xml")
                         try:
                             image_width, image_height = 0, 0
                             with Image.open(image_path) as img:
                                 image_width, image_height = img.size
                             result = []
                             tree = ET.parse(label_path)
                             root = tree.getroot()
@@ -171,26 +171,26 @@
                                 bbox = [float(x.text) for x in obj.find("bndbox")]
                                 yolo_bbox = pascalvoc2yolo(bbox[0], bbox[1], bbox[2], bbox[3], width, height)
                                 bbox_string = " ".join([str(x) for x in yolo_bbox])
                                 result.append(f"{index} {bbox_string}")
 
                             if result:
                                 label_name = filename.rsplit(".", 1)[0] + ".txt"
-                                with open(os.path.join(output_folder, "labels", label_name), "w", encoding="utf-8") as f:
+                                with open(os.path.join(out_dir, "labels", label_name), "w", encoding="utf-8") as f:
                                     f.write("\n".join(result))
                         except OSError:
                             print(image_path + " skipped")
                             pass
                         pbar.update(1)
                 with open(class_path, 'w', encoding='utf8') as f:
                     for item in class_lst:
                         f.write(item + '\n')
             print("Completed!")
 
-    if input_type == "coco":
+    if in_format == "coco":
         if json_file is None:
             raise ValueError("Missing argument: json_file. Please provide path to json file")
         else:
             print("starting")
             bbox_mapping = {}
             class_mapping = {}
             coco = json.load(open(json_file, 'r'))
@@ -213,44 +213,44 @@
                     for bbox in bboxes:
                         yolo_bbox = coco2yolo(bbox[1], bbox[2], bbox[3], bbox[4], im["width"], im["height"])
                         bbox_string = " ".join([str(x) for x in yolo_bbox])
                         result.append(f"{bbox[0]} {bbox_string}")
                     if result:
                         image_filename = os.path.basename(im["file_name"]).rsplit(".", 1)[0]
 
-                        with open(os.path.join(output_folder, "labels", f"{image_filename}.txt"), "w", encoding="utf-8") as f:
+                        with open(os.path.join(out_dir, "labels", f"{image_filename}.txt"), "w", encoding="utf-8") as f:
                             f.write("\n".join(result))
                     pbar.update(1)
             print("Completed!")
 
 
 
-def to_coco(input_type=None, image_folder=None, ann_folder=None, class_file=None, output_file_path=None):
-    if input_type is None:
+def to_coco(in_format=None, images=None, annotations=None, class_file=None, output_file_path=None):
+    if in_format is None:
         raise ValueError("Missing input argument: Please provide input type ('yolo' or 'voc')")
     if output_file_path is None:
         raise ValueError("Missing argument: output_file_path")
-    if image_folder is None:
-        raise ValueError("Missing argument: image_folder")
-    if ann_folder is None:
-        raise ValueError("Missing argument: ann_folder")
-    if input_type == "yolo":
+    if images is None:
+        raise ValueError("Missing argument: images")
+    if annotations is None:
+        raise ValueError("Missing argument: annotations")
+    if in_format == "yolo":
         if class_file is None:
             raise ValueError("Please provide path to classes.txt which has a list of all your classes (one class on each line)")
         coco = {"images": [{}], "categories": [], "annotations": [{}]}
         image_id = 0
         ann_id = 1
         image_info = []
         ann_info = []
-        image_files = [filename for filename in os.listdir(image_folder) if filename.endswith(('.png', '.jpg', '.jpeg', '.webp'))]
+        image_files = [filename for filename in os.listdir(images) if filename.endswith(('.png', '.jpg', '.jpeg', '.webp'))]
         with tqdm(total=len(image_files), desc="Converting...") as pbar:
-            for filename in os.listdir(image_folder):
+            for filename in os.listdir(images):
                 if filename.endswith(('.png', '.jpg', '.jpeg', '.webp')):
-                    image_path = os.path.join(image_folder, filename)
-                    label_path = os.path.join(ann_folder, filename.rsplit(".", 1)[0] + ".txt")
+                    image_path = os.path.join(images, filename)
+                    label_path = os.path.join(annotations, filename.rsplit(".", 1)[0] + ".txt")
                     try:
                         image_width, image_height = 0, 0
                         with Image.open(image_path) as img:
                             image_width, image_height = img.size
                             image_stats = {
                                             "file_name": image_path,
                                             "height": image_height,
@@ -296,33 +296,33 @@
                         "name": name,
                     }
                     coco["categories"].append(categories)
             with open(output_file_path, "w") as outfile:
                 json.dump(coco, outfile, indent=4)
         print("Completed!")
     
-    if input_type == "voc":
+    if in_format == "voc":
         if class_file is None:
             raise ValueError("Please provide path to classes.txt which has a list of all your classes (one class on each line)")
         coco = {"images": [{}], "categories": [], "annotations": [{}]}
         image_id = 0
         ann_id = 1
         image_info = []
         ann_info = []
         class_dict = {}
         with open(class_file, 'r') as file:
             for line_num, name in enumerate(file):
                 name = name.strip()
                 class_dict[name] = line_num + 1
-        image_files = [filename for filename in os.listdir(image_folder) if filename.endswith(('.png', '.jpg', '.jpeg', '.webp'))]
+        image_files = [filename for filename in os.listdir(images) if filename.endswith(('.png', '.jpg', '.jpeg', '.webp'))]
         with tqdm(total=len(image_files), desc="Converting...") as pbar:
-            for filename in os.listdir(image_folder):
+            for filename in os.listdir(images):
                 if filename.endswith(('.png', '.jpg', '.jpeg', '.webp')):
-                    image_path = os.path.join(image_folder, filename)
-                    label_path = os.path.join(ann_folder, filename.rsplit(".", 1)[0] + ".xml")
+                    image_path = os.path.join(images, filename)
+                    label_path = os.path.join(annotations, filename.rsplit(".", 1)[0] + ".xml")
                     tree = ET.parse(label_path)
                     root = tree.getroot()
                     image_height = int(root.find("size")[0].text)
                     image_width = int(root.find("size")[1].text)
                     image_channels = int(root.find("size")[2].text)
                     try:
                         image_width, image_height = 0, 0
@@ -367,11 +367,8 @@
                         "supercategory": "Null",
                         "id": line_num + 1,
                         "name": name,
                     }
                     coco["categories"].append(categories)
             with open(output_file_path, "w") as outfile:
                 json.dump(coco, outfile, indent=4)
-        print("Completed!")
-
-
-
+        print("Completed!")
```

### Comparing `VisualFlow-0.1.4/VisualFlow.egg-info/PKG-INFO` & `VisualFlow-0.1.5/VisualFlow.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: VisualFlow
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python library for object detection format conversion
 Home-page: https://github.com/Ojas-Sharma/VisualFlow
 Author: Ojas Sharma
 Author-email: ojassharma1607@gmail.com
 License: UNKNOWN
 Description: # VisualFlow
         
         VisualFlow is a Python library for object detection that provides conversion functions between Pascal VOC, YOLO, and COCO formats. It aims to simplify the process of converting annotated datasets between these popular object detection formats.
         
+        We have started this library with the vision of providing end to end object detection, from formatting all the way to inferencing multiple types of object detection models.
+        
+        Our initial version of VisualFlow allows format conversions between PASCAL VOC, COCO and YOLO. Stay tuned for future updates!
+        
         ## Installation
         
         You can install VisualFlow using pip:
         
         ```bash
         pip install visualflow
         ```
@@ -22,74 +26,74 @@
         VisualFlow provides three main conversion functions: to_voc(), to_yolo(), and to_coco(). Here's how you can use them:
         
         ### Conversion to YOLO Format
         To convert from PASCAL VOC or COCO format to YOLO format, use the to_yolo() function.
         
         For VOC to YOLO:
         ```python
-        import visualflow as vf
+        import VisualFlow as vf
         
-        vf.to_yolo(input_type='voc',
-               image_folder='path/to/images',
-               ann_folder='path/to/annotations',
-               output_folder='path/to/output')
+        vf.to_yolo(in_format='voc',
+               images='path/to/images',
+               annotations='path/to/annotations',
+               out_dir='path/to/output')
         ```
         For COCO to YOLO:
         ```python
-        import visualflow as vf
+        import VisualFlow as vf
         
-        vf.to_yolo(input_type='coco',
-               image_folder='path/to/images',
-               output_folder='path/to/output',
+        vf.to_yolo(in_format='coco',
+               images='path/to/images',
+               out_dir='path/to/output',
                json_file='path/to/annotations.json')
         ```
         
         ### Conversion to Pascal VOC Format
         To convert from COCO or YOLO format to Pascal VOC format, use the to_voc() function.
         
         For COCO to VOC:
         ```python
-        import visualflow as vf
+        import VisualFlow as vf
         
-        vf.to_voc(input_type='coco',
-               image_folder='path/to/images',
-               output_folder='path/to/output',
+        vf.to_voc(in_format='coco',
+               images='path/to/images',
+               out_dir='path/to/output',
                json_file='path/to/annotations.json')
         ```
         For YOLO to VOC:
         ```python
-        import visualflow as vf
+        import VisualFlow as vf
         
-        vf.to_voc(input_type='yolo',
-               image_folder='path/to/images',
-               ann_folder='path/to/annotations',
+        vf.to_voc(in_format='yolo',
+               images='path/to/images',
+               annotations='path/to/annotations',
                class_file='path/to/classes.txt',
-               output_folder='path/to/output')
+               out_dir='path/to/output')
         ```
         
         ### Conversion to COCO Format
         To convert from PASCAL VOC or YOLO format to COCO format, use the to_coco() function.
         
         For VOC to COCO:
         ```python
-        import visualflow as vf
+        import VisualFlow as vf
         
-        vf.to_coco(input_type='voc',
-               image_folder='path/to/images',
-               ann_folder='path/to/annotations',
+        vf.to_coco(in_format='voc',
+               images='path/to/images',
+               annotations='path/to/annotations',
                class_file='path/to/classes.txt',
                output_file_path='path/to/output.json')
         ```
         For YOLO to COCO:
         ```python
-        import visualflow as vf
+        import VisualFlow as vf
         
-        vf.to_coco(input_type='yolo',
-               image_folder='path/to/images',
-               ann_folder='path/to/annotations',
+        vf.to_coco(in_format='yolo',
+               images='path/to/images',
+               annotations='path/to/annotations',
                class_file='path/to/classes.txt',
                output_file_path='path/to/output.json')
         ```
         
         Make sure to replace 'path/to/images', 'path/to/annotations', 'path/to/classes.txt', and 'path/to/output' with the actual paths to your dataset files and folders.
         
         ## Contributing
```

### Comparing `VisualFlow-0.1.4/setup.py` & `VisualFlow-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='VisualFlow',
-    version='0.1.4',
+    version='0.1.5',
     author='Ojas Sharma',
     author_email='ojassharma1607@gmail.com',
     description='A Python library for object detection format conversion',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Ojas-Sharma/VisualFlow',
     packages=find_packages(),
```

