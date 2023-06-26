# Comparing `tmp/citation_utils-0.4.2.tar.gz` & `tmp/citation_utils-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_utils-0.4.2.tar", max compression
+gzip compressed data, was "citation_utils-0.4.3.tar", max compression
```

## Comparing `citation_utils-0.4.2.tar` & `citation_utils-0.4.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1491 2023-06-23 10:27:21.228309 citation_utils-0.4.2/LICENSE
--rw-r--r--   0        0        0      653 2023-06-25 09:54:14.887730 citation_utils-0.4.2/citation_utils/__init__.py
--rw-r--r--   0        0        0    17311 2023-06-25 10:40:38.517021 citation_utils-0.4.2/citation_utils/citation.py
--rw-r--r--   0        0        0     1179 2023-06-25 09:54:14.891749 citation_utils-0.4.2/citation_utils/dockets/__init__.py
--rw-r--r--   0        0        0     3155 2023-06-25 09:54:14.895013 citation_utils-0.4.2/citation_utils/dockets/constructed_ac.py
--rw-r--r--   0        0        0     3194 2023-06-25 09:54:14.895319 citation_utils-0.4.2/citation_utils/dockets/constructed_am.py
--rw-r--r--   0        0        0     2457 2023-06-25 09:54:14.895608 citation_utils-0.4.2/citation_utils/dockets/constructed_bm.py
--rw-r--r--   0        0        0     2893 2023-06-25 09:54:14.895906 citation_utils-0.4.2/citation_utils/dockets/constructed_gr.py
--rw-r--r--   0        0        0     2094 2023-06-25 09:54:14.896184 citation_utils-0.4.2/citation_utils/dockets/constructed_jib.py
--rw-r--r--   0        0        0     2385 2023-06-25 09:54:14.896448 citation_utils-0.4.2/citation_utils/dockets/constructed_oca.py
--rw-r--r--   0        0        0     1597 2023-06-25 09:54:14.896710 citation_utils-0.4.2/citation_utils/dockets/constructed_pet.py
--rw-r--r--   0        0        0     1767 2023-06-25 09:54:14.896999 citation_utils-0.4.2/citation_utils/dockets/constructed_udk.py
--rw-r--r--   0        0        0      364 2023-06-25 10:00:40.543092 citation_utils-0.4.2/citation_utils/dockets/models/__init__.py
--rw-r--r--   0        0        0     4834 2023-06-25 09:54:14.900031 citation_utils-0.4.2/citation_utils/dockets/models/constructor.py
--rw-r--r--   0        0        0     1373 2023-06-25 09:54:14.900293 citation_utils-0.4.2/citation_utils/dockets/models/docket_category.py
--rw-r--r--   0        0        0     1696 2023-06-25 09:54:14.900588 citation_utils-0.4.2/citation_utils/dockets/models/docket_citation.py
--rw-r--r--   0        0        0     4486 2023-06-25 10:27:22.297426 citation_utils-0.4.2/citation_utils/dockets/models/docket_model.py
--rw-r--r--   0        0        0     1419 2023-06-25 09:54:14.901088 citation_utils-0.4.2/citation_utils/dockets/models/docket_rules.py
--rw-r--r--   0        0        0     2911 2023-06-25 09:54:14.901368 citation_utils-0.4.2/citation_utils/dockets/models/gr_clean.py
--rw-r--r--   0        0        0       81 2023-06-25 09:54:14.902014 citation_utils-0.4.2/citation_utils/dockets/models/misc/__init__.py
--rw-r--r--   0        0        0      746 2023-06-25 09:54:14.903593 citation_utils-0.4.2/citation_utils/dockets/models/misc/extra.py
--rw-r--r--   0        0        0     1514 2023-06-25 09:54:14.903861 citation_utils-0.4.2/citation_utils/dockets/models/misc/num.py
--rw-r--r--   0        0        0      242 2023-06-25 09:54:14.904129 citation_utils-0.4.2/citation_utils/dockets/models/misc/x.py
--rw-r--r--   0        0        0     5760 2023-06-25 09:54:14.904387 citation_utils-0.4.2/citation_utils/document.py
--rw-r--r--   0        0        0     2531 2023-06-25 09:54:14.904670 citation_utils-0.4.2/citation_utils/special.py
--rw-r--r--   0        0        0     1312 2023-06-25 10:30:31.798804 citation_utils-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 citation_utils-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-23 10:27:21.228309 citation_utils-0.4.3/LICENSE
+-rw-r--r--   0        0        0      653 2023-06-25 09:54:14.887730 citation_utils-0.4.3/citation_utils/__init__.py
+-rw-r--r--   0        0        0    16831 2023-06-26 01:44:57.939840 citation_utils-0.4.3/citation_utils/citation.py
+-rw-r--r--   0        0        0     1179 2023-06-25 09:54:14.891749 citation_utils-0.4.3/citation_utils/dockets/__init__.py
+-rw-r--r--   0        0        0     3155 2023-06-25 09:54:14.895013 citation_utils-0.4.3/citation_utils/dockets/constructed_ac.py
+-rw-r--r--   0        0        0     3194 2023-06-25 09:54:14.895319 citation_utils-0.4.3/citation_utils/dockets/constructed_am.py
+-rw-r--r--   0        0        0     2457 2023-06-25 09:54:14.895608 citation_utils-0.4.3/citation_utils/dockets/constructed_bm.py
+-rw-r--r--   0        0        0     2893 2023-06-25 09:54:14.895906 citation_utils-0.4.3/citation_utils/dockets/constructed_gr.py
+-rw-r--r--   0        0        0     2094 2023-06-25 09:54:14.896184 citation_utils-0.4.3/citation_utils/dockets/constructed_jib.py
+-rw-r--r--   0        0        0     2385 2023-06-25 09:54:14.896448 citation_utils-0.4.3/citation_utils/dockets/constructed_oca.py
+-rw-r--r--   0        0        0     1597 2023-06-25 09:54:14.896710 citation_utils-0.4.3/citation_utils/dockets/constructed_pet.py
+-rw-r--r--   0        0        0     1767 2023-06-25 09:54:14.896999 citation_utils-0.4.3/citation_utils/dockets/constructed_udk.py
+-rw-r--r--   0        0        0      364 2023-06-25 10:00:40.543092 citation_utils-0.4.3/citation_utils/dockets/models/__init__.py
+-rw-r--r--   0        0        0     4834 2023-06-25 09:54:14.900031 citation_utils-0.4.3/citation_utils/dockets/models/constructor.py
+-rw-r--r--   0        0        0     1373 2023-06-25 09:54:14.900293 citation_utils-0.4.3/citation_utils/dockets/models/docket_category.py
+-rw-r--r--   0        0        0     1696 2023-06-25 09:54:14.900588 citation_utils-0.4.3/citation_utils/dockets/models/docket_citation.py
+-rw-r--r--   0        0        0     5272 2023-06-26 01:40:40.533138 citation_utils-0.4.3/citation_utils/dockets/models/docket_model.py
+-rw-r--r--   0        0        0     1419 2023-06-25 09:54:14.901088 citation_utils-0.4.3/citation_utils/dockets/models/docket_rules.py
+-rw-r--r--   0        0        0     2911 2023-06-25 09:54:14.901368 citation_utils-0.4.3/citation_utils/dockets/models/gr_clean.py
+-rw-r--r--   0        0        0       81 2023-06-25 09:54:14.902014 citation_utils-0.4.3/citation_utils/dockets/models/misc/__init__.py
+-rw-r--r--   0        0        0      746 2023-06-25 09:54:14.903593 citation_utils-0.4.3/citation_utils/dockets/models/misc/extra.py
+-rw-r--r--   0        0        0     1514 2023-06-25 09:54:14.903861 citation_utils-0.4.3/citation_utils/dockets/models/misc/num.py
+-rw-r--r--   0        0        0      242 2023-06-25 09:54:14.904129 citation_utils-0.4.3/citation_utils/dockets/models/misc/x.py
+-rw-r--r--   0        0        0     5760 2023-06-25 09:54:14.904387 citation_utils-0.4.3/citation_utils/document.py
+-rw-r--r--   0        0        0     2531 2023-06-25 09:54:14.904670 citation_utils-0.4.3/citation_utils/special.py
+-rw-r--r--   0        0        0     1312 2023-06-26 01:48:45.055874 citation_utils-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 citation_utils-0.4.3/PKG-INFO
```

### Comparing `citation_utils-0.4.2/LICENSE` & `citation_utils-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.2/citation_utils/__init__.py` & `citation_utils-0.4.3/citation_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.2/citation_utils/citation.py` & `citation_utils-0.4.3/citation_utils/citation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import datetime
 import logging
 from collections.abc import Iterator
+from functools import cached_property
 from typing import Self
 
+from citation_date import DOCKET_DATE_FORMAT
 from citation_report import Report
 from citation_report.main import is_eq
-from pydantic import BaseModel, ConfigDict, Field
+from dateutil.parser import parse
+from pydantic import BaseModel, ConfigDict, Field, field_serializer, model_serializer
 
 from .dockets import Docket, DocketCategory
 from .document import CitableDocument
 
 
 class Citation(BaseModel):
     """
@@ -41,66 +44,175 @@
     None | `offg` | optional (str) | combined `volume` O.G. `page`
     """  # noqa: E501
 
     model_config = ConfigDict(use_enum_values=True, str_strip_whitespace=True)
     docket_category: DocketCategory | None = Field(default=None)
     docket_serial: str | None = Field(default=None)
     docket_date: datetime.date | None = Field(default=None)
-    docket: str | None = Field(
-        default=None, description="Category + single serial id + date"
-    )
-    phil: str | None = Field(default=None, description="vol + Phil. (pub) + page")
-    scra: str | None = Field(default=None, description="vol + SCRA (pub) + page")
-    offg: str | None = Field(default=None, description="vol + O.G. (pub) + page")
-
-    @property
-    def elements(self) -> list[str]:
-        bits = []
-        if self.docket:
-            bits.append(self.docket)
+    phil: str | None = Field(default=None)
+    scra: str | None = Field(default=None)
+    offg: str | None = Field(default=None)
+
+    @cached_property
+    def bits(self) -> list[str]:
+        _bits = []
+        if docket := self.get_docket_display():
+            _bits.append(docket)
         if self.phil:
-            bits.append(self.phil)
+            _bits.append(self.phil)
         if self.scra:
-            bits.append(self.scra)
+            _bits.append(self.scra)
         if self.offg:
-            bits.append(self.offg)
-        return bits
+            _bits.append(self.offg)
+        return _bits
 
     def __repr__(self) -> str:
         return f"<Citation: {str(self)}>"
 
     def __str__(self) -> str:
-        return ", ".join(self.elements) if self.elements else "Bad citation."
+        return ", ".join(self.bits) if self.bits else "Bad citation."
 
     def __eq__(self, other: Self) -> bool:
-        """Relevant to determine `seen` value in `CountedCitation`."""
+        """Helps `seen` variable in `CountedCitation`."""
         ok_cat = self.docket_category is not None and other.docket_category is not None
         ok_serial = self.docket_serial is not None and other.docket_serial is not None
         ok_date = self.docket_date is not None and other.docket_date is not None
         return any(
             [
-                is_eq(self.docket, other.docket),
                 is_eq(self.scra, other.scra),
                 is_eq(self.offg, other.offg),
                 is_eq(self.phil, other.phil),
                 all(
                     [
                         ok_cat and (self.docket_category == other.docket_category),
                         ok_serial and (self.docket_serial == other.docket_serial),
                         ok_date and (self.docket_date == other.docket_date),
                     ]
                 ),
             ]
         )
 
+    @field_serializer("docket_date")
+    def serialize_dt(self, dt: datetime.date | None = None):
+        if dt:
+            return dt.isoformat()
+
+    @field_serializer("docket_serial")
+    def serialize_num(self, num: str | None = None):
+        if num:
+            return Docket.clean_serial(num)
+
+    @field_serializer("docket_category")
+    def serialize_cat(self, cat: DocketCategory | None = None):
+        if cat:
+            return cat.name.lower()
+
+    @field_serializer("phil")
+    def serialize_phil(self, phil: str | None = None):
+        if phil:
+            return phil.lower()
+
+    @field_serializer("scra")
+    def serialize_scra(self, scra: str | None = None):
+        if scra:
+            return scra.lower()
+
+    @field_serializer("offg")
+    def serialize_offg(self, offg: str | None = None):
+        if offg:
+            return offg.lower()
+
+    @model_serializer
+    def ser_model(self) -> dict[str, str | datetime.date | None]:
+        """Generate a database row-friendly format of the model. Note the different
+        field names: `cat`, `num`, `dt`, `phil`, `scra`, `offg` map to either a usable
+        database value or `None`. The docket values here have the option to be `None`
+        since some citations, especially the legacy variants, do not include their
+        docket equivalents in the source texts."""
+        return {
+            "cat": self.serialize_cat(self.docket_category),
+            "num": self.serialize_num(self.docket_serial),
+            "date": self.serialize_dt(self.docket_date),
+            "phil": self.serialize_phil(self.phil),
+            "scra": self.serialize_scra(self.scra),
+            "offg": self.serialize_offg(self.offg),
+        }
+
+    def get_db_id(self) -> str | None:
+        """Value created usable unique identifier of a decision."""
+        bits = [
+            self.serialize_cat(self.docket_category),
+            self.serialize_num(self.docket_serial),
+            self.serialize_dt(self.docket_date),
+        ]
+        if all(bits):
+            return "-".join(bits)  # type: ignore
+        return None
+
+    def make_docket_row(self):
+        """This presumes that a valid docket exists. Although a citation can
+        be a non-docket, e.g. phil, scra, etc., for purposes of creating a
+        a route-based row for a prospective decision object, the identifier will be
+        based on a docket id."""
+        if id := self.get_db_id():
+            return self.model_dump() | {"id": id}
+        logging.error(f"Undocketable: {self=}")
+        return None
+
+    @classmethod
+    def from_docket_row(
+        cls,
+        cat: str,
+        num: str,
+        date: str,
+        opt_phil: str | None,
+        opt_scra: str | None,
+        opt_offg: str | None,
+    ):
+        return cls(
+            docket_category=DocketCategory[cat.upper()],
+            docket_serial=num,
+            docket_date=parse(date).date(),
+            phil=cls.get_report(opt_phil),
+            scra=cls.get_report(opt_scra),
+            offg=cls.get_report(opt_offg),
+        )
+
+    @cached_property
+    def is_docket(self) -> bool:
+        return all([self.docket_category, self.docket_serial, self.docket_date])
+
+    @cached_property
+    def display_date(self):
+        if self.docket_date:
+            return self.docket_date.strftime(DOCKET_DATE_FORMAT)
+        return None
+
+    def get_docket_display(self) -> str | None:
+        if self.is_docket:
+            return f"{self.docket_category} No. {self.docket_serial}, {self.display_date}"  # type: ignore # noqa: E501
+        return None
+
     @classmethod
-    def get_report(cls, publisher: str, data: dict):
-        if publisher not in ("phil", "scra", "offg"):
-            raise Exception(f"Invalid {publisher=}")
-        raw = data.get(publisher)
+    def get_report(cls, raw: str | None = None) -> str | None:
+        """Get a lower cased volpubpage of `publisher` from the `data`. Assumes
+        that the publisher key is either `phil`, `scra` or `offg`.
+
+        Examples:
+            >>> raw = "123 Phil. 123"
+            >>> Citation.get_report(raw)
+            '123 phil. 123'
+
+        Args:
+            publisher (str): _description_
+            data (dict): _description_
+
+        Returns:
+            str | None: _description_
+        """
         if not raw:
             return None
 
         try:
             reports = Report.extract_reports(raw)
             report = next(reports)
             if result := report.volpubpage:
@@ -109,56 +221,33 @@
                 logging.warning(f"No volpubpage {raw=}")
                 return None
         except StopIteration:
             logging.warning(f"No {raw=} report")
             return None
 
     @classmethod
-    def from_data(cls, data: dict):
-        """Presumes data with keys: `cat`, `num`, and `date`"""
-        d = Docket.from_data(data)
-        return cls(
-            docket=str(d) if d else None,
-            docket_category=data.get("cat"),
-            docket_serial=data.get("num"),
-            docket_date=data.get("date"),
-            phil=cls.get_report("phil", data),
-            scra=cls.get_report("scra", data),
-            offg=cls.get_report("offg", data),
-        )
-
-    @classmethod
     def _set_report(cls, text: str):
         try:
             obj = next(Report.extract_reports(text))
-            return cls(
-                docket=None,
-                docket_category=None,
-                docket_serial=None,
-                docket_date=None,
-                phil=obj.phil.lower() if obj.phil else None,
-                scra=obj.scra.lower() if obj.scra else None,
-                offg=obj.offg.lower() if obj.offg else None,
-            )
+            return cls(phil=obj.phil, scra=obj.scra, offg=obj.offg)
         except StopIteration:
             logging.debug(f"{text} is not a Report instance.")
             return None
 
     @classmethod
     def _set_docket_report(cls, text: str):
         try:
             obj = next(CitableDocument.get_docketed_reports(text))
             return cls(
-                docket=f"{obj.category} {obj.serial_text}, {obj.docket_date}",
                 docket_category=obj.category,
                 docket_serial=obj.serial_text,
                 docket_date=obj.docket_date,
-                phil=obj.phil.lower() if obj.phil else None,
-                scra=obj.scra.lower() if obj.scra else None,
-                offg=obj.offg.lower() if obj.offg else None,
+                phil=obj.phil,
+                scra=obj.scra,
+                offg=obj.offg,
             )
         except StopIteration:
             logging.debug(f"{text} is not a Docket nor a Report instance.")
             return None
 
     @classmethod
     def extract_citations(cls, text: str) -> Iterator[Self]:
@@ -192,114 +281,27 @@
     def extract_citation(cls, text: str) -> Self | None:
         """Thin wrapper over `cls.extract_citations()`.
 
         Examples:
             >>> Citation.extract_citation('Hello World') is None
             True
             >>> next(Citation.extract_citations('12 Phil. 24'))
-            <Citation: 12 phil. 24>
+            <Citation: 12 Phil. 24>
 
         Args:
             text (str): Text to evaluate
 
         Returns:
             Self | None: First item found from `extract_citations`, if it exists.
         """
         try:
             return next(cls.extract_citations(text))
         except StopIteration:
             return None
 
-    @property
-    def db_phil(self):
-        if self.phil:
-            return self.phil.lower()
-        return None
-
-    @property
-    def db_scra(self):
-        if self.scra:
-            return self.scra.lower()
-        return None
-
-    @property
-    def db_offg(self):
-        if self.offg:
-            return self.offg.lower()
-        return None
-
-    @property
-    def db_cat(self) -> str | None:
-        """Should not be more than 3 characters."""
-        if self.docket_category:
-            return self.docket_category.name.lower()
-        return None
-
-    @property
-    def db_num(self) -> str | None:
-        """Needs to be alpha-numeric characters with a dash."""
-        if self.docket_serial:
-            candidate = self.docket_serial.lower()
-            if not Docket.check_serial_num(candidate):
-                logging.error(f"Invalid {candidate=}")
-                return None
-            return self.docket_serial.lower()
-        return None
-
-    @property
-    def db_date(self) -> str | None:
-        """Uses the ISO format of the date in the database."""
-        if self.docket_date:
-            return self.docket_date.isoformat()
-        return None
-
-    @property
-    def display_date(self):
-        if self.docket_date:
-            return self.docket_date.strftime("%b %d, %Y")
-        return None
-
-    def get_db_id(self) -> str | None:
-        """The value created can be used as the unique identifier of a decision."""
-        bits = [self.db_cat, self.db_num, self.db_date]
-        if all(bits):
-            return "-".join(bits)  # type: ignore
-        return None
-
-    def get_docket_display(self) -> str | None:
-        if self.get_db_id():
-            return f"{self.docket_category} No. {self.docket_serial}, {self.display_date}"  # type: ignore # noqa: E501
-        return None
-
-    @property
-    def db_row(self) -> dict:
-        """Generate a database row-friendly format of the model. Note the different
-        field names: `cat`, `num`, `dt`, `phil`, `scra`, `offg` map to either a usable
-        database value or `None`. The docket values here have the option to be `None`
-        since some citations, especially the legacy variants, do not include their
-        docket equivalents in the source texts."""
-        return {
-            "cat": self.db_cat,
-            "num": self.db_num,
-            "date": self.db_date,
-            "phil": self.db_phil,
-            "scra": self.db_scra,
-            "offg": self.db_offg,
-        }
-
-    def make_docket_row(self):
-        """This presumes that a valid docket exists. Although a citation can
-        be a non-docket, e.g. phil, scra, etc., for purposes of creating a
-        a route-based row for a prospective decision object, the identifier will be
-        based on a docket id."""
-        if id := self.get_db_id():
-            return self.db_row | {"id": id}
-        logging.error(f"Undocketable: {self=}")
-        return None
-
 
 class CountedCitation(Citation):
     mentions: int = Field(default=1, description="Get count via Citation __eq__")
 
     def __repr__(self) -> str:
         return f"{str(self)}: {self.mentions}"
 
@@ -318,16 +320,16 @@
     def from_source(cls, text: str) -> list[Self]:
         """Computes mentions of `counted_dockets()` vis-a-vis `counted_reports()` and
         count the number of unique items, taking into account the Citation
         structure and the use of __eq__ re: what is considered unique.
 
         Examples:
             >>> source = "374 Phil. 1, 10-11 (1999) 1111 SCRA 1111; G.R. No. 147033, April 30, 2003; G.R. No. 147033, April 30, 2003, 374 Phil. 1, 600; ABC v. XYZ, G.R. Nos. 138570, 138572, 138587, 138680, 138698, October 10, 2000, 342 SCRA 449;  XXX, G.R. No. 31711, Sept. 30, 1971, 35 SCRA 190; Hello World, 1111 SCRA 1111; Y v. Z, 35 SCRA 190; 1 Off. Gaz. 41 Bar Matter No. 803, Jan. 1, 2000 Bar Matter No. 411, Feb. 1, 2000 Bar Matter No. 412, Jan. 1, 2000, 1111 SCRA 1111; 374 Phil. 1"
-            >>> list(CountedCitation.from_source(source))
-            [BM No. 412, Jan 01, 2000, 1111 SCRA 1111: 3, GR No. 147033, Apr 30, 2003, 374 Phil. 1: 3, GR No. 138570, Oct 10, 2000, 342 SCRA 449: 1, GR No. 31711, Sep 30, 1971, 35 SCRA 190: 2, 1 Off. Gaz. 41: 1]
+            >>> len(CountedCitation.from_source(source))
+            6
 
         Args:
             text (str): Text to Evaluate.
 
         Returns:
             list[Self]: Unique citations with their counts.
         """  # noqa: E501
@@ -378,15 +380,14 @@
         a `seen` list. This will also populate the the unique records with missing
         values.
         """
         seen: list[cls] = []
         reports = Report.extract_reports(text=text)
         for report in reports:
             cite = Citation(
-                docket=None,
                 docket_category=None,
                 docket_serial=None,
                 docket_date=None,
                 phil=report.phil,
                 scra=report.scra,
                 offg=report.offg,
             )
@@ -404,15 +405,14 @@
         a `seen` list. This will also populate the the unique records with missing
         values.
         """
 
         seen: list[cls] = []
         for obj in CitableDocument.get_docketed_reports(text=text):
             cite = Citation(
-                docket=str(obj),
                 docket_category=obj.category,
                 docket_serial=obj.serial_text,
                 docket_date=obj.docket_date,
                 phil=obj.phil,
                 scra=obj.scra,
                 offg=obj.offg,
             )
@@ -430,17 +430,14 @@
 
         if not self.docket_serial and other.docket_serial:
             self.docket_serial = other.docket_serial
 
         if not self.docket_date and other.docket_date:
             self.docket_date = other.docket_date
 
-        if not self.docket and other.docket:
-            self.docket = other.docket
-
         if not self.scra and other.scra:
             self.scra = other.scra
 
         if not self.phil and other.phil:
             self.phil = other.phil
 
         if not self.offg and other.offg:
```

### Comparing `citation_utils-0.4.2/citation_utils/dockets/__init__.py` & `citation_utils-0.4.3/citation_utils/dockets/__init__.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.2/citation_utils/dockets/constructed_ac.py` & `citation_utils-0.4.3/citation_utils/dockets/constructed_ac.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.2/citation_utils/dockets/constructed_am.py` & `citation_utils-0.4.3/citation_utils/dockets/constructed_am.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.2/citation_utils/dockets/constructed_bm.py` & `citation_utils-0.4.3/citation_utils/dockets/constructed_bm.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.2/citation_utils/dockets/constructed_gr.py` & `citation_utils-0.4.3/citation_utils/dockets/constructed_gr.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.2/citation_utils/dockets/constructed_jib.py` & `citation_utils-0.4.3/citation_utils/dockets/constructed_jib.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.2/citation_utils/dockets/constructed_oca.py` & `citation_utils-0.4.3/citation_utils/dockets/constructed_oca.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.2/citation_utils/dockets/constructed_pet.py` & `citation_utils-0.4.3/citation_utils/dockets/constructed_pet.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.2/citation_utils/dockets/constructed_udk.py` & `citation_utils-0.4.3/citation_utils/dockets/constructed_udk.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.2/citation_utils/dockets/models/constructor.py` & `citation_utils-0.4.3/citation_utils/dockets/models/constructor.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.2/citation_utils/dockets/models/docket_category.py` & `citation_utils-0.4.3/citation_utils/dockets/models/docket_category.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.2/citation_utils/dockets/models/docket_citation.py` & `citation_utils-0.4.3/citation_utils/dockets/models/docket_citation.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.2/citation_utils/dockets/models/docket_model.py` & `citation_utils-0.4.3/citation_utils/dockets/models/docket_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,47 +6,60 @@
 from citation_report.main import is_eq
 from dateutil.parser import parse
 from pydantic import BaseModel, ConfigDict, Field
 
 from .docket_category import DocketCategory
 from .gr_clean import gr_prefix_clean
 
-DB_SERIAL_NUM = re.compile(r"^[a-z0-9-]+$")
-"""Ideally, the docket id for the database should only be alphanumeric, lowercase with dashes."""  # noqa: E501
+DB_SERIAL_NUM = re.compile(r"^(?P<serial>[a-z0-9-]+).*$")
+"""Ideally, the docket id for the database should only be alpha-numeric, lowercase with dashes."""  # noqa: E501
 
 
 class Docket(BaseModel):
     """
-    The Docket is the modern identifier of a Supreme Court decision.
+    The `Docket` is the modern identifier of a Supreme Court decision. This data structure
+    however is not the final form of the identifier since that description belongs to the `Citation`
+    and the `CountedCitation`.
+
+    The purpose of this intermediate structure is that a `Docket` is often paired with a `Report`, which
+    is the traditional identifier based on volume and page numbers. The pairing however is not
+    mandatory, thus needed flexibility to create structures with the following combinations of
+    the eventual Citation object:
+
+    Citation | Docket | Report
+    :--:|:--:|:--:
+    has both docket and report | yes | yes
+    only a docket | yes | no
+    only a report | no | yes
 
-    It is based on a `category`, a `serial id`, and a `date`.
+    See docket_citation.DocketReportCitation to see structure of paired content.
+
+    A `Docket` is based on a `category`, a `serial id`, and a `date`. Since the serial id
+    may required
 
     Field | Type | Description
     --:|:--:|:--
     `context` | optional (str) | Full text matched by the regex pattern
     `category` | optional (DocketCategory) | Whether GR, AC, etc.
     `ids` | optional (str) | The serial number of the docket category
     `docket_date` | optional (date) | The date associated with the docket
 
     Sample Citation | Category | Serial | Date
     :-- |:--:|:--:|:--:
     _G.R. Nos. 138570, October 10, 2000_ | GR | 74910 | October 10, 2000
     _A.M. RTJ-12-2317 (Formerly OCA I.P.I. No. 10-3378-RTJ), Jan 1, 2000_ | AM | RTJ-12-2317 |Jan 1, 2000
     _A.C. No. 10179 (Formerly CBD 11-2985), March 04, 2014_ | AC | 10179 | Mar. 4, 2014
-
-    The Docket is often paired with a Report, which is the traditional
-    identifier based on volume and page numbers.
-
-    # TODO: need further cleaning of serial_text
     """  # noqa: E501
 
     model_config = ConfigDict(use_enum_values=True)
     context: str = Field(..., description="Full text matched by regex pattern.")
     category: DocketCategory = Field(..., description="e.g. General Register, etc.")
-    ids: str = Field(..., description="May be comma-separated, e.g. '12, 32, and 41'")
+    ids: str = Field(
+        ..., description="Thismay not be May be comma-separated, e.g. '12, 32, and 41'"
+    )
     docket_date: date = Field(...)
 
     def __repr__(self) -> str:
         return f"<Docket: {self.category} {self.serial_text}, {self.formatted_date}>"
 
     def __str__(self) -> str:
         if self.serial_text:
@@ -99,25 +112,34 @@
     @property
     def formatted_date(self) -> str | None:
         if self.docket_date:
             return self.docket_date.strftime(DOCKET_DATE_FORMAT)
         return None
 
     @classmethod
-    def from_data(cls, data: dict):
-        """Presumes data with keys: `cat`, `num`, and `date`"""
-        cat, num, date = data.get("cat"), data.get("num"), data.get("date")
-        if not cat or not num or not date:
-            raise Exception(f"Missing field for construction from {data=}")
-        return cls(
-            context="",
-            category=DocketCategory[cat.upper()],
-            ids=num,
-            docket_date=parse(date).date(),
-        )
-
-    @classmethod
     def check_serial_num(cls, text: str) -> bool:
         """If a serial number exists, ensure it meets criteria prior to row creation."""
         if DB_SERIAL_NUM.search(text.lower()):
             return True
         return False
+
+    @classmethod
+    def clean_serial(cls, text: str) -> str | None:
+        """Criteria:
+
+        1. Must be lowercased
+        2. Characters that can be included `a-z`, `0-9`, `-`
+        3. Must only contain a single alpha-numeric reference
+
+        Args:
+            text (str): Raw text to clean
+
+        Returns:
+            str: Cleaned serial text fit for database input.
+        """
+        text = text.lower()
+        if " " in text:
+            text = text.split()[0]
+        if match := DB_SERIAL_NUM.search(text):
+            if candidate := match.group("serial"):
+                return candidate
+        return None
```

### Comparing `citation_utils-0.4.2/citation_utils/dockets/models/docket_rules.py` & `citation_utils-0.4.3/citation_utils/dockets/models/docket_rules.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.2/citation_utils/dockets/models/gr_clean.py` & `citation_utils-0.4.3/citation_utils/dockets/models/gr_clean.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.2/citation_utils/dockets/models/misc/extra.py` & `citation_utils-0.4.3/citation_utils/dockets/models/misc/extra.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.2/citation_utils/dockets/models/misc/num.py` & `citation_utils-0.4.3/citation_utils/dockets/models/misc/num.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.2/citation_utils/document.py` & `citation_utils-0.4.3/citation_utils/document.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.2/citation_utils/special.py` & `citation_utils-0.4.3/citation_utils/special.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.2/pyproject.toml` & `citation_utils-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citation_utils"
-version = "0.4.2"
+version = "0.4.3"
 description = "Pattern matching Philippine Supreme Court citations."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/citation-utils"
 documentation = "https://justmars.github.io/citation-utils"
 classifiers = [
   "Topic :: Text Processing :: General",
```

### Comparing `citation_utils-0.4.2/PKG-INFO` & `citation_utils-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation-utils
-Version: 0.4.2
+Version: 0.4.3
 Summary: Pattern matching Philippine Supreme Court citations.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pydantic
```

