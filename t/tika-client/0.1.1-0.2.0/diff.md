# Comparing `tmp/tika_client-0.1.1.tar.gz` & `tmp/tika_client-0.2.0.tar.gz`

## Comparing `tika_client-0.1.1.tar` & `tika_client-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 tika_client-0.1.1/.editorconfig
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 tika_client-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 tika_client-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 tika_client-0.1.1/TODO.md
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 tika_client-0.1.1/.docker/docker-compose.ci-test.yml
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tika_client-0.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 tika_client-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 tika_client-0.1.1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tika_client-0.1.1/src/tika_client/__about__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 tika_client-0.1.1/src/tika_client/__init__.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tika_client-0.1.1/src/tika_client/_constants.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 tika_client-0.1.1/src/tika_client/_resource_meta.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 tika_client-0.1.1/src/tika_client/_resource_recursive.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 tika_client-0.1.1/src/tika_client/_resource_tika.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 tika_client-0.1.1/src/tika_client/_types.py
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 tika_client-0.1.1/src/tika_client/_utils.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 tika_client-0.1.1/src/tika_client/client.py
--rw-r--r--   0        0        0     4251 2020-02-02 00:00:00.000000 tika_client-0.1.1/src/tika_client/data_models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tika_client-0.1.1/src/tika_client/py.typed
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/test_image_files.py
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/test_resource_metadata.py
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/test_resource_recursive_metadata.py
--rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/test_resource_tika.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/samples/README.md
--rw-r--r--   0        0        0    14164 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/samples/microsoft-sample.docx
--rw-r--r--   0        0        0     8843 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/samples/sample-spreadsheet.ods
--rw-r--r--   0        0        0     4743 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/samples/sample-spreadsheet.xlsx
--rw-r--r--   0        0        0    23552 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/samples/sample.doc
--rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/samples/sample.docx
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/samples/sample.html
--rw-r--r--   0        0        0   189116 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/samples/sample.jpg
--rw-r--r--   0        0        0     8271 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/samples/sample.odt
--rw-r--r--   0        0        0   980209 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/samples/sample.png
--rw-r--r--   0        0        0   936200 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/samples/test-document-images.odt
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 tika_client-0.1.1/.gitignore
--rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 tika_client-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 tika_client-0.1.1/README.md
--rw-r--r--   0        0        0     3920 2020-02-02 00:00:00.000000 tika_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 tika_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 tika_client-0.2.0/.editorconfig
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 tika_client-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 tika_client-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 tika_client-0.2.0/TODO.md
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 tika_client-0.2.0/.docker/docker-compose.ci-test.yml
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tika_client-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 tika_client-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 tika_client-0.2.0/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tika_client-0.2.0/src/tika_client/__about__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tika_client-0.2.0/src/tika_client/__init__.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tika_client-0.2.0/src/tika_client/_constants.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 tika_client-0.2.0/src/tika_client/_resource_meta.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 tika_client-0.2.0/src/tika_client/_resource_recursive.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 tika_client-0.2.0/src/tika_client/_resource_tika.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 tika_client-0.2.0/src/tika_client/_types.py
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 tika_client-0.2.0/src/tika_client/_utils.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 tika_client-0.2.0/src/tika_client/client.py
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 tika_client-0.2.0/src/tika_client/data_models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tika_client-0.2.0/src/tika_client/py.typed
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 tika_client-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 tika_client-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 tika_client-0.2.0/tests/test_image_files.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 tika_client-0.2.0/tests/test_resource_metadata.py
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 tika_client-0.2.0/tests/test_resource_recursive_metadata.py
+-rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 tika_client-0.2.0/tests/test_resource_tika.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tika_client-0.2.0/tests/samples/README.md
+-rw-r--r--   0        0        0    14164 2020-02-02 00:00:00.000000 tika_client-0.2.0/tests/samples/microsoft-sample.docx
+-rw-r--r--   0        0        0     8843 2020-02-02 00:00:00.000000 tika_client-0.2.0/tests/samples/sample-spreadsheet.ods
+-rw-r--r--   0        0        0     4743 2020-02-02 00:00:00.000000 tika_client-0.2.0/tests/samples/sample-spreadsheet.xlsx
+-rw-r--r--   0        0        0    23552 2020-02-02 00:00:00.000000 tika_client-0.2.0/tests/samples/sample.doc
+-rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 tika_client-0.2.0/tests/samples/sample.docx
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 tika_client-0.2.0/tests/samples/sample.html
+-rw-r--r--   0        0        0   189116 2020-02-02 00:00:00.000000 tika_client-0.2.0/tests/samples/sample.jpg
+-rw-r--r--   0        0        0     8271 2020-02-02 00:00:00.000000 tika_client-0.2.0/tests/samples/sample.odt
+-rw-r--r--   0        0        0   980209 2020-02-02 00:00:00.000000 tika_client-0.2.0/tests/samples/sample.png
+-rw-r--r--   0        0        0   936200 2020-02-02 00:00:00.000000 tika_client-0.2.0/tests/samples/test-document-images.odt
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 tika_client-0.2.0/.gitignore
+-rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 tika_client-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 tika_client-0.2.0/README.md
+-rw-r--r--   0        0        0     3920 2020-02-02 00:00:00.000000 tika_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 tika_client-0.2.0/PKG-INFO
```

### Comparing `tika_client-0.1.1/.editorconfig` & `tika_client-0.2.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.1/.pre-commit-config.yaml` & `tika_client-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.1/CHANGELOG.md` & `tika_client-0.2.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.2.0] - 2023-06-26
+
+### Fixed
+
+- Handling of filenames in the `Content-Disposition` header with non-ASCII characters
+
+### Changed
+
+- All endpoints now return a `TikaResponse`, which will have many of the common keys parsed into Python
+  native data types where possible, based on the list [from the Tika wiki](https://cwiki.apache.org/confluence/display/TIKA/Metadata+Overview).
+  If a key is not in the response, the value will be `None`
+
 ## [0.1.1] - 2023-06-18
 
 ### Fixed
 
 - Fixes an incorrect key when parsing new content types
 - Fixed handling of message/rfc822 content type documents
```

### Comparing `tika_client-0.1.1/.github/dependabot.yml` & `tika_client-0.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.1/.github/workflows/ci.yml` & `tika_client-0.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.1/.github/workflows/codeql.yml` & `tika_client-0.2.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.1/src/tika_client/_resource_meta.py` & `tika_client-0.2.0/src/tika_client/_resource_meta.py`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.1/src/tika_client/_resource_recursive.py` & `tika_client-0.2.0/src/tika_client/_resource_recursive.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 import logging
 from pathlib import Path
 from typing import Final
 from typing import List
-from typing import Union
 
 from httpx import Client
 
 from tika_client._types import MimeType
 from tika_client._utils import BaseResource
-from tika_client.data_models import ParsedDocument
-from tika_client.data_models import ParsedImage
 from tika_client.data_models import TikaResponse
 
 logger = logging.getLogger("tika-client.rmeta")
 
 
 class _TikaRmetaBase(BaseResource):
     def _common_call(
         self,
         endpoint: str,
         filepath: Path,
         mime_type: MimeType = None,
-    ) -> List[Union[ParsedDocument, ParsedImage, TikaResponse]]:
+    ) -> List[TikaResponse]:
         """
         Given a specific endpoint and a file, do a multipart put to the endpoint
         """
-        documents: List[Union[ParsedDocument, ParsedImage, TikaResponse]] = []
+        documents: List[TikaResponse] = []
         for item in self._put_multipart(endpoint, filepath, mime_type):
             documents.append(self._decoded_response(item))
         return documents
 
 
 class _RecursiveMetaHtml(_TikaRmetaBase):
     ENDPOINT: Final[str] = "/rmeta"
```

### Comparing `tika_client-0.1.1/src/tika_client/_resource_tika.py` & `tika_client-0.2.0/src/tika_client/_resource_tika.py`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.1/src/tika_client/_utils.py` & `tika_client-0.2.0/src/tika_client/_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import logging
+import urllib.parse
 from pathlib import Path
 from typing import Dict
 
 from httpx import Client
 
 from tika_client._constants import MIN_COMPRESS_LEN
 from tika_client._types import MimeType
 from tika_client._types import RequestContent
-from tika_client.data_models import KNOWN_CONTENT_TYPES
-from tika_client.data_models import TikaKey
 from tika_client.data_models import TikaResponse
 
 logger = logging.getLogger("tika-client.utils")
 
 
 class BaseResource:
     def __init__(self, client: Client, *, compress: bool) -> None:
@@ -27,19 +26,27 @@
         Returns the JSON response of the server
         """
         with filepath.open("rb") as handle:
             if mime_type is not None:
                 files = {"upload-file": (filepath.name, handle, mime_type)}
             else:
                 files = {"upload-file": (filepath.name, handle)}  # type: ignore
-            resp = self.client.post(
-                endpoint,
-                files=files,
-                headers={"Content-Disposition": f"attachment; filename={filepath.name}"},
-            )
+            try:
+                # Filename is valid ASCII, use it
+                filepath.name.encode("ascii")
+                content_header = {"Content-Disposition": f"attachment; filename={filepath.name}"}
+            except UnicodeEncodeError:
+                # Ignore non-ascii, in case RFC 5987 is not supported, but also encode it
+                filename_safed = filepath.name.encode("ascii", "ignore").decode("ascii")
+                filepath_quoted = urllib.parse.quote(filepath.name, encoding="utf-8")
+                content_header = {
+                    "Content-Disposition": f"attachment; filename={filename_safed}; filename*=UTF-8''{filepath_quoted}",
+                }
+
+            resp = self.client.post(endpoint, files=files, headers=content_header)
             resp.raise_for_status()
             # Always JSON
             return resp.json()
 
     def _put_content(self, endpoint: str, content: RequestContent, mime_type: MimeType = None) -> Dict:
         """
         Give, an endpoint, content and optional mime type, does an HTTP PUT with the given content.
@@ -67,12 +74,8 @@
     @staticmethod
     def _decoded_response(resp_json: Dict):
         """
         If possible, returns a more detailed class with properties that appear often in this
         mime type.  Otherwise, it's a basically raw data response, but with some helpers
         for processing fields into Python types
         """
-        if resp_json[TikaKey.ContentType] in KNOWN_CONTENT_TYPES:
-            return KNOWN_CONTENT_TYPES[resp_json[TikaKey.ContentType]](resp_json)
-        else:
-            logger.warning(f"Under-specified content-type: {resp_json[TikaKey.ContentType]}")
-            return TikaResponse(resp_json)
+        return TikaResponse(resp_json)
```

### Comparing `tika_client-0.1.1/src/tika_client/client.py` & `tika_client-0.2.0/src/tika_client/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             self._client.headers.update({"Accept-Encoding": "gzip"})
 
         # Add the resources
         self.metadata = Metadata(self._client, compress=compress)
         self.tika = Tika(self._client, compress=compress)
         self.rmeta = Recursive(self._client, compress=compress)
 
-    def add_headers(self, header: Dict[str, str]):
+    def add_headers(self, header: Dict[str, str]):  # pragma: no cover
         """
         Updates the httpx Client headers with the given values
         """
         self._client.headers.update(header)
 
     def __enter__(self) -> "TikaClient":
         return self
```

### Comparing `tika_client-0.1.1/tests/conftest.py` & `tika_client-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.1/tests/test_image_files.py` & `tika_client-0.2.0/tests/test_image_files.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import magic
 
 from tests.conftest import SAMPLE_DIR
 from tika_client.client import TikaClient
-from tika_client.data_models import ParsedImage
 
 
 class TestParseImageMetadata:
     def test_image_jpeg(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.jpg"
         resp = tika_client.metadata.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
-        assert isinstance(resp, ParsedImage)
         assert resp.type == "image/jpeg"
 
     def test_image_png(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.png"
         resp = tika_client.metadata.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
-        assert isinstance(resp, ParsedImage)
         assert resp.type == "image/png"
```

### Comparing `tika_client-0.1.1/tests/test_resource_metadata.py` & `tika_client-0.2.0/tests/test_resource_metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,57 +5,51 @@
 import magic
 import pytest
 from pytest_httpx import HTTPXMock
 
 from tests.conftest import SAMPLE_DIR
 from tests.conftest import TIKA_URL
 from tika_client.client import TikaClient
-from tika_client.data_models import ParsedDocument
 
 
 class TestMetadataResource:
     def test_metadata_from_docx(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.docx"
         resp = tika_client.metadata.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
-        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert resp.created is None
 
     def test_metadata_from_docx_no_mime(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.docx"
         resp = tika_client.metadata.from_file(test_file)
 
-        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert resp.created is None
 
     def test_metadata_from_word_docx(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "microsoft-sample.docx"
         resp = tika_client.metadata.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
-        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert resp.created == datetime(year=2023, month=5, day=17, hour=16, minute=41, tzinfo=timezone.utc)
         assert resp.modified == datetime(year=2023, month=5, day=17, hour=16, minute=44, tzinfo=timezone.utc)
 
     def test_metadata_from_odt(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.odt"
         resp = tika_client.metadata.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
-        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.oasis.opendocument.text"
         assert resp.data["generator"] == "LibreOfficeDev/6.0.5.2$Linux_X86_64 LibreOffice_project/"
         assert resp.created is None
 
     def test_metadata_from_doc(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.doc"
         resp = tika_client.metadata.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
-        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/msword"
         assert resp.language == "en"
 
     def test_http_error(self, httpx_mock: HTTPXMock):
         test_file = SAMPLE_DIR / "sample.odt"
 
         httpx_mock.add_response(status_code=500)
```

### Comparing `tika_client-0.1.1/tests/test_resource_recursive_metadata.py` & `tika_client-0.2.0/tests/test_resource_recursive_metadata.py`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.1/tests/test_resource_tika.py` & `tika_client-0.2.0/tests/test_resource_tika.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,34 @@
+import shutil
+import tempfile
+from pathlib import Path
+
 import magic
 
 from tests.conftest import SAMPLE_DIR
 from tika_client.client import TikaClient
-from tika_client.data_models import ParsedDocument
 
 
 class TestParseFormatted:
     """
     Test the Tika endpoint for returning HTML formatted content
     """
 
     def test_parse_docx_from_file_as_html(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.docx"
         resp = tika_client.tika.as_html.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
-        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert "<body><p>This is an DOCX test document, also made September 14, 2022</p>\n</body>" in resp.content
         assert resp.content_length == 6424
 
     def test_parse_doc_from_file_as_html(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.doc"
         resp = tika_client.tika.as_html.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
-        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/msword"
         assert (
             "body><p>This is a test document, saved in the older .doc format for Word documents (but created in Google Drive)</p>\n</body>"  # noqa: E501
             in resp.content
         )
         assert resp.content_length == 23739
         assert resp.character_count == 90
@@ -35,86 +36,87 @@
         assert resp.revision == 1
         assert resp.last_author == "cloudconvert_4"
 
     def test_parse_docx_no_mime_from_file_as_html(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.docx"
         resp = tika_client.tika.as_html.from_file(test_file)
 
-        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert "<body><p>This is an DOCX test document, also made September 14, 2022</p>\n</body>" in resp.content
 
     def test_parse_microsoft_word_docx_from_file_as_html(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "microsoft-sample.docx"
         resp = tika_client.tika.as_html.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
-        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert (
             "<body><p>This is a sample document, generated by Microsoft Office on Wednesday, May 17, 2023.</p>\n<p>It is in English.</p>\n</body>"  # noqa: E501
             in resp.content
         )
 
     def test_parse_odt_from_file_as_html(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.odt"
         resp = tika_client.tika.as_html.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
-        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.oasis.opendocument.text"
         assert "<body><p>This is an ODT test document, created September 14, 2022</p>\n</body>" in resp.content
 
+    def test_parse_docx_from_buffer_as_html(self, tika_client: TikaClient):
+        test_file = SAMPLE_DIR / "sample.docx"
+        content = test_file.read_bytes()
+        resp = tika_client.tika.as_html.from_buffer(content, magic.from_buffer(content, mime=True))
+
+        assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
+        assert "<body><p>This is an DOCX test document, also made September 14, 2022</p>\n</body>" in resp.content
+        assert resp.content_length == 6183
+
 
 class TestParsePlain:
     def test_parse_docx_from_file_as_text(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.docx"
 
         resp = tika_client.tika.as_text.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
-        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert "This is an DOCX test document, also made September 14, 2022" in resp.content
 
     def test_parse_odt_from_file_as_text(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.odt"
 
         resp = tika_client.tika.as_text.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
-        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.oasis.opendocument.text"
         assert "This is an ODT test document, created September 14, 2022" in resp.content
 
 
 class TestParseContentPlain:
     def test_parse_docx_from_bytes_buffer(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.docx"
         buffer = test_file.read_bytes()
 
         resp = tika_client.tika.as_text.from_buffer(buffer)
 
-        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert "This is an DOCX test document, also made September 14, 2022" in resp.content
 
     def test_parse_odt_from_bytes_buffer(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.odt"
         buffer = test_file.read_bytes()
 
         resp = tika_client.tika.as_text.from_buffer(buffer)
 
-        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.oasis.opendocument.text"
         assert "This is an ODT test document, created September 14, 2022" in resp.content
 
     def test_parse_odt_from_bytes_buffer_with_mime(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.odt"
         buffer = test_file.read_bytes()
 
         resp = tika_client.tika.as_text.from_buffer(buffer, "application/vnd.oasis.opendocument.text")
 
-        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.oasis.opendocument.text"
         assert "This is an ODT test document, created September 14, 2022" in resp.content
 
     def test_html_document_from_string_buffer(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.html"
         buffer = test_file.read_text()
 
@@ -130,9 +132,24 @@
 class TestParseContentCompress:
     def test_parse_odt_from_bytes_buffer_compress(self, tika_client_compressed: TikaClient):
         test_file = SAMPLE_DIR / "test-document-images.odt"
         buffer = test_file.read_bytes()
 
         resp = tika_client_compressed.tika.as_text.from_buffer(buffer)
 
-        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.oasis.opendocument.text"
+
+
+class TestFilenameContentDisposition:
+    def test_non_ascii_filename(self, tika_client: TikaClient):
+        test_file = SAMPLE_DIR / "sample.docx"
+
+        with tempfile.TemporaryDirectory() as temp_dir:
+            copy = shutil.copy(
+                test_file,
+                Path(temp_dir) / "Kostenerstattung für Meldebescheinigung Familienzuschlag.docx",
+            )
+
+            resp = tika_client.tika.as_text.from_file(copy, magic.from_file(str(copy), mime=True))
+
+            assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
+            assert "This is an DOCX test document, also made September 14, 2022" in resp.content
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tika_client-0.1.1/tests/samples/microsoft-sample.docx` & `tika_client-0.2.0/tests/samples/microsoft-sample.docx`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.1/tests/samples/sample-spreadsheet.ods` & `tika_client-0.2.0/tests/samples/sample-spreadsheet.ods`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.1/tests/samples/sample-spreadsheet.xlsx` & `tika_client-0.2.0/tests/samples/sample-spreadsheet.xlsx`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.1/tests/samples/sample.doc` & `tika_client-0.2.0/tests/samples/sample.doc`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.1/tests/samples/sample.docx` & `tika_client-0.2.0/tests/samples/sample.docx`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.1/tests/samples/sample.jpg` & `tika_client-0.2.0/tests/samples/sample.jpg`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.1/tests/samples/sample.odt` & `tika_client-0.2.0/tests/samples/sample.odt`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.1/tests/samples/sample.png` & `tika_client-0.2.0/tests/samples/sample.png`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.1/tests/samples/test-document-images.odt` & `tika_client-0.2.0/tests/samples/test-document-images.odt`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.1/.gitignore` & `tika_client-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.1/LICENSE.txt` & `tika_client-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.1/README.md` & `tika_client-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.1/pyproject.toml` & `tika_client-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.1/PKG-INFO` & `tika_client-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tika-client
-Version: 0.1.1
+Version: 0.2.0
 Summary: A modern REST client for Apache Tika server
 Project-URL: Documentation, https://github.com/stumpylog/tika-rest-client#readme
 Project-URL: Issues, https://github.com/stumpylog/tika-rest-client/issues
 Project-URL: Source, https://github.com/stumpylog/tika-rest-client
 Author-email: Trenton H <797416+stumpylog@users.noreply.github.com>
 License-Expression: GPL-3.0-only
 License-File: LICENSE.txt
```

