# Comparing `tmp/non-normal-0.1.1.tar.gz` & `tmp/non-normal-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "non-normal-0.1.1.tar", last modified: Sat Jun 24 10:17:00 2023, max compression
+gzip compressed data, was "non-normal-0.1.2.tar", last modified: Mon Jun 26 01:48:19 2023, max compression
```

## Comparing `non-normal-0.1.1.tar` & `non-normal-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-06-23 01:17:01.052831 non-normal-0.1.1/LICENSE
--rw-r--r--   0        0        0     1281 2023-06-24 10:15:57.209438 non-normal-0.1.1/README.md
--rw-r--r--   0        0        0     1022 2023-06-24 09:25:44.267393 non-normal-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       51 2023-06-24 09:26:10.655648 non-normal-0.1.1/src/non_normal/__init__.py
--rw-r--r--   0        0        0     7007 2023-06-24 10:04:12.771991 non-normal-0.1.1/src/non_normal/fleishman.py
--rw-r--r--   0        0        0     2126 2023-06-24 10:17:00.639711 non-normal-0.1.1/setup.py
--rw-r--r--   0        0        0     1964 2023-06-24 10:17:00.639967 non-normal-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-23 01:17:01.052831 non-normal-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2203 2023-06-26 01:46:59.456960 non-normal-0.1.2/README.md
+-rw-r--r--   0        0        0     1022 2023-06-26 01:47:43.968800 non-normal-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-06-26 01:47:57.402821 non-normal-0.1.2/src/non_normal/__init__.py
+-rw-r--r--   0        0        0     6988 2023-06-26 01:46:55.353347 non-normal-0.1.2/src/non_normal/fleishman.py
+-rw-r--r--   0        0        0     3057 2023-06-26 01:48:19.968865 non-normal-0.1.2/setup.py
+-rw-r--r--   0        0        0     2886 2023-06-26 01:48:19.969105 non-normal-0.1.2/PKG-INFO
```

### Comparing `non-normal-0.1.1/LICENSE` & `non-normal-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `non-normal-0.1.1/pyproject.toml` & `non-normal-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "non-normal"
-version = "0.1.1"
+version = "0.1.2"
 description = "Generate non-normal distributions with known mean, variance, skewness and kurtosis"
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/<your-username>/hypermodern-python"
 repository = "https://github.com/<your-username>/hypermodern-python"
 keywords = ["non-normal", "fleishman", "distribution", "statistics"]
```

### Comparing `non-normal-0.1.1/src/non_normal/fleishman.py` & `non-normal-0.1.2/src/non_normal/fleishman.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
     References
     ----------
         - https://link.springer.com/article/10.1007/BF02293811
         - https://support.sas.com/content/dam/SAS/support/en/books/simulating-data-with-sas/65378_Appendix_D_Functions_for_Simulating_Data_by_Using_Fleishmans_Transformation.pdf
         - https://www.diva-portal.org/smash/get/diva2:407995/FULLTEXT01.pd
         - https://pubmed.ncbi.nlm.nih.gov/34779511/
-        - https://gist.github.com/paddymccrudden/de5ab688b0d93e204098f03ccc211d88
+        - https://gist.github.com/zeimusu/7432603b85dc6406c6ea
         - https://link.springer.com/article/10.1007/BF02293687
     """
 
     def __init__(
         self,
         size=2**20,
         mean=0,
```

### Comparing `non-normal-0.1.1/setup.py` & `non-normal-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.25.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'non-normal',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Generate non-normal distributions with known mean, variance, skewness and kurtosis',
-    'long_description': "# non-normal\nGenerate a non-normal distributions with given a mean, variance, skewness and kurtosis using\nthe [Fleishman Method](https://link.springer.com/article/10.1007/BF02293811),\nessentially a cubic transformation on a standard normal [X~N(0, 1)]\n\n$$\nY =a +bX +cX^2 +dX^3\n$$\n\nwhere the coefficients ($a, b, c, d$) are tuned to create a distribution\nwith the desired statistic\n\n![Non-Normal Distribution](./docs/imgs/banner.png)\nFigure 1. A non-normal field generated in the `usage` section below. The title\nshows the input parameters, and the emperically measured statistics of the \ngenerated distribution\n\n### Installation\n\nInstalls cleanly with a single invocation of the standard Python package tool:\n\n```\n$ pip install non-normal\n```\n\n### Usage\n\n```\nfrom non_normal import fleishman\n\n# Input parameters for non-normal field\nmean = 0\nvar = 1\nskew = 1\nekurt = 2\nsize = 2**20\n\n# Create an instance of the Fleishman class\nff = fleishman.Fleishman(mean=mean, var=var, skew=skew, ekurt=ekurt, size=size)\n\n# Generate the field\nff.gen_field()\nnon_normal_data = ff.field\n\n# Measure the stats of the generated samples\nff.field_stats\n\n>>> {'mean':    0.000203128504124, \n     'var':     1.001352686678266, \n     'skew':    1.005612915524984, \n     'ekurt':   2.052527629375554,}\n```\n",
+    'long_description': "# non-normal\nGenerate a non-normal distributions with given a mean, variance, skewness and kurtosis using\nthe [Fleishman Method](https://link.springer.com/article/10.1007/BF02293811),\nessentially a cubic transformation on a standard normal [X~N(0, 1)]\n\n$$\nY =a +bX +cX^2 +dX^3\n$$\n\nwhere the coefficients ($a, b, c, d$) are tuned to create a distribution\nwith the desired statistic\n\n![Non-Normal Distribution](https://raw.githubusercontent.com/amanchokshi/non-normal/main/docs/imgs/banner.png)\nFigure 1. A non-normal field generated in the `usage` section below. The title\nshows the input parameters, and the emperically measured statistics of the \ngenerated distribution\n\n### Installation\n\nInstalls cleanly with a single invocation of the standard Python package tool:\n\n```\n$ pip install non-normal\n```\n\n### Usage\n\n```\nfrom non_normal import fleishman\n\n# Input parameters for non-normal field\nmean = 0\nvar = 1\nskew = 1\nekurt = 2\nsize = 2**20\n\n# Create an instance of the Fleishman class\nff = fleishman.Fleishman(mean=mean, var=var, skew=skew, ekurt=ekurt, size=size)\n\n# Generate the field\nff.gen_field()\nnon_normal_data = ff.field\n\n# Measure the stats of the generated samples\nff.field_stats\n\n>>> {'mean':    0.000203128504124, \n     'var':     1.001352686678266, \n     'skew':    1.005612915524984, \n     'ekurt':   2.052527629375554,}\n```\n\n### References\n\n1. [A method for simulating non-normal distributions](https://link.springer.com/article/10.1007/BF02293811)\n2. [Functions for Simulating Data by Using Fleishman’s Transformation](https://support.sas.com/content/dam/SAS/support/en/books/simulating-data-with-sas/65378_Appendix_D_Functions_for_Simulating_Data_by_Using_Fleishmans_Transformation.pdf)\n3. [Generation of Non-normal Data – A Study of Fleishman’s Power Method](https://www.diva-portal.org/smash/get/diva2:407995/FULLTEXT01.pd)\n4. [Computing the real solutions of Fleishman's equations for simulating non-normal data](https://pubmed.ncbi.nlm.nih.gov/34779511/)\n5. [Simulating multivariate nonnormal distributions](https://link.springer.com/article/10.1007/BF02293687)\n6. [https://gist.github.com/zeimusu/7432603b85dc6406c6ea](https://gist.github.com/zeimusu/7432603b85dc6406c6ea)\n",
     'author': 'Aman Chokshi',
     'author_email': 'achokshi@student.unimelb.edu.au',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/<your-username>/hypermodern-python',
     'package_dir': package_dir,
     'packages': packages,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

