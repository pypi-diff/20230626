# Comparing `tmp/CurrencyConverter-0.8.tar.gz` & `tmp/CurrencyConverter-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/CurrencyConverter-0.8.tar", last modified: Tue May  3 15:40:11 2016, max compression
+gzip compressed data, was "dist/CurrencyConverter-0.8.1.tar", last modified: Tue May 10 09:07:48 2016, max compression
```

## Comparing `CurrencyConverter-0.8.tar` & `CurrencyConverter-0.8.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 osboxes   (1000) osboxes   (1000)        0 2016-05-03 15:40:11.000000 CurrencyConverter-0.8/
-drwxr-xr-x   0 osboxes   (1000) osboxes   (1000)        0 2016-05-03 15:40:11.000000 CurrencyConverter-0.8/CurrencyConverter.egg-info/
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)      424 2016-05-03 15:40:10.000000 CurrencyConverter-0.8/CurrencyConverter.egg-info/SOURCES.txt
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)       83 2016-05-03 15:40:10.000000 CurrencyConverter-0.8/CurrencyConverter.egg-info/entry_points.txt
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)       19 2016-05-03 15:40:10.000000 CurrencyConverter-0.8/CurrencyConverter.egg-info/top_level.txt
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)        1 2015-11-26 13:12:27.000000 CurrencyConverter-0.8/CurrencyConverter.egg-info/not-zip-safe
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)        1 2016-05-03 15:40:10.000000 CurrencyConverter-0.8/CurrencyConverter.egg-info/dependency_links.txt
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)    16392 2016-05-03 15:40:10.000000 CurrencyConverter-0.8/CurrencyConverter.egg-info/PKG-INFO
-lrwxrwxrwx   0 osboxes   (1000) osboxes   (1000)        0 2015-11-12 14:00:27.000000 CurrencyConverter-0.8/README -> README.rst
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)      888 2016-04-29 08:00:45.000000 CurrencyConverter-0.8/setup.py
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)       89 2015-11-26 13:08:35.000000 CurrencyConverter-0.8/MANIFEST.in
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)        4 2016-05-03 06:45:09.000000 CurrencyConverter-0.8/VERSION
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)    16392 2016-05-03 15:40:11.000000 CurrencyConverter-0.8/PKG-INFO
-drwxr-xr-x   0 osboxes   (1000) osboxes   (1000)        0 2016-05-03 15:40:11.000000 CurrencyConverter-0.8/currency_converter/
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)  1197390 2016-05-03 18:36:28.000000 CurrencyConverter-0.8/currency_converter/eurofxref-hist.csv
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)    11668 2016-05-03 13:38:37.000000 CurrencyConverter-0.8/currency_converter/currency_converter.py
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)       88 2016-05-02 07:25:59.000000 CurrencyConverter-0.8/currency_converter/__init__.py
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)       59 2016-05-03 15:40:11.000000 CurrencyConverter-0.8/setup.cfg
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)    11323 2015-11-12 14:00:27.000000 CurrencyConverter-0.8/LICENSE
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)      108 2016-04-29 15:45:56.000000 CurrencyConverter-0.8/AUTHORS.rst
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)     3643 2016-05-03 15:24:52.000000 CurrencyConverter-0.8/README.rst
+drwxr-xr-x   0 osboxes   (1000) osboxes   (1000)        0 2016-05-10 09:07:48.000000 CurrencyConverter-0.8.1/
+drwxr-xr-x   0 osboxes   (1000) osboxes   (1000)        0 2016-05-10 09:07:48.000000 CurrencyConverter-0.8.1/CurrencyConverter.egg-info/
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)      424 2016-05-10 09:07:48.000000 CurrencyConverter-0.8.1/CurrencyConverter.egg-info/SOURCES.txt
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)       83 2016-05-10 09:07:48.000000 CurrencyConverter-0.8.1/CurrencyConverter.egg-info/entry_points.txt
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)       19 2016-05-10 09:07:48.000000 CurrencyConverter-0.8.1/CurrencyConverter.egg-info/top_level.txt
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)        1 2015-11-26 13:12:27.000000 CurrencyConverter-0.8.1/CurrencyConverter.egg-info/not-zip-safe
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)        1 2016-05-10 09:07:48.000000 CurrencyConverter-0.8.1/CurrencyConverter.egg-info/dependency_links.txt
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)    16131 2016-05-10 09:07:48.000000 CurrencyConverter-0.8.1/CurrencyConverter.egg-info/PKG-INFO
+lrwxrwxrwx   0 osboxes   (1000) osboxes   (1000)        0 2015-11-12 14:00:27.000000 CurrencyConverter-0.8.1/README -> README.rst
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)      888 2016-04-29 08:00:45.000000 CurrencyConverter-0.8.1/setup.py
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)       89 2015-11-26 13:08:35.000000 CurrencyConverter-0.8.1/MANIFEST.in
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)        6 2016-05-10 09:07:31.000000 CurrencyConverter-0.8.1/VERSION
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)    16131 2016-05-10 09:07:48.000000 CurrencyConverter-0.8.1/PKG-INFO
+drwxr-xr-x   0 osboxes   (1000) osboxes   (1000)        0 2016-05-10 09:07:48.000000 CurrencyConverter-0.8.1/currency_converter/
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)  1198202 2016-05-06 18:32:32.000000 CurrencyConverter-0.8.1/currency_converter/eurofxref-hist.csv
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)    11934 2016-05-10 06:10:21.000000 CurrencyConverter-0.8.1/currency_converter/currency_converter.py
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)       88 2016-05-02 07:25:59.000000 CurrencyConverter-0.8.1/currency_converter/__init__.py
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)       59 2016-05-10 09:07:48.000000 CurrencyConverter-0.8.1/setup.cfg
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)    11323 2015-11-12 14:00:27.000000 CurrencyConverter-0.8.1/LICENSE
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)      108 2016-04-29 15:45:56.000000 CurrencyConverter-0.8.1/AUTHORS.rst
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)     3436 2016-05-10 06:10:21.000000 CurrencyConverter-0.8.1/README.rst
```

### Comparing `CurrencyConverter-0.8/CurrencyConverter.egg-info/PKG-INFO` & `CurrencyConverter-0.8.1/CurrencyConverter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: CurrencyConverter
-Version: 0.8
+Version: 0.8.1
 Summary: A currency converter using the European Central Bank data.
 Home-page: https://github.com/alexprengere/currencyconverter
 Author: Alex Prengère
 Author-email: alexprengere@gmail.com
 License: Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
@@ -237,22 +237,15 @@
         -----------------
         
         After installation, you should have ``currency_converter`` in your ``$PATH``:
         
         .. code-block:: bash
         
          $ currency_converter 100 USD --to EUR
-         Available currencies [42]:
-         AUD BGN BRL CAD CHF CNY CYP CZK DKK EEK
-         EUR GBP HKD HRK HUF IDR ILS INR ISK JPY
-         KRW LTL LVL MTL MXN MYR NOK NZD PHP PLN
-         ROL RON RUB SEK SGD SIT SKK THB TRL TRY
-         USD ZAR
-        
-         "100.000 USD" is "87.881 EUR" on 2016-04-20
+         100.000 USD = 87.512 EUR on 2016-05-06
         
         Python API
         ----------
         
         Create once the currency converter object:
         
         .. code-block:: python
@@ -324,15 +317,15 @@
         
         .. code-block:: python
         
             >>> first_date, last_date = c.bounds['USD']
             >>> first_date
             datetime.date(1999, 1, 4)
             >>> last_date
-            datetime.date(2016, 5, 3)
+            datetime.date(2016, 5, 6)
         
         + ``currencies`` is a set containing all available currencies
         
         .. code-block:: python
         
             >>> c.currencies # doctest: +SKIP
             set(['SGD', 'CAD', 'SEK', 'GBP', ...
```

### Comparing `CurrencyConverter-0.8/setup.py` & `CurrencyConverter-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `CurrencyConverter-0.8/PKG-INFO` & `CurrencyConverter-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: CurrencyConverter
-Version: 0.8
+Version: 0.8.1
 Summary: A currency converter using the European Central Bank data.
 Home-page: https://github.com/alexprengere/currencyconverter
 Author: Alex Prengère
 Author-email: alexprengere@gmail.com
 License: Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
@@ -237,22 +237,15 @@
         -----------------
         
         After installation, you should have ``currency_converter`` in your ``$PATH``:
         
         .. code-block:: bash
         
          $ currency_converter 100 USD --to EUR
-         Available currencies [42]:
-         AUD BGN BRL CAD CHF CNY CYP CZK DKK EEK
-         EUR GBP HKD HRK HUF IDR ILS INR ISK JPY
-         KRW LTL LVL MTL MXN MYR NOK NZD PHP PLN
-         ROL RON RUB SEK SGD SIT SKK THB TRL TRY
-         USD ZAR
-        
-         "100.000 USD" is "87.881 EUR" on 2016-04-20
+         100.000 USD = 87.512 EUR on 2016-05-06
         
         Python API
         ----------
         
         Create once the currency converter object:
         
         .. code-block:: python
@@ -324,15 +317,15 @@
         
         .. code-block:: python
         
             >>> first_date, last_date = c.bounds['USD']
             >>> first_date
             datetime.date(1999, 1, 4)
             >>> last_date
-            datetime.date(2016, 5, 3)
+            datetime.date(2016, 5, 6)
         
         + ``currencies`` is a set containing all available currencies
         
         .. code-block:: python
         
             >>> c.currencies # doctest: +SKIP
             set(['SGD', 'CAD', 'SEK', 'GBP', ...
```

### Comparing `CurrencyConverter-0.8/currency_converter/eurofxref-hist.csv` & `CurrencyConverter-0.8.1/currency_converter/eurofxref-hist.csv`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 Date,USD,JPY,BGN,CYP,CZK,DKK,EEK,GBP,HUF,LTL,LVL,MTL,PLN,ROL,RON,SEK,SIT,SKK,CHF,ISK,NOK,HRK,RUB,TRL,TRY,AUD,BRL,CAD,CNY,HKD,IDR,INR,KRW,MXN,MYR,NZD,PHP,SGD,THB,ZAR,ILS,
+2016-05-06,1.1427,122.23,1.9558,N/A,27.021,7.439,N/A,0.7885,313.68,N/A,N/A,N/A,4.4198,N/A,4.5005,9.2753,N/A,N/A,1.107,N/A,9.3513,7.502,75.9135,N/A,3.3363,1.5501,4.065,1.4717,7.43,8.8678,15276.76,76.141,1339.64,20.5185,4.5845,1.6702,53.884,1.5526,40.189,17.0959,4.3191,
+2016-05-05,1.1439,122.51,1.9558,N/A,27.028,7.4401,N/A,0.7886,312.84,N/A,N/A,N/A,4.4234,N/A,4.5035,9.2575,N/A,N/A,1.1018,N/A,9.2985,7.515,75.0559,N/A,3.3166,1.5266,4.0282,1.4665,7.441,8.8775,15260.95,76.0745,1333.95,20.2155,4.5819,1.6577,54.171,1.5531,40.191,17.0751,4.3221,
+2016-05-04,1.1505,122.62,1.9558,N/A,27.031,7.4404,N/A,0.79284,312.58,N/A,N/A,N/A,4.3936,N/A,4.492,9.263,N/A,N/A,1.0993,N/A,9.341,7.511,75.956,N/A,3.2893,1.5379,4.1091,1.467,7.4789,8.9295,15320.06,76.611,1338.14,20.4573,4.612,1.6669,54.352,1.5605,40.377,17.0072,4.3407,
 2016-05-03,1.1569,122.53,1.9558,N/A,27.037,7.4424,N/A,0.79103,311.85,N/A,N/A,N/A,4.3844,N/A,4.4879,9.2305,N/A,N/A,1.0977,N/A,9.309,7.51,76.9498,N/A,3.2718,1.5303,4.102,1.4559,7.5013,8.9769,15276.83,76.8128,1323.75,20.146,4.5735,1.6572,54.425,1.5574,40.422,16.7316,4.3376,
 2016-05-02,1.1493,122.47,1.9558,N/A,27.048,7.4414,N/A,0.78248,310.84,N/A,N/A,N/A,4.3833,N/A,4.4815,9.1803,N/A,N/A,1.0999,N/A,9.233,7.513,74.4081,N/A,3.208,1.5025,3.9731,1.4388,7.4418,8.917,15125.45,76.3185,1307.85,19.6826,4.4875,1.6368,54.068,1.541,40.076,16.3027,4.3056,
 2016-04-29,1.1403,122.34,1.9558,N/A,27.038,7.444,N/A,0.78025,312.23,N/A,N/A,N/A,4.3965,N/A,4.477,9.1689,N/A,N/A,1.0984,N/A,9.215,7.511,73.2286,N/A,3.1934,1.4948,3.9738,1.4286,7.3943,8.8466,15034.86,75.6985,1301.53,19.557,4.4546,1.6357,53.504,1.5311,39.819,16.1567,4.2666,
 2016-04-28,1.1358,122.84,1.9558,N/A,27.045,7.4432,N/A,0.77838,310.7,N/A,N/A,N/A,4.388,N/A,4.4723,9.1763,N/A,N/A,1.0974,N/A,9.246,7.48,73.5195,N/A,3.1963,1.4906,3.9907,1.4262,7.3562,8.8111,14977.23,75.531,1295.54,19.6713,4.4251,1.6287,53.309,1.5273,39.804,16.3328,4.2697,
 2016-04-27,1.1303,125.79,1.9558,N/A,27.034,7.4428,N/A,0.77475,312.12,N/A,N/A,N/A,4.3918,N/A,4.464,9.1613,N/A,N/A,1.0998,N/A,9.2013,7.4773,73.7837,N/A,3.1908,1.4885,3.9826,1.4223,7.3411,8.7671,14915.43,75.1273,1299.53,19.6578,4.4318,1.6504,52.973,1.5251,39.707,16.351,4.2542,
 2016-04-26,1.1287,125.45,1.9558,N/A,27.027,7.4418,N/A,0.77483,312.2,N/A,N/A,N/A,4.3799,N/A,4.4747,9.1545,N/A,N/A,1.1,N/A,9.2278,7.4785,74.8948,N/A,3.1951,1.46,3.9943,1.4276,7.3345,8.7545,14917.56,75.1373,1299.14,19.7889,4.4279,1.6417,52.864,1.528,39.708,16.3492,4.2484,
 2016-04-25,1.1264,124.95,1.9558,N/A,27.047,7.4418,N/A,0.7764,311.3,N/A,N/A,N/A,4.3911,N/A,4.4801,9.157,N/A,N/A,1.0973,N/A,9.2735,7.4818,74.6713,N/A,3.2074,1.4587,4.0168,1.4286,7.3145,8.7373,14864.34,75.019,1291.46,19.8036,4.3982,1.6399,52.808,1.5215,39.499,16.3141,4.2447,
```

### Comparing `CurrencyConverter-0.8/currency_converter/currency_converter.py` & `CurrencyConverter-0.8.1/currency_converter/currency_converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from __future__ import with_statement, print_function, division
 
 import sys
 import os.path as op
+from functools import wraps
 import datetime
 from datetime import timedelta
 from collections import defaultdict, namedtuple
 
 # We could have used "six", but like this we have no dependency
 if sys.version_info[0] < 3:
     range = xrange
@@ -35,14 +36,15 @@
 __all__ = ['CurrencyConverter',
            'S3CurrencyConverter',
            'RateNotFoundError', ]
 
 
 def memoize(function):
     memo = {}
+    @wraps(function)
     def wrapper(*args):
         if args not in memo:
             memo[args] = function(*args)
         return memo[args]
     return wrapper
 
 
@@ -298,57 +300,64 @@
     parser.add_argument(
         '-d', '--date',
         help='date of rate, with format %%Y-%%m-%%d',
         default=None)
 
     parser.add_argument(
         '-v', '--verbose',
-        help=('display currency bounds, use twice (-vv) to also '
-              'display details of missing rates completion'),
+        help=('display available currencies, use twice (-vv) to '
+              'also display details of missing rates completion'),
         action='count',
         default=0)
 
     parser.add_argument(
         '-f', '--file',
         help='change currency file used, default is %(default)s',
         default=CURRENCY_FILE)
 
     args = parser.parse_args()
 
     c = CurrencyConverter(currency_file=args.file,
                           fallback_on_wrong_date=True,
                           fallback_on_missing_rate=True,
                           verbose=args.verbose > 1)
+    currencies = sorted(c.currencies)
 
-    print('\n{0} available currencies (-v/-vv for details):'.format(len(c.currencies)))
-    if not args.verbose:
-        for group in grouper(sorted(c.currencies), 10, fillvalue=''):
+    if args.verbose:
+        print('{0} available currencies:'.format(len(currencies)))
+        for group in grouper(currencies, 10, fillvalue=''):
             print(' '.join(group))
+        print()
 
-    else:
-        currencies = sorted(c.currencies)
         currencies.sort(key=lambda u: c.bounds[u].last_date, reverse=True)
         currencies.sort(key=lambda u: c.bounds[u].first_date)
         for currency in currencies:
             first_date, last_date = c.bounds[currency]
             print('{0}: from {1} to {2} ({3} days)'.format(
                 currency, first_date, last_date,
                 1 + (last_date - first_date).days))
+        print()
+
+    if args.currency not in c.currencies:
+        print(r'/!\ "{0}" is not in available currencies:'.format(args.currency))
+        for group in grouper(currencies, 10, fillvalue=''):
+            print(' '.join(group))
+        exit(1)
 
     if args.date is not None:
         date = parse_date(args.date)
     else:
         date = c.bounds[args.currency].last_date
 
     new_amount = c.convert(amount=args.amount,
                            currency=args.currency,
                            new_currency=args.to,
                            date=date)
 
-    print('\n"{0:.3f} {1}" is "{2:.3f} {3}" on {4}'.format(
+    print('{0:.3f} {1} = {2:.3f} {3} on {4}'.format(
         args.amount,
         args.currency,
         new_amount,
         args.to,
         date))
```

### Comparing `CurrencyConverter-0.8/LICENSE` & `CurrencyConverter-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CurrencyConverter-0.8/README.rst` & `CurrencyConverter-0.8.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -29,22 +29,15 @@
 -----------------
 
 After installation, you should have ``currency_converter`` in your ``$PATH``:
 
 .. code-block:: bash
 
  $ currency_converter 100 USD --to EUR
- Available currencies [42]:
- AUD BGN BRL CAD CHF CNY CYP CZK DKK EEK
- EUR GBP HKD HRK HUF IDR ILS INR ISK JPY
- KRW LTL LVL MTL MXN MYR NOK NZD PHP PLN
- ROL RON RUB SEK SGD SIT SKK THB TRL TRY
- USD ZAR
-
- "100.000 USD" is "87.881 EUR" on 2016-04-20
+ 100.000 USD = 87.512 EUR on 2016-05-06
 
 Python API
 ----------
 
 Create once the currency converter object:
 
 .. code-block:: python
@@ -116,15 +109,15 @@
 
 .. code-block:: python
 
     >>> first_date, last_date = c.bounds['USD']
     >>> first_date
     datetime.date(1999, 1, 4)
     >>> last_date
-    datetime.date(2016, 5, 3)
+    datetime.date(2016, 5, 6)
 
 + ``currencies`` is a set containing all available currencies
 
 .. code-block:: python
 
     >>> c.currencies # doctest: +SKIP
     set(['SGD', 'CAD', 'SEK', 'GBP', ...
```

