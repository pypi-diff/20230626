# Comparing `tmp/madml-0.0.2.tar.gz` & `tmp/madml-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madml-0.0.2.tar", last modified: Mon Jun 26 15:57:07 2023, max compression
+gzip compressed data, was "madml-0.0.3.tar", last modified: Mon Jun 26 16:04:10 2023, max compression
```

## Comparing `madml-0.0.2.tar` & `madml-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 15:57:07.698796 madml-0.0.2/
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     1097 2023-06-26 14:22:33.000000 madml-0.0.2/LICENSE
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     3671 2023-06-26 15:57:07.698796 madml-0.0.2/PKG-INFO
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     3163 2023-06-26 15:04:33.000000 madml-0.0.2/README.md
-drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 15:57:07.694796 madml-0.0.2/madml.egg-info/
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     3671 2023-06-26 15:57:07.000000 madml-0.0.2/madml.egg-info/PKG-INFO
--rw-rw-r--   0 nerve     (1000) nerve     (1000)      227 2023-06-26 15:57:07.000000 madml-0.0.2/madml.egg-info/SOURCES.txt
--rw-rw-r--   0 nerve     (1000) nerve     (1000)        1 2023-06-26 15:57:07.000000 madml-0.0.2/madml.egg-info/dependency_links.txt
--rw-rw-r--   0 nerve     (1000) nerve     (1000)       78 2023-06-26 15:57:07.000000 madml-0.0.2/madml.egg-info/requires.txt
--rw-rw-r--   0 nerve     (1000) nerve     (1000)        1 2023-06-26 15:57:07.000000 madml-0.0.2/madml.egg-info/top_level.txt
--rw-rw-r--   0 nerve     (1000) nerve     (1000)      142 2023-06-26 15:56:15.000000 madml-0.0.2/pyproject.toml
--rw-rw-r--   0 nerve     (1000) nerve     (1000)       38 2023-06-26 15:57:07.698796 madml-0.0.2/setup.cfg
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     1531 2023-06-26 15:56:54.000000 madml-0.0.2/setup.py
-drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 15:57:07.694796 madml-0.0.2/tests/
--rw-rw-r--   0 nerve     (1000) nerve     (1000)      318 2023-06-26 14:22:33.000000 madml-0.0.2/tests/test_load_data.py
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     1899 2023-06-26 14:22:33.000000 madml-0.0.2/tests/test_run.py
+drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:04:10.467337 madml-0.0.3/
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     1097 2023-06-26 14:22:33.000000 madml-0.0.3/LICENSE
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     3690 2023-06-26 16:04:10.467337 madml-0.0.3/PKG-INFO
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     3182 2023-06-26 15:58:15.000000 madml-0.0.3/README.md
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)      142 2023-06-26 15:56:15.000000 madml-0.0.3/pyproject.toml
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)       38 2023-06-26 16:04:10.467337 madml-0.0.3/setup.cfg
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     1572 2023-06-26 16:04:02.000000 madml-0.0.3/setup.py
+drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:04:10.467337 madml-0.0.3/src/
+drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:04:10.467337 madml-0.0.3/src/madml.egg-info/
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     3690 2023-06-26 16:04:10.000000 madml-0.0.3/src/madml.egg-info/PKG-INFO
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)      247 2023-06-26 16:04:10.000000 madml-0.0.3/src/madml.egg-info/SOURCES.txt
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)        1 2023-06-26 16:04:10.000000 madml-0.0.3/src/madml.egg-info/dependency_links.txt
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)       78 2023-06-26 16:04:10.000000 madml-0.0.3/src/madml.egg-info/requires.txt
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)        1 2023-06-26 16:04:10.000000 madml-0.0.3/src/madml.egg-info/top_level.txt
+drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:04:10.467337 madml-0.0.3/tests/
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)      318 2023-06-26 14:22:33.000000 madml-0.0.3/tests/test_load_data.py
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     1899 2023-06-26 14:22:33.000000 madml-0.0.3/tests/test_run.py
```

### Comparing `madml-0.0.2/LICENSE` & `madml-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `madml-0.0.2/PKG-INFO` & `madml-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: madml
-Version: 0.0.2
+Version: 0.0.3
 Summary: Application domain of machine learning in materials science.
 Home-page: https://github.com/leschultz/materials_application_domain_machine_learning.git
 Author: Lane E. Schultz
 Author-email: laneenriqueschultz@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Materials Application Domain (MAD)
+# Materials Application Domain Machine Learning (MADML)
 
 Research with respect to application domain with a materials science emphasis is contained within. The GitHub repo can be found in [here](https://github.com/leschultz/application_domain.git).
 
 ## Structure
 The structure of the code packages is as follows:
 
 ```
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_7qqp7k92_/tmp1dg06bhm_TarContainer/0/2", line 99, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_7qqp7k92_/tmp1dg06bhm_TarContainer/0/2", line 99, column 0: CDATA terminal not found*

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: madml Version: 0.0.2 Summary: Application domain of
+Metadata-Version: 2.1 Name: madml Version: 0.0.3 Summary: Application domain of
 machine learning in materials science. Home-page: https://github.com/leschultz/
 materials_application_domain_machine_learning.git Author: Lane E. Schultz
 Author-email: laneenriqueschultz@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
-Type: text/markdown License-File: LICENSE # Materials Application Domain (MAD)
-Research with respect to application domain with a materials science emphasis
-is contained within. The GitHub repo can be found in [here](https://github.com/
-leschultz/application_domain.git). ## Structure The structure of the code
-packages is as follows: ``` materials_application_domain_machine_learning/
-âââ examples âÂ Â  âââ auto_push âÂ Â  âÂ Â  âââ fit.py
-âÂ Â  âÂ Â  âââ run.sh âÂ Â  âÂ Â  âââ submit.sh âÂ Â 
-âââ single_runs âÂ Â  âââ make_runs.sh âÂ Â  âââ
-submit_jobs.sh âÂ Â  âââ template âÂ Â  âââ fit.py âÂ Â 
-âââ run.sh âÂ Â  âââ submit.sh âââ LICENSE âââ
-pyproject.toml âââ README.md âââ setup.py âââ src âÂ Â 
-âââ madml âÂ Â  âââ data âÂ Â  âÂ Â  âââ
+Type: text/markdown License-File: LICENSE # Materials Application Domain
+Machine Learning (MADML) Research with respect to application domain with a
+materials science emphasis is contained within. The GitHub repo can be found in
+[here](https://github.com/leschultz/application_domain.git). ## Structure The
+structure of the code packages is as follows: ```
+materials_application_domain_machine_learning/ âââ examples âÂ Â 
+âââ auto_push âÂ Â  âÂ Â  âââ fit.py âÂ Â  âÂ Â  âââ
+run.sh âÂ Â  âÂ Â  âââ submit.sh âÂ Â  âââ single_runs
+âÂ Â  âââ make_runs.sh âÂ Â  âââ submit_jobs.sh âÂ Â 
+âââ template âÂ Â  âââ fit.py âÂ Â  âââ run.sh âÂ Â 
+âââ submit.sh âââ LICENSE âââ pyproject.toml âââ
+README.md âââ setup.py âââ src âÂ Â  âââ madml âÂ Â 
+âââ data âÂ Â  âÂ Â  âââ
 citrine_thermal_conductivity_simplified.xlsx âÂ Â  âÂ Â  âââ
 Dataset_electromigration.xlsx âÂ Â  âÂ Â  âââ
 Dataset_Perovskite_Opband_simplified.xlsx âÂ Â  âÂ Â  âââ
 dielectric_constant_simplified.xlsx âÂ Â  âÂ Â  âââ diffusion.csv
 âÂ Â  âÂ Â  âââ double_perovskites_gap.xlsx âÂ Â  âÂ Â  âââ
 elastic_tensor_2015_simplified.xlsx âÂ Â  âÂ Â  âââ fluence.csv
 âÂ Â  âÂ Â  âââ heusler_magnetic_simplified.xlsx âÂ Â  âÂ Â
```

### Comparing `madml-0.0.2/README.md` & `madml-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Materials Application Domain (MAD)
+# Materials Application Domain Machine Learning (MADML)
 
 Research with respect to application domain with a materials science emphasis is contained within. The GitHub repo can be found in [here](https://github.com/leschultz/application_domain.git).
 
 ## Structure
 The structure of the code packages is as follows:
 
 ```
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_7qqp7k92_/tmp1dg06bhm_TarContainer/0/3.md", line 85, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_7qqp7k92_/tmp1dg06bhm_TarContainer/0/3.md", line 85, column 0: CDATA terminal not found*

```diff
@@ -1,19 +1,19 @@
-# Materials Application Domain (MAD) Research with respect to application
-domain with a materials science emphasis is contained within. The GitHub repo
-can be found in [here](https://github.com/leschultz/application_domain.git). ##
-Structure The structure of the code packages is as follows: ```
-materials_application_domain_machine_learning/ âââ examples âÂ Â 
-âââ auto_push âÂ Â  âÂ Â  âââ fit.py âÂ Â  âÂ Â  âââ
-run.sh âÂ Â  âÂ Â  âââ submit.sh âÂ Â  âââ single_runs
-âÂ Â  âââ make_runs.sh âÂ Â  âââ submit_jobs.sh âÂ Â 
-âââ template âÂ Â  âââ fit.py âÂ Â  âââ run.sh âÂ Â 
-âââ submit.sh âââ LICENSE âââ pyproject.toml âââ
-README.md âââ setup.py âââ src âÂ Â  âââ madml âÂ Â 
-âââ data âÂ Â  âÂ Â  âââ
+# Materials Application Domain Machine Learning (MADML) Research with respect
+to application domain with a materials science emphasis is contained within.
+The GitHub repo can be found in [here](https://github.com/leschultz/
+application_domain.git). ## Structure The structure of the code packages is as
+follows: ``` materials_application_domain_machine_learning/ âââ examples
+âÂ Â  âââ auto_push âÂ Â  âÂ Â  âââ fit.py âÂ Â  âÂ Â 
+âââ run.sh âÂ Â  âÂ Â  âââ submit.sh âÂ Â  âââ
+single_runs âÂ Â  âââ make_runs.sh âÂ Â  âââ submit_jobs.sh
+âÂ Â  âââ template âÂ Â  âââ fit.py âÂ Â  âââ run.sh
+âÂ Â  âââ submit.sh âââ LICENSE âââ pyproject.toml
+âââ README.md âââ setup.py âââ src âÂ Â  âââ madml
+âÂ Â  âââ data âÂ Â  âÂ Â  âââ
 citrine_thermal_conductivity_simplified.xlsx âÂ Â  âÂ Â  âââ
 Dataset_electromigration.xlsx âÂ Â  âÂ Â  âââ
 Dataset_Perovskite_Opband_simplified.xlsx âÂ Â  âÂ Â  âââ
 dielectric_constant_simplified.xlsx âÂ Â  âÂ Â  âââ diffusion.csv
 âÂ Â  âÂ Â  âââ double_perovskites_gap.xlsx âÂ Â  âÂ Â  âââ
 elastic_tensor_2015_simplified.xlsx âÂ Â  âÂ Â  âââ fluence.csv
 âÂ Â  âÂ Â  âââ heusler_magnetic_simplified.xlsx âÂ Â  âÂ Â
```

### Comparing `madml-0.0.2/madml.egg-info/PKG-INFO` & `madml-0.0.3/src/madml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: madml
-Version: 0.0.2
+Version: 0.0.3
 Summary: Application domain of machine learning in materials science.
 Home-page: https://github.com/leschultz/materials_application_domain_machine_learning.git
 Author: Lane E. Schultz
 Author-email: laneenriqueschultz@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Materials Application Domain (MAD)
+# Materials Application Domain Machine Learning (MADML)
 
 Research with respect to application domain with a materials science emphasis is contained within. The GitHub repo can be found in [here](https://github.com/leschultz/application_domain.git).
 
 ## Structure
 The structure of the code packages is as follows:
 
 ```
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_7qqp7k92_/tmp1dg06bhm_TarContainer/0/5", line 99, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_7qqp7k92_/tmp1dg06bhm_TarContainer/0/5", line 99, column 0: CDATA terminal not found*

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: madml Version: 0.0.2 Summary: Application domain of
+Metadata-Version: 2.1 Name: madml Version: 0.0.3 Summary: Application domain of
 machine learning in materials science. Home-page: https://github.com/leschultz/
 materials_application_domain_machine_learning.git Author: Lane E. Schultz
 Author-email: laneenriqueschultz@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
-Type: text/markdown License-File: LICENSE # Materials Application Domain (MAD)
-Research with respect to application domain with a materials science emphasis
-is contained within. The GitHub repo can be found in [here](https://github.com/
-leschultz/application_domain.git). ## Structure The structure of the code
-packages is as follows: ``` materials_application_domain_machine_learning/
-âââ examples âÂ Â  âââ auto_push âÂ Â  âÂ Â  âââ fit.py
-âÂ Â  âÂ Â  âââ run.sh âÂ Â  âÂ Â  âââ submit.sh âÂ Â 
-âââ single_runs âÂ Â  âââ make_runs.sh âÂ Â  âââ
-submit_jobs.sh âÂ Â  âââ template âÂ Â  âââ fit.py âÂ Â 
-âââ run.sh âÂ Â  âââ submit.sh âââ LICENSE âââ
-pyproject.toml âââ README.md âââ setup.py âââ src âÂ Â 
-âââ madml âÂ Â  âââ data âÂ Â  âÂ Â  âââ
+Type: text/markdown License-File: LICENSE # Materials Application Domain
+Machine Learning (MADML) Research with respect to application domain with a
+materials science emphasis is contained within. The GitHub repo can be found in
+[here](https://github.com/leschultz/application_domain.git). ## Structure The
+structure of the code packages is as follows: ```
+materials_application_domain_machine_learning/ âââ examples âÂ Â 
+âââ auto_push âÂ Â  âÂ Â  âââ fit.py âÂ Â  âÂ Â  âââ
+run.sh âÂ Â  âÂ Â  âââ submit.sh âÂ Â  âââ single_runs
+âÂ Â  âââ make_runs.sh âÂ Â  âââ submit_jobs.sh âÂ Â 
+âââ template âÂ Â  âââ fit.py âÂ Â  âââ run.sh âÂ Â 
+âââ submit.sh âââ LICENSE âââ pyproject.toml âââ
+README.md âââ setup.py âââ src âÂ Â  âââ madml âÂ Â 
+âââ data âÂ Â  âÂ Â  âââ
 citrine_thermal_conductivity_simplified.xlsx âÂ Â  âÂ Â  âââ
 Dataset_electromigration.xlsx âÂ Â  âÂ Â  âââ
 Dataset_Perovskite_Opband_simplified.xlsx âÂ Â  âÂ Â  âââ
 dielectric_constant_simplified.xlsx âÂ Â  âÂ Â  âââ diffusion.csv
 âÂ Â  âÂ Â  âââ double_perovskites_gap.xlsx âÂ Â  âÂ Â  âââ
 elastic_tensor_2015_simplified.xlsx âÂ Â  âÂ Â  âââ fluence.csv
 âÂ Â  âÂ Â  âââ heusler_magnetic_simplified.xlsx âÂ Â  âÂ Â
```

### Comparing `madml-0.0.2/setup.py` & `madml-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 # Package information
 name = 'madml'
-version = '0.0.2'
+version = '0.0.3'
 description = 'Application domain of machine learning in materials science.'
 url = 'https://github.com/leschultz/'\
       'materials_application_domain_machine_learning.git'
 author = 'Lane E. Schultz'
 author_email = 'laneenriqueschultz@gmail.com'
 python_requires = '>=3.6'
 classifiers = ['Programming Language :: Python :: 3',
@@ -34,13 +34,14 @@
                  name=name,
                  version=version,
                  description=description,
                  url=url,
                  author=author,
                  author_email=author_email,
                  packages=packages,
+                 package_dir={'':'src'},
                  python_requires=python_requires,
                  classifiers=classifiers,
                  install_requires=install_requires,
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  )
```

### Comparing `madml-0.0.2/tests/test_run.py` & `madml-0.0.3/tests/test_run.py`

 * *Files identical despite different names*

