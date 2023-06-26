# Comparing `tmp/e-models-1.3.3.tar.gz` & `tmp/e-models-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-models-1.3.3.tar", last modified: Thu Jun  8 13:46:59 2023, max compression
+gzip compressed data, was "e-models-1.4.tar", last modified: Mon Jun 26 14:30:46 2023, max compression
```

## Comparing `e-models-1.3.3.tar` & `e-models-1.4.tar`

### file list

```diff
@@ -1,27 +1,34 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-08 13:46:59.465554 e-models-1.3.3/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.3.3/LICENSE
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3468 2023-06-08 13:46:59.465554 e-models-1.3.3/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2928 2023-06-01 14:06:43.000000 e-models-1.3.3/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-08 13:46:59.461554 e-models-1.3.3/e_models.egg-info/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3468 2023-06-08 13:46:59.000000 e-models-1.3.3/e_models.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      471 2023-06-08 13:46:59.000000 e-models-1.3.3/e_models.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-06-08 13:46:59.000000 e-models-1.3.3/e_models.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        7 2023-06-08 13:46:59.000000 e-models-1.3.3/e_models.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-06-08 13:46:59.000000 e-models-1.3.3/e_models.egg-info/top_level.txt
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-08 13:46:59.461554 e-models-1.3.3/emodels/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       22 2023-06-08 13:46:29.000000 e-models-1.3.3/emodels/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-05-04 18:51:26.000000 e-models-1.3.3/emodels/config.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-08 13:46:59.465554 e-models-1.3.3/emodels/html2text/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35296 2023-06-08 13:46:29.000000 e-models-1.3.3/emodels/html2text/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.3.3/emodels/html2text/config.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.3.3/emodels/html2text/elements.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.3.3/emodels/html2text/typing.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.3.3/emodels/html2text/utils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.3.3/emodels/py.typed
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6744 2023-05-19 17:09:55.000000 e-models-1.3.3/emodels/scrapyutils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.3.3/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-06-08 13:46:59.465554 e-models-1.3.3/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      907 2023-06-08 13:46:29.000000 e-models-1.3.3/setup.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-08 13:46:59.465554 e-models-1.3.3/tests/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4951 2023-06-08 13:41:24.000000 e-models-1.3.3/tests/test_html2text.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7435 2023-05-04 18:49:39.000000 e-models-1.3.3/tests/test_scrapyutils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-26 14:30:46.338616 e-models-1.4/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.4/LICENSE
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3466 2023-06-26 14:30:46.338616 e-models-1.4/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2928 2023-06-01 14:06:43.000000 e-models-1.4/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-26 14:30:46.334616 e-models-1.4/e_models.egg-info/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3466 2023-06-26 14:30:46.000000 e-models-1.4/e_models.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      628 2023-06-26 14:30:46.000000 e-models-1.4/e_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-06-26 14:30:46.000000 e-models-1.4/e_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        7 2023-06-26 14:30:46.000000 e-models-1.4/e_models.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-06-26 14:30:46.000000 e-models-1.4/e_models.egg-info/top_level.txt
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-26 14:30:46.334616 e-models-1.4/emodels/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       20 2023-06-26 13:32:53.000000 e-models-1.4/emodels/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-05-04 18:51:26.000000 e-models-1.4/emodels/config.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-26 14:30:46.338616 e-models-1.4/emodels/datasets/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e-models-1.4/emodels/datasets/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1818 2023-06-23 22:31:59.000000 e-models-1.4/emodels/datasets/tokenizers.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4716 2023-06-23 22:38:40.000000 e-models-1.4/emodels/datasets/utils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-26 14:30:46.338616 e-models-1.4/emodels/html2text/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35296 2023-06-08 13:46:29.000000 e-models-1.4/emodels/html2text/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.4/emodels/html2text/config.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.4/emodels/html2text/elements.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.4/emodels/html2text/typing.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.4/emodels/html2text/utils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.4/emodels/py.typed
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-26 14:30:46.338616 e-models-1.4/emodels/scrapyutils/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      137 2023-06-23 22:04:28.000000 e-models-1.4/emodels/scrapyutils/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2544 2023-06-23 22:05:11.000000 e-models-1.4/emodels/scrapyutils/loader.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4351 2023-06-23 21:34:47.000000 e-models-1.4/emodels/scrapyutils/response.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.4/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-06-26 14:30:46.338616 e-models-1.4/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      905 2023-06-26 13:32:42.000000 e-models-1.4/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-26 14:30:46.338616 e-models-1.4/tests/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4948 2023-06-23 18:11:59.000000 e-models-1.4/tests/test_html2text.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7475 2023-06-23 23:01:17.000000 e-models-1.4/tests/test_scrapyutils.py
```

### Comparing `e-models-1.3.3/LICENSE` & `e-models-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `e-models-1.3.3/PKG-INFO` & `e-models-1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.3.3
+Version: 1.4
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.3.3/README.md` & `e-models-1.4/README.md`

 * *Files identical despite different names*

### Comparing `e-models-1.3.3/e_models.egg-info/PKG-INFO` & `e-models-1.4/e_models.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.3.3
+Version: 1.4
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.3.3/emodels/html2text/__init__.py` & `e-models-1.4/emodels/html2text/__init__.py`

 * *Files identical despite different names*

### Comparing `e-models-1.3.3/emodels/html2text/config.py` & `e-models-1.4/emodels/html2text/config.py`

 * *Files identical despite different names*

### Comparing `e-models-1.3.3/emodels/html2text/utils.py` & `e-models-1.4/emodels/html2text/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.3.3/setup.py` & `e-models-1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name         = 'e-models',
-    version      = '1.3.3',
+    version      = '1.4',
     description  = 'Tools for helping build of extraction models with scrapy spiders.',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     license      = 'BSD',
     author       = 'Martin Olveyra',
     author_email = 'molveyra@gmail.com',
     url          = 'https://github.com/kalessin/emodels',
```

### Comparing `e-models-1.3.3/tests/test_html2text.py` & `e-models-1.4/tests/test_html2text.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 <tr><td>Data 5</td><td><p>Data 6</p></td></tr>
 <tr><td>Data 7</td><td>Data 8</td></tr>
 </table>
 """
         response = ExtractTextResponse(url="http://example.com/example2.html", status=200, body=html)
         expected = """| Data 1| Data 2|
 | Data 3| Data 4|
-| Data 5| 
+| Data 5|
 
 Data 6
 
 |
 | Data 7| Data 8|
 """
         self.assertEqual(response.markdown, expected)
@@ -162,9 +162,7 @@
         html = b"""<div>There&amp;nbsp;are&amp;nbsp;spaces</div>"""
         response = ExtractTextResponse(url="http://example.com/example2.html", status=200, body=html)
         self.assertEqual(response.markdown, "There&nbsp;are&nbsp;spaces\n")
 
         html = b"""<div>There&nbspare&nbspspaces</div>"""
         response = ExtractTextResponse(url="http://example.com/example2.html", status=200, body=html)
         self.assertEqual(response.markdown, "There are spaces\n")
-
-
```

### Comparing `e-models-1.3.3/tests/test_scrapyutils.py` & `e-models-1.4/tests/test_scrapyutils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import os
 import re
-import gzip
-import json
 from unittest import TestCase
+from typing import Dict
 
 from itemloaders.processors import TakeFirst
 from scrapy import Item, Field
 from scrapy.http import TextResponse
 
 os.environ["EMODELS_SAVE_EXTRACT_ITEMS"] = "1"
 os.environ["EMODELS_DIR"] = os.path.dirname(__file__)
 
 from emodels import config  # noqa
-from emodels.scrapyutils import ExtractItemLoader, COMMENT_RE, ExtractTextResponse  # noqa
-
-SAMPLES_DIR = os.path.join(os.path.dirname(__file__), "samples")
+from emodels.scrapyutils.loader import ExtractItemLoader  # noqa
+from emodels.scrapyutils.response import COMMENT_RE, ExtractTextResponse  # noqa
+from emodels.datasets.utils import DatasetFilename, build_response_from_sample_data  # noqa
 
 
 class JobItem(Item):
     job_title = Field()
     description = Field()
     url = Field()
     employment_type = Field()
@@ -55,27 +54,32 @@
 
 class BusinessSearchItemLoader(ExtractItemLoader):
     default_item_class = BusinessSearchItem
     default_output_processor = TakeFirst()
 
 
 class ScrapyUtilsTests(TestCase):
-    jobs_result_file = os.path.join(config.EMODELS_DIR, "items/JobItem/0.jl.gz")
-    business_result_file = os.path.join(config.EMODELS_DIR, "items/BusinessSearchItem/0.jl.gz")
+    jobs_result_file = DatasetFilename(os.path.join(config.EMODELS_DIR, "items/JobItem/0.jl.gz"))
+    business_result_file = DatasetFilename(os.path.join(config.EMODELS_DIR, "items/BusinessSearchItem/0.jl.gz"))
+    samples_file = DatasetFilename(os.path.join(os.path.dirname(__file__), "samples.jl.gz"))
+    samples: Dict[str, TextResponse]
+
+    @classmethod
+    def setUpClass(cls):
+        cls.samples = {d["url"]: build_response_from_sample_data(d) for d in cls.samples_file}
 
     def tearDown(self):
         for col in "jobs", "business":
             fname = getattr(self, f"{col}_result_file")
-            if os.path.isfile(fname):
-                os.remove(fname)
+            dname = os.path.dirname(fname)
+            for f in os.listdir(dname):
+                os.remove(os.path.join(dname, f))
 
     def test_example_one(self):
-        sample_file = os.path.join(SAMPLES_DIR, "job21.html")
-        body = open(sample_file).read().encode("utf8")
-        tresponse = TextResponse(url="https://careers.und.edu/jobs/job21.html", body=body, status=200)
+        tresponse = self.samples["https://careers.und.edu/jobs/job21.html"]
         loader = JobItemLoader(response=tresponse)
         loader.add_text_re("job_title", tid="#job_title_2_2")
         loader.add_text_re("employment_type", tid="#employment_type_2_2_0_0")
         loader.add_text_re("job_id", tid="#requisition_identifier_2_2_0")
         loader.add_text_re("description", r"(###\s+.+?)\*\*apply now\*\*", flags=re.S | re.I)
 
         item = loader.load_item()
@@ -97,33 +101,30 @@
 
         self.assertEqual(
             response.markdown[slice(*loader.extract_indexes["job_title"])], "Student Athlete Support Services Coord"
         )
         self.assertEqual(response.markdown[slice(*loader.extract_indexes["job_id"])], "492556")
         self.assertEqual(response.markdown[slice(*loader.extract_indexes["employment_type"])], "Full-time Staff")
 
-        with gzip.open(self.jobs_result_file, "rt") as fz:
-            data = json.loads(next(fz))
+        data = next(self.jobs_result_file)
 
         self.assertFalse(COMMENT_RE.findall(data["markdown"]))
 
         self.assertEqual(
             data["markdown"][slice(*data["indexes"]["job_title"])], "Student Athlete Support Services Coord"
         )
         self.assertEqual(data["markdown"][slice(*data["indexes"]["job_id"])], "492556")
         self.assertEqual(data["markdown"][slice(*data["indexes"]["employment_type"])], "Full-time Staff")
 
         self.assertEqual(data["markdown"][slice(*data["indexes"]["description"])], item["description"])
 
         self.assertTrue(response.text_re(tid=".job-field job-title"))
 
     def test_example_two(self):
-        sample_file = os.path.join(SAMPLES_DIR, "yell.html")
-        body = open(sample_file).read().encode("utf8")
-        response = ExtractTextResponse(url="https://yell.com/result.html", body=body, status=200)
+        response = self.samples["https://yell.com/result.html"].replace(cls=ExtractTextResponse)
 
         for r in response.css_split(".businessCapsule--mainRow"):
             loader = BusinessSearchItemLoader(response=r)
             loader.add_text_re("name", r"##(.+)")
             loader.add_text_re("phone", r"Tel([\s\d]+)", tid="#telephone")
             loader.add_text_re("website", r"Website\]\((.+?)\)")
             loader.add_text_re("address", r"\[(?:.+\|)?(.+)\]\(.+view=map")
@@ -135,18 +136,16 @@
             loader.add_text_re("locality", tid="#addressLocality", strict_tid=True)
             loader.add_text_re("address_alt", reg=r"(?:.+\|)?(.+?),?", tid="#addressLocality")
             loader.add_text_re("street", reg=r"(?:.+\|)?(.+?),?", tid="#streetAddress")
             loader.add_text_re("postal_code", tid="#postalCode", strict_tid=True)
             loader.load_item()
 
         extracted = []
-        with gzip.open(self.business_result_file, "rt") as fz:
-            for line in fz:
-                d = json.loads(line)
-                extracted.append({attr: d["markdown"][slice(*d["indexes"][attr])] for attr in d["indexes"]})
+        for d in self.business_result_file:
+            extracted.append({attr: d["markdown"][slice(*d["indexes"][attr])] for attr in d["indexes"]})
 
         self.assertEqual(len(extracted), 25)
         self.assertEqual(len([e for e in extracted if "name" in e]), 25)
         self.assertEqual(len([e for e in extracted if "category" in e]), 25)
         categories = [e["category"] for e in extracted if "category" in e]
         self.assertEqual(categories.count("Solicitors"), 24)
         self.assertEqual(categories.count("Personal Injury"), 1)
```

