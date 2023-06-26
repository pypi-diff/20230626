# Comparing `tmp/alphavantage_api_client-2.2.2-py3-none-any.whl.zip` & `tmp/alphavantage_api_client-2.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 29088 bytes, number of entries: 21
+Zip file size: 29080 bytes, number of entries: 21
 -rw-rw-r--  2.0 unx      241 b- defN 23-May-30 16:40 alphavantage_api_client/__init__.py
 -rw-rw-r--  2.0 unx      800 b- defN 22-Jul-02 20:13 alphavantage_api_client/__main__.py
 -rw-rw-r--  2.0 unx    20255 b- defN 23-Jun-26 17:01 alphavantage_api_client/client.py
 -rw-rw-r--  2.0 unx     7951 b- defN 23-Jun-26 17:01 alphavantage_api_client/models.py
 -rw-rw-r--  2.0 unx     7725 b- defN 22-Sep-01 17:05 alphavantage_api_client/response_validation_rules.py
 -rw-rw-r--  2.0 unx    11793 b- defN 22-Jul-27 01:15 alphavantage_api_client/ticker.py
 -rw-rw-r--  2.0 unx      260 b- defN 22-May-21 19:54 alphavantage_api_client/version.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-26 17:01 examples/__init__.py
 -rw-rw-r--  2.0 unx     7031 b- defN 23-Jun-26 17:01 examples/getting_started.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Jun-30 16:06 tests/__init__.py
 -rw-rw-r--  2.0 unx     3373 b- defN 23-Jun-26 13:20 tests/mock_client.py
 -rw-rw-r--  2.0 unx     1948 b- defN 22-Sep-01 17:05 tests/test_evaluate_company.py
 -rw-rw-r--  2.0 unx     7788 b- defN 23-Jun-26 13:20 tests/test_mock_client_unit.py
--rw-rw-r--  2.0 unx    19650 b- defN 23-Jun-26 13:20 tests/test_multi_client_integration.py
--rw-rw-r--  2.0 unx    18669 b- defN 23-Jun-26 13:20 tests/test_single_client_cache_integration.py
+-rw-rw-r--  2.0 unx    19650 b- defN 23-Jun-26 18:00 tests/test_multi_client_integration.py
+-rw-rw-r--  2.0 unx    18640 b- defN 23-Jun-26 18:08 tests/test_single_client_cache_integration.py
 -rw-rw-r--  2.0 unx     2966 b- defN 22-Jul-27 01:15 tests/test_ticker.py
--rw-rw-r--  2.0 unx     1067 b- defN 23-Jun-26 17:18 alphavantage_api_client-2.2.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx    14032 b- defN 23-Jun-26 17:18 alphavantage_api_client-2.2.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-26 17:18 alphavantage_api_client-2.2.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       39 b- defN 23-Jun-26 17:18 alphavantage_api_client-2.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1876 b- defN 23-Jun-26 17:18 alphavantage_api_client-2.2.2.dist-info/RECORD
-21 files, 127556 bytes uncompressed, 25988 bytes compressed:  79.6%
+-rw-rw-r--  2.0 unx     1067 b- defN 23-Jun-26 18:11 alphavantage_api_client-2.2.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    14032 b- defN 23-Jun-26 18:11 alphavantage_api_client-2.2.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-26 18:11 alphavantage_api_client-2.2.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       39 b- defN 23-Jun-26 18:11 alphavantage_api_client-2.2.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1876 b- defN 23-Jun-26 18:11 alphavantage_api_client-2.2.3.dist-info/RECORD
+21 files, 127527 bytes uncompressed, 25980 bytes compressed:  79.6%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: tests/test_single_client_cache_integration.py
 Comment: 
 
 Filename: tests/test_ticker.py
 Comment: 
 
-Filename: alphavantage_api_client-2.2.2.dist-info/LICENSE
+Filename: alphavantage_api_client-2.2.3.dist-info/LICENSE
 Comment: 
 
-Filename: alphavantage_api_client-2.2.2.dist-info/METADATA
+Filename: alphavantage_api_client-2.2.3.dist-info/METADATA
 Comment: 
 
-Filename: alphavantage_api_client-2.2.2.dist-info/WHEEL
+Filename: alphavantage_api_client-2.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: alphavantage_api_client-2.2.2.dist-info/top_level.txt
+Filename: alphavantage_api_client-2.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: alphavantage_api_client-2.2.2.dist-info/RECORD
+Filename: alphavantage_api_client-2.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tests/test_multi_client_integration.py

 * *Ordering differences only*

```diff
@@ -154,29 +154,29 @@
 
     assert limit_reached, "Failed to reach limit"
     assert results.symbol == event['symbol'], f" Expected symbol doesn't match given: {event.get('symbol', None)}"
 
     logging.warning(f" Can Reach Limit while quoting for symbol {event.get('symbol', None)} in JSON")
 
 
-@pytest.mark.integration_paid
+@pytest.mark.integration
 def test_can_quote_intraday():
     event = {
         "symbol": "TSLA",
         "interval": "5min"
     }
     client = AlphavantageClient().should_retry_once()
     intra_day_quote = client.get_intraday_quote(event)
     assert not intra_day_quote.limit_reached, f"limit_reached should not be true {intra_day_quote.error_message}"
     assert intra_day_quote.success, f"success is false {intra_day_quote.error_message}"
     assert len(intra_day_quote.data), f"Did not return data for this symbol {intra_day_quote.symbol}"
     logging.warning(f" Successfully quoted cryptocurrency symbol {event['symbol']} in JSON")
 
 
-@pytest.mark.integration
+@pytest.mark.integration_paid
 def test_can_quote_daily():
     event = {
         "symbol": "VZ"
     }
     client = AlphavantageClient().should_retry_once()
     daily_quote = client.get_daily_quote(event)
     print(daily_quote.json())
```

## tests/test_single_client_cache_integration.py

```diff
@@ -5,15 +5,14 @@
 import json
 
 client = AlphavantageClient().should_retry_once().use_simple_cache()
 
 
 @pytest.mark.integration
 def test_can_get_news_and_sentiment():
-    client = AlphavantageClient()
     event = {
         "function" : "NEWS_SENTIMENT",
         "tickers": "TSLA"
     }
     result = client.get_data_from_alpha_vantage(event)
     print(json.dumps(result))
     assert result['success'], 'could not get news and sentiment'
@@ -159,15 +158,15 @@
     intra_day_quote = client.get_intraday_quote(event)
     assert not intra_day_quote.limit_reached, f"limit_reached should not be true {intra_day_quote.error_message}"
     assert intra_day_quote.success, f"success is false {intra_day_quote.error_message}"
     assert len(intra_day_quote.data), f"Did not return data for this symbol {intra_day_quote.symbol}"
     logging.warning(f" Successfully quoted symbol {event['symbol']} in JSON")
 
 
-@pytest.mark.integration
+@pytest.mark.integration_paid
 def test_can_quote_daily():
     event = {
         "symbol": "VZ"
     }
     daily_quote = client.get_daily_quote(event)
     assert not daily_quote.limit_reached, f"limit_reached should not be true {daily_quote.error_message}"
     assert daily_quote.success, f"success is false {daily_quote.error_message}"
```

## Comparing `alphavantage_api_client-2.2.2.dist-info/LICENSE` & `alphavantage_api_client-2.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `alphavantage_api_client-2.2.2.dist-info/METADATA` & `alphavantage_api_client-2.2.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphavantage-api-client
-Version: 2.2.2
+Version: 2.2.3
 Summary: Interact with Alphavantage REST API
 Home-page: https://github.com/xrgarcia/alphavantage-api-client
 Author: Slashbin, LLC
 Author-email: support@slashbin.us
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `alphavantage_api_client-2.2.2.dist-info/RECORD` & `alphavantage_api_client-2.2.3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 alphavantage_api_client/version.py,sha256=CPPPQtdj0x8RPK2m4AZHAS0xNcHBTFgGIjF6A9AkfBo,260
 examples/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 examples/getting_started.py,sha256=5VDhpBl1-OwT-Idtq-_YgomRs4v3p3tSJL1Y2NYgPF0,7031
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/mock_client.py,sha256=ph-nfsDXW7oKeWjIYko9IG7gUWGW95tUqgsv4ZGSpY8,3373
 tests/test_evaluate_company.py,sha256=4PykTBbFl2VMnNk_ci_ZKhLHJd3JLsiEdbqCOmHtec0,1948
 tests/test_mock_client_unit.py,sha256=mekmPYlJSwwylDXh8Kd6gjZIS4RIYGEsCq5WY1mbKh8,7788
-tests/test_multi_client_integration.py,sha256=dchlyLTWR-ni1xaV2pcG2nRjGqHsSSTnS7k9wbh-5Vs,19650
-tests/test_single_client_cache_integration.py,sha256=V7OnR7mJCRicvmMUG1W0nHgRB17yMowkooznSEGRnDM,18669
+tests/test_multi_client_integration.py,sha256=oeoYJ1CXFlVpLjIU7-UY7shbso4x38wNOBpmx_9Sq_Q,19650
+tests/test_single_client_cache_integration.py,sha256=D2Sabn2P4uHVZu2AMINYN-Vw2xWvMDermBOojhWBoiU,18640
 tests/test_ticker.py,sha256=rML0QZQ-yIyoQ8ZC6fzwk794t0py8sKxc_L49x1-J_Y,2966
-alphavantage_api_client-2.2.2.dist-info/LICENSE,sha256=pqc8PsXCbEEWs5MXtWyNwJoJn2LeEvbHPtghrWzjYl8,1067
-alphavantage_api_client-2.2.2.dist-info/METADATA,sha256=vTliJSgVg786i52L2MLYdINNavKueGhypxXl3n4AoDA,14032
-alphavantage_api_client-2.2.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-alphavantage_api_client-2.2.2.dist-info/top_level.txt,sha256=bvH2x4zTqLxAFEGVLW7WkHrZBz_hwN-nz-hfvx450IE,39
-alphavantage_api_client-2.2.2.dist-info/RECORD,,
+alphavantage_api_client-2.2.3.dist-info/LICENSE,sha256=pqc8PsXCbEEWs5MXtWyNwJoJn2LeEvbHPtghrWzjYl8,1067
+alphavantage_api_client-2.2.3.dist-info/METADATA,sha256=YpZ1dfPkXqHzotncjG_HzPlL8wR10B0FQHR-53yQ3ts,14032
+alphavantage_api_client-2.2.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+alphavantage_api_client-2.2.3.dist-info/top_level.txt,sha256=bvH2x4zTqLxAFEGVLW7WkHrZBz_hwN-nz-hfvx450IE,39
+alphavantage_api_client-2.2.3.dist-info/RECORD,,
```

