# Comparing `tmp/pulumi_okta-4.1.0a1687672875.tar.gz` & `tmp/pulumi_okta-4.1.0a1687800548.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_okta-4.1.0a1687672875.tar", last modified: Sun Jun 25 06:12:44 2023, max compression
+gzip compressed data, was "pulumi_okta-4.1.0a1687800548.tar", last modified: Mon Jun 26 17:34:11 2023, max compression
```

## Comparing `pulumi_okta-4.1.0a1687672875.tar` & `pulumi_okta-4.1.0a1687800548.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:12:44.868708 pulumi_okta-4.1.0a1687672875/
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-25 06:12:44.868708 pulumi_okta-4.1.0a1687672875/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:12:44.852708 pulumi_okta-4.1.0a1687672875/pulumi_okta/
--rw-r--r--   0 runner    (1001) docker     (123)    19391 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    21364 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/admin_role_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/admin_role_custom_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/admin_role_targets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:12:44.856709 pulumi_okta-4.1.0a1687672875/pulumi_okta/app/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63359 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app/auto_login.py
--rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app/basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    39876 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app/bookmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    10317 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app/get_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app/get_metadata_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    17697 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app/get_oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)    31761 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    14665 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app/group_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)   137739 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app/o_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app/o_auth_post_logout_redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app/o_auth_redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   137444 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app/saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    72331 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app/secure_password_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    58966 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app/swa.py
--rw-r--r--   0 runner    (1001) docker     (123)    66578 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app/three_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app_group_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app_oauth_api_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app_saml_app_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    65611 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app_shared_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app_signon_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    81293 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app_signon_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    23561 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app_user_base_schema_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    50905 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/app_user_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:12:44.856709 pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/get_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/get_server_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/get_server_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23427 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    24590 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/server_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/server_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    46621 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/server_policy_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)    46368 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/server_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    20705 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/server_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    19984 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/auth_server_claim_default.py
--rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/auth_server_default.py
--rw-r--r--   0 runner    (1001) docker     (123)    46170 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/behaviour.py
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/brand.py
--rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/captcha.py
--rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/captcha_org_wide_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:12:44.856709 pulumi_okta-4.1.0a1687672875/pulumi_okta/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/domain_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)    37986 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/email_customization.py
--rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/email_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/email_sender_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/event_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/event_hook_verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:12:44.860709 pulumi_okta-4.1.0a1687672875/pulumi_okta/factor/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/factor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/factor/factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/factor_totp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/get_app_group_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/get_app_signon_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/get_app_user_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/get_auth_server_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/get_auth_server_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/get_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/get_behaviour.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/get_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/get_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/get_brands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/get_email_customization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/get_email_customizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/get_network_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/get_role_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/get_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/get_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/get_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/get_themes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/get_trusted_origins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/get_user_security_questions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:12:44.860709 pulumi_okta-4.1.0a1687672875/pulumi_okta/group/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/group/get_everyone_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/group/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/group/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    23973 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/group/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    21025 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/group/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)    47214 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/group_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:12:44.860709 pulumi_okta-4.1.0a1687672875/pulumi_okta/idp/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/idp/get_metadata_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/idp/get_oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/idp/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    17510 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/idp/get_social.py
--rw-r--r--   0 runner    (1001) docker     (123)    87339 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/idp/oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)    83358 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/idp/saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/idp/saml_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    72824 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/idp/social.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:12:44.864709 pulumi_okta-4.1.0a1687672875/pulumi_okta/index/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/index/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/index/email_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/index/email_domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/index/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/index/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:12:44.864709 pulumi_okta-4.1.0a1687672875/pulumi_okta/inline/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/inline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/inline/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18690 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/inline/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/inline/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18793 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/link_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    14673 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/link_value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:12:44.864709 pulumi_okta-4.1.0a1687672875/pulumi_okta/network/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24327 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/network/zone.py
--rw-r--r--   0 runner    (1001) docker     (123)    35387 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/org_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/org_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    32891 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:12:44.864709 pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/get_default_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/get_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    69146 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/mfa.py
--rw-r--r--   0 runner    (1001) docker     (123)    14772 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    79587 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/password.py
--rw-r--r--   0 runner    (1001) docker     (123)    48541 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/rule_idp_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    30922 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/rule_mfa.py
--rw-r--r--   0 runner    (1001) docker     (123)    30689 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/rule_password.py
--rw-r--r--   0 runner    (1001) docker     (123)    66350 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/rule_signon.py
--rw-r--r--   0 runner    (1001) docker     (123)    13691 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/signon.py
--rw-r--r--   0 runner    (1001) docker     (123)    65319 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/policy_mfa_default.py
--rw-r--r--   0 runner    (1001) docker     (123)    71401 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/policy_password_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/policy_profile_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/policy_profile_enrollment_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    31670 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/policy_rule_profile_enrollment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:12:44.864709 pulumi_okta-4.1.0a1687672875/pulumi_okta/profile/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/profile/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22298 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/profile/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/profile/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23808 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/rate_limiting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/resource_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/role_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/security_notification_emails.py
--rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/template_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)    42242 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/theme.py
--rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/threat_insight_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:12:44.868708 pulumi_okta-4.1.0a1687672875/pulumi_okta/trustedorigin/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/trustedorigin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/trustedorigin/origin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:12:44.868708 pulumi_okta-4.1.0a1687672875/pulumi_okta/user/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/user/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24937 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/user/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/user/get_user_profile_mapping_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/user/get_user_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/user/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    22177 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/user/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    98382 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/user/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/user/user_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/user_admin_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/user_base_schema_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/user_factor_question.py
--rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/user_group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)    51704 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta/user_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:12:44.852708 pulumi_okta-4.1.0a1687672875/pulumi_okta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/pulumi_okta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 06:12:44.868708 pulumi_okta-4.1.0a1687672875/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-25 06:12:44.000000 pulumi_okta-4.1.0a1687672875/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.892634 pulumi_okta-4.1.0a1687800548/
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-26 17:34:11.892634 pulumi_okta-4.1.0a1687800548/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.880634 pulumi_okta-4.1.0a1687800548/pulumi_okta/
+-rw-r--r--   0 runner    (1001) docker     (123)    19391 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21364 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/admin_role_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/admin_role_custom_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/admin_role_targets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.884634 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63359 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/auto_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39876 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10317 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/get_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/get_metadata_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17697 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/get_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31761 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14665 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/group_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139451 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/o_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/o_auth_post_logout_redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/o_auth_redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137444 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72331 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/secure_password_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58966 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/swa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66578 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/three_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app_group_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app_oauth_api_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app_saml_app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65611 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app_shared_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app_signon_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81293 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app_signon_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23561 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app_user_base_schema_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50905 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app_user_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.884634 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/get_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/get_server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/get_server_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23427 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24590 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46621 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server_policy_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46368 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20705 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19984 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth_server_claim_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth_server_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46170 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16966 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/captcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/captcha_org_wide_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.884634 pulumi_okta-4.1.0a1687800548/pulumi_okta/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/domain_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37986 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/email_customization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/email_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/email_sender_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/event_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/event_hook_verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.884634 pulumi_okta-4.1.0a1687800548/pulumi_okta/factor/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/factor/factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/factor_totp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_app_group_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_app_signon_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_app_user_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_auth_server_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_auth_server_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_brands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_email_customization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_email_customizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_network_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_role_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_themes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_trusted_origins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_user_security_questions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.888635 pulumi_okta-4.1.0a1687800548/pulumi_okta/group/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/group/get_everyone_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/group/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/group/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23973 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/group/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21025 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/group/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47214 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/group_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.888635 pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/get_metadata_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/get_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17510 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/get_social.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87339 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83358 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/saml_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72824 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/social.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.888635 pulumi_okta-4.1.0a1687800548/pulumi_okta/index/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/index/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/index/email_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/index/email_domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/index/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/index/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.888635 pulumi_okta-4.1.0a1687800548/pulumi_okta/inline/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/inline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/inline/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18690 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/inline/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/inline/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18793 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/link_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14673 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/link_value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.888635 pulumi_okta-4.1.0a1687800548/pulumi_okta/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26167 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/network/zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35387 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/org_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/org_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.892634 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/get_default_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/get_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69146 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14772 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79587 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48541 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/rule_idp_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30922 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/rule_mfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30689 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/rule_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66350 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/rule_signon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13691 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/signon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65319 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy_mfa_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71401 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy_password_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy_profile_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy_profile_enrollment_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31670 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy_rule_profile_enrollment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.892634 pulumi_okta-4.1.0a1687800548/pulumi_okta/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/profile/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22298 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/profile/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/profile/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23808 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/rate_limiting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/resource_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/role_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/security_notification_emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/template_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42242 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/threat_insight_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.892634 pulumi_okta-4.1.0a1687800548/pulumi_okta/trustedorigin/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/trustedorigin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/trustedorigin/origin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.892634 pulumi_okta-4.1.0a1687800548/pulumi_okta/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24937 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user/get_user_profile_mapping_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user/get_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22177 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98382 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user/user_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user_admin_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user_base_schema_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user_factor_question.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user_group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51704 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.880634 pulumi_okta-4.1.0a1687800548/pulumi_okta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:34:11.892634 pulumi_okta-4.1.0a1687800548/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/setup.py
```

### Comparing `pulumi_okta-4.1.0a1687672875/PKG-INFO` & `pulumi_okta-4.1.0a1687800548/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_okta
-Version: 4.1.0a1687672875
+Version: 4.1.0a1687800548
 Summary: A Pulumi package for creating and managing okta resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-okta
 Keywords: pulumi okta
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_okta-4.1.0a1687672875/README.md` & `pulumi_okta-4.1.0a1687800548/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/__init__.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/_inputs.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/_utilities.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/admin_role_custom.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/admin_role_custom.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/admin_role_custom_assignments.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/admin_role_custom_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/admin_role_targets.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/admin_role_targets.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app/__init__.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app/_inputs.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app/auto_login.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/auto_login.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app/basic_auth.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app/bookmark.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/bookmark.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app/get_app.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/get_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app/get_metadata_saml.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/get_metadata_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app/get_oauth.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/get_oauth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app/get_saml.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/get_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app/group_assignment.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/group_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app/o_auth.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/o_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
                  grant_types: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  groups_claim: Optional[pulumi.Input['OAuthGroupsClaimArgs']] = None,
                  hide_ios: Optional[pulumi.Input[bool]] = None,
                  hide_web: Optional[pulumi.Input[bool]] = None,
                  implicit_assignment: Optional[pulumi.Input[bool]] = None,
                  issuer_mode: Optional[pulumi.Input[str]] = None,
                  jwks: Optional[pulumi.Input[Sequence[pulumi.Input['OAuthJwkArgs']]]] = None,
+                 jwks_uri: Optional[pulumi.Input[str]] = None,
                  login_mode: Optional[pulumi.Input[str]] = None,
                  login_scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  login_uri: Optional[pulumi.Input[str]] = None,
                  logo: Optional[pulumi.Input[str]] = None,
                  logo_uri: Optional[pulumi.Input[str]] = None,
                  omit_secret: Optional[pulumi.Input[bool]] = None,
                  pkce_required: Optional[pulumi.Input[bool]] = None,
@@ -90,14 +91,15 @@
         :param pulumi.Input['OAuthGroupsClaimArgs'] groups_claim: Groups claim for an OpenID Connect client application. **IMPORTANT**: this field is available only when using api token in the provider config.
         :param pulumi.Input[bool] hide_ios: Do not display application icon on mobile app.
         :param pulumi.Input[bool] hide_web: Do not display application icon to users.
         :param pulumi.Input[bool] implicit_assignment: *Early Access Property*. Enables [Federation Broker Mode](https://help.okta.com/en/prod/Content/Topics/Apps/apps-fbm-enable.htm). When this mode is enabled, `users` and `groups` arguments are ignored.
         :param pulumi.Input[str] issuer_mode: Indicates whether the Okta Authorization Server uses the original Okta org domain URL or a custom domain URL as the issuer of ID token for this client.
                Valid values: `"CUSTOM_URL"`,`"ORG_URL"` or `"DYNAMIC"`. Default is `"ORG_URL"`.
         :param pulumi.Input[Sequence[pulumi.Input['OAuthJwkArgs']]] jwks: JSON Web Key set. [Admin Console JWK Reference](https://developer.okta.com/docs/guides/implement-oauth-for-okta-serviceapp/main/#generate-the-jwk-in-the-admin-console)
+        :param pulumi.Input[str] jwks_uri: URL reference to JWKS
         :param pulumi.Input[str] login_mode: The type of Idp-Initiated login that the client supports, if any. Valid values: `"DISABLED"`, `"SPEC"`, `"OKTA"`. Default is `"DISABLED"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] login_scopes: List of scopes to use for the request. Valid values: `"openid"`, `"profile"`, `"email"`, `"address"`, `"phone"`. Required when `login_mode` is NOT `DISABLED`.
         :param pulumi.Input[str] login_uri: URI that initiates login. Required when `login_mode` is NOT `DISABLED`.
         :param pulumi.Input[str] logo: Local file path to the logo. The file must be in PNG, JPG, or GIF format, and less than 1 MB in size.
         :param pulumi.Input[str] logo_uri: URI that references a logo for the client.
         :param pulumi.Input[bool] omit_secret: This tells the provider not to persist the application's secret to state. Your app's `client_secret` will be recreated if this ever changes from true => false.
         :param pulumi.Input[bool] pkce_required: Require Proof Key for Code Exchange (PKCE) for
@@ -178,14 +180,16 @@
             pulumi.set(__self__, "hide_web", hide_web)
         if implicit_assignment is not None:
             pulumi.set(__self__, "implicit_assignment", implicit_assignment)
         if issuer_mode is not None:
             pulumi.set(__self__, "issuer_mode", issuer_mode)
         if jwks is not None:
             pulumi.set(__self__, "jwks", jwks)
+        if jwks_uri is not None:
+            pulumi.set(__self__, "jwks_uri", jwks_uri)
         if login_mode is not None:
             pulumi.set(__self__, "login_mode", login_mode)
         if login_scopes is not None:
             pulumi.set(__self__, "login_scopes", login_scopes)
         if login_uri is not None:
             pulumi.set(__self__, "login_uri", login_uri)
         if logo is not None:
@@ -508,14 +512,26 @@
         return pulumi.get(self, "jwks")
 
     @jwks.setter
     def jwks(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['OAuthJwkArgs']]]]):
         pulumi.set(self, "jwks", value)
 
     @property
+    @pulumi.getter(name="jwksUri")
+    def jwks_uri(self) -> Optional[pulumi.Input[str]]:
+        """
+        URL reference to JWKS
+        """
+        return pulumi.get(self, "jwks_uri")
+
+    @jwks_uri.setter
+    def jwks_uri(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "jwks_uri", value)
+
+    @property
     @pulumi.getter(name="loginMode")
     def login_mode(self) -> Optional[pulumi.Input[str]]:
         """
         The type of Idp-Initiated login that the client supports, if any. Valid values: `"DISABLED"`, `"SPEC"`, `"OKTA"`. Default is `"DISABLED"`.
         """
         return pulumi.get(self, "login_mode")
 
@@ -818,14 +834,15 @@
                  grant_types: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  groups_claim: Optional[pulumi.Input['OAuthGroupsClaimArgs']] = None,
                  hide_ios: Optional[pulumi.Input[bool]] = None,
                  hide_web: Optional[pulumi.Input[bool]] = None,
                  implicit_assignment: Optional[pulumi.Input[bool]] = None,
                  issuer_mode: Optional[pulumi.Input[str]] = None,
                  jwks: Optional[pulumi.Input[Sequence[pulumi.Input['OAuthJwkArgs']]]] = None,
+                 jwks_uri: Optional[pulumi.Input[str]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  login_mode: Optional[pulumi.Input[str]] = None,
                  login_scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  login_uri: Optional[pulumi.Input[str]] = None,
                  logo: Optional[pulumi.Input[str]] = None,
                  logo_uri: Optional[pulumi.Input[str]] = None,
                  logo_url: Optional[pulumi.Input[str]] = None,
@@ -877,14 +894,15 @@
         :param pulumi.Input['OAuthGroupsClaimArgs'] groups_claim: Groups claim for an OpenID Connect client application. **IMPORTANT**: this field is available only when using api token in the provider config.
         :param pulumi.Input[bool] hide_ios: Do not display application icon on mobile app.
         :param pulumi.Input[bool] hide_web: Do not display application icon to users.
         :param pulumi.Input[bool] implicit_assignment: *Early Access Property*. Enables [Federation Broker Mode](https://help.okta.com/en/prod/Content/Topics/Apps/apps-fbm-enable.htm). When this mode is enabled, `users` and `groups` arguments are ignored.
         :param pulumi.Input[str] issuer_mode: Indicates whether the Okta Authorization Server uses the original Okta org domain URL or a custom domain URL as the issuer of ID token for this client.
                Valid values: `"CUSTOM_URL"`,`"ORG_URL"` or `"DYNAMIC"`. Default is `"ORG_URL"`.
         :param pulumi.Input[Sequence[pulumi.Input['OAuthJwkArgs']]] jwks: JSON Web Key set. [Admin Console JWK Reference](https://developer.okta.com/docs/guides/implement-oauth-for-okta-serviceapp/main/#generate-the-jwk-in-the-admin-console)
+        :param pulumi.Input[str] jwks_uri: URL reference to JWKS
         :param pulumi.Input[str] label: The Application's display name.
         :param pulumi.Input[str] login_mode: The type of Idp-Initiated login that the client supports, if any. Valid values: `"DISABLED"`, `"SPEC"`, `"OKTA"`. Default is `"DISABLED"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] login_scopes: List of scopes to use for the request. Valid values: `"openid"`, `"profile"`, `"email"`, `"address"`, `"phone"`. Required when `login_mode` is NOT `DISABLED`.
         :param pulumi.Input[str] login_uri: URI that initiates login. Required when `login_mode` is NOT `DISABLED`.
         :param pulumi.Input[str] logo: Local file path to the logo. The file must be in PNG, JPG, or GIF format, and less than 1 MB in size.
         :param pulumi.Input[str] logo_uri: URI that references a logo for the client.
         :param pulumi.Input[str] logo_url: Direct link of application logo.
@@ -970,14 +988,16 @@
             pulumi.set(__self__, "hide_web", hide_web)
         if implicit_assignment is not None:
             pulumi.set(__self__, "implicit_assignment", implicit_assignment)
         if issuer_mode is not None:
             pulumi.set(__self__, "issuer_mode", issuer_mode)
         if jwks is not None:
             pulumi.set(__self__, "jwks", jwks)
+        if jwks_uri is not None:
+            pulumi.set(__self__, "jwks_uri", jwks_uri)
         if label is not None:
             pulumi.set(__self__, "label", label)
         if login_mode is not None:
             pulumi.set(__self__, "login_mode", login_mode)
         if login_scopes is not None:
             pulumi.set(__self__, "login_scopes", login_scopes)
         if login_uri is not None:
@@ -1298,14 +1318,26 @@
         return pulumi.get(self, "jwks")
 
     @jwks.setter
     def jwks(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['OAuthJwkArgs']]]]):
         pulumi.set(self, "jwks", value)
 
     @property
+    @pulumi.getter(name="jwksUri")
+    def jwks_uri(self) -> Optional[pulumi.Input[str]]:
+        """
+        URL reference to JWKS
+        """
+        return pulumi.get(self, "jwks_uri")
+
+    @jwks_uri.setter
+    def jwks_uri(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "jwks_uri", value)
+
+    @property
     @pulumi.getter
     def label(self) -> Optional[pulumi.Input[str]]:
         """
         The Application's display name.
         """
         return pulumi.get(self, "label")
 
@@ -1669,14 +1701,15 @@
                  grant_types: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  groups_claim: Optional[pulumi.Input[pulumi.InputType['OAuthGroupsClaimArgs']]] = None,
                  hide_ios: Optional[pulumi.Input[bool]] = None,
                  hide_web: Optional[pulumi.Input[bool]] = None,
                  implicit_assignment: Optional[pulumi.Input[bool]] = None,
                  issuer_mode: Optional[pulumi.Input[str]] = None,
                  jwks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['OAuthJwkArgs']]]]] = None,
+                 jwks_uri: Optional[pulumi.Input[str]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  login_mode: Optional[pulumi.Input[str]] = None,
                  login_scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  login_uri: Optional[pulumi.Input[str]] = None,
                  logo: Optional[pulumi.Input[str]] = None,
                  logo_uri: Optional[pulumi.Input[str]] = None,
                  omit_secret: Optional[pulumi.Input[bool]] = None,
@@ -1779,14 +1812,15 @@
         :param pulumi.Input[pulumi.InputType['OAuthGroupsClaimArgs']] groups_claim: Groups claim for an OpenID Connect client application. **IMPORTANT**: this field is available only when using api token in the provider config.
         :param pulumi.Input[bool] hide_ios: Do not display application icon on mobile app.
         :param pulumi.Input[bool] hide_web: Do not display application icon to users.
         :param pulumi.Input[bool] implicit_assignment: *Early Access Property*. Enables [Federation Broker Mode](https://help.okta.com/en/prod/Content/Topics/Apps/apps-fbm-enable.htm). When this mode is enabled, `users` and `groups` arguments are ignored.
         :param pulumi.Input[str] issuer_mode: Indicates whether the Okta Authorization Server uses the original Okta org domain URL or a custom domain URL as the issuer of ID token for this client.
                Valid values: `"CUSTOM_URL"`,`"ORG_URL"` or `"DYNAMIC"`. Default is `"ORG_URL"`.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['OAuthJwkArgs']]]] jwks: JSON Web Key set. [Admin Console JWK Reference](https://developer.okta.com/docs/guides/implement-oauth-for-okta-serviceapp/main/#generate-the-jwk-in-the-admin-console)
+        :param pulumi.Input[str] jwks_uri: URL reference to JWKS
         :param pulumi.Input[str] label: The Application's display name.
         :param pulumi.Input[str] login_mode: The type of Idp-Initiated login that the client supports, if any. Valid values: `"DISABLED"`, `"SPEC"`, `"OKTA"`. Default is `"DISABLED"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] login_scopes: List of scopes to use for the request. Valid values: `"openid"`, `"profile"`, `"email"`, `"address"`, `"phone"`. Required when `login_mode` is NOT `DISABLED`.
         :param pulumi.Input[str] login_uri: URI that initiates login. Required when `login_mode` is NOT `DISABLED`.
         :param pulumi.Input[str] logo: Local file path to the logo. The file must be in PNG, JPG, or GIF format, and less than 1 MB in size.
         :param pulumi.Input[str] logo_uri: URI that references a logo for the client.
         :param pulumi.Input[bool] omit_secret: This tells the provider not to persist the application's secret to state. Your app's `client_secret` will be recreated if this ever changes from true => false.
@@ -1921,14 +1955,15 @@
                  grant_types: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  groups_claim: Optional[pulumi.Input[pulumi.InputType['OAuthGroupsClaimArgs']]] = None,
                  hide_ios: Optional[pulumi.Input[bool]] = None,
                  hide_web: Optional[pulumi.Input[bool]] = None,
                  implicit_assignment: Optional[pulumi.Input[bool]] = None,
                  issuer_mode: Optional[pulumi.Input[str]] = None,
                  jwks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['OAuthJwkArgs']]]]] = None,
+                 jwks_uri: Optional[pulumi.Input[str]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  login_mode: Optional[pulumi.Input[str]] = None,
                  login_scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  login_uri: Optional[pulumi.Input[str]] = None,
                  logo: Optional[pulumi.Input[str]] = None,
                  logo_uri: Optional[pulumi.Input[str]] = None,
                  omit_secret: Optional[pulumi.Input[bool]] = None,
@@ -1975,14 +2010,15 @@
             __props__.__dict__["grant_types"] = grant_types
             __props__.__dict__["groups_claim"] = groups_claim
             __props__.__dict__["hide_ios"] = hide_ios
             __props__.__dict__["hide_web"] = hide_web
             __props__.__dict__["implicit_assignment"] = implicit_assignment
             __props__.__dict__["issuer_mode"] = issuer_mode
             __props__.__dict__["jwks"] = jwks
+            __props__.__dict__["jwks_uri"] = jwks_uri
             if label is None and not opts.urn:
                 raise TypeError("Missing required property 'label'")
             __props__.__dict__["label"] = label
             __props__.__dict__["login_mode"] = login_mode
             __props__.__dict__["login_scopes"] = login_scopes
             __props__.__dict__["login_uri"] = login_uri
             __props__.__dict__["logo"] = logo
@@ -2041,14 +2077,15 @@
             grant_types: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             groups_claim: Optional[pulumi.Input[pulumi.InputType['OAuthGroupsClaimArgs']]] = None,
             hide_ios: Optional[pulumi.Input[bool]] = None,
             hide_web: Optional[pulumi.Input[bool]] = None,
             implicit_assignment: Optional[pulumi.Input[bool]] = None,
             issuer_mode: Optional[pulumi.Input[str]] = None,
             jwks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['OAuthJwkArgs']]]]] = None,
+            jwks_uri: Optional[pulumi.Input[str]] = None,
             label: Optional[pulumi.Input[str]] = None,
             login_mode: Optional[pulumi.Input[str]] = None,
             login_scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             login_uri: Optional[pulumi.Input[str]] = None,
             logo: Optional[pulumi.Input[str]] = None,
             logo_uri: Optional[pulumi.Input[str]] = None,
             logo_url: Optional[pulumi.Input[str]] = None,
@@ -2105,14 +2142,15 @@
         :param pulumi.Input[pulumi.InputType['OAuthGroupsClaimArgs']] groups_claim: Groups claim for an OpenID Connect client application. **IMPORTANT**: this field is available only when using api token in the provider config.
         :param pulumi.Input[bool] hide_ios: Do not display application icon on mobile app.
         :param pulumi.Input[bool] hide_web: Do not display application icon to users.
         :param pulumi.Input[bool] implicit_assignment: *Early Access Property*. Enables [Federation Broker Mode](https://help.okta.com/en/prod/Content/Topics/Apps/apps-fbm-enable.htm). When this mode is enabled, `users` and `groups` arguments are ignored.
         :param pulumi.Input[str] issuer_mode: Indicates whether the Okta Authorization Server uses the original Okta org domain URL or a custom domain URL as the issuer of ID token for this client.
                Valid values: `"CUSTOM_URL"`,`"ORG_URL"` or `"DYNAMIC"`. Default is `"ORG_URL"`.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['OAuthJwkArgs']]]] jwks: JSON Web Key set. [Admin Console JWK Reference](https://developer.okta.com/docs/guides/implement-oauth-for-okta-serviceapp/main/#generate-the-jwk-in-the-admin-console)
+        :param pulumi.Input[str] jwks_uri: URL reference to JWKS
         :param pulumi.Input[str] label: The Application's display name.
         :param pulumi.Input[str] login_mode: The type of Idp-Initiated login that the client supports, if any. Valid values: `"DISABLED"`, `"SPEC"`, `"OKTA"`. Default is `"DISABLED"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] login_scopes: List of scopes to use for the request. Valid values: `"openid"`, `"profile"`, `"email"`, `"address"`, `"phone"`. Required when `login_mode` is NOT `DISABLED`.
         :param pulumi.Input[str] login_uri: URI that initiates login. Required when `login_mode` is NOT `DISABLED`.
         :param pulumi.Input[str] logo: Local file path to the logo. The file must be in PNG, JPG, or GIF format, and less than 1 MB in size.
         :param pulumi.Input[str] logo_uri: URI that references a logo for the client.
         :param pulumi.Input[str] logo_url: Direct link of application logo.
@@ -2180,14 +2218,15 @@
         __props__.__dict__["grant_types"] = grant_types
         __props__.__dict__["groups_claim"] = groups_claim
         __props__.__dict__["hide_ios"] = hide_ios
         __props__.__dict__["hide_web"] = hide_web
         __props__.__dict__["implicit_assignment"] = implicit_assignment
         __props__.__dict__["issuer_mode"] = issuer_mode
         __props__.__dict__["jwks"] = jwks
+        __props__.__dict__["jwks_uri"] = jwks_uri
         __props__.__dict__["label"] = label
         __props__.__dict__["login_mode"] = login_mode
         __props__.__dict__["login_scopes"] = login_scopes
         __props__.__dict__["login_uri"] = login_uri
         __props__.__dict__["logo"] = logo
         __props__.__dict__["logo_uri"] = logo_uri
         __props__.__dict__["logo_url"] = logo_url
@@ -2394,14 +2433,22 @@
     def jwks(self) -> pulumi.Output[Optional[Sequence['outputs.OAuthJwk']]]:
         """
         JSON Web Key set. [Admin Console JWK Reference](https://developer.okta.com/docs/guides/implement-oauth-for-okta-serviceapp/main/#generate-the-jwk-in-the-admin-console)
         """
         return pulumi.get(self, "jwks")
 
     @property
+    @pulumi.getter(name="jwksUri")
+    def jwks_uri(self) -> pulumi.Output[Optional[str]]:
+        """
+        URL reference to JWKS
+        """
+        return pulumi.get(self, "jwks_uri")
+
+    @property
     @pulumi.getter
     def label(self) -> pulumi.Output[str]:
         """
         The Application's display name.
         """
         return pulumi.get(self, "label")
```

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app/o_auth_post_logout_redirect_uri.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/o_auth_post_logout_redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app/o_auth_redirect_uri.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/o_auth_redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app/outputs.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app/saml.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app/secure_password_store.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/secure_password_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app/swa.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/swa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app/three_field.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/three_field.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app/user.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app_group_assignments.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app_group_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app_oauth_api_scope.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app_oauth_api_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app_saml_app_settings.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app_saml_app_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app_shared_credentials.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app_shared_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app_signon_policy.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app_signon_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app_signon_policy_rule.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app_signon_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app_user_base_schema_property.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app_user_base_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/app_user_schema_property.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/app_user_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/__init__.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/get_server.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/get_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/get_server_policy.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/get_server_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/get_server_scopes.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/get_server_scopes.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/outputs.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/server.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/server_claim.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/server_policy.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/server_policy_claim.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server_policy_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/server_policy_rule.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/auth/server_scope.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/auth_server_claim_default.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth_server_claim_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/auth_server_default.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth_server_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/authenticator.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/authenticator.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/behaviour.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/behaviour.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/brand.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/brand.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,31 +86,35 @@
 @pulumi.input_type
 class _BrandState:
     def __init__(__self__, *,
                  agree_to_custom_privacy_policy: Optional[pulumi.Input[bool]] = None,
                  brand_id: Optional[pulumi.Input[str]] = None,
                  custom_privacy_policy_url: Optional[pulumi.Input[str]] = None,
                  links: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
                  remove_powered_by_okta: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering Brand resources.
         :param pulumi.Input[bool] agree_to_custom_privacy_policy: Is a required input flag with when changing custom_privacy_url, shouldn't be considered as a readable property
         :param pulumi.Input[str] brand_id: Brand ID, used for read (faux-create)
         :param pulumi.Input[str] custom_privacy_policy_url: (Optional) Custom privacy policy URL
         :param pulumi.Input[str] links: (Read-only) Link relations for this object - JSON HAL - Discoverable resources related to the brand
+        :param pulumi.Input[str] name: Brand name
         :param pulumi.Input[bool] remove_powered_by_okta: (Optional) Removes "Powered by Okta" from the Okta-hosted sign-in page, and "© 2021 Okta, Inc." from the Okta End-User Dashboard
         """
         if agree_to_custom_privacy_policy is not None:
             pulumi.set(__self__, "agree_to_custom_privacy_policy", agree_to_custom_privacy_policy)
         if brand_id is not None:
             pulumi.set(__self__, "brand_id", brand_id)
         if custom_privacy_policy_url is not None:
             pulumi.set(__self__, "custom_privacy_policy_url", custom_privacy_policy_url)
         if links is not None:
             pulumi.set(__self__, "links", links)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
         if remove_powered_by_okta is not None:
             pulumi.set(__self__, "remove_powered_by_okta", remove_powered_by_okta)
 
     @property
     @pulumi.getter(name="agreeToCustomPrivacyPolicy")
     def agree_to_custom_privacy_policy(self) -> Optional[pulumi.Input[bool]]:
         """
@@ -155,14 +159,26 @@
         return pulumi.get(self, "links")
 
     @links.setter
     def links(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "links", value)
 
     @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Brand name
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+    @property
     @pulumi.getter(name="removePoweredByOkta")
     def remove_powered_by_okta(self) -> Optional[pulumi.Input[bool]]:
         """
         (Optional) Removes "Powered by Okta" from the Okta-hosted sign-in page, and "© 2021 Okta, Inc." from the Okta End-User Dashboard
         """
         return pulumi.get(self, "remove_powered_by_okta")
 
@@ -269,50 +285,54 @@
             __props__ = BrandArgs.__new__(BrandArgs)
 
             __props__.__dict__["agree_to_custom_privacy_policy"] = agree_to_custom_privacy_policy
             __props__.__dict__["brand_id"] = brand_id
             __props__.__dict__["custom_privacy_policy_url"] = custom_privacy_policy_url
             __props__.__dict__["remove_powered_by_okta"] = remove_powered_by_okta
             __props__.__dict__["links"] = None
+            __props__.__dict__["name"] = None
         super(Brand, __self__).__init__(
             'okta:index/brand:Brand',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             agree_to_custom_privacy_policy: Optional[pulumi.Input[bool]] = None,
             brand_id: Optional[pulumi.Input[str]] = None,
             custom_privacy_policy_url: Optional[pulumi.Input[str]] = None,
             links: Optional[pulumi.Input[str]] = None,
+            name: Optional[pulumi.Input[str]] = None,
             remove_powered_by_okta: Optional[pulumi.Input[bool]] = None) -> 'Brand':
         """
         Get an existing Brand resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] agree_to_custom_privacy_policy: Is a required input flag with when changing custom_privacy_url, shouldn't be considered as a readable property
         :param pulumi.Input[str] brand_id: Brand ID, used for read (faux-create)
         :param pulumi.Input[str] custom_privacy_policy_url: (Optional) Custom privacy policy URL
         :param pulumi.Input[str] links: (Read-only) Link relations for this object - JSON HAL - Discoverable resources related to the brand
+        :param pulumi.Input[str] name: Brand name
         :param pulumi.Input[bool] remove_powered_by_okta: (Optional) Removes "Powered by Okta" from the Okta-hosted sign-in page, and "© 2021 Okta, Inc." from the Okta End-User Dashboard
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _BrandState.__new__(_BrandState)
 
         __props__.__dict__["agree_to_custom_privacy_policy"] = agree_to_custom_privacy_policy
         __props__.__dict__["brand_id"] = brand_id
         __props__.__dict__["custom_privacy_policy_url"] = custom_privacy_policy_url
         __props__.__dict__["links"] = links
+        __props__.__dict__["name"] = name
         __props__.__dict__["remove_powered_by_okta"] = remove_powered_by_okta
         return Brand(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="agreeToCustomPrivacyPolicy")
     def agree_to_custom_privacy_policy(self) -> pulumi.Output[Optional[bool]]:
         """
@@ -341,14 +361,22 @@
     def links(self) -> pulumi.Output[str]:
         """
         (Read-only) Link relations for this object - JSON HAL - Discoverable resources related to the brand
         """
         return pulumi.get(self, "links")
 
     @property
+    @pulumi.getter
+    def name(self) -> pulumi.Output[str]:
+        """
+        Brand name
+        """
+        return pulumi.get(self, "name")
+
+    @property
     @pulumi.getter(name="removePoweredByOkta")
     def remove_powered_by_okta(self) -> pulumi.Output[Optional[bool]]:
         """
         (Optional) Removes "Powered by Okta" from the Okta-hosted sign-in page, and "© 2021 Okta, Inc." from the Okta End-User Dashboard
         """
         return pulumi.get(self, "remove_powered_by_okta")
```

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/captcha.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/captcha.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/captcha_org_wide_settings.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/captcha_org_wide_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/config/vars.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/domain.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/domain_certificate.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/domain_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/domain_verification.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/domain_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/email_customization.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/email_customization.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/email_sender.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/email_sender.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/email_sender_verification.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/email_sender_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/event_hook.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/event_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/event_hook_verification.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/event_hook_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/factor/factor.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/factor/factor.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/factor_totp.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/factor_totp.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/get_app_group_assignments.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_app_group_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/get_app_signon_policy.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_app_signon_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/get_app_user_assignments.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_app_user_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/get_auth_server_claim.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_auth_server_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/get_auth_server_claims.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_auth_server_claims.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/get_authenticator.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_authenticator.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/get_behaviour.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_behaviour.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/get_behaviours.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_behaviours.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/get_brand.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_brand.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,27 +17,30 @@
 ]
 
 @pulumi.output_type
 class GetBrandResult:
     """
     A collection of values returned by getBrand.
     """
-    def __init__(__self__, brand_id=None, custom_privacy_policy_url=None, id=None, links=None, remove_powered_by_okta=None):
+    def __init__(__self__, brand_id=None, custom_privacy_policy_url=None, id=None, links=None, name=None, remove_powered_by_okta=None):
         if brand_id and not isinstance(brand_id, str):
             raise TypeError("Expected argument 'brand_id' to be a str")
         pulumi.set(__self__, "brand_id", brand_id)
         if custom_privacy_policy_url and not isinstance(custom_privacy_policy_url, str):
             raise TypeError("Expected argument 'custom_privacy_policy_url' to be a str")
         pulumi.set(__self__, "custom_privacy_policy_url", custom_privacy_policy_url)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if links and not isinstance(links, str):
             raise TypeError("Expected argument 'links' to be a str")
         pulumi.set(__self__, "links", links)
+        if name and not isinstance(name, str):
+            raise TypeError("Expected argument 'name' to be a str")
+        pulumi.set(__self__, "name", name)
         if remove_powered_by_okta and not isinstance(remove_powered_by_okta, bool):
             raise TypeError("Expected argument 'remove_powered_by_okta' to be a bool")
         pulumi.set(__self__, "remove_powered_by_okta", remove_powered_by_okta)
 
     @property
     @pulumi.getter(name="brandId")
     def brand_id(self) -> str:
@@ -64,14 +67,19 @@
     def links(self) -> str:
         """
         Link relations for this object - JSON HAL - Discoverable resources related to the brand
         """
         return pulumi.get(self, "links")
 
     @property
+    @pulumi.getter
+    def name(self) -> str:
+        return pulumi.get(self, "name")
+
+    @property
     @pulumi.getter(name="removePoweredByOkta")
     def remove_powered_by_okta(self) -> bool:
         """
         Removes "Powered by Okta" from the Okta-hosted sign-in page, and "© 2021 Okta, Inc." from the Okta End-User Dashboard
         """
         return pulumi.get(self, "remove_powered_by_okta")
 
@@ -82,14 +90,15 @@
         if False:
             yield self
         return GetBrandResult(
             brand_id=self.brand_id,
             custom_privacy_policy_url=self.custom_privacy_policy_url,
             id=self.id,
             links=self.links,
+            name=self.name,
             remove_powered_by_okta=self.remove_powered_by_okta)
 
 
 def get_brand(brand_id: Optional[str] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetBrandResult:
     """
     Use this data source to retrieve a [Brand](https://developer.okta.com/docs/reference/api/brands/#brand-object) from Okta.
@@ -103,14 +112,15 @@
     __ret__ = pulumi.runtime.invoke('okta:index/getBrand:getBrand', __args__, opts=opts, typ=GetBrandResult).value
 
     return AwaitableGetBrandResult(
         brand_id=__ret__.brand_id,
         custom_privacy_policy_url=__ret__.custom_privacy_policy_url,
         id=__ret__.id,
         links=__ret__.links,
+        name=__ret__.name,
         remove_powered_by_okta=__ret__.remove_powered_by_okta)
 
 
 @_utilities.lift_output_func(get_brand)
 def get_brand_output(brand_id: Optional[pulumi.Input[str]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetBrandResult]:
     """
```

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/get_brands.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_brands.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/get_email_customization.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_email_customization.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/get_email_customizations.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_email_customizations.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/get_groups.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/get_network_zone.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_network_zone.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ]
 
 @pulumi.output_type
 class GetNetworkZoneResult:
     """
     A collection of values returned by getNetworkZone.
     """
-    def __init__(__self__, asns=None, dynamic_locations=None, dynamic_proxy_type=None, gateways=None, id=None, name=None, proxies=None, type=None, usage=None):
+    def __init__(__self__, asns=None, dynamic_locations=None, dynamic_proxy_type=None, gateways=None, id=None, name=None, proxies=None, status=None, type=None, usage=None):
         if asns and not isinstance(asns, list):
             raise TypeError("Expected argument 'asns' to be a list")
         pulumi.set(__self__, "asns", asns)
         if dynamic_locations and not isinstance(dynamic_locations, list):
             raise TypeError("Expected argument 'dynamic_locations' to be a list")
         pulumi.set(__self__, "dynamic_locations", dynamic_locations)
         if dynamic_proxy_type and not isinstance(dynamic_proxy_type, str):
@@ -39,14 +39,17 @@
         pulumi.set(__self__, "id", id)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
         if proxies and not isinstance(proxies, list):
             raise TypeError("Expected argument 'proxies' to be a list")
         pulumi.set(__self__, "proxies", proxies)
+        if status and not isinstance(status, str):
+            raise TypeError("Expected argument 'status' to be a str")
+        pulumi.set(__self__, "status", status)
         if type and not isinstance(type, str):
             raise TypeError("Expected argument 'type' to be a str")
         pulumi.set(__self__, "type", type)
         if usage and not isinstance(usage, str):
             raise TypeError("Expected argument 'usage' to be a str")
         pulumi.set(__self__, "usage", usage)
 
@@ -104,14 +107,22 @@
         """
         Array of values in CIDR/range form.
         """
         return pulumi.get(self, "proxies")
 
     @property
     @pulumi.getter
+    def status(self) -> str:
+        """
+        Network Status - can either be ACTIVE or INACTIVE only.
+        """
+        return pulumi.get(self, "status")
+
+    @property
+    @pulumi.getter
     def type(self) -> str:
         """
         Type of the Network Zone.
         """
         return pulumi.get(self, "type")
 
     @property
@@ -132,14 +143,15 @@
             asns=self.asns,
             dynamic_locations=self.dynamic_locations,
             dynamic_proxy_type=self.dynamic_proxy_type,
             gateways=self.gateways,
             id=self.id,
             name=self.name,
             proxies=self.proxies,
+            status=self.status,
             type=self.type,
             usage=self.usage)
 
 
 def get_network_zone(id: Optional[str] = None,
                      name: Optional[str] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetNetworkZoneResult:
@@ -169,14 +181,15 @@
         asns=__ret__.asns,
         dynamic_locations=__ret__.dynamic_locations,
         dynamic_proxy_type=__ret__.dynamic_proxy_type,
         gateways=__ret__.gateways,
         id=__ret__.id,
         name=__ret__.name,
         proxies=__ret__.proxies,
+        status=__ret__.status,
         type=__ret__.type,
         usage=__ret__.usage)
 
 
 @_utilities.lift_output_func(get_network_zone)
 def get_network_zone_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                             name: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/get_role_subscription.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_role_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/get_template.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/get_templates.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_templates.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/get_theme.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/get_themes.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_themes.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/get_trusted_origins.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_trusted_origins.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/get_user_security_questions.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_user_security_questions.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/group/get_everyone_group.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/group/get_everyone_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/group/get_group.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/group/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/group/group.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/group/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/group/role.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/group/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/group/rule.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/group/rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/group_memberships.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/group_schema_property.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/group_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/idp/get_metadata_saml.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/get_metadata_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/idp/get_oidc.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/get_oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/idp/get_saml.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/get_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/idp/get_social.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/get_social.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/idp/oidc.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/idp/saml.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/idp/saml_key.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/saml_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/idp/social.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/social.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/index/email_domain.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/index/email_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/index/email_domain_verification.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/index/email_domain_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/index/get_domain.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/index/get_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/index/outputs.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/index/outputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,27 +33,29 @@
         EmailDomainDnsValidationRecord.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  expiration: Optional[str] = None,
                  fqdn: Optional[str] = None,
                  record_type: Optional[str] = None,
-                 values: Optional[Sequence[str]] = None):
+                 value: Optional[str] = None):
         """
         :param str fqdn: DNS record name.
         :param str record_type: Record type can be TXT or cname.
+        :param str value: DNS record value
+               - `expiration ` - DNS TXT record expiration
         """
         if expiration is not None:
             pulumi.set(__self__, "expiration", expiration)
         if fqdn is not None:
             pulumi.set(__self__, "fqdn", fqdn)
         if record_type is not None:
             pulumi.set(__self__, "record_type", record_type)
-        if values is not None:
-            pulumi.set(__self__, "values", values)
+        if value is not None:
+            pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def expiration(self) -> Optional[str]:
         return pulumi.get(self, "expiration")
 
     @property
@@ -70,16 +72,20 @@
         """
         Record type can be TXT or cname.
         """
         return pulumi.get(self, "record_type")
 
     @property
     @pulumi.getter
-    def values(self) -> Optional[Sequence[str]]:
-        return pulumi.get(self, "values")
+    def value(self) -> Optional[str]:
+        """
+        DNS record value
+        - `expiration ` - DNS TXT record expiration
+        """
+        return pulumi.get(self, "value")
 
 
 @pulumi.output_type
 class GetDomainDnsRecordResult(dict):
     def __init__(__self__, *,
                  expiration: str,
                  fqdn: str,
```

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/inline/_inputs.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/inline/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/inline/hook.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/inline/hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/inline/outputs.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/inline/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/link_definition.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/link_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/link_value.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/link_value.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/network/zone.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/network/zone.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,25 +17,27 @@
                  type: pulumi.Input[str],
                  asns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  dynamic_locations: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  dynamic_proxy_type: Optional[pulumi.Input[str]] = None,
                  gateways: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  proxies: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 status: Optional[pulumi.Input[str]] = None,
                  usage: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Zone resource.
         :param pulumi.Input[str] type: Type of the Network Zone - can either be `"IP"` or `"DYNAMIC"` only.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] asns: Array of Autonomous System Numbers (each element is a string representation of an ASN numeric value).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] dynamic_locations: Array of locations [ISO-3166-1](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)
                and [ISO-3166-2](https://en.wikipedia.org/wiki/ISO_3166-2). Format code: countryCode OR countryCode-regionCode.
         :param pulumi.Input[str] dynamic_proxy_type: Type of proxy being controlled by this dynamic network zone - can be one of `Any`, `TorAnonymizer` or `NotTorAnonymizer`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] gateways: Array of values in CIDR/range form.
         :param pulumi.Input[str] name: Name of the Network Zone Resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] proxies: Array of values in CIDR/range form. Can not be set if `usage` is set to `"BLOCKLIST"`.
+        :param pulumi.Input[str] status: Network Status - can either be ACTIVE or INACTIVE only.
         :param pulumi.Input[str] usage: Usage of the Network Zone - can be either `"POLICY"` or `"BLOCKLIST"`. By default, it is `"POLICY"`.
         """
         pulumi.set(__self__, "type", type)
         if asns is not None:
             pulumi.set(__self__, "asns", asns)
         if dynamic_locations is not None:
             pulumi.set(__self__, "dynamic_locations", dynamic_locations)
@@ -43,14 +45,16 @@
             pulumi.set(__self__, "dynamic_proxy_type", dynamic_proxy_type)
         if gateways is not None:
             pulumi.set(__self__, "gateways", gateways)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if proxies is not None:
             pulumi.set(__self__, "proxies", proxies)
+        if status is not None:
+            pulumi.set(__self__, "status", status)
         if usage is not None:
             pulumi.set(__self__, "usage", usage)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
         """
@@ -133,14 +137,26 @@
 
     @proxies.setter
     def proxies(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "proxies", value)
 
     @property
     @pulumi.getter
+    def status(self) -> Optional[pulumi.Input[str]]:
+        """
+        Network Status - can either be ACTIVE or INACTIVE only.
+        """
+        return pulumi.get(self, "status")
+
+    @status.setter
+    def status(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "status", value)
+
+    @property
+    @pulumi.getter
     def usage(self) -> Optional[pulumi.Input[str]]:
         """
         Usage of the Network Zone - can be either `"POLICY"` or `"BLOCKLIST"`. By default, it is `"POLICY"`.
         """
         return pulumi.get(self, "usage")
 
     @usage.setter
@@ -153,25 +169,27 @@
     def __init__(__self__, *,
                  asns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  dynamic_locations: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  dynamic_proxy_type: Optional[pulumi.Input[str]] = None,
                  gateways: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  proxies: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 status: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  usage: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Zone resources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] asns: Array of Autonomous System Numbers (each element is a string representation of an ASN numeric value).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] dynamic_locations: Array of locations [ISO-3166-1](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)
                and [ISO-3166-2](https://en.wikipedia.org/wiki/ISO_3166-2). Format code: countryCode OR countryCode-regionCode.
         :param pulumi.Input[str] dynamic_proxy_type: Type of proxy being controlled by this dynamic network zone - can be one of `Any`, `TorAnonymizer` or `NotTorAnonymizer`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] gateways: Array of values in CIDR/range form.
         :param pulumi.Input[str] name: Name of the Network Zone Resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] proxies: Array of values in CIDR/range form. Can not be set if `usage` is set to `"BLOCKLIST"`.
+        :param pulumi.Input[str] status: Network Status - can either be ACTIVE or INACTIVE only.
         :param pulumi.Input[str] type: Type of the Network Zone - can either be `"IP"` or `"DYNAMIC"` only.
         :param pulumi.Input[str] usage: Usage of the Network Zone - can be either `"POLICY"` or `"BLOCKLIST"`. By default, it is `"POLICY"`.
         """
         if asns is not None:
             pulumi.set(__self__, "asns", asns)
         if dynamic_locations is not None:
             pulumi.set(__self__, "dynamic_locations", dynamic_locations)
@@ -179,14 +197,16 @@
             pulumi.set(__self__, "dynamic_proxy_type", dynamic_proxy_type)
         if gateways is not None:
             pulumi.set(__self__, "gateways", gateways)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if proxies is not None:
             pulumi.set(__self__, "proxies", proxies)
+        if status is not None:
+            pulumi.set(__self__, "status", status)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if usage is not None:
             pulumi.set(__self__, "usage", usage)
 
     @property
     @pulumi.getter
@@ -259,14 +279,26 @@
 
     @proxies.setter
     def proxies(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "proxies", value)
 
     @property
     @pulumi.getter
+    def status(self) -> Optional[pulumi.Input[str]]:
+        """
+        Network Status - can either be ACTIVE or INACTIVE only.
+        """
+        return pulumi.get(self, "status")
+
+    @status.setter
+    def status(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "status", value)
+
+    @property
+    @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
         Type of the Network Zone - can either be `"IP"` or `"DYNAMIC"` only.
         """
         return pulumi.get(self, "type")
 
     @type.setter
@@ -293,14 +325,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  asns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  dynamic_locations: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  dynamic_proxy_type: Optional[pulumi.Input[str]] = None,
                  gateways: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  proxies: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 status: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  usage: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Creates an Okta Network Zone.
 
         This resource allows you to create and configure an Okta Network Zone.
@@ -347,14 +380,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] asns: Array of Autonomous System Numbers (each element is a string representation of an ASN numeric value).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] dynamic_locations: Array of locations [ISO-3166-1](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)
                and [ISO-3166-2](https://en.wikipedia.org/wiki/ISO_3166-2). Format code: countryCode OR countryCode-regionCode.
         :param pulumi.Input[str] dynamic_proxy_type: Type of proxy being controlled by this dynamic network zone - can be one of `Any`, `TorAnonymizer` or `NotTorAnonymizer`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] gateways: Array of values in CIDR/range form.
         :param pulumi.Input[str] name: Name of the Network Zone Resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] proxies: Array of values in CIDR/range form. Can not be set if `usage` is set to `"BLOCKLIST"`.
+        :param pulumi.Input[str] status: Network Status - can either be ACTIVE or INACTIVE only.
         :param pulumi.Input[str] type: Type of the Network Zone - can either be `"IP"` or `"DYNAMIC"` only.
         :param pulumi.Input[str] usage: Usage of the Network Zone - can be either `"POLICY"` or `"BLOCKLIST"`. By default, it is `"POLICY"`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -419,14 +453,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  asns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  dynamic_locations: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  dynamic_proxy_type: Optional[pulumi.Input[str]] = None,
                  gateways: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  proxies: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 status: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  usage: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
@@ -436,14 +471,15 @@
 
             __props__.__dict__["asns"] = asns
             __props__.__dict__["dynamic_locations"] = dynamic_locations
             __props__.__dict__["dynamic_proxy_type"] = dynamic_proxy_type
             __props__.__dict__["gateways"] = gateways
             __props__.__dict__["name"] = name
             __props__.__dict__["proxies"] = proxies
+            __props__.__dict__["status"] = status
             if type is None and not opts.urn:
                 raise TypeError("Missing required property 'type'")
             __props__.__dict__["type"] = type
             __props__.__dict__["usage"] = usage
         super(Zone, __self__).__init__(
             'okta:network/zone:Zone',
             resource_name,
@@ -456,14 +492,15 @@
             opts: Optional[pulumi.ResourceOptions] = None,
             asns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             dynamic_locations: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             dynamic_proxy_type: Optional[pulumi.Input[str]] = None,
             gateways: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             name: Optional[pulumi.Input[str]] = None,
             proxies: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            status: Optional[pulumi.Input[str]] = None,
             type: Optional[pulumi.Input[str]] = None,
             usage: Optional[pulumi.Input[str]] = None) -> 'Zone':
         """
         Get an existing Zone resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
@@ -472,27 +509,29 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] asns: Array of Autonomous System Numbers (each element is a string representation of an ASN numeric value).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] dynamic_locations: Array of locations [ISO-3166-1](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)
                and [ISO-3166-2](https://en.wikipedia.org/wiki/ISO_3166-2). Format code: countryCode OR countryCode-regionCode.
         :param pulumi.Input[str] dynamic_proxy_type: Type of proxy being controlled by this dynamic network zone - can be one of `Any`, `TorAnonymizer` or `NotTorAnonymizer`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] gateways: Array of values in CIDR/range form.
         :param pulumi.Input[str] name: Name of the Network Zone Resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] proxies: Array of values in CIDR/range form. Can not be set if `usage` is set to `"BLOCKLIST"`.
+        :param pulumi.Input[str] status: Network Status - can either be ACTIVE or INACTIVE only.
         :param pulumi.Input[str] type: Type of the Network Zone - can either be `"IP"` or `"DYNAMIC"` only.
         :param pulumi.Input[str] usage: Usage of the Network Zone - can be either `"POLICY"` or `"BLOCKLIST"`. By default, it is `"POLICY"`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ZoneState.__new__(_ZoneState)
 
         __props__.__dict__["asns"] = asns
         __props__.__dict__["dynamic_locations"] = dynamic_locations
         __props__.__dict__["dynamic_proxy_type"] = dynamic_proxy_type
         __props__.__dict__["gateways"] = gateways
         __props__.__dict__["name"] = name
         __props__.__dict__["proxies"] = proxies
+        __props__.__dict__["status"] = status
         __props__.__dict__["type"] = type
         __props__.__dict__["usage"] = usage
         return Zone(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def asns(self) -> pulumi.Output[Optional[Sequence[str]]]:
@@ -540,14 +579,22 @@
         """
         Array of values in CIDR/range form. Can not be set if `usage` is set to `"BLOCKLIST"`.
         """
         return pulumi.get(self, "proxies")
 
     @property
     @pulumi.getter
+    def status(self) -> pulumi.Output[Optional[str]]:
+        """
+        Network Status - can either be ACTIVE or INACTIVE only.
+        """
+        return pulumi.get(self, "status")
+
+    @property
+    @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
         Type of the Network Zone - can either be `"IP"` or `"DYNAMIC"` only.
         """
         return pulumi.get(self, "type")
 
     @property
```

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/org_configuration.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/org_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/org_support.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/org_support.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/outputs.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -765,18 +765,20 @@
 
 @pulumi.output_type
 class GetBrandsBrandResult(dict):
     def __init__(__self__, *,
                  custom_privacy_policy_url: str,
                  id: str,
                  links: str,
+                 name: str,
                  remove_powered_by_okta: bool):
         pulumi.set(__self__, "custom_privacy_policy_url", custom_privacy_policy_url)
         pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "links", links)
+        pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "remove_powered_by_okta", remove_powered_by_okta)
 
     @property
     @pulumi.getter(name="customPrivacyPolicyUrl")
     def custom_privacy_policy_url(self) -> str:
         return pulumi.get(self, "custom_privacy_policy_url")
 
@@ -787,14 +789,19 @@
 
     @property
     @pulumi.getter
     def links(self) -> str:
         return pulumi.get(self, "links")
 
     @property
+    @pulumi.getter
+    def name(self) -> str:
+        return pulumi.get(self, "name")
+
+    @property
     @pulumi.getter(name="removePoweredByOkta")
     def remove_powered_by_okta(self) -> bool:
         return pulumi.get(self, "remove_powered_by_okta")
 
 
 @pulumi.output_type
 class GetEmailCustomizationsEmailCustomizationResult(dict):
```

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/__init__.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/_inputs.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/get_default_policy.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/get_default_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/get_policy.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/get_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/mfa.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/mfa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/outputs.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/password.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/password.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/rule_idp_discovery.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/rule_idp_discovery.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/rule_mfa.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/rule_mfa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/rule_password.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/rule_password.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/rule_signon.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/rule_signon.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/policy/signon.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/signon.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/policy_mfa_default.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy_mfa_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/policy_password_default.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy_password_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/policy_profile_enrollment.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy_profile_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/policy_profile_enrollment_apps.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy_profile_enrollment_apps.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/policy_rule_profile_enrollment.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy_rule_profile_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/profile/_inputs.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/profile/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/profile/mapping.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/profile/mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/profile/outputs.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/profile/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/provider.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/rate_limiting.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/resource_set.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/resource_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/role_subscription.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/role_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/security_notification_emails.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/security_notification_emails.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/template_sms.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/template_sms.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/theme.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/threat_insight_settings.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/threat_insight_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/trustedorigin/origin.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/trustedorigin/origin.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/user/_inputs.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/user/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/user/get_user.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/user/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/user/get_user_profile_mapping_source.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/user/get_user_profile_mapping_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/user/get_user_type.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/user/get_user_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/user/get_users.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/user/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/user/outputs.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/user/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/user/user.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/user/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/user/user_type.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/user/user_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/user_admin_roles.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/user_admin_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/user_base_schema_property.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/user_base_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/user_factor_question.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/user_factor_question.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/user_group_memberships.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/user_group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta/user_schema_property.py` & `pulumi_okta-4.1.0a1687800548/pulumi_okta/user_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta.egg-info/PKG-INFO` & `pulumi_okta-4.1.0a1687800548/pulumi_okta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-okta
-Version: 4.1.0a1687672875
+Version: 4.1.0a1687800548
 Summary: A Pulumi package for creating and managing okta resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-okta
 Keywords: pulumi okta
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_okta-4.1.0a1687672875/pulumi_okta.egg-info/SOURCES.txt` & `pulumi_okta-4.1.0a1687800548/pulumi_okta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687672875/setup.py` & `pulumi_okta-4.1.0a1687800548/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.1.0a1687672875"
-PLUGIN_VERSION = "4.1.0-alpha.1687672875+3da11109"
+VERSION = "4.1.0a1687800548"
+PLUGIN_VERSION = "4.1.0-alpha.1687800548+cc3da24f"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'okta', PLUGIN_VERSION])
         except OSError as error:
```

