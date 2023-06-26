# Comparing `tmp/dlc2kinematics-0.0.6.tar.gz` & `tmp/dlc2kinematics-0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlc2kinematics-0.0.6.tar", last modified: Mon Jun 26 20:40:11 2023, max compression
+gzip compressed data, was "dist/dlc2kinematics-0.0b1.tar", last modified: Sun Aug  8 20:17:03 2021, max compression
```

## Comparing `dlc2kinematics-0.0.6.tar` & `dlc2kinematics-0.0b1.tar`

### file list

```diff
@@ -1,59 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:11.151961 dlc2kinematics-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:11.139961 dlc2kinematics-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:11.143961 dlc2kinematics-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/.github/workflows/greetings.yml
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)  2229155 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/DEMO.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    94959 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/DEMO_c3d.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-06-26 20:40:11.151961 dlc2kinematics-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:11.143961 dlc2kinematics-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/docs/CLAC.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/docs/CLAI.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:11.147961 dlc2kinematics-0.0.6/docs/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      948 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/docs/scripts/autodoc.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      112 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/docs/scripts/module.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:11.147961 dlc2kinematics-0.0.6/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/examples/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   671373 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/examples/reachingDEMO_2D.h5
--rw-r--r--   0 runner    (1001) docker     (123)   671285 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/examples/reachingDEMO_3D.h5
--rw-r--r--   0 runner    (1001) docker     (123)   177432 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/examples/runway03.c3d
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      119 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/reinstall.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-26 20:40:11.151961 dlc2kinematics-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:11.139961 dlc2kinematics-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:11.151961 dlc2kinematics-0.0.6/src/dlc2kinematics/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/src/dlc2kinematics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:11.151961 dlc2kinematics-0.0.6/src/dlc2kinematics/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/src/dlc2kinematics/_tests/_init_.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/src/dlc2kinematics/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 20:40:11.000000 dlc2kinematics-0.0.6/src/dlc2kinematics/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/src/dlc2kinematics/joint_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/src/dlc2kinematics/mainfxns.py
--rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/src/dlc2kinematics/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/src/dlc2kinematics/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/src/dlc2kinematics/preprocess_c3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/src/dlc2kinematics/quaternions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:11.151961 dlc2kinematics-0.0.6/src/dlc2kinematics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/src/dlc2kinematics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/src/dlc2kinematics/utils/auxiliaryfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/src/dlc2kinematics/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15645 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/src/dlc2kinematics/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:11.151961 dlc2kinematics-0.0.6/src/dlc2kinematics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-06-26 20:40:11.000000 dlc2kinematics-0.0.6/src/dlc2kinematics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-26 20:40:11.000000 dlc2kinematics-0.0.6/src/dlc2kinematics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:40:11.000000 dlc2kinematics-0.0.6/src/dlc2kinematics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 20:40:11.000000 dlc2kinematics-0.0.6/src/dlc2kinematics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-26 20:40:11.000000 dlc2kinematics-0.0.6/src/dlc2kinematics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 20:40:11.000000 dlc2kinematics-0.0.6/src/dlc2kinematics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-26 20:39:50.000000 dlc2kinematics-0.0.6/tox.ini
+drwxr-xr-x   0 mwmathis   (501) staff       (20)        0 2021-08-08 20:17:03.000000 dlc2kinematics-0.0b1/
+-rw-r--r--   0 mwmathis   (501) staff       (20)     1112 2021-08-08 20:17:03.000000 dlc2kinematics-0.0b1/PKG-INFO
+-rw-r--r--   0 mwmathis   (501) staff       (20)      682 2021-08-08 20:00:21.000000 dlc2kinematics-0.0b1/README.md
+drwxr-xr-x   0 mwmathis   (501) staff       (20)        0 2021-08-08 20:17:03.000000 dlc2kinematics-0.0b1/dlc2kinematics/
+-rw-r--r--   0 mwmathis   (501) staff       (20)       87 2021-08-08 19:59:26.000000 dlc2kinematics-0.0b1/dlc2kinematics/__init__.py
+-rw-r--r--   0 mwmathis   (501) staff       (20)       20 2021-08-08 19:59:27.000000 dlc2kinematics-0.0b1/dlc2kinematics/version.py
+drwxr-xr-x   0 mwmathis   (501) staff       (20)        0 2021-08-08 20:17:03.000000 dlc2kinematics-0.0b1/dlc2kinematics.egg-info/
+-rw-r--r--   0 mwmathis   (501) staff       (20)     1112 2021-08-08 20:17:02.000000 dlc2kinematics-0.0b1/dlc2kinematics.egg-info/PKG-INFO
+-rw-r--r--   0 mwmathis   (501) staff       (20)      260 2021-08-08 20:17:02.000000 dlc2kinematics-0.0b1/dlc2kinematics.egg-info/SOURCES.txt
+-rw-r--r--   0 mwmathis   (501) staff       (20)        1 2021-08-08 20:17:02.000000 dlc2kinematics-0.0b1/dlc2kinematics.egg-info/dependency_links.txt
+-rw-r--r--   0 mwmathis   (501) staff       (20)      281 2021-08-08 20:17:02.000000 dlc2kinematics-0.0b1/dlc2kinematics.egg-info/requires.txt
+-rw-r--r--   0 mwmathis   (501) staff       (20)       15 2021-08-08 20:17:02.000000 dlc2kinematics-0.0b1/dlc2kinematics.egg-info/top_level.txt
+-rw-r--r--   0 mwmathis   (501) staff       (20)       38 2021-08-08 20:17:03.000000 dlc2kinematics-0.0b1/setup.cfg
+-rw-r--r--   0 mwmathis   (501) staff       (20)     1369 2021-08-08 19:59:05.000000 dlc2kinematics-0.0b1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `dlc2kinematics-0.0.6/setup.py` & `dlc2kinematics-0.0b1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,36 @@
 """
-dlc2kinematics
-© M. Mathis Lab
-https://github.com/AdaptiveMotorControlLab/dlc2kinematics/
+DLC2Kinematics Package
+© M. Mathis Labs
+https://github.com/AdaptiveMotorControlLab/DLC2Kinematics/
 
+Please see AUTHORS for contributors.
+https://github.com/AdaptiveMotorControlLab/DLC2Kinematics/blob/master/AUTHORS
 """
 
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dlc2kinematics",
-    version="0.0.6",
-    author="Mackenzie Mathis Lab Members",
+    version="0.0b1",
+    author="Mackenzie Mathis & Lab",
     author_email="mackenzie@post.harvard.edu",
-    description="Library for kinematic analysis of DeepLabCut outputs",
+    description="a post-DeepLabCut module for kinematic analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/AdaptiveMotorControlLab/dlc2kinematics/",
-    install_requires=[
-        "h5py",
-        "ipython",
-        "ipython-genutils",
-        "matplotlib>=3.0.3",
-        "numpy<1.25",
-        "pandas>=1.0",
-        "python-dateutil",
-        "pyyaml",
-        "requests",
-        "setuptools",
-        "scikit-image",
-        "scikit-learn<1.2.2",
-        "scikit-kinematics",
-        "scipy",
-        "tables",
-        "umap-learn",
-        "tqdm",
-        "ruamel.yaml>=0.15.0",
-        "wheel",
-    ],
+    url="https://github.com/AdaptiveMotorControlLab/DLC2Kinematics/",
+    install_requires=['h5py>=2.7','imageio>=2.3.0','intel-openmp',
+                      'ipython~=6.0.0','ipython-genutils==0.2.0',
+                      'matplotlib','moviepy','numpy','opencv-python',
+                      'pandas','patsy','python-dateutil','pyyaml>=5.1','requests',
+                      'ruamel.yaml>=0.15','setuptools','scikit-image','scikit-learn',
+                      'scikit-kinematics','scipy','six','statsmodels','tables',
+                      'tqdm>4','wheel'],
     packages=setuptools.find_packages(),
     include_package_data=True,
     classifiers=(
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
-    ),
-    entry_points="""[console_scripts]
-            kin=kin:main""",
-)
+))
```

