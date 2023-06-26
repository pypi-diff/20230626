# Comparing `tmp/raymics-0.5.9.tar.gz` & `tmp/raymics-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raymics-0.5.9.tar", last modified: Tue Apr  4 02:16:42 2023, max compression
+gzip compressed data, was "raymics-0.7.0.tar", last modified: Mon Jun 26 03:27:05 2023, max compression
```

## Comparing `raymics-0.5.9.tar` & `raymics-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-04-04 02:16:42.434664 raymics-0.5.9/
--rw-r--r--   0 john       (501) staff       (20)     5883 2023-04-04 02:16:42.434530 raymics-0.5.9/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)     5768 2023-03-23 07:26:30.000000 raymics-0.5.9/README.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-04-04 02:16:42.433528 raymics-0.5.9/raymics/
--rw-r--r--   0 john       (501) staff       (20)       47 2022-09-28 06:59:47.000000 raymics-0.5.9/raymics/__init__.py
--rw-r--r--   0 john       (501) staff       (20)      727 2023-01-09 05:52:34.000000 raymics-0.5.9/raymics/constants.py
--rw-r--r--   0 john       (501) staff       (20)     3921 2023-01-09 07:38:14.000000 raymics-0.5.9/raymics/dataset.py
--rw-r--r--   0 john       (501) staff       (20)    17432 2023-04-04 02:14:26.000000 raymics-0.5.9/raymics/extract_radiomics_features.py
--rw-r--r--   0 john       (501) staff       (20)      232 2023-04-04 02:15:26.000000 raymics-0.5.9/raymics/log.py
--rw-r--r--   0 john       (501) staff       (20)     5569 2022-09-28 05:46:07.000000 raymics-0.5.9/raymics/task.py
--rw-r--r--   0 john       (501) staff       (20)     2477 2022-10-19 09:11:40.000000 raymics-0.5.9/raymics/utils.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-04-04 02:16:42.434378 raymics-0.5.9/raymics.egg-info/
--rw-r--r--   0 john       (501) staff       (20)     5883 2023-04-04 02:16:42.000000 raymics-0.5.9/raymics.egg-info/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      318 2023-04-04 02:16:42.000000 raymics-0.5.9/raymics.egg-info/SOURCES.txt
--rw-r--r--   0 john       (501) staff       (20)        1 2023-04-04 02:16:42.000000 raymics-0.5.9/raymics.egg-info/dependency_links.txt
--rw-r--r--   0 john       (501) staff       (20)      101 2023-04-04 02:16:42.000000 raymics-0.5.9/raymics.egg-info/requires.txt
--rw-r--r--   0 john       (501) staff       (20)        8 2023-04-04 02:16:42.000000 raymics-0.5.9/raymics.egg-info/top_level.txt
--rw-r--r--   0 john       (501) staff       (20)       38 2023-04-04 02:16:42.434698 raymics-0.5.9/setup.cfg
--rw-r--r--   0 john       (501) staff       (20)      608 2023-04-04 02:16:24.000000 raymics-0.5.9/setup.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 03:27:05.033511 raymics-0.7.0/
+-rw-r--r--   0 john       (501) staff       (20)     6128 2023-06-26 03:27:05.033317 raymics-0.7.0/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)     6013 2023-06-25 03:11:09.000000 raymics-0.7.0/README.md
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 03:27:05.032586 raymics-0.7.0/raymics/
+-rw-r--r--   0 john       (501) staff       (20)       47 2023-06-25 03:11:09.000000 raymics-0.7.0/raymics/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)      727 2023-06-25 03:11:09.000000 raymics-0.7.0/raymics/constants.py
+-rw-r--r--   0 john       (501) staff       (20)     3921 2023-06-25 03:11:09.000000 raymics-0.7.0/raymics/dataset.py
+-rw-r--r--   0 john       (501) staff       (20)    21616 2023-06-26 03:12:52.000000 raymics-0.7.0/raymics/extract_radiomics_features.py
+-rw-r--r--   0 john       (501) staff       (20)      232 2023-06-25 03:11:09.000000 raymics-0.7.0/raymics/log.py
+-rw-r--r--   0 john       (501) staff       (20)     5569 2023-06-25 03:11:09.000000 raymics-0.7.0/raymics/task.py
+-rw-r--r--   0 john       (501) staff       (20)     2477 2023-06-25 03:11:09.000000 raymics-0.7.0/raymics/utils.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 03:27:05.033149 raymics-0.7.0/raymics.egg-info/
+-rw-r--r--   0 john       (501) staff       (20)     6128 2023-06-26 03:27:04.000000 raymics-0.7.0/raymics.egg-info/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      318 2023-06-26 03:27:05.000000 raymics-0.7.0/raymics.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2023-06-26 03:27:04.000000 raymics-0.7.0/raymics.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (501) staff       (20)      193 2023-06-26 03:27:04.000000 raymics-0.7.0/raymics.egg-info/requires.txt
+-rw-r--r--   0 john       (501) staff       (20)        8 2023-06-26 03:27:04.000000 raymics-0.7.0/raymics.egg-info/top_level.txt
+-rw-r--r--   0 john       (501) staff       (20)       38 2023-06-26 03:27:05.033565 raymics-0.7.0/setup.cfg
+-rw-r--r--   0 john       (501) staff       (20)      608 2023-06-26 03:14:44.000000 raymics-0.7.0/setup.py
```

### Comparing `raymics-0.5.9/PKG-INFO` & `raymics-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 Metadata-Version: 2.1
 Name: raymics
-Version: 0.5.9
+Version: 0.7.0
 Summary: Raymics Tools
 Description-Content-Type: text/markdown
 
 # 提取Radiomics特征
 
 ## 1. 安装特征提取工具包
 
 
 ```python
 !pip install --upgrade raymics
 ```
 
     Looking in indexes: https://pypi.org/simple, https://pypi.ngc.nvidia.com
-    Collecting raymics
-      Downloading raymics-0.5.5-py3-none-any.whl (13 kB)
-    Requirement already satisfied: av in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (10.0.0)
-    Requirement already satisfied: tqdm in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (4.64.1)
-    Requirement already satisfied: SimpleITK in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (2.2.1)
-    Requirement already satisfied: pandas in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (1.5.2)
+    Requirement already satisfied: raymics in /Users/john/PycharmProjects/raymics-python/raymics (0.5.9)
     Requirement already satisfied: numpy in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (1.22.4)
-    Requirement already satisfied: opencv-contrib-python in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (4.7.0.68)
+    Requirement already satisfied: pandas in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (1.5.2)
+    Requirement already satisfied: tqdm in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (4.64.1)
     Requirement already satisfied: imageio in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (2.24.0)
+    Requirement already satisfied: av in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (10.0.0)
+    Requirement already satisfied: SimpleITK in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (2.2.1)
     Requirement already satisfied: pyradiomics in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (3.0.1)
+    Requirement already satisfied: opencv-contrib-python in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (4.7.0.68)
     Requirement already satisfied: dicom2nifti in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (2.4.7)
-    Requirement already satisfied: scipy in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from dicom2nifti->raymics) (1.10.0)
     Requirement already satisfied: python-gdcm in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from dicom2nifti->raymics) (3.0.20)
     Requirement already satisfied: pydicom>=2.2.0 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from dicom2nifti->raymics) (2.3.1)
+    Requirement already satisfied: scipy in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from dicom2nifti->raymics) (1.10.0)
     Requirement already satisfied: nibabel in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from dicom2nifti->raymics) (4.0.2)
     Requirement already satisfied: pillow>=8.3.2 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from imageio->raymics) (9.4.0)
-    Requirement already satisfied: imageio-ffmpeg in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from imageio->raymics) (0.4.8)
     Requirement already satisfied: psutil in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from imageio->raymics) (5.9.4)
+    Requirement already satisfied: imageio-ffmpeg in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from imageio->raymics) (0.4.8)
     Requirement already satisfied: python-dateutil>=2.8.1 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pandas->raymics) (2.8.2)
     Requirement already satisfied: pytz>=2020.1 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pandas->raymics) (2022.7)
     Requirement already satisfied: PyWavelets>=0.4.0 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pyradiomics->raymics) (1.4.1)
     Requirement already satisfied: pykwalify>=1.6.0 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pyradiomics->raymics) (1.8.0)
     Requirement already satisfied: six>=1.10.0 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pyradiomics->raymics) (1.16.0)
-    Requirement already satisfied: docopt>=0.6.2 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pykwalify>=1.6.0->pyradiomics->raymics) (0.6.2)
     Requirement already satisfied: ruamel.yaml>=0.16.0 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pykwalify>=1.6.0->pyradiomics->raymics) (0.17.21)
+    Requirement already satisfied: docopt>=0.6.2 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pykwalify>=1.6.0->pyradiomics->raymics) (0.6.2)
     Requirement already satisfied: packaging>=17.0 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from nibabel->dicom2nifti->raymics) (22.0)
     Requirement already satisfied: setuptools in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from nibabel->dicom2nifti->raymics) (67.6.0)
     Requirement already satisfied: ruamel.yaml.clib>=0.2.6 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from ruamel.yaml>=0.16.0->pykwalify>=1.6.0->pyradiomics->raymics) (0.2.7)
-    Installing collected packages: raymics
-    Successfully installed raymics-0.5.5
 
 
 ## 2. 设定提取特征的选项
 按照实际文件路径修改下面变量：
 
 
 ```python
@@ -63,28 +60,37 @@
 ## 3. 执行特征提取
 
 
 ```python
 extract(dataset_dir=dataset_dir, config=config_path, result_dir=result_dir, processes=processes);
 ```
 
-    labels.csv with 182 rows and 4 columns: data_id, data_path, mask_path, label
+    100%|███████████████████████████████████████████████████████████████████████████████████████| 2/2 [00:07<00:00,  3.84s/it]
+
 
+注意，如果已经完成radiomics特征数据的提取，再次执行时会给出提示并终止执行，如下所示：
+
+
+```python
+extract(dataset_dir=dataset_dir, config=config_path, result_dir=result_dir, processes=processes);
+```
 
-    100%|███████████████████████████████████████████████████████████████████████████████████████| 2/2 [00:07<00:00,  3.83s/it]
+    2023-04-04 10:17:46 [ERROR] raymics.log - The result dir './radiomics_feature_data' is not empty with files:
+    - labels.csv
+    - features.csv
 
 
 ## 4.  特征数据输出
 
 在特征数据文件夹中会生成特征数据，如下所示(如不支持tree命令，可以直接到特征数据文件夹查看)：
 
 
 ```python
 !tree ./radiomics_feature_data    # 使用实际特征文件夹路径替换
 ```
 
-    [01;34m/tmp/radiomics_feature_data[0m
+    [01;34m./radiomics_feature_data[0m
     ├── [00mfeatures.csv[0m
     └── [00mlabels.csv[0m
     
     0 directories, 2 files
```

### Comparing `raymics-0.5.9/README.md` & `raymics-0.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,44 +4,41 @@
 
 
 ```python
 !pip install --upgrade raymics
 ```
 
     Looking in indexes: https://pypi.org/simple, https://pypi.ngc.nvidia.com
-    Collecting raymics
-      Downloading raymics-0.5.5-py3-none-any.whl (13 kB)
-    Requirement already satisfied: av in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (10.0.0)
-    Requirement already satisfied: tqdm in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (4.64.1)
-    Requirement already satisfied: SimpleITK in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (2.2.1)
-    Requirement already satisfied: pandas in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (1.5.2)
+    Requirement already satisfied: raymics in /Users/john/PycharmProjects/raymics-python/raymics (0.5.9)
     Requirement already satisfied: numpy in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (1.22.4)
-    Requirement already satisfied: opencv-contrib-python in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (4.7.0.68)
+    Requirement already satisfied: pandas in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (1.5.2)
+    Requirement already satisfied: tqdm in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (4.64.1)
     Requirement already satisfied: imageio in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (2.24.0)
+    Requirement already satisfied: av in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (10.0.0)
+    Requirement already satisfied: SimpleITK in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (2.2.1)
     Requirement already satisfied: pyradiomics in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (3.0.1)
+    Requirement already satisfied: opencv-contrib-python in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (4.7.0.68)
     Requirement already satisfied: dicom2nifti in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (2.4.7)
-    Requirement already satisfied: scipy in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from dicom2nifti->raymics) (1.10.0)
     Requirement already satisfied: python-gdcm in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from dicom2nifti->raymics) (3.0.20)
     Requirement already satisfied: pydicom>=2.2.0 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from dicom2nifti->raymics) (2.3.1)
+    Requirement already satisfied: scipy in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from dicom2nifti->raymics) (1.10.0)
     Requirement already satisfied: nibabel in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from dicom2nifti->raymics) (4.0.2)
     Requirement already satisfied: pillow>=8.3.2 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from imageio->raymics) (9.4.0)
-    Requirement already satisfied: imageio-ffmpeg in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from imageio->raymics) (0.4.8)
     Requirement already satisfied: psutil in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from imageio->raymics) (5.9.4)
+    Requirement already satisfied: imageio-ffmpeg in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from imageio->raymics) (0.4.8)
     Requirement already satisfied: python-dateutil>=2.8.1 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pandas->raymics) (2.8.2)
     Requirement already satisfied: pytz>=2020.1 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pandas->raymics) (2022.7)
     Requirement already satisfied: PyWavelets>=0.4.0 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pyradiomics->raymics) (1.4.1)
     Requirement already satisfied: pykwalify>=1.6.0 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pyradiomics->raymics) (1.8.0)
     Requirement already satisfied: six>=1.10.0 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pyradiomics->raymics) (1.16.0)
-    Requirement already satisfied: docopt>=0.6.2 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pykwalify>=1.6.0->pyradiomics->raymics) (0.6.2)
     Requirement already satisfied: ruamel.yaml>=0.16.0 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pykwalify>=1.6.0->pyradiomics->raymics) (0.17.21)
+    Requirement already satisfied: docopt>=0.6.2 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pykwalify>=1.6.0->pyradiomics->raymics) (0.6.2)
     Requirement already satisfied: packaging>=17.0 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from nibabel->dicom2nifti->raymics) (22.0)
     Requirement already satisfied: setuptools in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from nibabel->dicom2nifti->raymics) (67.6.0)
     Requirement already satisfied: ruamel.yaml.clib>=0.2.6 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from ruamel.yaml>=0.16.0->pykwalify>=1.6.0->pyradiomics->raymics) (0.2.7)
-    Installing collected packages: raymics
-    Successfully installed raymics-0.5.5
 
 
 ## 2. 设定提取特征的选项
 按照实际文件路径修改下面变量：
 
 
 ```python
@@ -57,28 +54,37 @@
 ## 3. 执行特征提取
 
 
 ```python
 extract(dataset_dir=dataset_dir, config=config_path, result_dir=result_dir, processes=processes);
 ```
 
-    labels.csv with 182 rows and 4 columns: data_id, data_path, mask_path, label
+    100%|███████████████████████████████████████████████████████████████████████████████████████| 2/2 [00:07<00:00,  3.84s/it]
+
 
+注意，如果已经完成radiomics特征数据的提取，再次执行时会给出提示并终止执行，如下所示：
+
+
+```python
+extract(dataset_dir=dataset_dir, config=config_path, result_dir=result_dir, processes=processes);
+```
 
-    100%|███████████████████████████████████████████████████████████████████████████████████████| 2/2 [00:07<00:00,  3.83s/it]
+    2023-04-04 10:17:46 [ERROR] raymics.log - The result dir './radiomics_feature_data' is not empty with files:
+    - labels.csv
+    - features.csv
 
 
 ## 4.  特征数据输出
 
 在特征数据文件夹中会生成特征数据，如下所示(如不支持tree命令，可以直接到特征数据文件夹查看)：
 
 
 ```python
 !tree ./radiomics_feature_data    # 使用实际特征文件夹路径替换
 ```
 
-    [01;34m/tmp/radiomics_feature_data[0m
+    [01;34m./radiomics_feature_data[0m
     ├── [00mfeatures.csv[0m
     └── [00mlabels.csv[0m
     
     0 directories, 2 files
```

### Comparing `raymics-0.5.9/raymics/constants.py` & `raymics-0.7.0/raymics/constants.py`

 * *Files identical despite different names*

### Comparing `raymics-0.5.9/raymics/dataset.py` & `raymics-0.7.0/raymics/dataset.py`

 * *Files identical despite different names*

### Comparing `raymics-0.5.9/raymics/extract_radiomics_features.py` & `raymics-0.7.0/raymics/extract_radiomics_features.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,23 +18,28 @@
 import tempfile
 import dicom2nifti
 import traceback
 
 from typing import List, Union, Tuple
 from multiprocessing import Manager, Pool
 from collections import OrderedDict
+from tsfresh import extract_features, select_features
+from tsfresh.feature_extraction import ComprehensiveFCParameters, MinimalFCParameters, EfficientFCParameters
+from tsfresh.utilities.dataframe_functions import impute
+
 from radiomics.featureextractor import RadiomicsFeatureExtractor
 from raymics import DatasetType
 from raymics.constants import COL_LABEL, RADIOMIC_FEATURE_FILENAME, COL_INDEX, \
     FILENAME_ANNOTATION, COL_DATA_PATH, COL_MASK_PATH, COL_ID
 from raymics.dataset import Dataset, LabeledDataset
 from raymics.utils import is_image, is_video, is_ndarray, is_labelme, \
     is_dicom_folder, isBase64
 from raymics.log import logger
 from radiomics.featureextractor import logger as rlogger
+
 rlogger.setLevel(logging.ERROR)
 
 GROUP_LEN = 100
 
 
 def pop_unnamed(df: pd.DataFrame) -> pd.DataFrame:
     unnamed_cols = [col for col in df.columns if col.startswith("Unnamed")]
@@ -243,17 +248,26 @@
                     os.path.join(tmpdir, f"{string.ascii_lowercase}.nii.gz")
                 dicom2nifti.dicom_series_to_nifti(data_path, tmp_img_path)
                 img = sitk.ReadImage(tmp_img_path)
 
         # try to read image using SimpleITK
         else:
             img = sitk.ReadImage(data_path)
+        h = img.GetHeight()
+        w = img.GetWidth()
+
+        try:
+            d = img.GetDepth()
+            shape = (h, w, d) if d != 0 else (h, w)
+        except:
+            shape = (h, w)
+
+        mask = get_mask(mask_path=mask_path, shape=shape)
 
-        mask = get_mask(mask_path=mask_path,
-                        shape=(img.GetHeight(), img.GetWidth()))
+        # shape=(img.GetHeight(), img.GetWidth()))
 
         # to avoiding ITK ERROR:
         # LabelStatisticsImageFilter(0x1263e0bb0): inputs do not occupy
         # the same physical space!
         mask.SetOrigin(img.GetOrigin())
         mask.SetSpacing(img.GetSpacing())
         mask.SetDirection(img.GetDirection())
@@ -321,15 +335,16 @@
         with lock:
             if not os.path.exists(result_labels_path):
                 result_labels_df = pd.read_csv(original_labels_path)
                 for col in [COL_ID, COL_DATA_PATH, COL_MASK_PATH]:
                     if col in result_labels_df:
                         result_labels_df.pop(col)
                 result_labels_df[COL_DATA_PATH] = None
-                result_labels_df[COL_INDEX] = list(range(result_labels_df.shape[0]))
+                result_labels_df[COL_INDEX] = list(
+                    range(result_labels_df.shape[0]))
                 result_labels_df.set_index(COL_INDEX)
             else:
                 result_labels_df = pd.read_csv(result_labels_path,
                                                index_col=COL_INDEX)
 
             rel_path = os.path.relpath(result_path, result_dir)
             result_labels_df.loc[data_idx, COL_DATA_PATH] = rel_path
@@ -365,42 +380,47 @@
 
     dataset = LabeledDataset(root_dir=dataset_dir)
 
     if not os.path.exists(result_dir):
         os.makedirs(result_dir)
     else:
         result_file_list = [_ for _ in os.listdir(result_dir)
-                            if not _.startswith(".") and not _.startswith("__")]
+                            if not _.startswith(".")
+                            and not _.startswith("__")
+                            and not _.endswith("pkl")]
         if len(result_file_list) > 0:
             file_list_string = '\n- '.join([""] + result_file_list)
-            logger.error(f"The result dir '{result_dir}' is not empty with files:{file_list_string}")
+            logger.error(
+                f"The result dir '{result_dir}' is not empty with files:{file_list_string}")
             logger.info("Please remove these files and try again!")
             return
 
     result_labels_path = os.path.join(result_dir, FILENAME_ANNOTATION)
 
     pool = Pool(processes=processes)
     extractor = RadiomicsFeatureExtractor(config)
     # force to output without additional info
     extractor.settings["additionalInfo"] = False
 
-    data_type = DatasetType.TS if is_video(dataset[0][2]) else DatasetType.NON_TS
+    data_type = DatasetType.TS if is_video(
+        dataset[0][2]) else DatasetType.NON_TS
 
     lock = Manager().Lock()
 
     # non-time series
     if data_type == DatasetType.NON_TS:
 
         idxs = list(range(len(dataset)))
         group_idxs = [idxs[i: i + GROUP_LEN]
                       for i in range(0, len(idxs), GROUP_LEN)]
         group_data_idxs = [dataset.data_idxs[i: i + GROUP_LEN]
                            for i in range(0, len(idxs), GROUP_LEN)]
 
-        for data_idxs, idx_list in tqdm.tqdm(list(zip(group_data_idxs, group_idxs))):
+        for data_idxs, idx_list in tqdm.tqdm(
+                list(zip(group_data_idxs, group_idxs))):
             extract_non_ts(data_idxs,
                            [dataset.data_ids[_] for _ in idx_list]
                            if dataset.data_ids else None,
                            [dataset.data_paths[_] for _ in idx_list],
                            [dataset.mask_paths[_] for _ in idx_list],
                            result_labels_path,
                            extractor,
@@ -483,14 +503,125 @@
                   [_ for _ in df.columns if _ != COL_DATA_PATH and
                    not _.startswith(COL_INDEX)]
         df[columns].to_csv(result_labels_path, index=False)
 
     return extractor
 
 
+def extract_radiomics(
+        dataset_dir: str,
+        result_dir: str,
+        fdr_level: int = 1,
+        is_feature_filter: bool = False,
+        feature_extracted_mode: str = "minimal_fc"
+):
+    """
+    tsfresh 扩展特征，筛选特征
+    """
+    def _transfer_label_index(labels: pd.Series):
+        _CLASSES_TO_IDX = {}
+        _CLASSES = sorted(list(set(labels)))
+        if len(_CLASSES) < 2:
+            logger.error(
+                f"Feature selection is only possible if more than 1 label/class"
+                f"is provided, _CLASSES is :{_CLASSES}")
+
+        _CLASSES_TO_IDX = {c: i for i, c in enumerate(_CLASSES)}
+        return _CLASSES_TO_IDX
+
+    def _read_csv(src_dir: str, dst_dir: str):
+        df = pd.read_csv(os.path.join(src_dir, FILENAME_ANNOTATION))
+
+        all_data_path = os.path.join(src_dir, "temp")
+        labels = df[COL_LABEL]
+        data_paths = df[COL_DATA_PATH]
+        for data_path, y in zip(data_paths, labels):
+            path = os.path.join(src_dir, data_path)
+            sub_df = pd.read_csv(path)
+            sub_df[COL_ID] = data_path.replace(".csv", "")
+            sub_df.to_csv(all_data_path, mode="a", index=False, header=not os.path.exists(all_data_path))
+
+        time_dataframe = pd.read_csv(all_data_path, low_memory=False)
+
+        if os.path.exists(all_data_path):
+            os.remove(all_data_path)
+
+        _CLASSES_TO_IDX = _transfer_label_index(labels)
+        data_id = df[COL_DATA_PATH].str.replace(".csv", "", regex=True)
+        _y = pd.Series(
+            np.array([_CLASSES_TO_IDX[l] for l in labels], dtype=np.int64),
+            index=data_id
+        )
+
+        # label to csv
+        df.rename(columns={COL_DATA_PATH: COL_ID}, inplace=True)
+        df[COL_ID] = data_id
+        if not os.path.exists(dst_dir):
+            os.makedirs(dst_dir)
+        df.to_csv(os.path.join(dst_dir, FILENAME_ANNOTATION), index=False)
+        return time_dataframe, _y
+
+    def _feature_filter(is_feature_filter, extracted_features, _y, fdr_level):
+        if is_feature_filter is False:
+            return extracted_features
+        impute(extracted_features)
+        features_filtered = select_features(
+            extracted_features,
+            _y,
+            fdr_level=fdr_level
+        )
+
+        if features_filtered.shape[1] <= 0:
+            logger.info(
+                f"sample count is zero after feature filtered,"
+                f"please check video data !"
+            )
+
+            features_filtered = extracted_features
+        return features_filtered
+
+    # csv io
+    time_dataframe, _y = _read_csv(
+        dataset_dir,
+        result_dir
+    )
+
+    if feature_extracted_mode == "comprehensive_fc":
+        fc_parameters = ComprehensiveFCParameters()
+    elif feature_extracted_mode == "efficient_fc":
+        fc_parameters = EfficientFCParameters()
+    else:
+        fc_parameters = MinimalFCParameters()
+
+    # 2.特征扩展
+    extracted_features = extract_features(
+        timeseries_container=time_dataframe,
+        column_id=COL_ID,
+        chunksize=None,
+        default_fc_parameters=dict(fc_parameters)
+    )
+    logger.info(
+        "extracted_features shape : {}".format(extracted_features.shape)
+    )
+
+    # 3.特征筛选
+    features_filtered = _feature_filter(
+        is_feature_filter,
+        extracted_features,
+        _y,
+        fdr_level)
+
+    logger.info("features filtered shape : {}".format(features_filtered.shape))
+
+    features_filtered.dropna(axis=1).to_csv(
+        os.path.join(result_dir, RADIOMIC_FEATURE_FILENAME), index=False)
+
+    logger.info(f"radiomics feature extension video end!")
+
+
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         "--dataset_dir",
         type=str,
         help="raw data dir"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `raymics-0.5.9/raymics/task.py` & `raymics-0.7.0/raymics/task.py`

 * *Files identical despite different names*

### Comparing `raymics-0.5.9/raymics/utils.py` & `raymics-0.7.0/raymics/utils.py`

 * *Files identical despite different names*

### Comparing `raymics-0.5.9/raymics.egg-info/PKG-INFO` & `raymics-0.7.0/raymics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 Metadata-Version: 2.1
 Name: raymics
-Version: 0.5.9
+Version: 0.7.0
 Summary: Raymics Tools
 Description-Content-Type: text/markdown
 
 # 提取Radiomics特征
 
 ## 1. 安装特征提取工具包
 
 
 ```python
 !pip install --upgrade raymics
 ```
 
     Looking in indexes: https://pypi.org/simple, https://pypi.ngc.nvidia.com
-    Collecting raymics
-      Downloading raymics-0.5.5-py3-none-any.whl (13 kB)
-    Requirement already satisfied: av in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (10.0.0)
-    Requirement already satisfied: tqdm in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (4.64.1)
-    Requirement already satisfied: SimpleITK in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (2.2.1)
-    Requirement already satisfied: pandas in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (1.5.2)
+    Requirement already satisfied: raymics in /Users/john/PycharmProjects/raymics-python/raymics (0.5.9)
     Requirement already satisfied: numpy in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (1.22.4)
-    Requirement already satisfied: opencv-contrib-python in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (4.7.0.68)
+    Requirement already satisfied: pandas in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (1.5.2)
+    Requirement already satisfied: tqdm in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (4.64.1)
     Requirement already satisfied: imageio in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (2.24.0)
+    Requirement already satisfied: av in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (10.0.0)
+    Requirement already satisfied: SimpleITK in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (2.2.1)
     Requirement already satisfied: pyradiomics in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (3.0.1)
+    Requirement already satisfied: opencv-contrib-python in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (4.7.0.68)
     Requirement already satisfied: dicom2nifti in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from raymics) (2.4.7)
-    Requirement already satisfied: scipy in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from dicom2nifti->raymics) (1.10.0)
     Requirement already satisfied: python-gdcm in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from dicom2nifti->raymics) (3.0.20)
     Requirement already satisfied: pydicom>=2.2.0 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from dicom2nifti->raymics) (2.3.1)
+    Requirement already satisfied: scipy in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from dicom2nifti->raymics) (1.10.0)
     Requirement already satisfied: nibabel in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from dicom2nifti->raymics) (4.0.2)
     Requirement already satisfied: pillow>=8.3.2 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from imageio->raymics) (9.4.0)
-    Requirement already satisfied: imageio-ffmpeg in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from imageio->raymics) (0.4.8)
     Requirement already satisfied: psutil in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from imageio->raymics) (5.9.4)
+    Requirement already satisfied: imageio-ffmpeg in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from imageio->raymics) (0.4.8)
     Requirement already satisfied: python-dateutil>=2.8.1 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pandas->raymics) (2.8.2)
     Requirement already satisfied: pytz>=2020.1 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pandas->raymics) (2022.7)
     Requirement already satisfied: PyWavelets>=0.4.0 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pyradiomics->raymics) (1.4.1)
     Requirement already satisfied: pykwalify>=1.6.0 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pyradiomics->raymics) (1.8.0)
     Requirement already satisfied: six>=1.10.0 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pyradiomics->raymics) (1.16.0)
-    Requirement already satisfied: docopt>=0.6.2 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pykwalify>=1.6.0->pyradiomics->raymics) (0.6.2)
     Requirement already satisfied: ruamel.yaml>=0.16.0 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pykwalify>=1.6.0->pyradiomics->raymics) (0.17.21)
+    Requirement already satisfied: docopt>=0.6.2 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from pykwalify>=1.6.0->pyradiomics->raymics) (0.6.2)
     Requirement already satisfied: packaging>=17.0 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from nibabel->dicom2nifti->raymics) (22.0)
     Requirement already satisfied: setuptools in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from nibabel->dicom2nifti->raymics) (67.6.0)
     Requirement already satisfied: ruamel.yaml.clib>=0.2.6 in /Users/john/.virtualenvs/venv_py3.10/lib/python3.10/site-packages (from ruamel.yaml>=0.16.0->pykwalify>=1.6.0->pyradiomics->raymics) (0.2.7)
-    Installing collected packages: raymics
-    Successfully installed raymics-0.5.5
 
 
 ## 2. 设定提取特征的选项
 按照实际文件路径修改下面变量：
 
 
 ```python
@@ -63,28 +60,37 @@
 ## 3. 执行特征提取
 
 
 ```python
 extract(dataset_dir=dataset_dir, config=config_path, result_dir=result_dir, processes=processes);
 ```
 
-    labels.csv with 182 rows and 4 columns: data_id, data_path, mask_path, label
+    100%|███████████████████████████████████████████████████████████████████████████████████████| 2/2 [00:07<00:00,  3.84s/it]
+
 
+注意，如果已经完成radiomics特征数据的提取，再次执行时会给出提示并终止执行，如下所示：
+
+
+```python
+extract(dataset_dir=dataset_dir, config=config_path, result_dir=result_dir, processes=processes);
+```
 
-    100%|███████████████████████████████████████████████████████████████████████████████████████| 2/2 [00:07<00:00,  3.83s/it]
+    2023-04-04 10:17:46 [ERROR] raymics.log - The result dir './radiomics_feature_data' is not empty with files:
+    - labels.csv
+    - features.csv
 
 
 ## 4.  特征数据输出
 
 在特征数据文件夹中会生成特征数据，如下所示(如不支持tree命令，可以直接到特征数据文件夹查看)：
 
 
 ```python
 !tree ./radiomics_feature_data    # 使用实际特征文件夹路径替换
 ```
 
-    [01;34m/tmp/radiomics_feature_data[0m
+    [01;34m./radiomics_feature_data[0m
     ├── [00mfeatures.csv[0m
     └── [00mlabels.csv[0m
     
     0 directories, 2 files
```

### Comparing `raymics-0.5.9/setup.py` & `raymics-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,14 @@
         with open(fname, 'r') as f:
             targets = f.read().splitlines()
     return targets
 
 
 setup(
     name="raymics",
-    version="0.5.9",
+    version="0.7.0",
     description="Raymics Tools",
     install_requires=get_install_requires(),
     packages=["raymics"],
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type='text/markdown'
 )
```

