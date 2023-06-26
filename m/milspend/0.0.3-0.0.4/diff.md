# Comparing `tmp/milspend-0.0.3.tar.gz` & `tmp/milspend-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milspend-0.0.3.tar", last modified: Wed May 24 09:50:06 2023, max compression
+gzip compressed data, was "milspend-0.0.4.tar", last modified: Mon Jun 26 11:47:29 2023, max compression
```

## Comparing `milspend-0.0.3.tar` & `milspend-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-24 09:50:06.894383 milspend-0.0.3/
--rw-r--r--   0 yt        (1000) yt        (1000)     1689 2023-05-24 09:50:06.894383 milspend-0.0.3/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)     1147 2022-02-27 14:19:58.000000 milspend-0.0.3/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-05-24 09:50:06.902366 milspend-0.0.3/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      962 2023-05-23 23:56:30.000000 milspend-0.0.3/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-24 09:50:06.887504 milspend-0.0.3/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-24 09:50:06.894383 milspend-0.0.3/src/milspend.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     1689 2023-05-24 09:50:06.000000 milspend-0.0.3/src/milspend.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      227 2023-05-24 09:50:06.000000 milspend-0.0.3/src/milspend.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-05-24 09:50:06.000000 milspend-0.0.3/src/milspend.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       44 2023-05-24 09:50:06.000000 milspend-0.0.3/src/milspend.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        9 2023-05-24 09:50:06.000000 milspend-0.0.3/src/milspend.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     1548 2023-05-24 09:49:23.000000 milspend-0.0.3/src/milspend.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-26 11:47:29.468096 milspend-0.0.4/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1689 2023-06-26 11:47:29.468096 milspend-0.0.4/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)     1147 2022-02-27 14:19:58.000000 milspend-0.0.4/README.md
+-rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-06-26 11:47:29.468096 milspend-0.0.4/setup.cfg
+-rw-r--r--   0 yt        (1000) yt        (1000)      962 2023-06-26 11:45:39.000000 milspend-0.0.4/setup.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-26 11:47:29.462125 milspend-0.0.4/src/
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-26 11:47:29.468096 milspend-0.0.4/src/milspend.egg-info/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1689 2023-06-26 11:47:28.000000 milspend-0.0.4/src/milspend.egg-info/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)      227 2023-06-26 11:47:28.000000 milspend-0.0.4/src/milspend.egg-info/SOURCES.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-06-26 11:47:28.000000 milspend-0.0.4/src/milspend.egg-info/dependency_links.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)       44 2023-06-26 11:47:28.000000 milspend-0.0.4/src/milspend.egg-info/entry_points.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        9 2023-06-26 11:47:28.000000 milspend-0.0.4/src/milspend.egg-info/top_level.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)     1579 2023-06-26 11:43:09.000000 milspend-0.0.4/src/milspend.py
```

### Comparing `milspend-0.0.3/PKG-INFO` & `milspend-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: milspend
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for visualizing military spending of up to 4 countries
 Home-page: https://github.com/ytakefuji/defense
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/defense
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # defense
 
 The goal of this project is to visualize military spending of countries.
 
 Using a SIPRI dataset, milspend can visualize military spending of up to four countries.
```

### Comparing `milspend-0.0.3/README.md` & `milspend-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `milspend-0.0.3/setup.py` & `milspend-0.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="milspend",
-    version="0.0.3",
+    version="0.0.4",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A package for visualizing military spending of up to 4 countries",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ytakefuji/defense",
     project_urls={
@@ -19,14 +19,14 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     py_modules=['milspend'],
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     entry_points = {
         'console_scripts': [
             'milspend = milspend:main'
         ]
     },
 )
```

### Comparing `milspend-0.0.3/src/milspend.egg-info/PKG-INFO` & `milspend-0.0.4/src/milspend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: milspend
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for visualizing military spending of up to 4 countries
 Home-page: https://github.com/ytakefuji/defense
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/defense
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # defense
 
 The goal of this project is to visualize military spending of countries.
 
 Using a SIPRI dataset, milspend can visualize military spending of up to four countries.
```

### Comparing `milspend-0.0.3/src/milspend.py` & `milspend-0.0.4/src/milspend.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,8 +52,9 @@
  plt.legend()
 
 # Show the plot
  plt.savefig('result.png')
  plt.show()
  plt.close()
  sys.exit()
-main(countries)
+if __name__ == "__main__":
+    main(countries)
```

