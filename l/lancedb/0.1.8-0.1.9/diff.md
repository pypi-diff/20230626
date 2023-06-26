# Comparing `tmp/lancedb-0.1.8.tar.gz` & `tmp/lancedb-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lancedb-0.1.8.tar", last modified: Mon Jun 12 22:36:00 2023, max compression
+gzip compressed data, was "lancedb-0.1.9.tar", last modified: Mon Jun 26 18:29:28 2023, max compression
```

## Comparing `lancedb-0.1.8.tar` & `lancedb-0.1.9.tar`

### file list

```diff
@@ -1,31 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:36:00.097548 lancedb-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-12 22:36:00.093548 lancedb-0.1.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:36:00.093548 lancedb-0.1.8/lancedb/
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-12 22:35:55.000000 lancedb-0.1.8/lancedb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-12 22:35:55.000000 lancedb-0.1.8/lancedb/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-12 22:35:55.000000 lancedb-0.1.8/lancedb/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-06-12 22:35:55.000000 lancedb-0.1.8/lancedb/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-06-12 22:35:55.000000 lancedb-0.1.8/lancedb/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-12 22:35:55.000000 lancedb-0.1.8/lancedb/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-12 22:35:55.000000 lancedb-0.1.8/lancedb/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-12 22:35:55.000000 lancedb-0.1.8/lancedb/fts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-06-12 22:35:55.000000 lancedb-0.1.8/lancedb/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-06-12 22:35:55.000000 lancedb-0.1.8/lancedb/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-12 22:35:55.000000 lancedb-0.1.8/lancedb/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:36:00.093548 lancedb-0.1.8/lancedb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-12 22:36:00.000000 lancedb-0.1.8/lancedb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-12 22:36:00.000000 lancedb-0.1.8/lancedb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 22:36:00.000000 lancedb-0.1.8/lancedb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-12 22:36:00.000000 lancedb-0.1.8/lancedb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 22:36:00.000000 lancedb-0.1.8/lancedb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-12 22:35:55.000000 lancedb-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 22:36:00.097548 lancedb-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-12 22:35:55.000000 lancedb-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:36:00.093548 lancedb-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-12 22:35:55.000000 lancedb-0.1.8/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-12 22:35:55.000000 lancedb-0.1.8/tests/test_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-12 22:35:55.000000 lancedb-0.1.8/tests/test_fts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-12 22:35:55.000000 lancedb-0.1.8/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-12 22:35:55.000000 lancedb-0.1.8/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-12 22:35:55.000000 lancedb-0.1.8/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-12 22:35:55.000000 lancedb-0.1.8/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:29:28.052642 lancedb-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-26 18:29:28.052642 lancedb-0.1.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:29:28.048642 lancedb-0.1.9/lancedb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-26 18:29:24.000000 lancedb-0.1.9/lancedb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-26 18:29:24.000000 lancedb-0.1.9/lancedb/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-26 18:29:24.000000 lancedb-0.1.9/lancedb/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-06-26 18:29:24.000000 lancedb-0.1.9/lancedb/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-06-26 18:29:24.000000 lancedb-0.1.9/lancedb/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-26 18:29:24.000000 lancedb-0.1.9/lancedb/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-26 18:29:24.000000 lancedb-0.1.9/lancedb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-26 18:29:24.000000 lancedb-0.1.9/lancedb/fts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-06-26 18:29:24.000000 lancedb-0.1.9/lancedb/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:29:28.048642 lancedb-0.1.9/lancedb/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-26 18:29:24.000000 lancedb-0.1.9/lancedb/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-26 18:29:24.000000 lancedb-0.1.9/lancedb/remote/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-26 18:29:24.000000 lancedb-0.1.9/lancedb/remote/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-06-26 18:29:24.000000 lancedb-0.1.9/lancedb/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-26 18:29:24.000000 lancedb-0.1.9/lancedb/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:29:28.048642 lancedb-0.1.9/lancedb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-26 18:29:28.000000 lancedb-0.1.9/lancedb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-26 18:29:28.000000 lancedb-0.1.9/lancedb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 18:29:28.000000 lancedb-0.1.9/lancedb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-26 18:29:28.000000 lancedb-0.1.9/lancedb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 18:29:28.000000 lancedb-0.1.9/lancedb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-26 18:29:24.000000 lancedb-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 18:29:28.052642 lancedb-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-26 18:29:24.000000 lancedb-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:29:28.052642 lancedb-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-26 18:29:24.000000 lancedb-0.1.9/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-26 18:29:24.000000 lancedb-0.1.9/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-26 18:29:24.000000 lancedb-0.1.9/tests/test_e2e_remote_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-26 18:29:24.000000 lancedb-0.1.9/tests/test_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-26 18:29:24.000000 lancedb-0.1.9/tests/test_fts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-26 18:29:24.000000 lancedb-0.1.9/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-26 18:29:24.000000 lancedb-0.1.9/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-26 18:29:24.000000 lancedb-0.1.9/tests/test_remote_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-26 18:29:24.000000 lancedb-0.1.9/tests/test_remote_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-06-26 18:29:24.000000 lancedb-0.1.9/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-26 18:29:24.000000 lancedb-0.1.9/tests/test_util.py
```

### Comparing `lancedb-0.1.8/PKG-INFO` & `lancedb-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lancedb
-Version: 0.1.8
+Version: 0.1.9
 Summary: lancedb
 Author-email: LanceDB Devs <dev@lancedb.com>
 Project-URL: repository, https://github.com/lancedb/lancedb
 Keywords: data-format,data-science,machine-learning,arrow,data-analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lancedb-0.1.8/lancedb/__init__.py` & `lancedb-0.1.9/lancedb/__init__.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.8/lancedb/common.py` & `lancedb-0.1.9/lancedb/common.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.8/lancedb/context.py` & `lancedb-0.1.9/lancedb/context.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from __future__ import annotations
 
 import pandas as pd
-from .exceptions import MissingValueError, MissingColumnError
+
+from .exceptions import MissingColumnError, MissingValueError
 
 
 def contextualize(raw_df: pd.DataFrame) -> Contextualizer:
     """Create a Contextualizer object for the given DataFrame.
 
     Used to create context windows. Context windows are rolling subsets of text
     data.
@@ -38,64 +39,88 @@
     ... })
 
     ``window`` determines how many rows to include in each window. In our case
     this how many tokens, but depending on the input data, it could be sentences,
     paragraphs, messages, etc.
 
     >>> contextualize(data).window(3).stride(1).text_col('token').to_df()
-                  token  document_id
-    0   The quick brown            1
-    1   quick brown fox            1
-    2  brown fox jumped            1
-    3   fox jumped over            1
-    4   jumped over the            1
-    5     over the lazy            1
-    6      the lazy dog            1
-    7        lazy dog I            1
-    8        dog I love            1
-    >>> contextualize(data).window(7).stride(1).text_col('token').to_df()
+                    token  document_id
+    0     The quick brown            1
+    1     quick brown fox            1
+    2    brown fox jumped            1
+    3     fox jumped over            1
+    4     jumped over the            1
+    5       over the lazy            1
+    6        the lazy dog            1
+    7          lazy dog I            1
+    8          dog I love            1
+    9   I love sandwiches            2
+    10    love sandwiches            2
+    >>> contextualize(data).window(7).stride(1).min_window_size(7).text_col('token').to_df()
                                       token  document_id
     0   The quick brown fox jumped over the            1
     1  quick brown fox jumped over the lazy            1
     2    brown fox jumped over the lazy dog            1
     3        fox jumped over the lazy dog I            1
     4       jumped over the lazy dog I love            1
-
+    5   over the lazy dog I love sandwiches            1
 
     ``stride`` determines how many rows to skip between each window start. This can
     be used to reduce the total number of windows generated.
 
     >>> contextualize(data).window(4).stride(2).text_col('token').to_df()
-                       token  document_id
-    0    The quick brown fox            1
-    2  brown fox jumped over            1
-    4   jumped over the lazy            1
-    6         the lazy dog I            1
+                        token  document_id
+    0     The quick brown fox            1
+    2   brown fox jumped over            1
+    4    jumped over the lazy            1
+    6          the lazy dog I            1
+    8   dog I love sandwiches            1
+    10        love sandwiches            2
 
     ``groupby`` determines how to group the rows. For example, we would like to have
     context windows that don't cross document boundaries. In this case, we can
     pass ``document_id`` as the group by.
 
     >>> contextualize(data).window(4).stride(2).text_col('token').groupby('document_id').to_df()
                        token  document_id
     0    The quick brown fox            1
     2  brown fox jumped over            1
     4   jumped over the lazy            1
+    6           the lazy dog            1
+    9      I love sandwiches            2
+
+    ``min_window_size`` determines the minimum size of the  context windows that are generated
+    This can be used to trim the last few context windows which have size less than
+    ``min_window_size``. By default context windows of size 1 are skipped.
+
+    >>> contextualize(data).window(6).stride(3).text_col('token').groupby('document_id').to_df()
+                                 token  document_id
+    0  The quick brown fox jumped over            1
+    3     fox jumped over the lazy dog            1
+    6                     the lazy dog            1
+    9                I love sandwiches            2
+
+    >>> contextualize(data).window(6).stride(3).min_window_size(4).text_col('token').groupby('document_id').to_df()
+                                 token  document_id
+    0  The quick brown fox jumped over            1
+    3     fox jumped over the lazy dog            1
+
     """
     return Contextualizer(raw_df)
 
 
 class Contextualizer:
     """Create context windows from a DataFrame. See [lancedb.context.contextualize][]."""
 
     def __init__(self, raw_df):
         self._text_col = None
         self._groupby = None
         self._stride = None
         self._window = None
+        self._min_window_size = 2
         self._raw_df = raw_df
 
     def window(self, window: int) -> Contextualizer:
         """Set the window size. i.e., how many rows to include in each window.
 
         Parameters
         ----------
@@ -135,14 +160,25 @@
         ----------
         text_col: str
             The text column.
         """
         self._text_col = text_col
         return self
 
+    def min_window_size(self, min_window_size: int) -> Contextualizer:
+        """Set the (optional) min_window_size size for the context window.
+
+        Parameters
+        ----------
+        min_window_size: int
+            The min_window_size.
+        """
+        self._min_window_size = min_window_size
+        return self
+
     def to_df(self) -> pd.DataFrame:
         """Create the context windows and return a DataFrame."""
 
         if self._text_col not in self._raw_df.columns.tolist():
             raise MissingColumnError(self._text_col)
 
         if self._window is None or self._window < 1:
@@ -155,20 +191,27 @@
             raise MissingValueError(
                 "The value of stride is None or less than 1. Specify the "
                 "stride (number of rows to skip between each window)"
             )
 
         def process_group(grp):
             # For each group, create the text rolling window
+            # with values of size >= min_window_size
             text = grp[self._text_col].values
-            contexts = grp.iloc[: -self._window : self._stride, :].copy()
-            contexts[self._text_col] = [
-                " ".join(text[start_i : start_i + self._window])
-                for start_i in range(0, len(grp) - self._window, self._stride)
+            contexts = grp.iloc[:: self._stride, :].copy()
+            windows = [
+                " ".join(text[start_i : min(start_i + self._window, len(grp))])
+                for start_i in range(0, len(grp), self._stride)
+                if start_i + self._window <= len(grp)
+                or len(grp) - start_i >= self._min_window_size
             ]
+            # if last few rows dropped
+            if len(windows) < len(contexts):
+                contexts = contexts.iloc[: len(windows)]
+            contexts[self._text_col] = windows
             return contexts
 
         if self._groupby is None:
             return process_group(self._raw_df)
         # concat result from all groups
         return pd.concat(
             [process_group(grp) for _, grp in self._raw_df.groupby(self._groupby)]
```

### Comparing `lancedb-0.1.8/lancedb/db.py` & `lancedb-0.1.9/lancedb/db.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from __future__ import annotations
 
+import functools
 import os
 from pathlib import Path
-import os
 
 import pyarrow as pa
 from pyarrow import fs
 
 from .common import DATA, URI
 from .table import LanceTable
-from .util import get_uri_scheme, get_uri_location
+from .util import get_uri_location, get_uri_scheme
 
 
 class LanceDBConnection:
     """
     A connection to a LanceDB database.
 
     Parameters
@@ -39,39 +39,87 @@
     >>> import lancedb
     >>> db = lancedb.connect("./.lancedb")
     >>> db.create_table("my_table", data=[{"vector": [1.1, 1.2], "b": 2},
     ...                                   {"vector": [0.5, 1.3], "b": 4}])
     LanceTable(my_table)
     >>> db.create_table("another_table", data=[{"vector": [0.4, 0.4], "b": 6}])
     LanceTable(another_table)
-    >>> db.table_names()
+    >>> sorted(db.table_names())
     ['another_table', 'my_table']
     >>> len(db)
     2
     >>> db["my_table"]
     LanceTable(my_table)
     >>> "my_table" in db
     True
     >>> db.drop_table("my_table")
     >>> db.drop_table("another_table")
     """
 
     def __init__(self, uri: URI):
-        is_local = isinstance(uri, Path) or get_uri_scheme(uri) == "file"
+        if not isinstance(uri, Path):
+            scheme = get_uri_scheme(uri)
+        is_local = isinstance(uri, Path) or scheme == "file"
+        # managed lancedb remote uses schema like lancedb+[http|grpc|...]://
+        self._is_managed_remote = not is_local and scheme.startswith("lancedb")
+        if self._is_managed_remote:
+            if len(scheme.split("+")) != 2:
+                raise ValueError(
+                    f"Invalid LanceDB URI: {uri}, expected uri to have scheme like lancedb+<flavor>://..."
+                )
         if is_local:
             if isinstance(uri, str):
                 uri = Path(uri)
             uri = uri.expanduser().absolute()
             Path(uri).mkdir(parents=True, exist_ok=True)
         self._uri = str(uri)
 
+        self._entered = False
+
     @property
     def uri(self) -> str:
         return self._uri
 
+    @functools.cached_property
+    def is_managed_remote(self) -> bool:
+        return self._is_managed_remote
+
+    @functools.cached_property
+    def remote_flavor(self) -> str:
+        if not self.is_managed_remote:
+            raise ValueError(
+                "Not a managed remote LanceDB, there should be no server flavor"
+            )
+        return get_uri_scheme(self.uri).split("+")[1]
+
+    @functools.cached_property
+    def _client(self) -> "lancedb.remote.LanceDBClient":
+        if not self.is_managed_remote:
+            raise ValueError("Not a managed remote LanceDB, there should be no client")
+
+        # don't import unless we are really using remote
+        from lancedb.remote.client import RestfulLanceDBClient
+
+        if self.remote_flavor == "http":
+            return RestfulLanceDBClient(self._uri)
+
+        raise ValueError("Unsupported remote flavor: " + self.remote_flavor)
+
+    async def close(self):
+        if self._entered:
+            raise ValueError("Cannot re-enter the same LanceDBConnection twice")
+        self._entered = True
+        await self._client.close()
+
+    async def __aenter__(self) -> LanceDBConnection:
+        return self
+
+    async def __aexit__(self, exc_type, exc_value, traceback):
+        await self.close()
+
     def table_names(self) -> list[str]:
         """Get the names of all tables in the database.
 
         Returns
         -------
         list of str
             A list of table names.
```

### Comparing `lancedb-0.1.8/lancedb/embeddings.py` & `lancedb-0.1.9/lancedb/embeddings.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.8/lancedb/fts.py` & `lancedb-0.1.9/lancedb/fts.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.8/lancedb/query.py` & `lancedb-0.1.9/lancedb/query.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from __future__ import annotations
-from typing import Literal
+
+import asyncio
+from typing import Awaitable, Literal
 
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 
 from .common import VECTOR_COLUMN_NAME
 
@@ -164,28 +166,61 @@
     def to_df(self) -> pd.DataFrame:
         """
         Execute the query and return the results as a pandas DataFrame.
         In addition to the selected columns, LanceDB also returns a vector
         and also the "score" column which is the distance between the query
         vector and the returned vector.
         """
+
+        return self.to_arrow().to_pandas()
+
+    def to_arrow(self) -> pa.Table:
+        """
+        Execute the query and return the results as a arrow Table.
+        In addition to the selected columns, LanceDB also returns a vector
+        and also the "score" column which is the distance between the query
+        vector and the returned vector.
+        """
+        if self._table._conn.is_managed_remote:
+            try:
+                loop = asyncio.get_running_loop()
+            except RuntimeError:
+                loop = asyncio.get_event_loop()
+            result = self._table._conn._client.query(
+                self._table.name, self.to_remote_query()
+            )
+            return loop.run_until_complete(result).to_arrow()
+
         ds = self._table.to_lance()
-        tbl = ds.to_table(
+        return ds.to_table(
             columns=self._columns,
             filter=self._where,
             nearest={
                 "column": VECTOR_COLUMN_NAME,
                 "q": self._query,
                 "k": self._limit,
                 "metric": self._metric,
                 "nprobes": self._nprobes,
                 "refine_factor": self._refine_factor,
             },
         )
-        return tbl.to_pandas()
+
+    def to_remote_query(self) -> "VectorQuery":
+        # don't import unless we are connecting to remote
+        from lancedb.remote.client import VectorQuery
+
+        return VectorQuery(
+            vector=self._query.tolist(),
+            filter=self._where,
+            k=self._limit,
+            _metric=self._metric,
+            columns=self._columns,
+            nprobes=self._nprobes,
+            refine_factor=self._refine_factor,
+        )
 
 
 class LanceFtsQueryBuilder(LanceQueryBuilder):
     def to_df(self) -> pd.DataFrame:
         try:
             import tantivy
         except ImportError:
```

### Comparing `lancedb-0.1.8/lancedb/table.py` & `lancedb-0.1.9/lancedb/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,28 +10,26 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from __future__ import annotations
 
 import os
-import shutil
 from functools import cached_property
 from typing import List, Union
 
 import lance
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 from lance import LanceDataset
 from lance.vector import vec_to_table
 
 from .common import DATA, VEC, VECTOR_COLUMN_NAME
 from .query import LanceFtsQueryBuilder, LanceQueryBuilder
-from .util import get_uri_scheme
 
 
 def _sanitize_data(data, schema):
     if isinstance(data, list):
         data = pa.Table.from_pylist(data)
         data = _sanitize_schema(data, schema=schema)
     if isinstance(data, dict):
@@ -290,14 +288,42 @@
     @classmethod
     def create(cls, db, name, data, schema=None, mode="create"):
         tbl = LanceTable(db, name)
         data = _sanitize_data(data, schema)
         lance.write_dataset(data, tbl._dataset_uri, mode=mode)
         return tbl
 
+    def delete(self, where: str):
+        """Delete rows from the table.
+
+        Parameters
+        ----------
+        where: str
+            The SQL where clause to use when deleting rows.
+
+        Examples
+        --------
+        >>> import lancedb
+        >>> import pandas as pd
+        >>> data = pd.DataFrame({"x": [1, 2, 3], "vector": [[1, 2], [3, 4], [5, 6]]})
+        >>> db = lancedb.connect("./.lancedb")
+        >>> table = db.create_table("my_table", data)
+        >>> table.to_pandas()
+           x      vector
+        0  1  [1.0, 2.0]
+        1  2  [3.0, 4.0]
+        2  3  [5.0, 6.0]
+        >>> table.delete("x = 2")
+        >>> table.to_pandas()
+           x      vector
+        0  1  [1.0, 2.0]
+        1  3  [5.0, 6.0]
+        """
+        self._dataset.delete(where)
+
 
 def _sanitize_schema(data: pa.Table, schema: pa.Schema = None) -> pa.Table:
     """Ensure that the table has the expected schema.
 
     Parameters
     ----------
     data: pa.Table
```

### Comparing `lancedb-0.1.8/lancedb/util.py` & `lancedb-0.1.9/lancedb/util.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.8/lancedb.egg-info/PKG-INFO` & `lancedb-0.1.9/lancedb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lancedb
-Version: 0.1.8
+Version: 0.1.9
 Summary: lancedb
 Author-email: LanceDB Devs <dev@lancedb.com>
 Project-URL: repository, https://github.com/lancedb/lancedb
 Keywords: data-format,data-science,machine-learning,arrow,data-analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lancedb-0.1.8/pyproject.toml` & `lancedb-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "lancedb"
-version = "0.1.8"
-dependencies = ["pylance>=0.4.20", "ratelimiter", "retry", "tqdm"]
+version = "0.1.9"
+dependencies = ["pylance~=0.5.0", "ratelimiter", "retry", "tqdm", "aiohttp", "pydantic", "attr"]
 description = "lancedb"
 authors = [
     { name = "LanceDB Devs", email = "dev@lancedb.com" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.8"
@@ -33,15 +33,15 @@
 ]
 
 [project.urls]
 repository = "https://github.com/lancedb/lancedb"
 
 [project.optional-dependencies]
 tests = [
-    "pytest", "pytest-mock", "doctest"
+    "pytest", "pytest-mock", "pytest-asyncio"
 ]
 dev = [
     "ruff", "pre-commit", "black"
 ]
 docs = [
     "mkdocs", "mkdocs-jupyter", "mkdocs-material", "mkdocstrings[python]"
 ]
```

### Comparing `lancedb-0.1.8/setup.py` & `lancedb-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.8/tests/test_db.py` & `lancedb-0.1.9/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.8/tests/test_embeddings.py` & `lancedb-0.1.9/tests/test_embeddings.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 import sys
 
 import numpy as np
 import pyarrow as pa
+
 from lancedb.embeddings import with_embeddings
 
 
 def mock_embed_func(input_data):
     return [np.random.randn(128).tolist() for _ in range(len(input_data))]
```

### Comparing `lancedb-0.1.8/tests/test_fts.py` & `lancedb-0.1.9/tests/test_fts.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 import os
 import random
 
-import lancedb.fts
 import numpy as np
 import pandas as pd
 import pytest
 import tantivy
 
 import lancedb as ldb
+import lancedb.fts
 
 
 @pytest.fixture
 def table(tmp_path) -> ldb.table.LanceTable:
     db = ldb.connect(tmp_path)
     vectors = [np.random.randn(128) for _ in range(100)]
```

### Comparing `lancedb-0.1.8/tests/test_io.py` & `lancedb-0.1.9/tests/test_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import os
+
 import pytest
 
 import lancedb
 
 # You need to setup AWS credentials an a base path to run this test. Example
 #    AWS_PROFILE=default TEST_S3_BASE_URL=s3://my_bucket/dataset pytest tests/test_io.py
```

### Comparing `lancedb-0.1.8/tests/test_query.py` & `lancedb-0.1.9/tests/test_query.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,20 +13,23 @@
 
 import lance
 import numpy as np
 import pandas as pd
 import pandas.testing as tm
 import pyarrow as pa
 import pytest
+
+from lancedb.db import LanceDBConnection
 from lancedb.query import LanceQueryBuilder
 
 
 class MockTable:
     def __init__(self, tmp_path):
         self.uri = tmp_path
+        self._conn = LanceDBConnection("/tmp/lance/")
 
     def to_lance(self):
         return lance.dataset(self.uri)
 
 
 @pytest.fixture
 def table(tmp_path) -> MockTable:
```

### Comparing `lancedb-0.1.8/tests/test_table.py` & `lancedb-0.1.9/tests/test_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,26 +7,32 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+import functools
 from pathlib import Path
 
 import pandas as pd
 import pyarrow as pa
 import pytest
+
 from lancedb.table import LanceTable
 
 
 class MockDB:
     def __init__(self, uri: Path):
         self.uri = uri
 
+    @functools.cached_property
+    def is_managed_remote(self) -> bool:
+        return False
+
 
 @pytest.fixture
 def db(tmp_path) -> MockDB:
     return MockDB(tmp_path)
 
 
 def test_basic(db):
```

### Comparing `lancedb-0.1.8/tests/test_util.py` & `lancedb-0.1.9/tests/test_util.py`

 * *Files identical despite different names*

