# Comparing `tmp/alphavantage_api_client-2.2.1-py3-none-any.whl.zip` & `tmp/alphavantage_api_client-2.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,23 @@
-Zip file size: 26290 bytes, number of entries: 19
--rw-rw-r--  2.0 unx      241 b- defN 22-Jul-13 23:52 alphavantage_api_client/__init__.py
+Zip file size: 29088 bytes, number of entries: 21
+-rw-rw-r--  2.0 unx      241 b- defN 23-May-30 16:40 alphavantage_api_client/__init__.py
 -rw-rw-r--  2.0 unx      800 b- defN 22-Jul-02 20:13 alphavantage_api_client/__main__.py
--rw-rw-r--  2.0 unx    19191 b- defN 22-Sep-01 17:05 alphavantage_api_client/client.py
--rw-rw-r--  2.0 unx     7614 b- defN 22-Jul-27 01:15 alphavantage_api_client/models.py
+-rw-rw-r--  2.0 unx    20255 b- defN 23-Jun-26 17:01 alphavantage_api_client/client.py
+-rw-rw-r--  2.0 unx     7951 b- defN 23-Jun-26 17:01 alphavantage_api_client/models.py
 -rw-rw-r--  2.0 unx     7725 b- defN 22-Sep-01 17:05 alphavantage_api_client/response_validation_rules.py
 -rw-rw-r--  2.0 unx    11793 b- defN 22-Jul-27 01:15 alphavantage_api_client/ticker.py
 -rw-rw-r--  2.0 unx      260 b- defN 22-May-21 19:54 alphavantage_api_client/version.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jun-26 17:01 examples/__init__.py
+-rw-rw-r--  2.0 unx     7031 b- defN 23-Jun-26 17:01 examples/getting_started.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Jun-30 16:06 tests/__init__.py
--rw-rw-r--  2.0 unx     3234 b- defN 22-Jun-30 16:06 tests/mock_client.py
+-rw-rw-r--  2.0 unx     3373 b- defN 23-Jun-26 13:20 tests/mock_client.py
 -rw-rw-r--  2.0 unx     1948 b- defN 22-Sep-01 17:05 tests/test_evaluate_company.py
--rw-rw-r--  2.0 unx     7437 b- defN 22-Jul-13 23:52 tests/test_mock_client_unit.py
--rw-rw-r--  2.0 unx    19644 b- defN 22-Sep-01 17:05 tests/test_multi_client_integration.py
--rw-rw-r--  2.0 unx    18350 b- defN 22-Sep-01 17:05 tests/test_single_client_cache_integration.py
+-rw-rw-r--  2.0 unx     7788 b- defN 23-Jun-26 13:20 tests/test_mock_client_unit.py
+-rw-rw-r--  2.0 unx    19650 b- defN 23-Jun-26 13:20 tests/test_multi_client_integration.py
+-rw-rw-r--  2.0 unx    18669 b- defN 23-Jun-26 13:20 tests/test_single_client_cache_integration.py
 -rw-rw-r--  2.0 unx     2966 b- defN 22-Jul-27 01:15 tests/test_ticker.py
--rw-rw-r--  2.0 unx     1067 b- defN 22-Sep-03 14:37 alphavantage_api_client-2.2.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx    14247 b- defN 22-Sep-03 14:37 alphavantage_api_client-2.2.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Sep-03 14:37 alphavantage_api_client-2.2.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       30 b- defN 22-Sep-03 14:37 alphavantage_api_client-2.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1718 b- defN 22-Sep-03 14:37 alphavantage_api_client-2.2.1.dist-info/RECORD
-19 files, 118357 bytes uncompressed, 23436 bytes compressed:  80.2%
+-rw-rw-r--  2.0 unx     1067 b- defN 23-Jun-26 17:18 alphavantage_api_client-2.2.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    14032 b- defN 23-Jun-26 17:18 alphavantage_api_client-2.2.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-26 17:18 alphavantage_api_client-2.2.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       39 b- defN 23-Jun-26 17:18 alphavantage_api_client-2.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1876 b- defN 23-Jun-26 17:18 alphavantage_api_client-2.2.2.dist-info/RECORD
+21 files, 127556 bytes uncompressed, 25988 bytes compressed:  79.6%
```

## zipnote {}

```diff
@@ -15,14 +15,20 @@
 
 Filename: alphavantage_api_client/ticker.py
 Comment: 
 
 Filename: alphavantage_api_client/version.py
 Comment: 
 
+Filename: examples/__init__.py
+Comment: 
+
+Filename: examples/getting_started.py
+Comment: 
+
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/mock_client.py
 Comment: 
 
 Filename: tests/test_evaluate_company.py
@@ -36,23 +42,23 @@
 
 Filename: tests/test_single_client_cache_integration.py
 Comment: 
 
 Filename: tests/test_ticker.py
 Comment: 
 
-Filename: alphavantage_api_client-2.2.1.dist-info/LICENSE
+Filename: alphavantage_api_client-2.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: alphavantage_api_client-2.2.1.dist-info/METADATA
+Filename: alphavantage_api_client-2.2.2.dist-info/METADATA
 Comment: 
 
-Filename: alphavantage_api_client-2.2.1.dist-info/WHEEL
+Filename: alphavantage_api_client-2.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: alphavantage_api_client-2.2.1.dist-info/top_level.txt
+Filename: alphavantage_api_client-2.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: alphavantage_api_client-2.2.1.dist-info/RECORD
+Filename: alphavantage_api_client-2.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## alphavantage_api_client/client.py

```diff
@@ -6,15 +6,15 @@
 from .response_validation_rules import ValidationRuleChecks
 import json
 from alphavantage_api_client.models import GlobalQuote, Quote, AccountingReport, CompanyOverview, RealGDP, \
     CsvNotSupported
 import copy
 import logging
 import hashlib
-from typing import Optional
+from typing import Optional, Union
 
 
 class ApiKeyNotFound(Exception):
 
     def __init__(self, message: str):
         super().__init__(message)
 
@@ -138,31 +138,36 @@
         """
         if api_key is None or len(api_key) == 0:
             raise ApiKeyNotFound("API Key is null or empty. Please specify a valid api key")
         self.__api_key__ = api_key
 
         return self
 
-    def get_global_quote(self, event: dict) -> GlobalQuote:
+    def get_global_quote(self, event: Union[str, dict]) -> GlobalQuote:
         """ Lightweight access to obtain stock quote data
 
         A lightweight alternative to the time series APIs, this service returns the price and volume information
         for a token of your choice.
         Args:
-            event (dict): A ``dict`` containing the paramters supported by the api.
+            event (dict): A ``dict`` containing the parameters supported by the api.
             Minimum required value is ``symbol (str)``
 
         Returns:
             :rtype: GlobalQuote
 
         """
+        event_dict = event
+        if isinstance(event, str):
+            event_dict = {
+                "symbol": event
+            }
         defaults = {
             "function": "GLOBAL_QUOTE"
         }
-        json_request = self.__create_api_request_from__(defaults, event)
+        json_request = self.__create_api_request_from__(defaults, event_dict)
         json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
 
         return GlobalQuote.parse_obj(json_response)
 
     def get_daily_quote(self, event: dict) -> Quote:
         """
         This API returns raw (as-traded) daily time series (date, daily open, daily high, daily low, daily close, daily
@@ -200,15 +205,20 @@
             :rtype: Quote
 
         """
         # default params
         defaults = {"symbol": None, "datatype": "json", "function": "TIME_SERIES_INTRADAY",
                     "interval": "60min", "slice": "year1month1",
                     "outputsize": "compact"}
-        json_request = self.__create_api_request_from__(defaults, event)
+        event_dict = event
+        if isinstance(event, str):
+            event_dict = {
+                "symbol": event
+            }
+        json_request = self.__create_api_request_from__(defaults, event_dict)
         json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
 
         return Quote.parse_obj(json_response)
 
     def get_income_statement(self, event: dict) -> AccountingReport:
         """
         This API returns the annual and quarterly income statements for the company of interest, with
@@ -224,29 +234,40 @@
 
         """
 
         defaults = {
             "function": "INCOME_STATEMENT",
             "datatype": "json"
         }
-        if event.get("datatype") == "csv":
-            raise CsvNotSupported(defaults.get("function"), event)
-        json_request = self.__create_api_request_from__(defaults, event)
+        event_dict = event
+        if isinstance(event, str):
+            event_dict = {
+                "symbol": event
+            }
+        if event_dict.get("datatype") == "csv":
+            raise CsvNotSupported(defaults.get("function"), event_dict)
+        json_request = self.__create_api_request_from__(defaults, event_dict)
         json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
 
         return AccountingReport.parse_obj(json_response)
 
     def get_balance_sheet(self, event: dict) -> AccountingReport:
         defaults = {
             "function": "BALANCE_SHEET",
             "datatype": "json"
         }
-        if event.get("datatype") == "csv":
-            raise CsvNotSupported(defaults.get("function"), event)
-        json_request = self.__create_api_request_from__(defaults, event)
+        event_dict = event
+        if isinstance(event, str):
+            event_dict = {
+                "symbol": event
+            }
+        if event_dict.get("datatype") == "csv":
+            raise CsvNotSupported(defaults.get("function"), event_dict)
+
+        json_request = self.__create_api_request_from__(defaults, event_dict)
         json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
 
         return AccountingReport.parse_obj(json_response)
 
     def get_cash_flow(self, event: dict) -> AccountingReport:
         """
         This API returns the annual and quarterly cash flow for the company of interest, with normalized fields
@@ -260,22 +281,27 @@
             :rtype: AccountingReport
 
         """
         defaults = {
             "function": "CASH_FLOW",
             "datatype": "json"
         }
-        if event.get("datatype") == "csv":
-            raise CsvNotSupported(defaults.get("function"), event)
-        json_request = self.__create_api_request_from__(defaults, event)
+        event_dict = event
+        if isinstance(event, str):
+            event_dict = {
+                "symbol": event
+            }
+        if event_dict.get("datatype") == "csv":
+            raise CsvNotSupported(defaults.get("function"), event_dict)
+        json_request = self.__create_api_request_from__(defaults, event_dict)
         json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
 
         return AccountingReport.parse_obj(json_response)
 
-    def get_earnings(self, event: dict) -> AccountingReport:
+    def get_earnings(self, event: Union[str, dict]) -> AccountingReport:
         """
         This API returns the annual and quarterly earnings (EPS) for the company of interest. Quarterly data also
         includes analyst estimates and surprise metrics.
 
         Args:
             event (dict): A Dictionary of parameters that will be passed to the api.
             Minimum required is ``symbol`` = ``str``
@@ -284,17 +310,23 @@
             :rtype: AccountingReport
 
         """
         defaults = {
             "function": "EARNINGS",
             "datatype": "json"
         }
-        if event.get("datatype") == "csv":
-            raise CsvNotSupported(defaults.get("function"), event)
-        json_request = self.__create_api_request_from__(defaults, event)
+        event_dict = event
+        if isinstance(event, str):
+            event_dict = {
+                "symbol": event
+            }
+
+        if event_dict.get("datatype") == "csv":
+            raise CsvNotSupported(defaults.get("function"), event_dict)
+        json_request = self.__create_api_request_from__(defaults, event_dict)
         json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
 
         return AccountingReport.parse_obj(json_response)
 
     def get_company_overview(self, event: dict) -> CompanyOverview:
         """
         This API returns the company information, financial ratios, and other key metrics for the equity specified.
@@ -307,17 +339,22 @@
         Returns:
             Return a CompanyOverview Object
 
         """
         defaults = {
             "function": "OVERVIEW"
         }
-        if event.get("datatype") == "csv":
-            raise CsvNotSupported(defaults.get("function"), event)
-        json_request = self.__create_api_request_from__(defaults, event)
+        event_dict = event
+        if isinstance(event, str):
+            event_dict = {
+                "symbol": event
+            }
+        if event_dict.get("datatype") == "csv":
+            raise CsvNotSupported(defaults.get("function"), event_dict)
+        json_request = self.__create_api_request_from__(defaults, event_dict)
         json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
 
         return CompanyOverview.parse_obj(json_response)
 
     def get_crypto_intraday(self, event: dict) -> Quote:
         """
         This API returns intraday time series (timestamp, open, high, low, close, volume) of the cryptocurrency
```

## alphavantage_api_client/models.py

```diff
@@ -42,14 +42,25 @@
             for quote_date in self.data:
                 quotes = self.data[quote_date]
                 quotes["query_date"] = quote_date
                 return quotes
 
         return None
 
+    def get_oldest_value(self) -> Optional[dict]:
+        if len(self.data) > 0:
+            quote_dates = list(self.data.keys())
+            last_quote_date = quote_dates[len(quote_dates)-1]
+            quote = self.data[last_quote_date]
+            quote["query_date"] = last_quote_date
+
+            return quote
+
+        return None
+
 
 class GlobalQuote(BaseQuote):
     data: dict = Field({}, alias='Global Quote')
 
     def get_open_price(self) -> str:
         field = "02. open"
         return self.get_data_value(field)
```

## tests/mock_client.py

```diff
@@ -54,14 +54,16 @@
             text_file = open(f"{self.base_path}/mock_technical_indicator_ema.json")
         elif event.get("function") == "SMA":
             text_file = open(f"{self.base_path}/mock_technical_indicator_sma_equity.json", "r")
         elif event.get("function") == "TIME_SERIES_DAILY" and event.get("outputsize") == "compact":
             text_file = open(f"{self.base_path}/mock_stock_price_full.json", "r")
         elif event.get("function") == "TIME_SERIES_INTRADAY" and event.get("interval") == "5min":
             text_file = open(f"{self.base_path}/mock_intraday_series_quote.json", "r")
+        elif event.get("function") == "NEWS_SENTIMENT":
+            text_file = open(f"{self.base_path}/mock_news_an_sentiment.json", "r")
         else:
             raise ValueError(f"We don't have a mock data file for your request {json.dumps(event)}")
 
         data = text_file.read()
         text_file.close()
         json_response = json.loads(data)
         json_response["success"] = True
```

## tests/test_mock_client_unit.py

```diff
@@ -1,10 +1,11 @@
 import pytest
 from .mock_client import MockAlphavantageClient
 import logging
+import json
 
 # Reference for logging in pytest: https://docs.pytest.org/en/7.1.x/how-to/logging.html
 # Reference for logging: https://docs.python.org/3/howto/logging.html
 # Reference for logging: https://www.youtube.com/watch?v=-ARI4Cz-awo&t=0s
 
 @pytest.mark.unit
 def test_get_intraday_quote():
@@ -37,14 +38,25 @@
     assert global_quote.symbol == event["symbol"], "Symbol from results don't match event"
     assert "meta_data" not in global_quote, "Metadata should not be present since it's not in the api"
     assert len(global_quote.data) > 0, "Data field is zero or not present"
     logging.warning(f"Successfully tested test_quote_stock_price for {event['symbol']}")
 
 
 @pytest.mark.unit
+def test_news_an_sentiment():
+    client = MockAlphavantageClient()
+    event = {
+        "function" : "NEWS_SENTIMENT",
+        "ticker": "TSLA"
+    }
+    result = client.get_data_from_alpha_vantage(event)
+    assert result['success'], 'We should have gotten news and sentiment correctly'
+    print(json.dumps(result))
+
+@pytest.mark.unit
 def test_get_cash_flow():
     
     client = MockAlphavantageClient()
     event = {
         "symbol": "ibm"
     }
     accounting_report = client.get_cash_flow(event)
```

## tests/test_multi_client_integration.py

```diff
@@ -154,15 +154,15 @@
 
     assert limit_reached, "Failed to reach limit"
     assert results.symbol == event['symbol'], f" Expected symbol doesn't match given: {event.get('symbol', None)}"
 
     logging.warning(f" Can Reach Limit while quoting for symbol {event.get('symbol', None)} in JSON")
 
 
-@pytest.mark.integration
+@pytest.mark.integration_paid
 def test_can_quote_intraday():
     event = {
         "symbol": "TSLA",
         "interval": "5min"
     }
     client = AlphavantageClient().should_retry_once()
     intra_day_quote = client.get_intraday_quote(event)
@@ -179,18 +179,18 @@
     }
     client = AlphavantageClient().should_retry_once()
     daily_quote = client.get_daily_quote(event)
     print(daily_quote.json())
     assert not daily_quote.limit_reached, f"limit_reached should not be true {daily_quote.error_message}"
     assert daily_quote.success, f"success is false {daily_quote.error_message}"
     assert len(daily_quote.data), f"Did not return data for this symbol {daily_quote.symbol}"
-    logging.warning(f" Successfully quoted cryptocurrency symbol {event['symbol']} in JSON")
+    logging.warning(f" Successfully quoted symbol {event['symbol']} in JSON")
 
 
-@pytest.mark.integration
+@pytest.mark.integrationn_paid
 def test_can_quote_crypto():
     event = {
         "function": "CRYPTO_INTRADAY",
         "symbol": "ETH",
         "market": "USD",
         "interval": "5min"
     }
@@ -198,15 +198,15 @@
     results = client.get_crypto_intraday(event)
     assert not results.limit_reached, f"limit_reached should not be true {results.error_message}"
     assert results.success, f"success is false {results.error_message}"
     assert len(results.data), "Data{} property is empty but should have information"
     logging.warning(f" Successfully quoted cryptocurrency symbol {event['symbol']} in JSON")
 
 
-@pytest.mark.integration
+@pytest.mark.integration_paid
 def test_can_quote_crypto_csv():
     event = {
         "function": "CRYPTO_INTRADAY",
         "symbol": "ETH",
         "market": "USD",
         "interval": "5min",
         "datatype": "csv"
@@ -482,15 +482,15 @@
     results = client.get_data_from_alpha_vantage(event)
     assert type(results) is dict, "Results object should be a dictionary"
     assert len(results) > 0, "There should be data in the results"
 
     logging.warning("Successfully queried data using get_data_from_alpha_vantage")
 
 
-@pytest.mark.integration
+@pytest.mark.integration_paid
 def test_get_fx_currency_data():
     event = {
         "function" : "CURRENCY_EXCHANGE_RATE",
         "from_currency" : "JPY",
         "to_currency" : "USD"
     }
     client = AlphavantageClient().should_retry_once()
```

## tests/test_single_client_cache_integration.py

```diff
@@ -4,14 +4,25 @@
 import logging
 import json
 
 client = AlphavantageClient().should_retry_once().use_simple_cache()
 
 
 @pytest.mark.integration
+def test_can_get_news_and_sentiment():
+    client = AlphavantageClient()
+    event = {
+        "function" : "NEWS_SENTIMENT",
+        "tickers": "TSLA"
+    }
+    result = client.get_data_from_alpha_vantage(event)
+    print(json.dumps(result))
+    assert result['success'], 'could not get news and sentiment'
+
+@pytest.mark.integration
 def test_can_query_from_cache():
     event = {
         "symbol": "tsla"
     }
 
     for i in range(200):
         global_quote = client.get_global_quote(event)
@@ -145,45 +156,45 @@
         "symbol": "TSLA",
         "interval": "5min"
     }
     intra_day_quote = client.get_intraday_quote(event)
     assert not intra_day_quote.limit_reached, f"limit_reached should not be true {intra_day_quote.error_message}"
     assert intra_day_quote.success, f"success is false {intra_day_quote.error_message}"
     assert len(intra_day_quote.data), f"Did not return data for this symbol {intra_day_quote.symbol}"
-    logging.warning(f" Successfully quoted cryptocurrency symbol {event['symbol']} in JSON")
+    logging.warning(f" Successfully quoted symbol {event['symbol']} in JSON")
 
 
 @pytest.mark.integration
 def test_can_quote_daily():
     event = {
         "symbol": "VZ"
     }
     daily_quote = client.get_daily_quote(event)
     assert not daily_quote.limit_reached, f"limit_reached should not be true {daily_quote.error_message}"
     assert daily_quote.success, f"success is false {daily_quote.error_message}"
     assert len(daily_quote.data), f"Did not return data for this symbol {daily_quote.symbol}"
-    logging.warning(f" Successfully quoted cryptocurrency symbol {event['symbol']} in JSON")
+    logging.warning(f" Successfully quoted symbol {event['symbol']} in JSON")
 
 
-@pytest.mark.integration
+@pytest.mark.integration_paid
 def test_can_quote_crypto():
     event = {
         "function": "CRYPTO_INTRADAY",
         "symbol": "ETH",
         "market": "USD",
         "interval": "5min"
     }
     results = client.get_crypto_intraday(event)
     assert not results.limit_reached, f"limit_reached should not be true {results.error_message}"
     assert results.success, f"success is false {results.error_message}"
     assert len(results.data), "Data{} property is empty but should have information"
     logging.warning(f" Successfully quoted cryptocurrency symbol {event['symbol']} in JSON")
 
 
-@pytest.mark.integration
+@pytest.mark.integration_paid
 def test_can_quote_crypto_csv():
     event = {
         "function": "CRYPTO_INTRADAY",
         "symbol": "ETH",
         "market": "USD",
         "interval": "5min",
         "datatype": "csv"
@@ -439,15 +450,15 @@
     }
     results = client.get_data_from_alpha_vantage(event)
     assert type(results) is dict, "Results object should be a dictionary"
     assert len(results) > 0, "There should be data in the results"
 
     logging.warning("Successfully queried data using get_data_from_alpha_vantage")
 
-@pytest.mark.integration
+@pytest.mark.integration_paid
 def test_get_fx_currency_data():
     event = {
         "function" : "CURRENCY_EXCHANGE_RATE",
         "from_currency" : "JPY",
         "to_currency" : "USD"
     }
     results = client.get_data_from_alpha_vantage(event)
```

## Comparing `alphavantage_api_client-2.2.1.dist-info/LICENSE` & `alphavantage_api_client-2.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `alphavantage_api_client-2.2.1.dist-info/RECORD` & `alphavantage_api_client-2.2.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 alphavantage_api_client/__init__.py,sha256=LjOK2KyjUSGIKm6-Ln0o5Xbre_eNBdtMdip1DshCFFU,241
 alphavantage_api_client/__main__.py,sha256=v0zu0x146Y8ll3NfbcMqX9YHz9Fe6U6iBJNAUx1CCB4,800
-alphavantage_api_client/client.py,sha256=Ej1hKXxD66yXZRk0MaF31GPC2eYpDTg_Yc7MoWen5cs,19191
-alphavantage_api_client/models.py,sha256=jKnBXtoINfds6EMdX8xBw-0mElzXGE6VTj7I3ctlxxM,7614
+alphavantage_api_client/client.py,sha256=5hqwlwcGZFCKetbRJzd3vy1LTL5pH4yumlkEdueKozU,20255
+alphavantage_api_client/models.py,sha256=B7k14QIvlRH-UeccI9W83qnZ4dNlyvDJJoiGOuK2ijk,7951
 alphavantage_api_client/response_validation_rules.py,sha256=gDQI09e6tctYGipYRDseueC2-y5QhXXetYb7JCTLfCM,7725
 alphavantage_api_client/ticker.py,sha256=rm2hEbTXSuy5OlJ614Cjo_J4kQNn2yqzTxLRh6heM-s,11793
 alphavantage_api_client/version.py,sha256=CPPPQtdj0x8RPK2m4AZHAS0xNcHBTFgGIjF6A9AkfBo,260
+examples/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+examples/getting_started.py,sha256=5VDhpBl1-OwT-Idtq-_YgomRs4v3p3tSJL1Y2NYgPF0,7031
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/mock_client.py,sha256=iUJgLwDlniyiYZ5upajRi2hwWkI8m_EKqYocFBxdv5Y,3234
+tests/mock_client.py,sha256=ph-nfsDXW7oKeWjIYko9IG7gUWGW95tUqgsv4ZGSpY8,3373
 tests/test_evaluate_company.py,sha256=4PykTBbFl2VMnNk_ci_ZKhLHJd3JLsiEdbqCOmHtec0,1948
-tests/test_mock_client_unit.py,sha256=rTMdqHmY8AdKo__Ko0Hz5Gt9xfudL1vM9CTP7Fm0Ceo,7437
-tests/test_multi_client_integration.py,sha256=TbkNlSnJPqm8xfaKVzINPSJbSJLfh9gY2uElMPvo3BA,19644
-tests/test_single_client_cache_integration.py,sha256=T65yfCdjvv7QG-6jsxi2cF2WpqN5OnaMmAQVwHV13OA,18350
+tests/test_mock_client_unit.py,sha256=mekmPYlJSwwylDXh8Kd6gjZIS4RIYGEsCq5WY1mbKh8,7788
+tests/test_multi_client_integration.py,sha256=dchlyLTWR-ni1xaV2pcG2nRjGqHsSSTnS7k9wbh-5Vs,19650
+tests/test_single_client_cache_integration.py,sha256=V7OnR7mJCRicvmMUG1W0nHgRB17yMowkooznSEGRnDM,18669
 tests/test_ticker.py,sha256=rML0QZQ-yIyoQ8ZC6fzwk794t0py8sKxc_L49x1-J_Y,2966
-alphavantage_api_client-2.2.1.dist-info/LICENSE,sha256=pqc8PsXCbEEWs5MXtWyNwJoJn2LeEvbHPtghrWzjYl8,1067
-alphavantage_api_client-2.2.1.dist-info/METADATA,sha256=jVlc4yLPub_Jzyn7-oRfEXvU0Uz9K-cBhD49KFMInyA,14247
-alphavantage_api_client-2.2.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-alphavantage_api_client-2.2.1.dist-info/top_level.txt,sha256=1xeKYpq6HidbyAHLOdd5jPALdg3qJVtDUCtx_0QeXcM,30
-alphavantage_api_client-2.2.1.dist-info/RECORD,,
+alphavantage_api_client-2.2.2.dist-info/LICENSE,sha256=pqc8PsXCbEEWs5MXtWyNwJoJn2LeEvbHPtghrWzjYl8,1067
+alphavantage_api_client-2.2.2.dist-info/METADATA,sha256=vTliJSgVg786i52L2MLYdINNavKueGhypxXl3n4AoDA,14032
+alphavantage_api_client-2.2.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+alphavantage_api_client-2.2.2.dist-info/top_level.txt,sha256=bvH2x4zTqLxAFEGVLW7WkHrZBz_hwN-nz-hfvx450IE,39
+alphavantage_api_client-2.2.2.dist-info/RECORD,,
```

