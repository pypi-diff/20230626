# Comparing `tmp/multidimio-0.3.1.tar.gz` & `tmp/multidimio-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidimio-0.3.1.tar", max compression
+gzip compressed data, was "multidimio-0.4.0.tar", max compression
```

## Comparing `multidimio-0.3.1.tar` & `multidimio-0.4.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0    10203 2023-05-02 23:32:42.112554 multidimio-0.3.1/LICENSE
--rw-r--r--   0        0        0     6043 2023-05-02 23:32:42.112554 multidimio-0.3.1/README.md
--rw-r--r--   0        0        0     2860 2023-05-02 23:32:58.152803 multidimio-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      474 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/__init__.py
--rw-r--r--   0        0        0     2697 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/__main__.py
--rw-r--r--   0        0        0      127 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/api/__init__.py
--rw-r--r--   0        0        0    24779 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/api/accessor.py
--rw-r--r--   0        0        0     2322 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/api/convenience.py
--rw-r--r--   0        0        0     4451 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/api/io_utils.py
--rw-r--r--   0        0        0      105 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/commands/__init__.py
--rw-r--r--   0        0        0    10623 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/commands/segy.py
--rw-r--r--   0        0        0      529 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/constants.py
--rw-r--r--   0        0        0      141 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/converters/__init__.py
--rw-r--r--   0        0        0      597 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/converters/exceptions.py
--rw-r--r--   0        0        0     6510 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/converters/mdio.py
--rw-r--r--   0        0        0    12386 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/converters/segy.py
--rw-r--r--   0        0        0      143 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/core/__init__.py
--rw-r--r--   0        0        0     3811 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/core/dimension.py
--rw-r--r--   0        0        0      268 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/core/exceptions.py
--rw-r--r--   0        0        0     3765 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/core/grid.py
--rw-r--r--   0        0        0     2917 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/core/indexing.py
--rw-r--r--   0        0        0     2727 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/core/serialization.py
--rw-r--r--   0        0        0      429 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/core/utils_write.py
--rw-r--r--   0        0        0     1646 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/py.typed
--rw-r--r--   0        0        0       44 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/__init__.py
--rw-r--r--   0        0        0      636 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/_standards_common.py
--rw-r--r--   0        0        0     9384 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/_standards_rev0.py
--rw-r--r--   0        0        0     7560 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/_workers.py
--rw-r--r--   0        0        0    11173 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/blocked_io.py
--rw-r--r--   0        0        0     1760 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/byte_utils.py
--rw-r--r--   0        0        0     9396 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/creation.py
--rw-r--r--   0        0        0     4856 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/ebcdic.py
--rw-r--r--   0        0        0      181 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/exceptions.py
--rw-r--r--   0        0        0     2748 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/headers.py
--rw-r--r--   0        0        0     3561 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/headers_text.py
--rw-r--r--   0        0        0     3232 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/helpers_segy.py
--rw-r--r--   0        0        0     5785 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/ibm_float.py
--rw-r--r--   0        0        0     4393 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/parsers.py
--rw-r--r--   0        0        0     6160 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/utilities.py
--rw-r--r--   0        0        0     7731 1970-01-01 00:00:00.000000 multidimio-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    10203 2023-06-26 20:41:02.942805 multidimio-0.4.0/LICENSE
+-rw-r--r--   0        0        0     6043 2023-06-26 20:41:02.946805 multidimio-0.4.0/README.md
+-rw-r--r--   0        0        0     2806 2023-06-26 20:41:14.826817 multidimio-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/__init__.py
+-rw-r--r--   0        0        0     2697 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/__main__.py
+-rw-r--r--   0        0        0      127 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/api/__init__.py
+-rw-r--r--   0        0        0    24779 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/api/accessor.py
+-rw-r--r--   0        0        0     2322 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/api/convenience.py
+-rw-r--r--   0        0        0     4451 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/api/io_utils.py
+-rw-r--r--   0        0        0      105 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/commands/__init__.py
+-rw-r--r--   0        0        0    12573 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/commands/segy.py
+-rw-r--r--   0        0        0      529 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/constants.py
+-rw-r--r--   0        0        0      141 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/converters/__init__.py
+-rw-r--r--   0        0        0      597 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/converters/exceptions.py
+-rw-r--r--   0        0        0     6510 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/converters/mdio.py
+-rw-r--r--   0        0        0    13393 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/converters/segy.py
+-rw-r--r--   0        0        0      143 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/core/__init__.py
+-rw-r--r--   0        0        0     3811 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/core/dimension.py
+-rw-r--r--   0        0        0      268 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/core/exceptions.py
+-rw-r--r--   0        0        0     3694 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/core/grid.py
+-rw-r--r--   0        0        0     2917 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/core/indexing.py
+-rw-r--r--   0        0        0     2727 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/core/serialization.py
+-rw-r--r--   0        0        0      429 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/core/utils_write.py
+-rw-r--r--   0        0        0     1646 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/py.typed
+-rw-r--r--   0        0        0       44 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/__init__.py
+-rw-r--r--   0        0        0      636 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/_standards_common.py
+-rw-r--r--   0        0        0     9384 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/_standards_rev0.py
+-rw-r--r--   0        0        0     8270 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/_workers.py
+-rw-r--r--   0        0        0    11128 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/blocked_io.py
+-rw-r--r--   0        0        0     2048 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/byte_utils.py
+-rw-r--r--   0        0        0     9408 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/creation.py
+-rw-r--r--   0        0        0     4856 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/ebcdic.py
+-rw-r--r--   0        0        0     1946 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/exceptions.py
+-rw-r--r--   0        0        0    10719 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/geometry.py
+-rw-r--r--   0        0        0     2748 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/headers.py
+-rw-r--r--   0        0        0     3561 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/headers_text.py
+-rw-r--r--   0        0        0     1120 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/helpers_segy.py
+-rw-r--r--   0        0        0     5785 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/ibm_float.py
+-rw-r--r--   0        0        0     4916 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/parsers.py
+-rw-r--r--   0        0        0     5170 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/utilities.py
+-rw-r--r--   0        0        0     7731 1970-01-01 00:00:00.000000 multidimio-0.4.0/PKG-INFO
```

### Comparing `multidimio-0.3.1/LICENSE` & `multidimio-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multidimio-0.3.1/README.md` & `multidimio-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `multidimio-0.3.1/pyproject.toml` & `multidimio-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [tool.poetry]
 name = "multidimio"
-version = "0.3.1"
+version = "0.4.0"
 description = "Cloud-native, scalable, and user-friendly multi dimensional energy data!"
 authors = ["TGS <sys-opensource@tgs.com>"]
 maintainers = [
     "Altay Sansal <altay.sansal@tgs.com>",
-    "Sri Kainkaryam <sribharath.kainkaryam@tgs.com>",
 ]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://mdio.dev"
 repository = "https://github.com/TGSAI/mdio-python"
 documentation = "https://mdio-python.readthedocs.io"
 classifiers = [
@@ -22,26 +21,26 @@
 
 [tool.poetry.urls]
 Changelog = "https://github.com/TGSAI/mdio-python/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 click = "^8.1.3"
-click-params = "^0.3.0"
+click-params = "^0.4.0"
 zarr = "^2.12.0"
 dask = ">=2022.11.0"
 tqdm = "^4.64.0"
 segyio = "^1.9.3"
 numba = ">=0.55.2,<1.0.0"
 psutil = "^5.9.1"
 distributed = {version = ">=2022.11.0", optional = true}
 bokeh = {version = "^2.4.3", optional = true}
-s3fs = {version = ">=2022.7.0", optional = true}
-gcsfs = {version = ">=2022.7.0", optional = true}
-adlfs = {version = ">=2022.7.0", optional = true}
+s3fs = {version = ">=2023.5.0", optional = true}
+gcsfs = {version = ">=2023.5.0", optional = true}
+adlfs = {version = ">=2023.4.0", optional = true}
 zfpy = {version = "^0.5.5", optional = true}
 
 [tool.poetry.extras]
 distributed = ["distributed", "bokeh"]
 cloud = ["s3fs", "gcsfs", "adlfs"]
 lossy = ["zfpy"]
```

### Comparing `multidimio-0.3.1/src/mdio/__main__.py` & `multidimio-0.4.0/src/mdio/__main__.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3.1/src/mdio/api/accessor.py` & `multidimio-0.4.0/src/mdio/api/accessor.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3.1/src/mdio/api/convenience.py` & `multidimio-0.4.0/src/mdio/api/convenience.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3.1/src/mdio/api/io_utils.py` & `multidimio-0.4.0/src/mdio/api/io_utils.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3.1/src/mdio/commands/segy.py` & `multidimio-0.4.0/src/mdio/commands/segy.py`

 * *Files 20% similar despite different names*

```diff
@@ -79,19 +79,19 @@
     "-loc",
     "--header-locations",
     required=True,
     help="Byte locations of the index attributes in SEG-Y trace header.",
     type=click_params.IntListParamType(),
 )
 @click.option(
-    "-len",
-    "--header-lengths",
+    "-types",
+    "--header-types",
     required=False,
-    help="Byte lengths of the index attributes in SEG-Y trace header.",
-    type=click_params.IntListParamType(),
+    help="Data types of the index attributes in SEG-Y trace header.",
+    type=click_params.StringListParamType(),
 )
 @click.option(
     "-names",
     "--header-names",
     required=False,
     help="Names of the index attributes",
     type=click_params.StringListParamType(),
@@ -143,26 +143,34 @@
     "--overwrite",
     required=False,
     default=False,
     help="Flag to overwrite if mdio file if it exists",
     type=click.BOOL,
     show_default=True,
 )
+@click.option(
+    "-grid-overrides",
+    "--grid-overrides",
+    required=False,
+    help="Option to add grid overrides.",
+    type=click_params.JSON,
+)
 def segy_import(
     input_segy_path,
     output_mdio_file,
     header_locations,
-    header_lengths,
+    header_types,
     header_names,
     chunk_size,
     endian,
     lossless,
     compression_tolerance,
     storage_options,
     overwrite,
+    grid_overrides,
 ):
     """Ingest SEG-Y file to MDIO.
 
     SEG-Y format is explained in the "segy" group of the command line
     interface. To see additional information run:
 
     mdio segy --help
@@ -257,27 +265,68 @@
         Let's assume streamer number is at byte 213 as
         a 2-byte integer field.
         Chunks: 8 shots x 2 cables x 256 channels x 512 samples
         --header-locations 9,213,13
         --header-names shot,cable,chan
         --header-lengths 4,2,4
         --chunk-size 8,2,256,512
+
+    We can override the dataset grid by the `grid_overrides` parameter.
+    This allows us to ingest files that don't conform to the true
+    geometry of the seismic acquisition.
+
+    For example if we are ingesting 3D seismic shots that don't have
+    a cable number and channel numbers are sequential (i.e. each cable
+    doesn't start with channel number 1; we can tell MDIO to ingest
+    this with the correct geometry by calculating cable numbers and
+    wrapped channel numbers. Note the missing byte location and word
+    length for the "cable" index.
+
+
+    Usage:
+        3D Seismic Shot Data (Byte Locations Vary):
+        Let's assume streamer number does not exist but there are
+        800 channels per cable.
+        Chunks: 8 shots x 2 cables x 256 channels x 512 samples
+        --header-locations 9,None,13
+        --header-names shot,cable,chan
+        --header-lengths 4,None,4
+        --chunk-size 8,2,256,512
+        --grid-overrides '{"ChannelWrap": True, "ChannelsPerCable": 800,
+                           "CalculateCable": True}'
+
+        \b
+        If we do have cable numbers in the headers, but channels are still
+        sequential (aka. unwrapped), we can still ingest it like this.
+        --header-locations 9,213,13
+        --header-names shot,cable,chan
+        --header-lengths 4,2,4
+        --chunk-size 8,2,256,512
+        --grid-overrides '{"ChannelWrap":True, "ChannelsPerCable": 800}'
+        \b
+        For shot gathers with channel numbers and wrapped channels, no
+        grid overrides are necessary.
+
+        In cases where the user does not know if the input has unwrapped
+        channels but desires to store with wrapped channel index use:
+        --grid-overrides '{"AutoChannelWrap": True}'
     """
     mdio.segy_to_mdio(
         segy_path=input_segy_path,
         mdio_path_or_buffer=output_mdio_file,
         index_bytes=header_locations,
-        index_lengths=header_lengths,
+        index_types=header_types,
         index_names=header_names,
         chunksize=chunk_size,
         endian=endian,
         lossless=lossless,
         compression_tolerance=compression_tolerance,
         storage_options=storage_options,
         overwrite=overwrite,
+        grid_overrides=grid_overrides,
     )
 
 
 @cli.command(name="export")
 @click.option(
     "-i",
     "--input-mdio-file",
```

### Comparing `multidimio-0.3.1/src/mdio/constants.py` & `multidimio-0.4.0/src/mdio/constants.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3.1/src/mdio/converters/exceptions.py` & `multidimio-0.4.0/src/mdio/converters/exceptions.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3.1/src/mdio/converters/mdio.py` & `multidimio-0.4.0/src/mdio/converters/mdio.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3.1/src/mdio/converters/segy.py` & `multidimio-0.4.0/src/mdio/converters/segy.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,34 +14,54 @@
 import zarr
 
 from mdio.api.io_utils import process_url
 from mdio.converters.exceptions import GridTraceCountError
 from mdio.core import Grid
 from mdio.core.utils_write import write_attribute
 from mdio.segy import blocked_io
+from mdio.segy.byte_utils import Dtype
 from mdio.segy.helpers_segy import create_zarr_hierarchy
 from mdio.segy.parsers import parse_binary_header
 from mdio.segy.parsers import parse_text_header
 from mdio.segy.utilities import get_grid_plan
 
 
 try:
     API_VERSION = metadata.version("multidimio")
 except metadata.PackageNotFoundError:
     API_VERSION = "unknown"
 
 BACKENDS = ["s3", "gcs", "gs", "az", "abfs"]
 
 
+def parse_index_types(
+    str_types: Sequence[str] | None, num_index: int
+) -> Sequence[Dtype]:
+    """Convert string type keys to Dtype enums."""
+    if str_types is None:
+        parsed_types = [Dtype.INT32] * num_index
+    else:
+        try:
+            parsed_types = [Dtype[_type.upper()] for _type in str_types]
+        except KeyError as exc:
+            msg = (
+                "Unsupported header data-type. 'index_types' must be in "
+                f"{list(Dtype.__members__.keys())}"
+            )
+            raise KeyError(msg) from exc
+
+    return parsed_types
+
+
 def segy_to_mdio(
     segy_path: str,
     mdio_path_or_buffer: str,
     index_bytes: Sequence[int],
     index_names: Sequence[str] | None = None,
-    index_lengths: Sequence[int] | None = None,
+    index_types: Sequence[str] | None = None,
     chunksize: Sequence[int] | None = None,
     endian: str = "big",
     lossless: bool = True,
     compression_tolerance: float = 0.01,
     storage_options: dict[str, Any] | None = None,
     overwrite: bool = False,
     grid_overrides: dict | None = None,
@@ -79,16 +99,17 @@
     values will compress more, but will introduce artifacts.
 
     Args:
         segy_path: Path to the input SEG-Y file
         mdio_path_or_buffer: Output path for MDIO file
         index_bytes: Tuple of the byte location for the index attributes
         index_names: Tuple of the index names for the index attributes
-        index_lengths: Tuple of the byte lengths for the index attributes
-            Default is 4-byte for each index key.
+        index_types: Tuple of the data-types for the index attributes.
+            Must be in {"int16, int32, float16, float32, ibm32"}
+            Default is 4-byte integers for each index key.
         chunksize : Override default chunk size, which is (64, 64, 64) if
             3D, and (512, 512) for 2D.
         endian: Endianness of the input SEG-Y. Rev.2 allows little endian.
             Default is 'big'. Must be in `{"big", "little"}`
         lossless: Lossless Blosc with zstandard, or ZFP with fixed precision.
         compression_tolerance: Tolerance ZFP compression, optional. The fixed
             accuracy mode in ZFP guarantees there won't be any errors larger
@@ -181,14 +202,19 @@
         ...     index_names=("shot", "cable", "channel"),
         ...     chunksize=(8, 2, 128, 1024),
         ...     grid_overrides={"ChannelWrap": True, "ChannelsPerCable": 800},
         ... )
 
         For shot gathers with channel numbers and wrapped channels, no
         grid overrides are necessary.
+
+        In cases where the user does not know if the input has unwrapped
+        channels but desires to store with wrapped channel index use:
+        >>>    grid_overrides={"AutoChannelWrap": True,
+                               "AutoChannelTraceQC":  1000000}
     """
     num_index = len(index_bytes)
 
     if chunksize is None:
         if num_index == 1:
             chunksize = (512,) * 2
 
@@ -217,20 +243,22 @@
     with segyio.open(
         filename=segy_path, mode="r", ignore_geometry=True, endian=endian
     ) as segy_handle:
         text_header = parse_text_header(segy_handle)
         binary_header = parse_binary_header(segy_handle)
         num_traces = segy_handle.tracecount
 
+    index_types = parse_index_types(index_types, num_index)
+
     dimensions, index_headers = get_grid_plan(
         segy_path=segy_path,
         segy_endian=endian,
         index_bytes=index_bytes,
         index_names=index_names,
-        index_lengths=index_lengths,
+        index_types=index_types,
         binary_header=binary_header,
         return_headers=True,
         grid_overrides=grid_overrides,
     )
 
     # Make grid and build global live trace mask
     grid = Grid(dims=dimensions)
```

### Comparing `multidimio-0.3.1/src/mdio/core/dimension.py` & `multidimio-0.4.0/src/mdio/core/dimension.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3.1/src/mdio/core/grid.py` & `multidimio-0.4.0/src/mdio/core/grid.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,17 +81,16 @@
     def build_map(self, index_headers):
         """Build a map for live traces based on `index_headers`.
 
         Args:
             index_headers: Headers to be normalized (indexed)
         """
         live_dim_indices = tuple()
-
-        # TODO: Add strict=True and remove noqa when minimum Python is 3.10
-        for dim, dim_hdr in zip(self.dims, index_headers.T):  # noqa: B905
+        for dim in self.dims[:-1]:
+            dim_hdr = index_headers[dim.name]
             live_dim_indices += (np.searchsorted(dim, dim_hdr),)
 
         # We set dead traces to uint32 max. Should be far away from actual trace counts.
         self.map = zarr.full(self.shape[:-1], dtype="uint32", fill_value=UINT32_MAX)
         self.map.vindex[live_dim_indices] = range(len(live_dim_indices[0]))
 
         self.live_mask = zarr.zeros(self.shape[:-1], dtype="bool")
```

### Comparing `multidimio-0.3.1/src/mdio/core/indexing.py` & `multidimio-0.4.0/src/mdio/core/indexing.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3.1/src/mdio/core/serialization.py` & `multidimio-0.4.0/src/mdio/core/serialization.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3.1/src/mdio/exceptions.py` & `multidimio-0.4.0/src/mdio/exceptions.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3.1/src/mdio/segy/_standards_common.py` & `multidimio-0.4.0/src/mdio/segy/_standards_common.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3.1/src/mdio/segy/_standards_rev0.py` & `multidimio-0.4.0/src/mdio/segy/_standards_rev0.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3.1/src/mdio/segy/_workers.py` & `multidimio-0.4.0/src/mdio/segy/_workers.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,57 +10,61 @@
 import segyio
 from numpy.typing import ArrayLike
 from zarr import Array
 
 from mdio.constants import UINT32_MAX
 from mdio.core import Grid
 from mdio.segy.byte_utils import ByteOrder
+from mdio.segy.byte_utils import Dtype
+from mdio.segy.ibm_float import ibm2ieee
 
 
 def header_scan_worker(
     segy_path_or_handle: str | segyio.SegyFile,
     trace_range: Sequence[int],
     byte_locs: Sequence[int],
-    byte_lengths: Sequence[int],
+    byte_types: Sequence[Dtype],
+    index_names: Sequence[str],
     segy_endian: str,
-) -> ArrayLike:
+) -> dict[str, ArrayLike]:
     """Header scan worker.
 
     Can accept file path or segyio.SegyFile.
 
     segyio.SegyFile is recommended in case it is called from another process
     that already opened the file (i.e. trace_worker).
 
     If SegyFile is not open, it can either accept a path string or a handle
     that was opened in a different context manager.
 
     Args:
         segy_path_or_handle: Path or handle to the input SEG-Y file
         byte_locs: Byte locations to return. It will be a subset of the headers.
-        byte_lengths: Tuple consisting of the byte lengths for the index
-            attributes. None sets it to 4 per index
+        byte_types: Tuple consisting of the data types for the index attributes.
         trace_range: Tuple consisting of the trace ranges to read
+        index_names: Tuple of the names for the index attributes
         segy_endian: Endianness of the input SEG-Y. Rev.2 allows little endian
 
     Returns:
-        Numpy array of parsed headers for the current block.
+        dictionary with headers:  keys are the index names, values are numpy
+            arrays of parsed headers for the current block. Array is of type
+            byte_type with the exception of IBM32 which is mapped to FLOAT32.
 
     Raises:
         TypeError: if segy_path_or_handle is incorrect / unsupported.
     """
     start, stop = trace_range
 
     if isinstance(segy_path_or_handle, str):
         with segyio.open(
             filename=segy_path_or_handle,
             mode="r",
             ignore_geometry=True,
             endian=segy_endian,
         ) as segy_handle:
-
             block_headers = [
                 segy_handle.header[trc_idx] for trc_idx in range(start, stop)
             ]
 
     elif isinstance(segy_path_or_handle, segyio.SegyFile):
         block_headers = [
             segy_path_or_handle.header[trc_idx] for trc_idx in range(start, stop)
@@ -73,43 +77,64 @@
     # Sometimes we have custom header locations that are not SEG-Y Std Rev 1.
     # In this case we can't use segyio's byte unpacking anymore.
     # First we create a struct to unpack the 240-byte trace headers.
     # The struct only knows about dimension keys, and their byte offsets.
     # Pads the rest of the data with voids.
     endian = ByteOrder[segy_endian.upper()]
 
-    # Handle byte locations and word lengths that are not specified for numpy struct
-    lengths = [4 if length is None else length for length in byte_lengths]
+    # Handle byte offsets
     offsets = [0 if byte_loc is None else byte_loc - 1 for byte_loc in byte_locs]
+    formats = [type_.numpy_dtype.newbyteorder(endian) for type_ in byte_types]
 
     struct_dtype = np.dtype(
         {
-            "names": [f"dim_{idx}" for idx in range(len(byte_locs))],
-            "formats": [endian + "i" + str(length) for length in lengths],
+            "names": index_names,
+            "formats": formats,
             "offsets": offsets,
             "itemsize": 240,
         }
     )
 
     # Then for each trace header, we take the unpacked byte buffer from segyio
     # and join them into one byte array. Then we use numpy's frombuffer() to unpack
     block_headers = b"".join([trace_headers.buf for trace_headers in block_headers])
     n_traces = stop - start
     block_headers = np.frombuffer(block_headers, struct_dtype, count=n_traces)
-    block_headers = [block_headers[dim] for dim in block_headers.dtype.names]
+    block_headers = {name: block_headers[name] for name in index_names}
+
+    out_dtype = []
+    for name, type_ in zip(index_names, byte_types):  # noqa: B905
+        if type_ == Dtype.IBM32:
+            native_dtype = Dtype.FLOAT32.numpy_dtype
+        else:
+            native_dtype = type_.numpy_dtype
+
+        out_dtype.append((name, native_dtype))
+
+    # out_array = np.empty(n_traces, out_dtype)
+    out_array = {}
+
+    # TODO: Add strict=True and remove noqa when minimum Python is 3.10
+    for name, loc, type_ in zip(index_names, byte_locs, byte_types):  # noqa: B905
+        # Handle exception when a byte_loc is None
+        if loc is None:
+            out_array[name] = 0
+            del block_headers[name]
+            continue
+
+        header = block_headers[name]
+
+        if type_ == Dtype.IBM32:
+            header = ibm2ieee(header)
 
-    block_headers = np.column_stack(block_headers)
+        out_array[name] = header
 
-    if None in byte_locs:
-        # Zero out the junk we read for `None` byte locations.
-        # We could have multiple None values.
-        none_idx = tuple(i for i, val in enumerate(byte_locs) if val is None)
-        block_headers[:, none_idx] = 0
+        del block_headers[name]
 
-    return block_headers
+    return out_array
 
 
 def trace_worker(
     segy_path: str,
     data_array: Array,
     metadata_array: Array,
     grid: Grid,
```

### Comparing `multidimio-0.3.1/src/mdio/segy/blocked_io.py` & `multidimio-0.4.0/src/mdio/segy/blocked_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,15 +293,14 @@
     The above algorithm extrapolates to higher dimensions.
 
     Args:
         samples: Sample array.
         headers: Header array.
         live_mask: Live mask array.
         out_dtype: Desired type of output samples.
-        out_dtype: Desired output data type.
         out_byteorder: Desired output data byte order.
         file_root: Root directory to write partial SEG-Y files.
         axis: Which axes to merge on. Excluding sample axis.
 
     Returns:
         Array containing final, flattened SEG-Y blocks.
     """
```

### Comparing `multidimio-0.3.1/src/mdio/segy/byte_utils.py` & `multidimio-0.4.0/src/mdio/segy/byte_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,30 +5,35 @@
 from dataclasses import dataclass
 from enum import Enum
 
 import numpy as np
 from numpy.typing import NDArray
 
 
-class Dtype(str, Enum):
+class Dtype(Enum):
     """Dtype string to Numpy format enum."""
 
-    STRING = "S"
-    UINT8 = "u1"
-    UINT16 = "u2"
-    UINT32 = "u4"
-    UINT64 = "u8"
-    INT8 = "i1"
-    INT16 = "i2"
-    INT32 = "i4"
-    INT64 = "i8"
-    FLOAT16 = "f2"
-    FLOAT32 = "f4"
-    FLOAT64 = "f8"
-    IBM32 = "u4"
+    STRING = ("STRING", "S")
+    UINT8 = ("UINT8", "u1")
+    UINT16 = ("UINT16", "u2")
+    UINT32 = ("UINT32", "u4")
+    UINT64 = ("UINT64", "u8")
+    INT8 = ("INT8", "i1")
+    INT16 = ("INT16", "i2")
+    INT32 = ("INT32", "i4")
+    INT64 = ("INT64", "i8")
+    FLOAT16 = ("FLOAT16", "f2")
+    FLOAT32 = ("FLOAT32", "f4")
+    FLOAT64 = ("FLOAT64", "f8")
+    IBM32 = ("IBM32", "u4")
+
+    @property
+    def numpy_dtype(self):
+        """Return a numpy dtype of the Enum."""
+        return np.dtype(self.value[1])
 
 
 class ByteOrder(str, Enum):
     """Endianness string to Numpy format enum."""
 
     LITTLE = "<"
     BIG = ">"
@@ -55,15 +60,15 @@
     def __len__(self) -> int:
         """Size of struct in bytes."""
         return self.dtype.itemsize
 
     @property
     def dtype(self):
         """Return Numpy dtype of the struct."""
-        return np.dtype(self.endian + self.type)
+        return np.dtype(self.endian + self.type.numpy_dtype)
 
     def byteswap(self):
         """Swap endianness in place."""
         swapped_dtype = self.dtype.newbyteorder()
         swapped_order = swapped_dtype.byteorder
         self.endian = ByteOrder(swapped_order)
```

### Comparing `multidimio-0.3.1/src/mdio/segy/creation.py` & `multidimio-0.4.0/src/mdio/segy/creation.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
     Returns:
         New structured array with pre-processing applied.
     """
     if out_dtype == Dtype.IBM32:
         samples = samples.astype("float32", copy=False)
         samples = ieee2ibm(samples)
     else:
-        samples = samples.astype(out_dtype, copy=False)
+        samples = samples.astype(out_dtype.numpy_dtype, copy=False)
 
     return samples
 
 
 # TODO: Abstract this to support various implementations by
 #  object stores and file systems. Probably fsspec solution.
 def concat_files(paths: list[str], progress=False) -> str:
```

### Comparing `multidimio-0.3.1/src/mdio/segy/ebcdic.py` & `multidimio-0.4.0/src/mdio/segy/ebcdic.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3.1/src/mdio/segy/headers.py` & `multidimio-0.4.0/src/mdio/segy/headers.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3.1/src/mdio/segy/headers_text.py` & `multidimio-0.4.0/src/mdio/segy/headers_text.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3.1/src/mdio/segy/ibm_float.py` & `multidimio-0.4.0/src/mdio/segy/ibm_float.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3.1/src/mdio/segy/parsers.py` & `multidimio-0.4.0/src/mdio/segy/parsers.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import numpy as np
 import segyio
 from psutil import cpu_count
 from tqdm.auto import tqdm
 
 from mdio.core import Dimension
 from mdio.segy._workers import header_scan_worker
+from mdio.segy.byte_utils import Dtype
 
 
 NUM_CORES = cpu_count(logical=False)
 
 
 def get_trace_count(segy_path, segy_endian):
     """Get trace count from SEG-Y file (size)."""
@@ -71,31 +72,36 @@
     return text_header
 
 
 def parse_trace_headers(
     segy_path: str,
     segy_endian: str,
     byte_locs: Sequence[int],
-    byte_lengths: Sequence[int],
+    byte_types: Sequence[Dtype],
+    index_names: Sequence[str],
     block_size: int = 50000,
     progress_bar: bool = True,
 ) -> np.ndarray:
     """Read and parse given `byte_locations` from SEG-Y file.
 
     Args:
         segy_path: Path to the input SEG-Y file.
         segy_endian: Endianness of the input SEG-Y in {'big', 'little'}.
         byte_locs: Byte locations to return. It will be a subset of headers.
-        byte_lengths: Byte lengths of each header key to index. Must be the
+        byte_types: Data types of each header key to index. Must be the
             same count as `byte_lengths`.
+        index_names: Tuple of the names for the index attributes
         block_size: Number of traces to read for each block.
         progress_bar: Enable or disable progress bar. Default is True.
 
     Returns:
-        Numpy array of parsed trace headers.
+        dictionary with headers:  keys are the index names, values are numpy
+            arrays of parsed headers for the current block. Array is of type
+            byte_type with the exception of IBM32 which is mapped to FLOAT32.
+
     """
     trace_count = get_trace_count(segy_path, segy_endian)
     n_blocks = int(ceil(trace_count / block_size))
 
     trace_ranges = []
     for idx in range(n_blocks):
         start, stop = idx * block_size, (idx + 1) * block_size
@@ -110,32 +116,37 @@
     with ProcessPoolExecutor(num_workers) as executor:
         # pool.imap is lazy
         lazy_work = executor.map(
             header_scan_worker,  # fn
             repeat(segy_path),
             trace_ranges,
             repeat(byte_locs),
-            repeat(byte_lengths),
+            repeat(byte_types),
+            repeat(index_names),
             repeat(segy_endian),
             chunksize=2,  # Not array chunks. This is for `multiprocessing`
         )
 
         if progress_bar is True:
             lazy_work = tqdm(
                 iterable=lazy_work,
                 total=n_blocks,
                 desc="Scanning SEG-Y for geometry attributes",
                 **tqdm_kw,
             )
 
         # This executes the lazy work.
         headers = list(lazy_work)
-
+    final_headers = {}
+    for header_name in index_names:
+        final_headers[header_name] = np.concatenate(
+            [header[header_name] for header in headers]
+        )
     # Merge blocks before return
-    return np.vstack(headers)
+    return final_headers
 
 
 def parse_sample_axis(binary_header: dict) -> Dimension:
     """Parse sample axis from binary header.
 
     Args:
         binary_header: Dictionary representing binary header.
```

### Comparing `multidimio-0.3.1/src/mdio/segy/utilities.py` & `multidimio-0.4.0/src/mdio/segy/utilities.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,24 +6,26 @@
 from typing import Sequence
 
 import numpy as np
 import numpy.typing as npt
 from dask.array.core import auto_chunks
 
 from mdio.core import Dimension
+from mdio.segy.byte_utils import Dtype
+from mdio.segy.geometry import GridOverrider
 from mdio.segy.parsers import parse_sample_axis
 from mdio.segy.parsers import parse_trace_headers
 
 
-def get_grid_plan(
+def get_grid_plan(  # noqa:  C901
     segy_path: str,
     segy_endian: str,
     index_bytes: Sequence[int],
     index_names: Sequence[str],
-    index_lengths: Sequence[int],
+    index_types: Sequence[Dtype],
     binary_header: dict,
     return_headers: bool = False,
     grid_overrides: dict | None = None,
 ) -> list[Dimension] | tuple[list[Dimension], npt.ArrayLike]:
     """Infer dimension ranges, and increments.
 
     Generates multiple dimensions with the following steps:
@@ -33,88 +35,62 @@
     4. Create `Dimension` for sample axis using binary header.
 
     Args:
         segy_path: Path to the input SEG-Y file
         segy_endian: Endianness of the input SEG-Y.
         index_bytes: Tuple of the byte location for the index attributes
         index_names: Tuple of the names for the index attributes
-        index_lengths: Tuple of the byte lengths for the index attributes.
-            Default will be 4-byte for all indices.
+        index_types: Tuple of the data types for the index attributes.
         binary_header: Dictionary containing binary header key, value pairs.
         return_headers: Option to return parsed headers with `Dimension` objects.
             Default is False.
         grid_overrides: Option to add grid overrides. See main documentation.
 
     Returns:
         All index dimensions or dimensions together with header values.
-
-    Raises:
-        ValueError: If appropriate grid override parameters are not provided.
     """
     if grid_overrides is None:
         grid_overrides = {}
 
     index_dim = len(index_bytes)
 
-    # Default is 4-byte for each index.
-    index_lengths = [4] * index_dim if index_lengths is None else index_lengths
+    if index_names is None:
+        index_names = [f"index_{dim}" for dim in range(index_dim)]
 
     index_headers = parse_trace_headers(
         segy_path=segy_path,
         segy_endian=segy_endian,
         byte_locs=index_bytes,
-        byte_lengths=index_lengths,
+        byte_types=index_types,
+        index_names=index_names,
     )
 
-    if index_names is None:
-        index_names = [f"index_{dim}" for dim in range(index_dim)]
-
     dims = []
 
-    if "CalculateCable" in grid_overrides:
-        cable_idx = index_names.index("cable")
-        chan_idx = index_names.index("channel")
-
-        if "ChannelsPerCable" in grid_overrides:
-            channels_per_cable = grid_overrides["ChannelsPerCable"]
-            index_headers[:, cable_idx] = (
-                index_headers[:, chan_idx] - 1
-            ) // channels_per_cable + 1
-        else:
-            raise ValueError("'ChannelsPerCable' must be specified to calculate cable.")
-
-    if "ChannelWrap" in grid_overrides:
-        chan_idx = index_names.index("channel")
-
-        if grid_overrides["ChannelWrap"] is True:
-            if "ChannelsPerCable" in grid_overrides:
-                channels_per_cable = grid_overrides["ChannelsPerCable"]
-                index_headers[:, chan_idx] = (
-                    index_headers[:, chan_idx] - 1
-                ) % channels_per_cable + 1
-        else:
-            raise ValueError("'ChannelsPerCable' must be specified to wrap channels.")
-
-    for dim, dim_name in enumerate(index_names):
-        dim_unique = np.unique(index_headers[:, dim])
-        dims.append(Dimension(coords=dim_unique, name=dim_name))
+    # Handle grid overrides.
+    override_handler = GridOverrider()
+    index_headers = override_handler.run(index_headers, grid_overrides)
+
+    for index_name in index_names:
+        dim_unique = np.unique(index_headers[index_name])
+        dims.append(Dimension(coords=dim_unique, name=index_name))
 
     sample_dim = parse_sample_axis(binary_header=binary_header)
 
     dims.append(sample_dim)
 
     return dims, index_headers if return_headers else dims
 
 
 def segy_export_rechunker(
-    chunks: tuple[int],
-    shape: tuple[int],
+    chunks: tuple[int, ...],
+    shape: tuple[int, ...],
     dtype: npt.DTypeLike,
     limit: str = "300M",
-) -> tuple[int]:
+) -> tuple[int, ...]:
     """Determine chunk sizes for writing out SEG-Y given limit.
 
     This module finds the desired chunk sizes for given chunk size
     `limit` in a depth first order.
 
     On disk chunks for MDIO are mainly optimized for visualization
     and ML applications. When we want to do export back to SEG-Y, it
```

### Comparing `multidimio-0.3.1/PKG-INFO` & `multidimio-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidimio
-Version: 0.3.1
+Version: 0.4.0
 Summary: Cloud-native, scalable, and user-friendly multi dimensional energy data!
 Home-page: https://mdio.dev
 License: Apache-2.0
 Keywords: mdio,multidimio,seismic,wind,data
 Author: TGS
 Author-email: sys-opensource@tgs.com
 Maintainer: Altay Sansal
@@ -16,24 +16,24 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cloud
 Provides-Extra: distributed
 Provides-Extra: lossy
-Requires-Dist: adlfs (>=2022.7.0) ; extra == "cloud"
+Requires-Dist: adlfs (>=2023.4.0) ; extra == "cloud"
 Requires-Dist: bokeh (>=2.4.3,<3.0.0) ; extra == "distributed"
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: click-params (>=0.3.0,<0.4.0)
+Requires-Dist: click-params (>=0.4.0,<0.5.0)
 Requires-Dist: dask (>=2022.11.0)
 Requires-Dist: distributed (>=2022.11.0) ; extra == "distributed"
-Requires-Dist: gcsfs (>=2022.7.0) ; extra == "cloud"
+Requires-Dist: gcsfs (>=2023.5.0) ; extra == "cloud"
 Requires-Dist: numba (>=0.55.2,<1.0.0)
 Requires-Dist: psutil (>=5.9.1,<6.0.0)
-Requires-Dist: s3fs (>=2022.7.0) ; extra == "cloud"
+Requires-Dist: s3fs (>=2023.5.0) ; extra == "cloud"
 Requires-Dist: segyio (>=1.9.3,<2.0.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
 Requires-Dist: zarr (>=2.12.0,<3.0.0)
 Requires-Dist: zfpy (>=0.5.5,<0.6.0) ; extra == "lossy"
 Project-URL: Changelog, https://github.com/TGSAI/mdio-python/releases
 Project-URL: Documentation, https://mdio-python.readthedocs.io
 Project-URL: Repository, https://github.com/TGSAI/mdio-python
```

