# Comparing `tmp/kerasfuse-0.1a0.tar.gz` & `tmp/kerasfuse-0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerasfuse-0.1a0.tar", max compression
+gzip compressed data, was "kerasfuse-0.1a1.tar", max compression
```

## Comparing `kerasfuse-0.1a0.tar` & `kerasfuse-0.1a1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    35149 2023-06-24 11:53:30.310712 kerasfuse-0.1a0/LICENSE
--rw-r--r--   0        0        0     2026 2023-06-24 11:53:30.310712 kerasfuse-0.1a0/README.md
--rw-r--r--   0        0        0      697 2023-06-24 11:53:30.310712 kerasfuse-0.1a0/kerasfuse/__init__.py
--rw-r--r--   0        0        0     4238 2023-06-24 11:53:30.310712 kerasfuse-0.1a0/kerasfuse/dataset/data_augmentation.py
--rw-r--r--   0        0        0     3015 2023-06-24 11:53:30.310712 kerasfuse-0.1a0/kerasfuse/dataset/generate_class_weights.py
--rw-r--r--   0        0        0     1781 2023-06-24 11:53:30.310712 kerasfuse-0.1a0/kerasfuse/dataset/load_images.py
--rw-r--r--   0        0        0     1192 2023-06-24 11:53:30.310712 kerasfuse-0.1a0/kerasfuse/evaluate.py
--rw-r--r--   0        0        0        0 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/losses/__init__.py
--rw-r--r--   0        0        0      502 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/losses/dice_loss.py
--rw-r--r--   0        0        0      697 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/losses/focal_loss.py
--rw-r--r--   0        0        0      973 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/losses/loss_functions.py
--rw-r--r--   0        0        0     3337 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/metrics/metrics.py
--rw-r--r--   0        0        0        0 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/models/__init__.py
--rw-r--r--   0        0        0        0 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/models/blocks/__init__.py
--rw-r--r--   0        0        0     7097 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/models/blocks/autoencoder.py
--rw-r--r--   0        0        0     2538 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/models/blocks/mlp.py
--rw-r--r--   0        0        0     2914 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/models/dense_net.py
--rw-r--r--   0        0        0    11069 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/models/layers/convutils.py
--rw-r--r--   0        0        0        6 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/models/layers/readme.md
--rw-r--r--   0        0        0     3776 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/models/mobile_net.py
--rw-r--r--   0        0        0     1785 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/models/res_net.py
--rw-r--r--   0        0        0     3070 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/models/u_net.py
--rw-r--r--   0        0        0     2476 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/models/v-net.py
--rw-r--r--   0        0        0     2654 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/train.py
--rw-r--r--   0        0        0     3182 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/pyproject.toml
--rw-r--r--   0        0        0     3429 1970-01-01 00:00:00.000000 kerasfuse-0.1a0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-24 14:27:41.811258 kerasfuse-0.1a1/LICENSE
+-rw-r--r--   0        0        0     3066 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/README.md
+-rw-r--r--   0        0        0      698 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/kerasfuse/__init__.py
+-rw-r--r--   0        0        0     4238 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/kerasfuse/dataset/data_augmentation.py
+-rw-r--r--   0        0        0     3015 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/kerasfuse/dataset/generate_class_weights.py
+-rw-r--r--   0        0        0     1781 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/kerasfuse/dataset/load_images.py
+-rw-r--r--   0        0        0     1192 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/kerasfuse/evaluate.py
+-rw-r--r--   0        0        0        0 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/kerasfuse/losses/__init__.py
+-rw-r--r--   0        0        0      502 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/kerasfuse/losses/dice_loss.py
+-rw-r--r--   0        0        0      697 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/kerasfuse/losses/focal_loss.py
+-rw-r--r--   0        0        0      973 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/kerasfuse/losses/loss_functions.py
+-rw-r--r--   0        0        0     3337 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/kerasfuse/metrics/metrics.py
+-rw-r--r--   0        0        0        0 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/kerasfuse/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/kerasfuse/models/blocks/__init__.py
+-rw-r--r--   0        0        0     7097 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/kerasfuse/models/blocks/autoencoder.py
+-rw-r--r--   0        0        0     2538 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/kerasfuse/models/blocks/mlp.py
+-rw-r--r--   0        0        0     2914 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/kerasfuse/models/dense_net.py
+-rw-r--r--   0        0        0    11069 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/kerasfuse/models/layers/convutils.py
+-rw-r--r--   0        0        0        6 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/kerasfuse/models/layers/readme.md
+-rw-r--r--   0        0        0     3776 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/kerasfuse/models/mobile_net.py
+-rw-r--r--   0        0        0     1785 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/kerasfuse/models/res_net.py
+-rw-r--r--   0        0        0     3070 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/kerasfuse/models/u_net.py
+-rw-r--r--   0        0        0     2476 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/kerasfuse/models/v-net.py
+-rw-r--r--   0        0        0     2654 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/kerasfuse/train.py
+-rw-r--r--   0        0        0     3183 2023-06-24 14:27:41.815258 kerasfuse-0.1a1/pyproject.toml
+-rw-r--r--   0        0        0     4469 1970-01-01 00:00:00.000000 kerasfuse-0.1a1/PKG-INFO
```

### Comparing `kerasfuse-0.1a0/LICENSE` & `kerasfuse-0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.1a0/kerasfuse/__init__.py` & `kerasfuse-0.1a1/kerasfuse/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-__version__ = "0.1a0"
+__version__ = "0.01a1"
```

### Comparing `kerasfuse-0.1a0/kerasfuse/dataset/data_augmentation.py` & `kerasfuse-0.1a1/kerasfuse/dataset/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.1a0/kerasfuse/dataset/generate_class_weights.py` & `kerasfuse-0.1a1/kerasfuse/dataset/generate_class_weights.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.1a0/kerasfuse/dataset/load_images.py` & `kerasfuse-0.1a1/kerasfuse/dataset/load_images.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.1a0/kerasfuse/evaluate.py` & `kerasfuse-0.1a1/kerasfuse/evaluate.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.1a0/kerasfuse/losses/focal_loss.py` & `kerasfuse-0.1a1/kerasfuse/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.1a0/kerasfuse/losses/loss_functions.py` & `kerasfuse-0.1a1/kerasfuse/losses/loss_functions.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.1a0/kerasfuse/metrics/metrics.py` & `kerasfuse-0.1a1/kerasfuse/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.1a0/kerasfuse/models/blocks/autoencoder.py` & `kerasfuse-0.1a1/kerasfuse/models/blocks/autoencoder.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.1a0/kerasfuse/models/blocks/mlp.py` & `kerasfuse-0.1a1/kerasfuse/models/blocks/mlp.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.1a0/kerasfuse/models/dense_net.py` & `kerasfuse-0.1a1/kerasfuse/models/dense_net.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.1a0/kerasfuse/models/layers/convutils.py` & `kerasfuse-0.1a1/kerasfuse/models/layers/convutils.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.1a0/kerasfuse/models/mobile_net.py` & `kerasfuse-0.1a1/kerasfuse/models/mobile_net.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.1a0/kerasfuse/models/res_net.py` & `kerasfuse-0.1a1/kerasfuse/models/res_net.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.1a0/kerasfuse/models/u_net.py` & `kerasfuse-0.1a1/kerasfuse/models/u_net.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.1a0/kerasfuse/models/v-net.py` & `kerasfuse-0.1a1/kerasfuse/models/v-net.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.1a0/kerasfuse/train.py` & `kerasfuse-0.1a1/kerasfuse/train.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.1a0/pyproject.toml` & `kerasfuse-0.1a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "KerasFuse"
-version = "0.1a0"
+version = "0.01a1"
 description = "KerasFuse is a Python library that combines the power of TensorFlow and Keras with various computer vision techniques for medical image analysis tasks."
 authors = ["Ayyuce Demirbas <a.ayyuced@gmail.com>"]
 maintainers = ["Ayyuce Demirbas <a.ayyuced@gmail.com>"]
 readme = "README.md"
 packages = [{include = "kerasfuse"}]
 homepage = "https://github.com/ayyucedemirbas/KerasFuse"
 repository = "https://github.com/ayyucedemirbas/KerasFuse"
```

### Comparing `kerasfuse-0.1a0/PKG-INFO` & `kerasfuse-0.1a1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kerasfuse
-Version: 0.1a0
+Version: 0.1a1
 Summary: KerasFuse is a Python library that combines the power of TensorFlow and Keras with various computer vision techniques for medical image analysis tasks.
 Home-page: https://github.com/ayyucedemirbas/KerasFuse
 Keywords: Tensorflow,Keras,KerasFuse
 Author: Ayyuce Demirbas
 Author-email: a.ayyuced@gmail.com
 Maintainer: Ayyuce Demirbas
 Maintainer-email: a.ayyuced@gmail.com
@@ -29,33 +29,64 @@
 
 <p align="center">
   <a href="https://github.com/ayyucedemirbas/KerasFuse"><img src="https://github.com/ayyucedemirbas/KerasFuse/assets/8023150/41d8880d-8117-448b-a725-2b72d2d08beb" alt="KerasFuse"></a>
 </p>
 
 <h1 align="center">KerasFuse</h1>
 
-<p>
+
+<p align="center">
   <img alt="GitHub" src="https://img.shields.io/github/license/ayyucedemirbas/Kerasfuse">
-  <img alt="Python3" src="https://img.shields.io/badge/Python-3.8.1 | 3.9 | 3.10 | 3.11-3776AB.svg?logo=Python&logoColor=white"/>
   <img alt="Tensorflow" src="https://img.shields.io/badge/Tensorflow-v2.12.0-%23FF6F00.svg?logo=Tensorflow&logoColor=white"/>
   <img alt="Keras" src="https://img.shields.io/badge/Keras-v2.12.0-%23D00000.svg?logo=Keras&logoColor=white"/>
   <img alt="Black" src="https://img.shields.io/badge/code%20style-black-black"/>
   <img alt="isort" src="https://img.shields.io/badge/isort-checked-yellow"/>
 </p>
+<p align="center">
+<a href="https://pypi.org/project/kerasfuse" target="_blank">
+    <img src="https://img.shields.io/pypi/v/kerasfuse?color=%2334D058&label=pypi%20package" alt="Package version">
+</a>
+<a href="https://pypi.org/project/kerasfuse" target="_blank">
+    <img src="https://img.shields.io/pypi/dm/kerasfuse?color=red" alt="Download Count">
+</a>
+<a href="https://pypi.org/project/kerasfuse" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/kerasfuse.svg?color=%2334D058" alt="Supported Python versions">
+</a>
+<a href="https://pypi.org/project/kerasfuse" target="_blank">
+    <img src="https://img.shields.io/pypi/status/kerasfuse?color=orange" alt="Project Status">
+</a>
+</p>
 
 <h4 align="center">🚧 Warning this project is under heavy development and not ready for production. ABI changes can happen frequently until reach stable version 🚧 </h4>
 
 
 KerasFuse is a Python library that combines the power of TensorFlow and Keras with various computer vision techniques for medical image analysis tasks. It provides a collection of modules and functions to facilitate the development of deep learning models in TensorFlow Keras for tasks such as image segmentation, classification, and more.
 
 
 
 ## Getting Started
 
-### Installation
+## Requirements
+
+KerasFuse is a project that relies heavily on the Tensorflow and Keras libraries. It is designed to work seamlessly with these powerful tools for deep learning and neural network development. In order to use KerasFuse effectively, please ensure that you have the following:
+
+* Python 3.8+
+* Tensorflow 2.12.0+ 
+* Keras 2.12.0+
+* OpenCV 4.7+
+* Scikit-Learn 1.2.2+
+
+## Installation
+
+```console
+$ pip install kerasfuse
+---> 100%
+```
+
+## Development 
 
 #### Poetry Installation
 
 ```bash
 poetry install
 poetry shell
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kerasfuse Version: 0.1a0 Summary: KerasFuse is a
+Metadata-Version: 2.1 Name: kerasfuse Version: 0.1a1 Summary: KerasFuse is a
 Python library that combines the power of TensorFlow and Keras with various
 computer vision techniques for medical image analysis tasks. Home-page: https:/
 /github.com/ayyucedemirbas/KerasFuse Keywords: Tensorflow,Keras,KerasFuse
 Author: Ayyuce Demirbas Author-email: a.ayyuced@gmail.com Maintainer: Ayyuce
 Demirbas Maintainer-email: a.ayyuced@gmail.com Requires-Python: >=3.8.1,<3.12.0
 Classifier: Development Status :: 3 - Alpha Classifier: License :: OSI Approved
 :: GNU General Public License v3 or later (GPLv3+) Classifier: Natural Language
@@ -15,24 +15,31 @@
 Requires-Dist: tensorflow (>=2.12.0) ; sys_platform != "darwin" Requires-Dist:
 tensorflow-macos (>=2.12.0) ; sys_platform == "darwin" Project-URL:
 Documentation, https://github.com/ayyucedemirbas/KerasFuse/blob/main/README.md
 Project-URL: Repository, https://github.com/ayyucedemirbas/KerasFuse
 Description-Content-Type: text/markdown
                                   [KerasFuse]
                             ****** KerasFuse ******
-[GitHub] [Python3] [Tensorflow] [Keras] [Black] [isort]
+                 [GitHub] [Tensorflow] [Keras] [Black] [isort]
+[Package_version] [Download_Count] [Supported_Python_versions] [Project_Status]
   *** ð§ Warning this project is under heavy development and not ready for
  production. ABI changes can happen frequently until reach stable version ð§
                                       ***
 KerasFuse is a Python library that combines the power of TensorFlow and Keras
 with various computer vision techniques for medical image analysis tasks. It
 provides a collection of modules and functions to facilitate the development of
 deep learning models in TensorFlow Keras for tasks such as image segmentation,
-classification, and more. ## Getting Started ### Installation #### Poetry
-Installation ```bash poetry install poetry shell ``` #### Tip If you have
-multiple Python versions on your system, you can set your Python version by
-using `poetry env` . Here's an example of how to use it: ```bash poetry env use
-python3.10 ``` More details at [poetry-switching-between-environments](https://
-python-poetry.org/docs/managing-environments/#switching-between-environments)
-#### Pip Installations ```bash python3 -m venv .venv source .venv/bin/activate
-pip3 install -r requirements.txt ``` ## License This project is licensed under
-the terms of the GPL-3.0 license.
+classification, and more. ## Getting Started ## Requirements KerasFuse is a
+project that relies heavily on the Tensorflow and Keras libraries. It is
+designed to work seamlessly with these powerful tools for deep learning and
+neural network development. In order to use KerasFuse effectively, please
+ensure that you have the following: * Python 3.8+ * Tensorflow 2.12.0+ * Keras
+2.12.0+ * OpenCV 4.7+ * Scikit-Learn 1.2.2+ ## Installation ```console $ pip
+install kerasfuse ---> 100% ``` ## Development #### Poetry Installation ```bash
+poetry install poetry shell ``` #### Tip If you have multiple Python versions
+on your system, you can set your Python version by using `poetry env` . Here's
+an example of how to use it: ```bash poetry env use python3.10 ``` More details
+at [poetry-switching-between-environments](https://python-poetry.org/docs/
+managing-environments/#switching-between-environments) #### Pip Installations
+```bash python3 -m venv .venv source .venv/bin/activate pip3 install -
+r requirements.txt ``` ## License This project is licensed under the terms of
+the GPL-3.0 license.
```

