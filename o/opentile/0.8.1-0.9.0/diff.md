# Comparing `tmp/opentile-0.8.1.tar.gz` & `tmp/opentile-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentile-0.8.1.tar", max compression
+gzip compressed data, was "opentile-0.9.0.tar", max compression
```

## Comparing `opentile-0.8.1.tar` & `opentile-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,33 @@
--rw-r--r--   0        0        0      684 2023-03-31 13:15:21.077314 opentile-0.8.1/opentile/__init__.py
--rw-r--r--   0        0        0    19945 2023-03-31 13:15:21.078984 opentile-0.8.1/opentile/common.py
--rw-r--r--   0        0        0    13800 2023-03-31 13:15:21.080501 opentile-0.8.1/opentile/geometry.py
--rw-r--r--   0        0        0     4676 2023-03-31 13:15:21.081501 opentile-0.8.1/opentile/histech_tiff_tiler.py
--rw-r--r--   0        0        0     3095 2023-03-31 13:15:21.083503 opentile-0.8.1/opentile/interface.py
--rw-r--r--   0        0        0    14482 2023-03-31 13:15:21.084502 opentile-0.8.1/opentile/jpeg.py
--rw-r--r--   0        0        0     2449 2023-03-31 13:15:21.085500 opentile-0.8.1/opentile/metadata.py
--rw-r--r--   0        0        0    38272 2023-03-31 13:15:21.087501 opentile-0.8.1/opentile/ndpi_tiler.py
--rw-r--r--   0        0        0    11535 2023-03-31 13:15:21.088500 opentile-0.8.1/opentile/philips_tiff_tiler.py
--rw-r--r--   0        0        0    18218 2023-03-31 13:15:21.089500 opentile-0.8.1/opentile/svs_tiler.py
--rw-r--r--   0        0        0    14017 2023-03-31 13:15:21.090499 opentile-0.8.1/opentile/turbojpeg_patch.py
--rw-r--r--   0        0        0      977 2023-03-31 13:15:21.093500 opentile-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     6015 2023-03-31 13:15:21.076313 opentile-0.8.1/README.md
--rw-r--r--   0        0        0     7009 1970-01-01 00:00:00.000000 opentile-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      728 2023-04-03 07:45:37.395693 opentile-0.9.0/opentile/__init__.py
+-rw-r--r--   0        0        0     1179 2023-04-03 07:45:37.407124 opentile-0.9.0/opentile/config.py
+-rw-r--r--   0        0        0      928 2023-04-03 07:45:37.415960 opentile-0.9.0/opentile/formats/__init__.py
+-rw-r--r--   0        0        0      773 2023-04-03 07:45:37.425689 opentile-0.9.0/opentile/formats/histech/__init__.py
+-rw-r--r--   0        0        0     2778 2023-04-03 07:45:37.434692 opentile-0.9.0/opentile/formats/histech/histech_tiff_image.py
+-rw-r--r--   0        0        0     2698 2023-04-03 07:45:37.443003 opentile-0.9.0/opentile/formats/histech/histech_tiff_tiler.py
+-rw-r--r--   0        0        0      745 2023-04-03 07:45:37.450564 opentile-0.9.0/opentile/formats/ndpi/__init__.py
+-rw-r--r--   0        0        0    21186 2023-04-03 07:45:37.459307 opentile-0.9.0/opentile/formats/ndpi/ndpi_image.py
+-rw-r--r--   0        0        0     3140 2023-04-03 07:45:37.467758 opentile-0.9.0/opentile/formats/ndpi/ndpi_metadata.py
+-rw-r--r--   0        0        0     5275 2023-04-03 07:45:37.476951 opentile-0.9.0/opentile/formats/ndpi/ndpi_tile.py
+-rw-r--r--   0        0        0     7698 2023-04-03 07:45:37.487773 opentile-0.9.0/opentile/formats/ndpi/ndpi_tiler.py
+-rw-r--r--   0        0        0      755 2023-04-03 07:45:37.496692 opentile-0.9.0/opentile/formats/ome/__init__.py
+-rw-r--r--   0        0        0     4552 2023-04-03 07:45:37.505977 opentile-0.9.0/opentile/formats/ome/ome_tiff_image.py
+-rw-r--r--   0        0        0     4882 2023-04-03 07:45:37.517656 opentile-0.9.0/opentile/formats/ome/ome_tiff_tiler.py
+-rw-r--r--   0        0        0      771 2023-04-03 07:45:37.526391 opentile-0.9.0/opentile/formats/philips/__init__.py
+-rw-r--r--   0        0        0     4515 2023-04-03 07:45:37.535654 opentile-0.9.0/opentile/formats/philips/philips_tiff_image.py
+-rw-r--r--   0        0        0     4867 2023-04-03 07:45:37.544830 opentile-0.9.0/opentile/formats/philips/philips_tiff_metadata.py
+-rw-r--r--   0        0        0     4186 2023-04-03 07:45:37.553834 opentile-0.9.0/opentile/formats/philips/philips_tiff_tiler.py
+-rw-r--r--   0        0        0      741 2023-04-03 07:45:37.562244 opentile-0.9.0/opentile/formats/svs/__init__.py
+-rw-r--r--   0        0        0    14116 2023-04-03 07:45:37.571653 opentile-0.9.0/opentile/formats/svs/svs_image.py
+-rw-r--r--   0        0        0     1866 2023-04-03 07:45:37.579657 opentile-0.9.0/opentile/formats/svs/svs_metadata.py
+-rw-r--r--   0        0        0     3770 2023-04-03 07:45:37.590656 opentile-0.9.0/opentile/formats/svs/svs_tiler.py
+-rw-r--r--   0        0        0    13832 2023-04-03 07:45:37.598655 opentile-0.9.0/opentile/geometry.py
+-rw-r--r--   0        0        0      712 2023-04-03 07:45:37.607365 opentile-0.9.0/opentile/jpeg/__init__.py
+-rw-r--r--   0        0        0    14563 2023-04-03 07:45:37.616255 opentile-0.9.0/opentile/jpeg/jpeg.py
+-rw-r--r--   0        0        0    11861 2023-04-03 07:45:37.624431 opentile-0.9.0/opentile/jpeg/turbojpeg_patch.py
+-rw-r--r--   0        0        0     2484 2023-04-03 07:45:37.632677 opentile-0.9.0/opentile/metadata.py
+-rw-r--r--   0        0        0     3267 2023-04-03 07:45:37.640407 opentile-0.9.0/opentile/opentile.py
+-rw-r--r--   0        0        0    15395 2023-04-03 07:45:37.649149 opentile-0.9.0/opentile/tiff_image.py
+-rw-r--r--   0        0        0     7590 2023-04-03 07:45:37.657544 opentile-0.9.0/opentile/tiler.py
+-rw-r--r--   0        0        0     1022 2023-04-03 07:45:37.669851 opentile-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6451 2023-04-03 07:45:37.394692 opentile-0.9.0/README.md
+-rw-r--r--   0        0        0     7525 1970-01-01 00:00:00.000000 opentile-0.9.0/PKG-INFO
```

### Comparing `opentile-0.8.1/opentile/__init__.py` & `opentile-0.9.0/opentile/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-#    Copyright 2021 SECTRA AB
+#    Copyright 2021-2023 SECTRA AB
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
-from opentile.interface import OpenTile
+from opentile.opentile import OpenTile
+from opentile.metadata import Metadata
 
-__version__ = "0.8.1"
+__version__ = "0.9.0"
```

### Comparing `opentile-0.8.1/opentile/common.py` & `opentile-0.9.0/opentile/tiff_image.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-#    Copyright 2021 SECTRA AB
+#    Copyright 2021-2023 SECTRA AB
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
+"""Base image classes."""
+
 import math
 import threading
-from abc import ABCMeta, abstractclassmethod, abstractmethod
+from abc import ABCMeta, abstractmethod
 from pathlib import Path
-from typing import List, Optional, Sequence, Tuple
+from typing import Iterator, List, Optional, Sequence, Tuple
 
 import numpy as np
 from tifffile.tifffile import (
     COMPRESSION,
     PHOTOMETRIC,
     FileHandle,
-    TiffFile,
     TiffPage,
-    TiffPageSeries,
     TiffTags,
 )
 
 from opentile.geometry import Point, Region, Size, SizeMm
 from opentile.jpeg import Jpeg
-from opentile.metadata import Metadata
 
 
 class LockableFileHandle:
     """A lockable file handle for reading frames."""
 
     def __init__(self, fh: FileHandle):
         self._fh = fh
@@ -110,75 +109,86 @@
         return self._fh.read(bytecount)
 
     def close(self) -> None:
         """Close the file handle"""
         self._fh.close()
 
 
-class OpenTilePage(metaclass=ABCMeta):
+class TiffImage(metaclass=ABCMeta):
     """Abstract class for reading tiles from TiffPage. Should be inherited to
-    support different tiff formats:
-
-    OpenTilePage
-        NativeTiledPage - Meta class for pages that are natively tiled
-            PhilipsTiffTiledPage - OpenTiledPage for Philips Tiff-page
-            SvsTiledPage - OpenTiledPage for Svs Tiff-page
-        NdpiPage - Ndpi page that should not be tiled
-            NdpiTiledPage - Metaclass for a tiled Ndpi page
-                NdpiOneFramePage - Tiled Ndpi page of only one frame
-                NdpiStripedPage - Tiled Ndpi page of striped frames
-
+    support different tiff formats.
     """
 
     _pyramid_index: int
 
     def __init__(
-        self, page: TiffPage, fh: FileHandle, add_rgb_colorspace_fix: bool = False
+        self,
+        page: TiffPage,
+        fh: LockableFileHandle,
+        add_rgb_colorspace_fix: bool = False,
     ):
         """Abstract class for reading tiles from TiffPage.
 
         Parameters
         ----------
         page: TiffPage
             TiffPage to get tiles from.
-        fh: FileHandle
+        fh: LockableFileHandle
             FileHandle for reading data.
         add_rgb_colorspace_fix: bool = False
             If to add color space fix for rgb image data.
         """
+        if (
+            self.supported_compressions is not None
+            and page.compression not in self.supported_compressions
+        ):
+            raise NotImplementedError(f"Non-supported compression {self.compression}.")
         self._page = page
-        self._fh = LockableFileHandle(fh)
+        self._fh = fh
         self._add_rgb_colorspace_fix = add_rgb_colorspace_fix
-        self._image_size = Size(self._page.shape[1], self._page.shape[0])
+        self._image_size = Size(self._page.imagewidth, self._page.imagelength)
         if self.page.is_tiled:
             self._tile_size = Size(self.page.tilewidth, self.page.tilelength)
         else:
             self._tile_size = self.image_size
         self._tiled_region = Region(position=Point(0, 0), size=self.tiled_size)
 
     @abstractmethod
     def __repr__(self) -> str:
         raise NotImplementedError()
 
     def __str__(self) -> str:
         return f"{type(self).__name__} of page {self._page}"
 
     @property
+    @abstractmethod
+    def pixel_spacing(self) -> Optional[SizeMm]:
+        """Should return the pixel size in mm/pixel of the image."""
+        raise NotImplementedError()
+
+    @property
+    @abstractmethod
+    def supported_compressions(self) -> Optional[List[COMPRESSION]]:
+        """Should return list of compressions supported, or None if class is
+        indenpendent on compression."""
+        raise NotImplementedError()
+
+    @property
     def filepath(self) -> Path:
         return self._fh.filepath
 
     @property
     def suggested_minimum_chunk_size(self) -> int:
         """Suggested minimum chunk size regarding performance for reading
         multiple tiles (get_tiles())."""
         return 1
 
     @property
     def compression(self) -> COMPRESSION:
-        """Return compression of page."""
+        """Return compression of image."""
         return COMPRESSION(self._page.compression)
 
     @property
     def photometric_interpretation(self) -> PHOTOMETRIC:
         """Return photometric interpretation, e.g. 'YCBCR" or "RGB"."""
         return PHOTOMETRIC(self._page.photometric)
 
@@ -189,14 +199,19 @@
 
     @property
     def samples_per_pixel(self) -> int:
         """Return samples per pixel."""
         return self._page.samplesperpixel
 
     @property
+    def bit_depth(self) -> int:
+        """Return the sample bit depth."""
+        return self._page.bitspersample
+
+    @property
     def page(self) -> TiffPage:
         """Return source TiffPage."""
         return self._page
 
     @property
     def focal_plane(self) -> float:
         """Return focal plane (in um)."""
@@ -211,15 +226,15 @@
     @property
     def image_size(self) -> Size:
         """The pixel size of the image."""
         return self._image_size
 
     @property
     def tile_size(self) -> Size:
-        """The pixel size of the tiles. Returns image size if not tiled page"""
+        """The pixel size of the tiles. Returns image size if not tiled image"""
         return self._tile_size
 
     @property
     def tiled_size(self) -> Size:
         """The size of the image when tiled."""
         if self.tile_size == Size(0, 0):
             return Size(1, 1)
@@ -227,20 +242,14 @@
 
     @property
     def pyramid_index(self) -> int:
         """The pyramidal index in relation to the base layer. Returns 0 for
         images not in pyramidal series."""
         return self._pyramid_index
 
-    @property
-    @abstractmethod
-    def pixel_spacing(self) -> Optional[SizeMm]:
-        """Should return the pixel size in mm/pixel of the page."""
-        raise NotImplementedError()
-
     @abstractmethod
     def get_tile(self, tile_position: Tuple[int, int]) -> bytes:
         """Should return image bytes for tile at tile position.
 
         Parameters
         ----------
         tile_position: Tuple[int, int]
@@ -297,24 +306,56 @@
         Returns
         ----------
         List[np.ndarray]
             List of decoded tiles.
         """
         return [self.get_decoded_tile(tile) for tile in tile_positions]
 
+    def get_all_tiles(self, raw: bool = False) -> Iterator[bytes]:
+        """Return iterator of all tiles in image.
+
+        Parameters
+        ----------
+        raw: bool = False
+            Set to True to not do any format-specifc processing on the tile.
+
+        Returns
+        ----------
+        Iterator[bytes]
+            Iterator of all tiles in image.
+        """
+        if raw:
+            return (self._read_frame(index) for index in range(self.tiled_size.area))
+        return (
+            self.get_tile(tile.to_tuple()) for tile in self.tiled_region.iterate_all()
+        )
+
+    def get_all_tiles_decoded(self) -> Iterator[np.ndarray]:
+        """Return iterator of all tiles in image decoded.
+
+        Returns
+        ----------
+        Iterator[np.ndarray]
+            Iterator of all tiles in image decoded.
+        """
+        return (
+            self.get_decoded_tile(tile.to_tuple())
+            for tile in self.tiled_region.iterate_all()
+        )
+
     def close(self) -> None:
         """Close filehandle."""
         self._fh.close()
 
     def pretty_str(self, indent: int = 0, depth: Optional[int] = None) -> str:
         return str(self)
 
     @property
     def tiled_region(self) -> Region:
-        """Tile region covering the OpenTilePage."""
+        """Tile region covering the TiffImage."""
         return self._tiled_region
 
     def valid_tiles(self, region: Region) -> bool:
         """Check if tile region is inside tile geometry and z coordinate and
         optical path exists.
 
         Parameters
@@ -356,32 +397,31 @@
             and tile_position.y < self.tiled_size.height
         )
 
     @staticmethod
     def _get_value_from_tiff_tags(
         tiff_tags: TiffTags, value_name: str
     ) -> Optional[str]:
-        for tag in tiff_tags:
-            if tag.name == value_name:
-                return str(tag.value)
-        return None
+        return next(
+            (str(tag.value) for tag in tiff_tags if tag.name == value_name), None
+        )
 
     def _calculate_pyramidal_index(
         self,
-        base_shape: Size,
+        base_size: Size,
     ) -> int:
-        return int(math.log2(base_shape.width / self.image_size.width))
+        return int(math.log2(base_size.width / self.image_size.width))
 
     def _calculate_mpp(self, base_mpp: SizeMm) -> SizeMm:
         return base_mpp * pow(2, self.pyramid_index)
 
 
-class NativeTiledPage(OpenTilePage, metaclass=ABCMeta):
+class NativeTiledTiffImage(TiffImage, metaclass=ABCMeta):
 
-    """Meta class for pages that are natively tiled (e.g. not ndpi)"""
+    """Meta class for images that are natively tiled (e.g. not ndpi)"""
 
     def get_tile(self, tile_position: Tuple[int, int]) -> bytes:
         """Return image bytes for tile at tile position.
 
         Parameters
         ----------
         tile_position: Tuple[int, int]
@@ -458,191 +498,7 @@
         data.shape = shape[1:]
         return data
 
     def _tile_point_to_frame_index(self, tile_point: Point) -> int:
         """Return linear frame index for tile position."""
         frame_index = tile_point.y * self.tiled_size.width + tile_point.x
         return frame_index
-
-
-class Tiler(metaclass=ABCMeta):
-    """Abstract class for reading pages from TiffFile."""
-
-    _level_series_index: int = 0
-    _overview_series_index: Optional[int] = None
-    _label_series_index: Optional[int] = None
-    _icc_profile: Optional[bytes] = None
-
-    def __init__(self, filepath: Path):
-        """Abstract class for reading pages from TiffFile.
-
-        Parameters
-        ----------
-        filepath: Path
-            Filepath to a TiffFile.
-        """
-        self._tiff_file = TiffFile(filepath)
-        base_page = self.series[self._level_series_index].pages[0]
-        assert isinstance(base_page, TiffPage)
-        self._base_page = base_page
-        self._base_size = Size(self.base_page.shape[1], self.base_page.shape[0])
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.close()
-
-    @property
-    def metadata(self) -> Metadata:
-        raise NotImplementedError()
-
-    @property
-    def base_page(self) -> TiffPage:
-        """Return base pyramid level in pyramid series."""
-        return self._base_page
-
-    @property
-    def base_size(self) -> Size:
-        """Return size of base pyramid level in pyramid series."""
-        return self._base_size
-
-    @property
-    def series(self) -> List[TiffPageSeries]:
-        """Return contained TiffPageSeries."""
-        return self._tiff_file.series
-
-    @property
-    def levels(self) -> List[OpenTilePage]:
-        """Return list of pyramid level OpenTilePages."""
-        if self._level_series_index is None:
-            return []
-        return [
-            self.get_level(level_index, page_index)
-            for level_index, level in enumerate(
-                self.series[self._level_series_index].levels
-            )
-            for page_index, page in enumerate(level.pages)
-        ]
-
-    @property
-    def labels(self) -> List[OpenTilePage]:
-        """Return list of label OpenTilePage."""
-        if self._label_series_index is None:
-            return []
-        return [
-            self.get_label(page_index)
-            for page_index, page in enumerate(
-                self.series[self._label_series_index].pages
-            )
-        ]
-
-    @property
-    def overviews(self) -> List[OpenTilePage]:
-        """Return list of overview OpenTilePage."""
-        if self._overview_series_index is None:
-            return []
-        return [
-            self.get_overview(page_index)
-            for page_index, page in enumerate(
-                self.series[self._overview_series_index].pages
-            )
-        ]
-
-    @property
-    def icc_profile(self) -> Optional[bytes]:
-        """Return icc profile if found in file."""
-        return self._icc_profile
-
-    @abstractmethod
-    def get_page(self, series: int, level: int, page: int) -> OpenTilePage:
-        """Should return a OpenTilePage for series, level, page in file."""
-        raise NotImplementedError()
-
-    @abstractclassmethod
-    def supported(cls, tiff_file: TiffFile) -> bool:
-        raise NotImplementedError()
-
-    def close(self) -> None:
-        """CLose tiff-file."""
-        self._tiff_file.close()
-
-    def get_tile(
-        self, series: int, level: int, page: int, tile_position: Tuple[int, int]
-    ) -> bytes:
-        """Return list of image bytes for tiles at tile positions.
-
-        Parameters
-        ----------
-        series: int
-            Series of page to get tile from.
-        level: int
-            Level of page to get tile from.
-        page: int
-            Page to get tile from.
-        tile_position: Tuple[int, int]
-            Position of tile to get.
-
-        Returns
-        ----------
-        bytes
-            Tile at position.
-        """
-        tiled_page = self.get_page(series, level, page)
-        return tiled_page.get_tile(tile_position)
-
-    def get_level(self, level: int, page: int = 0) -> OpenTilePage:
-        """Return OpenTilePage for level in pyramid series.
-
-        Parameters
-        ----------
-        level: int
-            Level to get.
-        page: int
-            Index of page to get.
-
-        Returns
-        ----------
-        OpenTilePage
-            Level OpenTilePage.
-        """
-        return self.get_page(self._level_series_index, level, page)
-
-    def get_label(self, page: int = 0) -> OpenTilePage:
-        """Return OpenTilePage for label in label series.
-
-        Parameters
-        ----------
-        page: int
-            Index of page to get.
-
-        Returns
-        ----------
-        OpenTilePage
-            Label OpenTilePage.
-        """
-        if self._label_series_index is None:
-            raise ValueError("No label detected in file")
-        return self.get_page(self._label_series_index, 0, page)
-
-    def get_overview(self, page: int = 0) -> OpenTilePage:
-        """Return OpenTilePage for overview in overview series.
-
-        Parameters
-        ----------
-        page: int
-            Index of page to get.
-
-        Returns
-        ----------
-        OpenTilePage
-            Overview OpenTilePage.
-        """
-        if self._overview_series_index is None:
-            raise ValueError("No overview detected in file")
-        return self.get_page(self._overview_series_index, 0, page)
-
-    def _get_tiff_page(self, series: int, level: int, page: int) -> TiffPage:
-        """Return TiffPage for series, level, page."""
-        tiff_page = self.series[series].levels[level].pages[page]
-        assert isinstance(tiff_page, TiffPage)
-        return tiff_page
```

### Comparing `opentile-0.8.1/opentile/geometry.py` & `opentile-0.9.0/opentile/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-#    Copyright 2021 SECTRA AB
+#    Copyright 2021-2023 SECTRA AB
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
+"""Geometry classes."""
+
 import math
 from dataclasses import dataclass
 from typing import Generator, Sequence, Tuple, Union
 
 
 @dataclass
 class SizeMm:
```

### Comparing `opentile-0.8.1/opentile/histech_tiff_tiler.py` & `opentile-0.9.0/opentile/formats/philips/philips_tiff_image.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,136 +1,137 @@
-#    Copyright 2022 SECTRA AB
+#    Copyright 2021-2023 SECTRA AB
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
-from pathlib import Path
-from typing import Dict, Optional, Tuple, Union
+"""Image implementation for Philips tiff files."""
 
-from tifffile.tifffile import (
-    PHOTOMETRIC,
-    FileHandle,
-    TiffFile,
-    TiffPage,
-    TiffPageSeries,
-)
+from typing import List, Optional
+
+from tifffile.tifffile import COMPRESSION, TiffPage
 
-from opentile.common import NativeTiledPage, Tiler
 from opentile.geometry import Size, SizeMm
 from opentile.jpeg import Jpeg
-from opentile.metadata import Metadata
+from opentile.tiff_image import LockableFileHandle, NativeTiledTiffImage
 
 
-class HistechTiffTiledPage(NativeTiledPage):
-    def __init__(self, page: TiffPage, fh: FileHandle, base_shape: Size):
-        """OpenTiledPage for 3DHistech Tiff-page.
+class PhilipsTiffImage(NativeTiledTiffImage):
+    def __init__(
+        self,
+        page: TiffPage,
+        fh: LockableFileHandle,
+        base_size: Size,
+        base_mpp: SizeMm,
+        jpeg: Jpeg,
+    ):
+        """OpenTiledPage for Philips Tiff image.
 
         Parameters
         ----------
         page: TiffPage
             TiffPage defining the page.
-        fh: FileHandler
+        fh: LockableFileHandle
             Filehandler to read data from.
-        base_shape: Size
+        base_size: Size
             Size of base level in pyramid.
+        base_mpp: SizeMm
+            Mpp (um/pixel) for base level in pyramid.
+        jpeg: Jpeg
+            Jpeg instance to use.
         """
         super().__init__(page, fh)
-        self._base_shape = base_shape
-        self._pyramid_index = self._calculate_pyramidal_index(self._base_shape)
-        self._mpp = self._get_mpp_from_page()
+        self._jpeg = jpeg
+        self._base_size = base_size
+        self._base_mpp = base_mpp
+        self._pyramid_index = self._calculate_pyramidal_index(self._base_size)
+        self._mpp = self._calculate_mpp(self._base_mpp)
+        self._blank_tile = self._create_blank_tile()
 
     def __repr__(self) -> str:
         return (
-            f"{type(self).__name__}({self._page}, {self._fh}, " f"{self._base_shape})"
+            f"{type(self).__name__}({self._page}, {self._fh}, "
+            f"{self._base_size}, {self._base_mpp}, {self._jpeg})"
         )
 
     @property
     def pixel_spacing(self) -> SizeMm:
         """Return pixel spacing in mm per pixel."""
         return self.mpp * 1000
 
     @property
+    def supported_compressions(self) -> Optional[List[COMPRESSION]]:
+        return [COMPRESSION.JPEG]
+
+    @property
     def mpp(self) -> SizeMm:
         """Return pixel spacing in um per pixel."""
         return self._mpp
 
     @property
-    def photometric_interpretation(self) -> PHOTOMETRIC:
-        photometric_interpretation = PHOTOMETRIC(self._page.photometric)
-        if photometric_interpretation == PHOTOMETRIC.PALETTE:
-            return PHOTOMETRIC.MINISBLACK
-        return photometric_interpretation
-
-    def _get_mpp_from_page(self) -> SizeMm:
-        items_split = self._page.description.split("|")
-        header = items_split.pop(0)
-        items = {
-            key: value
-            for (key, value) in (item.split(" = ", 1) for item in items_split)
-        }
-        return (
-            SizeMm(float(items["3dh_PixelSizeX"]), float(items["3dh_PixelSizeY"]))
-            / 1000
-            / 1000
-        )
-
-
-class HistechTiffTiler(Tiler):
-    def __init__(
-        self, filepath: Union[str, Path], turbo_path: Optional[Union[str, Path]] = None
-    ):
-        """Tiler for 3DHistech tiff file.
+    def blank_tile(self) -> bytes:
+        """Return blank tile."""
+        return self._blank_tile
+
+    def _create_blank_tile(self, luminance: float = 1.0) -> bytes:
+        """Create a blank tile from a valid tile. Uses the first found
+        valid frame (first frame with non-zero value in databytescounts) and
+        fills that image with white.
 
         Parameters
         ----------
-        filepath: Union[str, Path]
-            Filepath to a 3DHistech-TiffFile.
-        """
-        super().__init__(Path(filepath))
-        self._fh = self._tiff_file.filehandle
-
-        self._turbo_path = turbo_path
-        self._jpeg = Jpeg(self._turbo_path)
+        luminance: float = 1.0
+            Luminance for tile, 0 = black, 1 = white.
 
-        self._level_series_index = 0
-        for series_index, series in enumerate(self.series):
-            if self.is_label(series):
-                self._label_series_index = series_index
-            elif self.is_overview(series):
-                self._overview_series_index = series_index
-        self._pages: Dict[Tuple[int, int, int], HistechTiffTiledPage] = {}
+        Returns
+        ----------
+        bytes:
+            Frame bytes from blank tile.
 
-    @property
-    def metadata(self) -> Metadata:
-        """No known metadata for 3DHistech tiff files."""
-        return Metadata()
-
-    @classmethod
-    def supported(cls, tiff_file: TiffFile) -> bool:
-        return "3dh_PixelSizeX" in tiff_file.pages.first.description
-
-    def get_page(self, series: int, level: int, page: int = 0) -> HistechTiffTiledPage:
-        """Return PhilipsTiffTiledPage for series, level, page."""
-        if not (series, level, page) in self._pages:
-            self._pages[series, level, page] = HistechTiffTiledPage(
-                self._get_tiff_page(series, level, page), self._fh, self.base_size
+        """
+        # Todo, figure out what color to fill with.
+        try:
+            # Get first frame in page that is not 0 bytes
+            valid_frame_index = next(
+                index
+                for index, datalength in enumerate(self.page.databytecounts)
+                if datalength != 0
             )
-        return self._pages[series, level, page]
+        except StopIteration as exception:
+            raise ValueError("Could not find valid frame in image.") from exception
+        tile = self._read_frame(valid_frame_index)
+        if self.page.jpegtables is not None:
+            tile = Jpeg.add_jpeg_tables(tile, self.page.jpegtables, False)
+        tile = self._jpeg.fill_frame(tile, luminance)
+        return tile
+
+    def _read_frame(self, index: int) -> bytes:
+        """Read frame at frame index from image. Return blank tile if tile is
+        sparse (length of frame is zero or frame indexis outside length of
+        frames)
 
-    @staticmethod
-    def is_overview(series: TiffPageSeries) -> bool:
-        """Return true if series is a overview series."""
-        return False
-
-    @staticmethod
-    def is_label(series: TiffPageSeries) -> bool:
-        """Return true if series is a label series."""
-        return False
+        Parameters
+        ----------
+        index: int
+            Frame index to read from image.
+
+        Returns
+        ----------
+        bytes:
+            Frame bytes from frame index or blank tile.
+
+        """
+        if (
+            index >= len(self.page.databytecounts)
+            or self.page.databytecounts[index] == 0
+        ):
+            # Sparse tile
+            return self.blank_tile
+        return super()._read_frame(index)
```

### Comparing `opentile-0.8.1/opentile/interface.py` & `opentile-0.9.0/opentile/opentile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,97 @@
-#    Copyright 2021 SECTRA AB
+#    Copyright 2021-2023 SECTRA AB
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
+"""Main interface for OpenTile."""
+
 from pathlib import Path
 from typing import Dict, Optional, Tuple, Type, Union
 
 from tifffile import TiffFile, TiffFileError
 
-from opentile.common import Tiler
-from opentile.histech_tiff_tiler import HistechTiffTiler
-from opentile.ndpi_tiler import NdpiTiler
-from opentile.philips_tiff_tiler import PhilipsTiffTiler
-from opentile.svs_tiler import SvsTiler
-from opentile.turbojpeg_patch import find_turbojpeg_path
+from opentile.formats import (
+    HistechTiffTiler,
+    NdpiTiler,
+    OmeTiffTiler,
+    PhilipsTiffTiler,
+    SvsTiler,
+)
+from opentile.tiler import Tiler
 
 
 class OpenTile:
-    @staticmethod
-    def get_tiler(
-        filepath: Union[str, Path]
-    ) -> Tuple[Optional[str], Optional[Type[Tiler]]]:
-        """Return tiler that supports the tiff file in filepath, or None if
-        not supported"""
-        tilers: Dict[str, Type[Tiler]] = {
-            "ndpi": NdpiTiler,
-            "svs": SvsTiler,
-            "phillips_tiff": PhilipsTiffTiler,
-            "3dhistech tiff": HistechTiffTiler,
-        }
-        try:
-            tiff_file = TiffFile(filepath)
-            return next(
-                (tiler_name, tiler)
-                for (tiler_name, tiler) in tilers.items()
-                if tiler.supported(tiff_file)
-            )
-        except (TiffFileError, StopIteration):
-            return None, None
-
-    @classmethod
-    def detect_format(cls, filepath: Union[str, Path]) -> Optional[str]:
-        format, supported_tiler = cls.get_tiler(filepath)
-        return format
-
     @classmethod
     def open(
         cls,
         filepath: Union[str, Path],
         tile_size: int = 512,
+        turbo_path: Optional[Union[str, Path]] = None,
     ) -> Tiler:
         """Return a file type specific tiler for tiff file in filepath.
         Tile size and turbo jpeg path are optional but required for some file
         types.
 
         Parameters
         ----------
         filepath: Union[str, Path]
             Path to tiff file.
         tile_size: int = 512
             Tile size for creating tiles, if needed for file format.
+        turbo_path: Optional[Union[str, Path]] = None
+            Path to turbojpeg (dll or so).
         """
         format, supported_tiler = cls.get_tiler(filepath)
         if supported_tiler is NdpiTiler:
-            return NdpiTiler(filepath, tile_size, find_turbojpeg_path())
+            return NdpiTiler(filepath, tile_size, turbo_path)
 
         if supported_tiler is SvsTiler:
-            return SvsTiler(filepath, find_turbojpeg_path())
+            return SvsTiler(filepath, turbo_path)
 
         if supported_tiler is PhilipsTiffTiler:
-            return PhilipsTiffTiler(filepath, find_turbojpeg_path())
+            return PhilipsTiffTiler(filepath, turbo_path)
 
         if supported_tiler is HistechTiffTiler:
             return HistechTiffTiler(filepath)
 
+        if supported_tiler is OmeTiffTiler:
+            return OmeTiffTiler(filepath)
+
         raise NotImplementedError("Non supported tiff file")
+
+    @staticmethod
+    def get_tiler(
+        filepath: Union[str, Path]
+    ) -> Tuple[Optional[str], Optional[Type[Tiler]]]:
+        """Return tiler that supports the tiff file in filepath, or None if
+        not supported"""
+        tilers: Dict[str, Type[Tiler]] = {
+            "ndpi": NdpiTiler,
+            "svs": SvsTiler,
+            "phillips tiff": PhilipsTiffTiler,
+            "3dhistech tiff": HistechTiffTiler,
+            "ome-tiff tiler": OmeTiffTiler,
+        }
+        try:
+            tiff_file = TiffFile(filepath)
+            return next(
+                (tiler_name, tiler)
+                for (tiler_name, tiler) in tilers.items()
+                if tiler.supported(tiff_file)
+            )
+        except (TiffFileError, StopIteration):
+            return None, None
+
+    @classmethod
+    def detect_format(cls, filepath: Union[str, Path]) -> Optional[str]:
+        format, supported_tiler = cls.get_tiler(filepath)
+        return format
```

### Comparing `opentile-0.8.1/opentile/jpeg.py` & `opentile-0.9.0/opentile/jpeg/jpeg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-#    Copyright 2021 SECTRA AB
+#    Copyright 2021-2023 SECTRA AB
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
+"""Lossless jpeg handling and encoding and decoding."""
+
 from pathlib import Path
 from struct import pack, unpack
 from typing import Iterator, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 from turbojpeg import TJPF_RGB, tjMCUHeight, tjMCUWidth
 
 from opentile.geometry import Size
-from opentile.turbojpeg_patch import TurboJPEG_patch as TurboJPEG
-from opentile.turbojpeg_patch import find_turbojpeg_path
+from opentile.jpeg.turbojpeg_patch import TurboJPEG_patch as TurboJPEG
+from opentile.jpeg.turbojpeg_patch import find_turbojpeg_path
 
 
 class JpegTagNotFound(Exception):
     """Raised when expected Jpeg tag was not found."""
 
     pass
 
@@ -228,16 +230,16 @@
         List[bytes]:
             Croped frames.
         """
         try:
             return self._turbo_jpeg.crop_multiple(frame, crop_parameters)
         except OSError as exception:
             raise JpegCropError(
-                f"Crop of frame failed with parameters {crop_parameters}.", exception
-            )
+                f"Crop of frame failed " f"with parameters {crop_parameters}"
+            ) from exception
 
     @classmethod
     def add_jpeg_tables(
         cls,
         frame: bytes,
         jpeg_tables: bytes,
         apply_rgb_colorspace_fix: Optional[bool] = False,
```

### Comparing `opentile-0.8.1/opentile/metadata.py` & `opentile-0.9.0/opentile/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-#    Copyright 2022 SECTRA AB
+#    Copyright 2022-2023 SECTRA AB
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
+"""Base metadata class."""
+
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Tuple
 
 from tifffile.tifffile import TiffTags
 
 
 class Metadata:
```

### Comparing `opentile-0.8.1/opentile/philips_tiff_tiler.py` & `opentile-0.9.0/opentile/formats/svs/svs_image.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,314 +1,430 @@
-#    Copyright 2021 SECTRA AB
+#    Copyright 2021-2023 SECTRA AB
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
-from datetime import datetime
-from functools import cached_property
-from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple, Type, TypeVar, Union
-from xml.etree import ElementTree
+"""Image implementations for svs tiff files."""
 
-from tifffile.tifffile import FileHandle, TiffFile, TiffPage, TiffPageSeries
+import io
+from typing import Dict, List, Optional, Sequence, Tuple
 
-from opentile.common import NativeTiledPage, Tiler
-from opentile.geometry import Size, SizeMm
+import numpy as np
+from PIL import Image
+from tifffile.tifffile import COMPRESSION, TiffPage
+
+from opentile.geometry import Point, Region, Size, SizeMm
 from opentile.jpeg import Jpeg
-from opentile.metadata import Metadata
+from opentile.tiff_image import LockableFileHandle, NativeTiledTiffImage, TiffImage
+
+
+class SvsStripedImage(TiffImage):
+    _pyramid_index = 0
+
+    def __init__(self, page: TiffPage, fh: LockableFileHandle, jpeg: Jpeg):
+        """OpenTiledPage for jpeg striped Svs image, e.g. overview image.
+
+        Parameters
+        ----------
+        page: TiffPage
+            TiffPage defining the page.
+        fh: LockableFileHandle
+            Filehandler to read data from.
+        jpeg: Jpeg
+            Jpeg instance to use.
+
+        """
+        super().__init__(page, fh, True)
+        self._jpeg = jpeg
+
+    def __repr__(self) -> str:
+        return f"{type(self).__name__}({self._page}, {self._fh}, {self._jpeg}"
+
+    @property
+    def pixel_spacing(self) -> Optional[SizeMm]:
+        return None
+
+    @property
+    def supported_compressions(self) -> Optional[List[COMPRESSION]]:
+        return [COMPRESSION.JPEG]
+
+    def get_tile(self, tile_position: Tuple[int, int]) -> bytes:
+        """Return tile for tile position.
+
+        Parameters
+        ----------
+        tile_position: Tuple[int, int]
+            Tile position to get.
+
+        Returns
+        ----------
+        bytes
+            Produced tile at position.
+        """
+        if tile_position != (0, 0):
+            raise ValueError("Non-tiled image, expected tile_position (0, 0)")
+        indices = range(len(self.page.dataoffsets))
+        scans = (self._read_frame(index) for index in indices)
+        jpeg_tables = self.page.jpegtables
+        frame = self._jpeg.concatenate_scans(
+            scans, jpeg_tables, self._add_rgb_colorspace_fix
+        )
+        return frame
+
+    def get_decoded_tile(self, tile_position: Tuple[int, int]) -> np.ndarray:
+        """Return decoded tile for tile position.
+
+        Parameters
+        ----------
+        tile_position: Tuple[int, int]
+            Tile position to get.
+
+        Returns
+        ----------
+        bytes
+            Produced tile at position.
+        """
+        return self._jpeg.decode(self.get_tile(tile_position))
+
+
+class SvsLZWImage(TiffImage):
+    _pyramid_index = 0
+
+    def __init__(self, page: TiffPage, fh: LockableFileHandle, jpeg: Jpeg):
+        """OpenTiledPage for lzw striped Svs image, e.g. label image.
+
+        Parameters
+        ----------
+        page: TiffPage
+            TiffPage defining the page.
+        fh: LockableFileHandle
+            Filehandler to read data from.
+        jpeg: Jpeg
+            Jpeg instance to use.
+
+        """
+        super().__init__(page, fh)
+        self._jpeg = jpeg
+
+    def __repr__(self) -> str:
+        return f"{type(self).__name__}({self._page}, {self._fh}, {self._jpeg}"
+
+    @property
+    def compression(self) -> COMPRESSION:
+        """Return compression of page."""
+        return COMPRESSION.JPEG
+
+    @property
+    def pixel_spacing(self) -> Optional[SizeMm]:
+        return None
+
+    @property
+    def supported_compressions(self) -> Optional[List[COMPRESSION]]:
+        return [COMPRESSION.LZW]
+
+    def get_tile(self, tile_position: Tuple[int, int]) -> bytes:
+        """Return tile for tile position.
+
+        Parameters
+        ----------
+        tile_position: Tuple[int, int]
+            Tile position to get.
+
+        Returns
+        ----------
+        bytes
+            Produced tile at position.
+        """
+        return self._jpeg.encode(self.get_decoded_tile(tile_position))
 
+    def get_decoded_tile(self, tile_position: Tuple[int, int]) -> np.ndarray:
+        """Return decoded tile for tile position.
 
-class PhilipsTiffTiledPage(NativeTiledPage):
+        Parameters
+        ----------
+        tile_position: Tuple[int, int]
+            Tile position to get.
+
+        Returns
+        ----------
+        bytes
+            Produced tile at position.
+        """
+        if tile_position != (0, 0):
+            raise ValueError("Non-tiled image, expected tile_position (0, 0)")
+
+        tile = np.concatenate(
+            [self._get_row(index) for index in range(len(self.page.dataoffsets))],
+            axis=1,
+        )
+        return np.squeeze(tile)
+
+    def _get_row(self, index: int) -> np.ndarray:
+        row = self.page.decode(self._read_frame(index), index)[0]
+        assert isinstance(row, np.ndarray)
+        return row
+
+
+class SvsTiledImage(NativeTiledTiffImage):
     def __init__(
         self,
         page: TiffPage,
-        fh: FileHandle,
-        base_shape: Size,
+        fh: LockableFileHandle,
+        base_size: Size,
         base_mpp: SizeMm,
-        jpeg: Jpeg,
+        parent: Optional[TiffImage] = None,
     ):
-        """OpenTiledPage for Philips Tiff-page.
+        """Svs Tiff tiled image.
 
         Parameters
         ----------
         page: TiffPage
             TiffPage defining the page.
-        fh: FileHandle
+        fh: LockableFileHandle
             Filehandler to read data from.
-        base_shape: Size
+        base_size: Size
             Size of base level in pyramid.
         base_mpp: SizeMm
             Mpp (um/pixel) for base level in pyramid.
-        jpeg: Jpeg
-            Jpeg instance to use.
+        parent: Optional[TiffImage] = None
+            Parent TiffImage
         """
-        super().__init__(page, fh)
-        self._jpeg = jpeg
-        self._base_shape = base_shape
+
+        super().__init__(page, fh, True)
+        self._base_size = base_size
         self._base_mpp = base_mpp
-        self._pyramid_index = self._calculate_pyramidal_index(self._base_shape)
+        self._pyramid_index = self._calculate_pyramidal_index(self._base_size)
         self._mpp = self._calculate_mpp(self._base_mpp)
-        self._blank_tile = self._create_blank_tile()
+        self._parent = parent
+        (
+            self._right_edge_corrupt,
+            self._bottom_edge_corrupt,
+        ) = self._detect_corrupt_edges()
+        self._fixed_tiles: Dict[Point, bytes] = {}
 
     def __repr__(self) -> str:
         return (
             f"{type(self).__name__}({self._page}, {self._fh}, "
-            f"{self._base_shape}, {self._base_mpp}, {self._jpeg})"
+            f"{self._base_size}, {self._base_mpp})"
         )
 
     @property
     def pixel_spacing(self) -> SizeMm:
         """Return pixel spacing in mm per pixel."""
-        return self.mpp * 1000
+        return self.mpp / 1000
+
+    @property
+    def supported_compressions(self) -> Optional[List[COMPRESSION]]:
+        return [COMPRESSION.JPEG, COMPRESSION.APERIO_JP2000_RGB]
 
     @property
     def mpp(self) -> SizeMm:
         """Return pixel spacing in um per pixel."""
         return self._mpp
 
     @property
-    def blank_tile(self) -> bytes:
-        """Return blank tile."""
-        return self._blank_tile
+    def right_edge_corrupt(self) -> bool:
+        return self._right_edge_corrupt
 
-    def _create_blank_tile(self, luminance: float = 1.0) -> bytes:
-        """Create a blank tile from a valid tile. Uses the first found
-        valid frame (first frame with non-zero value in databytescounts) and
-        fills that image with white.
+    @property
+    def bottom_edge_corrupt(self) -> bool:
+        return self._bottom_edge_corrupt
 
+    def _detect_corrupt_edge(self, edge: Region) -> bool:
+        """Return true if tiles at edge are corrupt (any tile has a frame
+        that has 0 data length)
         Parameters
         ----------
-        luminance: float = 1.0
-            Luminance for tile, 0 = black, 1 = white.
+        edge: Region
+            Edge to check for corrupt tiles.
 
         Returns
         ----------
-        bytes:
-            Frame bytes from blank tile.
+        bool:
+            True if edge contains corrupt tiles.
+        """
+        for tile in edge.iterate_all():
+            frame_index = self._tile_point_to_frame_index(tile)
+            if self._page.databytecounts[frame_index] == 0:
+                return True
+        return False
+
+    def _detect_corrupt_edges(self) -> Tuple[bool, bool]:
+        """Returns tuple bool indiciting if right and/or bottom edge of page is
+        corrupt. Bottom and right edge tiles in svs pyramid levels > 1 can
+        sometimes corrupt. This manifests as tiles with 0-length (easy to
+        detect) and tiles with scrambled image data (not so easy detect).
+
+        Returns
+        ----------
+        Tuple[bool, bool]:
+            Tuple indicating if right and/or bottom edge is corrupt.
 
         """
-        # Todo, figure out what color to fill with.
-        try:
-            # Get first frame in page that is not 0 bytes
-            valid_frame_index = next(
-                index
-                for index, datalength in enumerate(self.page.databytecounts)
-                if datalength != 0
-            )
-        except StopIteration:
-            raise ValueError("Could not find valid frame in page.")
-        tile = self._read_frame(valid_frame_index)
-        if self.page.jpegtables is not None:
-            tile = Jpeg.add_jpeg_tables(tile, self.page.jpegtables, False)
-        tile = self._jpeg.fill_frame(tile, luminance)
-        return tile
-
-    def _read_frame(self, index: int) -> bytes:
-        """Read frame at frame index from page. Return blank tile if tile is
-        sparse (length of frame is zero or frame indexis outside length of
-        frames)
+        if self.pyramid_index == 0:
+            return False, False
+        right_edge = Region(
+            Point(self.tiled_size.width - 1, 0), Size(1, self.tiled_size.height - 1)
+        )
+        right_edge_corrupt = self._detect_corrupt_edge(right_edge)
+
+        bottom_edge = Region(
+            Point(0, self.tiled_size.height - 1), Size(self.tiled_size.width - 1, 1)
+        )
+        bottom_edge_corrupt = self._detect_corrupt_edge(bottom_edge)
+
+        return right_edge_corrupt, bottom_edge_corrupt
+
+    def _tile_is_at_right_edge(self, tile_point: Point) -> bool:
+        """Return true if tile is at right edge of tiled image."""
+        return tile_point.x == self.tiled_size.width - 1
+
+    def _tile_is_at_bottom_edge(self, tile_point: Point) -> bool:
+        """Return true if tile is at bottom edge of tiled image."""
+        return tile_point.y == self.tiled_size.height - 1
+
+    def _get_scaled_tile(self, tile_point: Point) -> bytes:
+        """Create a tile by downscaling from a lower (higher resolution)
+        level.
 
         Parameters
         ----------
-        index: int
-            Frame index to read from page.
+        tile_point: Point
+            Position of tile in this pyramid level.
 
         Returns
         ----------
         bytes:
-            Frame bytes from frame index or blank tile.
+            Scaled tile bytes.
 
         """
-        if (
-            index >= len(self.page.databytecounts)
-            or self.page.databytecounts[index] == 0
-        ):
-            # Sparse tile
-            return self.blank_tile
-        return super()._read_frame(index)
-
-
-CastType = TypeVar("CastType", int, float, str)
-
-
-class PhilipsMetadata(Metadata):
-    _scanner_manufacturer: Optional[str] = None
-    _scanner_software_versions: Optional[List[str]] = None
-    _scanner_serial_number: Optional[str] = None
-    _pixel_spacing: Optional[Tuple[float, float]] = None
-
-    TAGS = [
-        "DICOM_PIXEL_SPACING",
-        "DICOM_ACQUISITION_DATETIME",
-        "DICOM_MANUFACTURER",
-        "DICOM_SOFTWARE_VERSIONS",
-        "DICOM_DEVICE_SERIAL_NUMBER",
-        "DICOM_LOSSY_IMAGE_COMPRESSION_METHOD",
-        "DICOM_LOSSY_IMAGE_COMPRESSION_RATIO",
-        "DICOM_BITS_ALLOCATED",
-        "DICOM_BITS_STORED",
-        "DICOM_HIGH_BIT",
-        "DICOM_PIXEL_REPRESENTATION",
-    ]
-
-    def __init__(self, tiff_file: TiffFile):
-        if tiff_file.philips_metadata is None:
-            return
-
-        metadata = ElementTree.fromstring(tiff_file.philips_metadata)
-        self._tags: Dict[str, Optional[str]] = {tag: None for tag in self.TAGS}
-        for element in metadata.iter():
-            if element.tag == "Attribute" and element.text is not None:
-                name = element.attrib["Name"]
-                if name in self._tags and self._tags[name] is None:
-                    self._tags[name] = element.text
+        if self._parent is None:
+            raise ValueError("No parent level to get tiles from")
+        scale = int(pow(2, self.pyramid_index - self._parent.pyramid_index))
+        scaled_tile_region = Region(tile_point, Size(1, 1)) * scale
+
+        # Get decoded tiles
+        decoded_tiles = self._parent.get_decoded_tiles(
+            [tile.to_tuple() for tile in scaled_tile_region.iterate_all()]
+        )
+        image_data = np.zeros(
+            (self.tile_size * scale).to_tuple() + (3,), dtype=np.uint8
+        )
+        # Insert decoded_tiles into image_data
+        for y in range(scale):
+            for x in range(scale):
+                image_data_index = y * scale + x
+                image_data[
+                    y * self.tile_size.width : (y + 1) * self.tile_size.width,
+                    x * self.tile_size.height : (x + 1) * self.tile_size.height,
+                ] = decoded_tiles[image_data_index]
+
+        # Resize image_data using Pillow
+        image: Image.Image = Image.fromarray(image_data)
+        image = image.resize(
+            self.tile_size.to_tuple(), resample=Image.Resampling.BILINEAR
+        )
 
-    @property
-    def scanner_manufacturer(self) -> Optional[str]:
-        return self._tags["DICOM_MANUFACTURER"]
+        # Return compressed image
+        if self.compression == COMPRESSION.JPEG:
+            image_format = "jpeg"
+            image_options = {"quality": 95}
+        elif self.compression == COMPRESSION.APERIO_JP2000_RGB:
+            image_format = "jpeg2000"
+            image_options = {"irreversible": True}
+        else:
+            raise NotImplementedError("Non-supported compression")
+        with io.BytesIO() as buffer:
+            image.save(buffer, format=image_format, **image_options)
+            frame = buffer.getvalue()
+
+        if self.compression == COMPRESSION.APERIO_JP2000_RGB:
+            # PIL encodes in jp2, find start of j2k and return from there.
+            START_TAGS = bytes([0xFF, 0x4F, 0xFF, 0x51])
+            start_index = frame.find(START_TAGS)
+            return frame[start_index:]
+        return frame
 
-    @cached_property
-    def scanner_software_versions(self) -> Optional[List[str]]:
-        print(self._tags["DICOM_SOFTWARE_VERSIONS"])
-        if self._tags["DICOM_SOFTWARE_VERSIONS"] is None:
-            return None
-        return self._split_and_cast_text(self._tags["DICOM_SOFTWARE_VERSIONS"], str)
+    def _get_fixed_tile(self, tile_point: Point) -> bytes:
+        """Get or create a fixed tile inplace for a corrupt tile.
 
-    @property
-    def scanner_serial_number(self) -> Optional[str]:
-        return self._tags["DICOM_DEVICE_SERIAL_NUMBER"]
+        Parameters
+        ----------
+        tile_point: Point
+            Position of tile to get.
 
-    @cached_property
-    def aquisition_datetime(self) -> Optional[datetime]:
-        if self._tags["DICOM_ACQUISITION_DATETIME"] is None:
-            return None
-        try:
-            return datetime.strptime(
-                self._tags["DICOM_ACQUISITION_DATETIME"], r"%Y%m%d%H%M%S.%f"
-            )
-        except ValueError:
-            return None
-
-    @cached_property
-    def pixel_spacing(self) -> Optional[Tuple[float, float]]:
-        if self._tags["DICOM_PIXEL_SPACING"] is None:
-            return None
-        return tuple(
-            self._split_and_cast_text(self._tags["DICOM_PIXEL_SPACING"], float)[0:2]
-        )
+        Returns
+        ----------
+        bytes:
+            Fixed tile bytes.
 
-    @cached_property
-    def properties(self) -> Dict[str, Any]:
-        properties: Dict[str, Any] = {}
-        if self._tags["DICOM_LOSSY_IMAGE_COMPRESSION_METHOD"] is not None:
-            properties["lossy_image_compression_method"] = self._split_and_cast_text(
-                self._tags["DICOM_LOSSY_IMAGE_COMPRESSION_METHOD"], str
-            )
-        if self._tags["DICOM_LOSSY_IMAGE_COMPRESSION_RATIO"] is not None:
-            properties["lossy_image_compression_ratio"] = self._split_and_cast_text(
-                self._tags["DICOM_LOSSY_IMAGE_COMPRESSION_RATIO"], float
-            )[0]
-        if self._tags["DICOM_BITS_ALLOCATED"] is not None:
-            properties["bits_allocated"] = int(self._tags["DICOM_BITS_ALLOCATED"])
-        if self._tags["DICOM_BITS_STORED"] is not None:
-            properties["bits_stored"] = int(self._tags["DICOM_BITS_STORED"])
-        if self._tags["DICOM_HIGH_BIT"] is not None:
-            properties["high_bit"] = int(self._tags["DICOM_HIGH_BIT"])
-
-        if self._tags["DICOM_PIXEL_REPRESENTATION"] is not None:
-            properties["pixel_representation"] = self._tags[
-                "DICOM_PIXEL_REPRESENTATION"
-            ]
-        return properties
-
-    @staticmethod
-    def _split_and_cast_text(string: str, cast_type: Type[CastType]) -> List[CastType]:
-        return [cast_type(element) for element in string.replace('"', "").split()]
+        """
+        if tile_point not in self._fixed_tiles:
+            fixed_tile = self._get_scaled_tile(tile_point)
+            self._fixed_tiles[tile_point] = fixed_tile
+        return self._fixed_tiles[tile_point]
+
+    def get_tile(self, tile_position: Tuple[int, int]) -> bytes:
+        """Return image bytes for tile at tile position. If tile is marked as
+        corrupt, return a fixed tile. Add color space fix if jpeg compression.
 
+        Parameters
+        ----------
+        tile_position: Tuple[int, int]
+            Tile position to get.
 
-class PhilipsTiffTiler(Tiler):
-    def __init__(
-        self, filepath: Union[str, Path], turbo_path: Optional[Union[str, Path]] = None
-    ):
-        """Tiler for Philips tiff file.
+        Returns
+        ----------
+        bytes
+            Produced tile at position.
+        """
+        tile_point = Point.from_tuple(tile_position)
+        if self._tile_is_corrupt(tile_point):
+            return self._get_fixed_tile(tile_point)
+
+        return super().get_tile(tile_position)
+
+    def get_tiles(self, tile_positions: Sequence[Tuple[int, int]]) -> List[bytes]:
+        """Return list of image bytes for tiles at tile positions.
 
         Parameters
         ----------
-        filepath: Union[str, Path]
-            Filepath to a Philips-TiffFile.
-        turbo_path: Optional[Union[str, Path]] = None
-            Path to turbojpeg (dll or so).
-        """
-        super().__init__(Path(filepath))
-        self._fh = self._tiff_file.filehandle
-
-        self._turbo_path = turbo_path
-        self._jpeg = Jpeg(self._turbo_path)
-
-        self._level_series_index = 0
-        for series_index, series in enumerate(self.series):
-            if self.is_label(series):
-                self._label_series_index = series_index
-            elif self.is_overview(series):
-                self._overview_series_index = series_index
-        self._metadata = PhilipsMetadata(self._tiff_file)
-        assert self._metadata.pixel_spacing is not None
-        self._base_mpp = SizeMm.from_tuple(self._metadata.pixel_spacing) * 1000.0
-        self._pages: Dict[Tuple[int, int, int], PhilipsTiffTiledPage] = {}
+        tile_positions: Sequence[Tuple[int, int]]
+            Tile positions to get.
 
-    @property
-    def metadata(self) -> Metadata:
-        return self._metadata
-
-    @classmethod
-    def supported(cls, tiff_file: TiffFile) -> bool:
-        return tiff_file.is_philips
-
-    def get_page(self, series: int, level: int, page: int = 0) -> PhilipsTiffTiledPage:
-        """Return PhilipsTiffTiledPage for series, level, page."""
-        if not (series, level, page) in self._pages:
-            self._pages[series, level, page] = PhilipsTiffTiledPage(
-                self._get_tiff_page(series, level, page),
-                self._fh,
-                self.base_size,
-                self._base_mpp,
-                self._jpeg,
-            )
-        return self._pages[series, level, page]
-
-    @staticmethod
-    def is_overview(series: TiffPageSeries) -> bool:
-        """Return true if series is a overview series."""
-        page = series.pages[0]
-        assert isinstance(page, TiffPage)
-        return page.description.find("Macro") > -1
-
-    @staticmethod
-    def is_label(series: TiffPageSeries) -> bool:
-        """Return true if series is a label series."""
-        page = series.pages[0]
-        assert isinstance(page, TiffPage)
-        return page.description.find("Label") > -1
-
-    @staticmethod
-    def _get_associated_mpp_from_page(page: TiffPage):
-        """Return mpp (um/pixel) for associated image (label or
-        macro) from page."""
-        pixel_size_start_string = "pixelsize=("
-        pixel_size_start = page.description.find(pixel_size_start_string)
-        pixel_size_end = page.description.find(")", pixel_size_start)
-        pixel_size_string = page.description[
-            pixel_size_start + len(pixel_size_start_string) : pixel_size_end
+        Returns
+        ----------
+        List[bytes]
+            List of tile bytes.
+        """
+        tile_points = [
+            Point.from_tuple(tile_position) for tile_position in tile_positions
         ]
-        pixel_spacing = SizeMm.from_tuple(
-            [float(v) for v in pixel_size_string.replace('"', "").split(",")]
-        )
-        return pixel_spacing / 1000.0
+        if any(self._tile_is_corrupt(tile_point) for tile_point in tile_points):
+            return [self.get_tile(tile) for tile in tile_positions]
+        return super().get_tiles(tile_positions)
+
+    def _tile_is_corrupt(self, tile_point: Point) -> bool:
+        """Return true if tile is corrupt
+
+        Parameters
+        ----------
+        tile_point: Point
+            Tile to check
+
+        Returns
+        ----------
+        bool
+            True if tile is corrupt.
+        """
+        return (
+            self.right_edge_corrupt and self._tile_is_at_right_edge(tile_point)
+        ) or (self.bottom_edge_corrupt and self._tile_is_at_bottom_edge(tile_point))
```

### Comparing `opentile-0.8.1/opentile/svs_tiler.py` & `opentile-0.9.0/opentile/formats/ndpi/ndpi_image.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,96 @@
-#    Copyright 2021 SECTRA AB
+#    Copyright 2021-2023 SECTRA AB
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
-import io
-from datetime import datetime
-from functools import cached_property
-from pathlib import Path
-from typing import Any, Dict, List, Optional, Sequence, Tuple, Union, cast
+"""Image implementations for ndpi files."""
+
+from abc import ABCMeta, abstractmethod
+from functools import cached_property, lru_cache
+from typing import Dict, List, Optional, Sequence, Tuple
 
 import numpy as np
-from PIL import Image
-from tifffile.tifffile import (
-    COMPRESSION,
-    FileHandle,
-    TiffFile,
-    TiffPage,
-    svs_description_metadata,
-)
+from tifffile.tifffile import COMPRESSION, TIFF, TiffPage
 
-from opentile.common import NativeTiledPage, OpenTilePage, Tiler
+from opentile.config import settings
+from opentile.formats.ndpi.ndpi_tile import NdpiFrameJob, NdpiTile
 from opentile.geometry import Point, Region, Size, SizeMm
-from opentile.jpeg import Jpeg
-from opentile.metadata import Metadata
+from opentile.jpeg import Jpeg, JpegCropError
+from opentile.tiff_image import LockableFileHandle
+from opentile.tiler import TiffImage
 
 
-class SvsStripedPage(OpenTilePage):
+class NdpiImage(TiffImage):
     _pyramid_index = 0
 
-    def __init__(self, page: TiffPage, fh: FileHandle, jpeg: Jpeg):
-        """OpenTiledPage for jpeg striped Svs page, e.g. overview page.
+    def __init__(self, page: TiffPage, fh: LockableFileHandle, jpeg: Jpeg):
+        """Ndpi image that should not be tiled (e.g. overview or label).
+        Image data is assumed to be jpeg.
 
         Parameters
         ----------
         page: TiffPage
             TiffPage defining the page.
-        fh: FileHandle
+        fh: LockableFileHandle
             Filehandler to read data from.
         jpeg: Jpeg
             Jpeg instance to use.
-
         """
-        super().__init__(page, fh, True)
+        super().__init__(page, fh)
+        if self.compression != COMPRESSION.JPEG:
+            raise NotImplementedError(
+                f"{self.compression} is unsupported for ndpi "
+                "(Only jpeg is supported)"
+            )
         self._jpeg = jpeg
+        try:
+            # Defined in nm
+            assert isinstance(page.ndpi_tags, dict)
+            self._focal_plane = page.ndpi_tags["ZOffsetFromSlideCenter"] / 1000.0
+        except (KeyError, AssertionError):
+            self._focal_plane = 0.0
+
+        self._mpp = self._get_mpp_from_page()
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({self._page}, {self._fh}, {self._jpeg}"
 
     @property
-    def pixel_spacing(self) -> Optional[SizeMm]:
-        return None
+    def focal_plane(self) -> float:
+        """Return focal plane (in um)."""
+        return self._focal_plane
+
+    @property
+    def pixel_spacing(self) -> SizeMm:
+        """Return pixel spacing in mm per pixel."""
+        return self.mpp / 1000.0
+
+    @property
+    def supported_compressions(self) -> Optional[List[COMPRESSION]]:
+        return [COMPRESSION.JPEG]
+
+    @property
+    def mpp(self) -> SizeMm:
+        """Return pixel spacing in um per pixel."""
+        return self._mpp
+
+    @cached_property
+    def mcu(self) -> Size:
+        """Return mcu size of image."""
+        return self._jpeg.get_mcu(self._read_frame(0))
 
     def get_tile(self, tile_position: Tuple[int, int]) -> bytes:
         """Return tile for tile position.
 
         Parameters
         ----------
         tile_position: Tuple[int, int]
@@ -70,474 +98,546 @@
 
         Returns
         ----------
         bytes
             Produced tile at position.
         """
         if tile_position != (0, 0):
-            raise ValueError("Non-tiled page, expected tile_position (0, 0)")
-        indices = range(len(self.page.dataoffsets))
-        scans = (self._read_frame(index) for index in indices)
-        jpeg_tables = self.page.jpegtables
-        frame = self._jpeg.concatenate_scans(
-            scans, jpeg_tables, self._add_rgb_colorspace_fix
-        )
-        return frame
+            raise ValueError("Non-tiled image, expected tile_position (0, 0)")
+        return self._read_frame(0)
 
     def get_decoded_tile(self, tile_position: Tuple[int, int]) -> np.ndarray:
         """Return decoded tile for tile position.
 
         Parameters
         ----------
         tile_position: Tuple[int, int]
             Tile position to get.
 
         Returns
         ----------
         bytes
             Produced tile at position.
         """
-        return self._jpeg.decode(self.get_tile(tile_position))
+        tile = self.get_tile(tile_position)
+        return self._jpeg.decode(tile)
 
+    def _get_mpp_from_page(self) -> SizeMm:
+        """Return pixel spacing in um/pixel."""
+        x_resolution = self.page.tags["XResolution"].value[0]
+        y_resolution = self.page.tags["YResolution"].value[0]
+        resolution_unit = self.page.tags["ResolutionUnit"].value
+        if resolution_unit != TIFF.RESUNIT.CENTIMETER:
+            raise ValueError("Unknown resolution unit")
+        # 10*1000 um per cm
+        mpp_x = 10 * 1000 / x_resolution
+        mpp_y = 10 * 1000 / y_resolution
+        return SizeMm(mpp_x, mpp_y)
 
-class SvsLZWPage(OpenTilePage):
-    _pyramid_index = 0
 
-    def __init__(self, page: TiffPage, fh: FileHandle, jpeg: Jpeg):
-        """OpenTiledPage for lzw striped Svs page, e.g. label page.
+class NdpiCroppedImage(NdpiImage):
+    def __init__(
+        self,
+        page: TiffPage,
+        fh: LockableFileHandle,
+        jpeg: Jpeg,
+        crop: Tuple[float, float],
+    ):
+        """Ndpi image that should be cropped (e.g. overview or label).
+        Image data is assumed to be jpeg.
 
         Parameters
         ----------
         page: TiffPage
             TiffPage defining the page.
-        fh: FileHandle
+        fh: LockableFileHandle
             Filehandler to read data from.
         jpeg: Jpeg
             Jpeg instance to use.
-
+        crop: Tuple[float, float]
+            Crop start and end in x-direction relative to image width.
         """
-        super().__init__(page, fh)
-        self._jpeg = jpeg
-
-    def __repr__(self) -> str:
-        return f"{type(self).__name__}({self._page}, {self._fh}, {self._jpeg}"
-
-    @property
-    def compression(self) -> COMPRESSION:
-        """Return compression of page."""
-        return COMPRESSION.JPEG
-
-    @property
-    def pixel_spacing(self) -> Optional[SizeMm]:
-        return None
+        super().__init__(page, fh, jpeg)
+        crop_from = self._calculate_crop(crop[0])
+        crop_to = self._calculate_crop(crop[1])
+
+        self._image_size = Size(crop_to - crop_from, self._page.shape[0])
+        self._crop_parameters = (
+            crop_from,
+            0,
+            crop_to - crop_from,
+            self.image_size.height,
+        )
 
     def get_tile(self, tile_position: Tuple[int, int]) -> bytes:
         """Return tile for tile position.
 
         Parameters
         ----------
         tile_position: Tuple[int, int]
             Tile position to get.
 
         Returns
         ----------
         bytes
             Produced tile at position.
         """
-        return self._jpeg.encode(self.get_decoded_tile(tile_position))
+        if tile_position != (0, 0):
+            raise ValueError("Non-tiled image, expected tile_position (0, 0)")
+        full_frame = super().get_tile(tile_position)
+        return self._jpeg.crop_multiple(full_frame, [self._crop_parameters])[0]
 
-    def get_decoded_tile(self, tile_position: Tuple[int, int]) -> np.ndarray:
-        """Return decoded tile for tile position.
+    def _calculate_crop(self, crop: float) -> int:
+        """Return pixel position for crop position rounded down to closest mcu
+        boarder.
 
         Parameters
         ----------
-        tile_position: Tuple[int, int]
-            Tile position to get.
+        crop: float
+            Crop parameter relative to image width.
 
         Returns
         ----------
-        bytes
-            Produced tile at position.
+        int
+            Pixel position for crop.
         """
-        if tile_position != (0, 0):
-            raise ValueError("Non-tiled page, expected tile_position (0, 0)")
-
-        tile = np.concatenate(
-            [self._get_row(index) for index in range(len(self.page.dataoffsets))],
-            axis=1,
-        )
-        return np.squeeze(tile)
-
-    def _get_row(self, index: int) -> np.ndarray:
-        row = self.page.decode(self._read_frame(index), index)[0]
-        assert isinstance(row, np.ndarray)
-        return row
+        width = self._page.shape[1]
+        return int(width * crop / self.mcu.width) * self.mcu.width
 
 
-class SvsTiledPage(NativeTiledPage):
+class NdpiTiledImage(NdpiImage, metaclass=ABCMeta):
     def __init__(
         self,
         page: TiffPage,
-        fh: FileHandle,
-        base_shape: Size,
-        base_mpp: SizeMm,
-        parent: Optional["SvsTiledPage"] = None,
+        fh: LockableFileHandle,
+        base_size: Size,
+        tile_size: Size,
+        jpeg: Jpeg,
     ):
-        """OpenTiledPage for Svs Tiff-page.
+        """Metaclass for a tiled ndpi image.
 
         Parameters
         ----------
         page: TiffPage
             TiffPage defining the page.
-        fh: FileHandle
+        fh: LockableFileHandle
             Filehandler to read data from.
-        base_shape: Size
+        base_size: Size
             Size of base level in pyramid.
-        base_mpp: SizeMm
-            Mpp (um/pixel) for base level in pyramid.
-        parent: Optional['SvsTiledPage'] = None
-            Parent SvsTiledPage
-        """
-        super().__init__(page, fh, True)
-        self._base_shape = base_shape
-        self._base_mpp = base_mpp
-        self._pyramid_index = self._calculate_pyramidal_index(self._base_shape)
-        self._mpp = self._calculate_mpp(self._base_mpp)
-        self._parent = parent
-        (
-            self._right_edge_corrupt,
-            self._bottom_edge_corrupt,
-        ) = self._detect_corrupt_edges()
-        self._fixed_tiles: Dict[Point, bytes] = {}
+        tile_size: Size
+            Requested tile size.
+        jpeg: Jpeg
+            Jpeg instance to use.
+        """
+        super().__init__(page, fh, jpeg)
+        self._base_size = base_size
+        self._tile_size = tile_size
+        self._file_frame_size = self._get_file_frame_size()
+        self._frame_size = Size.max(self.tile_size, self._file_frame_size)
+        self._pyramid_index = self._calculate_pyramidal_index(self._base_size)
+        self._headers: Dict[Size, bytes] = {}
 
     def __repr__(self) -> str:
         return (
             f"{type(self).__name__}({self._page}, {self._fh}, "
-            f"{self._base_shape}, {self._base_mpp})"
+            f"{self._base_size}, {self.tile_size}, {self._jpeg}"
         )
 
     @property
-    def pixel_spacing(self) -> SizeMm:
-        """Return pixel spacing in mm per pixel."""
-        return self.mpp / 1000
+    def suggested_minimum_chunk_size(self) -> int:
+        return max(self._frame_size.width // self._tile_size.width, 1)
 
     @property
-    def mpp(self) -> SizeMm:
-        """Return pixel spacing in um per pixel."""
-        return self._mpp
+    def tile_size(self) -> Size:
+        """The size of the tiles to generate."""
+        return self._tile_size
 
     @property
-    def right_edge_corrupt(self) -> bool:
-        return self._right_edge_corrupt
+    def frame_size(self) -> Size:
+        """The default read size used for reading frames."""
+        return self._frame_size
 
-    @property
-    def bottom_edge_corrupt(self) -> bool:
-        return self._bottom_edge_corrupt
+    @abstractmethod
+    def _read_extended_frame(self, position: Point, frame_size: Size) -> bytes:
+        """Read a frame of size frame_size covering position."""
+        raise NotImplementedError()
+
+    @abstractmethod
+    def _get_file_frame_size(self) -> Size:
+        """Return size of single frame/stripe in file."""
+        raise NotImplementedError()
+
+    @abstractmethod
+    def _get_frame_size_for_tile(self, tile_position: Point) -> Size:
+        """Return frame size used for creating tile at tile position."""
+        raise NotImplementedError()
+
+    def get_tile(self, tile_position: Tuple[int, int]) -> bytes:
+        """Return image bytes for tile at tile position.
 
-    def _detect_corrupt_edge(self, edge: Region) -> bool:
-        """Return true if tiles at edge are corrupt (any tile has a frame
-        that has 0 data length)
         Parameters
         ----------
-        edge: Region
-            Edge to check for corrupt tiles.
+        tile_position: Tuple[int, int]
+            Tile position to get.
 
         Returns
         ----------
-        bool:
-            True if edge contains corrupt tiles.
+        bytes
+            Produced tile at position.
         """
-        for tile in edge.iterate_all():
-            frame_index = self._tile_point_to_frame_index(tile)
-            if self._page.databytecounts[frame_index] == 0:
-                return True
-        return False
+        return self.get_tiles([tile_position])[0]
 
-    def _detect_corrupt_edges(self) -> Tuple[bool, bool]:
-        """Returns tuple bool indiciting if right and/or bottom edge of page is
-        corrupt. Bottom and right edge tiles in svs pyramid levels > 1 can
-        sometimes corrupt. This manifests as tiles with 0-length (easy to
-        detect) and tiles with scrambled image data (not so easy detect).
+    def get_tiles(self, tile_positions: Sequence[Tuple[int, int]]) -> List[bytes]:
+        """Return list of image bytes for tile positions.
 
-        Returns
+        Parameters
         ----------
-        Tuple[bool, bool]:
-            Tuple indicating if right and/or bottom edge is corrupt.
+        tile_positions: Sequence[Tuple[int, int]]
+            Tile positions to get.
 
+        Returns
+        ----------
+        List[bytes]
+            List of tile bytes.
         """
-        if self.pyramid_index == 0:
-            return False, False
-        right_edge = Region(
-            Point(self.tiled_size.width - 1, 0), Size(1, self.tiled_size.height - 1)
-        )
-        right_edge_corrupt = self._detect_corrupt_edge(right_edge)
-
-        bottom_edge = Region(
-            Point(0, self.tiled_size.height - 1), Size(self.tiled_size.width - 1, 1)
-        )
-        bottom_edge_corrupt = self._detect_corrupt_edge(bottom_edge)
+        frame_jobs = self._sort_into_frame_jobs(tile_positions)
+        return [
+            tile
+            for frame_job in frame_jobs
+            for tile in self._create_tiles(frame_job).values()
+        ]
 
-        return right_edge_corrupt, bottom_edge_corrupt
+    def get_decoded_tiles(
+        self, tile_positions: Sequence[Tuple[int, int]]
+    ) -> List[np.ndarray]:
+        """Return list of decoded tiles for tiles at tile positions.
 
-    def _tile_is_at_right_edge(self, tile_point: Point) -> bool:
-        """Return true if tile is at right edge of tiled image."""
-        return tile_point.x == self.tiled_size.width - 1
+        Parameters
+        ----------
+        tile_positions: Sequence[Tuple[int, int]]
+            Tile positions to get.
 
-    def _tile_is_at_bottom_edge(self, tile_point: Point) -> bool:
-        """Return true if tile is at bottom edge of tiled image."""
-        return tile_point.y == self.tiled_size.height - 1
+        Returns
+        ----------
+        List[np.ndarray]
+            List of decoded tiles.
+        """
+        frame_jobs = self._sort_into_frame_jobs(tile_positions)
+        return [
+            self._jpeg.decode(tile)
+            for frame_job in frame_jobs
+            for tile in self._create_tiles(frame_job).values()
+        ]
 
-    def _get_scaled_tile(self, tile_point: Point) -> bytes:
-        """Create a tile by downscaling from a lower (higher resolution)
-        level.
+    def _create_tiles(self, frame_job: NdpiFrameJob) -> Dict[Point, bytes]:
+        """Return tiles defined by frame job. Read frames are cached by
+        frame position.
 
         Parameters
         ----------
-        tile_point: Point
-            Position of tile in this pyramid level.
+        frame_job: NdpiFrameJob
+            Tile job containing tiles that should be created.
 
         Returns
         ----------
-        bytes:
-            Scaled tile bytes.
-
+        Dict[Point, bytes]:
+            Created tiles ordered by tile coordinate.
         """
-        if self._parent is None:
-            raise ValueError("No parent level to get tiles from")
-        scale = int(pow(2, self.pyramid_index - self._parent.pyramid_index))
-        scaled_tile_region = Region(tile_point, Size(1, 1)) * scale
-
-        # Get decoded tiles
-        decoded_tiles = self._parent.get_decoded_tiles(
-            [tile.to_tuple() for tile in scaled_tile_region.iterate_all()]
-        )
-        image_data = np.zeros(
-            (self.tile_size * scale).to_tuple() + (3,), dtype=np.uint8
-        )
-        # Insert decoded_tiles into image_data
-        for y in range(scale):
-            for x in range(scale):
-                image_data_index = y * scale + x
-                image_data[
-                    y * self.tile_size.width : (y + 1) * self.tile_size.width,
-                    x * self.tile_size.height : (x + 1) * self.tile_size.height,
-                ] = decoded_tiles[image_data_index]
-
-        # Resize image_data using Pillow
-        image: Image.Image = Image.fromarray(image_data)
-        image = image.resize(
-            self.tile_size.to_tuple(), resample=Image.Resampling.BILINEAR
-        )
 
-        # Return compressed image
-        if self.compression == COMPRESSION.JPEG:
-            image_format = "jpeg"
-            image_options = {"quality": 95}
-        elif self.compression == COMPRESSION.APERIO_JP2000_RGB:
-            image_format = "jpeg2000"
-            image_options = {"irreversible": True}
-        else:
-            raise NotImplementedError("Not supported compression")
-        with io.BytesIO() as buffer:
-            image.save(buffer, format=image_format, **image_options)
-            frame = buffer.getvalue()
-
-        if self.compression == COMPRESSION.APERIO_JP2000_RGB:
-            # PIL encodes in jp2, find start of j2k and return from there.
-            START_TAGS = bytes([0xFF, 0x4F, 0xFF, 0x51])
-            start_index = frame.find(START_TAGS)
-            return frame[start_index:]
-        return frame
+        frame = self._read_extended_frame(frame_job.position, frame_job.frame_size)
+        tiles = self._crop_to_tiles(frame_job, frame)
+        return tiles
 
-    def _get_fixed_tile(self, tile_point: Point) -> bytes:
-        """Get or create a fixed tile inplace for a corrupt tile.
+    def _crop_to_tiles(
+        self, frame_job: NdpiFrameJob, frame: bytes
+    ) -> Dict[Point, bytes]:
+        """Crop jpeg data to tiles.
 
         Parameters
         ----------
-        tile_point: Point
-            Position of tile to get.
+        frame_job: NdpiFrameJob
+            Frame job defining the tiles to produce by cropping jpeg data.
+        frame: bytes
+            Data to crop from.
 
         Returns
         ----------
-        bytes:
-            Fixed tile bytes.
-
+        Dict[Point, bytes]:
+            Created tiles ordered by tile coordinate.
         """
-        if tile_point not in self._fixed_tiles:
-            fixed_tile = self._get_scaled_tile(tile_point)
-            self._fixed_tiles[tile_point] = fixed_tile
-        return self._fixed_tiles[tile_point]
+        try:
+            tiles: List[bytes] = self._jpeg.crop_multiple(
+                frame, frame_job.crop_parameters
+            )
+        except JpegCropError:
+            raise ValueError(
+                f"Failed to crop at position {frame_job.position} with "
+                f"parameters {frame_job.crop_parameters}. "
+                "This might be due using libjpeg-turbo < 2.1."
+            )
+        return {tile.position: tiles[i] for i, tile in enumerate(frame_job.tiles)}
 
-    def get_tile(self, tile_position: Tuple[int, int]) -> bytes:
-        """Return image bytes for tile at tile position. If tile is marked as
-        corrupt, return a fixed tile. Add color space fix if jpeg compression.
+    def _sort_into_frame_jobs(
+        self, tile_positions: Sequence[Tuple[int, int]]
+    ) -> List[NdpiFrameJob]:
+        """Sorts tile positions into frame jobs (i.e. from the same frame.)
 
         Parameters
         ----------
-        tile_position: Tuple[int, int]
-            Tile position to get.
+        tile_positions: Sequence[Point]
+            List of position to sort.
 
         Returns
         ----------
-        bytes
-            Produced tile at position.
+        List[NdpiFrameJob]
+            List of created frame jobs.
+
         """
-        tile_point = Point.from_tuple(tile_position)
-        if self._tile_is_corrupt(tile_point):
-            return self._get_fixed_tile(tile_point)
+        frame_jobs: Dict[Point, NdpiFrameJob] = {}
+        for tile_position in tile_positions:
+            tile_point = Point.from_tuple(tile_position)
+            if not self._check_if_tile_inside_image(tile_point):
+                raise ValueError(
+                    f"Tile {tile_point} is outside " f"tiled size {self.tiled_size}"
+                )
+            frame_size = self._get_frame_size_for_tile(tile_point)
+            tile = NdpiTile(tile_point, self.tile_size, frame_size)
+            if tile.frame_position in frame_jobs:
+                frame_jobs[tile.frame_position].append(tile)
+            else:
+                frame_jobs[tile.frame_position] = NdpiFrameJob(tile)
+        return list(frame_jobs.values())
 
-        return super().get_tile(tile_position)
 
-    def get_tiles(self, tile_positions: Sequence[Tuple[int, int]]) -> List[bytes]:
-        """Return list of image bytes for tiles at tile positions.
+class NdpiOneFrameImage(NdpiTiledImage):
+    """Class for a ndpi image containing only one frame that should be tiled.
+    The frame can be of any size (smaller or larger than the wanted tile size).
+    The frame is padded to an even multiple of tile size.
+    """
 
-        Parameters
+    def _get_file_frame_size(self) -> Size:
+        """Return size of the single frame in file. For single framed image
+        this is equal to the level size.
+
+        Returns
         ----------
-        tile_positions: Sequence[Tuple[int, int]]
-            Tile positions to get.
+        Size
+            The size of frame in the file.
+        """
+        return self.image_size
+
+    def _get_frame_size_for_tile(self, tile_position: Point) -> Size:
+        """Return read frame size for tile position. For single frame image
+        the read frame size is the image size rounded up to the closest tile
+        size.
 
         Returns
         ----------
-        List[bytes]
-            List of tile bytes.
+        Size
+            The read frame size.
         """
-        tile_points = [
-            Point.from_tuple(tile_position) for tile_position in tile_positions
-        ]
-        if any(self._tile_is_corrupt(tile_point) for tile_point in tile_points):
-            return [self.get_tile(tile) for tile in tile_positions]
-        return super().get_tiles(tile_positions)
+        return ((self.frame_size) // self.tile_size + 1) * self.tile_size
 
-    def _tile_is_corrupt(self, tile_point: Point) -> bool:
-        """Return true if tile is corrupt
+    @lru_cache(settings.ndpi_frame_cache)
+    def _read_extended_frame(self, position: Point, frame_size: Size) -> bytes:
+        """Return padded image covering tile coordinate as valid jpeg bytes.
 
         Parameters
         ----------
-        tile_point: Point
-            Tile to check
+        frame_position: Point
+            Upper left tile position that should be covered by the frame.
+        frame_size: Size
+            Size of the frame to read.
 
         Returns
         ----------
-        bool
-            True if tile is corrupt.
+        bytes
+            Frame
         """
-        return (
-            self.right_edge_corrupt and self._tile_is_at_right_edge(tile_point)
-        ) or (self.bottom_edge_corrupt and self._tile_is_at_bottom_edge(tile_point))
-
+        if position != Point(0, 0):
+            raise ValueError("Frame position not (0, 0) for one frame level.")
+        frame = self._read_frame(0)
+        if (
+            self.image_size.width % self.mcu.width != 0
+            or self.image_size.height % self.mcu.height != 0
+        ):
+            # Extend to whole MCUs
+            even_size = Size.ceil_div(self.image_size, self.mcu) * self.mcu
+            frame = Jpeg.manipulate_header(frame, even_size)
+        # Use crop_multiple as it allows extending frame
+        tile = self._jpeg.crop_multiple(
+            frame, [(0, 0, frame_size.width, frame_size.height)]
+        )[0]
+        return tile
+
+
+class NdpiStripedImage(NdpiTiledImage):
+    """Class for a ndpi image containing stripes. Frames are constructed by
+    concatenating multiple stripes, and from the frame one or more tiles can be
+    produced by lossless cropping.
+    """
 
-class SvsMetadata(Metadata):
-    def __init__(self, page: TiffPage):
-        self._svs_metadata = svs_description_metadata(page.description)
+    def __init__(
+        self,
+        page: TiffPage,
+        fh: LockableFileHandle,
+        base_size: Size,
+        tile_size: Size,
+        jpeg: Jpeg,
+    ):
+        """Ndpi image with striped image data.
 
-    @cached_property
-    def magnification(self) -> Optional[float]:
-        try:
-            return float(self._svs_metadata["AppMag"])
-        except (KeyError, ValueError):
-            return None
+        Parameters
+        ----------
+        page: TiffPage
+            TiffPage defining the page.
+        fh: LockableFileHandle
+            Filehandler to read data from.
+        base_size: Size
+            Size of base level in pyramid.
+        tile_size: Size
+            Requested tile size.
+        jpeg: Jpeg
+            Jpeg instance to use.
+        """
+        super().__init__(page, fh, base_size, tile_size, jpeg)
+        self._striped_size = Size(self.page.chunked[1], self.page.chunked[0])
+        jpeg_header = self.page.jpegheader
+        assert isinstance(jpeg_header, bytes)
+        self._jpeg_header = jpeg_header
 
-    @cached_property
-    def aquisition_datetime(self) -> Optional[datetime]:
-        try:
-            date = datetime.strptime(self._svs_metadata["Date"], r"%m/%d/%y")
-            time = datetime.strptime(self._svs_metadata["Time"], r"%H:%M:%S")
-        except (KeyError, ValueError):
-            return None
-        return datetime.combine(date, time.time())
+    @property
+    def stripe_size(self) -> Size:
+        """Size of stripes."""
+        return self._file_frame_size
 
     @property
-    def mpp(self) -> float:
-        return float(self._svs_metadata["MPP"])
+    def striped_size(self) -> Size:
+        """Number of stripes in columns and rows."""
+        return self._striped_size
 
     @property
-    def image_offset(self) -> Optional[Tuple[float, float]]:
-        return (float(self._svs_metadata["Left"]), float(self._svs_metadata["Top"]))
+    def jpeg_header(self) -> bytes:
+        """Jpeg header in image."""
+        return self._jpeg_header
 
+    def _get_file_frame_size(self) -> Size:
+        """Return size of stripes in file. For striped levels this is parsed
+        from the jpeg header.
 
-class SvsTiler(Tiler):
-    def __init__(
-        self, filepath: Union[str, Path], turbo_path: Optional[Union[str, Path]] = None
-    ):
-        """Tiler for svs file.
+        Returns
+        ----------
+        Size
+            The size of stripes in the file.
+        """
+        stripe_height, stripe_width, _ = self.page.chunks
+        return Size(stripe_width, stripe_height)
+
+    def _is_partial_frame(self, tile_position: Point) -> Tuple[bool, bool]:
+        """Return a tuple of bools, that are true if tile position is at the
+        edge of the image in x or y.
 
         Parameters
         ----------
-        filepath: Union[str, Path]
-            Filepath to a svs TiffFile.
+        tile_position: int
+            Tile position (x or y) to check.
+
+        Returns
+        ----------
+        Tuple[bool, bool]
+            Tuple that is True if tile position x or y is at edge of image.
         """
-        super().__init__(Path(filepath))
-        self._fh = self._tiff_file.filehandle
-        self._turbo_path = turbo_path
-        self._jpeg = Jpeg(self._turbo_path)
-
-        for series_index, series in enumerate(self.series):
-            if series.name == "Baseline":
-                self._level_series_index = series_index
-            elif series.name == "Label":
-                self._label_series_index = series_index
-            elif series.name == "Macro":
-                self._overview_series_index = series_index
-        self._pages: Dict[Tuple[int, int, int], OpenTilePage] = {}
-        if "InterColorProfile" in self._tiff_file.pages.first.tags:
-            icc_profile = self._tiff_file.pages.first.tags["InterColorProfile"].value
-            assert isinstance(icc_profile, bytes) or icc_profile is None
-            self._icc_profile = icc_profile
-        self._metadata = SvsMetadata(self.base_page)
-        self._base_mpp = SizeMm(self._metadata.mpp, self._metadata.mpp)
+        partial_x = (
+            tile_position.x == (self.tiled_size.width - 1)
+            and self.stripe_size.width < self.tile_size.width
+        )
+        partial_y = (
+            tile_position.y == (self.tiled_size.height - 1)
+            and self.stripe_size.height < self.tile_size.height
+        )
+        return partial_x, partial_y
 
-    @property
-    def base_mpp(self) -> SizeMm:
-        """Return pixel spacing in um/pixel for base level."""
-        return self._base_mpp
+    def _get_frame_size_for_tile(self, tile_position: Point) -> Size:
+        """Return frame size used for creating tile at tile position.
+        If tile is an edge tile, ensure that the frame does not extend beyond
+        the image limits.
 
-    @property
-    def metadata(self) -> Metadata:
-        return self._metadata
+        Parameters
+        ----------
+        tile_position: Point
+            Tile position for frame size calculation.
+
+        Returns
+        ----------
+        Size
+            Frame size to be used at tile position.
+        """
+        is_partial_x, is_partial_y = self._is_partial_frame(tile_position)
+        if is_partial_x:
+            width = (
+                self.stripe_size.width * self.striped_size.width
+                - tile_position.x * self.tile_size.width
+            )
+        else:
+            width = self.frame_size.width
 
-    @classmethod
-    def supported(cls, tiff_file: TiffFile) -> bool:
-        return tiff_file.is_svs
-
-    def _get_level_page(self, level: int, page: int = 0) -> SvsTiledPage:
-        series = self._level_series_index
-        if level > 0:
-            parent = self.get_page(series, level - 1, page)
-            parent = cast(SvsTiledPage, parent)
+        if is_partial_y:
+            height = (
+                self.stripe_size.height * self.striped_size.height
+                - tile_position.y * self.tile_size.height
+            )
         else:
-            parent = None
-        svs_page = SvsTiledPage(
-            self._get_tiff_page(series, level, page),
-            self._fh,
-            self.base_size,
-            self.base_mpp,
-            parent,
+            height = self.frame_size.height
+        return Size(width, height)
+
+    @lru_cache(settings.ndpi_frame_cache)
+    def _read_extended_frame(self, position: Point, frame_size: Size) -> bytes:
+        """Return extended frame of frame size starting at frame position.
+        Returned frame is jpeg bytes including header with correct image size.
+        Original restart markers are updated to get the proper incrementation.
+        End of image tag is appended.
+
+        Parameters
+        ----------
+        position: Point
+            Upper left tile position that should be covered by the frame.
+        frame_size: Size
+            Size of the frame to get.
+
+        Returns
+        ----------
+        bytes
+            Concatenated frame as jpeg bytes.
+        """
+        if frame_size in self._headers:
+            header = self._headers[frame_size]
+        else:
+            header = self._jpeg.manipulate_header(self.jpeg_header, frame_size)
+            self._headers[frame_size] = header
+
+        stripe_region = Region(
+            (position * self.tile_size) // self.stripe_size,
+            Size.max(frame_size // self.stripe_size, Size(1, 1)),
         )
-        return svs_page
+        indices = [
+            self._get_stripe_position_to_index(stripe_coordinate)
+            for stripe_coordinate in stripe_region.iterate_all()
+        ]
+        frame = self._jpeg.concatenate_fragments(
+            (self._read_frame(index) for index in indices), header
+        )
+        return frame
 
-    def get_page(self, series: int, level: int, page: int = 0) -> OpenTilePage:
-        """Return SvsTiledPage for series, level, page."""
-        if not (series, level, page) in self._pages:
-
-            if series == self._overview_series_index:
-                svs_page = SvsStripedPage(
-                    self._get_tiff_page(series, level, page), self._fh, self._jpeg
-                )
-            elif series == self._label_series_index:
-                svs_page = SvsLZWPage(
-                    self._get_tiff_page(series, level, page), self._fh, self._jpeg
-                )
-            elif series == self._level_series_index:
-                svs_page = self._get_level_page(level, page)
-            else:
-                raise NotImplementedError()
+    def _get_stripe_position_to_index(self, position: Point) -> int:
+        """Return stripe index from position.
 
-            self._pages[series, level, page] = svs_page
-        return self._pages[series, level, page]
+        Parameters
+        ----------
+        position: Point
+            position of stripe to get index for.
 
-    def _get_properties(self) -> Dict[str, Any]:
-        """Return dictionary with svs properties."""
-        svs_metadata = svs_description_metadata(self.base_page.description)
-        magnification = getattr(svs_metadata, "AppMag", None)
-        return {
-            "magnification": magnification,
-        }
+        Returns
+        ----------
+        int
+            Stripe index.
+        """
+        return position.x + position.y * self.striped_size.width
```

### Comparing `opentile-0.8.1/opentile/turbojpeg_patch.py` & `opentile-0.9.0/opentile/jpeg/turbojpeg_patch.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-#    Copyright 2021 SECTRA AB
+#    Copyright 2021-2023 SECTRA AB
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
+"""Extension of turbojpeg to enable replacing a frame with a constant color using the
+same tables."""
+
 import os
 from ctypes import (
     POINTER,
     Structure,
     _Pointer,
     byref,
     c_int,
@@ -27,26 +30,24 @@
     cdll,
     create_string_buffer,
     memmove,
     pointer,
 )
 from ctypes.util import find_library
 from pathlib import Path
-from struct import calcsize, unpack
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
 from turbojpeg import (
     CUSTOMFILTER,
     TJFLAG_ACCURATEDCT,
     TJXOP_NONE,
     TJXOPT_PERFECT,
     CroppingRegion,
     TurboJPEG,
-    split_byte_into_nibbles,
     tjMCUHeight,
     tjMCUWidth,
 )
 
 
 def find_turbojpeg_path() -> Optional[Path]:
     # Only windows installs libraries on strange places
@@ -91,102 +92,128 @@
         ("op", c_int),
         ("options", c_int),
         ("data", POINTER(BlankStruct)),
         ("customFilter", CUSTOMFILTER),
     ]
 
 
-def get_transform_data(transform_ptr):
-    # Cast the content of the transform pointer into a transform structure
-    transform = cast(transform_ptr, POINTER(BlankTransformStruct)).contents
-    # Cast the content of the callback data pointer in the transform
-    # structure to a background structure
-    return cast(transform.data, POINTER(BlankStruct)).contents
-
-
-def get_np_coeffs(coeffs_ptr, arrayRegion):
-    coeff_array_size = arrayRegion.w * arrayRegion.h
-    # Read the coefficients in the pointer as a np array (no copy)
-    ArrayType = c_short * coeff_array_size
-    array_pointer = cast(coeffs_ptr, POINTER(ArrayType))
-    coeffs = np.frombuffer(array_pointer.contents, dtype=np.int16)
-    coeffs.shape = (arrayRegion.h // 8, arrayRegion.w // 8, 64)
-    return coeffs
-
-
-def blank_image(
-    coeffs_ptr: c_void_p,
-    arrayRegion: CroppingRegion,
-    planeRegion: CroppingRegion,
-    componentID: int,
-    transformID: int,
-    transform_ptr: c_void_p,
-) -> int:
-    """Callback function for filling whole image with background color.
+class BlankImage:
+    _operation = TJXOP_NONE
+    _options = TJXOPT_PERFECT
 
-    Parameters
-    ----------
-    coeffs_ptr: c_void_p
-        Pointer to the coefficient array for the callback.
-    arrayRegion: CroppingRegion
-        The width and height coefficient array and its offset relative to
-        the component plane.
-    planeRegion: CroppingRegion
-        The width and height of the component plane of the coefficient array.
-    componentID: int
-        The component number (i.e. 0, 1, or 2)
-    transformID: int
-        The index of the transformation in the array of transformation given to
-        the transform function.
-    transform_ptr: pointer
-        Pointer to the transform structure used for the transformation.
+    @staticmethod
+    def get_transform_data(transform_ptr: _Pointer) -> BlankStruct:
+        # Cast the content of the transform pointer into a transform structure
+        transform = cast(transform_ptr, POINTER(BlankTransformStruct)).contents
+        # Cast the content of the callback data pointer in the transform
+        # structure to a background structure
+        return cast(transform.data, POINTER(BlankStruct)).contents
 
-    Returns
-    ----------
-    int
-        CFUNCTYPE function must return an int.
-    """
-    background_data = get_transform_data(transform_ptr)
+    @staticmethod
+    def get_np_coeffs(coeffs_ptr: _Pointer, array_region: CroppingRegion) -> np.ndarray:
+        coeff_array_size = array_region.w * array_region.h
+        # Read the coefficients in the pointer as a np array (no copy)
+        array_type = c_short * coeff_array_size
+        array_pointer = cast(coeffs_ptr, POINTER(array_type))
+        coeffs = np.frombuffer(array_pointer.contents, dtype=np.int16)
+        coeffs.shape = (array_region.h // 8, array_region.w // 8, 64)
+        return coeffs
 
-    if componentID == 0:
-        dc_component = background_data.lum
-        subsampling = 0
-    else:
-        dc_component = 0
-        subsampling = background_data.subsample
-    coeffs = get_np_coeffs(coeffs_ptr, arrayRegion)
-    coeffs[:][:][:] = 0
-
-    for x in range(0, arrayRegion.w // tjMCUWidth[subsampling]):
-        for y in range(0, arrayRegion.h // tjMCUHeight[subsampling]):
-            coeffs[y][x][0] = dc_component
+    @classmethod
+    def callback(
+        cls,
+        coeffs_ptr: _Pointer,
+        array_region: CroppingRegion,
+        plane_region: CroppingRegion,
+        component_ID: int,
+        transform_ID: int,
+        transform_ptr: _Pointer,
+    ) -> int:
+        """Callback function for filling whole image with background color.
 
-    return 1
+        Parameters
+        ----------
+        coeffs_ptr: _Pointer
+            Pointer to the coefficient array for the callback.
+        array_region: CroppingRegion
+            The width and height coefficient array and its offset relative to
+            the component plane.
+        plane_region: CroppingRegion
+            The width and height of the component plane of the coefficient
+            array.
+        component_ID: int
+            The component number (i.e. 0, 1, or 2)
+        transform_ID: int
+            The index of the transformation in the array of transformation
+            given to the transform function.
+        transform_ptr: _Pointer
+            Pointer to the transform structure used for the transformation.
+
+        Returns
+        ----------
+        int
+            CFUNCTYPE function must return an int.
+        """
+        background_data = cls.get_transform_data(transform_ptr)
+
+        if component_ID == 0:
+            dc_component = background_data.lum
+            subsampling = 0
+        else:
+            dc_component = 0
+            subsampling = background_data.subsample
+        coeffs = cls.get_np_coeffs(coeffs_ptr, array_region)
+        coeffs[:][:][:] = 0
+
+        for x in range(0, array_region.w // tjMCUWidth[subsampling]):
+            for y in range(0, array_region.h // tjMCUHeight[subsampling]):
+                coeffs[y][x][0] = dc_component
+
+        return 1
+
+    @staticmethod
+    def callback_data(jpeg_subsample: c_int, luminance: int) -> BlankStruct:
+        return BlankStruct(jpeg_subsample, luminance)
+
+    @classmethod
+    def transform(
+        cls,
+        region: CroppingRegion,
+        callback_data: BlankStruct,
+    ) -> BlankTransformStruct:
+        return BlankTransformStruct(
+            region,
+            cls._operation,
+            cls._options,
+            pointer(callback_data),
+            CUSTOMFILTER(cls.callback),
+        )
 
 
 class TurboJPEG_patch(TurboJPEG):
     def __init__(self, lib_turbojpeg_path: Optional[Union[str, Path]] = None):
         if lib_turbojpeg_path is not None:
             lib_turbojpeg_str_path = str(lib_turbojpeg_path)
         else:
             lib_turbojpeg_str_path = str(self._find_turbojpeg())
         super().__init__(lib_turbojpeg_str_path)
         turbo_jpeg = cdll.LoadLibrary(lib_turbojpeg_str_path)
-        self.__transform = turbo_jpeg.tjTransform
-        self.__transform.argtypes = [
+        self.__blank_transform = turbo_jpeg.tjTransform
+        self.__blank_transform.argtypes = [
             c_void_p,
             POINTER(c_ubyte),
             c_ulong,
             c_int,
             POINTER(c_void_p),
             POINTER(c_ulong),
             POINTER(BlankTransformStruct),
             c_int,
         ]
-        self.__transform.restype = c_int
+        self.__blank_transform.restype = c_int
+        self._blank_image_transform = BlankImage()
 
     def fill_image(
         self,
         jpeg_buf: bytes,
         background_luminance: float = 1.0,
     ) -> bytes:
         """Lossless fill jpeg image with background luminance.
@@ -224,38 +251,36 @@
                 byref(jpeg_colorspace),
             )
 
             if decompress_header_status != 0:
                 self._report_error(handle)
 
             # Use callback to fill in background post-transform
-            callback_data = BlankStruct(
+            callback_data = self._blank_image_transform.callback_data(
                 jpeg_subsample,
                 self._map_luminance_to_dc_dct_coefficient(
                     jpeg_buf, background_luminance
                 ),
             )
-            callback = CUSTOMFILTER(blank_image)
-
             # Pointers to output image buffers and buffer size
             dest_array = c_void_p()
             dest_size = c_ulong()
-            region = CroppingRegion(0, 0, image_width, image_height)
-            crop_transform = BlankTransformStruct(
-                region, TJXOP_NONE, TJXOPT_PERFECT, pointer(callback_data), callback
+            transform = self._blank_image_transform.transform(
+                CroppingRegion(0, 0, image_width, image_height),
+                callback_data,
             )
             # Do the transforms
-            transform_status = self.__transform(
+            transform_status = self.__blank_transform(
                 handle,
                 src_addr,
                 jpeg_array.size,
                 1,
                 byref(dest_array),
                 byref(dest_size),
-                byref(crop_transform),
+                byref(transform),
                 TJFLAG_ACCURATEDCT,
             )
 
             # Copy the transform results into python bytes
             dest_buf = create_string_buffer(dest_size.value)
             assert dest_array.value is not None
             memmove(dest_buf, dest_array.value, dest_size.value)
@@ -267,107 +292,21 @@
                 self._report_error(handle)
 
             return dest_buf.raw
 
         finally:
             self._destroy(handle)
 
-    @staticmethod
-    def _find_dqt(jpeg_data: bytes, dqt_index: int) -> Optional[int]:
-        """Return byte offset to quantification table with index dqt_index in
-        jpeg_data.
-
-        Parameters
-        ----------
-        jpeg_data: bytes
-            Jpeg data containing quantification table(s).
-        dqt_index: int
-            Index of quantificatin table to find (0 - luminance).
-
-        Returns
-        ----------
-        Optional[int]
-            Byte offset to quantification table, or None if not found.
-        """
-        offset = 0
-        while offset < len(jpeg_data):
-            dct_table_offset = jpeg_data[offset:].find(bytes([0xFF, 0xDB]))
-            if dct_table_offset == -1:
-                break
-            dct_table_offset += offset
-            dct_table_length = unpack(
-                ">H", jpeg_data[dct_table_offset + 2 : dct_table_offset + 4]
-            )[0]
-            dct_table_id_offset = dct_table_offset + 4
-            table_index, _ = split_byte_into_nibbles(jpeg_data[dct_table_id_offset])
-            if table_index == dqt_index:
-                return dct_table_offset
-            offset += dct_table_offset + dct_table_length
-        return None
-
-    @classmethod
-    def _get_dc_dqt_element(cls, jpeg_data: bytes, dqt_index: int) -> int:
-        """Return dc quantification element from jpeg_data for quantification
-        table dqt_index.
-
-        Parameters
-        ----------
-        jpeg_data: bytes
-            Jpeg data containing quantification table(s).
-        dqt_index: int
-            Index of quantificatin table to get (0 - luminance).
-
-        Returns
-        ----------
-        int
-            Dc quantification element.
-        """
-        dqt_offset = cls._find_dqt(jpeg_data, dqt_index)
-        if dqt_offset is None:
-            raise ValueError(f"Quantisation table {dqt_index} not found in header")
-        precision_offset = dqt_offset + 4
-        precision = split_byte_into_nibbles(jpeg_data[precision_offset])[0]
-        if precision == 0:
-            unpack_type = ">b"
-        elif precision == 1:
-            unpack_type = ">h"
-        else:
-            raise ValueError("Not valid precision definition in dqt")
-        dc_offset = dqt_offset + 5
-        dc_length = calcsize(unpack_type)
-        dc_value: int = unpack(
-            unpack_type, jpeg_data[dc_offset : dc_offset + dc_length]
-        )[0]
-        return dc_value
-
     @classmethod
     def _map_luminance_to_dc_dct_coefficient(
         cls, jpeg_data: bytes, luminance: float
     ) -> int:
-        """Map a luminance level (0 - 1) to quantified dc dct coefficient.
-        Before quantification dct coefficient have a range -1024 - 1023. This
-        is reduced upon quantification by the quantification factor. This
-        function maps the input luminance level range to the quantified dc dct
-        coefficient range.
-
-        Parameters
-        ----------
-        jpeg_data: bytes
-            Jpeg data containing quantification table(s).
-        luminance: float
-            Luminance level (0 - black, 1 - white).
-
-        Returns
-        ----------
-        int
-            Quantified luminance dc dct coefficent.
-        """
-        luminance = min(max(luminance, 0), 1)
-        dc_dqt_coefficient = cls._get_dc_dqt_element(jpeg_data, 0)
-        return round((luminance * 2047 - 1024) / dc_dqt_coefficient)
+        return cls._TurboJPEG__map_luminance_to_dc_dct_coefficient(  # type: ignore # NOQA
+            jpeg_data, luminance
+        )
 
     def _find_turbojpeg(self) -> str:
         return self._TurboJPEG__find_turbojpeg()  # type: ignore
 
     def _init_transform(self) -> c_void_p:
         return self._TurboJPEG__init_transform()  # type: ignore
```

### Comparing `opentile-0.8.1/pyproject.toml` & `opentile-0.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "opentile"
-version = "0.8.1"
+version = "0.9.0"
 description = "Read tiles from wsi-TIFF files"
 authors = ["Erik O Gabrielsson <erik.o.gabrielsson@sectra.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/imi-bigpicture/opentile"
 keywords = ["whole slide image", "digital pathology", "tiff"]
 classifiers = [
@@ -17,14 +17,16 @@
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 tifffile = "^2022.5.4"
 numpy = "^1.22.0"
 PyTurboJPEG = "^1.6.1"
 Pillow = "^9.1.1"
 imagecodecs = "^2022.12.24"
+defusedxml = "^0.7.1"
+ome-types = "^0.3.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 pytest-watch = "^4.2.0"
 pycodestyle = "^2.8.0"
 requests = "^2.28.1"
 flake8 = "^4.0.1"
```

### Comparing `opentile-0.8.1/README.md` & `opentile-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 *opentile* is a Python library for reading tiles from wsi tiff files. The aims of the proect are:
 
 - Allow compressed tiles to be losslessly read from wsi tiffs using 2D coordinates (tile position x, y).
 - Provide unified interface for relevant metadata.
 - Support all file formats supported by tifffile that has a non-overlapping tile structure.
 
-Crrently supported file formats are listed and described under *Supported file formats*.
+*opentile* does `not` provide methods for reading regions from images (e.g. `get_region()`). See [openslide-python](https://github.com/openslide/openslide-python), [tiffslide](https://github.com/bayer-science-for-a-better-life/tiffslide), or [wsidicomizer](https://github.com/imi-bigpicture/wsidicomizer) for such use.
+
+Currently implemented file formats are listed and described under *Implemented file formats*.
 
 ## Installing *opentile*
 
 *opentile* is available on PyPI:
 
 ```console
 pip install opentile
@@ -24,23 +26,23 @@
 
 ## Important note
 
 Please note that this is an early release and the API is not frozen yet. Function names and functionality is prone to change.
 
 ## Requirements
 
-*opentile* requires python >=3.8 and uses numpy, Pillow, TiffFile, and PyTurboJPEG (with lib-turbojpeg >= 2.1 ).
+*opentile* requires python >=3.8 and uses numpy, Pillow, TiffFile, and PyTurboJPEG (with lib-turbojpeg >= 2.1 ), imagecodecs, defusedxml, and ome-types.
 
 ## Limitations
 
 Files with z-stacks are currently not fully supported for all formats.
 
-## Supported file formats
+## Implemented file formats
 
-The following description of the workings of the supported file formats does not include the additional specifics for each format that is handled by tifffile. Additional formats supported by tifffile and that have non-overlapping tile layout are likely to be added in future release.
+The following description of the workings of the implemented file formats does not include the additional specifics for each format that is handled by tifffile. Additional formats supported by tifffile and that have non-overlapping tile layout are likely to be added in future release.
 
 ***Hamamatsu Ndpi***
 The Ndpi-format uses non-rectangular tile size typically 8 pixels high, i.e. stripes. To form tiles, first multiple stripes are concatenated to form a frame covering the tile region. Second, if the stripes are longer than the tile width, the tile is croped out of the frame. The concatenation and crop transformations are performed losslessly.
 
 A ndpi-file can also contain non-tiled images. If these are part of a pyramidal series, *opentile* tiles the image.
 
 The macro page in ndpi-files images the whole slide including label. A label and overview is created by cropping the macro image.
@@ -50,14 +52,17 @@
 
 ***Aperio svs***
 Some Asperio svs-files have corrupt tile data at edges of non-base pyramidal levels. This is observed as tiles with 0-byte length and tiles with incorrect pixel data. *opentile* detects such corruption and instead returns downscaled image data from lower levels. Associated images (label, overview) are currently not handled correctly.
 
 ***3DHistech tiff***
 Only the pyramidal levels are supported (not overviews or labels).
 
+***OME tiff***
+Metadata parsing is not yet implemented.
+
 ## Metadata
 
 File metadata can be accessed through the `metadata`-property of a tiler. Depending on file format and content, the following metadata is avaiable:
 
 - Magnification
 - Scanner manufacturer
 - Scanner model
@@ -143,10 +148,10 @@
 
 We recommend first creating an issue before creating potential contributions to check that the contribution is in line with the goals of the project. To submit your contribution, please issue a pull request on the imi-bigpicture/opentile repository with your changes for review.
 
 Our aim is to provide constructive and positive code reviews for all submissions. The project relies on gradual typing and roughly follows PEP8. However, we are not dogmatic. Most important is that the code is easy to read and understand.
 
 ## Acknowledgement
 
-*opentile*: Copyright 2021 Sectra AB, licensed under Apache 2.0.
+*opentile*: Copyright 2021-2023 Sectra AB, licensed under Apache 2.0.
 
 This project is part of a project that has received funding from the Innovative Medicines Initiative 2 Joint Undertaking under grant agreement No 945358. This Joint Undertaking receives support from the European Union’s Horizon 2020 research and innovation programme and EFPIA. IMI website: www.imi.europa.eu
```

### Comparing `opentile-0.8.1/PKG-INFO` & `opentile-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentile
-Version: 0.8.1
+Version: 0.9.0
 Summary: Read tiles from wsi-TIFF files
 Home-page: https://github.com/imi-bigpicture/opentile
 License: Apache-2.0
 Keywords: whole slide image,digital pathology,tiff
 Author: Erik O Gabrielsson
 Author-email: erik.o.gabrielsson@sectra.com
 Requires-Python: >=3.8,<3.12
@@ -16,29 +16,33 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.1.1,<10.0.0)
 Requires-Dist: PyTurboJPEG (>=1.6.1,<2.0.0)
+Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: imagecodecs (>=2022.12.24,<2023.0.0)
 Requires-Dist: numpy (>=1.22.0,<2.0.0)
+Requires-Dist: ome-types (>=0.3.1,<0.4.0)
 Requires-Dist: tifffile (>=2022.5.4,<2023.0.0)
 Project-URL: Repository, https://github.com/imi-bigpicture/opentile
 Description-Content-Type: text/markdown
 
 # *opentile*
 
 *opentile* is a Python library for reading tiles from wsi tiff files. The aims of the proect are:
 
 - Allow compressed tiles to be losslessly read from wsi tiffs using 2D coordinates (tile position x, y).
 - Provide unified interface for relevant metadata.
 - Support all file formats supported by tifffile that has a non-overlapping tile structure.
 
-Crrently supported file formats are listed and described under *Supported file formats*.
+*opentile* does `not` provide methods for reading regions from images (e.g. `get_region()`). See [openslide-python](https://github.com/openslide/openslide-python), [tiffslide](https://github.com/bayer-science-for-a-better-life/tiffslide), or [wsidicomizer](https://github.com/imi-bigpicture/wsidicomizer) for such use.
+
+Currently implemented file formats are listed and described under *Implemented file formats*.
 
 ## Installing *opentile*
 
 *opentile* is available on PyPI:
 
 ```console
 pip install opentile
@@ -52,23 +56,23 @@
 
 ## Important note
 
 Please note that this is an early release and the API is not frozen yet. Function names and functionality is prone to change.
 
 ## Requirements
 
-*opentile* requires python >=3.8 and uses numpy, Pillow, TiffFile, and PyTurboJPEG (with lib-turbojpeg >= 2.1 ).
+*opentile* requires python >=3.8 and uses numpy, Pillow, TiffFile, and PyTurboJPEG (with lib-turbojpeg >= 2.1 ), imagecodecs, defusedxml, and ome-types.
 
 ## Limitations
 
 Files with z-stacks are currently not fully supported for all formats.
 
-## Supported file formats
+## Implemented file formats
 
-The following description of the workings of the supported file formats does not include the additional specifics for each format that is handled by tifffile. Additional formats supported by tifffile and that have non-overlapping tile layout are likely to be added in future release.
+The following description of the workings of the implemented file formats does not include the additional specifics for each format that is handled by tifffile. Additional formats supported by tifffile and that have non-overlapping tile layout are likely to be added in future release.
 
 ***Hamamatsu Ndpi***
 The Ndpi-format uses non-rectangular tile size typically 8 pixels high, i.e. stripes. To form tiles, first multiple stripes are concatenated to form a frame covering the tile region. Second, if the stripes are longer than the tile width, the tile is croped out of the frame. The concatenation and crop transformations are performed losslessly.
 
 A ndpi-file can also contain non-tiled images. If these are part of a pyramidal series, *opentile* tiles the image.
 
 The macro page in ndpi-files images the whole slide including label. A label and overview is created by cropping the macro image.
@@ -78,14 +82,17 @@
 
 ***Aperio svs***
 Some Asperio svs-files have corrupt tile data at edges of non-base pyramidal levels. This is observed as tiles with 0-byte length and tiles with incorrect pixel data. *opentile* detects such corruption and instead returns downscaled image data from lower levels. Associated images (label, overview) are currently not handled correctly.
 
 ***3DHistech tiff***
 Only the pyramidal levels are supported (not overviews or labels).
 
+***OME tiff***
+Metadata parsing is not yet implemented.
+
 ## Metadata
 
 File metadata can be accessed through the `metadata`-property of a tiler. Depending on file format and content, the following metadata is avaiable:
 
 - Magnification
 - Scanner manufacturer
 - Scanner model
@@ -171,11 +178,11 @@
 
 We recommend first creating an issue before creating potential contributions to check that the contribution is in line with the goals of the project. To submit your contribution, please issue a pull request on the imi-bigpicture/opentile repository with your changes for review.
 
 Our aim is to provide constructive and positive code reviews for all submissions. The project relies on gradual typing and roughly follows PEP8. However, we are not dogmatic. Most important is that the code is easy to read and understand.
 
 ## Acknowledgement
 
-*opentile*: Copyright 2021 Sectra AB, licensed under Apache 2.0.
+*opentile*: Copyright 2021-2023 Sectra AB, licensed under Apache 2.0.
 
 This project is part of a project that has received funding from the Innovative Medicines Initiative 2 Joint Undertaking under grant agreement No 945358. This Joint Undertaking receives support from the European Union’s Horizon 2020 research and innovation programme and EFPIA. IMI website: www.imi.europa.eu
```

