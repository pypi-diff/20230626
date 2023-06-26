# Comparing `tmp/openai_parallel_toolkit-0.5.0-py3-none-any.whl.zip` & `tmp/openai_parallel_toolkit-0.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 18885 bytes, number of entries: 19
+Zip file size: 18533 bytes, number of entries: 19
 -rw-r--r--  2.0 unx      147 b- defN 23-Jun-19 11:22 openai_parallel_toolkit/__init__.py
 -rw-r--r--  2.0 unx       20 b- defN 23-May-17 01:58 openai_parallel_toolkit/config.py
 -rw-r--r--  2.0 unx      113 b- defN 23-May-17 12:36 openai_parallel_toolkit/api/__init__.py
 -rw-r--r--  2.0 unx     5216 b- defN 23-Jun-19 07:03 openai_parallel_toolkit/api/api.py
 -rw-r--r--  2.0 unx     5809 b- defN 23-May-23 12:55 openai_parallel_toolkit/api/keys.py
 -rw-r--r--  2.0 unx     3034 b- defN 23-May-25 08:28 openai_parallel_toolkit/api/request.py
 -rw-r--r--  2.0 unx       95 b- defN 23-May-17 01:02 openai_parallel_toolkit/core/__init__.py
 -rw-r--r--  2.0 unx     4532 b- defN 23-May-25 08:13 openai_parallel_toolkit/core/main.py
 -rw-r--r--  2.0 unx     4852 b- defN 23-May-18 11:47 openai_parallel_toolkit/core/multithread.py
 -rw-r--r--  2.0 unx      148 b- defN 23-Jun-19 11:22 openai_parallel_toolkit/utils/__init__.py
 -rw-r--r--  2.0 unx     1042 b- defN 23-May-18 11:32 openai_parallel_toolkit/utils/logger.py
--rw-r--r--  2.0 unx     4077 b- defN 23-May-25 08:22 openai_parallel_toolkit/utils/reader.py
+-rw-r--r--  2.0 unx     4107 b- defN 23-Jun-26 03:26 openai_parallel_toolkit/utils/reader.py
 -rw-r--r--  2.0 unx      913 b- defN 23-May-17 11:15 openai_parallel_toolkit/utils/token.py
 -rw-r--r--  2.0 unx      753 b- defN 23-May-18 11:47 openai_parallel_toolkit/utils/tqdm.py
--rw-r--r--  2.0 unx     1063 b- defN 23-Jun-19 11:23 openai_parallel_toolkit-0.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    14633 b- defN 23-Jun-19 11:23 openai_parallel_toolkit-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 11:23 openai_parallel_toolkit-0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-Jun-19 11:23 openai_parallel_toolkit-0.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1783 b- defN 23-Jun-19 11:23 openai_parallel_toolkit-0.5.0.dist-info/RECORD
-19 files, 48346 bytes uncompressed, 15887 bytes compressed:  67.1%
+-rw-r--r--  2.0 unx     1063 b- defN 23-Jun-26 03:29 openai_parallel_toolkit-0.5.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13483 b- defN 23-Jun-26 03:29 openai_parallel_toolkit-0.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 03:29 openai_parallel_toolkit-0.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-Jun-26 03:29 openai_parallel_toolkit-0.5.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1783 b- defN 23-Jun-26 03:29 openai_parallel_toolkit-0.5.1.dist-info/RECORD
+19 files, 47226 bytes uncompressed, 15535 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: openai_parallel_toolkit/utils/token.py
 Comment: 
 
 Filename: openai_parallel_toolkit/utils/tqdm.py
 Comment: 
 
-Filename: openai_parallel_toolkit-0.5.0.dist-info/LICENSE
+Filename: openai_parallel_toolkit-0.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: openai_parallel_toolkit-0.5.0.dist-info/METADATA
+Filename: openai_parallel_toolkit-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: openai_parallel_toolkit-0.5.0.dist-info/WHEEL
+Filename: openai_parallel_toolkit-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: openai_parallel_toolkit-0.5.0.dist-info/top_level.txt
+Filename: openai_parallel_toolkit-0.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: openai_parallel_toolkit-0.5.0.dist-info/RECORD
+Filename: openai_parallel_toolkit-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openai_parallel_toolkit/utils/reader.py

```diff
@@ -29,35 +29,36 @@
     Args:
         input_path (str): The path to the directory containing input files.
         output_path (str): The path to the directory containing output files.
         process_input (function): Function to process the input file data.
         file_count (int, optional): Maximum number of files to process. Processes all if not specified. Default is None.
 
     Returns:
-        dict: A dictionary mapping filenames (without extension) to processed data. Returns None if there's no data to process.
+        dict: A dictionary mapping filenames (without extension) to processed data. Returns None if there's no data
+        to process.
     """
     skipped_files_count = 0
     if output_path is not None:
         output_files = read_files(output_path)
         output_files_basename = [os.path.splitext(f)[0] for f in output_files]
         files = [f for f in read_files(input_path) if os.path.splitext(f)[0] not in output_files_basename][:file_count]
         skipped_files_count = len(output_files)
         logging.info(f"{LOG_LABEL}Output path: {output_path} Skipped files count: {skipped_files_count}")
     else:
         files = [
                     f for f in os.listdir(input_path) if
                     os.path.isfile(os.path.join(input_path, f)) and f[0] != "." and not os.path.splitext(f)[
                         0].startswith(
-                        ".")
+                            ".")
                 ][:file_count]
 
     data = {}
     for file in files:
         file_path = os.path.join(input_path, file)
-        with open(file_path, 'r') as f:
+        with open(file_path, 'r', encoding='utf-8') as f:
             file_name = os.path.splitext(file)[0]
             data[file_name] = process_input(f)
     if len(data) == 0:
         if skipped_files_count != 0:
             logging.info(f"{LOG_LABEL}All files have been processed: {input_path},file count: {skipped_files_count}")
             return None
         logging.error(f"{LOG_LABEL}input_path error, No data to process:{input_path}")
```

## Comparing `openai_parallel_toolkit-0.5.0.dist-info/LICENSE` & `openai_parallel_toolkit-0.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `openai_parallel_toolkit-0.5.0.dist-info/METADATA` & `openai_parallel_toolkit-0.5.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-parallel-toolkit
-Version: 0.5.0
+Version: 0.5.1
 Summary: OpenAI-Parallel-Toolkit is a Python library for handling multiple OpenAI API keys and parallel tasks. It provides API key rotation, multithreading for faster task execution, and utility functions to boost your OpenAI integration. Ideal for efficient large-scale OpenAI usage.
 Home-page: https://github.com/CZT0/OpenAI-Parallel-Toolkit
 Author: Jellow
 Author-email: dvdx@foxmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -269,46 +269,14 @@
 
 This allows the API key manager to automatically rotate API keys once the per-minute limit is reached, which is
 beneficial for streamlining the management of multiple keys and ensuring uninterrupted service.
 
 `request_openai_api` and `multi_process_one` also provides handling of OpenAI request errors, including automatic retry,
 removal of keys that reach the quota, and so on.
 
-## Additional Utility Classes
-
-### Token Count Calculation
-
-The `num_tokens_from_string` function is provided to calculate the number of tokens in a string, using the default
-behavior of GPT-3.5. It can be used as follows:
-
-```python
-from openai_parallel_toolkit import num_tokens_from_string
-
-print(num_tokens_from_string("hello world"))
-```
-
-### Splitting Text by Token Length
-
-The `split_string_by_tokens` function allows you to split a long text into segments of a specified token length and
-store them in a list. It can be used as follows:
-
-```python
-from openai_parallel_toolkit import split_string_by_tokens
-
-results = split_string_by_tokens(string="hello world", thunk_len=2, split_signal="。")
-```
-
-The parameters for `split_string_by_tokens` are as follows:
-
-- `string (str)`: The text to be segmented.
-- `thunk_len (int)`: The length of each segment in tokens.
-- `split_signal (str)`: The delimiter used for splitting.
-  It's important to note that if a sentence within a segment is too long, the segment may exceed the specified length.
-  This function does not truncate the text, but only splits it when encountering the split signal.
-
 ## Contributing
 
 We truly appreciate and value contributions from the community, as they play a significant role in enhancing the
 OpenAI-Parallel-Toolkit. Whether it's by reporting bugs, proposing new features, or directly contributing code, you can
 help us improve this project. Here are a few guidelines on how you can contribute:
 
 1. **Reporting Bugs**: If you encounter any bugs or issues, please open an issue in the GitHub repository detailing the
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `openai_parallel_toolkit-0.5.0.dist-info/RECORD` & `openai_parallel_toolkit-0.5.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 openai_parallel_toolkit/api/keys.py,sha256=RB9BmU7Qth3QIUWP30KXcfgmyblWVFYUnH0uB538ISs,5809
 openai_parallel_toolkit/api/request.py,sha256=75V3R79jE055WovuwQp7Pp29Ib_NUCDbFFqYVyaBA0w,3034
 openai_parallel_toolkit/core/__init__.py,sha256=bgIhoLSNMQAno1ICwhMfEhEZQMHqVCwEcnKvxZuXd70,95
 openai_parallel_toolkit/core/main.py,sha256=omai73kazjZ_8iHOaayG0jlfyPxwGUc8tYQ3M8bhQ2g,4532
 openai_parallel_toolkit/core/multithread.py,sha256=v8GPaJ7Wukxfv43i1szqreOvtCgzbK6yjh_PkiZ3qnY,4852
 openai_parallel_toolkit/utils/__init__.py,sha256=CyPVG9jS8tZGfoi5k-tFIyE9OKkyZ10vc7Ri91jOScM,148
 openai_parallel_toolkit/utils/logger.py,sha256=6PnPaAsBTr0PnA8tslgR0L7WSQcMZF08e8iqv-_Tvjo,1042
-openai_parallel_toolkit/utils/reader.py,sha256=3V0ZSTwLiJbpUVERTqDFySSN41Bcd94Mm4RaqIcp62Q,4077
+openai_parallel_toolkit/utils/reader.py,sha256=dNg4KLWMZI7-6zn2YGOPtCtg9X0Ogr7Qk2m6iYS3Ipg,4107
 openai_parallel_toolkit/utils/token.py,sha256=lN3oasNGcHesWjoBiIfn5hMwjPYb3wTcRFUCIFtNY4k,913
 openai_parallel_toolkit/utils/tqdm.py,sha256=Xc4ymtGfZzCdbmWdqNR6bAoGDWQWOtjQqvNpvrxv-KY,753
-openai_parallel_toolkit-0.5.0.dist-info/LICENSE,sha256=GcBhJWMnrpUPC70Dvfs6cFG8fLIitA0WwucEgQjGWcw,1063
-openai_parallel_toolkit-0.5.0.dist-info/METADATA,sha256=mtksCsqHkGonCtrUDfMvuKqmMQRwnCIoPHmWu-JDhmo,14633
-openai_parallel_toolkit-0.5.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-openai_parallel_toolkit-0.5.0.dist-info/top_level.txt,sha256=EaHQWFuNRtse4G2kzDTEMstiiaGFy0zIAHBJ0Mm9a_E,24
-openai_parallel_toolkit-0.5.0.dist-info/RECORD,,
+openai_parallel_toolkit-0.5.1.dist-info/LICENSE,sha256=GcBhJWMnrpUPC70Dvfs6cFG8fLIitA0WwucEgQjGWcw,1063
+openai_parallel_toolkit-0.5.1.dist-info/METADATA,sha256=QA4Iq82sdP1Vsx-w7NQUrVEFq8NfeJ48mFtK9y4MxFQ,13483
+openai_parallel_toolkit-0.5.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+openai_parallel_toolkit-0.5.1.dist-info/top_level.txt,sha256=EaHQWFuNRtse4G2kzDTEMstiiaGFy0zIAHBJ0Mm9a_E,24
+openai_parallel_toolkit-0.5.1.dist-info/RECORD,,
```

