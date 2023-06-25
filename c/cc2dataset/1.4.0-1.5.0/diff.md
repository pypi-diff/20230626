# Comparing `tmp/cc2dataset-1.4.0.tar.gz` & `tmp/cc2dataset-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cc2dataset-1.4.0.tar", last modified: Tue Dec  6 00:38:03 2022, max compression
+gzip compressed data, was "cc2dataset-1.5.0.tar", last modified: Sun Jun 25 22:54:58 2023, max compression
```

## Comparing `cc2dataset-1.4.0.tar` & `cc2dataset-1.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 00:38:03.160033 cc2dataset-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2022-12-06 00:37:51.000000 cc2dataset-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2022-12-06 00:38:03.160033 cc2dataset-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2022-12-06 00:37:51.000000 cc2dataset-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 00:38:03.156033 cc2dataset-1.4.0/cc2dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-06 00:37:51.000000 cc2dataset-1.4.0/cc2dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2022-12-06 00:37:51.000000 cc2dataset-1.4.0/cc2dataset/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2022-12-06 00:37:51.000000 cc2dataset-1.4.0/cc2dataset/spark_session_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 00:38:03.156033 cc2dataset-1.4.0/cc2dataset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2022-12-06 00:38:03.000000 cc2dataset-1.4.0/cc2dataset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2022-12-06 00:38:03.000000 cc2dataset-1.4.0/cc2dataset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 00:38:03.000000 cc2dataset-1.4.0/cc2dataset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2022-12-06 00:38:03.000000 cc2dataset-1.4.0/cc2dataset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-06 00:38:03.000000 cc2dataset-1.4.0/cc2dataset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-06 00:38:03.160033 cc2dataset-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2022-12-06 00:37:51.000000 cc2dataset-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:54:58.664130 cc2dataset-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-25 22:54:45.000000 cc2dataset-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-06-25 22:54:58.664130 cc2dataset-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-06-25 22:54:45.000000 cc2dataset-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:54:58.660130 cc2dataset-1.5.0/cc2dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-25 22:54:45.000000 cc2dataset-1.5.0/cc2dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-06-25 22:54:45.000000 cc2dataset-1.5.0/cc2dataset/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-25 22:54:45.000000 cc2dataset-1.5.0/cc2dataset/spark_session_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:54:58.664130 cc2dataset-1.5.0/cc2dataset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-06-25 22:54:58.000000 cc2dataset-1.5.0/cc2dataset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-25 22:54:58.000000 cc2dataset-1.5.0/cc2dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 22:54:58.000000 cc2dataset-1.5.0/cc2dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-25 22:54:58.000000 cc2dataset-1.5.0/cc2dataset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-25 22:54:58.000000 cc2dataset-1.5.0/cc2dataset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 22:54:58.664130 cc2dataset-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-25 22:54:45.000000 cc2dataset-1.5.0/setup.py
```

### Comparing `cc2dataset-1.4.0/LICENSE` & `cc2dataset-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cc2dataset-1.4.0/PKG-INFO` & `cc2dataset-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cc2dataset
-Version: 1.4.0
+Version: 1.5.0
 Summary: Easily convert common crawl to image caption set using pyspark
 Home-page: https://github.com/rom1504/cc2dataset
 Author: Romain Beaumont
 Author-email: romain.rom1@gmail.com
 License: MIT
 Description: # cc2dataset
         [![pypi](https://img.shields.io/pypi/v/cc2dataset.svg)](https://pypi.python.org/pypi/cc2dataset)
@@ -25,20 +25,23 @@
         This tool produces a collection of link + caption. It is meant as the stage 1 of creating a dataset. It does deduplication and as minimal as possible filtering (does it look like an url / is the caption non empty).
         
         This produces a large quantity of raw data that can then be further filtered by appropriate techniques.
         An example of stage 2 can be to estimate the similarity between (link, text) with a model such as CLIP. This may reduce the quantity of data by a factor of up to 100x depending on the chosen threshold.
         
         ## What hardware to pick ?
         
+        CC is big and located at s3 us east 1, so it makes a lot of sense in term of network to use machines located in the same place.
+        
         `cpu128-dy-c6i-32xlarge` instances are advised. Spark stores the non duplicated first stage in local disk. They should be nvme drive for speed during deduplication. At this first stage, one wat takes about 20MB, so the total (over all workers) space must be more than 20MB times wat count. So for example for the whole CC, that means 100TB. So for example that can fit in 150 instances with 1TB nvme drive each. 150 instances of 128 cores is 19200 cores so the whole processing takes 2h. Less instances with bigger hard drives can work too. It's also a possibility to do the processing in multiple pieces if temporary disk space is an issue by specifying `--multipart`.
         
         ## Document type
         
         This tool support extracting several documents from CC:
         * image/text: about 300B after dedup
+        * image/text even with empty text: estimated 1T
         * audio/text: about 2B after dedup
         * text doc : about 10B after dedup
         * video/text: about 2B after dedup
         
         They can be selected with eg `--document_type audio`.
         You may experiment with more document kinds by running `python example single_warc_example.py` and exploring the resulting output.parquet.
```

### Comparing `cc2dataset-1.4.0/README.md` & `cc2dataset-1.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,20 +17,23 @@
 This tool produces a collection of link + caption. It is meant as the stage 1 of creating a dataset. It does deduplication and as minimal as possible filtering (does it look like an url / is the caption non empty).
 
 This produces a large quantity of raw data that can then be further filtered by appropriate techniques.
 An example of stage 2 can be to estimate the similarity between (link, text) with a model such as CLIP. This may reduce the quantity of data by a factor of up to 100x depending on the chosen threshold.
 
 ## What hardware to pick ?
 
+CC is big and located at s3 us east 1, so it makes a lot of sense in term of network to use machines located in the same place.
+
 `cpu128-dy-c6i-32xlarge` instances are advised. Spark stores the non duplicated first stage in local disk. They should be nvme drive for speed during deduplication. At this first stage, one wat takes about 20MB, so the total (over all workers) space must be more than 20MB times wat count. So for example for the whole CC, that means 100TB. So for example that can fit in 150 instances with 1TB nvme drive each. 150 instances of 128 cores is 19200 cores so the whole processing takes 2h. Less instances with bigger hard drives can work too. It's also a possibility to do the processing in multiple pieces if temporary disk space is an issue by specifying `--multipart`.
 
 ## Document type
 
 This tool support extracting several documents from CC:
 * image/text: about 300B after dedup
+* image/text even with empty text: estimated 1T
 * audio/text: about 2B after dedup
 * text doc : about 10B after dedup
 * video/text: about 2B after dedup
 
 They can be selected with eg `--document_type audio`.
 You may experiment with more document kinds by running `python example single_warc_example.py` and exploring the resulting output.parquet.
```

### Comparing `cc2dataset-1.4.0/cc2dataset/main.py` & `cc2dataset-1.5.0/cc2dataset/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,68 +13,118 @@
 from pyspark.sql.functions import rand
 from pyspark.sql import SparkSession
 import random
 import math
 import time
 from .spark_session_builder import build_spark_session
 from io import BytesIO
+from urllib.parse import urljoin
 
 
 def valid_video_link(link):
-    valid_http = link.get("url", "").startswith("http")
-    valid_video = any(link.get("url", "").endswith(ext) for ext in [".avi", ".mp4", ".mkv", ".webm", ".mov"])
-    return valid_http and valid_video
+    valid_video = any(
+        link.get("url", "").endswith(ext) for ext in [".avi", ".mp4", ".mkv", ".webm", ".mov", ".mpg", ".mpeg", ".m4v"]
+    )
+    return valid_video
 
 
 def extract_video_from_links(links):
     filtered_links = [{"url": link["url"], "alt": link.get("text", "")} for link in links if valid_video_link(link)]
     return filtered_links
 
 
+text_extensions = set(
+    [
+        "pdf",
+        "epub",
+        "djvu",
+        "mobi",
+        "doc",
+        "docx",
+        "rtf",
+        "txt",
+        "odt",
+        "ppt",
+        "pptx",
+        "pages",
+        "keynote",
+        "wps",
+        "md",
+    ]
+)
+
+
 def valid_text_link(link):
-    valid_http = link.get("url", "").startswith("http")
-    valid_text = any(link.get("url", "").endswith(ext) for ext in [".pdf", ".epub", ".djvu"])
-    return valid_http and valid_text
+    splits = link.get("url", "").split(".")
+    if len(splits) < 2:
+        return False
+    if splits[-1] not in text_extensions:
+        return False
+    return True
 
 
 def extract_text_from_links(links):
     filtered_links = [{"url": link["url"], "alt": link.get("text", "")} for link in links if valid_text_link(link)]
     return filtered_links
 
 
 def valid_audio_link(link):
-    valid_http = link.get("url", "").startswith("http")
     valid_audio = any(link.get("url", "").endswith(ext) for ext in [".ogg", ".wav", ".mp3", ".flac", ".m4a"])
-    return valid_http and valid_audio
+    return valid_audio
 
 
 def extract_audio_from_links(links):
     """Extract image from links"""
     filtered_links = [{"url": link["url"], "alt": link.get("text", "")} for link in links if valid_audio_link(link)]
     return filtered_links
 
 
 def valid_image_link(link):
     valid_path = link.get("path", "") == "IMG@/src"
     valid_alt = len(link.get("alt", "")) > 0
-    valid_http = link.get("url", "").startswith("http")
-    return valid_path and valid_http and valid_alt
+    return valid_path and valid_alt
 
 
 def extract_image_from_links(links):
     """Extract image from links"""
     filtered_links = [{"url": link["url"], "alt": link["alt"]} for link in links if valid_image_link(link)]
     return filtered_links
 
 
+def valid_image_only_link(link):
+    valid_path = link.get("path", "") == "IMG@/src"
+    return valid_path
+
+
+def extract_image_only_from_links(links):
+    """Extract image from links even when no caption is present"""
+    filtered_links = [{"url": link["url"], "alt": link.get("alt", "")} for link in links if valid_image_only_link(link)]
+    return filtered_links
+
+
+def make_link_absolute(url, base_url):
+    if url.startswith("http://") or url.startswith("https://"):
+        return url
+    try:
+        return urljoin(base_url, url)
+    except ValueError:
+        return url
+
+
+def make_links_absolute(links, base_url):
+    return [{"url": make_link_absolute(link["url"], base_url), "alt": link["alt"]} for link in links]
+
+
 def extract_documents_from_links(links, document_type):
     """Extract documents from links ; this function returns a list of dict {"alt": ..., "url": ...}"""
 
     if document_type == "image":
         return extract_image_from_links(links)
+    elif document_type == "image_only":
+        return extract_image_only_from_links(links)
     elif document_type == "audio":
         return extract_audio_from_links(links)
     elif document_type == "text":
         return extract_text_from_links(links)
     elif document_type == "video":
         return extract_video_from_links(links)
     else:
@@ -99,18 +149,35 @@
             if "HTML-Metadata" not in http_resp:
                 continue
             metadata = http_resp["HTML-Metadata"]
             if "Links" not in metadata:
                 continue
 
             links = metadata["Links"]
+            cc_filename = record_data["Container"]["Filename"]
+            page_url = envelope["WARC-Header-Metadata"]["WARC-Target-URI"]
+            # extract base URL to resolve relative URLs
+            base_url = envelope["WARC-Header-Metadata"]["WARC-Target-URI"]
+            if "Head" in metadata and "Base" in metadata["Head"]:
+                try:
+                    base_url = urljoin(base_url, metadata["Head"]["Base"])
+                except ValueError:
+                    pass
 
             filtered_links = extract_documents_from_links(links, document_type)
+            filtered_links = make_links_absolute(filtered_links, base_url)
+            filtered_links = [
+                link
+                for link in filtered_links
+                if link["url"].startswith("http://") or link["url"].startswith("https://")
+            ]
             for link in filtered_links:
                 link["uid"] = str(hashlib.md5((link["alt"] + link["url"]).encode()).hexdigest())
+                link["cc_filename"] = cc_filename
+                link["page_url"] = page_url
             all_links.extend(filtered_links)
     except Exception as e:  # pylint: disable=broad-except
         logger.info(e)
         logger.info("A shard failed to parse")
         return []
 
     return all_links
@@ -129,15 +196,15 @@
                     logger.info("failed 10 times, skipping ", path)
                     return
                 logger.info(ex)
                 logger.info(f"retrying reading {i}/10")
                 time.sleep(1)
 
         for e in extract_documents_from_wat(tf, document_type):
-            yield (e["uid"], e["url"], e["alt"])
+            yield (e["uid"], e["url"], e["alt"], e["cc_filename"], e["page_url"])
     end_read = timer()
     tot_read_time = end_read - begin_read
     logger.info(f"Took {tot_read_time} to parse")
 
 
 def get_cc_wat_links(source_cc_protocol):
     """Get cc wat links"""
@@ -186,15 +253,15 @@
 
 def deduplicate_repartition_count(df, output_path, wat_count, spark, shuffle=False):
     """Deduplicate and repartition"""
     uniques = df.dropDuplicates(["uid"])
     s = time.time()
     if shuffle:
         uniques = uniques.sort(rand())
-    repartitioned = uniques.repartition(max(256, wat_count // 100))
+    repartitioned = uniques.repartition(max(256, wat_count // 500))
     repartitioned.write.mode("overwrite").parquet(output_path)
     e = time.time()
     logger.info(f"Took {e - s} seconds")
     logger.info("Computing size")
     df = spark.read.parquet(output_path)
     logger.info(f"Size: {df.count()}")
 
@@ -211,25 +278,25 @@
         prefix = "https://data.commoncrawl.org/"
 
     def extract(x):
         x = list(x)
         yield from process_wat(prefix + x[0], document_type)
 
     output = wat_rdd.mapPartitions(extract)
-    df = output.toDF(["uid", "url", "alt"])
+    df = output.toDF(["uid", "url", "alt", "cc_filename", "page_url"])
 
     deduplicate_repartition_count(df, output_path, wat_count, spark, shuffle)
 
 
 def get_last_successful_part(output_path):
     """Get the last successful part"""
     output_path = output_path.replace("s3a", "s3")
     fs, _ = fsspec.core.url_to_fs(output_path)
     successful_parts = fs.glob(output_path + "/*/_SUCCESS")
-    last_part = sorted([int(e.split("/")[-2].split("_")[-1]) for e in successful_parts])[-1]
+    last_part = sorted([int(e.split("/")[-2].split("_")[-1]) for e in successful_parts if "merged" not in e])[-1]
     return last_part
 
 
 def process_multi_part(
     output_path, wat_index_files, build_spark, multipart, shuffle, resume, document_type, source_cc_protocol
 ):
     """Process multi part"""
@@ -248,14 +315,15 @@
         part_paths.append(part_path)
         logger.info(f"Processing part {i} from {start} to {end} into {part_path}")
         process_one_part(part_path, wat_index_files[start:end], build_spark, False, document_type, source_cc_protocol)
 
     spark = build_spark()
     logger.info("Merging parts")
     df = None
+    part_paths = [f"{output_path}/part_{i}" for i in range(0, multipart)]
     for part_path in part_paths:
         if df is None:
             df = spark.read.parquet(part_path)
         else:
             df = df.union(spark.read.parquet(part_path))
 
     deduplicate_repartition_count(df, output_path + "/merged", wat_count, spark, shuffle)
```

### Comparing `cc2dataset-1.4.0/cc2dataset/spark_session_builder.py` & `cc2dataset-1.5.0/cc2dataset/spark_session_builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,19 +30,22 @@
     """Build a spark session on AWS EC2"""
     os.environ["PYSPARK_PYTHON"] = sys.executable
     os.environ["PYSPARK_DRIVER_PYTHON"] = sys.executable
     main_memory = str(int(mem_gb * 0.9)) + "g"
     memory_overhead = str(mem_gb - int(mem_gb * 0.9)) + "g"
     spark = (
         SparkSession.builder.config("spark.submit.deployMode", "client")
+        .config("spark.driver.cores", "20")
+        .config("spark.driver.memory", "50g")
+        .config("spark.driver.maxResultSize", "10g")
         .config("spark.executor.memory", main_memory)
         .config("spark.executor.cores", str(num_cores))  # this can be set to the number of cores of the machine
         .config("spark.task.cpus", "1")
         .config("spark.executor.memoryOverhead", memory_overhead)
-        .config("spark.task.maxFailures", "2")
+        .config("spark.task.maxFailures", "10")
         .config(
             "spark.jars.packages", "org.apache.hadoop:hadoop-aws:3.3.1,org.apache.spark:spark-hadoop-cloud_2.13:3.3.1"
         )
         # change to the appropriate auth method, see https://hadoop.apache.org/docs/stable/hadoop-aws/tools/hadoop-aws/index.html
         .config("spark.hadoop.fs.s3a.aws.credentials.provider", "com.amazonaws.auth.InstanceProfileCredentialsProvider")
         # ton of options to try and make s3a run faster
         .config("spark.hadoop.fs.s3a.threads.max", "512")
```

### Comparing `cc2dataset-1.4.0/cc2dataset.egg-info/PKG-INFO` & `cc2dataset-1.5.0/cc2dataset.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cc2dataset
-Version: 1.4.0
+Version: 1.5.0
 Summary: Easily convert common crawl to image caption set using pyspark
 Home-page: https://github.com/rom1504/cc2dataset
 Author: Romain Beaumont
 Author-email: romain.rom1@gmail.com
 License: MIT
 Description: # cc2dataset
         [![pypi](https://img.shields.io/pypi/v/cc2dataset.svg)](https://pypi.python.org/pypi/cc2dataset)
@@ -25,20 +25,23 @@
         This tool produces a collection of link + caption. It is meant as the stage 1 of creating a dataset. It does deduplication and as minimal as possible filtering (does it look like an url / is the caption non empty).
         
         This produces a large quantity of raw data that can then be further filtered by appropriate techniques.
         An example of stage 2 can be to estimate the similarity between (link, text) with a model such as CLIP. This may reduce the quantity of data by a factor of up to 100x depending on the chosen threshold.
         
         ## What hardware to pick ?
         
+        CC is big and located at s3 us east 1, so it makes a lot of sense in term of network to use machines located in the same place.
+        
         `cpu128-dy-c6i-32xlarge` instances are advised. Spark stores the non duplicated first stage in local disk. They should be nvme drive for speed during deduplication. At this first stage, one wat takes about 20MB, so the total (over all workers) space must be more than 20MB times wat count. So for example for the whole CC, that means 100TB. So for example that can fit in 150 instances with 1TB nvme drive each. 150 instances of 128 cores is 19200 cores so the whole processing takes 2h. Less instances with bigger hard drives can work too. It's also a possibility to do the processing in multiple pieces if temporary disk space is an issue by specifying `--multipart`.
         
         ## Document type
         
         This tool support extracting several documents from CC:
         * image/text: about 300B after dedup
+        * image/text even with empty text: estimated 1T
         * audio/text: about 2B after dedup
         * text doc : about 10B after dedup
         * video/text: about 2B after dedup
         
         They can be selected with eg `--document_type audio`.
         You may experiment with more document kinds by running `python example single_warc_example.py` and exploring the resulting output.parquet.
```

### Comparing `cc2dataset-1.4.0/setup.py` & `cc2dataset-1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     REQUIREMENTS = _read_reqs("requirements.txt")
 
     setup(
         name="cc2dataset",
         packages=find_packages(),
         include_package_data=True,
-        version="1.4.0",
+        version="1.5.0",
         license="MIT",
         description="Easily convert common crawl to image caption set using pyspark",
         long_description=long_description,
         long_description_content_type="text/markdown",
         author="Romain Beaumont",
         author_email="romain.rom1@gmail.com",
         url="https://github.com/rom1504/cc2dataset",
```

