# Comparing `tmp/zdatasets-0.2.5.tar.gz` & `tmp/zdatasets-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zdatasets-0.2.5.tar", max compression
+gzip compressed data, was "zdatasets-1.2.5.tar", max compression
```

## Comparing `zdatasets-0.2.5.tar` & `zdatasets-1.2.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    11357 2023-04-27 19:33:50.998113 zdatasets-0.2.5/LICENSE
--rw-r--r--   0        0        0     1872 2023-04-27 19:33:50.998113 zdatasets-0.2.5/README.md
--rw-r--r--   0        0        0      431 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/__init__.py
--rw-r--r--   0        0        0      387 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/_typing.py
--rw-r--r--   0        0        0      269 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/context.py
--rw-r--r--   0        0        0     8435 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/dataset_plugin.py
--rwxr-xr-x   0        0        0     1828 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/datasets_decorator.py
--rw-r--r--   0        0        0       53 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/exceptions.py
--rw-r--r--   0        0        0     4452 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/metaflow.py
--rw-r--r--   0        0        0      295 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/mode.py
--rw-r--r--   0        0        0      404 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/plugins/batch/__init__.py
--rw-r--r--   0        0        0     6064 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/plugins/batch/batch_base_plugin.py
--rw-r--r--   0        0        0     9814 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/plugins/batch/batch_dataset.py
--rw-r--r--   0        0        0     2084 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/plugins/batch/flow_dataset.py
--rw-r--r--   0        0        0    10225 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/plugins/batch/hive_dataset.py
--rw-r--r--   0        0        0        0 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/plugins/executors/__init__.py
--rw-r--r--   0        0        0     1172 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/plugins/executors/metaflow_executor.py
--rw-r--r--   0        0        0      752 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/plugins/register_plugins.py
--rw-r--r--   0        0        0      850 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/program_executor.py
--rw-r--r--   0        0        0        0 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/__init__.py
--rw-r--r--   0        0        0     1887 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/conftest.py
--rw-r--r--   0        0        0    21810 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/data/train/date=2020-07-23/region=king/data.parquet
--rw-r--r--   0        0        0    21810 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/data/train/date=2020-07-23/region=la/data.parquet
--rw-r--r--   0        0        0     9280 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/test_batch_dataset.py
--rw-r--r--   0        0        0    11420 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/test_dataset_plugin.py
--rw-r--r--   0        0        0     1489 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/test_datasets_decorator.py
--rw-r--r--   0        0        0      842 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/test_flow_dataset.py
--rw-r--r--   0        0        0    11095 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/test_hive_dataset.py
--rw-r--r--   0        0        0     4748 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/test_metaflow.py
--rw-r--r--   0        0        0     2173 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/test_tutorials.py
--rw-r--r--   0        0        0        0 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/utils/__init__.py
--rw-r--r--   0        0        0     1270 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/utils/test_case_utils.py
--rw-r--r--   0        0        0     2195 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/utils/test_partitions.py
--rw-r--r--   0        0        0     7252 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/utils/test_secret_fetcher.py
--rwxr-xr-x   0        0        0     1433 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tutorials/0_hello_dataset_flow.py
--rwxr-xr-x   0        0        0     1093 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tutorials/1_input_output_flow.py
--rwxr-xr-x   0        0        0      818 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tutorials/2_spark_dask_flow.py
--rwxr-xr-x   0        0        0     1449 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tutorials/3_foreach_dataset_flow.py
--rwxr-xr-x   0        0        0      910 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tutorials/4_hello_plugin_flow.py
--rwxr-xr-x   0        0        0     1450 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tutorials/5_consistent_flow.py
--rwxr-xr-x   0        0        0     1395 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tutorials/6_hive_dataset_flow.py
--rw-r--r--   0        0        0     3762 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tutorials/README.ipynb
--rw-r--r--   0        0        0     1751 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tutorials/online_plugin.py
--rw-r--r--   0        0        0       63 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/utils/__init__.py
--rw-r--r--   0        0        0     4075 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/utils/aws.py
--rw-r--r--   0        0        0     1079 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/utils/case_utils.py
--rw-r--r--   0        0        0     2374 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/utils/partitions.py
--rw-r--r--   0        0        0     9584 2023-04-27 19:33:51.006113 zdatasets-0.2.5/datasets/utils/secret_fetcher.py
--rw-r--r--   0        0        0     2073 2023-04-27 19:33:51.006113 zdatasets-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3085 1970-01-01 00:00:00.000000 zdatasets-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-26 16:43:16.965031 zdatasets-1.2.5/LICENSE
+-rw-r--r--   0        0        0     1878 2023-06-26 16:43:16.965031 zdatasets-1.2.5/README.md
+-rw-r--r--   0        0        0     2082 2023-06-26 16:43:16.965031 zdatasets-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0      439 2023-06-26 16:43:16.965031 zdatasets-1.2.5/zdatasets/__init__.py
+-rw-r--r--   0        0        0      387 2023-06-26 16:43:16.965031 zdatasets-1.2.5/zdatasets/_typing.py
+-rw-r--r--   0        0        0      269 2023-06-26 16:43:16.965031 zdatasets-1.2.5/zdatasets/context.py
+-rw-r--r--   0        0        0     8438 2023-06-26 16:43:16.965031 zdatasets-1.2.5/zdatasets/dataset_plugin.py
+-rwxr-xr-x   0        0        0     1832 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/datasets_decorator.py
+-rw-r--r--   0        0        0       53 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/exceptions.py
+-rw-r--r--   0        0        0     4458 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/metaflow.py
+-rw-r--r--   0        0        0      295 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/mode.py
+-rw-r--r--   0        0        0      409 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/plugins/batch/__init__.py
+-rw-r--r--   0        0        0     6069 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/plugins/batch/batch_base_plugin.py
+-rw-r--r--   0        0        0     9820 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/plugins/batch/batch_dataset.py
+-rw-r--r--   0        0        0     2089 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/plugins/batch/flow_dataset.py
+-rw-r--r--   0        0        0    10232 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/plugins/batch/hive_dataset.py
+-rw-r--r--   0        0        0        0 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/plugins/executors/__init__.py
+-rw-r--r--   0        0        0     1174 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/plugins/executors/metaflow_executor.py
+-rw-r--r--   0        0        0      756 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/plugins/register_plugins.py
+-rw-r--r--   0        0        0      852 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/program_executor.py
+-rw-r--r--   0        0        0        0 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/tests/__init__.py
+-rw-r--r--   0        0        0     1890 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/tests/conftest.py
+-rw-r--r--   0        0        0    21810 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/tests/data/train/date=2020-07-23/region=king/data.parquet
+-rw-r--r--   0        0        0    21810 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/tests/data/train/date=2020-07-23/region=la/data.parquet
+-rw-r--r--   0        0        0     9287 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/tests/test_batch_dataset.py
+-rw-r--r--   0        0        0    11428 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/tests/test_dataset_plugin.py
+-rw-r--r--   0        0        0     1491 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/tests/test_datasets_decorator.py
+-rw-r--r--   0        0        0      844 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/tests/test_flow_dataset.py
+-rw-r--r--   0        0        0    11100 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/tests/test_hive_dataset.py
+-rw-r--r--   0        0        0     4758 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/tests/test_metaflow.py
+-rw-r--r--   0        0        0     2174 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/tests/test_tutorials.py
+-rw-r--r--   0        0        0        0 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1271 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/tests/utils/test_case_utils.py
+-rw-r--r--   0        0        0     2197 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/tests/utils/test_partitions.py
+-rw-r--r--   0        0        0     7257 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/tests/utils/test_secret_fetcher.py
+-rwxr-xr-x   0        0        0     1437 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/tutorials/0_hello_dataset_flow.py
+-rwxr-xr-x   0        0        0     1095 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/tutorials/1_input_output_flow.py
+-rwxr-xr-x   0        0        0      820 2023-06-26 16:43:16.969031 zdatasets-1.2.5/zdatasets/tutorials/2_spark_dask_flow.py
+-rwxr-xr-x   0        0        0     1451 2023-06-26 16:43:16.973031 zdatasets-1.2.5/zdatasets/tutorials/3_foreach_dataset_flow.py
+-rwxr-xr-x   0        0        0      915 2023-06-26 16:43:16.973031 zdatasets-1.2.5/zdatasets/tutorials/4_hello_plugin_flow.py
+-rwxr-xr-x   0        0        0     1456 2023-06-26 16:43:16.973031 zdatasets-1.2.5/zdatasets/tutorials/5_consistent_flow.py
+-rwxr-xr-x   0        0        0     1399 2023-06-26 16:43:16.973031 zdatasets-1.2.5/zdatasets/tutorials/6_hive_dataset_flow.py
+-rw-r--r--   0        0        0     3762 2023-06-26 16:43:16.973031 zdatasets-1.2.5/zdatasets/tutorials/README.ipynb
+-rw-r--r--   0        0        0     1753 2023-06-26 16:43:16.973031 zdatasets-1.2.5/zdatasets/tutorials/online_plugin.py
+-rw-r--r--   0        0        0       63 2023-06-26 16:43:16.973031 zdatasets-1.2.5/zdatasets/utils/__init__.py
+-rw-r--r--   0        0        0     4075 2023-06-26 16:43:16.973031 zdatasets-1.2.5/zdatasets/utils/aws.py
+-rw-r--r--   0        0        0     1079 2023-06-26 16:43:16.973031 zdatasets-1.2.5/zdatasets/utils/case_utils.py
+-rw-r--r--   0        0        0     2375 2023-06-26 16:43:16.973031 zdatasets-1.2.5/zdatasets/utils/partitions.py
+-rw-r--r--   0        0        0     9584 2023-06-26 16:43:16.973031 zdatasets-1.2.5/zdatasets/utils/secret_fetcher.py
+-rw-r--r--   0        0        0     3041 1970-01-01 00:00:00.000000 zdatasets-1.2.5/PKG-INFO
```

### Comparing `zdatasets-0.2.5/LICENSE` & `zdatasets-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.5/README.md` & `zdatasets-1.2.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 ![Tests](https://github.com/zillow/datasets/actions/workflows/test.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/zillow/datasets/badge.svg)](https://coveralls.io/github/zillow/datasets)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zillow/datasets/main?urlpath=lab/tree/datasets/tutorials)
 
 
-Welcome to @datasets
+# Welcome to zdatasets
 ==================================================
 
 TODO
 
 ```python
 import pandas as pd
 from metaflow import FlowSpec, step
 
-from datasets import Dataset, Mode
-from datasets.metaflow import DatasetParameter
-from datasets.plugins import BatchOptions
+from zdatasets import Dataset, Mode
+from zdatasets.metaflow import DatasetParameter
+from zdatasets.plugins import BatchOptions
 
 
 # Can also invoke from CLI:
-#  > python datasets/tutorials/0_hello_dataset_flow.py run \
+#  > python zdatasets/tutorials/0_hello_dataset_flow.py run \
 #    --hello_dataset '{"name": "HelloDataset", "mode": "READ_WRITE", \
 #    "options": {"type": "BatchOptions", "partition_by": "region"}}'
 class HelloDatasetFlow(FlowSpec):
     hello_dataset = DatasetParameter(
         "hello_dataset",
         default=Dataset("HelloDataset", mode=Mode.READ_WRITE, options=BatchOptions(partition_by="region")),
     )
```

### Comparing `zdatasets-0.2.5/datasets/dataset_plugin.py` & `zdatasets-1.2.5/zdatasets/dataset_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import dataclasses
 import logging
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Callable, Dict, Iterable, Optional, Tuple, Type, Union
 
-from datasets._typing import ColumnNames, DataFrameType
-from datasets.context import Context
-from datasets.utils.case_utils import is_upper_pascal_case
+from zdatasets._typing import ColumnNames, DataFrameType
+from zdatasets.context import Context
+from zdatasets.utils.case_utils import is_upper_pascal_case
 
 from .mode import Mode
 from .program_executor import ProgramExecutor
 
 
 _logger = logging.getLogger(__name__)
 _logger.setLevel(logging.DEBUG)
```

### Comparing `zdatasets-0.2.5/datasets/datasets_decorator.py` & `zdatasets-1.2.5/zdatasets/datasets_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import functools
 import keyword
 from typing import Callable, Dict, Optional, Union
 
-from datasets._typing import ColumnNames
-from datasets.dataset_plugin import Context, DatasetPlugin, StorageOptions
-from datasets.mode import Mode
-from datasets.utils.case_utils import pascal_to_snake_case
+from zdatasets._typing import ColumnNames
+from zdatasets.dataset_plugin import Context, DatasetPlugin, StorageOptions
+from zdatasets.mode import Mode
+from zdatasets.utils.case_utils import pascal_to_snake_case
 
 
 def dataset(
     name: Optional[str] = None,
     logical_key: Optional[str] = None,
     columns: Optional[ColumnNames] = None,
     run_id: Optional[str] = None,
```

### Comparing `zdatasets-0.2.5/datasets/metaflow.py` & `zdatasets-1.2.5/zdatasets/metaflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import json
 from dataclasses import dataclass
 from typing import Dict, List, Optional, Type, Union
 
 from metaflow._vendor.click import ParamType
 from metaflow.parameters import Parameter
 
-from datasets import DataFrameType
-from datasets._typing import ColumnNames
-from datasets.context import Context
-from datasets.dataset_plugin import DatasetPlugin, StorageOptions
-from datasets.mode import Mode
-from datasets.utils.secret_fetcher import SecretFetcher
+from zdatasets import DataFrameType
+from zdatasets._typing import ColumnNames
+from zdatasets.context import Context
+from zdatasets.dataset_plugin import DatasetPlugin, StorageOptions
+from zdatasets.mode import Mode
+from zdatasets.utils.secret_fetcher import SecretFetcher
 
 
 class _DatasetTypeClass(ParamType):
     name = "Dataset"
 
     def convert(self, value, param, ctx) -> DatasetPlugin:
         if isinstance(value, str):
```

### Comparing `zdatasets-0.2.5/datasets/plugins/batch/batch_base_plugin.py` & `zdatasets-1.2.5/zdatasets/plugins/batch/batch_base_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     Iterable,
     List,
     Optional,
     Tuple,
     Union,
 )
 
-from datasets._typing import ColumnNames, DataFrameType
-from datasets.dataset_plugin import DatasetPlugin, StorageOptions
-from datasets.exceptions import InvalidOperationException
-from datasets.mode import Mode
-from datasets.utils.case_utils import pascal_to_snake_case
+from zdatasets._typing import ColumnNames, DataFrameType
+from zdatasets.dataset_plugin import DatasetPlugin, StorageOptions
+from zdatasets.exceptions import InvalidOperationException
+from zdatasets.mode import Mode
+from zdatasets.utils.case_utils import pascal_to_snake_case
 
 
 _logger = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
     from pyspark import SparkConf
     from pyspark.sql import SparkSession
```

### Comparing `zdatasets-0.2.5/datasets/plugins/batch/batch_dataset.py` & `zdatasets-1.2.5/zdatasets/plugins/batch/batch_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
 from typing import TYPE_CHECKING, List, Optional, Tuple, Union
 
 import pandas as pd
 
-from datasets import Mode
-from datasets._typing import ColumnNames, DataFrameType
-from datasets.context import Context
-from datasets.dataset_plugin import DatasetPlugin
-from datasets.exceptions import InvalidOperationException
-from datasets.plugins.batch.batch_base_plugin import (
+from zdatasets import Mode
+from zdatasets._typing import ColumnNames, DataFrameType
+from zdatasets.context import Context
+from zdatasets.dataset_plugin import DatasetPlugin
+from zdatasets.exceptions import InvalidOperationException
+from zdatasets.plugins.batch.batch_base_plugin import (
     BatchBasePlugin,
     BatchOptions,
 )
 
 
 _logger = logging.getLogger(__name__)
 _logger.setLevel(logging.INFO)
```

### Comparing `zdatasets-0.2.5/datasets/plugins/batch/flow_dataset.py` & `zdatasets-1.2.5/zdatasets/plugins/batch/flow_dataset.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Optional, Tuple, Union
 
-from datasets._typing import ColumnNames
-from datasets.context import Context
-from datasets.dataset_plugin import DatasetPlugin, StorageOptions
-from datasets.mode import Mode
-from datasets.plugins import BatchDataset
+from zdatasets._typing import ColumnNames
+from zdatasets.context import Context
+from zdatasets.dataset_plugin import DatasetPlugin, StorageOptions
+from zdatasets.mode import Mode
+from zdatasets.plugins import BatchDataset
 
 
 if TYPE_CHECKING:
     from metaflow import Run
 
 
 @dataclass
```

### Comparing `zdatasets-0.2.5/datasets/plugins/batch/hive_dataset.py` & `zdatasets-1.2.5/zdatasets/plugins/batch/hive_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import time
 from dataclasses import dataclass
 from functools import partial
 from typing import TYPE_CHECKING, Callable, List, Optional, Union
 
 import pandas as pd
 
-from datasets._typing import ColumnNames
-from datasets.context import Context
-from datasets.dataset_plugin import DatasetPlugin
-from datasets.exceptions import InvalidOperationException
-from datasets.mode import Mode
-from datasets.plugins.batch.batch_base_plugin import (
+from zdatasets._typing import ColumnNames
+from zdatasets.context import Context
+from zdatasets.dataset_plugin import DatasetPlugin
+from zdatasets.exceptions import InvalidOperationException
+from zdatasets.mode import Mode
+from zdatasets.plugins.batch.batch_base_plugin import (
     BatchBasePlugin,
     BatchOptions,
 )
-from datasets.utils.case_utils import (
+from zdatasets.utils.case_utils import (
     is_upper_pascal_case,
     snake_case_to_pascal,
 )
 
 
 _logger = logging.getLogger(__name__)
 _logger.setLevel(logging.INFO)
```

### Comparing `zdatasets-0.2.5/datasets/plugins/executors/metaflow_executor.py` & `zdatasets-1.2.5/zdatasets/plugins/executors/metaflow_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 
 from dateutil import parser
 
-from datasets.context import Context
-from datasets.program_executor import ProgramExecutor
+from zdatasets.context import Context
+from zdatasets.program_executor import ProgramExecutor
 
 
 class MetaflowExecutor(ProgramExecutor):
     @property
     def current_run_id(self) -> str:
         from metaflow import current
```

### Comparing `zdatasets-0.2.5/datasets/plugins/register_plugins.py` & `zdatasets-1.2.5/zdatasets/plugins/register_plugins.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from datasets.dataset_plugin import DatasetPlugin
-from datasets.plugins import MetaflowExecutor
+from zdatasets.dataset_plugin import DatasetPlugin
+from zdatasets.plugins import MetaflowExecutor
 
 
 def register():
     from importlib_metadata import entry_points
 
     # Register plugins
-    for entry in entry_points(group="datasets.plugins"):
+    for entry in entry_points(group="zdatasets.plugins"):
         entry.load()
 
     # Register default executor first
     DatasetPlugin.register_executor(executor=MetaflowExecutor())
 
-    for entry in entry_points(group="datasets.executors"):
+    for entry in entry_points(group="zdatasets.executors"):
         executor = entry.load()
         if not isinstance(executor, type(MetaflowExecutor)):
             DatasetPlugin.register_executor(executor=executor)
 
     DatasetPlugin.register_plugin_factory(DatasetPlugin.default_plugin_factory)
     DatasetPlugin.register_dataset_name_validator(DatasetPlugin.validate_dataset_name)
```

### Comparing `zdatasets-0.2.5/datasets/program_executor.py` & `zdatasets-1.2.5/zdatasets/program_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 
-from datasets.context import Context
+from zdatasets.context import Context
 
 
 class ProgramExecutor(ABC):
     """
     Class to access information about the program currently being executed.
     """
 
@@ -32,10 +32,10 @@
         pass
 
     @property
     @abstractmethod
     def run_time(self) -> int:
         """
         UTC Epoch time when the program started, used as the run_time column in Batch & Hive
-        datasets.
+        zdatasets.
         """
         pass
```

### Comparing `zdatasets-0.2.5/datasets/tests/conftest.py` & `zdatasets-1.2.5/zdatasets/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import time
 import uuid
 from pathlib import Path
 
 import pytest
 from pyspark.sql import SparkSession
 
-from datasets import Context
-from datasets.dataset_plugin import DatasetPlugin
-from datasets.program_executor import ProgramExecutor
+from zdatasets import Context
+from zdatasets.dataset_plugin import DatasetPlugin
+from zdatasets.program_executor import ProgramExecutor
 
 
 test_dir = Path(os.path.realpath(__file__)).parent
 _run_id = str(uuid.uuid1())
 _run_time = time.time()
```

### Comparing `zdatasets-0.2.5/datasets/tests/data/train/date=2020-07-23/region=king/data.parquet` & `zdatasets-1.2.5/zdatasets/tests/data/train/date=2020-07-23/region=king/data.parquet`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.5/datasets/tests/data/train/date=2020-07-23/region=la/data.parquet` & `zdatasets-1.2.5/zdatasets/tests/data/train/date=2020-07-23/region=la/data.parquet`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.5/datasets/tests/test_batch_dataset.py` & `zdatasets-1.2.5/zdatasets/tests/test_batch_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 import dask.dataframe as dd
 import pandas as pd
 import pytest
 from pandas._testing import assert_frame_equal
 from pyspark import pandas as ps
 from pyspark.sql import DataFrame as SparkDataFrame
 
-from datasets import Dataset, Mode
-from datasets.exceptions import InvalidOperationException
-from datasets.plugins.batch.batch_base_plugin import BatchOptions
-from datasets.plugins.batch.batch_dataset import BatchDataset
-from datasets.tests.conftest import TestExecutor
+from zdatasets import Dataset, Mode
+from zdatasets.exceptions import InvalidOperationException
+from zdatasets.plugins.batch.batch_base_plugin import BatchOptions
+from zdatasets.plugins.batch.batch_dataset import BatchDataset
+from zdatasets.tests.conftest import TestExecutor
 
 
 csv_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), "data/pandas.csv")
 
 
 @pytest.fixture
 def path(data_path: str) -> str:
@@ -156,15 +156,15 @@
 
 @pytest.mark.parametrize("path", [None])
 @pytest.mark.parametrize("partition_by", ["col1,col3", ["col1", "col3"]])
 @pytest.mark.parametrize("mode", [Mode.WRITE, Mode.READ_WRITE])
 def test_get_dataset_path(dataset: BatchDataset, df: pd.DataFrame):
     dataset.write(df.copy())
     path = dataset._get_dataset_path()
-    assert path.endswith("datasets/tests/data/datastore/my_program/ds_1")
+    assert path.endswith("zdatasets/tests/data/datastore/my_program/ds_1")
     os.path.exists(f"{path}/col1=A/col3=A1")
     shutil.rmtree(path)
 
 
 @pytest.mark.parametrize("mode", [Mode.READ])
 def test_write_on_read_only_pandas(dataset: BatchDataset):
     df = pd.DataFrame({"col1": ["A", "A", "A", "B", "B", "B"], "col2": [1, 2, 3, 4, 5, 6]})
@@ -261,15 +261,15 @@
 @pytest.mark.parametrize("path", [None])
 @pytest.mark.parametrize("name", ["MyTable"])
 def test_register_dataset_path_plugin(dataset: BatchDataset, df: pd.DataFrame):
     dataset.write(df.copy())
 
     assert dataset.name == "MyTable"
     path = dataset._get_dataset_path()
-    assert path.endswith("datasets/tests/data/datastore/my_program/my_table")
+    assert path.endswith("zdatasets/tests/data/datastore/my_program/my_table")
 
     def test_dataset_path_func(passed_dataset: BatchDataset) -> str:
         return "fee_foo"
 
     BatchDataset.register_dataset_path_func(test_dataset_path_func)
 
     os.environ["ZODIAC_SERVICE"] = "test_service"
```

### Comparing `zdatasets-0.2.5/datasets/tests/test_dataset_plugin.py` & `zdatasets-1.2.5/zdatasets/tests/test_dataset_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from dataclasses import dataclass
 from typing import Optional, Union
 
 import pandas as pd
 import pytest
 
-from datasets import Context, DataFrameType, Dataset, Mode
-from datasets._typing import ColumnNames
-from datasets.dataset_plugin import DatasetPlugin, StorageOptions
-from datasets.metaflow import _DatasetTypeClass
-from datasets.plugins import HiveDataset
-from datasets.plugins.batch.hive_dataset import HiveOptions
-from datasets.tests.conftest import TestExecutor
-from datasets.utils.secret_fetcher import SecretFetcher
+from zdatasets import Context, DataFrameType, Dataset, Mode
+from zdatasets._typing import ColumnNames
+from zdatasets.dataset_plugin import DatasetPlugin, StorageOptions
+from zdatasets.metaflow import _DatasetTypeClass
+from zdatasets.plugins import HiveDataset
+from zdatasets.plugins.batch.hive_dataset import HiveOptions
+from zdatasets.tests.conftest import TestExecutor
+from zdatasets.utils.secret_fetcher import SecretFetcher
 
 
 # We'll need to inherit dict too to make this class json serializable
 class _TestPlugin(DatasetPlugin, dict):
     def __init__(
         self,
         name: str,
```

### Comparing `zdatasets-0.2.5/datasets/tests/test_datasets_decorator.py` & `zdatasets-1.2.5/zdatasets/tests/test_datasets_decorator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 
-from datasets import dataset
-from datasets.plugins import HiveDataset
+from zdatasets import dataset
+from zdatasets.plugins import HiveDataset
 
 
 def test_step_decorator():
     class Foo:
         @dataset("DsFee")
         def hi(self):
             assert self.ds_fee.name == "DsFee"
```

### Comparing `zdatasets-0.2.5/datasets/tests/test_flow_dataset.py` & `zdatasets-1.2.5/zdatasets/tests/test_flow_dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from metaflow import Flow, namespace
 
-from datasets.plugins.batch.flow_dataset import _get_run_id
-from datasets.tests.test_tutorials import run_flow
+from zdatasets.plugins.batch.flow_dataset import _get_run_id
+from zdatasets.tests.test_tutorials import run_flow
 
 
 def test_get_run_id():
     flow_name = "HelloDatasetFlow"
     namespace(None)
     run_1_output = run_flow("tutorials/0_hello_dataset_flow.py")
     run_1_id = Flow(flow_name).latest_successful_run.id
```

### Comparing `zdatasets-0.2.5/datasets/tests/test_hive_dataset.py` & `zdatasets-1.2.5/zdatasets/tests/test_hive_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 import dask.dataframe as dd
 import pandas as pd
 import pytest
 from pandas._testing import assert_frame_equal
 from pyspark import pandas as ps
 from pyspark.sql import DataFrame as SparkDataFrame, SparkSession
 
-from datasets import Dataset, Mode
-from datasets.exceptions import InvalidOperationException
-from datasets.plugins import HiveDataset
-from datasets.plugins.batch.hive_dataset import (
+from zdatasets import Dataset, Mode
+from zdatasets.exceptions import InvalidOperationException
+from zdatasets.plugins import HiveDataset
+from zdatasets.plugins.batch.hive_dataset import (
     HiveOptions,
     _retry_with_backoff,
 )
-from datasets.tests.conftest import TestExecutor
+from zdatasets.tests.conftest import TestExecutor
 
 
 @pytest.fixture
 def mode():
     return Mode.READ_WRITE
```

### Comparing `zdatasets-0.2.5/datasets/tests/test_metaflow.py` & `zdatasets-1.2.5/zdatasets/tests/test_metaflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import json
 
-from datasets import Dataset
-from datasets.context import Context
-from datasets.dataset_plugin import StorageOptions
-from datasets.metaflow import (
+from zdatasets import Dataset
+from zdatasets.context import Context
+from zdatasets.dataset_plugin import StorageOptions
+from zdatasets.metaflow import (
     _DatasetParams,
     _DatasetParamsDecoder,
     _DatasetTypeClass,
 )
-from datasets.mode import Mode
-from datasets.plugins.batch.batch_base_plugin import BatchOptions
-from datasets.plugins.batch.batch_dataset import BatchDataset
-from datasets.plugins.batch.hive_dataset import HiveOptions
-from datasets.tests.test_dataset_plugin import (
+from zdatasets.mode import Mode
+from zdatasets.plugins.batch.batch_base_plugin import BatchOptions
+from zdatasets.plugins.batch.batch_dataset import BatchDataset
+from zdatasets.plugins.batch.hive_dataset import HiveOptions
+from zdatasets.tests.test_dataset_plugin import (
     SecretDatasetPluginTest,
     SecretDatasetTestOptions,
 )
-from datasets.utils.secret_fetcher import SecretFetcher
+from zdatasets.utils.secret_fetcher import SecretFetcher
 
 
 def test_dataset_dumps_load():
     dataset = Dataset(
         name="Example",
         logical_key="my_key",
         mode=Mode.READ_WRITE,
```

### Comparing `zdatasets-0.2.5/datasets/tests/test_tutorials.py` & `zdatasets-1.2.5/zdatasets/tests/test_tutorials.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 def test_hive_flow():
     run_flow("tutorials/6_hive_dataset_flow.py")
 
 
 def run_flow(flow_py, args: Optional[list] = None, context: Optional[str] = None) -> str:
-    os.environ["METAFLOW_COVERAGE_SOURCE"] = "tutorial,datasets"
+    os.environ["METAFLOW_COVERAGE_SOURCE"] = "tutorial,zdatasets"
     os.environ["METAFLOW_COVERAGE_OMIT"] = "metaflow"
     os.environ["METAFLOW_USER"] = "compile_only_user"
     if context:
         os.environ["CONTEXT"] = context
 
     base_dir = dirname(dirname(realpath(__file__)))
     file_name = os.path.join(base_dir, flow_py)
```

### Comparing `zdatasets-0.2.5/datasets/tests/utils/test_case_utils.py` & `zdatasets-1.2.5/zdatasets/tests/utils/test_case_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datasets.utils.case_utils import (
+from zdatasets.utils.case_utils import (
     is_snake_case,
     is_upper_pascal_case,
     pascal_to_snake_case,
     snake_case_to_pascal,
 )
```

### Comparing `zdatasets-0.2.5/datasets/tests/utils/test_partitions.py` & `zdatasets-1.2.5/zdatasets/tests/utils/test_partitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from typing import List
 
 import pytest
 from moto import mock_s3, mock_sts
 
-from datasets.utils.aws import get_aws_client
-from datasets.utils.partitions import Partition, get_path_partitions
+from zdatasets.utils.aws import get_aws_client
+from zdatasets.utils.partitions import Partition, get_path_partitions
 
 
 @pytest.fixture
 def assume_role() -> str:
     return "arn:aws:iam::333333333333:role/test-role"
```

### Comparing `zdatasets-0.2.5/datasets/tests/utils/test_secret_fetcher.py` & `zdatasets-1.2.5/zdatasets/tests/utils/test_secret_fetcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import unittest
 from unittest import mock
 
 import boto3
 import pytest
 from moto import mock_secretsmanager
 
-from datasets.utils.secret_fetcher import (
+from zdatasets.utils.secret_fetcher import (
     SecretFetcher,
     get_current_namespace,
     try_import_kubernetes,
 )
 
 
 case = unittest.TestCase()
@@ -67,15 +67,15 @@
     assert SecretFetcher(env_var="EXAMPLE_SECRET").value == "example_value"
     with pytest.raises(ValueError):
         SecretFetcher(env_var="EXAMPLE_SECRET", key="key").value
 
 
 @mock_secretsmanager
 def test_fetch_aws_secret():
-    from datasets.utils.secret_fetcher import logger, secret_cache
+    from zdatasets.utils.secret_fetcher import logger, secret_cache
 
     conn = boto3.client("secretsmanager", region_name="us-west-2")
     conn.create_secret(Name="json-decodable-dict", SecretString='{"key": "value"}')
     conn.create_secret(Name="json-decodable-str", SecretString='"example_value"')
     conn.create_secret(Name="not-json-decodable", SecretString="example_value")
     conn.create_secret(Name="empty", SecretString="")
 
@@ -109,18 +109,18 @@
         SecretFetcher(aws_secret_arn="not-json-decodable", key="key").value
 
     # Empty string
     with pytest.raises(ValueError):
         SecretFetcher(aws_secret_arn="empty").value
 
 
-@mock.patch("datasets.utils.secret_fetcher.get_current_namespace")
-@mock.patch("datasets.utils.secret_fetcher.try_import_kubernetes")
+@mock.patch("zdatasets.utils.secret_fetcher.get_current_namespace")
+@mock.patch("zdatasets.utils.secret_fetcher.try_import_kubernetes")
 def test_fetch_kubernetes_secret(kubernetes, namespace):
-    from datasets.utils.secret_fetcher import logger, secret_cache
+    from zdatasets.utils.secret_fetcher import logger, secret_cache
 
     example_kubernetes_secret = {
         "key": base64.b64encode(b"value"),
     }
 
     example_new_kubernetes_secret = {
         "key": base64.b64encode(b"new_value"),
```

### Comparing `zdatasets-0.2.5/datasets/tutorials/0_hello_dataset_flow.py` & `zdatasets-1.2.5/zdatasets/tutorials/0_hello_dataset_flow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pandas as pd
 from metaflow import FlowSpec, step
 
-from datasets import Dataset, Mode
-from datasets.metaflow import DatasetParameter
-from datasets.plugins import BatchOptions
+from zdatasets import Dataset, Mode
+from zdatasets.metaflow import DatasetParameter
+from zdatasets.plugins import BatchOptions
 
 
 # Can also invoke from CLI:
-#  > python datasets/tutorials/0_hello_dataset_flow.py run \
+#  > python zdatasets/tutorials/0_hello_dataset_flow.py run \
 #    --hello_dataset '{"name": "HelloDataset", "mode": "READ_WRITE", \
 #    "options": {"type": "BatchOptions", "partition_by": "region"}}'
 class HelloDatasetFlow(FlowSpec):
     hello_dataset = DatasetParameter(
         "hello_dataset",
         default=Dataset("HelloDataset", mode=Mode.READ_WRITE, options=BatchOptions(partition_by="region")),
     )
```

### Comparing `zdatasets-0.2.5/datasets/tutorials/1_input_output_flow.py` & `zdatasets-1.2.5/zdatasets/tutorials/1_input_output_flow.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 from metaflow import Flow, FlowSpec, step
 
-from datasets import Mode, dataset
-from datasets.plugins import BatchOptions, FlowOptions
+from zdatasets import Mode, dataset
+from zdatasets.plugins import BatchOptions, FlowOptions
 
 
 class InputOutputDatasetFlow(FlowSpec):
     @dataset("HelloDataset", options=FlowOptions(flow_dataset="HelloDatasetFlow.output_dataset"))
     @dataset("OutputDataset", options=BatchOptions(partition_by="date_key,region"), mode=Mode.READ_WRITE)
     @step
     def start(self):
```

### Comparing `zdatasets-0.2.5/datasets/tutorials/2_spark_dask_flow.py` & `zdatasets-1.2.5/zdatasets/tutorials/2_spark_dask_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dask.dataframe import DataFrame
 from metaflow import FlowSpec, step
 
-from datasets import dataset
-from datasets.plugins import FlowOptions
+from zdatasets import dataset
+from zdatasets.plugins import FlowOptions
 
 
 class SparkDaskFlow(FlowSpec):
     @dataset(
         field_name="io_dataset", options=FlowOptions(flow_dataset="InputOutputDatasetFlow.output_dataset")
     )
     @step
```

### Comparing `zdatasets-0.2.5/datasets/tutorials/3_foreach_dataset_flow.py` & `zdatasets-1.2.5/zdatasets/tutorials/3_foreach_dataset_flow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 import pandas as pd  # type: ignore
 from metaflow import FlowSpec, step
 
-from datasets import Mode, dataset
-from datasets.plugins import BatchDataset, BatchOptions
+from zdatasets import Mode, dataset
+from zdatasets.plugins import BatchDataset, BatchOptions
 
 
 flow_dir = os.path.dirname(os.path.realpath(__file__))
 my_dataset_foreach_path = os.path.join(flow_dir, "data/my_dataset_foreach")
 
 
 class ForeachDatasetFlow(FlowSpec):
```

### Comparing `zdatasets-0.2.5/datasets/tutorials/4_hello_plugin_flow.py` & `zdatasets-1.2.5/zdatasets/tutorials/4_hello_plugin_flow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas as pd
 from metaflow import FlowSpec, step
 
-from datasets import dataset
-from datasets.context import Context
-from datasets.dataset_plugin import DatasetPlugin
-from datasets.plugins import MetaflowExecutor
-from datasets.tutorials.online_plugin import DefaultOnlineDatasetPlugin
+from zdatasets import dataset
+from zdatasets.context import Context
+from zdatasets.dataset_plugin import DatasetPlugin
+from zdatasets.plugins import MetaflowExecutor
+from zdatasets.tutorials.online_plugin import DefaultOnlineDatasetPlugin
 
 
 # An online executor context!
 class OnlineExecutor(MetaflowExecutor):
     @property
     def context(self) -> Context:
         return Context.ONLINE
```

### Comparing `zdatasets-0.2.5/datasets/tutorials/5_consistent_flow.py` & `zdatasets-1.2.5/zdatasets/tutorials/5_consistent_flow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 
 import pandas as pd
 from metaflow import FlowSpec, step
 
-from datasets import Dataset, Mode
-from datasets.context import Context
-from datasets.dataset_plugin import DatasetPlugin
-from datasets.metaflow import DatasetParameter
-from datasets.plugins import BatchOptions, MetaflowExecutor
-from datasets.tutorials.online_plugin import OnlineOptions
+from zdatasets import Dataset, Mode
+from zdatasets.context import Context
+from zdatasets.dataset_plugin import DatasetPlugin
+from zdatasets.metaflow import DatasetParameter
+from zdatasets.plugins import BatchOptions, MetaflowExecutor
+from zdatasets.tutorials.online_plugin import OnlineOptions
 
 
 class PortableExecutor(MetaflowExecutor):
     @property
     def context(self) -> Context:
         context_str = os.environ.get("CONTEXT", "BATCH")
         return Context[context_str]
```

### Comparing `zdatasets-0.2.5/datasets/tutorials/6_hive_dataset_flow.py` & `zdatasets-1.2.5/zdatasets/tutorials/6_hive_dataset_flow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pandas as pd
 from metaflow import FlowSpec, step
 
-from datasets import Dataset, Mode
-from datasets.metaflow import DatasetParameter
-from datasets.plugins import HiveDataset, HiveOptions
+from zdatasets import Dataset, Mode
+from zdatasets.metaflow import DatasetParameter
+from zdatasets.plugins import HiveDataset, HiveOptions
 
 
 # Can also invoke from CLI:
-#  > python datasets/tutorials/6_hive_dataset_flow.py.py run \
+#  > python zdatasets/tutorials/6_hive_dataset_flow.py.py run \
 #    --zpids_dataset '{"name": "ZpidsDataset", hive_table="zpids_dataset", \
 #    "partition_by": "region", "mode": "READ_WRITE"}'
 
 
 class HiveDatasetFlow(FlowSpec):
     zpids_dataset = DatasetParameter(
         "zpids_dataset",
```

### Comparing `zdatasets-0.2.5/datasets/tutorials/README.ipynb` & `zdatasets-1.2.5/zdatasets/tutorials/README.ipynb`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.5/datasets/tutorials/online_plugin.py` & `zdatasets-1.2.5/zdatasets/tutorials/online_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # The default online plugin!
 from dataclasses import dataclass
 from typing import List, Optional, Union
 
 import pandas as pd
 
-from datasets.context import Context
-from datasets.dataset_plugin import DatasetPlugin, StorageOptions
+from zdatasets.context import Context
+from zdatasets.dataset_plugin import DatasetPlugin, StorageOptions
 
 
 @dataclass
 class OnlineOptions(StorageOptions):
     keys: Optional[str] = None
```

### Comparing `zdatasets-0.2.5/datasets/utils/aws.py` & `zdatasets-1.2.5/zdatasets/utils/aws.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.5/datasets/utils/case_utils.py` & `zdatasets-1.2.5/zdatasets/utils/case_utils.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.5/datasets/utils/partitions.py` & `zdatasets-1.2.5/zdatasets/utils/partitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from os import listdir
 from pathlib import Path
 from typing import List, NamedTuple, Union
 
-from datasets.utils.aws import (
+from zdatasets.utils.aws import (
     get_aws_client,
     get_paginated_list_objects_iterator,
     get_s3_bucket_key,
 )
 
 
 Partition = NamedTuple("Partition", [("name", str), ("path", str)])
```

### Comparing `zdatasets-0.2.5/datasets/utils/secret_fetcher.py` & `zdatasets-1.2.5/zdatasets/utils/secret_fetcher.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.5/pyproject.toml` & `zdatasets-1.2.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "zdatasets"
-version = "0.2.5"
+version = "1.2.5"
 description = "Dataset SDK for consistent read/write [batch, online, streaming] data."
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
   "Natural Language :: English",
   "Programming Language :: Python :: 3.8",
 ]
 authors = ["Taleb Zeghmi"]
 readme = "README.md"
 
 [[tool.poetry.packages]]
-include = "datasets"
+include = "zdatasets"
 
 # https://packaging.python.org/guides/creating-and-discovering-plugins/
 [tool.poetry.plugins]
-[tool.poetry.plugins."datasets.plugins"]
-batch_dataset = "datasets.plugins:BatchDataset"
-flow_dataset = "datasets.plugins:FlowDataset"
-hive_dataset = "datasets.plugins:HiveDataset"
+[tool.poetry.plugins."zdatasets.plugins"]
+batch_dataset = "zdatasets.plugins:BatchDataset"
+flow_dataset = "zdatasets.plugins:FlowDataset"
+hive_dataset = "zdatasets.plugins:HiveDataset"
 
-[tool.poetry.plugins."datasets.executors"]
-metaflow_executor = "datasets.plugins:MetaflowExecutor"
+[tool.poetry.plugins."zdatasets.executors"]
+metaflow_executor = "zdatasets.plugins:MetaflowExecutor"
 
 [tool.poetry.dependencies]
 python = ">=3.8.0,<4"
 pandas = ">=1.1.0"
 pyarrow = ">=6.0.0"
 dask = { version = ">=2021.9.1", optional = true }
 pyspark = { version = "^3.2.0", optional = true }
@@ -53,16 +53,16 @@
 doc = ["sphinx", "sphinx_rtd_theme"]
 metaflow = ["zillow-metaflow"]
 dask = ["dask"]
 spark = ["pyspark"]
 kubernetes = ["kubernetes"]
 
 [tool.isort]
-known_first_party = 'datasets'
-known_third_party = ["datasets", "numpy", "orbital_core", "pandas"]
+known_first_party = 'zdatasets'
+known_third_party = ["zdatasets", "numpy", "orbital_core", "pandas"]
 multi_line_output = 3
 lines_after_imports = 2
 force_grid_wrap = 0
 combine_as_imports = true
 include_trailing_comma = true
 
 [tool.black]
```

### Comparing `zdatasets-0.2.5/PKG-INFO` & `zdatasets-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: zdatasets
-Version: 0.2.5
+Version: 1.2.5
 Summary: Dataset SDK for consistent read/write [batch, online, streaming] data.
 Author: Taleb Zeghmi
 Requires-Python: >=3.8.0,<4
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: dask
 Provides-Extra: doc
 Provides-Extra: kubernetes
 Provides-Extra: metaflow
 Provides-Extra: spark
 Requires-Dist: click (>=7.0,<8.1)
 Requires-Dist: dask (>=2021.9.1) ; extra == "dask"
@@ -31,30 +30,30 @@
 Description-Content-Type: text/markdown
 
 ![Tests](https://github.com/zillow/datasets/actions/workflows/test.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/zillow/datasets/badge.svg)](https://coveralls.io/github/zillow/datasets)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zillow/datasets/main?urlpath=lab/tree/datasets/tutorials)
 
 
-Welcome to @datasets
+# Welcome to zdatasets
 ==================================================
 
 TODO
 
 ```python
 import pandas as pd
 from metaflow import FlowSpec, step
 
-from datasets import Dataset, Mode
-from datasets.metaflow import DatasetParameter
-from datasets.plugins import BatchOptions
+from zdatasets import Dataset, Mode
+from zdatasets.metaflow import DatasetParameter
+from zdatasets.plugins import BatchOptions
 
 
 # Can also invoke from CLI:
-#  > python datasets/tutorials/0_hello_dataset_flow.py run \
+#  > python zdatasets/tutorials/0_hello_dataset_flow.py run \
 #    --hello_dataset '{"name": "HelloDataset", "mode": "READ_WRITE", \
 #    "options": {"type": "BatchOptions", "partition_by": "region"}}'
 class HelloDatasetFlow(FlowSpec):
     hello_dataset = DatasetParameter(
         "hello_dataset",
         default=Dataset("HelloDataset", mode=Mode.READ_WRITE, options=BatchOptions(partition_by="region")),
     )
```

