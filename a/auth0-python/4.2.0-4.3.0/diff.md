# Comparing `tmp/auth0-python-4.2.0.tar.gz` & `tmp/auth0-python-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth0-python-4.2.0.tar", last modified: Tue May  2 17:27:39 2023, max compression
+gzip compressed data, was "auth0-python-4.3.0.tar", last modified: Mon Jun 26 15:34:12 2023, max compression
```

## Comparing `auth0-python-4.2.0.tar` & `auth0-python-4.3.0.tar`

### file list

```diff
@@ -1,120 +1,121 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:39.080303 auth0-python-4.2.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1121 2023-05-02 17:27:38.000000 auth0-python-4.2.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8806 2023-05-02 17:27:39.080303 auth0-python-4.2.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8039 2023-05-02 17:27:38.000000 auth0-python-4.2.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:39.068303 auth0-python-4.2.0/auth0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      169 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2776 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/asyncify.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:39.068303 auth0-python-4.2.0/auth0/authentication/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      408 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6779 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/async_token_verifier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2439 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2498 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/client_authentication.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2794 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/database.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1073 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/delegated.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      654 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/enterprise.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7777 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/get_token.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2268 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/passwordless.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      958 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/revoke_token.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1137 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/social.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15298 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/token_verifier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1499 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/users.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      572 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/exceptions.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:39.072303 auth0-python-4.2.0/auth0/management/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1689 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7908 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/actions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1672 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/async_auth0.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3762 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/attack_protection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3910 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/auth0.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2069 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/blacklists.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4670 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/branding.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2818 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/client_credentials.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3447 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/client_grants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5304 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/clients.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5595 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/connections.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2700 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/custom_domains.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3687 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/device_credentials.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2834 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/email_templates.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2831 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/emails.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2750 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/grants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5042 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/guardian.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5866 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/hooks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4551 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/jobs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2818 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/log_streams.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3742 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/logs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13772 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/organizations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2348 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/prompts.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3473 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/resource_servers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7165 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/roles.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4877 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/rules.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2256 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/rules_configs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2039 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/stats.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2228 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/tenants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1893 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/tickets.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2608 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/user_blocks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18274 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/users.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2048 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/users_by_email.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10884 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/rest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4919 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/rest_async.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:39.072303 auth0-python-4.2.0/auth0/test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:39.072303 auth0-python-4.2.0/auth0/test/authentication/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/authentication/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11856 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/authentication/test_base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2446 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/authentication/test_database.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2052 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/authentication/test_delegated.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      789 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/authentication/test_enterprise.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8225 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/authentication/test_get_token.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3038 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/authentication/test_passwordless.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      936 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/authentication/test_revoke_token.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1301 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/authentication/test_social.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    33387 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/authentication/test_token_verifier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      433 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/authentication/test_users.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:39.076303 auth0-python-4.2.0/auth0/test/management/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8426 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_actions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3585 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_atack_protection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4545 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_auth0.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1578 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_blacklists.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4476 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_branding.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1992 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_client_credentials.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3770 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_client_grants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4428 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_clients.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5887 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_connections.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1989 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_custom_domains.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2794 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_device_credentials.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1674 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_email_endpoints.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2271 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_emails.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1449 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_grants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5181 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_guardian.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5649 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_hooks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3542 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_jobs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2781 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_log_streams.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1954 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_logs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15308 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_organizations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2168 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_prompts.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2910 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_resource_servers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    30831 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_rest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6515 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_roles.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4115 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_rules.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1546 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_rules_configs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1364 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_stats.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1867 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_tenants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1236 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_tickets.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2080 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_user_blocks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14460 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_users.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1398 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_users_by_email.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:39.080303 auth0-python-4.2.0/auth0/test_async/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test_async/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2250 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test_async/test_async_auth0.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10099 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test_async/test_async_token_verifier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6618 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test_async/test_asyncify.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      178 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:39.080303 auth0-python-4.2.0/auth0_python.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8806 2023-05-02 17:27:39.000000 auth0-python-4.2.0/auth0_python.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3750 2023-05-02 17:27:39.000000 auth0-python-4.2.0/auth0_python.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-02 17:27:39.000000 auth0-python-4.2.0/auth0_python.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       66 2023-05-02 17:27:39.000000 auth0-python-4.2.0/auth0_python.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-05-02 17:27:39.000000 auth0-python-4.2.0/auth0_python.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-05-02 17:27:39.080303 auth0-python-4.2.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1454 2023-05-02 17:27:38.000000 auth0-python-4.2.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:12.106607 auth0-python-4.3.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1121 2023-06-26 15:34:11.000000 auth0-python-4.3.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8806 2023-06-26 15:34:12.106607 auth0-python-4.3.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8039 2023-06-26 15:34:11.000000 auth0-python-4.3.0/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:12.094607 auth0-python-4.3.0/auth0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      169 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3138 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/asyncify.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:12.098607 auth0-python-4.3.0/auth0/authentication/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      408 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7385 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/async_token_verifier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2958 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2684 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/client_authentication.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3101 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/database.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1190 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/delegated.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      692 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/enterprise.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8511 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/get_token.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2397 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/passwordless.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      994 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/revoke_token.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1185 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/social.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16375 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/token_verifier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1697 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/users.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      747 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/exceptions.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:12.102607 auth0-python-4.3.0/auth0/management/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1689 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7908 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/actions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1672 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/async_auth0.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3762 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/attack_protection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3910 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/auth0.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2069 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/blacklists.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4670 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/branding.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2818 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/client_credentials.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3447 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/client_grants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5304 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/clients.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5716 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/connections.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2700 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/custom_domains.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3687 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/device_credentials.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2834 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/email_templates.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2831 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/emails.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2750 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/grants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5042 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/guardian.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5866 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/hooks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4551 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/jobs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2818 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/log_streams.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3742 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/logs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13772 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/organizations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2348 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/prompts.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3473 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/resource_servers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7165 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/roles.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4877 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/rules.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2256 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/rules_configs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2039 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/stats.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2228 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/tenants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1893 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/tickets.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2608 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/user_blocks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18274 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/users.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2048 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/users_by_email.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11953 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/rest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5710 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/rest_async.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:12.102607 auth0-python-4.3.0/auth0/test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:12.102607 auth0-python-4.3.0/auth0/test/authentication/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/authentication/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11856 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/authentication/test_base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2446 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/authentication/test_database.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2052 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/authentication/test_delegated.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      789 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/authentication/test_enterprise.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8743 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/authentication/test_get_token.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3038 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/authentication/test_passwordless.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      936 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/authentication/test_revoke_token.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1301 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/authentication/test_social.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    33387 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/authentication/test_token_verifier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      433 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/authentication/test_users.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:12.106607 auth0-python-4.3.0/auth0/test/management/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8426 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_actions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3585 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_atack_protection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4545 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_auth0.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1578 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_blacklists.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4537 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_branding.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1992 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_client_credentials.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3770 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_client_grants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4428 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_clients.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6501 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_connections.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1989 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_custom_domains.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2794 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_device_credentials.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1674 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_email_endpoints.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2271 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_emails.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1449 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_grants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5181 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_guardian.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5649 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_hooks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3542 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_jobs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2781 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_log_streams.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1954 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_logs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15308 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_organizations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2168 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_prompts.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2910 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_resource_servers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    30831 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_rest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6515 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_roles.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4115 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_rules.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1546 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_rules_configs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1364 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_stats.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1867 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_tenants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1236 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_tickets.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2080 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_user_blocks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14460 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_users.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1398 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_users_by_email.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:12.106607 auth0-python-4.3.0/auth0/test_async/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test_async/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2250 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test_async/test_async_auth0.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10099 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test_async/test_async_token_verifier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7641 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test_async/test_asyncify.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/types.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      186 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:12.106607 auth0-python-4.3.0/auth0_python.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8806 2023-06-26 15:34:12.000000 auth0-python-4.3.0/auth0_python.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3765 2023-06-26 15:34:12.000000 auth0-python-4.3.0/auth0_python.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-26 15:34:12.000000 auth0-python-4.3.0/auth0_python.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       66 2023-06-26 15:34:12.000000 auth0-python-4.3.0/auth0_python.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-06-26 15:34:12.000000 auth0-python-4.3.0/auth0_python.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-26 15:34:12.106607 auth0-python-4.3.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1454 2023-06-26 15:34:11.000000 auth0-python-4.3.0/setup.py
```

### Comparing `auth0-python-4.2.0/LICENSE` & `auth0-python-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/PKG-INFO` & `auth0-python-4.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth0-python
-Version: 4.2.0
+Version: 4.3.0
 Summary: Auth0 Python SDK
 Home-page: https://github.com/auth0/auth0-python
 Author: Auth0
 Author-email: support@auth0.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: auth0-python Version: 4.2.0 Summary: Auth0 Python
+Metadata-Version: 2.1 Name: auth0-python Version: 4.3.0 Summary: Auth0 Python
 SDK Home-page: https://github.com/auth0/auth0-python Author: Auth0 Author-
 email: support@auth0.com License: MIT Platform: UNKNOWN Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `auth0-python-4.2.0/README.md` & `auth0-python-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/asyncify.py` & `auth0-python-4.3.0/auth0/management/tickets.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,92 +1,62 @@
-import aiohttp
+from ..rest import RestClient
 
-from auth0.rest_async import AsyncRestClient
 
+class Tickets:
+    """Auth0 tickets endpoints
 
-def _gen_async(client, method):
-    m = getattr(client, method)
+    Args:
+        domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
 
-    async def closure(*args, **kwargs):
-        return await m(*args, **kwargs)
-
-    return closure
-
-
-def asyncify(cls):
-    methods = [
-        func
-        for func in dir(cls)
-        if callable(getattr(cls, func)) and not func.startswith("_")
-    ]
-
-    class AsyncClient(cls):
-        def __init__(
-            self,
-            domain,
-            token,
-            telemetry=True,
-            timeout=5.0,
-            protocol="https",
-            rest_options=None,
-        ):
-            if token is None:
-                # Wrap the auth client
-                super().__init__(domain, telemetry, timeout, protocol)
-            else:
-                # Wrap the mngtmt client
-                super().__init__(
-                    domain, token, telemetry, timeout, protocol, rest_options
-                )
-            self.client = AsyncRestClient(
-                jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
-            )
-
-    class Wrapper(cls):
-        def __init__(
-            self,
-            domain,
-            token=None,
-            telemetry=True,
-            timeout=5.0,
-            protocol="https",
-            rest_options=None,
-        ):
-            if token is None:
-                # Wrap the auth client
-                super().__init__(domain, telemetry, timeout, protocol)
-            else:
-                # Wrap the mngtmt client
-                super().__init__(
-                    domain, token, telemetry, timeout, protocol, rest_options
-                )
-
-            self._async_client = AsyncClient(
-                domain, token, telemetry, timeout, protocol, rest_options
-            )
-            for method in methods:
-                setattr(
-                    self,
-                    f"{method}_async",
-                    _gen_async(self._async_client, method),
-                )
-
-        def set_session(self, session):
-            """Set Client Session to improve performance by reusing session.
-
-            Args:
-                session (aiohttp.ClientSession): The client session which should be closed
-                    manually or within context manager.
-            """
-            self._session = session
-            self._async_client.client.set_session(self._session)
-
-        async def __aenter__(self):
-            """Automatically create and set session within context manager."""
-            self.set_session(aiohttp.ClientSession())
-            return self
-
-        async def __aexit__(self, exc_type, exc_val, exc_tb):
-            """Automatically close session within context manager."""
-            await self._session.close()
-
-    return Wrapper
+        token (str): Management API v2 Token
+
+        telemetry (bool, optional): Enable or disable Telemetry
+            (defaults to True)
+
+        timeout (float or tuple, optional): Change the requests
+            connect and read timeout. Pass a tuple to specify
+            both values separately or a float to set both to it.
+            (defaults to 5.0 for both)
+
+        rest_options (RestClientOptions): Pass an instance of
+            RestClientOptions to configure additional RestClient
+            options, such as rate-limit retries.
+            (defaults to None)
+    """
+
+    def __init__(
+        self,
+        domain,
+        token,
+        telemetry=True,
+        timeout=5.0,
+        protocol="https",
+        rest_options=None,
+    ):
+        self.domain = domain
+        self.protocol = protocol
+        self.client = RestClient(
+            jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
+        )
+
+    def _url(self, action):
+        return f"{self.protocol}://{self.domain}/api/v2/tickets/{action}"
+
+    def create_email_verification(self, body):
+        """Create an email verification ticket.
+
+        Args:
+            body (dict): attributes to set on the email verification request.
+
+        See: https://auth0.com/docs/api/v2#!/Tickets/post_email_verification
+        """
+        return self.client.post(self._url("email-verification"), data=body)
+
+    def create_pswd_change(self, body):
+        """Create password change ticket.
+
+        Args:
+            body (dict): attributes to set on the password change request.
+
+        See: https://auth0.com/docs/api/v2#!/Tickets/post_password_change
+        """
+        return self.client.post(self._url("password-change"), data=body)
```

### Comparing `auth0-python-4.2.0/auth0/authentication/async_token_verifier.py` & `auth0-python-4.3.0/auth0/authentication/async_token_verifier.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 """Token Verifier module"""
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Any
+
 from .. import TokenValidationError
 from ..rest_async import AsyncRestClient
 from .token_verifier import AsymmetricSignatureVerifier, JwksFetcher, TokenVerifier
 
+if TYPE_CHECKING:
+    from aiohttp import ClientSession
+    from cryptography.hazmat.primitives.asymmetric.rsa import RSAPublicKey
+
 
 class AsyncAsymmetricSignatureVerifier(AsymmetricSignatureVerifier):
     """Async verifier for RSA signatures, which rely on public key certificates.
 
     Args:
         jwks_url (str): The url where the JWK set is located.
         algorithm (str, optional): The expected signing algorithm. Defaults to "RS256".
     """
 
-    def __init__(self, jwks_url, algorithm="RS256"):
+    def __init__(self, jwks_url: str, algorithm: str = "RS256") -> None:
         super().__init__(jwks_url, algorithm)
         self._fetcher = AsyncJwksFetcher(jwks_url)
 
-    def set_session(self, session):
+    def set_session(self, session: ClientSession) -> None:
         """Set Client Session to improve performance by reusing session.
 
         Args:
             session (aiohttp.ClientSession): The client session which should be closed
                 manually or within context manager.
         """
         self._fetcher.set_session(session)
@@ -28,15 +36,15 @@
     async def _fetch_key(self, key_id=None):
         """Request the JWKS.
 
         Args:
         key_id (str): The key's key id."""
         return await self._fetcher.get_key(key_id)
 
-    async def verify_signature(self, token):
+    async def verify_signature(self, token) -> dict[str, Any]:
         """Verifies the signature of the given JSON web token.
 
         Args:
             token (str): The JWT to get its signature verified.
 
         Raises:
             TokenValidationError: if the token cannot be decoded, the algorithm is invalid
@@ -53,28 +61,28 @@
     This class makes use of an in-memory cache. For it to work properly, define this instance once and re-use it.
 
     Args:
         jwks_url (str): The url where the JWK set is located.
         cache_ttl (str, optional): The lifetime of the JWK set cache in seconds. Defaults to 600 seconds.
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self._async_client = AsyncRestClient(None)
 
-    def set_session(self, session):
+    def set_session(self, session: ClientSession) -> None:
         """Set Client Session to improve performance by reusing session.
 
         Args:
             session (aiohttp.ClientSession): The client session which should be closed
                 manually or within context manager.
         """
         self._async_client.set_session(session)
 
-    async def _fetch_jwks(self, force=False):
+    async def _fetch_jwks(self, force: bool = False) -> dict[str, RSAPublicKey]:
         """Attempts to obtain the JWK set from the cache, as long as it's still valid.
         When not, it will perform a network request to the jwks_url to obtain a fresh result
         and update the cache value with it.
 
         Args:
             force (bool, optional): whether to ignore the cache and force a network request or not. Defaults to False.
         """
@@ -86,15 +94,15 @@
             except:  # noqa: E722
                 return self._cache_value
             return self._cache_value
 
         self._cache_is_fresh = False
         return self._cache_value
 
-    async def get_key(self, key_id):
+    async def get_key(self, key_id: str) -> RSAPublicKey:
         """Obtains the JWK associated with the given key id.
 
         Args:
             key_id (str): The id of the key to fetch.
 
         Returns:
             the JWK associated with the given key id.
@@ -122,38 +130,50 @@
         signature_verifier (AsyncAsymmetricSignatureVerifier): The instance that knows how to verify the signature.
         issuer (str): The expected issuer claim value.
         audience (str): The expected audience claim value.
         leeway (int, optional): The clock skew to accept when verifying date related claims in seconds.
         Defaults to 60 seconds.
     """
 
-    def __init__(self, signature_verifier, issuer, audience, leeway=0):
+    def __init__(
+        self,
+        signature_verifier: AsyncAsymmetricSignatureVerifier,
+        issuer: str,
+        audience: str,
+        leeway: int = 0,
+    ) -> None:
         if not signature_verifier or not isinstance(
             signature_verifier, AsyncAsymmetricSignatureVerifier
         ):
             raise TypeError(
                 "signature_verifier must be an instance of AsyncAsymmetricSignatureVerifier."
             )
 
         self.iss = issuer
         self.aud = audience
         self.leeway = leeway
         self._sv = signature_verifier
         self._clock = None  # legacy testing requirement
 
-    def set_session(self, session):
+    def set_session(self, session: ClientSession) -> None:
         """Set Client Session to improve performance by reusing session.
 
         Args:
             session (aiohttp.ClientSession): The client session which should be closed
                 manually or within context manager.
         """
         self._sv.set_session(session)
 
-    async def verify(self, token, nonce=None, max_age=None, organization=None):
+    async def verify(
+        self,
+        token: str,
+        nonce: str | None = None,
+        max_age: int | None = None,
+        organization: str | None = None,
+    ) -> dict[str, Any]:
         """Attempts to verify the given ID token, following the steps defined in the OpenID Connect spec.
 
         Args:
             token (str): The JWT to verify.
             nonce (str, optional): The nonce value sent during authentication.
             max_age (int, optional): The max_age value sent during authentication.
             organization (str, optional): The expected organization ID (org_id) claim value. This should be specified
```

### Comparing `auth0-python-4.2.0/auth0/authentication/base.py` & `auth0-python-4.3.0/auth0/asyncify.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,63 +1,101 @@
-from auth0.rest import RestClient, RestClientOptions
+import aiohttp
 
-from .client_authentication import add_client_authentication
+from auth0.authentication.base import AuthenticationBase
+from auth0.rest import RestClientOptions
+from auth0.rest_async import AsyncRestClient
+
+
+def _gen_async(client, method):
+    m = getattr(client, method)
+
+    async def closure(*args, **kwargs):
+        return await m(*args, **kwargs)
+
+    return closure
+
+
+def asyncify(cls):
+    methods = [
+        func
+        for func in dir(cls)
+        if callable(getattr(cls, func)) and not func.startswith("_")
+    ]
+
+    class AsyncManagementClient(cls):
+        def __init__(
+            self,
+            domain,
+            token,
+            telemetry=True,
+            timeout=5.0,
+            protocol="https",
+            rest_options=None,
+        ):
+            super().__init__(domain, token, telemetry, timeout, protocol, rest_options)
+            self.client = AsyncRestClient(
+                jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
+            )
+
+    class AsyncAuthenticationClient(cls):
+        def __init__(
+            self,
+            domain,
+            client_id,
+            client_secret=None,
+            client_assertion_signing_key=None,
+            client_assertion_signing_alg=None,
+            telemetry=True,
+            timeout=5.0,
+            protocol="https",
+        ):
+            super().__init__(
+                domain,
+                client_id,
+                client_secret,
+                client_assertion_signing_key,
+                client_assertion_signing_alg,
+                telemetry,
+                timeout,
+                protocol,
+            )
+            self.client = AsyncRestClient(
+                None,
+                options=RestClientOptions(
+                    telemetry=telemetry, timeout=timeout, retries=0
+                ),
+            )
+
+    class Wrapper(cls):
+        def __init__(self, *args, **kwargs):
+            super().__init__(*args, **kwargs)
+            if AuthenticationBase in cls.__bases__:
+                self._async_client = AsyncAuthenticationClient(*args, **kwargs)
+            else:
+                self._async_client = AsyncManagementClient(*args, **kwargs)
+            for method in methods:
+                setattr(
+                    self,
+                    f"{method}_async",
+                    _gen_async(self._async_client, method),
+                )
+
+        def set_session(self, session):
+            """Set Client Session to improve performance by reusing session.
+
+            Args:
+                session (aiohttp.ClientSession): The client session which should be closed
+                    manually or within context manager.
+            """
+            self._session = session
+            self._async_client.client.set_session(self._session)
+
+        async def __aenter__(self):
+            """Automatically create and set session within context manager."""
+            self.set_session(aiohttp.ClientSession())
+            return self
+
+        async def __aexit__(self, exc_type, exc_val, exc_tb):
+            """Automatically close session within context manager."""
+            await self._session.close()
 
-UNKNOWN_ERROR = "a0.sdk.internal.unknown"
-
-
-class AuthenticationBase:
-    """Base authentication object providing simple REST methods.
-
-    Args:
-        domain (str): The domain of your Auth0 tenant
-        client_id (str): Your application's client ID
-        client_secret (str, optional): Your application's client secret
-        client_assertion_signing_key (str, optional): Private key used to sign the client assertion JWT.
-        client_assertion_signing_alg (str, optional): Algorithm used to sign the client assertion JWT (defaults to 'RS256').
-        telemetry (bool, optional): Enable or disable telemetry (defaults to True)
-        timeout (float or tuple, optional): Change the requests connect and read timeout. Pass a tuple to specify both values separately or a float to set both to it. (defaults to 5.0 for both)
-        protocol (str, optional): Useful for testing. (defaults to 'https')
-    """
-
-    def __init__(
-        self,
-        domain,
-        client_id,
-        client_secret=None,
-        client_assertion_signing_key=None,
-        client_assertion_signing_alg=None,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-    ):
-        self.domain = domain
-        self.client_id = client_id
-        self.client_secret = client_secret
-        self.client_assertion_signing_key = client_assertion_signing_key
-        self.client_assertion_signing_alg = client_assertion_signing_alg
-        self.protocol = protocol
-        self.client = RestClient(
-            None,
-            options=RestClientOptions(telemetry=telemetry, timeout=timeout, retries=0),
-        )
-
-    def _add_client_authentication(self, payload):
-        return add_client_authentication(
-            payload,
-            self.domain,
-            self.client_id,
-            self.client_secret,
-            self.client_assertion_signing_key,
-            self.client_assertion_signing_alg,
-        )
-
-    def post(self, url, data=None, headers=None):
-        return self.client.post(url, data=data, headers=headers)
-
-    def authenticated_post(self, url, data=None, headers=None):
-        return self.client.post(
-            url, data=self._add_client_authentication(data), headers=headers
-        )
-
-    def get(self, url, params=None, headers=None):
-        return self.client.get(url, params, headers)
+    return Wrapper
```

### Comparing `auth0-python-4.2.0/auth0/authentication/client_authentication.py` & `auth0-python-4.3.0/auth0/authentication/client_authentication.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+from __future__ import annotations
+
 import datetime
 import uuid
+from typing import Any
 
 import jwt
 
 
 def create_client_assertion_jwt(
-    domain, client_id, client_assertion_signing_key, client_assertion_signing_alg
-):
+    domain: str,
+    client_id: str,
+    client_assertion_signing_key: str,
+    client_assertion_signing_alg: str | None,
+) -> str:
     """Creates a JWT for the client_assertion field.
 
     Args:
         domain (str): The domain of your Auth0 tenant
         client_id (str): Your application's client ID
-        client_assertion_signing_key (str, optional): Private key used to sign the client assertion JWT
+        client_assertion_signing_key (str): Private key used to sign the client assertion JWT
         client_assertion_signing_alg (str, optional): Algorithm used to sign the client assertion JWT (defaults to 'RS256')
 
     Returns:
         A JWT signed with the `client_assertion_signing_key`.
     """
     client_assertion_signing_alg = client_assertion_signing_alg or "RS256"
     now = datetime.datetime.utcnow()
@@ -31,28 +37,28 @@
         },
         client_assertion_signing_key,
         client_assertion_signing_alg,
     )
 
 
 def add_client_authentication(
-    payload,
-    domain,
-    client_id,
-    client_secret,
-    client_assertion_signing_key,
-    client_assertion_signing_alg,
-):
+    payload: dict[str, Any],
+    domain: str,
+    client_id: str,
+    client_secret: str | None,
+    client_assertion_signing_key: str | None,
+    client_assertion_signing_alg: str | None,
+) -> dict[str, Any]:
     """Adds the client_assertion or client_secret fields to authenticate a payload.
 
     Args:
         payload (dict): The POST payload that needs additional fields to be authenticated.
         domain (str): The domain of your Auth0 tenant
         client_id (str): Your application's client ID
-        client_secret (str): Your application's client secret
+        client_secret (str, optional): Your application's client secret
         client_assertion_signing_key (str, optional): Private key used to sign the client assertion JWT
         client_assertion_signing_alg (str, optional): Algorithm used to sign the client assertion JWT (defaults to 'RS256')
 
     Returns:
         A copy of the payload with client authentication fields added.
     """
```

### Comparing `auth0-python-4.2.0/auth0/authentication/database.py` & `auth0-python-4.3.0/auth0/authentication/database.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-import warnings
+from __future__ import annotations
+
+from typing import Any
 
 from .base import AuthenticationBase
 
 
 class Database(AuthenticationBase):
     """Database & Active Directory / LDAP Authentication.
 
     Args:
         domain (str): Your auth0 domain (e.g: username.auth0.com)
     """
 
     def signup(
         self,
-        email,
-        password,
-        connection,
-        username=None,
-        user_metadata=None,
-        given_name=None,
-        family_name=None,
-        name=None,
-        nickname=None,
-        picture=None,
-    ):
+        email: str,
+        password: str,
+        connection: str,
+        username: str | None = None,
+        user_metadata: dict[str, Any] | None = None,
+        given_name: str | None = None,
+        family_name: str | None = None,
+        name: str | None = None,
+        nickname: str | None = None,
+        picture: str | None = None,
+    ) -> dict[str, Any]:
         """Signup using email and password.
 
         Args:
            email (str): The user's email address.
 
            password (str): The user's desired password.
 
@@ -46,15 +48,15 @@
            nickname (str, optional): The user's nickname.
 
            picture (str, optional): A URI pointing to the user's picture.
 
 
         See: https://auth0.com/docs/api/authentication#signup
         """
-        body = {
+        body: dict[str, Any] = {
             "client_id": self.client_id,
             "email": email,
             "password": password,
             "connection": connection,
         }
         if username:
             body.update({"username": username})
@@ -67,28 +69,32 @@
         if name:
             body.update({"name": name})
         if nickname:
             body.update({"nickname": nickname})
         if picture:
             body.update({"picture": picture})
 
-        return self.post(
+        data: dict[str, Any] = self.post(
             f"{self.protocol}://{self.domain}/dbconnections/signup", data=body
         )
+        return data
 
-    def change_password(self, email, connection, password=None):
+    def change_password(
+        self, email: str, connection: str, password: str | None = None
+    ) -> str:
         """Asks to change a password for a given user.
 
         email (str): The user's email address.
 
         connection (str): The name of the database connection where this user should be created.
         """
         body = {
             "client_id": self.client_id,
             "email": email,
             "connection": connection,
         }
 
-        return self.post(
+        data: str = self.post(
             f"{self.protocol}://{self.domain}/dbconnections/change_password",
             data=body,
         )
+        return data
```

### Comparing `auth0-python-4.2.0/auth0/authentication/delegated.py` & `auth0-python-4.3.0/auth0/authentication/delegated.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,30 @@
+from __future__ import annotations
+
+from typing import Any
+
 from .base import AuthenticationBase
 
 
 class Delegated(AuthenticationBase):
     """Delegated authentication endpoints.
 
     Args:
         domain (str): Your auth0 domain (e.g: username.auth0.com)
     """
 
     def get_token(
         self,
-        target,
-        api_type,
-        grant_type,
-        id_token=None,
-        refresh_token=None,
-        scope="openid",
-    ):
+        target: str,
+        api_type: str,
+        grant_type: str,
+        id_token: str | None = None,
+        refresh_token: str | None = None,
+        scope: str = "openid",
+    ) -> Any:
         """Obtain a delegation token."""
 
         if id_token and refresh_token:
             raise ValueError("Only one of id_token or refresh_token can be None")
 
         data = {
             "client_id": self.client_id,
```

### Comparing `auth0-python-4.2.0/auth0/authentication/enterprise.py` & `auth0-python-4.3.0/auth0/authentication/enterprise.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,28 @@
+from typing import Any
+
 from .base import AuthenticationBase
 
 
 class Enterprise(AuthenticationBase):
 
     """Enterprise endpoints.
 
     Args:
         domain (str): Your auth0 domain (e.g: my-domain.us.auth0.com)
     """
 
-    def saml_metadata(self):
+    def saml_metadata(self) -> Any:
         """Get SAML2.0 Metadata."""
 
         return self.get(
             url="{}://{}/samlp/metadata/{}".format(
                 self.protocol, self.domain, self.client_id
             )
         )
 
-    def wsfed_metadata(self):
+    def wsfed_metadata(self) -> Any:
         """Returns the WS-Federation Metadata."""
 
         url = "{}://{}/wsfed/FederationMetadata/2007-06/FederationMetadata.xml"
 
         return self.get(url=url.format(self.protocol, self.domain))
```

### Comparing `auth0-python-4.2.0/auth0/authentication/get_token.py` & `auth0-python-4.3.0/auth0/authentication/get_token.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+from __future__ import annotations
+
+from typing import Any
+
 from .base import AuthenticationBase
-from .client_authentication import add_client_authentication
 
 
 class GetToken(AuthenticationBase):
 
     """/oauth/token related endpoints
 
     Args:
         domain (str): Your auth0 domain (e.g: username.auth0.com)
     """
 
     def authorization_code(
         self,
-        code,
-        redirect_uri,
-        grant_type="authorization_code",
-    ):
+        code: str,
+        redirect_uri: str | None,
+        grant_type: str = "authorization_code",
+    ) -> Any:
         """Authorization code grant
 
         This is the OAuth 2.0 grant that regular web apps utilize in order
         to access an API. Use this endpoint to exchange an Authorization Code
         for a Token.
 
         Args:
@@ -43,19 +46,19 @@
                 "grant_type": grant_type,
                 "redirect_uri": redirect_uri,
             },
         )
 
     def authorization_code_pkce(
         self,
-        code_verifier,
-        code,
-        redirect_uri,
-        grant_type="authorization_code",
-    ):
+        code_verifier: str,
+        code: str,
+        redirect_uri: str | None,
+        grant_type: str = "authorization_code",
+    ) -> Any:
         """Authorization code pkce grant
 
         This is the OAuth 2.0 grant that mobile apps utilize in order to access an API.
         Use this endpoint to exchange an Authorization Code for a Token.
 
         Args:
             code_verifier (str): Cryptographically random key that was used to generate
@@ -82,17 +85,17 @@
                 "grant_type": grant_type,
                 "redirect_uri": redirect_uri,
             },
         )
 
     def client_credentials(
         self,
-        audience,
-        grant_type="client_credentials",
-    ):
+        audience: str,
+        grant_type: str = "client_credentials",
+    ) -> Any:
         """Client credentials grant
 
         This is the OAuth 2.0 grant that server processes utilize in
         order to access an API. Use this endpoint to directly request
         an access_token by using the Application Credentials (a Client Id and
         a Client Secret).
 
@@ -112,21 +115,22 @@
                 "audience": audience,
                 "grant_type": grant_type,
             },
         )
 
     def login(
         self,
-        username,
-        password,
-        scope=None,
-        realm=None,
-        audience=None,
-        grant_type="http://auth0.com/oauth/grant-type/password-realm",
-    ):
+        username: str,
+        password: str,
+        scope: str | None = None,
+        realm: str | None = None,
+        audience: str | None = None,
+        grant_type: str = "http://auth0.com/oauth/grant-type/password-realm",
+        forwarded_for: str | None = None,
+    ) -> Any:
         """Calls /oauth/token endpoint with password-realm grant type
 
 
         This is the OAuth 2.0 grant that highly trusted apps utilize in order
         to access an API. In this flow the end-user is asked to fill in credentials
         (username/password) typically using an interactive form in the user-agent
         (browser). This information is later on sent to the client and Auth0.
@@ -145,37 +149,45 @@
             Set this if you want to add realm support at this grant.
 
             audience (str, optional): The unique identifier of the target API you want to access.
 
             grant_type (str, optional): Denotes the flow you're using. For password realm
             use http://auth0.com/oauth/grant-type/password-realm
 
+            forwarded_for (str, optional): End-user IP as a string value. Set this if you want
+            brute-force protection to work in server-side scenarios.
+            See https://auth0.com/docs/get-started/authentication-and-authorization-flow/avoid-common-issues-with-resource-owner-password-flow-and-attack-protection
+
         Returns:
             access_token, id_token
         """
+        headers = None
+        if forwarded_for:
+            headers = {"auth0-forwarded-for": forwarded_for}
 
         return self.authenticated_post(
             f"{self.protocol}://{self.domain}/oauth/token",
             data={
                 "client_id": self.client_id,
                 "username": username,
                 "password": password,
                 "realm": realm,
                 "scope": scope,
                 "audience": audience,
                 "grant_type": grant_type,
             },
+            headers=headers,
         )
 
     def refresh_token(
         self,
-        refresh_token,
-        scope="",
-        grant_type="refresh_token",
-    ):
+        refresh_token: str,
+        scope: str = "",
+        grant_type: str = "refresh_token",
+    ) -> Any:
         """Calls /oauth/token endpoint with refresh token grant type
 
         Use this endpoint to refresh an access token, using the refresh token you got during authorization.
 
         Args:
             refresh_token (str): The refresh token returned from the initial token request.
 
@@ -195,15 +207,17 @@
                 "client_id": self.client_id,
                 "refresh_token": refresh_token,
                 "scope": scope,
                 "grant_type": grant_type,
             },
         )
 
-    def passwordless_login(self, username, otp, realm, scope, audience):
+    def passwordless_login(
+        self, username: str, otp: str, realm: str, scope: str, audience: str
+    ) -> Any:
         """Calls /oauth/token endpoint with http://auth0.com/oauth/grant-type/passwordless/otp grant type
 
         Once the verification code was received, login the user using this endpoint with their
         phone number/email and verification code.
 
         Args:
             username (str): The user's phone number or email address.
```

### Comparing `auth0-python-4.2.0/auth0/authentication/passwordless.py` & `auth0-python-4.3.0/auth0/authentication/passwordless.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-import warnings
+from __future__ import annotations
+
+from typing import Any
 
 from .base import AuthenticationBase
 
 
 class Passwordless(AuthenticationBase):
 
     """Passwordless connections endpoints.
 
     Args:
         domain (str): Your auth0 domain (e.g: my-domain.us.auth0.com)
     """
 
-    def email(self, email, send="link", auth_params=None):
+    def email(
+        self, email: str, send: str = "link", auth_params: dict[str, str] | None = None
+    ) -> Any:
         """Start flow sending an email.
 
         Given the user email address, it will send an email with:
 
           - A link (default, send:"link"). You can then authenticate with
             this user opening the link and he will be automatically logged in
             to the application. Optionally, you can append/override
@@ -31,28 +35,28 @@
             email (str): Email address.
 
             send (str, optional): Can be: 'link' or 'code'. Defaults to 'link'.
 
             auth_params (dict, optional): Parameters to append or override.
         """
 
-        data = {
+        data: dict[str, Any] = {
             "client_id": self.client_id,
             "connection": "email",
             "email": email,
             "send": send,
         }
         if auth_params:
             data.update({"authParams": auth_params})
 
         return self.authenticated_post(
             f"{self.protocol}://{self.domain}/passwordless/start", data=data
         )
 
-    def sms(self, phone_number):
+    def sms(self, phone_number: str) -> Any:
         """Start flow sending an SMS message.
 
         Given the user phone number, it will send an SMS with
         a verification code. You can then authenticate with
         this user using phone number as username and code as password.
 
         Complete the authentication using the get_token.passwordless_login method.
```

### Comparing `auth0-python-4.2.0/auth0/authentication/revoke_token.py` & `auth0-python-4.3.0/auth0/authentication/revoke_token.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from typing import Any
+
 from .base import AuthenticationBase
 
 
 class RevokeToken(AuthenticationBase):
     """Revoke Refresh Token endpoint
 
     Args:
         domain (str): Your auth0 domain (e.g: my-domain.us.auth0.com)
     """
 
-    def revoke_refresh_token(self, token):
+    def revoke_refresh_token(self, token: str) -> Any:
         """Revokes a Refresh Token if it has been compromised
 
         Each revocation request invalidates not only the specific token, but all other tokens
         based on the same authorization grant. This means that all Refresh Tokens that have
         been issued for the same user, application, and audience will be revoked.
 
         Args:
```

### Comparing `auth0-python-4.2.0/auth0/authentication/social.py` & `auth0-python-4.3.0/auth0/authentication/social.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+from typing import Any
+
 from .base import AuthenticationBase
 
 
 class Social(AuthenticationBase):
 
     """Social provider's endpoints.
 
     Args:
         domain (str): Your auth0 domain (e.g: my-domain.us.auth0.com)
     """
 
-    def login(self, access_token, connection, scope="openid"):
+    def login(self, access_token: str, connection: str, scope: str = "openid") -> Any:
         """Login using a social provider's access token
 
         Given the social provider's access_token and the connection specified,
         it will do the authentication on the provider and return a dict with
         the access_token and id_token. Currently, this endpoint only works for
         Facebook, Google, Twitter and Weibo.
```

### Comparing `auth0-python-4.2.0/auth0/authentication/token_verifier.py` & `auth0-python-4.3.0/auth0/authentication/token_verifier.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 """Token Verifier module"""
+from __future__ import annotations
+
 import json
 import time
+from typing import TYPE_CHECKING, Any, ClassVar
 
 import jwt
 import requests
 
 from auth0.exceptions import TokenValidationError
 
+if TYPE_CHECKING:
+    from cryptography.hazmat.primitives.asymmetric.rsa import RSAPublicKey
+
 
 class SignatureVerifier:
     """Abstract class that will verify a given JSON web token's signature
     using the key fetched internally given its key id.
 
     Args:
         algorithm (str): The expected signing algorithm (e.g. RS256).
     """
 
-    DISABLE_JWT_CHECKS = {
+    DISABLE_JWT_CHECKS: ClassVar[dict[str, bool]] = {
         "verify_signature": True,
         "verify_exp": False,
         "verify_nbf": False,
         "verify_iat": False,
         "verify_aud": False,
         "verify_iss": False,
         "require_exp": False,
         "require_iat": False,
         "require_nbf": False,
     }
 
-    def __init__(self, algorithm):
+    def __init__(self, algorithm: str) -> None:
         if not algorithm or type(algorithm) != str:
             raise ValueError("algorithm must be specified.")
         self._algorithm = algorithm
 
-    def _fetch_key(self, key_id=None):
+    def _fetch_key(self, key_id: str) -> str | RSAPublicKey:
         """Obtains the key associated to the given key id.
         Must be implemented by subclasses.
 
         Args:
-            key_id (str, optional): The id of the key to fetch.
+            key_id (str): The id of the key to fetch.
 
         Returns:
             the key to use for verifying a cryptographic signature
         """
         raise NotImplementedError
 
-    def _get_kid(self, token):
+    def _get_kid(self, token: str) -> str | None:
         """Gets the key id from the kid claim of the header of the token
 
         Args:
             token (str): The JWT to get the header from.
 
         Raises:
             TokenValidationError: if the token cannot be decoded, the algorithm is invalid
@@ -68,15 +74,15 @@
             raise TokenValidationError(
                 'Signature algorithm of "{}" is not supported. Expected the token '
                 'to be signed with "{}"'.format(alg, self._algorithm)
             )
 
         return header.get("kid", None)
 
-    def _decode_jwt(self, token, secret_or_certificate):
+    def _decode_jwt(self, token: str, secret_or_certificate: str) -> dict[str, Any]:
         """Verifies and decodes the given JSON web token with the given public key or shared secret.
 
         Args:
             token (str): The JWT to get its signature verified.
             secret_or_certificate (str): The public key or shared secret.
 
         Raises:
@@ -90,120 +96,123 @@
                 algorithms=[self._algorithm],
                 options=self.DISABLE_JWT_CHECKS,
             )
         except jwt.exceptions.InvalidSignatureError:
             raise TokenValidationError("Invalid token signature.")
         return decoded
 
-    def verify_signature(self, token):
+    def verify_signature(self, token: str) -> dict[str, Any]:
         """Verifies the signature of the given JSON web token.
 
         Args:
             token (str): The JWT to get its signature verified.
 
         Raises:
             TokenValidationError: if the token cannot be decoded, the algorithm is invalid
             or the token's signature doesn't match the calculated one.
         """
         kid = self._get_kid(token)
+        if kid is None:
+            kid = ""
         secret_or_certificate = self._fetch_key(key_id=kid)
 
-        return self._decode_jwt(token, secret_or_certificate)
+        return self._decode_jwt(token, secret_or_certificate)  # type: ignore[arg-type]
 
 
 class SymmetricSignatureVerifier(SignatureVerifier):
     """Verifier for HMAC signatures, which rely on shared secrets.
 
     Args:
         shared_secret (str): The shared secret used to decode the token.
         algorithm (str, optional): The expected signing algorithm. Defaults to "HS256".
     """
 
-    def __init__(self, shared_secret, algorithm="HS256"):
+    def __init__(self, shared_secret: str, algorithm: str = "HS256") -> None:
         super().__init__(algorithm)
         self._shared_secret = shared_secret
 
-    def _fetch_key(self, key_id=None):
+    def _fetch_key(self, key_id: str = "") -> str:
         return self._shared_secret
 
 
 class JwksFetcher:
     """Class that fetches and holds a JSON web key set.
     This class makes use of an in-memory cache. For it to work properly, define this instance once and re-use it.
 
     Args:
         jwks_url (str): The url where the JWK set is located.
         cache_ttl (str, optional): The lifetime of the JWK set cache in seconds. Defaults to 600 seconds.
     """
 
-    CACHE_TTL = 600  # 10 min cache lifetime
+    CACHE_TTL: ClassVar[int] = 600  # 10 min cache lifetime
 
-    def __init__(self, jwks_url, cache_ttl=CACHE_TTL):
+    def __init__(self, jwks_url: str, cache_ttl: int = CACHE_TTL) -> None:
         self._jwks_url = jwks_url
         self._init_cache(cache_ttl)
-        return
 
-    def _init_cache(self, cache_ttl):
-        self._cache_value = {}
-        self._cache_date = 0
+    def _init_cache(self, cache_ttl: int) -> None:
+        self._cache_value: dict[str, RSAPublicKey] = {}
+        self._cache_date = 0.0
         self._cache_ttl = cache_ttl
         self._cache_is_fresh = False
 
-    def _cache_expired(self):
+    def _cache_expired(self) -> bool:
         """Checks if the cache is expired
 
         Returns:
             True if it should use the cache.
         """
         return self._cache_date + self._cache_ttl < time.time()
 
-    def _cache_jwks(self, jwks):
+    def _cache_jwks(self, jwks: dict[str, Any]) -> None:
         """Cache the response of the JWKS request
 
         Args:
             jwks (dict): The JWKS
         """
         self._cache_value = self._parse_jwks(jwks)
         self._cache_is_fresh = True
         self._cache_date = time.time()
 
-    def _fetch_jwks(self, force=False):
+    def _fetch_jwks(self, force: bool = False) -> dict[str, RSAPublicKey]:
         """Attempts to obtain the JWK set from the cache, as long as it's still valid.
         When not, it will perform a network request to the jwks_url to obtain a fresh result
         and update the cache value with it.
 
         Args:
             force (bool, optional): whether to ignore the cache and force a network request or not. Defaults to False.
         """
         if force or self._cache_expired():
             self._cache_value = {}
             response = requests.get(self._jwks_url)
             if response.ok:
-                jwks = response.json()
+                jwks: dict[str, Any] = response.json()
                 self._cache_jwks(jwks)
             return self._cache_value
 
         self._cache_is_fresh = False
         return self._cache_value
 
     @staticmethod
-    def _parse_jwks(jwks):
+    def _parse_jwks(jwks: dict[str, Any]) -> dict[str, RSAPublicKey]:
         """
         Converts a JWK string representation into a binary certificate in PEM format.
         """
-        keys = {}
+        keys: dict[str, RSAPublicKey] = {}
 
         for key in jwks["keys"]:
             # noinspection PyUnresolvedReferences
             # requirement already includes cryptography -> pyjwt[crypto]
-            rsa_key = jwt.algorithms.RSAAlgorithm.from_jwk(json.dumps(key))
+            rsa_key: RSAPublicKey = jwt.algorithms.RSAAlgorithm.from_jwk(
+                json.dumps(key)
+            )
             keys[key["kid"]] = rsa_key
         return keys
 
-    def get_key(self, key_id):
+    def get_key(self, key_id: str) -> RSAPublicKey:
         """Obtains the JWK associated with the given key id.
 
         Args:
             key_id (str): The id of the key to fetch.
 
         Returns:
             the JWK associated with the given key id.
@@ -228,19 +237,24 @@
 
     Args:
         jwks_url (str): The url where the JWK set is located.
         algorithm (str, optional): The expected signing algorithm. Defaults to "RS256".
         cache_ttl (int, optional): The lifetime of the JWK set cache in seconds. Defaults to 600 seconds.
     """
 
-    def __init__(self, jwks_url, algorithm="RS256", cache_ttl=JwksFetcher.CACHE_TTL):
+    def __init__(
+        self,
+        jwks_url: str,
+        algorithm: str = "RS256",
+        cache_ttl: int = JwksFetcher.CACHE_TTL,
+    ) -> None:
         super().__init__(algorithm)
         self._fetcher = JwksFetcher(jwks_url, cache_ttl)
 
-    def _fetch_key(self, key_id=None):
+    def _fetch_key(self, key_id: str) -> RSAPublicKey:
         return self._fetcher.get_key(key_id)
 
 
 class TokenVerifier:
     """Class that verifies ID tokens following the steps defined in the OpenID Connect spec.
     An OpenID Connect ID token is not meant to be consumed until it's verified.
 
@@ -248,29 +262,41 @@
         signature_verifier (SignatureVerifier): The instance that knows how to verify the signature.
         issuer (str): The expected issuer claim value.
         audience (str): The expected audience claim value.
         leeway (int, optional): The clock skew to accept when verifying date related claims in seconds.
         Defaults to 60 seconds.
     """
 
-    def __init__(self, signature_verifier, issuer, audience, leeway=0):
+    def __init__(
+        self,
+        signature_verifier: SignatureVerifier,
+        issuer: str,
+        audience: str,
+        leeway: int = 0,
+    ) -> None:
         if not signature_verifier or not isinstance(
             signature_verifier, SignatureVerifier
         ):
             raise TypeError(
                 "signature_verifier must be an instance of SignatureVerifier."
             )
 
         self.iss = issuer
         self.aud = audience
         self.leeway = leeway
         self._sv = signature_verifier
         self._clock = None  # visible for testing
 
-    def verify(self, token, nonce=None, max_age=None, organization=None):
+    def verify(
+        self,
+        token: str,
+        nonce: str | None = None,
+        max_age: int | None = None,
+        organization: str | None = None,
+    ) -> dict[str, Any]:
         """Attempts to verify the given ID token, following the steps defined in the OpenID Connect spec.
 
         Args:
             token (str): The JWT to verify.
             nonce (str, optional): The nonce value sent during authentication.
             max_age (int, optional): The max_age value sent during authentication.
             organization (str, optional): The expected organization ID (org_id) claim value. This should be specified
@@ -292,15 +318,21 @@
         payload = self._sv.verify_signature(token)
 
         # Verify claims
         self._verify_payload(payload, nonce, max_age, organization)
 
         return payload
 
-    def _verify_payload(self, payload, nonce=None, max_age=None, organization=None):
+    def _verify_payload(
+        self,
+        payload: dict[str, Any],
+        nonce: str | None = None,
+        max_age: int | None = None,
+        organization: str | None = None,
+    ) -> None:
         # Issuer
         if "iss" not in payload or not isinstance(payload["iss"], str):
             raise TokenValidationError(
                 "Issuer (iss) claim must be a string present in the ID token"
             )
         if payload["iss"] != self.iss:
             raise TokenValidationError(
```

### Comparing `auth0-python-4.2.0/auth0/authentication/users.py` & `auth0-python-4.3.0/auth0/authentication/users.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,54 @@
+from __future__ import annotations
+
+from typing import Any
+
 from auth0.rest import RestClient, RestClientOptions
+from auth0.types import TimeoutType
 
 
 class Users:
     """Users client.
 
     Args:
         domain (str): The domain of your Auth0 tenant
         telemetry (bool, optional): Enable or disable telemetry (defaults to True)
         timeout (float or tuple, optional): Change the requests connect and read timeout. Pass a tuple to specify both values separately or a float to set both to it. (defaults to 5.0 for both)
         protocol (str, optional): Useful for testing. (defaults to 'https')
     """
 
     def __init__(
         self,
-        domain,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-    ):
+        domain: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             None,
             options=RestClientOptions(telemetry=telemetry, timeout=timeout, retries=0),
         )
 
     """Userinfo related endpoints.
 
     Args:
         domain (str): Your auth0 domain (e.g: username.auth0.com)
     """
 
-    def userinfo(self, access_token):
+    def userinfo(self, access_token: str) -> dict[str, Any]:
         """Returns the user information based on the Auth0 access token.
         This endpoint will work only if openid was granted as a scope for the access_token.
 
         Args:
             access_token (str): Auth0 access token (obtained during login).
 
         Returns:
             The user profile.
         """
 
-        return self.client.get(
+        data: dict[str, Any] = self.client.get(
             url=f"{self.protocol}://{self.domain}/userinfo",
             headers={"Authorization": f"Bearer {access_token}"},
         )
+        return data
```

### Comparing `auth0-python-4.2.0/auth0/exceptions.py` & `auth0-python-4.3.0/auth0/exceptions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,30 @@
+from __future__ import annotations
+
+from typing import Any
+
+
 class Auth0Error(Exception):
-    def __init__(self, status_code, error_code, message, content=None):
+    def __init__(
+        self,
+        status_code: int,
+        error_code: str,
+        message: str,
+        content: Any | None = None,
+    ) -> None:
         self.status_code = status_code
         self.error_code = error_code
         self.message = message
         self.content = content
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"{self.status_code}: {self.message}"
 
 
 class RateLimitError(Auth0Error):
-    def __init__(self, error_code, message, reset_at):
+    def __init__(self, error_code: str, message: str, reset_at: int) -> None:
         super().__init__(status_code=429, error_code=error_code, message=message)
         self.reset_at = reset_at
 
 
 class TokenValidationError(Exception):
     pass
```

### Comparing `auth0-python-4.2.0/auth0/management/__init__.py` & `auth0-python-4.3.0/auth0/management/__init__.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/actions.py` & `auth0-python-4.3.0/auth0/management/actions.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/async_auth0.py` & `auth0-python-4.3.0/auth0/management/async_auth0.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/attack_protection.py` & `auth0-python-4.3.0/auth0/management/attack_protection.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/auth0.py` & `auth0-python-4.3.0/auth0/management/auth0.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/blacklists.py` & `auth0-python-4.3.0/auth0/management/blacklists.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/branding.py` & `auth0-python-4.3.0/auth0/management/branding.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             body (str): Complete HTML content to assign to the template. See linked API documentation for example.
 
         See: https://auth0.com/docs/api/management/v2#!/Branding/put_universal_login
         """
 
         return self.client.put(
             self._url("templates", "universal-login"),
-            body={"template": body},
+            data={"template": body},
         )
 
     def get_default_branding_theme(self):
         """Retrieve default branding theme.
 
         See: https://auth0.com/docs/api/management/v2#!/Branding/get_default_branding_theme
         """
```

### Comparing `auth0-python-4.2.0/auth0/management/client_credentials.py` & `auth0-python-4.3.0/auth0/management/client_credentials.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/client_grants.py` & `auth0-python-4.3.0/auth0/management/client_grants.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/clients.py` & `auth0-python-4.3.0/auth0/management/clients.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/connections.py` & `auth0-python-4.3.0/auth0/management/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         self,
         strategy=None,
         fields=None,
         include_fields=True,
         page=None,
         per_page=None,
         extra_params=None,
+        name=None,
     ):
         """Retrieves all connections.
 
         Args:
            strategy (str, optional): Only retrieve connections of
               this strategy type. (e.g: strategy='amazon')
 
@@ -72,26 +73,29 @@
            per_page (int, optional): The amount of entries per page. When not set,
               the default value is up to the server.
 
            extra_params (dictionary, optional): The extra parameters to add to
              the request. The fields, include_fields, page and per_page values
              specified as parameters take precedence over the ones defined here.
 
+           name (str): Provide the name of the connection to retrieve.
+
         See: https://auth0.com/docs/api/management/v2#!/Connections/get_connections
 
         Returns:
            A list of connection objects.
         """
 
         params = extra_params or {}
         params["strategy"] = strategy or None
         params["fields"] = fields and ",".join(fields) or None
         params["include_fields"] = str(include_fields).lower()
         params["page"] = page
         params["per_page"] = per_page
+        params["name"] = name
 
         return self.client.get(self._url(), params=params)
 
     def get(self, id, fields=None, include_fields=True):
         """Retrieve connection by id.
 
         Args:
```

### Comparing `auth0-python-4.2.0/auth0/management/custom_domains.py` & `auth0-python-4.3.0/auth0/management/custom_domains.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/device_credentials.py` & `auth0-python-4.3.0/auth0/management/device_credentials.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/email_templates.py` & `auth0-python-4.3.0/auth0/management/email_templates.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/emails.py` & `auth0-python-4.3.0/auth0/management/emails.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/grants.py` & `auth0-python-4.3.0/auth0/management/grants.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/guardian.py` & `auth0-python-4.3.0/auth0/management/guardian.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/hooks.py` & `auth0-python-4.3.0/auth0/management/hooks.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/jobs.py` & `auth0-python-4.3.0/auth0/management/jobs.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/log_streams.py` & `auth0-python-4.3.0/auth0/management/log_streams.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/logs.py` & `auth0-python-4.3.0/auth0/management/logs.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/organizations.py` & `auth0-python-4.3.0/auth0/management/organizations.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/prompts.py` & `auth0-python-4.3.0/auth0/management/prompts.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/resource_servers.py` & `auth0-python-4.3.0/auth0/management/resource_servers.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/roles.py` & `auth0-python-4.3.0/auth0/management/roles.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/rules.py` & `auth0-python-4.3.0/auth0/management/rules.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/rules_configs.py` & `auth0-python-4.3.0/auth0/management/rules_configs.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/stats.py` & `auth0-python-4.3.0/auth0/management/stats.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/tenants.py` & `auth0-python-4.3.0/auth0/management/tenants.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/tickets.py` & `auth0-python-4.3.0/auth0/management/users_by_email.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ..rest import RestClient
 
 
-class Tickets:
-    """Auth0 tickets endpoints
+class UsersByEmail:
+    """Auth0 users by email endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
 
         token (str): Management API v2 Token
 
         telemetry (bool, optional): Enable or disable Telemetry
@@ -34,29 +34,32 @@
     ):
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, action):
-        return f"{self.protocol}://{self.domain}/api/v2/tickets/{action}"
+    def _url(self):
+        return f"{self.protocol}://{self.domain}/api/v2/users-by-email"
 
-    def create_email_verification(self, body):
-        """Create an email verification ticket.
+    def search_users_by_email(self, email, fields=None, include_fields=True):
+        """List or search users.
 
         Args:
-            body (dict): attributes to set on the email verification request.
 
-        See: https://auth0.com/docs/api/v2#!/Tickets/post_email_verification
-        """
-        return self.client.post(self._url("email-verification"), data=body)
+            email: Email to search.
 
-    def create_pswd_change(self, body):
-        """Create password change ticket.
+            fields (list of str, optional): A list of fields to include or
+                exclude from the result (depending on include_fields). Leave empty to
+                retrieve all fields.
 
-        Args:
-            body (dict): attributes to set on the password change request.
+            include_fields (bool, optional): True if the fields specified are
+                to be include in the result, False otherwise.
 
-        See: https://auth0.com/docs/api/v2#!/Tickets/post_password_change
+        See: https://auth0.com/docs/api/management/v2#!/Users_By_Email/get_users_by_email
         """
-        return self.client.post(self._url("password-change"), data=body)
+        params = {
+            "email": email,
+            "fields": fields and ",".join(fields) or None,
+            "include_fields": str(include_fields).lower(),
+        }
+        return self.client.get(self._url(), params=params)
```

### Comparing `auth0-python-4.2.0/auth0/management/user_blocks.py` & `auth0-python-4.3.0/auth0/management/user_blocks.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/management/users.py` & `auth0-python-4.3.0/auth0/management/users.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/rest.py` & `auth0-python-4.3.0/auth0/rest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,24 @@
+from __future__ import annotations
+
 import base64
 import json
 import platform
 import sys
 from random import randint
 from time import sleep
+from typing import TYPE_CHECKING, Any, Mapping
 
 import requests
 
 from auth0.exceptions import Auth0Error, RateLimitError
+from auth0.types import RequestData, TimeoutType
+
+if TYPE_CHECKING:
+    from auth0.rest_async import RequestsResponse
 
 UNKNOWN_ERROR = "a0.sdk.internal.unknown"
 
 
 class RestClientOptions:
     """Configuration object for RestClient. Used for configuring
             additional RestClient options, such as rate-limit
@@ -28,47 +35,50 @@
             429 response header (indicating rate-limit has been
             hit), the RestClient will retry the request this many
             times using an exponential backoff strategy, before
             raising a RateLimitError exception. 10 retries max.
             (defaults to 3)
     """
 
-    def __init__(self, telemetry=None, timeout=None, retries=None):
-        self.telemetry = True
-        self.timeout = 5.0
-        self.retries = 3
-
-        if telemetry is not None:
-            self.telemetry = telemetry
-
-        if timeout is not None:
-            self.timeout = timeout
-
-        if retries is not None:
-            self.retries = retries
+    def __init__(
+        self,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        retries: int = 3,
+    ) -> None:
+        self.telemetry = telemetry
+        self.timeout = timeout
+        self.retries = retries
 
 
 class RestClient:
     """Provides simple methods for handling all RESTful api endpoints.
 
     Args:
+        jwt (str, optional): The JWT to be used with the RestClient.
         telemetry (bool, optional): Enable or disable Telemetry
             (defaults to True)
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
         options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries. Overrides matching
             options passed to the constructor.
             (defaults to 3)
     """
 
-    def __init__(self, jwt, telemetry=True, timeout=5.0, options=None):
+    def __init__(
+        self,
+        jwt: str | None,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        options: RestClientOptions | None = None,
+    ) -> None:
         if options is None:
             options = RestClientOptions(telemetry=telemetry, timeout=timeout)
 
         self.options = options
         self.jwt = jwt
 
         self._metrics = {"retries": 0, "backoff": []}
@@ -107,30 +117,35 @@
 
         # For backwards compatibility reasons only
         # TODO: Deprecate in the next major so we can prune these arguments. Guidance should be to use RestClient.options.*
         self.telemetry = options.telemetry
         self.timeout = options.timeout
 
     # Returns a hard cap for the maximum number of retries allowed (10)
-    def MAX_REQUEST_RETRIES(self):
+    def MAX_REQUEST_RETRIES(self) -> int:
         return 10
 
     # Returns the maximum amount of jitter to introduce in milliseconds (100ms)
-    def MAX_REQUEST_RETRY_JITTER(self):
+    def MAX_REQUEST_RETRY_JITTER(self) -> int:
         return 100
 
     # Returns the maximum delay window allowed (1000ms)
-    def MAX_REQUEST_RETRY_DELAY(self):
+    def MAX_REQUEST_RETRY_DELAY(self) -> int:
         return 1000
 
     # Returns the minimum delay window allowed (100ms)
-    def MIN_REQUEST_RETRY_DELAY(self):
+    def MIN_REQUEST_RETRY_DELAY(self) -> int:
         return 100
 
-    def get(self, url, params=None, headers=None):
+    def get(
+        self,
+        url: str,
+        params: dict[str, Any] | None = None,
+        headers: dict[str, str] | None = None,
+    ) -> Any:
         request_headers = self.base_headers.copy()
         request_headers.update(headers or {})
 
         # Track the API request attempt number
         attempt = 0
 
         # Reset the metrics tracker
@@ -158,61 +173,76 @@
             if self._skip_sleep is False:
                 # sleep() functions in seconds, so convert the milliseconds formula above accordingly
                 sleep(wait / 1000)
 
         # Return the final Response
         return self._process_response(response)
 
-    def post(self, url, data=None, headers=None):
+    def post(
+        self,
+        url: str,
+        data: RequestData | None = None,
+        headers: dict[str, str] | None = None,
+    ) -> Any:
         request_headers = self.base_headers.copy()
         request_headers.update(headers or {})
 
         response = requests.post(
             url, json=data, headers=request_headers, timeout=self.options.timeout
         )
         return self._process_response(response)
 
-    def file_post(self, url, data=None, files=None):
+    def file_post(
+        self,
+        url: str,
+        data: RequestData | None = None,
+        files: dict[str, Any] | None = None,
+    ) -> Any:
         headers = self.base_headers.copy()
         headers.pop("Content-Type", None)
 
         response = requests.post(
             url, data=data, files=files, headers=headers, timeout=self.options.timeout
         )
         return self._process_response(response)
 
-    def patch(self, url, data=None):
+    def patch(self, url: str, data: RequestData | None = None) -> Any:
         headers = self.base_headers.copy()
 
         response = requests.patch(
             url, json=data, headers=headers, timeout=self.options.timeout
         )
         return self._process_response(response)
 
-    def put(self, url, data=None):
+    def put(self, url: str, data: RequestData | None = None) -> Any:
         headers = self.base_headers.copy()
 
         response = requests.put(
             url, json=data, headers=headers, timeout=self.options.timeout
         )
         return self._process_response(response)
 
-    def delete(self, url, params=None, data=None):
+    def delete(
+        self,
+        url: str,
+        params: dict[str, Any] | None = None,
+        data: RequestData | None = None,
+    ) -> Any:
         headers = self.base_headers.copy()
 
         response = requests.delete(
             url,
             headers=headers,
             params=params or {},
             json=data,
             timeout=self.options.timeout,
         )
         return self._process_response(response)
 
-    def _calculate_wait(self, attempt):
+    def _calculate_wait(self, attempt: int) -> int:
         # Retry the request. Apply a exponential backoff for subsequent attempts, using this formula:
         # max(MIN_REQUEST_RETRY_DELAY, min(MAX_REQUEST_RETRY_DELAY, (100ms * (2 ** attempt - 1)) + random_between(1, MAX_REQUEST_RETRY_JITTER)))
 
         # Increases base delay by (100ms * (2 ** attempt - 1))
         wait = 100 * 2 ** (attempt - 1)
 
         # Introduces jitter to the base delay; increases delay between 1ms to MAX_REQUEST_RETRY_JITTER (100ms)
@@ -221,37 +251,39 @@
         # Is never more than MAX_REQUEST_RETRY_DELAY (1s)
         wait = min(self.MAX_REQUEST_RETRY_DELAY(), wait)
 
         # Is never less than MIN_REQUEST_RETRY_DELAY (100ms)
         wait = max(self.MIN_REQUEST_RETRY_DELAY(), wait)
 
         self._metrics["retries"] = attempt
-        self._metrics["backoff"].append(wait)
+        self._metrics["backoff"].append(wait)  # type: ignore[attr-defined]
 
         return wait
 
-    def _process_response(self, response):
+    def _process_response(self, response: requests.Response) -> Any:
         return self._parse(response).content()
 
-    def _parse(self, response):
+    def _parse(self, response: requests.Response) -> Response:
         if not response.text:
             return EmptyResponse(response.status_code)
         try:
             return JsonResponse(response)
         except ValueError:
             return PlainResponse(response)
 
 
 class Response:
-    def __init__(self, status_code, content, headers):
+    def __init__(
+        self, status_code: int, content: Any, headers: Mapping[str, str]
+    ) -> None:
         self._status_code = status_code
         self._content = content
         self._headers = headers
 
-    def content(self):
+    def content(self) -> Any:
         if self._is_error():
             if self._status_code == 429:
                 reset_at = int(self._headers.get("x-ratelimit-reset", "-1"))
                 raise RateLimitError(
                     error_code=self._error_code(),
                     message=self._error_message(),
                     reset_at=reset_at,
@@ -268,62 +300,62 @@
                 status_code=self._status_code,
                 error_code=self._error_code(),
                 message=self._error_message(),
             )
         else:
             return self._content
 
-    def _is_error(self):
+    def _is_error(self) -> bool:
         return self._status_code is None or self._status_code >= 400
 
     # Adding these methods to force implementation in subclasses because they are references in this parent class
     def _error_code(self):
         raise NotImplementedError
 
     def _error_message(self):
         raise NotImplementedError
 
 
 class JsonResponse(Response):
-    def __init__(self, response):
+    def __init__(self, response: requests.Response | RequestsResponse) -> None:
         content = json.loads(response.text)
         super().__init__(response.status_code, content, response.headers)
 
-    def _error_code(self):
+    def _error_code(self) -> str:
         if "errorCode" in self._content:
             return self._content.get("errorCode")
         elif "error" in self._content:
             return self._content.get("error")
         elif "code" in self._content:
             return self._content.get("code")
         else:
             return UNKNOWN_ERROR
 
-    def _error_message(self):
+    def _error_message(self) -> str:
         if "error_description" in self._content:
             return self._content.get("error_description")
         message = self._content.get("message", "")
         if message is not None and message != "":
             return message
         return self._content.get("error", "")
 
 
 class PlainResponse(Response):
-    def __init__(self, response):
+    def __init__(self, response: requests.Response | RequestsResponse) -> None:
         super().__init__(response.status_code, response.text, response.headers)
 
-    def _error_code(self):
+    def _error_code(self) -> str:
         return UNKNOWN_ERROR
 
-    def _error_message(self):
+    def _error_message(self) -> str:
         return self._content
 
 
 class EmptyResponse(Response):
-    def __init__(self, status_code):
+    def __init__(self, status_code: int) -> None:
         super().__init__(status_code, "", {})
 
-    def _error_code(self):
+    def _error_code(self) -> str:
         return UNKNOWN_ERROR
 
-    def _error_message(self):
+    def _error_message(self) -> str:
         return ""
```

### Comparing `auth0-python-4.2.0/auth0/rest_async.py` & `auth0-python-4.3.0/auth0/rest_async.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+from __future__ import annotations
+
 import asyncio
+from typing import Any
 
 import aiohttp
 
 from auth0.exceptions import RateLimitError
+from auth0.types import RequestData
 
-from .rest import EmptyResponse, JsonResponse, PlainResponse, RestClient
+from .rest import EmptyResponse, JsonResponse, PlainResponse, Response, RestClient
 
 
-def _clean_params(params):
+def _clean_params(params: dict[Any, Any] | None) -> dict[Any, Any] | None:
     if params is None:
         return params
     return {k: v for k, v in params.items() if v is not None}
 
 
 class AsyncRestClient(RestClient):
     """Provides simple methods for handling all RESTful api endpoints.
@@ -26,46 +30,51 @@
         options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries. Overrides matching
             options passed to the constructor.
             (defaults to 3)
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
-        self._session = None
+        self._session: aiohttp.ClientSession | None = None
         sock_connect, sock_read = (
             self.timeout
             if isinstance(self.timeout, tuple)
             else (self.timeout, self.timeout)
         )
         self.timeout = aiohttp.ClientTimeout(
             sock_connect=sock_connect, sock_read=sock_read
         )
 
-    def set_session(self, session):
+    def set_session(self, session: aiohttp.ClientSession) -> None:
         """Set Client Session to improve performance by reusing session.
         Session should be closed manually or within context manager.
         """
         self._session = session
 
-    async def _request(self, *args, **kwargs):
+    async def _request(self, *args: Any, **kwargs: Any) -> Any:
         kwargs["headers"] = kwargs.get("headers", self.base_headers)
         kwargs["timeout"] = self.timeout
         if self._session is not None:
             # Request with re-usable session
             async with self._session.request(*args, **kwargs) as response:
                 return await self._process_response(response)
         else:
             # Request without re-usable session
             async with aiohttp.ClientSession() as session:
                 async with session.request(*args, **kwargs) as response:
                     return await self._process_response(response)
 
-    async def get(self, url, params=None, headers=None):
+    async def get(
+        self,
+        url: str,
+        params: dict[str, Any] | None = None,
+        headers: dict[str, str] | None = None,
+    ) -> Any:
         request_headers = self.base_headers.copy()
         request_headers.update(headers or {})
         # Track the API request attempt number
         attempt = 0
 
         # Reset the metrics tracker
         self._metrics = {"retries": 0, "backoff": []}
@@ -88,48 +97,63 @@
             wait = self._calculate_wait(attempt)
 
             # Skip calling sleep() when running unit tests
             if self._skip_sleep is False:
                 # sleep() functions in seconds, so convert the milliseconds formula above accordingly
                 await asyncio.sleep(wait / 1000)
 
-    async def post(self, url, data=None, headers=None):
+    async def post(
+        self,
+        url: str,
+        data: RequestData | None = None,
+        headers: dict[str, str] | None = None,
+    ) -> Any:
         request_headers = self.base_headers.copy()
         request_headers.update(headers or {})
         return await self._request("post", url, json=data, headers=request_headers)
 
-    async def file_post(self, url, data=None, files=None):
+    async def file_post(
+        self,
+        url: str,
+        data: dict[str, Any],
+        files: dict[str, Any],
+    ) -> Any:
         headers = self.base_headers.copy()
         headers.pop("Content-Type", None)
         return await self._request("post", url, data={**data, **files}, headers=headers)
 
-    async def patch(self, url, data=None):
+    async def patch(self, url: str, data: RequestData | None = None) -> Any:
         return await self._request("patch", url, json=data)
 
-    async def put(self, url, data=None):
+    async def put(self, url: str, data: RequestData | None = None) -> Any:
         return await self._request("put", url, json=data)
 
-    async def delete(self, url, params=None, data=None):
+    async def delete(
+        self,
+        url: str,
+        params: dict[str, Any] | None = None,
+        data: RequestData | None = None,
+    ) -> Any:
         return await self._request(
             "delete", url, json=data, params=_clean_params(params) or {}
         )
 
-    async def _process_response(self, response):
+    async def _process_response(self, response: aiohttp.ClientResponse) -> Any:
         parsed_response = await self._parse(response)
         return parsed_response.content()
 
-    async def _parse(self, response):
+    async def _parse(self, response: aiohttp.ClientResponse) -> Response:
         text = await response.text()
         requests_response = RequestsResponse(response, text)
         if not text:
             return EmptyResponse(response.status)
         try:
             return JsonResponse(requests_response)
         except ValueError:
             return PlainResponse(requests_response)
 
 
 class RequestsResponse:
-    def __init__(self, response, text):
+    def __init__(self, response: aiohttp.ClientResponse, text: str) -> None:
         self.status_code = response.status
         self.headers = response.headers
         self.text = text
```

### Comparing `auth0-python-4.2.0/auth0/test/authentication/test_base.py` & `auth0-python-4.3.0/auth0/test/authentication/test_base.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/authentication/test_database.py` & `auth0-python-4.3.0/auth0/test/authentication/test_database.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/authentication/test_delegated.py` & `auth0-python-4.3.0/auth0/test/authentication/test_delegated.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/authentication/test_enterprise.py` & `auth0-python-4.3.0/auth0/test/authentication/test_enterprise.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/authentication/test_get_token.py` & `auth0-python-4.3.0/auth0/test/authentication/test_get_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,30 @@
                 "scope": None,
                 "audience": None,
                 "grant_type": "http://auth0.com/oauth/grant-type/password-realm",
             },
         )
 
     @mock.patch("auth0.rest.RestClient.post")
+    def test_login_with_forwarded_for(self, mock_post):
+        g = GetToken("my.domain.com", "cid", client_secret="clsec")
+
+        g.login(username="usrnm", password="pswd", forwarded_for="192.168.0.1")
+
+        args, kwargs = mock_post.call_args
+
+        self.assertEqual(args[0], "https://my.domain.com/oauth/token")
+        self.assertEqual(
+            kwargs["headers"],
+            {
+                "auth0-forwarded-for": "192.168.0.1",
+            },
+        )
+
+    @mock.patch("auth0.rest.RestClient.post")
     def test_refresh_token(self, mock_post):
         g = GetToken("my.domain.com", "cid", client_secret="clsec")
 
         g.refresh_token(
             refresh_token="rt",
             grant_type="gt",
             scope="s",
```

### Comparing `auth0-python-4.2.0/auth0/test/authentication/test_passwordless.py` & `auth0-python-4.3.0/auth0/test/authentication/test_passwordless.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/authentication/test_revoke_token.py` & `auth0-python-4.3.0/auth0/test/authentication/test_revoke_token.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/authentication/test_social.py` & `auth0-python-4.3.0/auth0/test/authentication/test_social.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/authentication/test_token_verifier.py` & `auth0-python-4.3.0/auth0/test/authentication/test_token_verifier.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_actions.py` & `auth0-python-4.3.0/auth0/test/management/test_actions.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_atack_protection.py` & `auth0-python-4.3.0/auth0/test/management/test_atack_protection.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_auth0.py` & `auth0-python-4.3.0/auth0/test/management/test_auth0.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_blacklists.py` & `auth0-python-4.3.0/auth0/test/management/test_blacklists.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_branding.py` & `auth0-python-4.3.0/auth0/test/management/test_branding.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,25 +55,27 @@
         branding = Branding(domain="domain", token="jwttoken")
         branding.delete_template_universal_login()
 
         api.delete.assert_called_with(
             "https://domain/api/v2/branding/templates/universal-login",
         )
 
-    @mock.patch("auth0.management.branding.RestClient")
+    @mock.patch("auth0.rest.requests.put")
     def test_update_template_universal_login(self, mock_rc):
-        api = mock_rc.return_value
-        api.put.return_value = {}
+        mock_rc.return_value.status_code = 200
+        mock_rc.return_value.text = "{}"
 
         branding = Branding(domain="domain", token="jwttoken")
         branding.update_template_universal_login({"a": "b", "c": "d"})
 
-        api.put.assert_called_with(
+        mock_rc.assert_called_with(
             "https://domain/api/v2/branding/templates/universal-login",
-            body={"template": {"a": "b", "c": "d"}},
+            json={"template": {"a": "b", "c": "d"}},
+            headers=mock.ANY,
+            timeout=5.0,
         )
 
     @mock.patch("auth0.management.branding.RestClient")
     def test_get_default_branding_theme(self, mock_rc):
         api = mock_rc.return_value
         api.get.return_value = {}
```

### Comparing `auth0-python-4.2.0/auth0/test/management/test_client_credentials.py` & `auth0-python-4.3.0/auth0/test/management/test_client_credentials.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_client_grants.py` & `auth0-python-4.3.0/auth0/test/management/test_client_grants.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_clients.py` & `auth0-python-4.3.0/auth0/test/management/test_clients.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_connections.py` & `auth0-python-4.3.0/auth0/test/management/test_connections.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
             kwargs["params"],
             {
                 "fields": None,
                 "strategy": None,
                 "page": None,
                 "per_page": None,
                 "include_fields": "true",
+                "name": None,
             },
         )
 
         # Fields filter
         c.all(fields=["a", "b"], include_fields=False)
 
         args, kwargs = mock_instance.get.call_args
@@ -46,14 +47,15 @@
             kwargs["params"],
             {
                 "fields": "a,b",
                 "strategy": None,
                 "page": None,
                 "per_page": None,
                 "include_fields": "false",
+                "name": None,
             },
         )
 
         # Fields + strategy filter
         c.all(fields=["a", "b"], strategy="auth0", include_fields=True)
 
         args, kwargs = mock_instance.get.call_args
@@ -63,14 +65,15 @@
             kwargs["params"],
             {
                 "fields": "a,b",
                 "strategy": "auth0",
                 "page": None,
                 "per_page": None,
                 "include_fields": "true",
+                "name": None,
             },
         )
 
         # Specific pagination
         c.all(page=7, per_page=25)
 
         args, kwargs = mock_instance.get.call_args
@@ -80,14 +83,15 @@
             kwargs["params"],
             {
                 "fields": None,
                 "strategy": None,
                 "page": 7,
                 "per_page": 25,
                 "include_fields": "true",
+                "name": None,
             },
         )
 
         # Extra parameters
         c.all(extra_params={"some_key": "some_value"})
 
         args, kwargs = mock_instance.get.call_args
@@ -98,14 +102,33 @@
             {
                 "fields": None,
                 "strategy": None,
                 "page": None,
                 "per_page": None,
                 "include_fields": "true",
                 "some_key": "some_value",
+                "name": None,
+            },
+        )
+
+        # Name
+        c.all(name="foo")
+
+        args, kwargs = mock_instance.get.call_args
+
+        self.assertEqual("https://domain/api/v2/connections", args[0])
+        self.assertEqual(
+            kwargs["params"],
+            {
+                "fields": None,
+                "strategy": None,
+                "page": None,
+                "per_page": None,
+                "include_fields": "true",
+                "name": "foo",
             },
         )
 
     @mock.patch("auth0.management.connections.RestClient")
     def test_get(self, mock_rc):
         mock_instance = mock_rc.return_value
         mock_instance.get.return_value = {}
```

### Comparing `auth0-python-4.2.0/auth0/test/management/test_custom_domains.py` & `auth0-python-4.3.0/auth0/test/management/test_custom_domains.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_device_credentials.py` & `auth0-python-4.3.0/auth0/test/management/test_device_credentials.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_email_endpoints.py` & `auth0-python-4.3.0/auth0/test/management/test_email_endpoints.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_emails.py` & `auth0-python-4.3.0/auth0/test/management/test_emails.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_grants.py` & `auth0-python-4.3.0/auth0/test/management/test_grants.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_guardian.py` & `auth0-python-4.3.0/auth0/test/management/test_guardian.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_hooks.py` & `auth0-python-4.3.0/auth0/test/management/test_hooks.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_jobs.py` & `auth0-python-4.3.0/auth0/test/management/test_jobs.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_log_streams.py` & `auth0-python-4.3.0/auth0/test/management/test_log_streams.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_logs.py` & `auth0-python-4.3.0/auth0/test/management/test_logs.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_organizations.py` & `auth0-python-4.3.0/auth0/test/management/test_organizations.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_prompts.py` & `auth0-python-4.3.0/auth0/test/management/test_prompts.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_resource_servers.py` & `auth0-python-4.3.0/auth0/test/management/test_resource_servers.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_rest.py` & `auth0-python-4.3.0/auth0/test/management/test_rest.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_roles.py` & `auth0-python-4.3.0/auth0/test/management/test_roles.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_rules.py` & `auth0-python-4.3.0/auth0/test/management/test_rules.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_rules_configs.py` & `auth0-python-4.3.0/auth0/test/management/test_rules_configs.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_stats.py` & `auth0-python-4.3.0/auth0/test/management/test_stats.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_tenants.py` & `auth0-python-4.3.0/auth0/test/management/test_tenants.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_tickets.py` & `auth0-python-4.3.0/auth0/test/management/test_tickets.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_user_blocks.py` & `auth0-python-4.3.0/auth0/test/management/test_user_blocks.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_users.py` & `auth0-python-4.3.0/auth0/test/management/test_users.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test/management/test_users_by_email.py` & `auth0-python-4.3.0/auth0/test/management/test_users_by_email.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test_async/test_async_auth0.py` & `auth0-python-4.3.0/auth0/test_async/test_async_auth0.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test_async/test_async_token_verifier.py` & `auth0-python-4.3.0/auth0/test_async/test_async_token_verifier.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.2.0/auth0/test_async/test_asyncify.py` & `auth0-python-4.3.0/auth0/test_async/test_asyncify.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 from unittest.mock import ANY, MagicMock
 
 import aiohttp
 from aioresponses import CallbackResult, aioresponses
 from callee import Attrs
 
 from auth0.asyncify import asyncify
+from auth0.authentication import GetToken
 from auth0.management import Clients, Guardian, Jobs
 
 clients = re.compile(r"^https://example\.com/api/v2/clients.*")
+token = re.compile(r"^https://example\.com/oauth/token.*")
 factors = re.compile(r"^https://example\.com/api/v2/guardian/factors.*")
 users_imports = re.compile(r"^https://example\.com/api/v2/jobs/users-imports.*")
 payload = {"foo": "bar"}
 
 telemetry = base64.b64encode(
     json.dumps(
         {
@@ -81,14 +83,39 @@
             allow_redirects=True,
             json=data,
             headers=headers,
             timeout=ANY,
         )
 
     @aioresponses()
+    async def test_post_auth(self, mocked):
+        callback, mock = get_callback()
+        mocked.post(token, callback=callback)
+        c = asyncify(GetToken)("example.com", "cid", client_secret="clsec")
+        self.assertEqual(
+            await c.login_async(username="usrnm", password="pswd"), payload
+        )
+        mock.assert_called_with(
+            Attrs(path="/oauth/token"),
+            allow_redirects=True,
+            json={
+                "client_id": "cid",
+                "username": "usrnm",
+                "password": "pswd",
+                "realm": None,
+                "scope": None,
+                "audience": None,
+                "grant_type": "http://auth0.com/oauth/grant-type/password-realm",
+                "client_secret": "clsec",
+            },
+            headers={i: headers[i] for i in headers if i != "Authorization"},
+            timeout=ANY,
+        )
+
+    @aioresponses()
     async def test_file_post(self, mocked):
         callback, mock = get_callback()
         mocked.post(users_imports, callback=callback)
         j = asyncify(Jobs)(domain="example.com", token="jwt")
         users = TemporaryFile()
         self.assertEqual(await j.import_users_async("connection-1", users), payload)
         file_port_headers = headers.copy()
```

### Comparing `auth0-python-4.2.0/auth0_python.egg-info/PKG-INFO` & `auth0-python-4.3.0/auth0_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth0-python
-Version: 4.2.0
+Version: 4.3.0
 Summary: Auth0 Python SDK
 Home-page: https://github.com/auth0/auth0-python
 Author: Auth0
 Author-email: support@auth0.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: auth0-python Version: 4.2.0 Summary: Auth0 Python
+Metadata-Version: 2.1 Name: auth0-python Version: 4.3.0 Summary: Auth0 Python
 SDK Home-page: https://github.com/auth0/auth0-python Author: Auth0 Author-
 email: support@auth0.com License: MIT Platform: UNKNOWN Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `auth0-python-4.2.0/auth0_python.egg-info/SOURCES.txt` & `auth0-python-4.3.0/auth0_python.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.py
 auth0/__init__.py
 auth0/asyncify.py
 auth0/exceptions.py
 auth0/rest.py
 auth0/rest_async.py
+auth0/types.py
 auth0/utils.py
 auth0/authentication/__init__.py
 auth0/authentication/async_token_verifier.py
 auth0/authentication/base.py
 auth0/authentication/client_authentication.py
 auth0/authentication/database.py
 auth0/authentication/delegated.py
```

### Comparing `auth0-python-4.2.0/setup.py` & `auth0-python-4.3.0/setup.py`

 * *Files identical despite different names*

