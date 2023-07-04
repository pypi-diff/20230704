# Comparing `tmp/port_ocean-0.1.0.dev5.tar.gz` & `tmp/port_ocean-0.1.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_ocean-0.1.0.dev5.tar", max compression
+gzip compressed data, was "port_ocean-0.1.0.dev6.tar", max compression
```

## Comparing `port_ocean-0.1.0.dev5.tar` & `port_ocean-0.1.0.dev6.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     4418 2023-07-04 13:21:06.764844 port_ocean-0.1.0.dev5/README.md
--rw-r--r--   0        0        0      537 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/__init__.py
--rw-r--r--   0        0        0      121 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/cli.py
--rw-r--r--   0        0        0     5085 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/commands.py
--rw-r--r--   0        0        0      429 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/cookiecutter.json
--rw-r--r--   0        0        0       54 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
--rw-r--r--   0        0        0     2832 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
--rw-r--r--   0        0        0      449 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
--rw-r--r--   0        0        0     1718 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
--rw-r--r--   0        0        0      406 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
--rw-r--r--   0        0        0      392 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
--rw-r--r--   0        0        0       46 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
--rw-r--r--   0        0        0     1184 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
--rw-r--r--   0        0        0     1334 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/cli/download_git_folder.py
--rw-r--r--   0        0        0      766 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/cli/list_integrations.py
--rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/clients/port/__init__.py
--rw-r--r--   0        0        0     2593 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/clients/port/authentication.py
--rw-r--r--   0        0        0     2803 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/clients/port/client.py
--rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/clients/port/mixins/__init__.py
--rw-r--r--   0        0        0     6097 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/clients/port/mixins/entities.py
--rw-r--r--   0        0        0     3029 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/clients/port/mixins/integrations.py
--rw-r--r--   0        0        0      593 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/clients/port/types.py
--rw-r--r--   0        0        0      142 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/clients/port/utils.py
--rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/config/__init__.py
--rw-r--r--   0        0        0     2463 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/config/base.py
--rw-r--r--   0        0        0      997 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/config/integration.py
--rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/consumers/__init__.py
--rw-r--r--   0        0        0      125 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/consumers/base_consumer.py
--rw-r--r--   0        0        0     3991 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/consumers/kafka_consumer.py
--rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/context/__init__.py
--rw-r--r--   0        0        0     3119 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/context/event.py
--rw-r--r--   0        0        0     4032 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/context/ocean.py
--rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/__init__.py
--rw-r--r--   0        0        0      219 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/base.py
--rw-r--r--   0        0        0      300 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/manipulation/__init__.py
--rw-r--r--   0        0        0      946 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/manipulation/base.py
--rw-r--r--   0        0        0     2674 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/manipulation/jq_manipulation.py
--rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/port_app_config/__init__.py
--rw-r--r--   0        0        0      452 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/port_app_config/api.py
--rw-r--r--   0        0        0      651 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/port_app_config/base.py
--rw-r--r--   0        0        0     1432 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/port_app_config/models.py
--rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/transport/__init__.py
--rw-r--r--   0        0        0      852 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/transport/base.py
--rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/transport/port/__init__.py
--rw-r--r--   0        0        0     1339 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/transport/port/get_related_entities.py
--rw-r--r--   0        0        0     1043 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py
--rw-r--r--   0        0        0     7619 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/transport/port/transport.py
--rw-r--r--   0        0        0     1375 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/transport/port/validate_entity_relations.py
--rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/integrations/__init__.py
--rw-r--r--   0        0        0     2085 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/integrations/base.py
--rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/integrations/mixins/__init__.py
--rw-r--r--   0        0        0      692 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/integrations/mixins/events.py
--rw-r--r--   0        0        0     2557 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/integrations/mixins/handler.py
--rw-r--r--   0        0        0     9868 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/integrations/mixins/sync.py
--rw-r--r--   0        0        0      588 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/models.py
--rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/trigger_channel/__init__.py
--rw-r--r--   0        0        0      448 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/trigger_channel/base.py
--rw-r--r--   0        0        0     2962 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/trigger_channel/factory.py
--rw-r--r--   0        0        0      898 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/trigger_channel/http.py
--rw-r--r--   0        0        0     3568 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/trigger_channel/kafka.py
--rw-r--r--   0        0        0      909 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/trigger_channel/settings.py
--rw-r--r--   0        0        0      563 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/types.py
--rw-r--r--   0        0        0     2044 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/utils.py
--rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/exceptions/__init__.py
--rw-r--r--   0        0        0      426 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/exceptions/api.py
--rw-r--r--   0        0        0       46 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/exceptions/base.py
--rw-r--r--   0        0        0      180 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/exceptions/clients.py
--rw-r--r--   0        0        0      235 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/exceptions/context.py
--rw-r--r--   0        0        0      473 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/exceptions/core.py
--rw-r--r--   0        0        0      756 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/logger_setup.py
--rw-r--r--   0        0        0     2434 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/middlewares.py
--rw-r--r--   0        0        0     4376 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/ocean.py
--rw-r--r--   0        0        0      765 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/utils.py
--rw-r--r--   0        0        0     2041 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/pyproject.toml
--rw-r--r--   0        0        0     5503 1970-01-01 00:00:00.000000 port_ocean-0.1.0.dev5/PKG-INFO
+-rw-r--r--   0        0        0     4418 2023-07-04 14:14:33.384030 port_ocean-0.1.0.dev6/README.md
+-rw-r--r--   0        0        0      537 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/cli/__init__.py
+-rw-r--r--   0        0        0      121 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/cli/cli.py
+-rw-r--r--   0        0        0     5085 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/cli/commands.py
+-rw-r--r--   0        0        0      429 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/cli/cookiecutter/cookiecutter.json
+-rw-r--r--   0        0        0       54 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
+-rw-r--r--   0        0        0     2832 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
+-rw-r--r--   0        0        0      449 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
+-rw-r--r--   0        0        0     1718 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
+-rw-r--r--   0        0        0      406 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
+-rw-r--r--   0        0        0      392 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
+-rw-r--r--   0        0        0       46 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
+-rw-r--r--   0        0        0     1184 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0     1334 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/cli/download_git_folder.py
+-rw-r--r--   0        0        0      766 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/cli/list_integrations.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/clients/port/__init__.py
+-rw-r--r--   0        0        0     2593 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/clients/port/authentication.py
+-rw-r--r--   0        0        0     2803 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/clients/port/client.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/clients/port/mixins/__init__.py
+-rw-r--r--   0        0        0     6097 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/clients/port/mixins/entities.py
+-rw-r--r--   0        0        0     3029 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/clients/port/mixins/integrations.py
+-rw-r--r--   0        0        0      593 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/clients/port/types.py
+-rw-r--r--   0        0        0      142 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/clients/port/utils.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/config/__init__.py
+-rw-r--r--   0        0        0     2463 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/config/base.py
+-rw-r--r--   0        0        0      997 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/config/integration.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/consumers/__init__.py
+-rw-r--r--   0        0        0      125 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/consumers/base_consumer.py
+-rw-r--r--   0        0        0     3991 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/consumers/kafka_consumer.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/context/__init__.py
+-rw-r--r--   0        0        0     3119 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/context/event.py
+-rw-r--r--   0        0        0     4032 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/context/ocean.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/core/__init__.py
+-rw-r--r--   0        0        0      219 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/core/base.py
+-rw-r--r--   0        0        0      300 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/core/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/core/handlers/manipulation/__init__.py
+-rw-r--r--   0        0        0      946 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/core/handlers/manipulation/base.py
+-rw-r--r--   0        0        0     2674 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/core/handlers/manipulation/jq_manipulation.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/core/handlers/port_app_config/__init__.py
+-rw-r--r--   0        0        0      452 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/core/handlers/port_app_config/api.py
+-rw-r--r--   0        0        0      651 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/core/handlers/port_app_config/base.py
+-rw-r--r--   0        0        0     1432 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/core/handlers/port_app_config/models.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/core/handlers/transport/__init__.py
+-rw-r--r--   0        0        0      852 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/core/handlers/transport/base.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/core/handlers/transport/port/__init__.py
+-rw-r--r--   0        0        0     1339 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/core/handlers/transport/port/get_related_entities.py
+-rw-r--r--   0        0        0     1043 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py
+-rw-r--r--   0        0        0     7619 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/core/handlers/transport/port/transport.py
+-rw-r--r--   0        0        0     1375 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/core/handlers/transport/port/validate_entity_relations.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/core/integrations/__init__.py
+-rw-r--r--   0        0        0     2085 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/core/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:14:33.420031 port_ocean-0.1.0.dev6/port_ocean/core/integrations/mixins/__init__.py
+-rw-r--r--   0        0        0      692 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/port_ocean/core/integrations/mixins/events.py
+-rw-r--r--   0        0        0     2557 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/port_ocean/core/integrations/mixins/handler.py
+-rw-r--r--   0        0        0     9868 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/port_ocean/core/integrations/mixins/sync.py
+-rw-r--r--   0        0        0      588 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/port_ocean/core/models.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/port_ocean/core/trigger_channel/__init__.py
+-rw-r--r--   0        0        0      448 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/port_ocean/core/trigger_channel/base.py
+-rw-r--r--   0        0        0     2962 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/port_ocean/core/trigger_channel/factory.py
+-rw-r--r--   0        0        0      898 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/port_ocean/core/trigger_channel/http.py
+-rw-r--r--   0        0        0     3568 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/port_ocean/core/trigger_channel/kafka.py
+-rw-r--r--   0        0        0      909 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/port_ocean/core/trigger_channel/settings.py
+-rw-r--r--   0        0        0      563 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/port_ocean/core/types.py
+-rw-r--r--   0        0        0     2044 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/port_ocean/core/utils.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/port_ocean/exceptions/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/port_ocean/exceptions/api.py
+-rw-r--r--   0        0        0       46 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/port_ocean/exceptions/base.py
+-rw-r--r--   0        0        0      180 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/port_ocean/exceptions/clients.py
+-rw-r--r--   0        0        0      235 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/port_ocean/exceptions/context.py
+-rw-r--r--   0        0        0      473 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/port_ocean/exceptions/core.py
+-rw-r--r--   0        0        0      756 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/port_ocean/logger_setup.py
+-rw-r--r--   0        0        0     2434 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/port_ocean/middlewares.py
+-rw-r--r--   0        0        0     4376 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/port_ocean/ocean.py
+-rw-r--r--   0        0        0      765 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/port_ocean/utils.py
+-rw-r--r--   0        0        0     2041 2023-07-04 14:14:33.424031 port_ocean-0.1.0.dev6/pyproject.toml
+-rw-r--r--   0        0        0     5503 1970-01-01 00:00:00.000000 port_ocean-0.1.0.dev6/PKG-INFO
```

### Comparing `port_ocean-0.1.0.dev5/README.md` & `port_ocean-0.1.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/__init__.py` & `port_ocean-0.1.0.dev6/port_ocean/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/cli/commands.py` & `port_ocean-0.1.0.dev6/port_ocean/cli/commands.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore` & `port_ocean-0.1.0.dev6/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile` & `port_ocean-0.1.0.dev6/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml` & `port_ocean-0.1.0.dev6/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/cli/download_git_folder.py` & `port_ocean-0.1.0.dev6/port_ocean/cli/download_git_folder.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/cli/list_integrations.py` & `port_ocean-0.1.0.dev6/port_ocean/cli/list_integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/clients/port/authentication.py` & `port_ocean-0.1.0.dev6/port_ocean/clients/port/authentication.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/clients/port/client.py` & `port_ocean-0.1.0.dev6/port_ocean/clients/port/client.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/clients/port/mixins/entities.py` & `port_ocean-0.1.0.dev6/port_ocean/clients/port/mixins/entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/clients/port/mixins/integrations.py` & `port_ocean-0.1.0.dev6/port_ocean/clients/port/mixins/integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/clients/port/types.py` & `port_ocean-0.1.0.dev6/port_ocean/clients/port/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/config/base.py` & `port_ocean-0.1.0.dev6/port_ocean/config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/config/integration.py` & `port_ocean-0.1.0.dev6/port_ocean/config/integration.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/consumers/kafka_consumer.py` & `port_ocean-0.1.0.dev6/port_ocean/consumers/kafka_consumer.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/context/event.py` & `port_ocean-0.1.0.dev6/port_ocean/context/event.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/context/ocean.py` & `port_ocean-0.1.0.dev6/port_ocean/context/ocean.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/core/handlers/manipulation/base.py` & `port_ocean-0.1.0.dev6/port_ocean/core/handlers/manipulation/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/core/handlers/manipulation/jq_manipulation.py` & `port_ocean-0.1.0.dev6/port_ocean/core/handlers/manipulation/jq_manipulation.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/core/handlers/port_app_config/base.py` & `port_ocean-0.1.0.dev6/port_ocean/core/handlers/port_app_config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/core/handlers/port_app_config/models.py` & `port_ocean-0.1.0.dev6/port_ocean/core/handlers/port_app_config/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/core/handlers/transport/base.py` & `port_ocean-0.1.0.dev6/port_ocean/core/handlers/transport/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/core/handlers/transport/port/get_related_entities.py` & `port_ocean-0.1.0.dev6/port_ocean/core/handlers/transport/port/get_related_entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py` & `port_ocean-0.1.0.dev6/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/core/handlers/transport/port/transport.py` & `port_ocean-0.1.0.dev6/port_ocean/core/handlers/transport/port/transport.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/core/handlers/transport/port/validate_entity_relations.py` & `port_ocean-0.1.0.dev6/port_ocean/core/handlers/transport/port/validate_entity_relations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/core/integrations/base.py` & `port_ocean-0.1.0.dev6/port_ocean/core/integrations/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/core/integrations/mixins/events.py` & `port_ocean-0.1.0.dev6/port_ocean/core/integrations/mixins/events.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/core/integrations/mixins/handler.py` & `port_ocean-0.1.0.dev6/port_ocean/core/integrations/mixins/handler.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/core/integrations/mixins/sync.py` & `port_ocean-0.1.0.dev6/port_ocean/core/integrations/mixins/sync.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/core/models.py` & `port_ocean-0.1.0.dev6/port_ocean/core/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/core/trigger_channel/factory.py` & `port_ocean-0.1.0.dev6/port_ocean/core/trigger_channel/factory.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/core/trigger_channel/http.py` & `port_ocean-0.1.0.dev6/port_ocean/core/trigger_channel/http.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/core/trigger_channel/kafka.py` & `port_ocean-0.1.0.dev6/port_ocean/core/trigger_channel/kafka.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/core/trigger_channel/settings.py` & `port_ocean-0.1.0.dev6/port_ocean/core/trigger_channel/settings.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/core/types.py` & `port_ocean-0.1.0.dev6/port_ocean/core/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/core/utils.py` & `port_ocean-0.1.0.dev6/port_ocean/core/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/logger_setup.py` & `port_ocean-0.1.0.dev6/port_ocean/logger_setup.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/middlewares.py` & `port_ocean-0.1.0.dev6/port_ocean/middlewares.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/ocean.py` & `port_ocean-0.1.0.dev6/port_ocean/ocean.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/port_ocean/utils.py` & `port_ocean-0.1.0.dev6/port_ocean/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev5/pyproject.toml` & `port_ocean-0.1.0.dev6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "port-ocean"
-version = "0.1.0.dev5"
+version = "0.1.0.dev6"
 description = "Port Ocean is a CLI tool for managing your Port projects."
 readme = "README.md"
 authors = ["Daniel Sinai <daniel@getport.io>", "Yair Siman-Tov <yair@getport.io>"]
 packages = [
     { include = "port_ocean", from = "." }
 ]
```

### Comparing `port_ocean-0.1.0.dev5/PKG-INFO` & `port_ocean-0.1.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-ocean
-Version: 0.1.0.dev5
+Version: 0.1.0.dev6
 Summary: Port Ocean is a CLI tool for managing your Port projects.
 Author: Daniel Sinai
 Author-email: daniel@getport.io
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cli
```

