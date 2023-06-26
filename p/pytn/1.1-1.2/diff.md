# Comparing `tmp/pytn-1.1.tar.gz` & `tmp/pytn-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytn-1.1.tar", last modified: Tue Dec  6 13:45:11 2022, max compression
+gzip compressed data, was "pytn-1.2.tar", last modified: Mon Jun 26 18:38:31 2023, max compression
```

## Comparing `pytn-1.1.tar` & `pytn-1.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-12-06 13:45:11.442591 pytn-1.1/
--rw-rw-rw-   0        0        0     3897 2022-12-06 13:45:11.442591 pytn-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3038 2022-12-06 13:44:43.000000 pytn-1.1/README.md
-drwxrwxrwx   0        0        0        0 2022-12-06 13:45:11.416845 pytn-1.1/pytn/
--rw-rw-rw-   0        0        0     3916 2022-12-06 13:38:27.000000 pytn-1.1/pytn/MainFiles.py
--rw-rw-rw-   0        0        0     1531 2022-11-15 14:34:53.000000 pytn-1.1/pytn/SupportFuncs.py
--rw-rw-rw-   0        0        0     1242 2022-11-15 15:29:09.000000 pytn-1.1/pytn/__init__.py
--rw-rw-rw-   0        0        0      700 2022-11-15 15:28:10.000000 pytn-1.1/pytn/compiler.py
-drwxrwxrwx   0        0        0        0 2022-12-06 13:45:11.430873 pytn-1.1/pytn.egg-info/
--rw-rw-rw-   0        0        0     3897 2022-12-06 13:45:11.000000 pytn-1.1/pytn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2022-12-06 13:45:11.000000 pytn-1.1/pytn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-06 13:45:11.000000 pytn-1.1/pytn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-12-06 13:45:11.000000 pytn-1.1/pytn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-12-06 13:45:11.000000 pytn-1.1/pytn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-06 13:45:11.442591 pytn-1.1/setup.cfg
--rw-rw-rw-   0        0        0      975 2022-12-06 13:44:06.000000 pytn-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:38:31.450617 pytn-1.2/
+-rw-rw-rw-   0        0        0    35129 2022-12-06 13:51:56.000000 pytn-1.2/LICENSE
+-rw-rw-rw-   0        0        0     3899 2023-06-26 18:38:31.448616 pytn-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3038 2022-12-06 13:44:43.000000 pytn-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 18:38:31.420590 pytn-1.2/pytn/
+-rw-rw-rw-   0        0        0     2926 2023-06-22 17:46:44.000000 pytn-1.2/pytn/MainFiles.py
+-rw-rw-rw-   0        0        0     1794 2023-06-22 17:43:21.000000 pytn-1.2/pytn/SupportFuncs.py
+-rw-rw-rw-   0        0        0     1263 2023-06-26 18:38:08.000000 pytn-1.2/pytn/__init__.py
+-rw-rw-rw-   0        0        0      700 2022-11-15 15:28:10.000000 pytn-1.2/pytn/compiler.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:38:31.446614 pytn-1.2/pytn.egg-info/
+-rw-rw-rw-   0        0        0     3899 2023-06-26 18:38:31.000000 pytn-1.2/pytn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-06-26 18:38:31.000000 pytn-1.2/pytn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 18:38:31.000000 pytn-1.2/pytn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-26 18:38:31.000000 pytn-1.2/pytn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-26 18:38:31.000000 pytn-1.2/pytn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 18:38:31.450617 pytn-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1009 2023-06-26 18:38:21.000000 pytn-1.2/setup.py
```

### Comparing `pytn-1.1/PKG-INFO` & `pytn-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pytn
-Version: 1.1
+Version: 1.2
 Summary: Python text notation
 Home-page: https://github.com/kshitij1235/filemod
 Author: kshitij jathar
 Author-email: kshitijjathar7@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kshitij1235/filemod/issues
 Keywords: file
-Platform: UNKNOWN
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ## pytn
 
 With the help of pytn you can use your txt file as a json file in a very simple way
 
 pytn stands for - python text notation
 
@@ -142,8 +142,7 @@
   
 ## Authors
 
 - [@kshitij1235](https://github.com/kshitij1235)
 - [website](https://sites.google.com/view/pytn)
 
   
-
```

### Comparing `pytn-1.1/README.md` & `pytn-1.2/README.md`

 * *Files identical despite different names*

### Comparing `pytn-1.1/pytn/SupportFuncs.py` & `pytn-1.2/pytn/SupportFuncs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# json_txt/SupportFuncs.py - version 1.4.6
-
+from filemod import writer
 
 def number_detect(letter):
     """Detect the nature of letter is number or not"""
 
     try:
         int(letter)
         return True
@@ -37,20 +36,28 @@
 
 
 def collab_words_in_list(list):
     """collab word into strings"""
     return ''.join(list)
 
 
-def allot_values(values):
+def allot_values(values : list):
     processed_values=[]
     for elements in values:
+        
         if elements[0] == "[":
             processed_values.append(list(generate_array(elements)))
         elif elements=="True":
             processed_values.append(True)
         elif elements=="False":
             processed_values.append(False)
         else:
             processed_values.append(number_string(elements))
     return processed_values
 
+
+def write_dict_in_file(filename : str ,data:dict)->bool:
+    write_file = "{ \n"
+    for key , value  in data.items():
+        write_file = f"{write_file} {key} : {value}\n"
+    write_file = write_file+"\n"+"}"
+    return writer(filename, write_file, "w")
```

### Comparing `pytn-1.1/pytn/__init__.py` & `pytn-1.2/pytn/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,9 +17,11 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Extracting keys and values out of txt file and convert it into dic"""
+
+__version__ = 1.2
 from pytn.MainFiles import *
```

### Comparing `pytn-1.1/pytn/compiler.py` & `pytn-1.2/pytn/compiler.py`

 * *Files identical despite different names*

### Comparing `pytn-1.1/pytn.egg-info/PKG-INFO` & `pytn-1.2/pytn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pytn
-Version: 1.1
+Version: 1.2
 Summary: Python text notation
 Home-page: https://github.com/kshitij1235/filemod
 Author: kshitij jathar
 Author-email: kshitijjathar7@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kshitij1235/filemod/issues
 Keywords: file
-Platform: UNKNOWN
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ## pytn
 
 With the help of pytn you can use your txt file as a json file in a very simple way
 
 pytn stands for - python text notation
 
@@ -142,8 +142,7 @@
   
 ## Authors
 
 - [@kshitij1235](https://github.com/kshitij1235)
 - [website](https://sites.google.com/view/pytn)
 
   
-
```

### Comparing `pytn-1.1/setup.py` & `pytn-1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
-
+from pytn import __version__
 from filemod import reader
 
 
 classifiers=[
     'Intended Audience :: Education',
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8"
 ]
 setuptools.setup(
     name="pytn",
-    version="1.1",
+    version=__version__,
     author="kshitij jathar",
     author_email="kshitijjathar7@gmail.com",
     description="Python text notation",
     long_description=reader('README.md'),
     long_description_content_type="text/markdown",
     url="https://github.com/kshitij1235/filemod",
     project_urls={
```

