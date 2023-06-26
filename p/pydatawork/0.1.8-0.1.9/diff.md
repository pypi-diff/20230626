# Comparing `tmp/pydatawork-0.1.8.tar.gz` & `tmp/pydatawork-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.1.8.tar", last modified: Sat Jun 24 10:07:12 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.1.9.tar", last modified: Sat Jun 24 10:41:02 2023, max compression
```

## Comparing `pydatawork-0.1.8.tar` & `pydatawork-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-24 10:07:12.000000 pydatawork-0.1.8/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     3707 2023-06-24 10:07:12.000000 pydatawork-0.1.8/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     2431 2023-06-24 09:58:59.000000 pydatawork-0.1.8/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-24 10:07:12.000000 pydatawork-0.1.8/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     3707 2023-06-24 10:07:12.000000 pydatawork-0.1.8/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-24 10:07:12.000000 pydatawork-0.1.8/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-24 10:07:12.000000 pydatawork-0.1.8/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-24 10:07:12.000000 pydatawork-0.1.8/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    10361 2023-06-24 09:32:45.000000 pydatawork-0.1.8/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-24 10:07:12.000000 pydatawork-0.1.8/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-24 09:59:20.000000 pydatawork-0.1.8/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-24 10:41:02.000000 pydatawork-0.1.9/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     4787 2023-06-24 10:41:02.000000 pydatawork-0.1.9/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     3383 2023-06-24 10:39:38.000000 pydatawork-0.1.9/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-24 10:41:02.000000 pydatawork-0.1.9/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     4787 2023-06-24 10:41:02.000000 pydatawork-0.1.9/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-24 10:41:02.000000 pydatawork-0.1.9/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-24 10:41:02.000000 pydatawork-0.1.9/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-24 10:41:02.000000 pydatawork-0.1.9/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    14474 2023-06-24 10:36:49.000000 pydatawork-0.1.9/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-24 10:41:02.000000 pydatawork-0.1.9/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-24 10:40:44.000000 pydatawork-0.1.9/setup.py
```

### Comparing `pydatawork-0.1.8/PKG-INFO` & `pydatawork-0.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,34 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.1.8
+Version: 0.1.9
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         
         
+        ###### Sat Jun 24 18:37:16 CST 2023
+        
+        #### move_obsidian_md_or_canvas_linked_images() 移动obsidian中.md文档、.canvas文档及文档中链接的图片，实现附件管理、库空间管理、笔记归档 (v 0.1.9)
+        
+        ```python
+        def move_obsidian_md_or_canvas_linked_images(images_path,folder_path,target_folder):
+            """
+            移动obsidian中.md文档、.canvas文档及文档中链接的图片，实现附件管理、库空间管理、笔记归档。
+            需要指定三个路径：
+            images_path:图片附件所在的文件夹。通常是笔记库的附件文件夹
+            folder_path:待移动、待整理的md、canvas文档所在文件夹。通常临时建立一个文件夹,将要移动的文件存放进去
+            target_folder:提前准备的文件夹，可以建立在folder_path中，用于存放那个提取出来的图片
+            执行结束后，可以将文档和对应的图片一起进行归档，实现笔记管理的目的。
+            """
+        ```
+        
         ###### Sun Jun 18 23:34:45 CST 2023
         
         #### hello_jkzhou() Always grow together（v 0.1.7）
         
         ```python
         def hello_jkzhou():
             """If you need help or have a better idea, send me an e-mail."""
```

### Comparing `pydatawork-0.1.8/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.1.9/pydatawork.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,34 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.1.8
+Version: 0.1.9
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         
         
+        ###### Sat Jun 24 18:37:16 CST 2023
+        
+        #### move_obsidian_md_or_canvas_linked_images() 移动obsidian中.md文档、.canvas文档及文档中链接的图片，实现附件管理、库空间管理、笔记归档 (v 0.1.9)
+        
+        ```python
+        def move_obsidian_md_or_canvas_linked_images(images_path,folder_path,target_folder):
+            """
+            移动obsidian中.md文档、.canvas文档及文档中链接的图片，实现附件管理、库空间管理、笔记归档。
+            需要指定三个路径：
+            images_path:图片附件所在的文件夹。通常是笔记库的附件文件夹
+            folder_path:待移动、待整理的md、canvas文档所在文件夹。通常临时建立一个文件夹,将要移动的文件存放进去
+            target_folder:提前准备的文件夹，可以建立在folder_path中，用于存放那个提取出来的图片
+            执行结束后，可以将文档和对应的图片一起进行归档，实现笔记管理的目的。
+            """
+        ```
+        
         ###### Sun Jun 18 23:34:45 CST 2023
         
         #### hello_jkzhou() Always grow together（v 0.1.7）
         
         ```python
         def hello_jkzhou():
             """If you need help or have a better idea, send me an e-mail."""
```

### Comparing `pydatawork-0.1.8/pydatawork.py` & `pydatawork-0.1.9/pydatawork.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 
 # -*- coding: utf-8 -*-
 import urllib.request
 import json
 import requests
 import os
+import shutil
+import re
 
 
 
 # def break_words(stuff):
 #     """This function will break up words for us."""
 #     words = stuff.split(' ')
 #     return words
@@ -219,12 +221,75 @@
     for i, folder in enumerate(subfolders, start=1): # 遍历排序后的子文件夹，从1开始序列化 @ 知识卡片
         new_name = f"{folder}_{i}" # 将序列化的值加在原文件名末尾，以_进行拼接
         os.rename(folder, new_name) # 重命名文件夹 @ 知识卡片
         print(os.path.basename(new_name)) # 打印重命名后的文件夹名字，不包括路径
 
 
 
+def move_obsidian_md_or_canvas_linked_images(images_path,folder_path,target_folder):
+    """
+    移动obsidian中.md文档、.canvas文档及文档中链接的图片，实现附件管理、库空间管理、笔记归档。
+    需要指定三个路径：
+    images_path:图片附件所在的文件夹。通常是笔记库的附件文件夹
+    folder_path:待移动、待整理的md、canvas文档所在文件夹。通常临时建立一个文件夹,将要移动的文件存放进去
+    target_folder:提前准备的文件夹，可以建立在folder_path中，用于存放那个提取出来的图片
+    执行结束后，可以将文档和对应的图片一起进行归档，实现笔记管理的目的。
+    """
+
+    # 001-图片文件夹:原始库的附件文件夹路径
+    images_path = "/home/jkzhou/Desktop/手机笔记同步-附件"
+    # 002-文件夹路径：准备移动归档的文件夹，里面包含.md和.canvas格式的文件
+    folder_path = "/home/jkzhou/Desktop/file"
+    # 003-图片移动的目标文件夹：通常，在002中建立一个文件夹，用于存放图片即可
+    target_folder = "/home/jkzhou/Desktop/file/附件"
+
+    for root, dirs, files in os.walk(folder_path):
+        for file in files:
+            if file.endswith(".md"):
+            # 将md文件打印出来
+                print(file)
+            # 处理markdown文档
+                with open(os.path.join(root, file), "r", encoding="utf-8") as f:
+                    content = f.read()
+                    # 查找文档中的图片
+                    images = re.findall(r"\!\[\[(.*?)\]\]", content) # @@知识卡片 正则匹配
+                    # exit()
+                    for image_name in images:
+                        # 在images文件夹中查找对应图片
+                        for image_root, _, image_files in os.walk(images_path):
+                            if image_name in image_files:
+                                # 移动图片到指定文件夹
+                                shutil.move(os.path.join(image_root, image_name), os.path.join(target_folder, image_name))
+                                # 打印移动过程
+                                print(f"moving:{os.path.join(image_root, image_name)}--->{os.path.join(target_folder, image_name)}")
+            # exit()
+
+            # 处理canvas文档
+            elif file.endswith(".canvas"):
+                # 将canvas文件打印出来
+                print(file)
+                with open(os.path.join(root, file), "r", encoding="utf-8") as f:
+                    content = f.read() # @知识卡片 不必非用json的读取方式
+                    # 查找文档中的图片
+                    # images = re.findall(r'"file":"(.*?\.png)"', content) # @知识卡片 匹配形如"file":"Pasted image 20230531214326.png"的字符串，得到的是绝对路径
+                    images = re.findall(r'"file":"(.*?)"', content) # @知识卡片 匹配形如"file":"Pasted image 20230531214326.png"的字符串，得到的是绝对路径。不用指定png、jpeg等格式。
+                    # print(images)
+                    for file_path in images:
+                        # print(file_path)
+                        image_name = os.path.basename(file_path) #  @知识卡片 从绝对路径中提取文件名。Pasted image 20230531214326.png
+                        # 在images文件夹中查找对应图片
+                        for image_root, _, image_files in os.walk(images_path):
+                            if image_name in image_files:
+                                # 移动图片到指定文件夹
+                                shutil.move(os.path.join(image_root, image_name), os.path.join(target_folder, image_name))
+                                # 打印移动过程
+                                print(f"moving:{os.path.join(image_root, image_name)}--->{os.path.join(target_folder, image_name)}")
+
+    # 统计附件整理情况
+    images_list = os.listdir(target_folder)
+    num_images = len(images_list)
 
+    print(f"\n已整理{num_images}个附件！")
```

### Comparing `pydatawork-0.1.8/setup.py` & `pydatawork-0.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.1.8',
+    version='0.1.9',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

