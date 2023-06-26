# Comparing `tmp/fastapi-framework-1.5.3.3.tar.gz` & `tmp/fastapi_framework-1.5.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-framework-1.5.3.3.tar", last modified: Sat Feb 25 13:15:37 2023, max compression
+gzip compressed data, was "fastapi_framework-1.5.3.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fastapi-framework-1.5.3.3.tar` & `fastapi_framework-1.5.3.4.tar`

### file list

```diff
@@ -1,77 +1,76 @@
--rw-r--r--   0        0        0       25 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/.dockerignore
--rw-r--r--   0        0        0       49 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/.flake8
--rw-r--r--   0        0        0      837 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      266 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/.github/ISSUE_TEMPLATE/documentation_request.md
--rw-r--r--   0        0        0      222 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      157 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      710 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/.github/dependabot.yml
--rw-r--r--   0        0        0      673 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/.github/workflows/codestyle.yaml
--rw-r--r--   0        0        0      635 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/.github/workflows/deploy_docs.yaml
--rw-r--r--   0        0        0      513 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/.github/workflows/deploy_pypi.yaml
--rw-r--r--   0        0        0      432 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/.github/workflows/tests.yaml
--rw-r--r--   0        0        0     2100 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/.gitignore
--rw-r--r--   0        0        0     5202 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      366 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/Dockerfile
--rw-r--r--   0        0        0     1055 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/LICENSE
--rw-r--r--   0        0        0     1430 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/README.md
--rwxr-xr-x   0        0        0      188 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/coverage.sh
--rw-r--r--   0        0        0      219 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/docker-compose.yaml
--rw-r--r--   0        0        0      897 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/docs/config/index.md
--rw-r--r--   0        0        0      968 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/docs/database/example.md
--rw-r--r--   0        0        0      197 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/docs/database/index.md
--rw-r--r--   0        0        0      887 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/docs/database/insert_delete_modify.md
--rw-r--r--   0        0        0      571 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/docs/database/models.md
--rw-r--r--   0        0        0     1907 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/docs/database/query.md
--rw-r--r--   0        0        0     2012 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/docs/environment.md
--rw-r--r--   0        0        0      241 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/docs/in_memory_backends/api/delete_exists.md
--rw-r--r--   0        0        0      588 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/docs/in_memory_backends/api/expires.md
--rw-r--r--   0        0        0      301 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/docs/in_memory_backends/api/increase_decrease.md
--rw-r--r--   0        0        0      128 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/docs/in_memory_backends/api/index.md
--rw-r--r--   0        0        0      610 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/docs/in_memory_backends/api/set_get.md
--rw-r--r--   0        0        0      341 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/docs/in_memory_backends/api/sets.md
--rw-r--r--   0        0        0      246 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/docs/in_memory_backends/in_memory_backend/index.md
--rw-r--r--   0        0        0      529 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/docs/in_memory_backends/redis/connection.md
--rw-r--r--   0        0        0      103 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/docs/in_memory_backends/redis/index.md
--rw-r--r--   0        0        0     1430 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/docs/index.md
--rw-r--r--   0        0        0     2481 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/docs/jwt/example.md
--rw-r--r--   0        0        0       85 2023-02-25 13:15:33.277188 fastapi-framework-1.5.3.3/docs/jwt/index.md
--rw-r--r--   0        0        0    68491 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/docs/jwt/jwt_io_screenshot.png
--rw-r--r--   0        0        0     5713 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/docs/jwt/jwt_tokens.md
--rw-r--r--   0        0        0     1208 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/docs/rate_limit/example.md
--rw-r--r--   0        0        0      151 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/docs/rate_limit/index.md
--rw-r--r--   0        0        0      981 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/docs/rate_limit/rate_limit_manager.md
--rw-r--r--   0        0        0     3212 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/docs/session/callbacks-middleware.md
--rw-r--r--   0        0        0     1152 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/docs/session/example.md
--rw-r--r--   0        0        0       82 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/docs/session/index.md
--rw-r--r--   0        0        0      776 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/docs/session/initialize.md
--rw-r--r--   0        0        0     1975 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/docs/session/session-data.md
--rw-r--r--   0        0        0      874 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/fastapi_framework/__init__.py
--rw-r--r--   0        0        0     3793 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/fastapi_framework/config.py
--rw-r--r--   0        0        0     5334 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/fastapi_framework/database.py
--rw-r--r--   0        0        0     6949 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/fastapi_framework/in_memory_backend.py
--rw-r--r--   0        0        0     3274 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/fastapi_framework/jwt_auth.py
--rw-r--r--   0        0        0      687 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/fastapi_framework/logger.py
--rw-r--r--   0        0        0     1081 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/fastapi_framework/modules.py
--rw-r--r--   0        0        0      369 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/fastapi_framework/permissions.py
--rw-r--r--   0        0        0     4719 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/fastapi_framework/rate_limit.py
--rw-r--r--   0        0        0     3426 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/fastapi_framework/redis.py
--rw-r--r--   0        0        0     4381 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/fastapi_framework/session.py
--rw-r--r--   0        0        0     1898 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/fastapi_framework/settings.py
--rw-r--r--   0        0        0     1977 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/mkdocs.yml
--rw-r--r--   0        0        0       63 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/mypy.ini
--rw-r--r--   0        0        0     1176 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/pyproject.toml
--rw-r--r--   0        0        0      141 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/requirements.txt
--rw-r--r--   0        0        0      687 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/setup.py
--rw-r--r--   0        0        0      379 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/test.env
--rwxr-xr-x   0        0        0       46 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/test.sh
--rw-r--r--   0        0        0     4062 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/tests/test_config.py
--rw-r--r--   0        0        0     7176 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/tests/test_database.py
--rw-r--r--   0        0        0     9343 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/tests/test_in_memory_backend.py
--rw-r--r--   0        0        0     9258 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/tests/test_jwt_auth.py
--rw-r--r--   0        0        0     1498 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/tests/test_logger.py
--rw-r--r--   0        0        0      735 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/tests/test_modules.py
--rw-r--r--   0        0        0     6220 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/tests/test_rate_limit.py
--rw-r--r--   0        0        0     3481 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/tests/test_redis.py
--rw-r--r--   0        0        0    10376 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/tests/test_session.py
--rw-r--r--   0        0        0     2443 2023-02-25 13:15:33.281188 fastapi-framework-1.5.3.3/tests/test_settings.py
--rw-r--r--   0        0        0     2937 1970-01-01 00:00:00.000000 fastapi-framework-1.5.3.3/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-06-26 12:53:26.831052 fastapi_framework-1.5.3.4/.dockerignore
+-rw-r--r--   0        0        0       49 2023-06-26 12:53:26.831052 fastapi_framework-1.5.3.4/.flake8
+-rw-r--r--   0        0        0      837 2023-06-26 12:53:26.831052 fastapi_framework-1.5.3.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      266 2023-06-26 12:53:26.831052 fastapi_framework-1.5.3.4/.github/ISSUE_TEMPLATE/documentation_request.md
+-rw-r--r--   0        0        0      222 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      157 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      710 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/.github/dependabot.yml
+-rw-r--r--   0        0        0      673 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/.github/workflows/codestyle.yaml
+-rw-r--r--   0        0        0      635 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/.github/workflows/deploy_docs.yaml
+-rw-r--r--   0        0        0      515 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/.github/workflows/deploy_pypi.yaml
+-rw-r--r--   0        0        0      432 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0     2100 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/.gitignore
+-rw-r--r--   0        0        0     5202 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      434 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/Dockerfile
+-rw-r--r--   0        0        0     1055 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/LICENSE
+-rw-r--r--   0        0        0     1430 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/README.md
+-rwxr-xr-x   0        0        0      188 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/coverage.sh
+-rw-r--r--   0        0        0      219 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docker-compose.yaml
+-rw-r--r--   0        0        0      897 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/config/index.md
+-rw-r--r--   0        0        0      968 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/database/example.md
+-rw-r--r--   0        0        0      197 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/database/index.md
+-rw-r--r--   0        0        0      887 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/database/insert_delete_modify.md
+-rw-r--r--   0        0        0      571 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/database/models.md
+-rw-r--r--   0        0        0     1907 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/database/query.md
+-rw-r--r--   0        0        0     2012 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/environment.md
+-rw-r--r--   0        0        0      241 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/in_memory_backends/api/delete_exists.md
+-rw-r--r--   0        0        0      588 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/in_memory_backends/api/expires.md
+-rw-r--r--   0        0        0      301 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/in_memory_backends/api/increase_decrease.md
+-rw-r--r--   0        0        0      128 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/in_memory_backends/api/index.md
+-rw-r--r--   0        0        0      610 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/in_memory_backends/api/set_get.md
+-rw-r--r--   0        0        0      341 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/in_memory_backends/api/sets.md
+-rw-r--r--   0        0        0      246 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/in_memory_backends/in_memory_backend/index.md
+-rw-r--r--   0        0        0      529 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/in_memory_backends/redis/connection.md
+-rw-r--r--   0        0        0      103 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/in_memory_backends/redis/index.md
+-rw-r--r--   0        0        0     1430 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/index.md
+-rw-r--r--   0        0        0     2481 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/jwt/example.md
+-rw-r--r--   0        0        0       85 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/jwt/index.md
+-rw-r--r--   0        0        0    68491 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/jwt/jwt_io_screenshot.png
+-rw-r--r--   0        0        0     5713 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/jwt/jwt_tokens.md
+-rw-r--r--   0        0        0     1208 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/rate_limit/example.md
+-rw-r--r--   0        0        0      151 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/rate_limit/index.md
+-rw-r--r--   0        0        0      981 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/rate_limit/rate_limit_manager.md
+-rw-r--r--   0        0        0     3212 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/session/callbacks-middleware.md
+-rw-r--r--   0        0        0     1152 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/session/example.md
+-rw-r--r--   0        0        0       82 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/session/index.md
+-rw-r--r--   0        0        0      776 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/session/initialize.md
+-rw-r--r--   0        0        0     1975 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/docs/session/session-data.md
+-rw-r--r--   0        0        0      874 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/fastapi_framework/__init__.py
+-rw-r--r--   0        0        0     3793 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/fastapi_framework/config.py
+-rw-r--r--   0        0        0     5334 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/fastapi_framework/database.py
+-rw-r--r--   0        0        0     6949 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/fastapi_framework/in_memory_backend.py
+-rw-r--r--   0        0        0     3274 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/fastapi_framework/jwt_auth.py
+-rw-r--r--   0        0        0      687 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/fastapi_framework/logger.py
+-rw-r--r--   0        0        0     1081 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/fastapi_framework/modules.py
+-rw-r--r--   0        0        0      369 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/fastapi_framework/permissions.py
+-rw-r--r--   0        0        0     4719 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/fastapi_framework/rate_limit.py
+-rw-r--r--   0        0        0     3426 2023-06-26 12:53:26.835052 fastapi_framework-1.5.3.4/fastapi_framework/redis.py
+-rw-r--r--   0        0        0     4381 2023-06-26 12:53:26.839052 fastapi_framework-1.5.3.4/fastapi_framework/session.py
+-rw-r--r--   0        0        0     1898 2023-06-26 12:53:26.839052 fastapi_framework-1.5.3.4/fastapi_framework/settings.py
+-rw-r--r--   0        0        0     1977 2023-06-26 12:53:26.839052 fastapi_framework-1.5.3.4/mkdocs.yml
+-rw-r--r--   0        0        0       63 2023-06-26 12:53:26.839052 fastapi_framework-1.5.3.4/mypy.ini
+-rw-r--r--   0        0        0     1213 2023-06-26 12:53:26.839052 fastapi_framework-1.5.3.4/pyproject.toml
+-rw-r--r--   0        0        0      687 2023-06-26 12:53:26.839052 fastapi_framework-1.5.3.4/setup.py
+-rw-r--r--   0        0        0      379 2023-06-26 12:53:26.839052 fastapi_framework-1.5.3.4/test.env
+-rwxr-xr-x   0        0        0       46 2023-06-26 12:53:26.839052 fastapi_framework-1.5.3.4/test.sh
+-rw-r--r--   0        0        0     4062 2023-06-26 12:53:26.839052 fastapi_framework-1.5.3.4/tests/test_config.py
+-rw-r--r--   0        0        0     7176 2023-06-26 12:53:26.839052 fastapi_framework-1.5.3.4/tests/test_database.py
+-rw-r--r--   0        0        0     9343 2023-06-26 12:53:26.839052 fastapi_framework-1.5.3.4/tests/test_in_memory_backend.py
+-rw-r--r--   0        0        0     9258 2023-06-26 12:53:26.839052 fastapi_framework-1.5.3.4/tests/test_jwt_auth.py
+-rw-r--r--   0        0        0     1498 2023-06-26 12:53:26.839052 fastapi_framework-1.5.3.4/tests/test_logger.py
+-rw-r--r--   0        0        0      735 2023-06-26 12:53:26.839052 fastapi_framework-1.5.3.4/tests/test_modules.py
+-rw-r--r--   0        0        0     6220 2023-06-26 12:53:26.839052 fastapi_framework-1.5.3.4/tests/test_rate_limit.py
+-rw-r--r--   0        0        0     3481 2023-06-26 12:53:26.839052 fastapi_framework-1.5.3.4/tests/test_redis.py
+-rw-r--r--   0        0        0    10376 2023-06-26 12:53:26.839052 fastapi_framework-1.5.3.4/tests/test_session.py
+-rw-r--r--   0        0        0     2443 2023-06-26 12:53:26.839052 fastapi_framework-1.5.3.4/tests/test_settings.py
+-rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 fastapi_framework-1.5.3.4/PKG-INFO
```

### Comparing `fastapi-framework-1.5.3.3/.github/ISSUE_TEMPLATE/bug_report.md` & `fastapi_framework-1.5.3.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/.github/dependabot.yml` & `fastapi_framework-1.5.3.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/.github/workflows/codestyle.yaml` & `fastapi_framework-1.5.3.4/.github/workflows/codestyle.yaml`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/.github/workflows/deploy_docs.yaml` & `fastapi_framework-1.5.3.4/.github/workflows/deploy_docs.yaml`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/.github/workflows/deploy_pypi.yaml` & `fastapi_framework-1.5.3.4/.github/workflows/deploy_pypi.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 jobs:
   publish:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v3
 
-      - name: Set up Python 3.9
+      - name: Set up Python 3.10
         uses: actions/setup-python@v4
         with:
-          python-version: "3.9"
+          python-version: "3.10"
 
       - name: Install Flit
         run: pip install flit
 
       - name: Publish
         env:
           FLIT_USERNAME: ${{ secrets.FLIT_USERNAME }}
```

### Comparing `fastapi-framework-1.5.3.3/.gitignore` & `fastapi_framework-1.5.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/CODE_OF_CONDUCT.md` & `fastapi_framework-1.5.3.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/LICENSE` & `fastapi_framework-1.5.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/README.md` & `fastapi_framework-1.5.3.4/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/docs/config/index.md` & `fastapi_framework-1.5.3.4/docs/config/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/docs/database/example.md` & `fastapi_framework-1.5.3.4/docs/database/example.md`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/docs/database/insert_delete_modify.md` & `fastapi_framework-1.5.3.4/docs/database/insert_delete_modify.md`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/docs/database/models.md` & `fastapi_framework-1.5.3.4/docs/database/models.md`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/docs/database/query.md` & `fastapi_framework-1.5.3.4/docs/database/query.md`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/docs/environment.md` & `fastapi_framework-1.5.3.4/docs/environment.md`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/docs/in_memory_backends/api/expires.md` & `fastapi_framework-1.5.3.4/docs/in_memory_backends/api/expires.md`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/docs/in_memory_backends/api/set_get.md` & `fastapi_framework-1.5.3.4/docs/in_memory_backends/api/set_get.md`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/docs/in_memory_backends/redis/connection.md` & `fastapi_framework-1.5.3.4/docs/in_memory_backends/redis/connection.md`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/docs/index.md` & `fastapi_framework-1.5.3.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/docs/jwt/example.md` & `fastapi_framework-1.5.3.4/docs/jwt/example.md`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/docs/jwt/jwt_io_screenshot.png` & `fastapi_framework-1.5.3.4/docs/jwt/jwt_io_screenshot.png`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/docs/jwt/jwt_tokens.md` & `fastapi_framework-1.5.3.4/docs/jwt/jwt_tokens.md`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/docs/rate_limit/example.md` & `fastapi_framework-1.5.3.4/docs/rate_limit/example.md`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/docs/rate_limit/rate_limit_manager.md` & `fastapi_framework-1.5.3.4/docs/rate_limit/rate_limit_manager.md`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/docs/session/callbacks-middleware.md` & `fastapi_framework-1.5.3.4/docs/session/callbacks-middleware.md`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/docs/session/example.md` & `fastapi_framework-1.5.3.4/docs/session/example.md`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/docs/session/initialize.md` & `fastapi_framework-1.5.3.4/docs/session/initialize.md`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/docs/session/session-data.md` & `fastapi_framework-1.5.3.4/docs/session/session-data.md`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/fastapi_framework/__init__.py` & `fastapi_framework-1.5.3.4/fastapi_framework/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A FastAPI Framework for things like Database, Redis, Logging, JWT Authentication and Rate Limits"""
 
-__version__ = "1.5.3.3"
+__version__ = "1.5.3.4"
 
 from .modules import check_dependencies, disabled_modules
 
 check_dependencies()  # noqa: FLK-E402
 from .database import database_dependency
 from .jwt_auth import (
     create_jwt_token,
```

### Comparing `fastapi-framework-1.5.3.3/fastapi_framework/config.py` & `fastapi_framework-1.5.3.4/fastapi_framework/config.py`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/fastapi_framework/database.py` & `fastapi_framework-1.5.3.4/fastapi_framework/database.py`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/fastapi_framework/in_memory_backend.py` & `fastapi_framework-1.5.3.4/fastapi_framework/in_memory_backend.py`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/fastapi_framework/jwt_auth.py` & `fastapi_framework-1.5.3.4/fastapi_framework/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/fastapi_framework/logger.py` & `fastapi_framework-1.5.3.4/fastapi_framework/logger.py`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/fastapi_framework/modules.py` & `fastapi_framework-1.5.3.4/fastapi_framework/modules.py`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/fastapi_framework/rate_limit.py` & `fastapi_framework-1.5.3.4/fastapi_framework/rate_limit.py`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/fastapi_framework/redis.py` & `fastapi_framework-1.5.3.4/fastapi_framework/redis.py`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/fastapi_framework/session.py` & `fastapi_framework-1.5.3.4/fastapi_framework/session.py`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/fastapi_framework/settings.py` & `fastapi_framework-1.5.3.4/fastapi_framework/settings.py`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/mkdocs.yml` & `fastapi_framework-1.5.3.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/pyproject.toml` & `fastapi_framework-1.5.3.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 [build-system]
-requires = ["flit_core >=2,<4"]
+requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
-[tool.flit.metadata]
-dist-name = "fastapi-framework"
-module = "fastapi_framework"
-author = "Tert0"
-home-page = "https://github.com/Tert0/fastapi-framework"
+[project]
+name = "fastapi-framework"
+authors = [
+    {name = "Tert0"}
+]
+readme = "README.md"
 classifiers = [ "License :: OSI Approved :: MIT License", "Framework :: AsyncIO", "Intended Audience :: Developers", "Operating System :: POSIX :: Linux", "Programming Language :: Python :: 3.9", "Programming Language :: Python :: Implementation :: CPython", "Topic :: Database", "Topic :: Software Development :: Libraries", "Topic :: Software Development :: Libraries :: Python Modules", "Typing :: Typed"]
-description-file = "README.md"
-requires = [
-    "fastapi==0.92.0",
+requires-python = ">=3.6"
+dynamic = ["version", "description"]
+
+dependencies = [
+    "fastapi==0.98.0",
     "aioredis==1.3.1",
     "passlib==1.7.4",
-    "PyJWT==2.6.0",
+    "PyJWT==2.7.0",
     "python-dotenv==1.0.0",
-    "SQLAlchemy==2.0.4",
+    "SQLAlchemy==2.0.17",
     "pyyaml==6.0",
     "toml==0.10.2",
-    "pydantic==1.10.5"
+    "pydantic==1.10.9"
 ]
 
-[tool.flit.metadata.requires-extra]
+[project.urls]
+Documentation = "https://tert0.github.io/fastapi-framework"
+Source = "https://github.com/Tert0/fastapi-framework"
+
+[project.optional-dependencies]
 test = [
     "httpx",
-    "coverage"
+    "coverage",
+    "aiosqlite"
+]
+doc = [
+    "mkdocs-material"
 ]
-doc = ["mkdocs-material"]
 lint = [
     "black",
     "flake8",
     "mypy",
     "types-PyYAML",
     "types-toml"
-]
-
-[tool.flit.metadata.urls]
-Documentation = "https://tert0.github.io/fastapi-framework/"
+]
```

### Comparing `fastapi-framework-1.5.3.3/setup.py` & `fastapi_framework-1.5.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/tests/test_config.py` & `fastapi_framework-1.5.3.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/tests/test_database.py` & `fastapi_framework-1.5.3.4/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/tests/test_in_memory_backend.py` & `fastapi_framework-1.5.3.4/tests/test_in_memory_backend.py`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/tests/test_jwt_auth.py` & `fastapi_framework-1.5.3.4/tests/test_jwt_auth.py`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/tests/test_logger.py` & `fastapi_framework-1.5.3.4/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/tests/test_modules.py` & `fastapi_framework-1.5.3.4/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/tests/test_rate_limit.py` & `fastapi_framework-1.5.3.4/tests/test_rate_limit.py`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/tests/test_redis.py` & `fastapi_framework-1.5.3.4/tests/test_redis.py`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/tests/test_session.py` & `fastapi_framework-1.5.3.4/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/tests/test_settings.py` & `fastapi_framework-1.5.3.4/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `fastapi-framework-1.5.3.3/PKG-INFO` & `fastapi_framework-1.5.3.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: fastapi-framework
-Version: 1.5.3.3
+Version: 1.5.3.4
 Summary: A FastAPI Framework for things like Database, Redis, Logging, JWT Authentication and Rate Limits
-Home-page: https://github.com/Tert0/fastapi-framework
 Author: Tert0
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Dist: fastapi==0.92.0
+Requires-Dist: fastapi==0.98.0
 Requires-Dist: aioredis==1.3.1
 Requires-Dist: passlib==1.7.4
-Requires-Dist: PyJWT==2.6.0
+Requires-Dist: PyJWT==2.7.0
 Requires-Dist: python-dotenv==1.0.0
-Requires-Dist: SQLAlchemy==2.0.4
+Requires-Dist: SQLAlchemy==2.0.17
 Requires-Dist: pyyaml==6.0
 Requires-Dist: toml==0.10.2
-Requires-Dist: pydantic==1.10.5
+Requires-Dist: pydantic==1.10.9
 Requires-Dist: mkdocs-material ; extra == "doc"
 Requires-Dist: black ; extra == "lint"
 Requires-Dist: flake8 ; extra == "lint"
 Requires-Dist: mypy ; extra == "lint"
 Requires-Dist: types-PyYAML ; extra == "lint"
 Requires-Dist: types-toml ; extra == "lint"
 Requires-Dist: httpx ; extra == "test"
 Requires-Dist: coverage ; extra == "test"
-Project-URL: Documentation, https://tert0.github.io/fastapi-framework/
+Requires-Dist: aiosqlite ; extra == "test"
+Project-URL: Documentation, https://tert0.github.io/fastapi-framework
+Project-URL: Source, https://github.com/Tert0/fastapi-framework
 Provides-Extra: doc
 Provides-Extra: lint
 Provides-Extra: test
 
 [![Codestyle](https://github.com/Tert0/fastapi-framework/actions/workflows/codestyle.yaml/badge.svg)](https://github.com/Tert0/fastapi-framework/actions/workflows/codestyle.yaml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Tests](https://github.com/Tert0/fastapi-framework/actions/workflows/tests.yaml/badge.svg)](https://github.com/Tert0/fastapi-framework/actions/workflows/tests.yaml)
```

