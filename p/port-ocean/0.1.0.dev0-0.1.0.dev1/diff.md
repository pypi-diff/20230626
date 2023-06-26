# Comparing `tmp/port_ocean-0.1.0.dev0.tar.gz` & `tmp/port_ocean-0.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_ocean-0.1.0.dev0.tar", max compression
+gzip compressed data, was "port_ocean-0.1.0.dev1.tar", max compression
```

## Comparing `port_ocean-0.1.0.dev0.tar` & `port_ocean-0.1.0.dev1.tar`

### file list

```diff
@@ -1,61 +1,62 @@
--rw-r--r--   0        0        0     3218 2023-06-19 13:04:16.027920 port_ocean-0.1.0.dev0/README.md
--rw-r--r--   0        0        0      440 2023-06-19 13:04:16.083920 port_ocean-0.1.0.dev0/port_ocean/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 13:04:16.083920 port_ocean-0.1.0.dev0/port_ocean/cli/__init__.py
--rw-r--r--   0        0        0      121 2023-06-19 13:04:16.083920 port_ocean-0.1.0.dev0/port_ocean/cli/cli.py
--rw-r--r--   0        0        0     3386 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/cli/commands.py
--rw-r--r--   0        0        0      429 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/cli/cookiecutter/cookiecutter.json
--rw-r--r--   0        0        0       54 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
--rw-r--r--   0        0        0      598 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
--rw-r--r--   0        0        0      751 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
--rw-r--r--   0        0        0      406 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
--rw-r--r--   0        0        0     1091 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/example.config.yaml
--rw-r--r--   0        0        0      452 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
--rw-r--r--   0        0        0      640 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/project.toml
--rw-r--r--   0        0        0        0 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
--rw-r--r--   0        0        0     1334 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/cli/download_git_folder.py
--rw-r--r--   0        0        0      766 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/cli/list_integrations.py
--rw-r--r--   0        0        0        0 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/clients/port/__init__.py
--rw-r--r--   0        0        0     9170 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/clients/port/client.py
--rw-r--r--   0        0        0      708 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/clients/port/types.py
--rw-r--r--   0        0        0        0 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/config/__init__.py
--rw-r--r--   0        0        0     1940 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/config/base.py
--rw-r--r--   0        0        0      964 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/config/integration.py
--rw-r--r--   0        0        0        0 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/consumers/__init__.py
--rw-r--r--   0        0        0      125 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/consumers/base_consumer.py
--rw-r--r--   0        0        0     3785 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/consumers/kafka_consumer.py
--rw-r--r--   0        0        0        0 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/context/__init__.py
--rw-r--r--   0        0        0     1525 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/context/event.py
--rw-r--r--   0        0        0     2706 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/context/integration.py
--rw-r--r--   0        0        0        0 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/core/__init__.py
--rw-r--r--   0        0        0      225 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/core/base.py
--rw-r--r--   0        0        0      225 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/core/handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/core/handlers/manipulation/__init__.py
--rw-r--r--   0        0        0     1216 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/core/handlers/manipulation/base.py
--rw-r--r--   0        0        0     3654 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/core/handlers/manipulation/jq_manipulation.py
--rw-r--r--   0        0        0        0 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/core/handlers/port_app_config/__init__.py
--rw-r--r--   0        0        0      548 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/core/handlers/port_app_config/api.py
--rw-r--r--   0        0        0      301 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/core/handlers/port_app_config/base.py
--rw-r--r--   0        0        0     1834 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/core/handlers/port_app_config/models.py
--rw-r--r--   0        0        0        0 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/core/handlers/transport/__init__.py
--rw-r--r--   0        0        0      308 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/core/handlers/transport/base.py
--rw-r--r--   0        0        0        0 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/core/handlers/transport/port/__init__.py
--rw-r--r--   0        0        0     1198 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/core/handlers/transport/port/get_required_entities.py
--rw-r--r--   0        0        0     1062 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py
--rw-r--r--   0        0        0     3856 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/core/handlers/transport/port/transport.py
--rw-r--r--   0        0        0     1545 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/core/handlers/transport/port/validate_entity_relations.py
--rw-r--r--   0        0        0        0 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/core/integrations/__init__.py
--rw-r--r--   0        0        0     5121 2023-06-19 13:04:16.087920 port_ocean-0.1.0.dev0/port_ocean/core/integrations/base.py
--rw-r--r--   0        0        0     2724 2023-06-19 13:04:16.091920 port_ocean-0.1.0.dev0/port_ocean/core/integrations/mixins.py
--rw-r--r--   0        0        0      395 2023-06-19 13:04:16.091920 port_ocean-0.1.0.dev0/port_ocean/core/models.py
--rw-r--r--   0        0        0        0 2023-06-19 13:04:16.091920 port_ocean-0.1.0.dev0/port_ocean/core/trigger_channel/__init__.py
--rw-r--r--   0        0        0      444 2023-06-19 13:04:16.091920 port_ocean-0.1.0.dev0/port_ocean/core/trigger_channel/base_trigger_channel.py
--rw-r--r--   0        0        0     2112 2023-06-19 13:04:16.091920 port_ocean-0.1.0.dev0/port_ocean/core/trigger_channel/kafka_trigger_channel.py
--rw-r--r--   0        0        0     2580 2023-06-19 13:04:16.091920 port_ocean-0.1.0.dev0/port_ocean/core/trigger_channel/trigger_channel_factory.py
--rw-r--r--   0        0        0     2292 2023-06-19 13:04:16.091920 port_ocean-0.1.0.dev0/port_ocean/core/utils.py
--rw-r--r--   0        0        0      166 2023-06-19 13:04:16.091920 port_ocean-0.1.0.dev0/port_ocean/errors.py
--rw-r--r--   0        0        0      534 2023-06-19 13:04:16.091920 port_ocean-0.1.0.dev0/port_ocean/logging.py
--rw-r--r--   0        0        0     3944 2023-06-19 13:04:16.091920 port_ocean-0.1.0.dev0/port_ocean/port_ocean.py
--rw-r--r--   0        0        0      400 2023-06-19 13:04:16.091920 port_ocean-0.1.0.dev0/port_ocean/types.py
--rw-r--r--   0        0        0     1869 2023-06-19 13:04:16.091920 port_ocean-0.1.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     4292 1970-01-01 00:00:00.000000 port_ocean-0.1.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0     3218 2023-06-26 14:41:58.550973 port_ocean-0.1.0.dev1/README.md
+-rw-r--r--   0        0        0      440 2023-06-26 14:41:58.586973 port_ocean-0.1.0.dev1/port_ocean/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 14:41:58.586973 port_ocean-0.1.0.dev1/port_ocean/cli/__init__.py
+-rw-r--r--   0        0        0      121 2023-06-26 14:41:58.586973 port_ocean-0.1.0.dev1/port_ocean/cli/cli.py
+-rw-r--r--   0        0        0     3385 2023-06-26 14:41:58.586973 port_ocean-0.1.0.dev1/port_ocean/cli/commands.py
+-rw-r--r--   0        0        0      429 2023-06-26 14:41:58.586973 port_ocean-0.1.0.dev1/port_ocean/cli/cookiecutter/cookiecutter.json
+-rw-r--r--   0        0        0       54 2023-06-26 14:41:58.586973 port_ocean-0.1.0.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
+-rw-r--r--   0        0        0      598 2023-06-26 14:41:58.586973 port_ocean-0.1.0.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
+-rw-r--r--   0        0        0      751 2023-06-26 14:41:58.586973 port_ocean-0.1.0.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
+-rw-r--r--   0        0        0      406 2023-06-26 14:41:58.586973 port_ocean-0.1.0.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
+-rw-r--r--   0        0        0     1091 2023-06-26 14:41:58.586973 port_ocean-0.1.0.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/example.config.yaml
+-rw-r--r--   0        0        0      404 2023-06-26 14:41:58.586973 port_ocean-0.1.0.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
+-rw-r--r--   0        0        0      640 2023-06-26 14:41:58.586973 port_ocean-0.1.0.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/project.toml
+-rw-r--r--   0        0        0        0 2023-06-26 14:41:58.586973 port_ocean-0.1.0.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0     1334 2023-06-26 14:41:58.586973 port_ocean-0.1.0.dev1/port_ocean/cli/download_git_folder.py
+-rw-r--r--   0        0        0      766 2023-06-26 14:41:58.586973 port_ocean-0.1.0.dev1/port_ocean/cli/list_integrations.py
+-rw-r--r--   0        0        0        0 2023-06-26 14:41:58.586973 port_ocean-0.1.0.dev1/port_ocean/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 14:41:58.586973 port_ocean-0.1.0.dev1/port_ocean/clients/port/__init__.py
+-rw-r--r--   0        0        0    11004 2023-06-26 14:41:58.586973 port_ocean-0.1.0.dev1/port_ocean/clients/port/client.py
+-rw-r--r--   0        0        0      700 2023-06-26 14:41:58.586973 port_ocean-0.1.0.dev1/port_ocean/clients/port/types.py
+-rw-r--r--   0        0        0        0 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/config/__init__.py
+-rw-r--r--   0        0        0     1984 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/config/base.py
+-rw-r--r--   0        0        0     1453 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/config/integration.py
+-rw-r--r--   0        0        0        0 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/consumers/__init__.py
+-rw-r--r--   0        0        0      125 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/consumers/base_consumer.py
+-rw-r--r--   0        0        0     3785 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/consumers/kafka_consumer.py
+-rw-r--r--   0        0        0        0 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/context/__init__.py
+-rw-r--r--   0        0        0     1902 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/context/event.py
+-rw-r--r--   0        0        0     3290 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/context/ocean.py
+-rw-r--r--   0        0        0        0 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/base.py
+-rw-r--r--   0        0        0      300 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/handlers/manipulation/__init__.py
+-rw-r--r--   0        0        0      715 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/handlers/manipulation/base.py
+-rw-r--r--   0        0        0     2822 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/handlers/manipulation/jq_manipulation.py
+-rw-r--r--   0        0        0        0 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/handlers/port_app_config/__init__.py
+-rw-r--r--   0        0        0      458 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/handlers/port_app_config/api.py
+-rw-r--r--   0        0        0      657 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/handlers/port_app_config/base.py
+-rw-r--r--   0        0        0     1438 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/handlers/port_app_config/models.py
+-rw-r--r--   0        0        0        0 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/handlers/transport/__init__.py
+-rw-r--r--   0        0        0      925 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/handlers/transport/base.py
+-rw-r--r--   0        0        0        0 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/handlers/transport/port/__init__.py
+-rw-r--r--   0        0        0     1205 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/handlers/transport/port/get_required_entities.py
+-rw-r--r--   0        0        0     1062 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py
+-rw-r--r--   0        0        0     4698 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/handlers/transport/port/transport.py
+-rw-r--r--   0        0        0     1495 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/handlers/transport/port/validate_entity_relations.py
+-rw-r--r--   0        0        0        0 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/integrations/__init__.py
+-rw-r--r--   0        0        0     4283 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/integrations/base.py
+-rw-r--r--   0        0        0     7212 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/integrations/mixins.py
+-rw-r--r--   0        0        0      600 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/models.py
+-rw-r--r--   0        0        0        0 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/trigger_channel/__init__.py
+-rw-r--r--   0        0        0      444 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/trigger_channel/base_trigger_channel.py
+-rw-r--r--   0        0        0     2106 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/trigger_channel/kafka_trigger_channel.py
+-rw-r--r--   0        0        0     2657 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/trigger_channel/trigger_channel_factory.py
+-rw-r--r--   0        0        0     1772 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/core/utils.py
+-rw-r--r--   0        0        0      166 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/errors.py
+-rw-r--r--   0        0        0      534 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/logging.py
+-rw-r--r--   0        0        0     2815 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/middlewares.py
+-rw-r--r--   0        0        0     4435 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/port_ocean.py
+-rw-r--r--   0        0        0      583 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/port_ocean/types.py
+-rw-r--r--   0        0        0     1845 2023-06-26 14:41:58.590973 port_ocean-0.1.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     4247 1970-01-01 00:00:00.000000 port_ocean-0.1.0.dev1/PKG-INFO
```

### Comparing `port_ocean-0.1.0.dev0/README.md` & `port_ocean-0.1.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev0/port_ocean/cli/commands.py` & `port_ocean-0.1.0.dev1/port_ocean/cli/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 @click.group()
 def cli_start() -> None:
     # Ocean root command
     pass
 
 
 @cli_start.command()
-@click.argument("path", default=".")
+@click.argument("path", default="")
 def sail(path: str) -> None:
     from port_ocean.port_ocean import run
 
     print_logo()
 
     print("Setting sail... ⛵️⚓️⛵️⚓️ All hands on deck! ⚓️")
     run(path)
```

### Comparing `port_ocean-0.1.0.dev0/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile` & `port_ocean-0.1.0.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev0/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile` & `port_ocean-0.1.0.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev0/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/example.config.yaml` & `port_ocean-0.1.0.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/example.config.yaml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev0/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/project.toml` & `port_ocean-0.1.0.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/project.toml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev0/port_ocean/cli/download_git_folder.py` & `port_ocean-0.1.0.dev1/port_ocean/cli/download_git_folder.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev0/port_ocean/cli/list_integrations.py` & `port_ocean-0.1.0.dev1/port_ocean/cli/list_integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev0/port_ocean/clients/port/client.py` & `port_ocean-0.1.0.dev1/port_ocean/clients/port/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from loguru import logger
 from pydantic import BaseModel, Field, PrivateAttr
 
 from port_ocean.clients.port.types import (
     KafkaCreds,
     ChangelogDestination,
     RequestOptions,
+    UserAgentType,
 )
-from port_ocean.core.handlers.port_app_config.models import PortAppConfig
 from port_ocean.core.models import Entity, Blueprint
 
 
 class TokenResponse(BaseModel):
     access_token: str = Field(alias="accessToken")
     expires_in: int = Field(alias="expiresIn")
     token_type: str = Field(alias="tokenType")
@@ -30,38 +30,46 @@
     @property
     def full_token(self) -> str:
         return f"{self.token_type} {self.access_token}"
 
 
 class PortClient:
     def __init__(
-        self, base_url: str, client_id: str, client_secret: str, user_agent: str
+        self, base_url: str, client_id: str, client_secret: str, user_agent_id: str
     ):
         self.api_url = base_url
         self.client_id = client_id
         self.client_secret = client_secret
-        self.user_agent = user_agent
+        self.user_agent_id = user_agent_id
         self._last_token_object: TokenResponse | None = None
 
     async def _get_token(self, client_id: str, client_secret: str) -> TokenResponse:
         async with httpx.AsyncClient() as client:
             logger.info(f"Fetching access token for clientId: {client_id}")
 
             credentials = {"clientId": client_id, "clientSecret": client_secret}
             token_response = await client.post(
                 f"{self.api_url}/auth/access_token", json=credentials
             )
             token_response.raise_for_status()
             return TokenResponse(**token_response.json())
 
-    @property
-    async def headers(self) -> Dict[Any, Any]:
+    def _user_agent(self, user_agent_type: UserAgentType | None = None) -> str:
+        user_agent = f"port-ocean/{self.user_agent_id}"
+        if user_agent_type:
+            user_agent += f"/{user_agent_type.value or UserAgentType.exporter.value}"
+
+        return user_agent
+
+    async def _headers(
+        self, user_agent_type: UserAgentType | None = None
+    ) -> Dict[Any, Any]:
         return {
             "Authorization": await self.token,
-            "User-Agent": self.user_agent,
+            "User-Agent": self._user_agent(user_agent_type),
         }
 
     @property
     async def token(self) -> str:
         logger.info("Fetching access token")
         if not self._last_token_object or self._last_token_object.expired:
             self._last_token_object = await self._get_token(
@@ -69,26 +77,30 @@
             )
         else:
             logger.info("Access token found in cache")
 
         return self._last_token_object.full_token
 
     async def upsert_entity(
-        self, entity: Entity, request_options: RequestOptions
+        self,
+        entity: Entity,
+        request_options: RequestOptions,
+        user_agent_type: UserAgentType | None = None,
     ) -> None:
         validation_only = request_options.get("validation_only", False)
         logger.info(
             f"{'Validating' if validation_only else 'Upserting'} entity: {entity.identifier} of blueprint: {entity.blueprint}"
         )
+        headers = await self._headers(user_agent_type)
 
         async with httpx.AsyncClient() as client:
             response = await client.post(
                 f"{self.api_url}/blueprints/{entity.blueprint}/entities",
                 json=entity.dict(exclude_unset=True),
-                headers=await self.headers,
+                headers=headers,
                 params={
                     "upsert": "true",
                     "merge": str(request_options.get("merge", False)).lower(),
                     "create_missing_related_entities": str(
                         request_options.get("create_missing_related_entities", False)
                     ).lower(),
                     "validation_only": str(validation_only).lower(),
@@ -98,24 +110,26 @@
         if not response.status_code < 400:
             logger.error(
                 f"Error upserting "
                 f"entity: {entity.identifier} of "
                 f"blueprint: {entity.blueprint}, "
                 f"error: {response.text}"
             )
-            response.raise_for_status()
+        response.raise_for_status()
 
-    async def delete_entity(self, entity: Entity) -> None:
+    async def delete_entity(
+        self, entity: Entity, user_agent_type: UserAgentType | None = None
+    ) -> None:
         logger.info(
             f"Delete entity: {entity.identifier} of blueprint: {entity.blueprint}"
         )
         async with httpx.AsyncClient() as client:
             response = await client.delete(
                 f"{self.api_url}/blueprints/{entity.blueprint}/entities/{entity.identifier}",
-                headers=await self.headers,
+                headers=await self._headers(user_agent_type),
                 params={"delete_dependents": "true"},
             )
 
         if not response.status_code < 400:
             logger.error(
                 f"Error deleting "
                 f"entity: {entity.identifier} of "
@@ -124,15 +138,15 @@
             )
             response.raise_for_status()
 
     async def get_kafka_creds(self) -> KafkaCreds:
         logger.info("Fetching organization kafka credentials")
         async with httpx.AsyncClient() as client:
             response = await client.get(
-                f"{self.api_url}/kafka-credentials", headers=await self.headers
+                f"{self.api_url}/kafka-credentials", headers=await self._headers()
             )
         if not response.status_code < 400:
             logger.error(f"Error getting kafka credentials, error: {response.text}")
             response.raise_for_status()
 
         credentials = response.json()["credentials"]
 
@@ -142,51 +156,84 @@
         return credentials
 
     async def get_org_id(self) -> str:
         logger.info("Fetching organization id")
 
         async with httpx.AsyncClient() as client:
             response = await client.get(
-                f"{self.api_url}/organization", headers=await self.headers
+                f"{self.api_url}/organization", headers=await self._headers()
             )
         if not response.status_code < 400:
             logger.error(f"Error getting organization id, error: {response.text}")
             response.raise_for_status()
 
         return response.json()["organization"]["id"]
 
     async def validate_entity_exist(self, identifier: str, blueprint: str) -> None:
         logger.info(f"Validating entity {identifier} of blueprint {blueprint} exists")
 
         async with httpx.AsyncClient() as client:
             response = await client.get(
-                f"{self.api_url}/v1/blueprints/{blueprint}/entities/{identifier}",
-                headers=await self.headers,
+                f"{self.api_url}/blueprints/{blueprint}/entities/{identifier}",
+                headers=await self._headers(),
+            )
+        if response.status_code >= 400:
+            logger.error(
+                f"Error validating "
+                f"entity: {identifier} of "
+                f"blueprint: {blueprint}, "
+                f"error: {response.text}"
             )
         response.raise_for_status()
 
+    async def search_entities(self, user_agent_type: UserAgentType) -> List[Entity]:
+        query = {
+            "combinator": "and",
+            "rules": [
+                {
+                    "property": "$datasource",
+                    "operator": "=",
+                    "value": self._user_agent(user_agent_type),
+                },
+            ],
+        }
+
+        async with httpx.AsyncClient() as client:
+            search_req = await client.post(
+                f"{self.api_url}/entities/search",
+                json=query,
+                headers=await self._headers(),
+                params={
+                    "exclude_calculated_properties": "true",
+                    "include": ["blueprint", "identifier"],
+                },
+            )
+            search_req.raise_for_status()
+            return [
+                Entity.parse_obj(result) for result in search_req.json()["entities"]
+            ]
+
     async def search_dependent_entities(self, entity: Entity) -> List[Entity]:
         body = {
             "combinator": "and",
             "rules": [
                 {
                     "operator": "relatedTo",
                     "blueprint": entity.blueprint,
                     "value": entity.identifier,
-                    "required": "true",
                     "direction": "downstream",
                 }
             ],
         }
 
         logger.info(f"Search dependent entity with body {body}")
         async with httpx.AsyncClient() as client:
             response = await client.post(
-                f"{self.api_url}/v1/entities/search",
-                headers=await self.headers,
+                f"{self.api_url}/entities/search",
+                headers=await self._headers(),
                 json=body,
             )
         response.raise_for_status()
 
         return [Entity.parse_obj(result) for result in response.json()["entities"]]
 
     async def validate_entity_payload(
@@ -204,45 +251,51 @@
             },
         )
 
     async def get_integration(self, identifier: str) -> Dict[str, Any]:
         logger.info(f"Fetching integration with id: {identifier}")
         async with httpx.AsyncClient() as client:
             integration = await client.get(
-                f"{self.api_url}/integration/{identifier}", headers=await self.headers
+                f"{self.api_url}/integration/{identifier}",
+                headers=await self._headers(),
             )
         integration.raise_for_status()
         return integration.json()["integration"]
 
     async def initiate_integration(
         self, _id: str, _type: str, changelog_destination: ChangelogDestination
     ) -> None:
         logger.info(f"Initiating integration with id: {_id}")
         async with httpx.AsyncClient() as client:
             installation = await client.post(
                 f"{self.api_url}/integration",
-                headers=await self.headers,
+                headers=await self._headers(),
                 json={
                     "installationId": _id,
                     "installationAppType": _type,
                     "changelogDestination": changelog_destination,
                 },
             )
 
         if installation.status_code == 409:
             logger.info(
                 f"Integration with id: {_id} already exists, skipping registration"
             )
 
             return
 
+        if not installation.status_code >= 400:
+            logger.error(
+                f"Error initiating integration with id: {_id}, error: {installation.text}"
+            )
+
         installation.raise_for_status()
         logger.info(f"Integration with id: {_id} successfully registered")
 
     async def get_blueprint(self, identifier: str) -> Blueprint:
         logger.info(f"Fetching blueprint with id: {identifier}")
         async with httpx.AsyncClient() as client:
             response = await client.get(
-                f"{self.api_url}/v1/blueprints/{identifier}", headers=await self.headers
+                f"{self.api_url}/blueprints/{identifier}", headers=await self._headers()
             )
         response.raise_for_status()
         return Blueprint.parse_obj(response.json()["blueprint"])
```

### Comparing `port_ocean-0.1.0.dev0/port_ocean/clients/port/types.py` & `port_ocean-0.1.0.dev1/port_ocean/clients/port/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+from enum import Enum
 from typing import TypedDict, NotRequired
 
-Headers = TypedDict(
-    "Headers",
-    {
-        "Authorization": str,
-        "User-Agent": str,
-    },
-)
+
+class UserAgentType(Enum):
+    exporter = "exporter"
+    gitops = "gitops"
+
+
 KafkaCreds = TypedDict(
     "KafkaCreds",
     {
         "username": str,
         "password": str,
     },
 )
```

### Comparing `port_ocean-0.1.0.dev0/port_ocean/config/base.py` & `port_ocean-0.1.0.dev1/port_ocean/config/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     base_path: str
 
     class Config:
         secrets_dir = "./secrets.yml"
         yaml_file = "./config.yaml"
 
         @classmethod
-        def customise_sources(cls, init_settings, *_, **__):  # type: ignore
+        def customise_sources(cls, init_settings, env_settings, *_, **__):  # type: ignore
             return (
                 init_settings,
+                env_settings,
                 lambda s: yaml_config_settings_source(
                     s, init_settings.init_kwargs["base_path"]
                 ),
             )
```

### Comparing `port_ocean-0.1.0.dev0/port_ocean/consumers/kafka_consumer.py` & `port_ocean-0.1.0.dev1/port_ocean/consumers/kafka_consumer.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev0/port_ocean/context/integration.py` & `port_ocean-0.1.0.dev1/port_ocean/context/ocean.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 from dataclasses import dataclass
-from typing import Callable, TYPE_CHECKING
+from typing import Callable, TYPE_CHECKING, Any, Dict, List
 
 from fastapi import APIRouter
 from werkzeug.local import LocalProxy, LocalStack
 
 from port_ocean.clients.port.client import PortClient
+from port_ocean.clients.port.types import UserAgentType
 from port_ocean.config.integration import IntegrationConfiguration
+from port_ocean.core.models import Entity
 from port_ocean.errors import PortOceanContextNotFoundError
-from port_ocean.types import RESYNC_EVENT_LISTENER, START_EVENT_LISTENER, ObjectDiff
+from port_ocean.types import (
+    RESYNC_EVENT_LISTENER,
+    START_EVENT_LISTENER,
+    EntityRawDiff,
+)
 
 if TYPE_CHECKING:
     from port_ocean.core.integrations.base import BaseIntegration
     from port_ocean.port_ocean import Ocean
 
 
 @dataclass
@@ -27,42 +33,58 @@
         return self.app.integration_router
 
     @property
     def integration(self) -> "BaseIntegration":
         return self.app.integration
 
     @property
+    def integration_config(self) -> Dict[str, Any]:
+        return self.app.config.integration.config
+
+    @property
     def port_client(self) -> PortClient:
         return self.app.port_client
 
     def on_resync(
         self,
+        kind: str | None = None,
     ) -> Callable[[RESYNC_EVENT_LISTENER], RESYNC_EVENT_LISTENER]:
         def wrapper(function: RESYNC_EVENT_LISTENER) -> RESYNC_EVENT_LISTENER:
-            if self.integration:
-                return self.integration.on_resync(function)
-            else:
-                raise Exception("Integration not set")
+            return self.integration.on_resync(function, kind)
 
         return wrapper
 
     def on_start(self) -> Callable[[START_EVENT_LISTENER], START_EVENT_LISTENER]:
         def wrapper(function: START_EVENT_LISTENER) -> START_EVENT_LISTENER:
-            if self.integration:
-                return self.integration.on_start(function)
-            else:
-                raise Exception("Integration not set")
+            return self.integration.on_start(function)
 
         return wrapper
 
-    async def register_change(self, kind: str, change: ObjectDiff) -> None:
-        if self.integration:
-            await self.integration.register_state(kind, change)
-        else:
-            raise Exception("Integration not set")
+    async def register_raw(
+        self,
+        kind: str,
+        change: EntityRawDiff,
+        user_agent_type: UserAgentType = UserAgentType.exporter,
+    ) -> None:
+        await self.integration.register_raw(kind, change, user_agent_type)
+
+    async def register(
+        self,
+        entities: List[Entity],
+        user_agent_type: UserAgentType = UserAgentType.exporter,
+    ) -> None:
+        await self.integration.register(entities, user_agent_type)
+
+    async def sync(
+        self, entities: List[Entity], user_agent_type: UserAgentType
+    ) -> None:
+        await self.integration.sync(entities, user_agent_type)
+
+    async def trigger_resync(self) -> None:
+        await self.integration.trigger_resync(trigger_type="manual")
 
 
 _port_ocean_context_stack: LocalStack[PortOceanContext] = LocalStack()
 
 
 def initialize_port_ocean_context(ocean_app: "Ocean") -> None:
     """
```

### Comparing `port_ocean-0.1.0.dev0/port_ocean/core/handlers/port_app_config/models.py` & `port_ocean-0.1.0.dev1/port_ocean/core/handlers/port_app_config/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,27 @@
-from typing import List, Optional, Dict, TypeVar, Union, Generic
+from typing import List, Optional, Dict
 
 from pydantic import BaseModel, Field
 
 from port_ocean.clients.port.types import RequestOptions
 
 
 class EntityMapping(BaseModel):
     identifier: str
     title: str
     blueprint: str
     properties: Dict[str, str] = Field(default_factory=dict)
     relations: Dict[str, str] = Field(default_factory=dict)
 
 
-class BlueprintMapping(BaseModel):
-    identifier: str
-    title: str
-    properties: Dict[str, str] = Field(default_factory=dict)
-    relations: Dict[str, str] = Field(default_factory=dict)
-
-
-MappingType = TypeVar("MappingType", bound=Union[EntityMapping, BlueprintMapping])
-
-
 class PortResourceConfig(BaseModel):
-    class MappingsConfig(BaseModel, Generic[MappingType]):
-        mappings: MappingType
+    class MappingsConfig(BaseModel):
+        mappings: EntityMapping
 
-    entity: Optional[MappingsConfig[EntityMapping]]
-    blueprint: Optional[MappingsConfig[BlueprintMapping]]
+    entity: Optional[MappingsConfig]
 
 
 class ResourceConfig(BaseModel):
     class Selector(BaseModel):
         query: str
 
     kind: str
```

### Comparing `port_ocean-0.1.0.dev0/port_ocean/core/handlers/transport/port/get_required_entities.py` & `port_ocean-0.1.0.dev1/port_ocean/core/handlers/transport/port/get_required_entities.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     entity_to_blueprint: List[Tuple[Entity, Blueprint]],
     forbidden_entities: List[Entity],
     excluded_entities: List[Entity],
 ) -> List[Entity]:
     required_entities = []
     for entity, blueprint in entity_to_blueprint:
         for relation_name, relation in entity.relations.items():
-            relation_blueprint = blueprint.relations[relation_name]
+            relation_blueprint = blueprint.relations[relation_name].target
             target_entity = Entity(identifier=relation, blueprint=relation_blueprint)
 
             if any(is_same_entity(item, target_entity) for item in forbidden_entities):
                 raise Exception(
                     f"Cant delete entity {target_entity} of blueprint {target_entity.blueprint} "
                     f"because it was specified as relation target of entity {entity} "
                     f"of blueprint {entity.blueprint}"
```

### Comparing `port_ocean-0.1.0.dev0/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py` & `port_ocean-0.1.0.dev1/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev0/port_ocean/core/handlers/transport/port/transport.py` & `port_ocean-0.1.0.dev1/port_ocean/core/handlers/transport/port/transport.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,59 @@
 import asyncio
 from itertools import chain
 from typing import List
 
 from loguru import logger
 
+from port_ocean.clients.port.types import UserAgentType
 from port_ocean.context.event import event
 from port_ocean.core.handlers.manipulation.base import (
-    PortDiff,
-    PortObjectDiff,
-    flatten_diff,
+    EntityPortDiff,
 )
-from port_ocean.core.models import Entity, Blueprint
 from port_ocean.core.handlers.transport.base import BaseTransport
 from port_ocean.core.handlers.transport.port.order_by_entities_dependencies import (
     order_by_entities_dependencies,
 )
 from port_ocean.core.handlers.transport.port.validate_entity_relations import (
     validate_entity_relations,
 )
-from port_ocean.core.utils import is_same_entity, get_unique
+from port_ocean.core.models import Entity
+from port_ocean.core.utils import (
+    is_same_entity,
+    get_unique,
+    get_port_diff,
+)
+from port_ocean.types import EntityDiff
 
 
 class HttpPortTransport(BaseTransport):
-    async def _update_entity_diff(self, diff: PortObjectDiff[Entity]) -> None:
-        ordered_deleted_entities = order_by_entities_dependencies(diff.deleted)
-        for entity in ordered_deleted_entities:
-            await self.context.port_client.delete_entity(entity)
-
-        ordered_created_entities = reversed(
-            order_by_entities_dependencies(diff.created)
-        )
-        for entity in ordered_created_entities:
-            await self.context.port_client.upsert_entity(
-                entity, event.port_app_config.get_port_request_options()
-            )
-
-        ordered_modified_entities = reversed(
-            order_by_entities_dependencies(diff.modified)
-        )
-        for entity in ordered_modified_entities:
-            await self.context.port_client.upsert_entity(
-                entity, event.port_app_config.get_port_request_options()
-            )
-
-    async def _validate_delete_dependent_entities(
-        self, diff: PortObjectDiff[Entity]
-    ) -> None:
+    async def _validate_delete_dependent_entities(self, diff: EntityPortDiff) -> None:
         logger.info("Validated deleted entities")
         if not event.port_app_config.delete_dependent_entities:
             deps = await asyncio.gather(
                 *[
                     self.context.port_client.search_dependent_entities(entity)
                     for entity in diff.deleted
                 ]
             )
             new_dependent = get_unique(
                 [
                     entity
-                    for entity in chain(deps)
+                    for entity in chain.from_iterable(deps)
                     if not any([is_same_entity(item, entity) for item in diff.deleted])
-                ],
-                is_same_entity,
+                ]
             )
 
             if new_dependent:
                 raise Exception(
                     f"Must enable delete_dependent_entities flag or delete also dependent entities:"
                     f" {[(dep.blueprint, dep.identifier) for dep in new_dependent]}"
                 )
 
-    async def _validate_entity_diff(self, diff: PortObjectDiff[Entity]) -> None:
+    async def _validate_entity_diff(self, diff: EntityPortDiff) -> None:
         config = event.port_app_config
         await self._validate_delete_dependent_entities(diff)
         modified_or_created_entities = diff.modified + diff.created
         logger.info("Validating modified or created entities")
 
         await asyncio.gather(
             *[
@@ -85,18 +65,63 @@
                     },
                 )
                 for entity in modified_or_created_entities
             ]
         )
         await validate_entity_relations(diff, self.context.port_client)
 
-    async def update_diff(self, changes: List[PortDiff]) -> None:
-        blueprints: PortObjectDiff[Blueprint] = flatten_diff(
-            [change[1] for change in changes]
+    async def update_diff(
+        self,
+        entities: EntityDiff,
+        user_agent_type: UserAgentType | None = None,
+    ) -> None:
+        entities_diff = get_port_diff(entities["before"], entities["after"])
+
+        logger.info(
+            f"Registering entity diff (created: {len(entities_diff.created)}, deleted: {len(entities_diff.deleted)}, modified: {len(entities_diff.modified)})"
         )
-        # ToDo: update blueprint diff
+        await self._validate_entity_diff(entities_diff)
+
+        user_agent_type = user_agent_type or self.DEFAULT_USER_AGENT_TYPE
+        await self.delete(entities_diff.deleted, user_agent_type)
+        await self.upsert(entities_diff.created, user_agent_type)
+        await self.upsert(entities_diff.modified, user_agent_type)
 
-        entities: PortObjectDiff[Entity] = flatten_diff(
-            [change[0] for change in changes]
+    async def upsert(
+        self, entities: List[Entity], user_agent_type: UserAgentType
+    ) -> None:
+        ordered_created_entities = reversed(order_by_entities_dependencies(entities))
+        for entity in ordered_created_entities:
+            await self.context.port_client.upsert_entity(
+                entity,
+                event.port_app_config.get_port_request_options(),
+                user_agent_type,
+            )
+
+    async def delete(
+        self, entities: List[Entity], user_agent_type: UserAgentType
+    ) -> None:
+        ordered_deleted_entities = order_by_entities_dependencies(entities)
+
+        await asyncio.gather(
+            *[
+                self.context.port_client.delete_entity(entity, user_agent_type)
+                for entity in ordered_deleted_entities
+            ]
+        )
+
+    async def delete_diff(
+        self, entities: List[Entity], user_agent_type: UserAgentType
+    ) -> None:
+        entities_at_port = await self.context.port_client.search_entities(
+            user_agent_type
+        )
+        diff = get_port_diff(entities_at_port, entities)
+
+        ordered_deleted_entities = order_by_entities_dependencies(diff.deleted)
+
+        await asyncio.gather(
+            *[
+                self.context.port_client.delete_entity(entity, user_agent_type)
+                for entity in ordered_deleted_entities
+            ]
         )
-        await self._validate_entity_diff(entities)
-        await self._update_entity_diff(entities)
```

### Comparing `port_ocean-0.1.0.dev0/port_ocean/core/handlers/transport/port/validate_entity_relations.py` & `port_ocean-0.1.0.dev1/port_ocean/core/handlers/transport/port/validate_entity_relations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import asyncio
 from itertools import groupby
 
 from port_ocean.clients.port.client import PortClient
-from port_ocean.core.handlers.manipulation.base import PortObjectDiff
-from port_ocean.core.models import Entity
+from port_ocean.core.handlers.manipulation.base import EntityPortDiff
 from port_ocean.core.handlers.transport.port.get_required_entities import (
     get_required_entities,
 )
 
 
 async def validate_entity_relations(
-    diff: PortObjectDiff[Entity], port_client: PortClient
+    diff: EntityPortDiff, port_client: PortClient
 ) -> None:
     modified_or_created_entities = diff.modified + diff.created
     entities_with_relations = [
         entity for entity in modified_or_created_entities if entity.relations
     ]
     blueprint_identifier_to_entity = dict(
         groupby(
```

### Comparing `port_ocean-0.1.0.dev0/port_ocean/core/trigger_channel/kafka_trigger_channel.py` & `port_ocean-0.1.0.dev1/port_ocean/core/trigger_channel/kafka_trigger_channel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import threading
 from typing import Dict, Any, Callable
 
 from port_ocean.consumers.kafka_consumer import KafkaConsumer, KafkaConsumerConfig
-from port_ocean.context.integration import (
+from port_ocean.context.ocean import (
     PortOceanContext,
     initialize_port_ocean_context,
     ocean,
 )
 from port_ocean.core.trigger_channel.base_trigger_channel import (
     BaseTriggerChannel,
     TriggerEventEvents,
```

### Comparing `port_ocean-0.1.0.dev0/port_ocean/core/trigger_channel/trigger_channel_factory.py` & `port_ocean-0.1.0.dev1/port_ocean/core/trigger_channel/trigger_channel_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from port_ocean.core.base import BaseWithContext
 from port_ocean.core.trigger_channel.base_trigger_channel import (
     BaseTriggerChannel,
     TriggerEventEvents,
 )
 from port_ocean.core.trigger_channel.kafka_trigger_channel import KafkaTriggerChannel
 
-from port_ocean.context.integration import PortOceanContext
+from port_ocean.context.ocean import PortOceanContext
 
 
 class TriggerChannelFactory(BaseWithContext):
     def __init__(
         self,
         context: PortOceanContext,
         installation_id: str,
@@ -36,15 +36,18 @@
             if integration_identifier == self.installation_id:
                 await callback(event)
 
         return wrapper
 
     async def create_trigger_channel(self) -> None:
         if self.trigger_channel_type.lower() == "kafka":
-            kafka_creds = await self.context.port_client.get_kafka_creds()
+            kafka_creds = {
+                "username": "",
+                "password": "",
+            }  # await self.context.port_client.get_kafka_creds()
             org_id = await self.context.port_client.get_org_id()
             self._trigger_channel = KafkaTriggerChannel(
                 {
                     "on_resync": self.on_event(self.events["on_resync"]),
                     "on_action": self.on_event(self.events["on_action"]),
                 },
                 KafkaConsumerConfig(
```

### Comparing `port_ocean-0.1.0.dev0/port_ocean/logging.py` & `port_ocean-0.1.0.dev1/port_ocean/logging.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev0/pyproject.toml` & `port_ocean-0.1.0.dev1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "port-ocean"
-version = "0.1.0.dev0"
+version = "0.1.0.dev1"
 description = "Port Ocean is a CLI tool for managing your Port projects."
 readme = "README.md"
 authors = ["Daniel Sinai <daniel@getport.io>", "Yair Siman-Tov <yair@getport.io>"]
 packages = [
     { include = "port_ocean", from = "." }
 ]
 
@@ -20,25 +20,24 @@
 pydantic = "^1.10.8"
 requests = "^2.31.0"
 loguru = "^0.7.0"
 pyyaml = "^6.0"
 werkzeug = "^2.3.4"
 fastapi = "^0.96.0"
 uvicorn = "^0.22.0"
+confluent-kafka = "^2.1.1"
+httpx = "^0.24.1"
+pyjq = "^2.6.0"
 urllib3 = "^1.26.16"
 six = "^1.16.0"
 
 # CLI
 click = { version = "^8.1.3", optional = true }
 rich = { version = "^13.4.1", optional = true }
 cookiecutter = { version = "^2.1.1", optional = true }
-confluent-kafka = "^2.1.1"
-pyjq = "^2.6.0"
-httpx = "^0.24.1"
-nest-asyncio = "^1.5.6"
 
 [tool.poetry.extras]
 cli = ["click", "rich", "cookiecutter"]
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2"
```

### Comparing `port_ocean-0.1.0.dev0/PKG-INFO` & `port_ocean-0.1.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: port-ocean
-Version: 0.1.0.dev0
+Version: 0.1.0.dev1
 Summary: Port Ocean is a CLI tool for managing your Port projects.
 Author: Daniel Sinai
 Author-email: daniel@getport.io
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cli
 Requires-Dist: click (>=8.1.3,<9.0.0) ; extra == "cli"
 Requires-Dist: confluent-kafka (>=2.1.1,<3.0.0)
 Requires-Dist: cookiecutter (>=2.1.1,<3.0.0) ; extra == "cli"
 Requires-Dist: fastapi (>=0.96.0,<0.97.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
-Requires-Dist: nest-asyncio (>=1.5.6,<2.0.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: pyjq (>=2.6.0,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.4.1,<14.0.0) ; extra == "cli"
 Requires-Dist: six (>=1.16.0,<2.0.0)
 Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
```

