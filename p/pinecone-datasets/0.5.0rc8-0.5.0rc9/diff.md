# Comparing `tmp/pinecone_datasets-0.5.0rc8.tar.gz` & `tmp/pinecone_datasets-0.5.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinecone_datasets-0.5.0rc8.tar", max compression
+gzip compressed data, was "pinecone_datasets-0.5.0rc9.tar", max compression
```

## Comparing `pinecone_datasets-0.5.0rc8.tar` & `pinecone_datasets-0.5.0rc9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     8945 2023-06-10 20:04:06.109588 pinecone_datasets-0.5.0rc8/README.md
--rw-r--r--   0        0        0      263 2023-06-22 11:27:52.743731 pinecone_datasets-0.5.0rc8/pinecone_datasets/__init__.py
--rw-r--r--   0        0        0     3088 2023-06-01 03:29:23.061670 pinecone_datasets-0.5.0rc8/pinecone_datasets/catalog.py
--rw-r--r--   0        0        0     1185 2023-06-12 13:33:01.718779 pinecone_datasets-0.5.0rc8/pinecone_datasets/cfg.py
--rw-r--r--   0        0        0    21160 2023-06-22 11:17:50.597209 pinecone_datasets-0.5.0rc8/pinecone_datasets/dataset.py
--rw-r--r--   0        0        0     1765 2023-06-10 19:50:50.284354 pinecone_datasets-0.5.0rc8/pinecone_datasets/ds_utils.py
--rw-r--r--   0        0        0      969 2023-06-09 17:14:09.503269 pinecone_datasets-0.5.0rc8/pinecone_datasets/fs.py
--rw-r--r--   0        0        0     1657 2023-05-31 11:31:31.876795 pinecone_datasets-0.5.0rc8/pinecone_datasets/public.py
--rw-r--r--   0        0        0      227 2023-06-10 19:50:50.277429 pinecone_datasets-0.5.0rc8/pinecone_datasets/testing.py
--rw-r--r--   0        0        0      915 2023-06-22 11:27:48.939559 pinecone_datasets-0.5.0rc8/pyproject.toml
--rw-r--r--   0        0        0     9956 1970-01-01 00:00:00.000000 pinecone_datasets-0.5.0rc8/PKG-INFO
+-rw-r--r--   0        0        0     8945 2023-06-25 09:17:35.695850 pinecone_datasets-0.5.0rc9/README.md
+-rw-r--r--   0        0        0      291 2023-06-26 17:28:59.587083 pinecone_datasets-0.5.0rc9/pinecone_datasets/__init__.py
+-rw-r--r--   0        0        0     3471 2023-06-25 18:34:09.170949 pinecone_datasets-0.5.0rc9/pinecone_datasets/catalog.py
+-rw-r--r--   0        0        0     1185 2023-06-25 09:17:35.697617 pinecone_datasets-0.5.0rc9/pinecone_datasets/cfg.py
+-rw-r--r--   0        0        0    22497 2023-06-26 13:24:10.799023 pinecone_datasets-0.5.0rc9/pinecone_datasets/dataset.py
+-rw-r--r--   0        0        0     1765 2023-06-25 09:17:35.699080 pinecone_datasets-0.5.0rc9/pinecone_datasets/ds_utils.py
+-rw-r--r--   0        0        0      969 2023-06-09 17:14:09.503269 pinecone_datasets-0.5.0rc9/pinecone_datasets/fs.py
+-rw-r--r--   0        0        0     1657 2023-05-31 11:31:31.876795 pinecone_datasets-0.5.0rc9/pinecone_datasets/public.py
+-rw-r--r--   0        0        0      227 2023-06-25 09:17:35.699474 pinecone_datasets-0.5.0rc9/pinecone_datasets/testing.py
+-rw-r--r--   0        0        0      907 2023-06-26 17:28:46.149152 pinecone_datasets-0.5.0rc9/pyproject.toml
+-rw-r--r--   0        0        0     9956 1970-01-01 00:00:00.000000 pinecone_datasets-0.5.0rc9/PKG-INFO
```

### Comparing `pinecone_datasets-0.5.0rc8/README.md` & `pinecone_datasets-0.5.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc8/pinecone_datasets/catalog.py` & `pinecone_datasets-0.5.0rc9/pinecone_datasets/catalog.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,14 +39,27 @@
     task: Optional[str]
     dense_model: DenseModelMetadata
     sparse_model: Optional[SparseModelMetdata]
     description: Optional[str]
     tags: Optional[List[str]]
     args: Optional[Dict[str, Any]]
 
+    @staticmethod
+    def empty() -> "DatasetMetadata":
+        return DatasetMetadata(
+            name="",
+            created_at=get_time_now(),
+            documents=0,
+            queries=0,
+            dense_model=DenseModelMetadata(name="", dimension=0),
+        )
+
+    def is_empty(self) -> bool:
+        return self.name == "" and self.documents == 0 and self.queries == 0
+
 
 class Catalog(BaseModel):
     datasets: List[DatasetMetadata] = []
 
     @staticmethod
     def load(**kwargs) -> "Catalog":
         public_datasets_base_path = os.environ.get(
```

### Comparing `pinecone_datasets-0.5.0rc8/pinecone_datasets/cfg.py` & `pinecone_datasets-0.5.0rc9/pinecone_datasets/cfg.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc8/pinecone_datasets/dataset.py` & `pinecone_datasets-0.5.0rc9/pinecone_datasets/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,33 +22,57 @@
 from pinecone_datasets.catalog import DatasetMetadata
 from pinecone_datasets.fs import get_cloud_fs, LocalFileSystem
 
 if version("pinecone-client").startswith("3"):
     from pinecone import Client as pc, Index
 elif version("pinecone-client").startswith("2"):
     import pinecone as pc
-    from pinecone import GRPCIndex as Index
+
+    try:
+        from pinecone import GRPCIndex as Index
+    except ImportError:
+        from pinecone import Index
 else:
     warnings.warn(
         message="Pinecone client version not supported or non-existent,"
         + "please use pip ineall pinecone-client to install v2 or "
         + "pip install pinecone-datasets[clientv3] to install v3"
     )
 
 
+class DatasetInitializationError(Exception):
+    long_message = """
+    This dataset was not initialized from path, but from memory, e.g. Dataset.from_pandas(...)
+    Therefore this dataset cannot be reloaded from path, or use methods that require a path.
+    If you want to reload a dataset from path, please use the `from_path` method and pass a valid path.
+    """
+
+    def __init__(self, message=long_message):
+        self.message = message
+        super().__init__(self.message)
+
+
+# TODO: import from Client
 @dataclass
 class UpsertResponse:
     upserted_count: int
 
 
 def iter_pandas_dataframe_slices(
-    df: pd.DataFrame, batch_size=1
+    df: pd.DataFrame, batch_size, return_indexes
 ) -> Generator[List[Dict[str, Any]], None, None]:
     for i in range(0, len(df), batch_size):
-        yield df.iloc[i : i + batch_size].to_dict(orient="records")
+        if return_indexes:
+            yield (
+                i,
+                df.iloc[i : i + batch_size].to_dict(orient="records"),
+                df.iloc[i : i + batch_size].index,
+            )
+        else:
+            yield df.iloc[i : i + batch_size].to_dict(orient="records")
 
 
 def iter_pandas_dataframe_single(
     df: pd.DataFrame,
 ) -> Generator[Dict[str, Any], None, None]:
     for i in range(0, len(df), 1):
         yield df.iloc[i : i + 1].to_dict(orient="records")[0]
@@ -112,15 +136,15 @@
 
         Keyword Args:
             kwargs (Dict): additional arguments to pass to the fsspec constructor
 
         Returns:
             Dataset: a Dataset object
         """
-        clazz = Dataset(dataset_path=os.getcwd(), **kwargs)
+        clazz = cls(dataset_path=None, **kwargs)
         clazz._documents = cls._read_pandas_dataframe(
             documents, documents_column_mapping, cfg.Schema.Names.documents
         )
         clazz._queries = cls._read_pandas_dataframe(
             queries, queries_column_mapping, cfg.Schema.Names.queries
         )
         clazz._metadata = metadata
@@ -181,31 +205,43 @@
             # or
             dataset.documents # returns a pandas/polars DataFrame
             dataset.queries # returns a pandas/polars DataFrame
             ```
 
         """
         self._config = cfg
-        endpoint = urlparse(dataset_path)._replace(path="").geturl()
-        self._fs = get_cloud_fs(endpoint, **kwargs)
-        self._dataset_path = dataset_path
+        if dataset_path is not None:
+            endpoint = urlparse(dataset_path)._replace(path="").geturl()
+            self._fs = get_cloud_fs(endpoint, **kwargs)
+            self._dataset_path = dataset_path
+            if not self._fs.exists(self._dataset_path):
+                raise FileNotFoundError(
+                    "Dataset does not exist. Please check the path or dataset_id"
+                )
+        else:
+            self._fs = None
+            self._dataset_path = None
+        self._documents = pd.DataFrame(
+            columns=getattr(self._config.Schema.Names, "documents")
+        )
+        self._queries = pd.DataFrame(
+            columns=getattr(self._config.Schema.Names, "queries")
+        )
+        self._metadata = DatasetMetadata.empty()
         self._pinecone_client = None
-        self._documents = None
-        self._queries = None
-        self._metadata = None
-
-        if not self._fs.exists(self._dataset_path):
-            raise FileNotFoundError(
-                "Dataset does not exist. Please check the path or dataset_id"
-            )
 
     def _is_datatype_exists(self, data_type: str) -> bool:
+        if not self._fs:
+            raise DatasetInitializationError()
         return self._fs.exists(os.path.join(self._dataset_path, data_type))
 
     def _safe_read_from_path(self, data_type: str) -> pd.DataFrame:
+        if not self._fs:
+            raise DatasetInitializationError()
+
         read_path_str = os.path.join(self._dataset_path, data_type, "*.parquet")
         read_path = self._fs.glob(read_path_str)
         if self._is_datatype_exists(data_type):
             dataset = pq.ParquetDataset(read_path, filesystem=self._fs)
             dataset_schema_names = dataset.schema.names
             columns_to_null = []
             columns_not_null = []
@@ -237,45 +273,46 @@
                 ),
                 UserWarning,
                 stacklevel=0,
             )
             return pd.DataFrame(columns=getattr(self._config.Schema.Names, data_type))
 
     def _load_metadata(self) -> DatasetMetadata:
+        if not self._fs:
+            raise DatasetInitializationError()
+
         with self._fs.open(
             os.path.join(self._dataset_path, "metadata.json"), "rb"
         ) as f:
             metadata = json.load(f)
         try:
             out = DatasetMetadata(**metadata)
             return out
         # TODO: add more specific error handling, explain what is wrong
         except ValidationError as e:
             raise e
 
-    def _save_metadata(self, metadata: DatasetMetadata) -> None:  # pragma: no cover
-        with self._fs.open(os.path.join(self._dataset_path, "metadata.json"), "w") as f:
-            json.dump(metadata.dict(), f)
-
     def __getitem__(self, key: str):
         if key in ["documents", "queries"]:
             return getattr(self, key)
         else:
             raise KeyError("Dataset does not have key: {}".format(key))
 
     def __len__(self) -> int:
         return self.documents.shape[0]
 
     @property
     def documents(self) -> pd.DataFrame:
-        if self._documents is None:
+        if self._documents.empty:
             self._documents = self._safe_read_from_path("documents")
         return self._documents
 
-    def iter_documents(self, batch_size: int = 1) -> Iterator[List[Dict[str, Any]]]:
+    def iter_documents(
+        self, batch_size: int = 1, return_indexes=False
+    ) -> Iterator[List[Dict[str, Any]]]:
         """
         Iterates over the documents in the dataset.
 
         Args:
             batch_size (int, optional): The batch size to use for the iterator. Defaults to 1.
 
         Returns:
@@ -283,25 +320,26 @@
 
         Examples:
             for batch in dataset.iter_documents(batch_size=100):
                 index.upsert(batch)
         """
         if isinstance(batch_size, int) and batch_size > 0:
             return iter_pandas_dataframe_slices(
-                self.documents[self._config.Schema.documents_select_columns].dropna(
+                df=self.documents[self._config.Schema.documents_select_columns].dropna(
                     axis=1, how="all"
                 ),
-                batch_size,
+                batch_size=batch_size,
+                return_indexes=return_indexes,
             )
         else:
             raise ValueError("batch_size must be greater than 0")
 
     @property
     def queries(self) -> pd.DataFrame:
-        if self._queries is None:
+        if self._queries.empty:
             self._queries = self._safe_read_from_path("queries")
         return self._queries
 
     def iter_queries(self) -> Iterator[Dict[str, Any]]:
         """
         Iterates over the queries in the dataset.
 
@@ -315,15 +353,15 @@
         """
         return iter_pandas_dataframe_single(
             self.queries[self._config.Schema.queries_select_columns]
         )
 
     @property
     def metadata(self) -> DatasetMetadata:
-        if not self._metadata:
+        if self._metadata.is_empty():
             self._metadata = self._load_metadata()
         return self._metadata
 
     def head(self, n: int = 5) -> pd.DataFrame:
         return self.documents.head(n)
 
     def to_path(self, dataset_path: str, **kwargs):
@@ -358,15 +396,14 @@
         with fs.open(os.path.join(dataset_path, "metadata.json"), "w") as f:
             json.dump(self.metadata.dict(), f)
 
     def to_catalog(
         self,
         dataset_id: str,
         catalog_base_path: str = "",
-        import_metadata_from_blob_mapping: dict = {},
         **kwargs,
     ):
         """
         Saves the dataset to the public catalog.
         """
 
         # TODO: duplicated code
@@ -376,51 +413,55 @@
             if catalog_base_path
             else os.environ.get("DATASETS_CATALOG_BASEPATH", cfg.Storage.endpoint)
         )
         dataset_path = os.path.join(catalog_base_path, f"{dataset_id}")
         self.to_path(dataset_path, **kwargs)
 
     async def _async_upsert(self, index_name: str, batch_size: int, concurrency: int):
-        index = (
+        pinecone_index = (
             self._pinecone_client.get_index(index_name=index_name)
             if version("pinecone-client").startswith("3")
             else Index(index_name=index_name)
         )
 
         sem = asyncio.Semaphore(concurrency)
 
         pinecone_failed_batches: Dict[Int, Any] = {}
 
-        async def send_batch(batch, i):
+        async def send_batch(i, df, idx):
             async with sem:
                 try:
-                    return await index.upsert(vectors=batch, async_req=True)
+                    batch = df.loc[idx]
+                    return await pinecone_index.upsert(vectors=batch, async_req=True)
                 except Exception as pe:
                     if i in pinecone_failed_batches:
                         raise pe
                     else:
-                        pinecone_failed_batches[i] = batch
+                        pinecone_failed_batches[i] = idx
                         print(f"failed batches: {pinecone_failed_batches.keys()}")
                         return UpsertResponse(upserted_count=0)
 
         tasks = [
-            send_batch(chunk, i)
-            for i, chunk in enumerate(self.iter_documents(batch_size=batch_size))
+            send_batch(i, self.documents, idx)
+            for i, chunk, idx in self.iter_documents(
+                batch_size=batch_size, return_indexes=True
+            )
         ]
         failed_tasks_pinecone = []
 
         pbar = tqdm(total=len(self.documents), desc="Upserting Vectors")
         total_upserted_count = 0
         for task in asyncio.as_completed(tasks):
             res = await task
             total_upserted_count += res.upserted_count
             pbar.update(res.upserted_count)
 
         failed_tasks = [
-            send_batch(chunk, i) for i, chunk in pinecone_failed_batches.items()
+            send_batch(i, self.documents, index)
+            for i, index in pinecone_failed_batches.items()
         ]
 
         for task in asyncio.as_completed(failed_tasks):
             res = await task
             total_upserted_count += res.upserted_count
             pbar.update(res.upserted_count)
```

### Comparing `pinecone_datasets-0.5.0rc8/pinecone_datasets/ds_utils.py` & `pinecone_datasets-0.5.0rc9/pinecone_datasets/ds_utils.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc8/pinecone_datasets/fs.py` & `pinecone_datasets-0.5.0rc9/pinecone_datasets/fs.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc8/pinecone_datasets/public.py` & `pinecone_datasets-0.5.0rc9/pinecone_datasets/public.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc8/pyproject.toml` & `pinecone_datasets-0.5.0rc9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pinecone-datasets"
-version = "0.5.0-rc.8"
+version = "0.5.0-rc.9"
 description = "Pinecone Datasets lets you easily load datasets into your Pinecone index."
 authors = ["Pinecone"]
 maintainers = [
     "Roy Miara <miararoy@gmail.com>",
 ]
 readme = "README.md"
 
@@ -13,15 +13,15 @@
 python = "^3.8"
 polars = "^0.16.4"
 pyarrow = "^12.0.0"
 fsspec = "^2023.1.0"
 gcsfs = "^2023.1.0"
 s3fs = "^2023.1.0"
 pydantic = "^1.10.5"
-protobuf = ">=3.19.3,<3.20.0"
+protobuf = "~=3.20.0"
 pandas = "^2.0.0"
 tqdm = "^4.65.0"
 pinecone-client = { version = "3.0.0rc2", optional = true }
 
 [tool.poetry.extras]
 clientv3 = ["pinecone-client"]
```

### Comparing `pinecone_datasets-0.5.0rc8/PKG-INFO` & `pinecone_datasets-0.5.0rc9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinecone-datasets
-Version: 0.5.0rc8
+Version: 0.5.0rc9
 Summary: Pinecone Datasets lets you easily load datasets into your Pinecone index.
 Author: Pinecone
 Maintainer: Roy Miara
 Maintainer-email: miararoy@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: clientv3
 Requires-Dist: fsspec (>=2023.1.0,<2024.0.0)
 Requires-Dist: gcsfs (>=2023.1.0,<2024.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: pinecone-client (==3.0.0rc2) ; extra == "clientv3"
 Requires-Dist: polars (>=0.16.4,<0.17.0)
-Requires-Dist: protobuf (>=3.19.3,<3.20.0)
+Requires-Dist: protobuf (>=3.20.0,<3.21.0)
 Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: s3fs (>=2023.1.0,<2024.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Pinecone Datasets
```

