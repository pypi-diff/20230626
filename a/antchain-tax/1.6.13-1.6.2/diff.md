# Comparing `tmp/antchain_tax-1.6.13.tar.gz` & `tmp/antchain_tax-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_tax-1.6.13.tar", last modified: Mon Jun 26 06:08:13 2023, max compression
+gzip compressed data, was "dist/antchain_tax-1.6.2.tar", last modified: Tue Aug 30 02:25:10 2022, max compression
```

## Comparing `antchain_tax-1.6.13.tar` & `antchain_tax-1.6.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 06:08:13.000000 antchain_tax-1.6.13/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-26 06:08:12.000000 antchain_tax-1.6.13/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-26 06:08:12.000000 antchain_tax-1.6.13/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2163 2023-06-26 06:08:13.000000 antchain_tax-1.6.13/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2023-06-26 06:08:12.000000 antchain_tax-1.6.13/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      990 2023-06-26 06:08:12.000000 antchain_tax-1.6.13/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 06:08:13.000000 antchain_tax-1.6.13/antchain_sdk_tax/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-26 06:08:12.000000 antchain_tax-1.6.13/antchain_sdk_tax/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58384 2023-06-26 06:08:12.000000 antchain_tax-1.6.13/antchain_sdk_tax/client.py
--rw-r--r--   0 root         (0) root         (0)   160605 2023-06-26 06:08:12.000000 antchain_tax-1.6.13/antchain_sdk_tax/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 06:08:13.000000 antchain_tax-1.6.13/antchain_tax.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2163 2023-06-26 06:08:13.000000 antchain_tax-1.6.13/antchain_tax.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      323 2023-06-26 06:08:13.000000 antchain_tax-1.6.13/antchain_tax.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 06:08:13.000000 antchain_tax-1.6.13/antchain_tax.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-26 06:08:13.000000 antchain_tax-1.6.13/antchain_tax.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-26 06:08:13.000000 antchain_tax-1.6.13/antchain_tax.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-26 06:08:13.000000 antchain_tax-1.6.13/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2488 2023-06-26 06:08:12.000000 antchain_tax-1.6.13/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-30 02:25:10.000000 antchain_tax-1.6.2/
+-rw-r--r--   0 root         (0) root         (0)      600 2022-08-30 02:25:09.000000 antchain_tax-1.6.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-08-30 02:25:09.000000 antchain_tax-1.6.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2162 2022-08-30 02:25:10.000000 antchain_tax-1.6.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2022-08-30 02:25:09.000000 antchain_tax-1.6.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      990 2022-08-30 02:25:09.000000 antchain_tax-1.6.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-30 02:25:10.000000 antchain_tax-1.6.2/antchain_sdk_tax/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-08-30 02:25:09.000000 antchain_tax-1.6.2/antchain_sdk_tax/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47556 2022-08-30 02:25:09.000000 antchain_tax-1.6.2/antchain_sdk_tax/client.py
+-rw-r--r--   0 root         (0) root         (0)   130518 2022-08-30 02:25:09.000000 antchain_tax-1.6.2/antchain_sdk_tax/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-30 02:25:10.000000 antchain_tax-1.6.2/antchain_tax.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2162 2022-08-30 02:25:10.000000 antchain_tax-1.6.2/antchain_tax.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      323 2022-08-30 02:25:10.000000 antchain_tax-1.6.2/antchain_tax.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-30 02:25:10.000000 antchain_tax-1.6.2/antchain_tax.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2022-08-30 02:25:10.000000 antchain_tax-1.6.2/antchain_tax.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2022-08-30 02:25:10.000000 antchain_tax-1.6.2/antchain_tax.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-08-30 02:25:10.000000 antchain_tax-1.6.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2488 2022-08-30 02:25:09.000000 antchain_tax-1.6.2/setup.py
```

### Comparing `antchain_tax-1.6.13/LICENSE` & `antchain_tax-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_tax-1.6.13/PKG-INFO` & `antchain_tax-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_tax
-Version: 1.6.13
+Version: 1.6.2
 Summary: Ant Chain TAX SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_tax-1.6.13/README-CN.md` & `antchain_tax-1.6.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_tax-1.6.13/README.md` & `antchain_tax-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `antchain_tax-1.6.13/antchain_sdk_tax/client.py` & `antchain_tax-1.6.2/antchain_sdk_tax/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDuration': self._keep_alive_duration_millis,
+            'keepAliveDurationMillis': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.6.13',
+                    'sdk_version': '1.6.2',
                     '_prod_code': 'TAX',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -198,15 +198,15 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDuration': self._keep_alive_duration_millis,
+            'keepAliveDurationMillis': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.6.13',
+                    'sdk_version': '1.6.2',
                     '_prod_code': 'TAX',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -1060,58 +1060,58 @@
         )
 
     def auth_icm_enterprise(
         self,
         request: tax_models.AuthIcmEnterpriseRequest,
     ) -> tax_models.AuthIcmEnterpriseResponse:
         """
-        Description: 授权接口
-        Summary: 授权
+        Description: 企业的授权接口
+        Summary: 企业授权
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.auth_icm_enterprise_ex(request, headers, runtime)
 
     async def auth_icm_enterprise_async(
         self,
         request: tax_models.AuthIcmEnterpriseRequest,
     ) -> tax_models.AuthIcmEnterpriseResponse:
         """
-        Description: 授权接口
-        Summary: 授权
+        Description: 企业的授权接口
+        Summary: 企业授权
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.auth_icm_enterprise_ex_async(request, headers, runtime)
 
     def auth_icm_enterprise_ex(
         self,
         request: tax_models.AuthIcmEnterpriseRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> tax_models.AuthIcmEnterpriseResponse:
         """
-        Description: 授权接口
-        Summary: 授权
+        Description: 企业的授权接口
+        Summary: 企业授权
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             tax_models.AuthIcmEnterpriseResponse(),
             self.do_request('1.0', 'blockchain.tax.icm.enterprise.auth', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def auth_icm_enterprise_ex_async(
         self,
         request: tax_models.AuthIcmEnterpriseRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> tax_models.AuthIcmEnterpriseResponse:
         """
-        Description: 授权接口
-        Summary: 授权
+        Description: 企业的授权接口
+        Summary: 企业授权
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             tax_models.AuthIcmEnterpriseResponse(),
             await self.do_request_async('1.0', 'blockchain.tax.icm.enterprise.auth', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
@@ -1166,287 +1166,7 @@
         Summary: 可信授权链接获取接口
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             tax_models.CreateApiAuthurlResponse(),
             await self.do_request_async('1.0', 'blockchain.tax.api.authurl.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
-
-    def match_icm_simpleauth(
-        self,
-        request: tax_models.MatchIcmSimpleauthRequest,
-    ) -> tax_models.MatchIcmSimpleauthResponse:
-        """
-        Description: 极简授权-检查数据是否支持接口，检查是否在白名单中的接口
-        Summary: 极简授权-检查数据是否支持接口
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.match_icm_simpleauth_ex(request, headers, runtime)
-
-    async def match_icm_simpleauth_async(
-        self,
-        request: tax_models.MatchIcmSimpleauthRequest,
-    ) -> tax_models.MatchIcmSimpleauthResponse:
-        """
-        Description: 极简授权-检查数据是否支持接口，检查是否在白名单中的接口
-        Summary: 极简授权-检查数据是否支持接口
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.match_icm_simpleauth_ex_async(request, headers, runtime)
-
-    def match_icm_simpleauth_ex(
-        self,
-        request: tax_models.MatchIcmSimpleauthRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> tax_models.MatchIcmSimpleauthResponse:
-        """
-        Description: 极简授权-检查数据是否支持接口，检查是否在白名单中的接口
-        Summary: 极简授权-检查数据是否支持接口
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            tax_models.MatchIcmSimpleauthResponse(),
-            self.do_request('1.0', 'blockchain.tax.icm.simpleauth.match', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def match_icm_simpleauth_ex_async(
-        self,
-        request: tax_models.MatchIcmSimpleauthRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> tax_models.MatchIcmSimpleauthResponse:
-        """
-        Description: 极简授权-检查数据是否支持接口，检查是否在白名单中的接口
-        Summary: 极简授权-检查数据是否支持接口
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            tax_models.MatchIcmSimpleauthResponse(),
-            await self.do_request_async('1.0', 'blockchain.tax.icm.simpleauth.match', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    def query_icm_simpleauth(
-        self,
-        request: tax_models.QueryIcmSimpleauthRequest,
-    ) -> tax_models.QueryIcmSimpleauthResponse:
-        """
-        Description: 极简授权-获取数据，用于获取指标类的数据
-        Summary: 极简授权-获取数据
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.query_icm_simpleauth_ex(request, headers, runtime)
-
-    async def query_icm_simpleauth_async(
-        self,
-        request: tax_models.QueryIcmSimpleauthRequest,
-    ) -> tax_models.QueryIcmSimpleauthResponse:
-        """
-        Description: 极简授权-获取数据，用于获取指标类的数据
-        Summary: 极简授权-获取数据
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.query_icm_simpleauth_ex_async(request, headers, runtime)
-
-    def query_icm_simpleauth_ex(
-        self,
-        request: tax_models.QueryIcmSimpleauthRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> tax_models.QueryIcmSimpleauthResponse:
-        """
-        Description: 极简授权-获取数据，用于获取指标类的数据
-        Summary: 极简授权-获取数据
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            tax_models.QueryIcmSimpleauthResponse(),
-            self.do_request('1.0', 'blockchain.tax.icm.simpleauth.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def query_icm_simpleauth_ex_async(
-        self,
-        request: tax_models.QueryIcmSimpleauthRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> tax_models.QueryIcmSimpleauthResponse:
-        """
-        Description: 极简授权-获取数据，用于获取指标类的数据
-        Summary: 极简授权-获取数据
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            tax_models.QueryIcmSimpleauthResponse(),
-            await self.do_request_async('1.0', 'blockchain.tax.icm.simpleauth.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    def query_api_simpleauthasync(
-        self,
-        request: tax_models.QueryApiSimpleauthasyncRequest,
-    ) -> tax_models.QueryApiSimpleauthasyncResponse:
-        """
-        Description: 极简授权异步查询接口
-        Summary: 极简授权-异步获取数据
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.query_api_simpleauthasync_ex(request, headers, runtime)
-
-    async def query_api_simpleauthasync_async(
-        self,
-        request: tax_models.QueryApiSimpleauthasyncRequest,
-    ) -> tax_models.QueryApiSimpleauthasyncResponse:
-        """
-        Description: 极简授权异步查询接口
-        Summary: 极简授权-异步获取数据
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.query_api_simpleauthasync_ex_async(request, headers, runtime)
-
-    def query_api_simpleauthasync_ex(
-        self,
-        request: tax_models.QueryApiSimpleauthasyncRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> tax_models.QueryApiSimpleauthasyncResponse:
-        """
-        Description: 极简授权异步查询接口
-        Summary: 极简授权-异步获取数据
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            tax_models.QueryApiSimpleauthasyncResponse(),
-            self.do_request('1.0', 'blockchain.tax.api.simpleauthasync.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def query_api_simpleauthasync_ex_async(
-        self,
-        request: tax_models.QueryApiSimpleauthasyncRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> tax_models.QueryApiSimpleauthasyncResponse:
-        """
-        Description: 极简授权异步查询接口
-        Summary: 极简授权-异步获取数据
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            tax_models.QueryApiSimpleauthasyncResponse(),
-            await self.do_request_async('1.0', 'blockchain.tax.api.simpleauthasync.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    def auth_risk_evaluation(
-        self,
-        request: tax_models.AuthRiskEvaluationRequest,
-    ) -> tax_models.AuthRiskEvaluationResponse:
-        """
-        Description: 授权接口
-        Summary: 授权接口
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.auth_risk_evaluation_ex(request, headers, runtime)
-
-    async def auth_risk_evaluation_async(
-        self,
-        request: tax_models.AuthRiskEvaluationRequest,
-    ) -> tax_models.AuthRiskEvaluationResponse:
-        """
-        Description: 授权接口
-        Summary: 授权接口
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.auth_risk_evaluation_ex_async(request, headers, runtime)
-
-    def auth_risk_evaluation_ex(
-        self,
-        request: tax_models.AuthRiskEvaluationRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> tax_models.AuthRiskEvaluationResponse:
-        """
-        Description: 授权接口
-        Summary: 授权接口
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            tax_models.AuthRiskEvaluationResponse(),
-            self.do_request('1.0', 'blockchain.tax.risk.evaluation.auth', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def auth_risk_evaluation_ex_async(
-        self,
-        request: tax_models.AuthRiskEvaluationRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> tax_models.AuthRiskEvaluationResponse:
-        """
-        Description: 授权接口
-        Summary: 授权接口
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            tax_models.AuthRiskEvaluationResponse(),
-            await self.do_request_async('1.0', 'blockchain.tax.risk.evaluation.auth', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    def query_risk_evaluation(
-        self,
-        request: tax_models.QueryRiskEvaluationRequest,
-    ) -> tax_models.QueryRiskEvaluationResponse:
-        """
-        Description: 查询
-        Summary: 查询
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.query_risk_evaluation_ex(request, headers, runtime)
-
-    async def query_risk_evaluation_async(
-        self,
-        request: tax_models.QueryRiskEvaluationRequest,
-    ) -> tax_models.QueryRiskEvaluationResponse:
-        """
-        Description: 查询
-        Summary: 查询
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.query_risk_evaluation_ex_async(request, headers, runtime)
-
-    def query_risk_evaluation_ex(
-        self,
-        request: tax_models.QueryRiskEvaluationRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> tax_models.QueryRiskEvaluationResponse:
-        """
-        Description: 查询
-        Summary: 查询
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            tax_models.QueryRiskEvaluationResponse(),
-            self.do_request('1.0', 'blockchain.tax.risk.evaluation.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def query_risk_evaluation_ex_async(
-        self,
-        request: tax_models.QueryRiskEvaluationRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> tax_models.QueryRiskEvaluationResponse:
-        """
-        Description: 查询
-        Summary: 查询
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            tax_models.QueryRiskEvaluationResponse(),
-            await self.do_request_async('1.0', 'blockchain.tax.risk.evaluation.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
```

### Comparing `antchain_tax-1.6.13/antchain_sdk_tax/models.py` & `antchain_tax-1.6.2/antchain_sdk_tax/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -818,90 +818,14 @@
             self.is_leef_node = m.get('is_leef_node')
         if m.get('card') is not None:
             temp_model = Card()
             self.card = temp_model.from_map(m['card'])
         return self
 
 
-class RiskEvaluationAgreementExtRequest(TeaModel):
-    def __init__(
-        self,
-        type: str = None,
-        file_type: str = None,
-        content: str = None,
-    ):
-        # URL：文件地址
-        # CONTENT:Base64的文件流
-        # 
-        self.type = type
-        # 文件类型
-        # PDF
-        self.file_type = file_type
-        # type为url是传入文件地址
-        # type为CONTENT时传入Base64文件内容编码
-        # 
-        self.content = content
-
-    def validate(self):
-        self.validate_required(self.type, 'type')
-        self.validate_required(self.content, 'content')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.type is not None:
-            result['type'] = self.type
-        if self.file_type is not None:
-            result['file_type'] = self.file_type
-        if self.content is not None:
-            result['content'] = self.content
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('type') is not None:
-            self.type = m.get('type')
-        if m.get('file_type') is not None:
-            self.file_type = m.get('file_type')
-        if m.get('content') is not None:
-            self.content = m.get('content')
-        return self
-
-
-class RiskEvaluationDistrictExtRequest(TeaModel):
-    def __init__(
-        self,
-        city_code: str = None,
-    ):
-        # 地区编码
-        self.city_code = city_code
-
-    def validate(self):
-        self.validate_required(self.city_code, 'city_code')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.city_code is not None:
-            result['city_code'] = self.city_code
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('city_code') is not None:
-            self.city_code = m.get('city_code')
-        return self
-
-
 class InvoiceItem(TeaModel):
     def __init__(
         self,
         spbm: str = None,
         mc: str = None,
         jldw: str = None,
         shul: str = None,
@@ -1149,62 +1073,14 @@
         if m.get('desc') is not None:
             self.desc = m.get('desc')
         if m.get('timeout') is not None:
             self.timeout = m.get('timeout')
         return self
 
 
-class RiskEvaluationExtendInfoRequest(TeaModel):
-    def __init__(
-        self,
-        agreement_list: List[RiskEvaluationAgreementExtRequest] = None,
-        district_ext: RiskEvaluationDistrictExtRequest = None,
-    ):
-        # 协议集合
-        self.agreement_list = agreement_list
-        # 地区请求
-        self.district_ext = district_ext
-
-    def validate(self):
-        self.validate_required(self.agreement_list, 'agreement_list')
-        if self.agreement_list:
-            for k in self.agreement_list:
-                if k:
-                    k.validate()
-        self.validate_required(self.district_ext, 'district_ext')
-        if self.district_ext:
-            self.district_ext.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        result['agreement_list'] = []
-        if self.agreement_list is not None:
-            for k in self.agreement_list:
-                result['agreement_list'].append(k.to_map() if k else None)
-        if self.district_ext is not None:
-            result['district_ext'] = self.district_ext.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        self.agreement_list = []
-        if m.get('agreement_list') is not None:
-            for k in m.get('agreement_list'):
-                temp_model = RiskEvaluationAgreementExtRequest()
-                self.agreement_list.append(temp_model.from_map(k))
-        if m.get('district_ext') is not None:
-            temp_model = RiskEvaluationDistrictExtRequest()
-            self.district_ext = temp_model.from_map(m['district_ext'])
-        return self
-
-
 class TreeTemplate(TeaModel):
     def __init__(
         self,
         tree_node: TreeNode = None,
         id: str = None,
         version: str = None,
         compatible_min_version: str = None,
@@ -2788,16 +2664,14 @@
         product_instance_id: str = None,
         inst_code: str = None,
         biz_request_id: str = None,
         identity_id: str = None,
         auth_type: str = None,
         order_no: str = None,
         content: str = None,
-        query_type: str = None,
-        sub_tenant: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 机构号码
         self.inst_code = inst_code
         # 请求流水号(必填),调用方保证每次请求号唯一，受理方用来校验唯一性，同一受理号返回请求结果一致
@@ -2806,20 +2680,14 @@
         self.identity_id = identity_id
         # 授权类型(必填)
         self.auth_type = auth_type
         # 订单号
         self.order_no = order_no
         # 补充内容,如果不动产中字段为空的话查的就是授权中的cityCode
         self.content = content
-        # 查询类型
-        # NORMAL 正常调用
-        # BATCH_HAND  批刷
-        self.query_type = query_type
-        # 子机构编码，字典由系统预设白名单
-        self.sub_tenant = sub_tenant
 
     def validate(self):
         self.validate_required(self.inst_code, 'inst_code')
         self.validate_required(self.biz_request_id, 'biz_request_id')
         self.validate_required(self.identity_id, 'identity_id')
         self.validate_required(self.auth_type, 'auth_type')
         self.validate_required(self.order_no, 'order_no')
@@ -2843,18 +2711,14 @@
             result['identity_id'] = self.identity_id
         if self.auth_type is not None:
             result['auth_type'] = self.auth_type
         if self.order_no is not None:
             result['order_no'] = self.order_no
         if self.content is not None:
             result['content'] = self.content
-        if self.query_type is not None:
-            result['query_type'] = self.query_type
-        if self.sub_tenant is not None:
-            result['sub_tenant'] = self.sub_tenant
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
@@ -2867,34 +2731,28 @@
             self.identity_id = m.get('identity_id')
         if m.get('auth_type') is not None:
             self.auth_type = m.get('auth_type')
         if m.get('order_no') is not None:
             self.order_no = m.get('order_no')
         if m.get('content') is not None:
             self.content = m.get('content')
-        if m.get('query_type') is not None:
-            self.query_type = m.get('query_type')
-        if m.get('sub_tenant') is not None:
-            self.sub_tenant = m.get('sub_tenant')
         return self
 
 
 class ExecIcmSyncgatheringResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         biz_content: str = None,
         query_time: str = None,
         return_mode: str = None,
         return_result: List[ReturnDetail] = None,
         null_data_flag: bool = None,
-        query_type: str = None,
-        reauth: bool = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
@@ -2904,18 +2762,14 @@
         self.query_time = query_time
         # 返回模式
         self.return_mode = return_mode
         # 返回结果
         self.return_result = return_result
         # 是否查得
         self.null_data_flag = null_data_flag
-        # 参考区块链给出的标准字段定义
-        self.query_type = query_type
-        # 是否需要重新授权
-        self.reauth = reauth
 
     def validate(self):
         if self.return_result:
             for k in self.return_result:
                 if k:
                     k.validate()
 
@@ -2939,18 +2793,14 @@
             result['return_mode'] = self.return_mode
         result['return_result'] = []
         if self.return_result is not None:
             for k in self.return_result:
                 result['return_result'].append(k.to_map() if k else None)
         if self.null_data_flag is not None:
             result['null_data_flag'] = self.null_data_flag
-        if self.query_type is not None:
-            result['query_type'] = self.query_type
-        if self.reauth is not None:
-            result['reauth'] = self.reauth
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
@@ -2966,18 +2816,14 @@
         self.return_result = []
         if m.get('return_result') is not None:
             for k in m.get('return_result'):
                 temp_model = ReturnDetail()
                 self.return_result.append(temp_model.from_map(k))
         if m.get('null_data_flag') is not None:
             self.null_data_flag = m.get('null_data_flag')
-        if m.get('query_type') is not None:
-            self.query_type = m.get('query_type')
-        if m.get('reauth') is not None:
-            self.reauth = m.get('reauth')
         return self
 
 
 class QueryApiAuthteplateRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
@@ -3517,15 +3363,14 @@
         identity_name: str = None,
         auth_type: str = None,
         order_no: str = None,
         extend_info: StandardAuthExtendInfoRequest = None,
         cognizant_name: str = None,
         cognizant_mobile: str = None,
         cognizant_id: str = None,
-        sub_tenant: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 身份id，统一社会信用编码or其他
         self.identity_id = identity_id
         # 企业名称
@@ -3538,16 +3383,14 @@
         self.extend_info = extend_info
         # 法人姓名
         self.cognizant_name = cognizant_name
         # 法人手机号
         self.cognizant_mobile = cognizant_mobile
         # 法人身份证号
         self.cognizant_id = cognizant_id
-        # 字典由系统设置，子机构编码
-        self.sub_tenant = sub_tenant
 
     def validate(self):
         self.validate_required(self.identity_id, 'identity_id')
         self.validate_required(self.auth_type, 'auth_type')
         self.validate_required(self.order_no, 'order_no')
         self.validate_required(self.extend_info, 'extend_info')
         if self.extend_info:
@@ -3575,16 +3418,14 @@
             result['extend_info'] = self.extend_info.to_map()
         if self.cognizant_name is not None:
             result['cognizant_name'] = self.cognizant_name
         if self.cognizant_mobile is not None:
             result['cognizant_mobile'] = self.cognizant_mobile
         if self.cognizant_id is not None:
             result['cognizant_id'] = self.cognizant_id
-        if self.sub_tenant is not None:
-            result['sub_tenant'] = self.sub_tenant
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
@@ -3602,16 +3443,14 @@
             self.extend_info = temp_model.from_map(m['extend_info'])
         if m.get('cognizant_name') is not None:
             self.cognizant_name = m.get('cognizant_name')
         if m.get('cognizant_mobile') is not None:
             self.cognizant_mobile = m.get('cognizant_mobile')
         if m.get('cognizant_id') is not None:
             self.cognizant_id = m.get('cognizant_id')
-        if m.get('sub_tenant') is not None:
-            self.sub_tenant = m.get('sub_tenant')
         return self
 
 
 class AuthIcmEnterpriseResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -3779,30 +3618,27 @@
 
 class CreateApiAuthurlResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
-        order_no: str = None,
         login_url: str = None,
-        origin_login_url: str = None,
+        order_no: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
-        # 蚂蚁生成的订单号，此次授权的唯一标识
-        self.order_no = order_no
         # 短链接地址
         self.login_url = login_url
-        # 授权原始链接
-        self.origin_login_url = origin_login_url
+        # 蚂蚁生成的订单号，此次授权的唯一标识
+        self.order_no = order_no
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -3811,693 +3647,28 @@
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
-        if self.order_no is not None:
-            result['order_no'] = self.order_no
         if self.login_url is not None:
             result['login_url'] = self.login_url
-        if self.origin_login_url is not None:
-            result['origin_login_url'] = self.origin_login_url
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('req_msg_id') is not None:
-            self.req_msg_id = m.get('req_msg_id')
-        if m.get('result_code') is not None:
-            self.result_code = m.get('result_code')
-        if m.get('result_msg') is not None:
-            self.result_msg = m.get('result_msg')
-        if m.get('order_no') is not None:
-            self.order_no = m.get('order_no')
-        if m.get('login_url') is not None:
-            self.login_url = m.get('login_url')
-        if m.get('origin_login_url') is not None:
-            self.origin_login_url = m.get('origin_login_url')
-        return self
-
-
-class MatchIcmSimpleauthRequest(TeaModel):
-    def __init__(
-        self,
-        auth_token: str = None,
-        product_instance_id: str = None,
-        inst_code: str = None,
-        identity_id: str = None,
-        biz_request_id: str = None,
-    ):
-        # OAuth模式下的授权token
-        self.auth_token = auth_token
-        self.product_instance_id = product_instance_id
-        # 租户号/子租户号，如果为租户号获取，则为租户号，如果为子租户号获取，则传输子租户号
-        self.inst_code = inst_code
-        # 纳税人识别号
-        self.identity_id = identity_id
-        # 用于幂等控制
-        self.biz_request_id = biz_request_id
-
-    def validate(self):
-        self.validate_required(self.inst_code, 'inst_code')
-        self.validate_required(self.identity_id, 'identity_id')
-        self.validate_required(self.biz_request_id, 'biz_request_id')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.auth_token is not None:
-            result['auth_token'] = self.auth_token
-        if self.product_instance_id is not None:
-            result['product_instance_id'] = self.product_instance_id
-        if self.inst_code is not None:
-            result['inst_code'] = self.inst_code
-        if self.identity_id is not None:
-            result['identity_id'] = self.identity_id
-        if self.biz_request_id is not None:
-            result['biz_request_id'] = self.biz_request_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('auth_token') is not None:
-            self.auth_token = m.get('auth_token')
-        if m.get('product_instance_id') is not None:
-            self.product_instance_id = m.get('product_instance_id')
-        if m.get('inst_code') is not None:
-            self.inst_code = m.get('inst_code')
-        if m.get('identity_id') is not None:
-            self.identity_id = m.get('identity_id')
-        if m.get('biz_request_id') is not None:
-            self.biz_request_id = m.get('biz_request_id')
-        return self
-
-
-class MatchIcmSimpleauthResponse(TeaModel):
-    def __init__(
-        self,
-        req_msg_id: str = None,
-        result_code: str = None,
-        result_msg: str = None,
-        cover_result: List[str] = None,
-    ):
-        # 请求唯一ID，用于链路跟踪和问题排查
-        self.req_msg_id = req_msg_id
-        # 结果码，一般OK表示调用成功
-        self.result_code = result_code
-        # 异常信息的文本描述
-        self.result_msg = result_msg
-        # 支持的数据类型
-        self.cover_result = cover_result
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.req_msg_id is not None:
-            result['req_msg_id'] = self.req_msg_id
-        if self.result_code is not None:
-            result['result_code'] = self.result_code
-        if self.result_msg is not None:
-            result['result_msg'] = self.result_msg
-        if self.cover_result is not None:
-            result['cover_result'] = self.cover_result
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('req_msg_id') is not None:
-            self.req_msg_id = m.get('req_msg_id')
-        if m.get('result_code') is not None:
-            self.result_code = m.get('result_code')
-        if m.get('result_msg') is not None:
-            self.result_msg = m.get('result_msg')
-        if m.get('cover_result') is not None:
-            self.cover_result = m.get('cover_result')
-        return self
-
-
-class QueryIcmSimpleauthRequest(TeaModel):
-    def __init__(
-        self,
-        auth_token: str = None,
-        product_instance_id: str = None,
-        inst_code: str = None,
-        identity_id: str = None,
-        biz_request_id: str = None,
-        auth_type: str = None,
-        auth_code: str = None,
-        biz_context: str = None,
-    ):
-        # OAuth模式下的授权token
-        self.auth_token = auth_token
-        self.product_instance_id = product_instance_id
-        # 租户名称
-        self.inst_code = inst_code
-        # 纳税人识别号
-        self.identity_id = identity_id
-        # 请求id，用于幂等控制
-        self.biz_request_id = biz_request_id
-        # 产品类型：发票指标-301，税务指标-302，发票加税务指标-303
-        self.auth_type = auth_type
-        # 行方生成的授权编号
-        self.auth_code = auth_code
-        # 如果有的话，作为透传字段
-        self.biz_context = biz_context
-
-    def validate(self):
-        self.validate_required(self.inst_code, 'inst_code')
-        self.validate_required(self.identity_id, 'identity_id')
-        self.validate_required(self.biz_request_id, 'biz_request_id')
-        self.validate_required(self.auth_type, 'auth_type')
-        self.validate_required(self.auth_code, 'auth_code')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.auth_token is not None:
-            result['auth_token'] = self.auth_token
-        if self.product_instance_id is not None:
-            result['product_instance_id'] = self.product_instance_id
-        if self.inst_code is not None:
-            result['inst_code'] = self.inst_code
-        if self.identity_id is not None:
-            result['identity_id'] = self.identity_id
-        if self.biz_request_id is not None:
-            result['biz_request_id'] = self.biz_request_id
-        if self.auth_type is not None:
-            result['auth_type'] = self.auth_type
-        if self.auth_code is not None:
-            result['auth_code'] = self.auth_code
-        if self.biz_context is not None:
-            result['biz_context'] = self.biz_context
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('auth_token') is not None:
-            self.auth_token = m.get('auth_token')
-        if m.get('product_instance_id') is not None:
-            self.product_instance_id = m.get('product_instance_id')
-        if m.get('inst_code') is not None:
-            self.inst_code = m.get('inst_code')
-        if m.get('identity_id') is not None:
-            self.identity_id = m.get('identity_id')
-        if m.get('biz_request_id') is not None:
-            self.biz_request_id = m.get('biz_request_id')
-        if m.get('auth_type') is not None:
-            self.auth_type = m.get('auth_type')
-        if m.get('auth_code') is not None:
-            self.auth_code = m.get('auth_code')
-        if m.get('biz_context') is not None:
-            self.biz_context = m.get('biz_context')
-        return self
-
-
-class QueryIcmSimpleauthResponse(TeaModel):
-    def __init__(
-        self,
-        req_msg_id: str = None,
-        result_code: str = None,
-        result_msg: str = None,
-        return_result: str = None,
-    ):
-        # 请求唯一ID，用于链路跟踪和问题排查
-        self.req_msg_id = req_msg_id
-        # 结果码，一般OK表示调用成功
-        self.result_code = result_code
-        # 异常信息的文本描述
-        self.result_msg = result_msg
-        # 支持的数据类型，结果数据
-        self.return_result = return_result
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.req_msg_id is not None:
-            result['req_msg_id'] = self.req_msg_id
-        if self.result_code is not None:
-            result['result_code'] = self.result_code
-        if self.result_msg is not None:
-            result['result_msg'] = self.result_msg
-        if self.return_result is not None:
-            result['return_result'] = self.return_result
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('req_msg_id') is not None:
-            self.req_msg_id = m.get('req_msg_id')
-        if m.get('result_code') is not None:
-            self.result_code = m.get('result_code')
-        if m.get('result_msg') is not None:
-            self.result_msg = m.get('result_msg')
-        if m.get('return_result') is not None:
-            self.return_result = m.get('return_result')
-        return self
-
-
-class QueryApiSimpleauthasyncRequest(TeaModel):
-    def __init__(
-        self,
-        auth_token: str = None,
-        product_instance_id: str = None,
-        inst_code: str = None,
-        identity_id: str = None,
-        biz_request_id: str = None,
-        auth_type: str = None,
-        auth_code: str = None,
-    ):
-        # OAuth模式下的授权token
-        self.auth_token = auth_token
-        self.product_instance_id = product_instance_id
-        # 租户号/子租户号，如果为租户号获取，则为租户号，如果为子租户号获取，则传输子租户号
-        self.inst_code = inst_code
-        # 纳税人识别号
-        self.identity_id = identity_id
-        # 用于幂等控制
-        self.biz_request_id = biz_request_id
-        # 产品类型：发票指标-301，税务指标-302，发票加税务指标-303
-        self.auth_type = auth_type
-        # 行方生成的授权编号
-        # 
-        self.auth_code = auth_code
-
-    def validate(self):
-        self.validate_required(self.inst_code, 'inst_code')
-        self.validate_required(self.identity_id, 'identity_id')
-        self.validate_required(self.biz_request_id, 'biz_request_id')
-        self.validate_required(self.auth_type, 'auth_type')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.auth_token is not None:
-            result['auth_token'] = self.auth_token
-        if self.product_instance_id is not None:
-            result['product_instance_id'] = self.product_instance_id
-        if self.inst_code is not None:
-            result['inst_code'] = self.inst_code
-        if self.identity_id is not None:
-            result['identity_id'] = self.identity_id
-        if self.biz_request_id is not None:
-            result['biz_request_id'] = self.biz_request_id
-        if self.auth_type is not None:
-            result['auth_type'] = self.auth_type
-        if self.auth_code is not None:
-            result['auth_code'] = self.auth_code
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('auth_token') is not None:
-            self.auth_token = m.get('auth_token')
-        if m.get('product_instance_id') is not None:
-            self.product_instance_id = m.get('product_instance_id')
-        if m.get('inst_code') is not None:
-            self.inst_code = m.get('inst_code')
-        if m.get('identity_id') is not None:
-            self.identity_id = m.get('identity_id')
-        if m.get('biz_request_id') is not None:
-            self.biz_request_id = m.get('biz_request_id')
-        if m.get('auth_type') is not None:
-            self.auth_type = m.get('auth_type')
-        if m.get('auth_code') is not None:
-            self.auth_code = m.get('auth_code')
-        return self
-
-
-class QueryApiSimpleauthasyncResponse(TeaModel):
-    def __init__(
-        self,
-        req_msg_id: str = None,
-        result_code: str = None,
-        result_msg: str = None,
-        return_result: str = None,
-    ):
-        # 请求唯一ID，用于链路跟踪和问题排查
-        self.req_msg_id = req_msg_id
-        # 结果码，一般OK表示调用成功
-        self.result_code = result_code
-        # 异常信息的文本描述
-        self.result_msg = result_msg
-        # 成功
-        self.return_result = return_result
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.req_msg_id is not None:
-            result['req_msg_id'] = self.req_msg_id
-        if self.result_code is not None:
-            result['result_code'] = self.result_code
-        if self.result_msg is not None:
-            result['result_msg'] = self.result_msg
-        if self.return_result is not None:
-            result['return_result'] = self.return_result
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('req_msg_id') is not None:
-            self.req_msg_id = m.get('req_msg_id')
-        if m.get('result_code') is not None:
-            self.result_code = m.get('result_code')
-        if m.get('result_msg') is not None:
-            self.result_msg = m.get('result_msg')
-        if m.get('return_result') is not None:
-            self.return_result = m.get('return_result')
-        return self
-
-
-class AuthRiskEvaluationRequest(TeaModel):
-    def __init__(
-        self,
-        auth_token: str = None,
-        product_instance_id: str = None,
-        identity_id: str = None,
-        identity_name: str = None,
-        enterprise_id: str = None,
-        enterprise_name: str = None,
-        identity_type: str = None,
-        auth_type: str = None,
-        order_no: str = None,
-        sub_tenant: str = None,
-        extend_info: RiskEvaluationExtendInfoRequest = None,
-    ):
-        # OAuth模式下的授权token
-        self.auth_token = auth_token
-        self.product_instance_id = product_instance_id
-        # 个人身份证号
-        self.identity_id = identity_id
-        # 个人姓名
-        self.identity_name = identity_name
-        # 企业的统一社会信用编码
-        self.enterprise_id = enterprise_id
-        # 企业的名称
-        self.enterprise_name = enterprise_name
-        # 企业或者个人企业：ENTERPRISE  个人：PERSONAL
-        # 
-        self.identity_type = identity_type
-        # 授权的业务类型
-        self.auth_type = auth_type
-        # 授权订单号
-        self.order_no = order_no
-        # 子渠道渠道编码，需要同步蚂蚁，由蚂蚁设置。如果是银行本身，可不填
-        # 备注：如果同一信贷客户在不同银行的调用需要严格区分，分别授权
-        # 
-        self.sub_tenant = sub_tenant
-        # 扩展信息
-        self.extend_info = extend_info
-
-    def validate(self):
-        if self.identity_id is not None:
-            self.validate_max_length(self.identity_id, 'identity_id', 30)
-        if self.identity_name is not None:
-            self.validate_max_length(self.identity_name, 'identity_name', 128)
-        if self.enterprise_id is not None:
-            self.validate_max_length(self.enterprise_id, 'enterprise_id', 64)
-        self.validate_required(self.identity_type, 'identity_type')
-        self.validate_required(self.auth_type, 'auth_type')
-        self.validate_required(self.order_no, 'order_no')
-        self.validate_required(self.extend_info, 'extend_info')
-        if self.extend_info:
-            self.extend_info.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.auth_token is not None:
-            result['auth_token'] = self.auth_token
-        if self.product_instance_id is not None:
-            result['product_instance_id'] = self.product_instance_id
-        if self.identity_id is not None:
-            result['identity_id'] = self.identity_id
-        if self.identity_name is not None:
-            result['identity_name'] = self.identity_name
-        if self.enterprise_id is not None:
-            result['enterprise_id'] = self.enterprise_id
-        if self.enterprise_name is not None:
-            result['enterprise_name'] = self.enterprise_name
-        if self.identity_type is not None:
-            result['identity_type'] = self.identity_type
-        if self.auth_type is not None:
-            result['auth_type'] = self.auth_type
-        if self.order_no is not None:
-            result['order_no'] = self.order_no
-        if self.sub_tenant is not None:
-            result['sub_tenant'] = self.sub_tenant
-        if self.extend_info is not None:
-            result['extend_info'] = self.extend_info.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('auth_token') is not None:
-            self.auth_token = m.get('auth_token')
-        if m.get('product_instance_id') is not None:
-            self.product_instance_id = m.get('product_instance_id')
-        if m.get('identity_id') is not None:
-            self.identity_id = m.get('identity_id')
-        if m.get('identity_name') is not None:
-            self.identity_name = m.get('identity_name')
-        if m.get('enterprise_id') is not None:
-            self.enterprise_id = m.get('enterprise_id')
-        if m.get('enterprise_name') is not None:
-            self.enterprise_name = m.get('enterprise_name')
-        if m.get('identity_type') is not None:
-            self.identity_type = m.get('identity_type')
-        if m.get('auth_type') is not None:
-            self.auth_type = m.get('auth_type')
-        if m.get('order_no') is not None:
-            self.order_no = m.get('order_no')
-        if m.get('sub_tenant') is not None:
-            self.sub_tenant = m.get('sub_tenant')
-        if m.get('extend_info') is not None:
-            temp_model = RiskEvaluationExtendInfoRequest()
-            self.extend_info = temp_model.from_map(m['extend_info'])
-        return self
-
-
-class AuthRiskEvaluationResponse(TeaModel):
-    def __init__(
-        self,
-        req_msg_id: str = None,
-        result_code: str = None,
-        result_msg: str = None,
-        order_no: str = None,
-        auth_success: bool = None,
-        expire_time: int = None,
-        auth_time: str = None,
-    ):
-        # 请求唯一ID，用于链路跟踪和问题排查
-        self.req_msg_id = req_msg_id
-        # 结果码，一般OK表示调用成功
-        self.result_code = result_code
-        # 异常信息的文本描述
-        self.result_msg = result_msg
-        # 授权订单订单号
-        self.order_no = order_no
-        # 是否授权成功true是，false否
-        self.auth_success = auth_success
-        # 过期时间，unix时间戳 毫秒
-        self.expire_time = expire_time
-        # 授权时间，unix时间戳 毫秒
-        self.auth_time = auth_time
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.req_msg_id is not None:
-            result['req_msg_id'] = self.req_msg_id
-        if self.result_code is not None:
-            result['result_code'] = self.result_code
-        if self.result_msg is not None:
-            result['result_msg'] = self.result_msg
         if self.order_no is not None:
             result['order_no'] = self.order_no
-        if self.auth_success is not None:
-            result['auth_success'] = self.auth_success
-        if self.expire_time is not None:
-            result['expire_time'] = self.expire_time
-        if self.auth_time is not None:
-            result['auth_time'] = self.auth_time
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
+        if m.get('login_url') is not None:
+            self.login_url = m.get('login_url')
         if m.get('order_no') is not None:
             self.order_no = m.get('order_no')
-        if m.get('auth_success') is not None:
-            self.auth_success = m.get('auth_success')
-        if m.get('expire_time') is not None:
-            self.expire_time = m.get('expire_time')
-        if m.get('auth_time') is not None:
-            self.auth_time = m.get('auth_time')
-        return self
-
-
-class QueryRiskEvaluationRequest(TeaModel):
-    def __init__(
-        self,
-        auth_token: str = None,
-        product_instance_id: str = None,
-        biz_request_id: str = None,
-        identity_id: str = None,
-        auth_type: str = None,
-        order_no: str = None,
-        inst_code: str = None,
-    ):
-        # OAuth模式下的授权token
-        self.auth_token = auth_token
-        self.product_instance_id = product_instance_id
-        # 请求流水号(必填),调用方保证每次请求号唯一，受理方用来校验唯一性，同一受理号返回请求结果一致
-        self.biz_request_id = biz_request_id
-        # 信贷用户的纳税人识别号或者身份证号
-        self.identity_id = identity_id
-        # 授权类型
-        self.auth_type = auth_type
-        # 授权订单号
-        self.order_no = order_no
-        # 机构编码
-        self.inst_code = inst_code
-
-    def validate(self):
-        self.validate_required(self.biz_request_id, 'biz_request_id')
-        self.validate_required(self.identity_id, 'identity_id')
-        self.validate_required(self.auth_type, 'auth_type')
-        self.validate_required(self.order_no, 'order_no')
-        self.validate_required(self.inst_code, 'inst_code')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.auth_token is not None:
-            result['auth_token'] = self.auth_token
-        if self.product_instance_id is not None:
-            result['product_instance_id'] = self.product_instance_id
-        if self.biz_request_id is not None:
-            result['biz_request_id'] = self.biz_request_id
-        if self.identity_id is not None:
-            result['identity_id'] = self.identity_id
-        if self.auth_type is not None:
-            result['auth_type'] = self.auth_type
-        if self.order_no is not None:
-            result['order_no'] = self.order_no
-        if self.inst_code is not None:
-            result['inst_code'] = self.inst_code
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('auth_token') is not None:
-            self.auth_token = m.get('auth_token')
-        if m.get('product_instance_id') is not None:
-            self.product_instance_id = m.get('product_instance_id')
-        if m.get('biz_request_id') is not None:
-            self.biz_request_id = m.get('biz_request_id')
-        if m.get('identity_id') is not None:
-            self.identity_id = m.get('identity_id')
-        if m.get('auth_type') is not None:
-            self.auth_type = m.get('auth_type')
-        if m.get('order_no') is not None:
-            self.order_no = m.get('order_no')
-        if m.get('inst_code') is not None:
-            self.inst_code = m.get('inst_code')
-        return self
-
-
-class QueryRiskEvaluationResponse(TeaModel):
-    def __init__(
-        self,
-        req_msg_id: str = None,
-        result_code: str = None,
-        result_msg: str = None,
-        query_time: str = None,
-    ):
-        # 请求唯一ID，用于链路跟踪和问题排查
-        self.req_msg_id = req_msg_id
-        # 结果码，一般OK表示调用成功
-        self.result_code = result_code
-        # 异常信息的文本描述
-        self.result_msg = result_msg
-        # unix秒时间戳,查询时间，用来对账使用
-        self.query_time = query_time
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.req_msg_id is not None:
-            result['req_msg_id'] = self.req_msg_id
-        if self.result_code is not None:
-            result['result_code'] = self.result_code
-        if self.result_msg is not None:
-            result['result_msg'] = self.result_msg
-        if self.query_time is not None:
-            result['query_time'] = self.query_time
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('req_msg_id') is not None:
-            self.req_msg_id = m.get('req_msg_id')
-        if m.get('result_code') is not None:
-            self.result_code = m.get('result_code')
-        if m.get('result_msg') is not None:
-            self.result_msg = m.get('result_msg')
-        if m.get('query_time') is not None:
-            self.query_time = m.get('query_time')
         return self
```

### Comparing `antchain_tax-1.6.13/antchain_tax.egg-info/PKG-INFO` & `antchain_tax-1.6.2/antchain_tax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-tax
-Version: 1.6.13
+Version: 1.6.2
 Summary: Ant Chain TAX SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_tax-1.6.13/setup.py` & `antchain_tax-1.6.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_tax.
 
-Created on 26/06/2023
+Created on 30/08/2022
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_tax"
 NAME = "antchain_tax" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain TAX SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.6, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

