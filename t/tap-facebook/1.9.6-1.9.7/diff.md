# Comparing `tmp/tap-facebook-1.9.6.tar.gz` & `tmp/tap-facebook-1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tap-facebook-1.9.6.tar", last modified: Mon Jan 25 19:01:14 2021, max compression
+gzip compressed data, was "dist/tap-facebook-1.9.7.tar", last modified: Wed Jan 27 20:38:44 2021, max compression
```

## Comparing `tap-facebook-1.9.6.tar` & `tap-facebook-1.9.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-01-25 19:01:14.000000 tap-facebook-1.9.6/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    32395 2019-10-15 19:19:51.000000 tap-facebook-1.9.6/LICENSE
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-01-25 19:01:14.000000 tap-facebook-1.9.6/tap_facebook.egg-info/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       13 2021-01-25 19:01:14.000000 tap-facebook-1.9.6/tap_facebook.egg-info/top_level.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1024 2021-01-25 19:01:14.000000 tap-facebook-1.9.6/tap_facebook.egg-info/SOURCES.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      301 2021-01-25 19:01:14.000000 tap-facebook-1.9.6/tap_facebook.egg-info/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       76 2021-01-25 19:01:14.000000 tap-facebook-1.9.6/tap_facebook.egg-info/entry_points.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2021-01-25 19:01:14.000000 tap-facebook-1.9.6/tap_facebook.egg-info/dependency_links.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      132 2021-01-25 19:01:14.000000 tap-facebook-1.9.6/tap_facebook.egg-info/requires.txt
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-01-25 19:01:14.000000 tap-facebook-1.9.6/tap_facebook/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     8064 2021-01-19 20:59:05.000000 tap-facebook-1.9.6/tap_facebook/insights_experiment.py
--rwxrwxr-x   0 vagrant   (1000) vagrant   (1000)    28947 2021-01-25 18:11:47.000000 tap-facebook-1.9.6/tap_facebook/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     3020 2021-01-19 19:10:03.000000 tap-facebook-1.9.6/tap_facebook/process_output.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-01-25 19:01:14.000000 tap-facebook-1.9.6/tap_facebook/schemas/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     6168 2021-01-19 20:59:05.000000 tap-facebook-1.9.6/tap_facebook/schemas/ads_insights_platform_and_device.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5929 2021-01-19 20:59:05.000000 tap-facebook-1.9.6/tap_facebook/schemas/ads_insights_age_and_gender.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5811 2021-01-19 20:59:05.000000 tap-facebook-1.9.6/tap_facebook/schemas/ads_insights.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5891 2021-01-19 20:59:05.000000 tap-facebook-1.9.6/tap_facebook/schemas/ads_insights_region.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1661 2021-01-19 19:10:03.000000 tap-facebook-1.9.6/tap_facebook/schemas/campaigns.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4436 2021-01-19 20:59:05.000000 tap-facebook-1.9.6/tap_facebook/schemas/ads_insights_dma.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     3730 2021-01-19 19:10:03.000000 tap-facebook-1.9.6/tap_facebook/schemas/adsets.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    16588 2021-01-19 19:10:03.000000 tap-facebook-1.9.6/tap_facebook/schemas/ads.json
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-01-25 19:01:14.000000 tap-facebook-1.9.6/tap_facebook/schemas/shared/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      428 2021-01-19 20:59:05.000000 tap-facebook-1.9.6/tap_facebook/schemas/shared/ads_histogram_stats.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4688 2021-01-19 19:10:03.000000 tap-facebook-1.9.6/tap_facebook/schemas/shared/geo_locations.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1983 2021-01-19 19:10:03.000000 tap-facebook-1.9.6/tap_facebook/schemas/shared/ads_image_crops.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1094 2021-01-19 19:10:03.000000 tap-facebook-1.9.6/tap_facebook/schemas/shared/ads_action_stats.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     8313 2021-01-19 19:10:03.000000 tap-facebook-1.9.6/tap_facebook/schemas/shared/targeting.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    36189 2021-01-19 19:10:03.000000 tap-facebook-1.9.6/tap_facebook/schemas/adcreative.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5892 2021-01-19 20:59:05.000000 tap-facebook-1.9.6/tap_facebook/schemas/ads_insights_country.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      301 2021-01-25 19:01:14.000000 tap-facebook-1.9.6/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       95 2021-01-19 19:10:03.000000 tap-facebook-1.9.6/MANIFEST.in
--rwxrwxr-x   0 vagrant   (1000) vagrant   (1000)     1045 2021-01-25 18:53:23.000000 tap-facebook-1.9.6/setup.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       79 2021-01-25 19:01:14.000000 tap-facebook-1.9.6/setup.cfg
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2710 2021-01-19 19:10:03.000000 tap-facebook-1.9.6/README.md
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-01-27 20:38:44.000000 tap-facebook-1.9.7/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    32395 2019-10-15 19:19:51.000000 tap-facebook-1.9.7/LICENSE
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-01-27 20:38:44.000000 tap-facebook-1.9.7/tap_facebook.egg-info/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       13 2021-01-27 20:38:44.000000 tap-facebook-1.9.7/tap_facebook.egg-info/top_level.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1024 2021-01-27 20:38:44.000000 tap-facebook-1.9.7/tap_facebook.egg-info/SOURCES.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      301 2021-01-27 20:38:44.000000 tap-facebook-1.9.7/tap_facebook.egg-info/PKG-INFO
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       76 2021-01-27 20:38:44.000000 tap-facebook-1.9.7/tap_facebook.egg-info/entry_points.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2021-01-27 20:38:44.000000 tap-facebook-1.9.7/tap_facebook.egg-info/dependency_links.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      132 2021-01-27 20:38:44.000000 tap-facebook-1.9.7/tap_facebook.egg-info/requires.txt
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-01-27 20:38:44.000000 tap-facebook-1.9.7/tap_facebook/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     8064 2021-01-19 20:59:05.000000 tap-facebook-1.9.7/tap_facebook/insights_experiment.py
+-rwxrwxr-x   0 vagrant   (1000) vagrant   (1000)    29261 2021-01-27 19:23:08.000000 tap-facebook-1.9.7/tap_facebook/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     3020 2021-01-19 19:10:03.000000 tap-facebook-1.9.7/tap_facebook/process_output.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-01-27 20:38:44.000000 tap-facebook-1.9.7/tap_facebook/schemas/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     6168 2021-01-19 20:59:05.000000 tap-facebook-1.9.7/tap_facebook/schemas/ads_insights_platform_and_device.json
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5929 2021-01-19 20:59:05.000000 tap-facebook-1.9.7/tap_facebook/schemas/ads_insights_age_and_gender.json
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5811 2021-01-19 20:59:05.000000 tap-facebook-1.9.7/tap_facebook/schemas/ads_insights.json
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5891 2021-01-19 20:59:05.000000 tap-facebook-1.9.7/tap_facebook/schemas/ads_insights_region.json
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1661 2021-01-19 19:10:03.000000 tap-facebook-1.9.7/tap_facebook/schemas/campaigns.json
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4436 2021-01-19 20:59:05.000000 tap-facebook-1.9.7/tap_facebook/schemas/ads_insights_dma.json
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     3730 2021-01-19 19:10:03.000000 tap-facebook-1.9.7/tap_facebook/schemas/adsets.json
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    16588 2021-01-19 19:10:03.000000 tap-facebook-1.9.7/tap_facebook/schemas/ads.json
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-01-27 20:38:44.000000 tap-facebook-1.9.7/tap_facebook/schemas/shared/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      428 2021-01-19 20:59:05.000000 tap-facebook-1.9.7/tap_facebook/schemas/shared/ads_histogram_stats.json
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4688 2021-01-19 19:10:03.000000 tap-facebook-1.9.7/tap_facebook/schemas/shared/geo_locations.json
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1983 2021-01-19 19:10:03.000000 tap-facebook-1.9.7/tap_facebook/schemas/shared/ads_image_crops.json
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1094 2021-01-19 19:10:03.000000 tap-facebook-1.9.7/tap_facebook/schemas/shared/ads_action_stats.json
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     8313 2021-01-19 19:10:03.000000 tap-facebook-1.9.7/tap_facebook/schemas/shared/targeting.json
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    36189 2021-01-19 19:10:03.000000 tap-facebook-1.9.7/tap_facebook/schemas/adcreative.json
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5892 2021-01-19 20:59:05.000000 tap-facebook-1.9.7/tap_facebook/schemas/ads_insights_country.json
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      301 2021-01-27 20:38:44.000000 tap-facebook-1.9.7/PKG-INFO
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       95 2021-01-19 19:10:03.000000 tap-facebook-1.9.7/MANIFEST.in
+-rwxrwxr-x   0 vagrant   (1000) vagrant   (1000)     1045 2021-01-27 20:37:47.000000 tap-facebook-1.9.7/setup.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       79 2021-01-27 20:38:44.000000 tap-facebook-1.9.7/setup.cfg
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2710 2021-01-19 19:10:03.000000 tap-facebook-1.9.7/README.md
```

### Comparing `tap-facebook-1.9.6/LICENSE` & `tap-facebook-1.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-facebook-1.9.6/tap_facebook.egg-info/SOURCES.txt` & `tap-facebook-1.9.7/tap_facebook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tap-facebook-1.9.6/tap_facebook/insights_experiment.py` & `tap-facebook-1.9.7/tap_facebook/insights_experiment.py`

 * *Files identical despite different names*

### Comparing `tap-facebook-1.9.6/tap_facebook/__init__.py` & `tap-facebook-1.9.7/tap_facebook/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,21 +114,25 @@
     def log_retry_attempt(details):
         _, exception, _ = sys.exc_info()
         LOGGER.info(exception)
         LOGGER.info('Caught retryable error after %s tries. Waiting %s more seconds then retrying...',
                     details["tries"],
                     details["wait"])
 
+        if isinstance(exception, TypeError) and str(exception) == "string indices must be integers":
+            LOGGER.info('TypeError due to bad JSON response')
     def should_retry_api_error(exception):
         if isinstance(exception, FacebookBadObjectError):
             return True
         elif isinstance(exception, FacebookRequestError):
             return exception.api_transient_error() or exception.api_error_subcode() == 99 or exception.http_status() == 500
         elif isinstance(exception, InsightsJobTimeout):
             return True
+        elif isinstance(exception, TypeError) and str(exception) == "string indices must be integers":
+            return True
         return False
 
     return backoff.on_exception(
         backoff_type,
         exception,
         jitter=None,
         on_backoff=log_retry_attempt,
@@ -218,15 +222,15 @@
     '''
 
     field_class = adcreative.AdCreative.Field
     key_properties = ['id']
 
 
     def sync(self):
-        @retry_pattern(backoff.expo, FacebookRequestError, max_tries=5, factor=5)
+        @retry_pattern(backoff.expo, (FacebookRequestError, TypeError), max_tries=5, factor=5)
         def do_request():
             return self.account.get_ad_creatives(params={'limit': RESULT_RETURN_LIMIT})
 
         ad_creative = do_request()
 
         # Create the initial batch
         api_batch = API.new_batch()
@@ -493,15 +497,15 @@
                 'time_increment': self.time_increment,
                 'action_attribution_windows': list(self.action_attribution_windows),
                 'time_ranges': [{'since': buffered_start_date.to_date_string(),
                                  'until': buffered_start_date.to_date_string()}]
             }
             buffered_start_date = buffered_start_date.add(days=1)
 
-    @retry_pattern(backoff.expo, (FacebookRequestError, InsightsJobTimeout, FacebookBadObjectError), max_tries=5, factor=5)
+    @retry_pattern(backoff.expo, (FacebookRequestError, InsightsJobTimeout, FacebookBadObjectError, TypeError), max_tries=5, factor=5)
     def run_job(self, params):
         LOGGER.info('Starting adsinsights job with params %s', params)
         job = self.account.get_insights( # pylint: disable=no-member
             params=params,
             is_async=True)
         status = None
         time_start = time.time()
```

### Comparing `tap-facebook-1.9.6/tap_facebook/process_output.py` & `tap-facebook-1.9.7/tap_facebook/process_output.py`

 * *Files identical despite different names*

### Comparing `tap-facebook-1.9.6/tap_facebook/schemas/ads_insights_platform_and_device.json` & `tap-facebook-1.9.7/tap_facebook/schemas/ads_insights_platform_and_device.json`

 * *Files identical despite different names*

### Comparing `tap-facebook-1.9.6/tap_facebook/schemas/ads_insights_age_and_gender.json` & `tap-facebook-1.9.7/tap_facebook/schemas/ads_insights_age_and_gender.json`

 * *Files identical despite different names*

### Comparing `tap-facebook-1.9.6/tap_facebook/schemas/ads_insights.json` & `tap-facebook-1.9.7/tap_facebook/schemas/ads_insights.json`

 * *Files identical despite different names*

### Comparing `tap-facebook-1.9.6/tap_facebook/schemas/ads_insights_region.json` & `tap-facebook-1.9.7/tap_facebook/schemas/ads_insights_region.json`

 * *Files identical despite different names*

### Comparing `tap-facebook-1.9.6/tap_facebook/schemas/campaigns.json` & `tap-facebook-1.9.7/tap_facebook/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `tap-facebook-1.9.6/tap_facebook/schemas/ads_insights_dma.json` & `tap-facebook-1.9.7/tap_facebook/schemas/ads_insights_dma.json`

 * *Files identical despite different names*

### Comparing `tap-facebook-1.9.6/tap_facebook/schemas/adsets.json` & `tap-facebook-1.9.7/tap_facebook/schemas/adsets.json`

 * *Files identical despite different names*

### Comparing `tap-facebook-1.9.6/tap_facebook/schemas/ads.json` & `tap-facebook-1.9.7/tap_facebook/schemas/ads.json`

 * *Files identical despite different names*

### Comparing `tap-facebook-1.9.6/tap_facebook/schemas/shared/geo_locations.json` & `tap-facebook-1.9.7/tap_facebook/schemas/shared/geo_locations.json`

 * *Files identical despite different names*

### Comparing `tap-facebook-1.9.6/tap_facebook/schemas/shared/ads_image_crops.json` & `tap-facebook-1.9.7/tap_facebook/schemas/shared/ads_image_crops.json`

 * *Files identical despite different names*

### Comparing `tap-facebook-1.9.6/tap_facebook/schemas/shared/ads_action_stats.json` & `tap-facebook-1.9.7/tap_facebook/schemas/shared/ads_action_stats.json`

 * *Files identical despite different names*

### Comparing `tap-facebook-1.9.6/tap_facebook/schemas/shared/targeting.json` & `tap-facebook-1.9.7/tap_facebook/schemas/shared/targeting.json`

 * *Files identical despite different names*

### Comparing `tap-facebook-1.9.6/tap_facebook/schemas/adcreative.json` & `tap-facebook-1.9.7/tap_facebook/schemas/adcreative.json`

 * *Files identical despite different names*

### Comparing `tap-facebook-1.9.6/tap_facebook/schemas/ads_insights_country.json` & `tap-facebook-1.9.7/tap_facebook/schemas/ads_insights_country.json`

 * *Files identical despite different names*

### Comparing `tap-facebook-1.9.6/setup.py` & `tap-facebook-1.9.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(name='tap-facebook',
-      version='1.9.6',
+      version='1.9.7',
       description='Singer.io tap for extracting data from the Facebook Ads API',
       author='Stitch',
       url='https://singer.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_facebook'],
       install_requires=[
           'attrs==16.3.0',
```

### Comparing `tap-facebook-1.9.6/README.md` & `tap-facebook-1.9.7/README.md`

 * *Files identical despite different names*

