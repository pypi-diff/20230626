# Comparing `tmp/spothinta_api-0.3.0.tar.gz` & `tmp/spothinta_api-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spothinta_api-0.3.0.tar", max compression
+gzip compressed data, was "spothinta_api-0.4.0.tar", max compression
```

## Comparing `spothinta_api-0.3.0.tar` & `spothinta_api-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1082 2023-05-28 18:21:41.739913 spothinta_api-0.3.0/LICENSE
--rw-r--r--   0        0        0     5127 2023-05-28 18:21:41.739913 spothinta_api-0.3.0/README.md
--rw-r--r--   0        0        0     3607 2023-05-28 18:22:08.980031 spothinta_api-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      346 2023-05-28 18:21:41.739913 spothinta_api-0.3.0/spothinta_api/__init__.py
--rw-r--r--   0        0        0      399 2023-05-28 18:21:41.739913 spothinta_api-0.3.0/spothinta_api/const.py
--rw-r--r--   0        0        0      410 2023-05-28 18:21:41.739913 spothinta_api-0.3.0/spothinta_api/exceptions.py
--rw-r--r--   0        0        0     6615 2023-05-28 18:21:41.739913 spothinta_api-0.3.0/spothinta_api/models.py
--rw-r--r--   0        0        0        0 2023-05-28 18:21:41.743913 spothinta_api-0.3.0/spothinta_api/py.typed
--rw-r--r--   0        0        0     4751 2023-05-28 18:21:41.743913 spothinta_api-0.3.0/spothinta_api/spothinta.py
--rw-r--r--   0        0        0     6045 1970-01-01 00:00:00.000000 spothinta_api-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-26 18:24:39.817314 spothinta_api-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5127 2023-06-26 18:24:39.817314 spothinta_api-0.4.0/README.md
+-rw-r--r--   0        0        0     3614 2023-06-26 18:24:54.549281 spothinta_api-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      346 2023-06-26 18:24:39.817314 spothinta_api-0.4.0/spothinta_api/__init__.py
+-rw-r--r--   0        0        0     1133 2023-06-26 18:24:39.817314 spothinta_api-0.4.0/spothinta_api/const.py
+-rw-r--r--   0        0        0      410 2023-06-26 18:24:39.817314 spothinta_api-0.4.0/spothinta_api/exceptions.py
+-rw-r--r--   0        0        0     9421 2023-06-26 18:24:39.817314 spothinta_api-0.4.0/spothinta_api/models.py
+-rw-r--r--   0        0        0        0 2023-06-26 18:24:39.817314 spothinta_api-0.4.0/spothinta_api/py.typed
+-rw-r--r--   0        0        0     4840 2023-06-26 18:24:39.817314 spothinta_api-0.4.0/spothinta_api/spothinta.py
+-rw-r--r--   0        0        0     6045 1970-01-01 00:00:00.000000 spothinta_api-0.4.0/PKG-INFO
```

### Comparing `spothinta_api-0.3.0/LICENSE` & `spothinta_api-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spothinta_api-0.3.0/README.md` & `spothinta_api-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `spothinta_api-0.3.0/pyproject.toml` & `spothinta_api-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spothinta-api"
-version = "0.3.0"
+version = "0.4.0"
 description = "Asynchronous Python client providing energy prices from spot-hinta.fi"
 authors = ["Sebastian Lövdahl <sebastian.lovdahl@hibox.fi>"]
 maintainers = ["Sebastian Lövdahl <sebastian.lovdahl@hibox.fi>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["energy", "spothinta", "prices", "api", "async", "client"]
 classifiers = [
@@ -27,21 +27,21 @@
 
 [tool.poetry.dependencies]
 aiohttp = ">=3.0.0"
 python = "^3.9"
 yarl = ">=1.6.0"
 
 [tool.poetry.group.dev.dependencies]
-ruff = ">=0.0.243,<0.0.271"
+ruff = ">=0.0.243,<0.0.276"
 aresponses = "^2.1.6"
-black = "^22.12"
+black = ">=22.12,<24.0"
 blacken-docs = "^1.13.0"
 codespell = "^2.2.2"
 coverage = {version = ">=7.2,<8.0", extras = ["toml"]}
-mypy = ">=1.0,<1.4"
+mypy = ">=1.0,<1.5"
 pre-commit = "^3.3.2"
 pre-commit-hooks = "^4.4.0"
 pylint = "^2.16.1"
 pytest = "^7.2.1"
 pytest-asyncio = ">=0.20.3,<0.22.0"
 pytest-cov = "^4.0.0"
 pytest-freezer = "^0.4.6"
```

### Comparing `spothinta_api-0.3.0/spothinta_api/models.py` & `spothinta_api-0.4.0/spothinta_api/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Data models for the spot-hinta.fi API."""
 from __future__ import annotations
 
 from dataclasses import dataclass
-from datetime import datetime, timedelta, timezone
+from datetime import datetime, timedelta
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from collections.abc import Callable
+    from zoneinfo import ZoneInfo
 
 
 def _timed_value(moment: datetime, prices: dict[datetime, float]) -> float | None:
     """Return a function that returns a value at a specific time.
 
     Args:
     ----
@@ -51,24 +52,25 @@
 
 
 @dataclass
 class Electricity:
     """Object representing electricity data."""
 
     prices: dict[datetime, float]
+    time_zone: ZoneInfo
 
     @property
     def current_price(self) -> float | None:
         """Return the price for the current hour.
 
         Returns
         -------
             The price for the current hour or None if no price is available.
         """
-        return self.price_at_time(self.utcnow())
+        return self.price_at_time(self.now_in_timezone())
 
     @property
     def lowest_price_today(self) -> float | None:
         """Return the minimum price today.
 
         Returns
         -------
@@ -78,14 +80,29 @@
 
         if len(prices) == 0:
             return None
 
         return round(min(prices.values()), 5)
 
     @property
+    def lowest_price_tomorrow(self) -> float | None:
+        """Return the minimum price tomorrow.
+
+        Returns
+        -------
+            The minimum price tomorrow or None if no prices are available for tomorrow.
+        """
+        prices = self.prices_tomorrow()
+
+        if len(prices) == 0:
+            return None
+
+        return round(min(prices.values()), 5)
+
+    @property
     def highest_price_today(self) -> float | None:
         """Return the maximum price today.
 
         Returns
         -------
             The maximum price today or None if no prices are available for today.
         """
@@ -93,55 +110,117 @@
 
         if len(prices) == 0:
             return None
 
         return round(max(prices.values()), 5)
 
     @property
-    def average_price(self) -> float | None:
+    def highest_price_tomorrow(self) -> float | None:
+        """Return the maximum price tomorrow.
+
+        Returns
+        -------
+            The maximum price tomorrow or None if no prices are available for tomorrow.
+        """
+        prices = self.prices_tomorrow()
+
+        if len(prices) == 0:
+            return None
+
+        return round(max(prices.values()), 5)
+
+    @property
+    def average_price_today(self) -> float | None:
         """Return the average price today.
 
         Returns
         -------
             The average price today or None if no prices are available for today.
         """
         prices_today = self.prices_today()
 
         if len(prices_today) == 0:
             return None
 
         return round(sum(prices_today.values()) / len(prices_today), 5)
 
     @property
-    def highest_price_time(self) -> datetime | None:
-        """Return the time of the highest price.
+    def average_price_tomorrow(self) -> float | None:
+        """Return the average price tomorrow.
+
+        Returns
+        -------
+            The average price tomorrow or None if no prices are available for tomorrow.
+        """
+        prices_tomorrow = self.prices_tomorrow()
+
+        if len(prices_tomorrow) == 0:
+            return None
+
+        return round(sum(prices_tomorrow.values()) / len(prices_tomorrow), 5)
+
+    @property
+    def highest_price_time_today(self) -> datetime | None:
+        """Return the time of the highest price today.
 
         Returns
         -------
             The time of the highest price or None if no prices are available for today.
         """
         return _get_pricetime(self.prices_today(), max)
 
     @property
-    def lowest_price_time(self) -> datetime | None:
-        """Return the time of the lowest price.
+    def highest_price_time_tomorrow(self) -> datetime | None:
+        """Return the time of the highest price tomorrow.
+
+        Returns
+        -------
+            The time of the highest price or None if no prices are available for
+            tomorrow.
+        """
+        return _get_pricetime(self.prices_tomorrow(), max)
+
+    @property
+    def lowest_price_time_today(self) -> datetime | None:
+        """Return the time of the lowest price today.
 
         Returns
         -------
             The time of the lowest price or None if no prices are available for today.
         """
         return _get_pricetime(self.prices_today(), min)
 
     @property
+    def lowest_price_time_tomorrow(self) -> datetime | None:
+        """Return the time of the lowest price tomorrow.
+
+        Returns
+        -------
+            The time of the lowest price or None if no prices are available for
+            tomorrow.
+        """
+        return _get_pricetime(self.prices_tomorrow(), min)
+
+    @property
     def timestamp_prices(self) -> list[dict[str, float | datetime]]:
-        """Return a dictionary with the prices.
+        """Return a dictionary with all known prices.
+
+        Returns
+        -------
+            A dictionary with the prices for all known prices.
+        """
+        return self.generate_timestamp_list(self.prices)
+
+    @property
+    def timestamp_prices_today(self) -> list[dict[str, float | datetime]]:
+        """Return a dictionary with the prices for today.
 
         Returns
         -------
-            A dictionary with the prices.
+            A dictionary with the prices for today.
         """
         return self.generate_timestamp_list(self.prices_today())
 
     @property
     def hours_priced_equal_or_lower(self) -> int:
         """Return the number of hours with the current price or better.
 
@@ -156,28 +235,43 @@
         """Return the prices for today.
 
         Returns
         -------
             The prices for today.
         """
         prices_today = {}
-        today = datetime.utcnow().astimezone().date()  # noqa: DTZ003
+        today = self.now_in_timezone().astimezone().date()
         for timestamp, price in self.prices.items():
             if timestamp.date() == today:
                 prices_today[timestamp] = price
         return prices_today
 
-    def utcnow(self) -> datetime:
-        """Return the current timestamp in the UTC timezone.
+    def prices_tomorrow(self) -> dict[datetime, float]:
+        """Return the prices for tomorrow.
+
+        Returns
+        -------
+            The prices for tomorrow.
+        """
+        prices_tomorrow = {}
+        tomorrow = (self.now_in_timezone() + timedelta(days=1)).astimezone().date()
+
+        for timestamp, price in self.prices.items():
+            if timestamp.date() == tomorrow:
+                prices_tomorrow[timestamp] = price
+        return prices_tomorrow
+
+    def now_in_timezone(self) -> datetime:
+        """Return the current timestamp in the current timezone.
 
         Returns
         -------
-            The current timestamp in the UTC timezone.
+            The current timestamp in the current timezone.
         """
-        return datetime.now(timezone.utc)
+        return datetime.now(tz=self.time_zone)
 
     def generate_timestamp_list(
         self,
         prices: dict[datetime, float],
     ) -> list[dict[str, float | datetime]]:
         """Return a list of dictionaries with the prices and timestamps.
 
@@ -196,40 +290,43 @@
 
     def price_at_time(self, moment: datetime) -> float | None:
         """Return the price at a specific time.
 
         Args:
         ----
             moment: The time to get the price for.
-            data_type: The type of data to get the price for.
-                Can be "usage" (default) or "return".
 
         Returns:
         -------
             The price at the specified time.
         """
-        # Get the price at the specified time
         value = _timed_value(moment, self.prices)
         if value is not None or value == 0:
             return value
         return None
 
     @classmethod
-    def from_dict(cls: type[Electricity], data: list[dict[str, Any]]) -> Electricity:
+    def from_dict(
+        cls: type[Electricity],
+        data: list[dict[str, Any]],
+        time_zone: ZoneInfo,
+    ) -> Electricity:
         """Create an Electricity object from a dictionary.
 
         Args:
         ----
             data: A dictionary with the data from the API.
+            time_zone: The timezone to use for determining "today" and "tomorrow".
 
         Returns:
         -------
             An Electricity object.
         """
         prices: dict[datetime, float] = {}
         for item in data:
             prices[datetime.strptime(item["DateTime"], "%Y-%m-%dT%H:%M:%S%z")] = item[
                 "PriceWithTax"
             ]
         return cls(
             prices=prices,
+            time_zone=time_zone,
         )
```

### Comparing `spothinta_api-0.3.0/spothinta_api/spothinta.py` & `spothinta_api-0.4.0/spothinta_api/spothinta.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import async_timeout
 from aiohttp import ClientResponseError
 from aiohttp.client import ClientError, ClientSession
 from aiohttp.hdrs import METH_GET
 from yarl import URL
 
-from .const import API_HOST, Region
+from .const import API_HOST, REGION_TO_TIMEZONE, Region
 from .exceptions import (
     SpotHintaConnectionError,
     SpotHintaError,
     SpotHintaNoDataError,
     SpotHintaRateLimitError,
 )
 from .models import Electricity
@@ -133,15 +133,17 @@
             uri="/TodayAndDayForward",
             params={"region": region.name},
         )
 
         if len(data) == 0:
             msg = "No energy prices found."
             raise SpotHintaNoDataError(msg)
-        return Electricity.from_dict(data)
+
+        time_zone = REGION_TO_TIMEZONE[region]
+        return Electricity.from_dict(data, time_zone=time_zone)
 
     async def close(self) -> None:
         """Close open client session."""
         if self.session and self._close_session:
             await self.session.close()
 
     async def __aenter__(self) -> SpotHinta:
```

### Comparing `spothinta_api-0.3.0/PKG-INFO` & `spothinta_api-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spothinta-api
-Version: 0.3.0
+Version: 0.4.0
 Summary: Asynchronous Python client providing energy prices from spot-hinta.fi
 License: MIT
 Keywords: energy,spothinta,prices,api,async,client
 Author: Sebastian Lövdahl
 Author-email: sebastian.lovdahl@hibox.fi
 Maintainer: Sebastian Lövdahl
 Maintainer-email: sebastian.lovdahl@hibox.fi
```

