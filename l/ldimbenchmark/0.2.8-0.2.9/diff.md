# Comparing `tmp/ldimbenchmark-0.2.8.tar.gz` & `tmp/ldimbenchmark-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ldimbenchmark-0.2.8.tar", max compression
+gzip compressed data, was "ldimbenchmark-0.2.9.tar", max compression
```

## Comparing `ldimbenchmark-0.2.8.tar` & `ldimbenchmark-0.2.9.tar`

### file list

```diff
@@ -1,40 +1,44 @@
--rw-r--r--   0        0        0     3330 2023-05-22 05:33:47.340415 ldimbenchmark-0.2.8/README.md
--rw-r--r--   0        0        0     2359 2023-05-22 05:34:04.176545 ldimbenchmark-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      158 2023-05-22 05:33:47.364415 ldimbenchmark-0.2.8/src/ldimbenchmark/__init__.py
--rw-r--r--   0        0        0       60 2023-05-22 05:33:47.364415 ldimbenchmark-0.2.8/src/ldimbenchmark/benchmark/__init__.py
--rw-r--r--   0        0        0    38982 2023-05-22 05:33:47.364415 ldimbenchmark-0.2.8/src/ldimbenchmark/benchmark/benchmark.py
--rw-r--r--   0        0        0     2926 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/benchmark/results.py
--rw-r--r--   0        0        0     6456 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/benchmark/runners/BaseMethodRunner.py
--rw-r--r--   0        0        0     8690 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/benchmark/runners/DockerMethodRunner.py
--rw-r--r--   0        0        0     3467 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/benchmark/runners/FileMethodRunner.py
--rw-r--r--   0        0        0     7945 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/benchmark/runners/LocalMethodRunner.py
--rw-r--r--   0        0        0      195 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/benchmark/runners/__init__.py
--rw-r--r--   0        0        0     8019 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/benchmark_complexity.py
--rw-r--r--   0        0        0     6578 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/benchmark_evaluation.py
--rw-r--r--   0        0        0    10115 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/classes.py
--rw-r--r--   0        0        0     3928 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/cli.py
--rw-r--r--   0        0        0      176 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/constants.py
--rw-r--r--   0        0        0      211 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/datasets/__init__.py
--rw-r--r--   0        0        0    10884 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/datasets/analysis.py
--rw-r--r--   0        0        0    18617 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/datasets/classes.py
--rw-r--r--   0        0        0    11765 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/datasets/derivation.py
--rw-r--r--   0        0        0     1285 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/datasets/derivation_show.py
--rw-r--r--   0        0        0     2087 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/datasets/library.py
--rw-r--r--   0        0        0        0 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/datasets/loaders/__init__.py
--rw-r--r--   0        0        0     9939 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/datasets/loaders/load_battledim.py
--rw-r--r--   0        0        0      880 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/datasets/loaders/load_dataset_base.py
--rw-r--r--   0        0        0     1288 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/evaluation_metrics/__init__.py
--rw-r--r--   0        0        0     9680 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/generator/__init__.py
--rw-r--r--   0        0        0    12993 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/generator/dataset_generator.py
--rw-r--r--   0        0        0     6332 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/generator/poulakis_network.py
--rw-r--r--   0        0        0      158 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/methods/__init__.py
--rw-r--r--   0        0        0    13338 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/methods/dualmethod.py
--rw-r--r--   0        0        0    19401 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/methods/lila.py
--rw-r--r--   0        0        0    10445 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/methods/mnf.py
--rw-r--r--   0        0        0     1171 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/methods/null.py
--rw-r--r--   0        0        0     2033 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/methods/random.py
--rw-r--r--   0        0        0        0 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/methods/utils/__init__.py
--rw-r--r--   0        0        0     5309 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/methods/utils/cusum.py
--rw-r--r--   0        0        0     8349 2023-05-22 05:33:47.368415 ldimbenchmark-0.2.8/src/ldimbenchmark/utilities.py
--rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 ldimbenchmark-0.2.8/setup.py
--rw-r--r--   0        0        0     4517 1970-01-01 00:00:00.000000 ldimbenchmark-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     3330 2023-05-22 12:17:28.373792 ldimbenchmark-0.2.9/README.md
+-rw-r--r--   0        0        0     2359 2023-05-22 12:17:37.233717 ldimbenchmark-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      158 2023-05-22 12:17:28.393792 ldimbenchmark-0.2.9/src/ldimbenchmark/__init__.py
+-rw-r--r--   0        0        0       60 2023-05-22 12:17:28.393792 ldimbenchmark-0.2.9/src/ldimbenchmark/benchmark/__init__.py
+-rw-r--r--   0        0        0    38982 2023-05-22 12:17:28.393792 ldimbenchmark-0.2.9/src/ldimbenchmark/benchmark/benchmark.py
+-rw-r--r--   0        0        0     2926 2023-05-22 12:17:28.393792 ldimbenchmark-0.2.9/src/ldimbenchmark/benchmark/results.py
+-rw-r--r--   0        0        0     6456 2023-05-22 12:17:28.393792 ldimbenchmark-0.2.9/src/ldimbenchmark/benchmark/runners/BaseMethodRunner.py
+-rw-r--r--   0        0        0     8690 2023-05-22 12:17:28.393792 ldimbenchmark-0.2.9/src/ldimbenchmark/benchmark/runners/DockerMethodRunner.py
+-rw-r--r--   0        0        0     3467 2023-05-22 12:17:28.393792 ldimbenchmark-0.2.9/src/ldimbenchmark/benchmark/runners/FileMethodRunner.py
+-rw-r--r--   0        0        0     7945 2023-05-22 12:17:28.393792 ldimbenchmark-0.2.9/src/ldimbenchmark/benchmark/runners/LocalMethodRunner.py
+-rw-r--r--   0        0        0      195 2023-05-22 12:17:28.393792 ldimbenchmark-0.2.9/src/ldimbenchmark/benchmark/runners/__init__.py
+-rw-r--r--   0        0        0     8019 2023-05-22 12:17:28.393792 ldimbenchmark-0.2.9/src/ldimbenchmark/benchmark_complexity.py
+-rw-r--r--   0        0        0     6578 2023-05-22 12:17:28.393792 ldimbenchmark-0.2.9/src/ldimbenchmark/benchmark_evaluation.py
+-rw-r--r--   0        0        0    10115 2023-05-22 12:17:28.393792 ldimbenchmark-0.2.9/src/ldimbenchmark/classes.py
+-rw-r--r--   0        0        0     3928 2023-05-22 12:17:28.393792 ldimbenchmark-0.2.9/src/ldimbenchmark/cli.py
+-rw-r--r--   0        0        0      176 2023-05-22 12:17:28.393792 ldimbenchmark-0.2.9/src/ldimbenchmark/constants.py
+-rw-r--r--   0        0        0      211 2023-05-22 12:17:28.393792 ldimbenchmark-0.2.9/src/ldimbenchmark/datasets/__init__.py
+-rw-r--r--   0        0        0    10884 2023-05-22 12:17:28.393792 ldimbenchmark-0.2.9/src/ldimbenchmark/datasets/analysis.py
+-rw-r--r--   0        0        0    18617 2023-05-22 12:17:28.393792 ldimbenchmark-0.2.9/src/ldimbenchmark/datasets/classes.py
+-rw-r--r--   0        0        0    11765 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/datasets/derivation.py
+-rw-r--r--   0        0        0     1285 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/datasets/derivation_show.py
+-rw-r--r--   0        0        0     2087 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/datasets/library.py
+-rw-r--r--   0        0        0        0 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/datasets/loaders/__init__.py
+-rw-r--r--   0        0        0     9939 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/datasets/loaders/load_battledim.py
+-rw-r--r--   0        0        0      880 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/datasets/loaders/load_dataset_base.py
+-rw-r--r--   0        0        0     1288 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/evaluation_metrics/__init__.py
+-rw-r--r--   0        0        0     9680 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/generator/__init__.py
+-rw-r--r--   0        0        0    12993 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/generator/dataset_generator.py
+-rw-r--r--   0        0        0     6332 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/generator/poulakis_network.py
+-rw-r--r--   0        0        0      158 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/methods/__init__.py
+-rw-r--r--   0        0        0    13338 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/methods/dualmethod.py
+-rw-r--r--   0        0        0    19401 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/methods/lila.py
+-rw-r--r--   0        0        0    10445 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/methods/mnf.py
+-rw-r--r--   0        0        0     1171 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/methods/null.py
+-rw-r--r--   0        0        0     2033 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/methods/random.py
+-rw-r--r--   0        0        0     1208 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/methods/test_complexity_constant.py
+-rw-r--r--   0        0        0     1418 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/methods/test_complexity_exponential.py
+-rw-r--r--   0        0        0     1390 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/methods/test_complexity_linear.py
+-rw-r--r--   0        0        0     1406 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/methods/test_complexity_polynomial.py
+-rw-r--r--   0        0        0        0 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/methods/utils/__init__.py
+-rw-r--r--   0        0        0     5309 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/methods/utils/cusum.py
+-rw-r--r--   0        0        0     8349 2023-05-22 12:17:28.397792 ldimbenchmark-0.2.9/src/ldimbenchmark/utilities.py
+-rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 ldimbenchmark-0.2.9/setup.py
+-rw-r--r--   0        0        0     4517 1970-01-01 00:00:00.000000 ldimbenchmark-0.2.9/PKG-INFO
```

### Comparing `ldimbenchmark-0.2.8/README.md` & `ldimbenchmark-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/pyproject.toml` & `ldimbenchmark-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ldimbenchmark"
-version = "0.2.8"
+version = "0.2.9"
 description = ""
 authors = ["DanielHabenicht <daniel-habenicht@outlook.de>"]
 readme = "README.md"
 exclude = [
     "tests",
     "experiments"
 ]
```

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/benchmark/benchmark.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/benchmark/results.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/benchmark/results.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/benchmark/runners/BaseMethodRunner.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/benchmark/runners/BaseMethodRunner.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/benchmark/runners/DockerMethodRunner.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/benchmark/runners/DockerMethodRunner.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/benchmark/runners/FileMethodRunner.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/benchmark/runners/FileMethodRunner.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/benchmark/runners/LocalMethodRunner.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/benchmark/runners/LocalMethodRunner.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/benchmark_complexity.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/benchmark_complexity.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/benchmark_evaluation.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/benchmark_evaluation.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/classes.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/classes.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/cli.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/cli.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/datasets/analysis.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/datasets/analysis.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/datasets/classes.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/datasets/classes.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/datasets/derivation.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/datasets/derivation.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/datasets/derivation_show.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/datasets/derivation_show.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/datasets/library.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/datasets/library.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/datasets/loaders/load_battledim.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/datasets/loaders/load_battledim.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/datasets/loaders/load_dataset_base.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/datasets/loaders/load_dataset_base.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/evaluation_metrics/__init__.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/evaluation_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/generator/__init__.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/generator/dataset_generator.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/generator/dataset_generator.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/generator/poulakis_network.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/generator/poulakis_network.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/methods/dualmethod.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/methods/dualmethod.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/methods/lila.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/methods/lila.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/methods/mnf.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/methods/mnf.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/methods/null.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/methods/null.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/methods/random.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/methods/random.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/methods/utils/cusum.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/methods/utils/cusum.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/src/ldimbenchmark/utilities.py` & `ldimbenchmark-0.2.9/src/ldimbenchmark/utilities.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.8/setup.py` & `ldimbenchmark-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
  'wntr>=0.5.0,<0.6.0']
 
 entry_points = \
 {'console_scripts': ['ldimbenchmark = ldimbenchmark.cli:cli']}
 
 setup_kwargs = {
     'name': 'ldimbenchmark',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': '',
     'long_description': '[![ldimbenchmark version](https://badgen.net/pypi/v/ldimbenchmark/)](https://pypi.org/project/ldimbenchmark)\n[![Documentation badge](https://img.shields.io/badge/Documentation-here!-GREEN.svg)](https://tumt2022.github.io/LDIMBench/)\n\n# LDIMBenchmark\n\nLeakage Detection and Isolation Methods Benchmark\n\n> Instead of collecting all the different dataset to benchmark different methods on. We wanted to create a Benchmarking Tool which makes it easy to reproduce the results of the different methods locally on your own dataset.\n\nIt provides a close to real-world conditions environment and forces researchers to provide a reproducible method implementation, which is supposed to run automated on any input dataset, thus hindering custom solutions which work well in one specific case.\n\n## Usage\n\n### Installation\n\n```bash\npip install ldimbenchmark\n```\n\n### Python\n\n```python\nfrom ldimbenchmark.datasets import DatasetLibrary, DATASETS\nfrom ldimbenchmark import (\n    LDIMBenchmark,\n    BenchmarkData,\n    BenchmarkLeakageResult,\n)\nfrom ldimbenchmark.classes import LDIMMethodBase\nfrom typing import List\n\nclass YourCustomLDIMMethod(LDIMMethodBase):\n    def __init__(self):\n        super().__init__(\n            name="YourCustomLDIMMethod",\n            version="0.1.0"\n        )\n\n    def train(self, data: BenchmarkData):\n        pass\n\n    def detect(self, data: BenchmarkData) -> List[BenchmarkLeakageResult]:\n        return [\n            {\n                "leak_start": "2020-01-01",\n                "leak_end": "2020-01-02",\n                "leak_area": 0.2,\n                "pipe_id": "test",\n            }\n        ]\n\n    def detect_datapoint(self, evaluation_data) -> BenchmarkLeakageResult:\n        return {}\n\n\ndatasets = DatasetLibrary("datasets").download(DATASETS.BATTLEDIM)\n\nlocal_methods = [YourCustomLDIMMethod()]\n\nhyperparameters = {}\n\nbenchmark = LDIMBenchmark(\n    hyperparameters, datasets, results_dir="./benchmark-results"\n)\nbenchmark.add_local_methods(local_methods)\n\nbenchmark.run_benchmark()\n\nbenchmark.evaluate()\n```\n\n### CLI\n\n```bash\nldimbenchmark --help\n```\n\n## Roadmap\n\n- v1: Just Leakage Detection\n- v2: Provides Benchmark of Isolation Methods\n\nhttps://mathspp.com/blog/how-to-create-a-python-package-in-2022\n\n## Development\n\nhttps://python-poetry.org/docs/basic-usage/\n\n```bash\n# python 3.10\n# Use Environment\npoetry config virtualenvs.in-project true\npoetry shell\npoetry install --without ci # --with ci\n\n\n# Test\npoetry build\ncp -r dist tests/dist\ncd tests\ndocker build . -t testmethod\npytest -s -o log_cli=true\npytest tests/test_derivation.py -k \'test_mything\'\npytest --testmon\npytest --snapshot-update\n\n# Pytest watch\nptw\nptw -- --testmon\n\n# Watch a file during development\nnpm install -g nodemon\nnodemon -L experiments/auto_hyperparameter.py\n\n# Test-Publish\npoetry config repositories.testpypi https://test.pypi.org/legacy/\npoetry config http-basic.testpypi __token__ pypi-your-api-token-here\npoetry build\npoetry publish -r testpypi\n\n# Real Publish\npoetry config pypi-token.pypi pypi-your-token-here\n```\n\n### Documentation\n\nhttps://squidfunk.github.io/mkdocs-material/\nhttps://click.palletsprojects.com/en/8.1.x/\n\n```\nmkdocs serve\n```\n\n# TODO\n\nLDIMBenchmark:\nData Cleansing before working with them\n\n- per sensor type, e.g. waterflow (cut of at 0)\n- removing datapoints which are clearly a malfunction\n',
     'author': 'DanielHabenicht',
     'author_email': 'daniel-habenicht@outlook.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ldimbenchmark-0.2.8/PKG-INFO` & `ldimbenchmark-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldimbenchmark
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 Author: DanielHabenicht
 Author-email: daniel-habenicht@outlook.de
 Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

