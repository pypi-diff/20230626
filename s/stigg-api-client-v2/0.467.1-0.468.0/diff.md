# Comparing `tmp/stigg_api_client_v2-0.467.1.tar.gz` & `tmp/stigg_api_client_v2-0.468.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.467.1.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.468.0.tar", max compression
```

## Comparing `stigg_api_client_v2-0.467.1.tar` & `stigg_api_client_v2-0.468.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1644 2023-06-22 11:32:47.050355 stigg_api_client_v2-0.467.1/README.md
--rw-r--r--   0        0        0      653 2023-06-22 11:33:33.509060 stigg_api_client_v2-0.467.1/pyproject.toml
--rw-r--r--   0        0        0       44 2023-06-22 11:32:47.050355 stigg_api_client_v2-0.467.1/stigg/__init__.py
--rw-r--r--   0        0        0      363 2023-06-22 11:32:47.050355 stigg_api_client_v2-0.467.1/stigg/client.py
--rw-r--r--   0        0        0    39611 2023-06-22 11:33:31.552959 stigg_api_client_v2-0.467.1/stigg/generated/__init__.py
--rw-r--r--   0        0        0     7303 2023-06-22 11:33:31.124937 stigg_api_client_v2-0.467.1/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0     1951 2023-06-22 11:33:31.124937 stigg_api_client_v2-0.467.1/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-06-22 11:33:30.104884 stigg_api_client_v2-0.467.1/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-06-22 11:33:30.124885 stigg_api_client_v2-0.467.1/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    70260 2023-06-22 11:33:31.376950 stigg_api_client_v2-0.467.1/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-06-22 11:33:30.152886 stigg_api_client_v2-0.467.1/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0      541 2023-06-22 11:33:30.252892 stigg_api_client_v2-0.467.1/stigg/generated/entitlements_updated.py
--rw-r--r--   0        0        0    23792 2023-06-22 11:33:27.516754 stigg_api_client_v2-0.467.1/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-06-22 11:33:30.112884 stigg_api_client_v2-0.467.1/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-06-22 11:33:30.120885 stigg_api_client_v2-0.467.1/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-06-22 11:33:31.124937 stigg_api_client_v2-0.467.1/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    53605 2023-06-22 11:33:31.124937 stigg_api_client_v2-0.467.1/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-06-22 11:33:30.176888 stigg_api_client_v2-0.467.1/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-06-22 11:33:30.184888 stigg_api_client_v2-0.467.1/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-06-22 11:33:30.168887 stigg_api_client_v2-0.467.1/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-06-22 11:33:30.228891 stigg_api_client_v2-0.467.1/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-06-22 11:33:30.200889 stigg_api_client_v2-0.467.1/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-06-22 11:33:30.196889 stigg_api_client_v2-0.467.1/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-06-22 11:33:30.240891 stigg_api_client_v2-0.467.1/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-06-22 11:33:30.192889 stigg_api_client_v2-0.467.1/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-06-22 11:33:30.212890 stigg_api_client_v2-0.467.1/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-06-22 11:33:30.220890 stigg_api_client_v2-0.467.1/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-06-22 11:33:30.068882 stigg_api_client_v2-0.467.1/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-06-22 11:33:30.060882 stigg_api_client_v2-0.467.1/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-06-22 11:33:30.092883 stigg_api_client_v2-0.467.1/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   125885 2023-06-22 11:33:30.044881 stigg_api_client_v2-0.467.1/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-06-22 11:33:30.160887 stigg_api_client_v2-0.467.1/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-06-22 11:33:30.056882 stigg_api_client_v2-0.467.1/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-06-22 11:33:30.084883 stigg_api_client_v2-0.467.1/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-06-22 11:33:30.144886 stigg_api_client_v2-0.467.1/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-06-22 11:33:30.140886 stigg_api_client_v2-0.467.1/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-06-22 11:33:30.136886 stigg_api_client_v2-0.467.1/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-06-22 11:33:31.128937 stigg_api_client_v2-0.467.1/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-06-22 11:33:30.076882 stigg_api_client_v2-0.467.1/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-06-22 11:33:30.100884 stigg_api_client_v2-0.467.1/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-06-22 11:33:30.244891 stigg_api_client_v2-0.467.1/stigg/generated/usage_history.py
--rw-r--r--   0        0        0      451 2023-06-22 11:33:30.260892 stigg_api_client_v2-0.467.1/stigg/generated/usage_updated.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.467.1/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-06-26 16:35:37.998444 stigg_api_client_v2-0.468.0/README.md
+-rw-r--r--   0        0        0      653 2023-06-26 16:36:16.654441 stigg_api_client_v2-0.468.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-06-26 16:35:37.998444 stigg_api_client_v2-0.468.0/stigg/__init__.py
+-rw-r--r--   0        0        0      363 2023-06-26 16:35:37.998444 stigg_api_client_v2-0.468.0/stigg/client.py
+-rw-r--r--   0        0        0    39681 2023-06-26 16:36:15.026442 stigg_api_client_v2-0.468.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0     7303 2023-06-26 16:36:14.666442 stigg_api_client_v2-0.468.0/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0     1951 2023-06-26 16:36:14.666442 stigg_api_client_v2-0.468.0/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-06-26 16:36:13.826442 stigg_api_client_v2-0.468.0/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-06-26 16:36:13.842442 stigg_api_client_v2-0.468.0/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    70260 2023-06-26 16:36:14.878442 stigg_api_client_v2-0.468.0/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-06-26 16:36:13.866442 stigg_api_client_v2-0.468.0/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0      541 2023-06-26 16:36:13.950442 stigg_api_client_v2-0.468.0/stigg/generated/entitlements_updated.py
+-rw-r--r--   0        0        0    23994 2023-06-26 16:36:11.658443 stigg_api_client_v2-0.468.0/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-06-26 16:36:13.830442 stigg_api_client_v2-0.468.0/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-06-26 16:36:13.838442 stigg_api_client_v2-0.468.0/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-06-26 16:36:14.666442 stigg_api_client_v2-0.468.0/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    53605 2023-06-26 16:36:14.666442 stigg_api_client_v2-0.468.0/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-06-26 16:36:13.886442 stigg_api_client_v2-0.468.0/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-06-26 16:36:13.894442 stigg_api_client_v2-0.468.0/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-06-26 16:36:13.878442 stigg_api_client_v2-0.468.0/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-06-26 16:36:13.930442 stigg_api_client_v2-0.468.0/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-06-26 16:36:13.910442 stigg_api_client_v2-0.468.0/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-06-26 16:36:13.902442 stigg_api_client_v2-0.468.0/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-06-26 16:36:13.938442 stigg_api_client_v2-0.468.0/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-06-26 16:36:13.898442 stigg_api_client_v2-0.468.0/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-06-26 16:36:13.918442 stigg_api_client_v2-0.468.0/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-06-26 16:36:13.926442 stigg_api_client_v2-0.468.0/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-06-26 16:36:13.794442 stigg_api_client_v2-0.468.0/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-06-26 16:36:13.786442 stigg_api_client_v2-0.468.0/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-06-26 16:36:13.814442 stigg_api_client_v2-0.468.0/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   126193 2023-06-26 16:36:13.770442 stigg_api_client_v2-0.468.0/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-06-26 16:36:13.870442 stigg_api_client_v2-0.468.0/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-06-26 16:36:13.782442 stigg_api_client_v2-0.468.0/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-06-26 16:36:13.806442 stigg_api_client_v2-0.468.0/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-06-26 16:36:13.858442 stigg_api_client_v2-0.468.0/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-06-26 16:36:13.854442 stigg_api_client_v2-0.468.0/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-06-26 16:36:13.850442 stigg_api_client_v2-0.468.0/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-06-26 16:36:14.670442 stigg_api_client_v2-0.468.0/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-06-26 16:36:13.798442 stigg_api_client_v2-0.468.0/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-06-26 16:36:13.818442 stigg_api_client_v2-0.468.0/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-06-26 16:36:13.946442 stigg_api_client_v2-0.468.0/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0      451 2023-06-26 16:36:13.958442 stigg_api_client_v2-0.468.0/stigg/generated/usage_updated.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.468.0/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.467.1/README.md` & `stigg_api_client_v2-0.468.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.467.1/pyproject.toml` & `stigg_api_client_v2-0.468.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stigg-api-client-v2"
-version = "0.467.1"
+version = "0.468.0"
 description = ""
 authors = ["Stigg <support@stigg.io>"]
 readme = "README.md"
 packages = [{ include = "stigg" }]
 include = ["stigg/generated/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/__init__.py` & `stigg_api_client_v2-0.468.0/stigg/generated/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 
 from .async_base_client import AsyncBaseClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
     CancelSubscriptionCancelSubscription,
 )
@@ -494,14 +494,15 @@
     PromotionalEntitlementStatusFilterComparison,
     PromotionalEntitlementUpdateInput,
     ProvisionCustomerInput,
     ProvisionCustomerSubscriptionInput,
     ProvisionSandboxInput,
     ProvisionSubscription,
     ProvisionSubscriptionInput,
+    RecalculateEntitlementsInput,
     RemoveBasePlanFromPlanInput,
     RemoveCompatibleAddonsFromPlanInput,
     RemoveCouponFromCustomerInput,
     RemoveCouponFromCustomerSubscriptionInput,
     RemoveExperimentFromCustomerInput,
     RemoveExperimentFromCustomerSubscriptionInput,
     ReportUsageInput,
@@ -1007,14 +1008,15 @@
     "ProvisionSubscription",
     "ProvisionSubscription",
     "ProvisionSubscriptionInput",
     "ProvisionSubscriptionProvisionSubscription",
     "ProvisionSubscriptionProvisionSubscriptionSubscription",
     "ProvisionSubscriptionStatus",
     "PublishMigrationType",
+    "RecalculateEntitlementsInput",
     "RemoveBasePlanFromPlanInput",
     "RemoveCompatibleAddonsFromPlanInput",
     "RemoveCouponFromCustomerInput",
     "RemoveCouponFromCustomerSubscriptionInput",
     "RemoveExperimentFromCustomerInput",
     "RemoveExperimentFromCustomerSubscriptionInput",
     "ReportEntitlementCheckRequested",
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.468.0/stigg/generated/async_base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/base_model.py` & `stigg_api_client_v2-0.468.0/stigg/generated/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.468.0/stigg/generated/cancel_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/client.py` & `stigg_api_client_v2-0.468.0/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 # Source: operations.graphql
 
 from typing import AsyncIterator
 
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.468.0/stigg/generated/create_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/entitlements_updated.py` & `stigg_api_client_v2-0.468.0/stigg/generated/entitlements_updated.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import EntitlementsUpdatedPayload
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/enums.py` & `stigg_api_client_v2-0.468.0/stigg/generated/enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerNotFound = "CustomerNotFound"
@@ -404,14 +404,15 @@
     PromotionCodeCustomerNotFirstPurchase = "PromotionCodeCustomerNotFirstPurchase"
     PromotionCodeMaxRedemptionsReached = "PromotionCodeMaxRedemptionsReached"
     PromotionCodeMinimumAmountNotReached = "PromotionCodeMinimumAmountNotReached"
     PromotionCodeNotActive = "PromotionCodeNotActive"
     PromotionCodeNotForCustomer = "PromotionCodeNotForCustomer"
     PromotionCodeNotFound = "PromotionCodeNotFound"
     RateLimitExceeded = "RateLimitExceeded"
+    RecalculateEntitlementsError = "RecalculateEntitlementsError"
     ResyncAlreadyInProgress = "ResyncAlreadyInProgress"
     ScheduledMigrationAlreadyExistsError = "ScheduledMigrationAlreadyExistsError"
     SelectedBillingModelDoesntMatchImportedItemError = (
         "SelectedBillingModelDoesntMatchImportedItemError"
     )
     StripeCustomerIsDeleted = "StripeCustomerIsDeleted"
     StripeError = "StripeError"
@@ -468,14 +469,15 @@
     PRODUCT_CREATED = "PRODUCT_CREATED"
     PRODUCT_DELETED = "PRODUCT_DELETED"
     PRODUCT_UPDATED = "PRODUCT_UPDATED"
     PROMOTIONAL_ENTITLEMENT_EXPIRED = "PROMOTIONAL_ENTITLEMENT_EXPIRED"
     PROMOTIONAL_ENTITLEMENT_GRANTED = "PROMOTIONAL_ENTITLEMENT_GRANTED"
     PROMOTIONAL_ENTITLEMENT_REVOKED = "PROMOTIONAL_ENTITLEMENT_REVOKED"
     PROMOTIONAL_ENTITLEMENT_UPDATED = "PROMOTIONAL_ENTITLEMENT_UPDATED"
+    RECALCULATE_ENTITLEMENTS_TRIGGERED = "RECALCULATE_ENTITLEMENTS_TRIGGERED"
     RESYNC_INTEGRATION_TRIGGERED = "RESYNC_INTEGRATION_TRIGGERED"
     SUBSCRIPTION_CANCELED = "SUBSCRIPTION_CANCELED"
     SUBSCRIPTION_CREATED = "SUBSCRIPTION_CREATED"
     SUBSCRIPTION_EXPIRED = "SUBSCRIPTION_EXPIRED"
     SUBSCRIPTION_TRIAL_CONVERTED = "SUBSCRIPTION_TRIAL_CONVERTED"
     SUBSCRIPTION_TRIAL_ENDS_SOON = "SUBSCRIPTION_TRIAL_ENDS_SOON"
     SUBSCRIPTION_TRIAL_EXPIRED = "SUBSCRIPTION_TRIAL_EXPIRED"
@@ -826,14 +828,15 @@
     PARTIALLY_FAILED = "PARTIALLY_FAILED"
     PENDING = "PENDING"
 
 
 class TaskType(str, Enum):
     IMPORT_INTEGRATION_CATALOG = "IMPORT_INTEGRATION_CATALOG"
     IMPORT_INTEGRATION_CUSTOMERS = "IMPORT_INTEGRATION_CUSTOMERS"
+    RECALCULATE_ENTITLEMENTS = "RECALCULATE_ENTITLEMENTS"
     RESYNC_INTEGRATION = "RESYNC_INTEGRATION"
     SUBSCRIPTION_MIGRATION = "SUBSCRIPTION_MIGRATION"
 
 
 class TrialPeriodUnits(str, Enum):
     DAY = "DAY"
     MONTH = "MONTH"
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.468.0/stigg/generated/estimate_subscription.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.468.0/stigg/generated/estimate_subscription_update.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.468.0/stigg/generated/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/fragments.py` & `stigg_api_client_v2-0.468.0/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -328,14 +328,21 @@
     weekly_according_to: Optional[WeeklyAccordingTo] = Field(alias="weeklyAccordingTo")
 
 
 class CustomerPortalEntitlementFeature(FeatureFragment):
     pass
 
 
+class CustomerPortalSubscriptionAddon(BaseModel):
+    addon_id: str = Field(alias="addonId")
+    description: Optional[str]
+    display_name: str = Field(alias="displayName")
+    quantity: int
+
+
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
     target_package: Optional[
@@ -379,21 +386,14 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
-class CustomerPortalSubscriptionAddon(BaseModel):
-    addon_id: str = Field(alias="addonId")
-    description: Optional[str]
-    display_name: str = Field(alias="displayName")
-    quantity: int
-
-
 class CustomerPortalSubscriptionFragment(BaseModel):
     subscription_id: str = Field(alias="subscriptionId")
     plan_name: str = Field(alias="planName")
     pricing: "CustomerPortalSubscriptionFragmentPricing"
     status: SubscriptionStatus
     trial_remaining_days: Optional[int] = Field(alias="trialRemainingDays")
     billing_period_range: Optional[
@@ -462,27 +462,27 @@
 
 class CustomerPortalSubscriptionFragmentScheduledUpdates(
     CustomerPortalSubscriptionScheduledUpdateData
 ):
     pass
 
 
+class CustomerResourceFragment(BaseModel):
+    resource_id: str = Field(alias="resourceId")
+
+
 class CustomerPortalPromotionalEntitlement(BaseModel):
     display_name: str = Field(alias="displayName")
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     usage_limit: Optional[float] = Field(alias="usageLimit")
     period: PromotionalEntitlementPeriod
     start_date: Any = Field(alias="startDate")
     end_date: Optional[Any] = Field(alias="endDate")
 
 
-class CustomerResourceFragment(BaseModel):
-    resource_id: str = Field(alias="resourceId")
-
-
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
     promotional_entitlements: List[
         "CustomerPortalFragmentPromotionalEntitlements"
     ] = Field(alias="promotionalEntitlements")
     billing_information: "CustomerPortalFragmentBillingInformation" = Field(
@@ -517,14 +517,29 @@
     pass
 
 
 class CustomerPortalFragmentResource(CustomerResourceFragment):
     pass
 
 
+class TotalPriceFragment(BaseModel):
+    sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
+    total: "TotalPriceFragmentTotal"
+
+
+class TotalPriceFragmentSubTotal(BaseModel):
+    amount: float
+    currency: Currency
+
+
+class TotalPriceFragmentTotal(BaseModel):
+    amount: float
+    currency: Currency
+
+
 class ProductFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: Optional[str] = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     product_settings: "ProductFragmentProductSettings" = Field(alias="productSettings")
 
@@ -589,29 +604,14 @@
 
 
 class PlanFragmentDefaultTrialConfig(BaseModel):
     duration: float
     units: TrialPeriodUnits
 
 
-class TotalPriceFragment(BaseModel):
-    sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
-    total: "TotalPriceFragmentTotal"
-
-
-class TotalPriceFragmentSubTotal(BaseModel):
-    amount: float
-    currency: Currency
-
-
-class TotalPriceFragmentTotal(BaseModel):
-    amount: float
-    currency: Currency
-
-
 class SubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
     target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
@@ -1317,54 +1317,54 @@
 CustomerPortalConfigurationFragmentPalette.update_forward_refs()
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
+CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
-CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricing.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingFeature.update_forward_refs()
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceAddonsTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentAddons.update_forward_refs()
 CustomerPortalSubscriptionFragmentScheduledUpdates.update_forward_refs()
-CustomerPortalPromotionalEntitlement.update_forward_refs()
 CustomerResourceFragment.update_forward_refs()
+CustomerPortalPromotionalEntitlement.update_forward_refs()
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
+TotalPriceFragment.update_forward_refs()
+TotalPriceFragmentSubTotal.update_forward_refs()
+TotalPriceFragmentTotal.update_forward_refs()
 ProductFragment.update_forward_refs()
 ProductFragmentProductSettings.update_forward_refs()
 ProductFragmentProductSettingsDowngradePlan.update_forward_refs()
 PlanFragment.update_forward_refs()
 PlanFragmentProduct.update_forward_refs()
 PlanFragmentBasePlan.update_forward_refs()
 PlanFragmentEntitlements.update_forward_refs()
 PlanFragmentInheritedEntitlements.update_forward_refs()
 PlanFragmentCompatibleAddons.update_forward_refs()
 PlanFragmentPrices.update_forward_refs()
 PlanFragmentDefaultTrialConfig.update_forward_refs()
-TotalPriceFragment.update_forward_refs()
-TotalPriceFragmentSubTotal.update_forward_refs()
-TotalPriceFragmentTotal.update_forward_refs()
 SubscriptionScheduledUpdateData.update_forward_refs()
 SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 SubscriptionFragment.update_forward_refs()
 SubscriptionFragmentResource.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.468.0/stigg/generated/get_active_subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.468.0/stigg/generated/get_coupons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.468.0/stigg/generated/get_customer_by_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.468.0/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.468.0/stigg/generated/get_mock_paywall.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/get_products.py` & `stigg_api_client_v2-0.468.0/stigg/generated/get_products.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.468.0/stigg/generated/get_sdk_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/input_types.py` & `stigg_api_client_v2-0.468.0/stigg/generated/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -1914,14 +1914,20 @@
     resource_id: Optional[str] = Field(alias="resourceId")
     skip_trial: Optional[bool] = Field(alias="skipTrial", default=False)
     start_date: Optional[Any] = Field(alias="startDate")
     subscription_id: Optional[str] = Field(alias="subscriptionId")
     unit_quantity: Optional[float] = Field(alias="unitQuantity", default=-1)
 
 
+class RecalculateEntitlementsInput(BaseModel):
+    customer_ids: Optional[List[str]] = Field(alias="customerIds")
+    environment_id: str = Field(alias="environmentId")
+    for_all_customers: Optional[bool] = Field(alias="forAllCustomers", default=False)
+
+
 class RemoveBasePlanFromPlanInput(BaseModel):
     id: str
     relation_id: str = Field(alias="relationId")
 
 
 class RemoveCompatibleAddonsFromPlanInput(BaseModel):
     id: str
@@ -2923,14 +2929,15 @@
 PromotionalEntitlementStatusFilterComparison.update_forward_refs()
 PromotionalEntitlementUpdateInput.update_forward_refs()
 ProvisionCustomerInput.update_forward_refs()
 ProvisionCustomerSubscriptionInput.update_forward_refs()
 ProvisionSandboxInput.update_forward_refs()
 ProvisionSubscription.update_forward_refs()
 ProvisionSubscriptionInput.update_forward_refs()
+RecalculateEntitlementsInput.update_forward_refs()
 RemoveBasePlanFromPlanInput.update_forward_refs()
 RemoveCompatibleAddonsFromPlanInput.update_forward_refs()
 RemoveCouponFromCustomerInput.update_forward_refs()
 RemoveCouponFromCustomerSubscriptionInput.update_forward_refs()
 RemoveExperimentFromCustomerInput.update_forward_refs()
 RemoveExperimentFromCustomerSubscriptionInput.update_forward_refs()
 ReportUsageInput.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.468.0/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.468.0/stigg/generated/provision_customer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.468.0/stigg/generated/provision_subscription.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.468.0/stigg/generated/report_usage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.467.1/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.468.0/stigg/generated/update_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-22 11:33
+# Generated by ariadne-codegen on 2023-06-26 16:36
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.467.1/PKG-INFO` & `stigg_api_client_v2-0.468.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.467.1
+Version: 0.468.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

