# Comparing `tmp/openai_parallel_toolkit-0.5.1-py3-none-any.whl.zip` & `tmp/openai_parallel_toolkit-0.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 18533 bytes, number of entries: 19
--rw-r--r--  2.0 unx      147 b- defN 23-Jun-19 11:22 openai_parallel_toolkit/__init__.py
+Zip file size: 18556 bytes, number of entries: 19
+-rw-r--r--  2.0 unx      184 b- defN 23-Jun-26 03:34 openai_parallel_toolkit/__init__.py
 -rw-r--r--  2.0 unx       20 b- defN 23-May-17 01:58 openai_parallel_toolkit/config.py
--rw-r--r--  2.0 unx      113 b- defN 23-May-17 12:36 openai_parallel_toolkit/api/__init__.py
+-rw-r--r--  2.0 unx      150 b- defN 23-Jun-26 03:34 openai_parallel_toolkit/api/__init__.py
 -rw-r--r--  2.0 unx     5216 b- defN 23-Jun-19 07:03 openai_parallel_toolkit/api/api.py
 -rw-r--r--  2.0 unx     5809 b- defN 23-May-23 12:55 openai_parallel_toolkit/api/keys.py
 -rw-r--r--  2.0 unx     3034 b- defN 23-May-25 08:28 openai_parallel_toolkit/api/request.py
 -rw-r--r--  2.0 unx       95 b- defN 23-May-17 01:02 openai_parallel_toolkit/core/__init__.py
 -rw-r--r--  2.0 unx     4532 b- defN 23-May-25 08:13 openai_parallel_toolkit/core/main.py
 -rw-r--r--  2.0 unx     4852 b- defN 23-May-18 11:47 openai_parallel_toolkit/core/multithread.py
 -rw-r--r--  2.0 unx      148 b- defN 23-Jun-19 11:22 openai_parallel_toolkit/utils/__init__.py
 -rw-r--r--  2.0 unx     1042 b- defN 23-May-18 11:32 openai_parallel_toolkit/utils/logger.py
 -rw-r--r--  2.0 unx     4107 b- defN 23-Jun-26 03:26 openai_parallel_toolkit/utils/reader.py
 -rw-r--r--  2.0 unx      913 b- defN 23-May-17 11:15 openai_parallel_toolkit/utils/token.py
 -rw-r--r--  2.0 unx      753 b- defN 23-May-18 11:47 openai_parallel_toolkit/utils/tqdm.py
--rw-r--r--  2.0 unx     1063 b- defN 23-Jun-26 03:29 openai_parallel_toolkit-0.5.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    13483 b- defN 23-Jun-26 03:29 openai_parallel_toolkit-0.5.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 03:29 openai_parallel_toolkit-0.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-Jun-26 03:29 openai_parallel_toolkit-0.5.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1783 b- defN 23-Jun-26 03:29 openai_parallel_toolkit-0.5.1.dist-info/RECORD
-19 files, 47226 bytes uncompressed, 15535 bytes compressed:  67.1%
+-rw-r--r--  2.0 unx     1063 b- defN 23-Jun-26 03:34 openai_parallel_toolkit-0.5.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13483 b- defN 23-Jun-26 03:34 openai_parallel_toolkit-0.5.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 03:34 openai_parallel_toolkit-0.5.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-Jun-26 03:34 openai_parallel_toolkit-0.5.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1783 b- defN 23-Jun-26 03:34 openai_parallel_toolkit-0.5.2.dist-info/RECORD
+19 files, 47300 bytes uncompressed, 15558 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: openai_parallel_toolkit/utils/token.py
 Comment: 
 
 Filename: openai_parallel_toolkit/utils/tqdm.py
 Comment: 
 
-Filename: openai_parallel_toolkit-0.5.1.dist-info/LICENSE
+Filename: openai_parallel_toolkit-0.5.2.dist-info/LICENSE
 Comment: 
 
-Filename: openai_parallel_toolkit-0.5.1.dist-info/METADATA
+Filename: openai_parallel_toolkit-0.5.2.dist-info/METADATA
 Comment: 
 
-Filename: openai_parallel_toolkit-0.5.1.dist-info/WHEEL
+Filename: openai_parallel_toolkit-0.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: openai_parallel_toolkit-0.5.1.dist-info/top_level.txt
+Filename: openai_parallel_toolkit-0.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: openai_parallel_toolkit-0.5.1.dist-info/RECORD
+Filename: openai_parallel_toolkit-0.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openai_parallel_toolkit/__init__.py

```diff
@@ -1,2 +1,2 @@
-from .api import APIKeyManager, Gpt35Turbo, OpenAIModel, request_openai_api
+from .api import APIKeyManager, Gpt35Turbo, OpenAIModel, request_openai_api, Gpt35Turbo0613, Gpt4, Gpt35Turbo16K
 from .core import ParallelToolkit, multi_process_one, multi_thread_run
```

## openai_parallel_toolkit/api/__init__.py

```diff
@@ -1,3 +1,3 @@
-from .api import OpenAIModel, Gpt35Turbo
+from .api import OpenAIModel, Gpt35Turbo, Gpt35Turbo0613, Gpt4, Gpt35Turbo16K
 from .keys import APIKeyManager
 from .request import request_openai_api
```

## Comparing `openai_parallel_toolkit-0.5.1.dist-info/LICENSE` & `openai_parallel_toolkit-0.5.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `openai_parallel_toolkit-0.5.1.dist-info/METADATA` & `openai_parallel_toolkit-0.5.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-parallel-toolkit
-Version: 0.5.1
+Version: 0.5.2
 Summary: OpenAI-Parallel-Toolkit is a Python library for handling multiple OpenAI API keys and parallel tasks. It provides API key rotation, multithreading for faster task execution, and utility functions to boost your OpenAI integration. Ideal for efficient large-scale OpenAI usage.
 Home-page: https://github.com/CZT0/OpenAI-Parallel-Toolkit
 Author: Jellow
 Author-email: dvdx@foxmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `openai_parallel_toolkit-0.5.1.dist-info/RECORD` & `openai_parallel_toolkit-0.5.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-openai_parallel_toolkit/__init__.py,sha256=doqRzVrcQRtSVspTP1V4IgTEnRR4Lwm6iZ5UFHGZpzo,147
+openai_parallel_toolkit/__init__.py,sha256=u44miRj78hpYdl4SdE_USz7GLANZzosBMUbPQ9okyzs,184
 openai_parallel_toolkit/config.py,sha256=UvWwqK1cxCx4XId6pswW4jkSF1XDozEg58RftfY8yxU,20
-openai_parallel_toolkit/api/__init__.py,sha256=eabIIe9ATUy6StxNz50Ul9Dr7iPPuc3I7ebAyGWvNLQ,113
+openai_parallel_toolkit/api/__init__.py,sha256=wAUTdp_SZKJL0yQiRnEIhDo505fAOdLW7UeAg33z9_I,150
 openai_parallel_toolkit/api/api.py,sha256=KJgFQ_fZebwS0jxMiD0kzgPgpPWOH7DeEB7hvVqPBtU,5216
 openai_parallel_toolkit/api/keys.py,sha256=RB9BmU7Qth3QIUWP30KXcfgmyblWVFYUnH0uB538ISs,5809
 openai_parallel_toolkit/api/request.py,sha256=75V3R79jE055WovuwQp7Pp29Ib_NUCDbFFqYVyaBA0w,3034
 openai_parallel_toolkit/core/__init__.py,sha256=bgIhoLSNMQAno1ICwhMfEhEZQMHqVCwEcnKvxZuXd70,95
 openai_parallel_toolkit/core/main.py,sha256=omai73kazjZ_8iHOaayG0jlfyPxwGUc8tYQ3M8bhQ2g,4532
 openai_parallel_toolkit/core/multithread.py,sha256=v8GPaJ7Wukxfv43i1szqreOvtCgzbK6yjh_PkiZ3qnY,4852
 openai_parallel_toolkit/utils/__init__.py,sha256=CyPVG9jS8tZGfoi5k-tFIyE9OKkyZ10vc7Ri91jOScM,148
 openai_parallel_toolkit/utils/logger.py,sha256=6PnPaAsBTr0PnA8tslgR0L7WSQcMZF08e8iqv-_Tvjo,1042
 openai_parallel_toolkit/utils/reader.py,sha256=dNg4KLWMZI7-6zn2YGOPtCtg9X0Ogr7Qk2m6iYS3Ipg,4107
 openai_parallel_toolkit/utils/token.py,sha256=lN3oasNGcHesWjoBiIfn5hMwjPYb3wTcRFUCIFtNY4k,913
 openai_parallel_toolkit/utils/tqdm.py,sha256=Xc4ymtGfZzCdbmWdqNR6bAoGDWQWOtjQqvNpvrxv-KY,753
-openai_parallel_toolkit-0.5.1.dist-info/LICENSE,sha256=GcBhJWMnrpUPC70Dvfs6cFG8fLIitA0WwucEgQjGWcw,1063
-openai_parallel_toolkit-0.5.1.dist-info/METADATA,sha256=QA4Iq82sdP1Vsx-w7NQUrVEFq8NfeJ48mFtK9y4MxFQ,13483
-openai_parallel_toolkit-0.5.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-openai_parallel_toolkit-0.5.1.dist-info/top_level.txt,sha256=EaHQWFuNRtse4G2kzDTEMstiiaGFy0zIAHBJ0Mm9a_E,24
-openai_parallel_toolkit-0.5.1.dist-info/RECORD,,
+openai_parallel_toolkit-0.5.2.dist-info/LICENSE,sha256=GcBhJWMnrpUPC70Dvfs6cFG8fLIitA0WwucEgQjGWcw,1063
+openai_parallel_toolkit-0.5.2.dist-info/METADATA,sha256=C5Z5FoI2YsPsQciP1abzPMc735Y33_igKnwQ3A5f4gA,13483
+openai_parallel_toolkit-0.5.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+openai_parallel_toolkit-0.5.2.dist-info/top_level.txt,sha256=EaHQWFuNRtse4G2kzDTEMstiiaGFy0zIAHBJ0Mm9a_E,24
+openai_parallel_toolkit-0.5.2.dist-info/RECORD,,
```

