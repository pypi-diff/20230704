# Comparing `tmp/port_ocean-0.1.0.dev4.tar.gz` & `tmp/port_ocean-0.1.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_ocean-0.1.0.dev4.tar", max compression
+gzip compressed data, was "port_ocean-0.1.0.dev5.tar", max compression
```

## Comparing `port_ocean-0.1.0.dev4.tar` & `port_ocean-0.1.0.dev5.tar`

### file list

```diff
@@ -1,73 +1,79 @@
--rw-r--r--   0        0        0     4337 2023-07-02 12:33:49.649332 port_ocean-0.1.0.dev4/README.md
--rw-r--r--   0        0        0      440 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/__init__.py
--rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/__init__.py
--rw-r--r--   0        0        0      121 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/cli.py
--rw-r--r--   0        0        0     3380 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/commands.py
--rw-r--r--   0        0        0      429 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/cookiecutter/cookiecutter.json
--rw-r--r--   0        0        0       54 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
--rw-r--r--   0        0        0      449 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
--rw-r--r--   0        0        0     1718 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
--rw-r--r--   0        0        0      406 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
--rw-r--r--   0        0        0      392 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
--rw-r--r--   0        0        0       46 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
--rw-r--r--   0        0        0     1184 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
--rw-r--r--   0        0        0     1334 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/download_git_folder.py
--rw-r--r--   0        0        0      766 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/list_integrations.py
--rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/clients/port/__init__.py
--rw-r--r--   0        0        0    11337 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/clients/port/client.py
--rw-r--r--   0        0        0      593 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/clients/port/types.py
--rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/config/__init__.py
--rw-r--r--   0        0        0     2592 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/config/base.py
--rw-r--r--   0        0        0     1035 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/config/integration.py
--rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/consumers/__init__.py
--rw-r--r--   0        0        0      125 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/consumers/base_consumer.py
--rw-r--r--   0        0        0     3821 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/consumers/kafka_consumer.py
--rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/context/__init__.py
--rw-r--r--   0        0        0     3234 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/context/event.py
--rw-r--r--   0        0        0     4012 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/context/ocean.py
--rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/__init__.py
--rw-r--r--   0        0        0      219 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/base.py
--rw-r--r--   0        0        0      300 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/manipulation/__init__.py
--rw-r--r--   0        0        0      690 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/manipulation/base.py
--rw-r--r--   0        0        0     2629 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/manipulation/jq_manipulation.py
--rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/port_app_config/__init__.py
--rw-r--r--   0        0        0      452 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/port_app_config/api.py
--rw-r--r--   0        0        0      651 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/port_app_config/base.py
--rw-r--r--   0        0        0     1432 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/port_app_config/models.py
--rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/transport/__init__.py
--rw-r--r--   0        0        0      914 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/transport/base.py
--rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/transport/port/__init__.py
--rw-r--r--   0        0        0     1258 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/transport/port/get_required_entities.py
--rw-r--r--   0        0        0     1043 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py
--rw-r--r--   0        0        0     5115 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/transport/port/transport.py
--rw-r--r--   0        0        0     1495 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/transport/port/validate_entity_relations.py
--rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/integrations/__init__.py
--rw-r--r--   0        0        0     3734 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/integrations/base.py
--rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/integrations/mixins/__init__.py
--rw-r--r--   0        0        0      692 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/integrations/mixins/events.py
--rw-r--r--   0        0        0     2556 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/integrations/mixins/handler.py
--rw-r--r--   0        0        0     7748 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/integrations/mixins/sync.py
--rw-r--r--   0        0        0      588 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/models.py
--rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/trigger_channel/__init__.py
--rw-r--r--   0        0        0      448 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/trigger_channel/base.py
--rw-r--r--   0        0        0     2840 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/trigger_channel/factory.py
--rw-r--r--   0        0        0      898 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/trigger_channel/http.py
--rw-r--r--   0        0        0     3303 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/trigger_channel/kafka.py
--rw-r--r--   0        0        0      909 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/trigger_channel/settings.py
--rw-r--r--   0        0        0      563 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/types.py
--rw-r--r--   0        0        0     2044 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/port_ocean/core/utils.py
--rw-r--r--   0        0        0      166 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/port_ocean/errors.py
--rw-r--r--   0        0        0        0 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/port_ocean/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/port_ocean/exceptions/api/__init__.py
--rw-r--r--   0        0        0      426 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/port_ocean/exceptions/api/base.py
--rw-r--r--   0        0        0      461 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/port_ocean/exceptions/base.py
--rw-r--r--   0        0        0      180 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/port_ocean/exceptions/clients.py
--rw-r--r--   0        0        0      626 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/port_ocean/logger_setup.py
--rw-r--r--   0        0        0     2429 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/port_ocean/middlewares.py
--rw-r--r--   0        0        0     4246 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/port_ocean/ocean.py
--rw-r--r--   0        0        0      765 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/port_ocean/utils.py
--rw-r--r--   0        0        0     1938 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/pyproject.toml
--rw-r--r--   0        0        0     5366 1970-01-01 00:00:00.000000 port_ocean-0.1.0.dev4/PKG-INFO
+-rw-r--r--   0        0        0     4418 2023-07-04 13:21:06.764844 port_ocean-0.1.0.dev5/README.md
+-rw-r--r--   0        0        0      537 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/__init__.py
+-rw-r--r--   0        0        0      121 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/cli.py
+-rw-r--r--   0        0        0     5085 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/commands.py
+-rw-r--r--   0        0        0      429 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/cookiecutter.json
+-rw-r--r--   0        0        0       54 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
+-rw-r--r--   0        0        0     2832 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
+-rw-r--r--   0        0        0      449 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
+-rw-r--r--   0        0        0     1718 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
+-rw-r--r--   0        0        0      406 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
+-rw-r--r--   0        0        0      392 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
+-rw-r--r--   0        0        0       46 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
+-rw-r--r--   0        0        0     1184 2023-07-04 13:21:06.804844 port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0     1334 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/cli/download_git_folder.py
+-rw-r--r--   0        0        0      766 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/cli/list_integrations.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/clients/port/__init__.py
+-rw-r--r--   0        0        0     2593 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/clients/port/authentication.py
+-rw-r--r--   0        0        0     2803 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/clients/port/client.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/clients/port/mixins/__init__.py
+-rw-r--r--   0        0        0     6097 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/clients/port/mixins/entities.py
+-rw-r--r--   0        0        0     3029 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/clients/port/mixins/integrations.py
+-rw-r--r--   0        0        0      593 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/clients/port/types.py
+-rw-r--r--   0        0        0      142 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/clients/port/utils.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/config/__init__.py
+-rw-r--r--   0        0        0     2463 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/config/base.py
+-rw-r--r--   0        0        0      997 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/config/integration.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/consumers/__init__.py
+-rw-r--r--   0        0        0      125 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/consumers/base_consumer.py
+-rw-r--r--   0        0        0     3991 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/consumers/kafka_consumer.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/context/__init__.py
+-rw-r--r--   0        0        0     3119 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/context/event.py
+-rw-r--r--   0        0        0     4032 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/context/ocean.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/__init__.py
+-rw-r--r--   0        0        0      219 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/base.py
+-rw-r--r--   0        0        0      300 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/manipulation/__init__.py
+-rw-r--r--   0        0        0      946 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/manipulation/base.py
+-rw-r--r--   0        0        0     2674 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/manipulation/jq_manipulation.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/port_app_config/__init__.py
+-rw-r--r--   0        0        0      452 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/port_app_config/api.py
+-rw-r--r--   0        0        0      651 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/port_app_config/base.py
+-rw-r--r--   0        0        0     1432 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/port_app_config/models.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/transport/__init__.py
+-rw-r--r--   0        0        0      852 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/transport/base.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/transport/port/__init__.py
+-rw-r--r--   0        0        0     1339 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/transport/port/get_related_entities.py
+-rw-r--r--   0        0        0     1043 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py
+-rw-r--r--   0        0        0     7619 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/transport/port/transport.py
+-rw-r--r--   0        0        0     1375 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/handlers/transport/port/validate_entity_relations.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/integrations/__init__.py
+-rw-r--r--   0        0        0     2085 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/integrations/mixins/__init__.py
+-rw-r--r--   0        0        0      692 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/integrations/mixins/events.py
+-rw-r--r--   0        0        0     2557 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/integrations/mixins/handler.py
+-rw-r--r--   0        0        0     9868 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/integrations/mixins/sync.py
+-rw-r--r--   0        0        0      588 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/models.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/trigger_channel/__init__.py
+-rw-r--r--   0        0        0      448 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/trigger_channel/base.py
+-rw-r--r--   0        0        0     2962 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/trigger_channel/factory.py
+-rw-r--r--   0        0        0      898 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/trigger_channel/http.py
+-rw-r--r--   0        0        0     3568 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/trigger_channel/kafka.py
+-rw-r--r--   0        0        0      909 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/trigger_channel/settings.py
+-rw-r--r--   0        0        0      563 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/types.py
+-rw-r--r--   0        0        0     2044 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/core/utils.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/exceptions/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/exceptions/api.py
+-rw-r--r--   0        0        0       46 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/exceptions/base.py
+-rw-r--r--   0        0        0      180 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/exceptions/clients.py
+-rw-r--r--   0        0        0      235 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/exceptions/context.py
+-rw-r--r--   0        0        0      473 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/exceptions/core.py
+-rw-r--r--   0        0        0      756 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/logger_setup.py
+-rw-r--r--   0        0        0     2434 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/middlewares.py
+-rw-r--r--   0        0        0     4376 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/ocean.py
+-rw-r--r--   0        0        0      765 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/port_ocean/utils.py
+-rw-r--r--   0        0        0     2041 2023-07-04 13:21:06.808845 port_ocean-0.1.0.dev5/pyproject.toml
+-rw-r--r--   0        0        0     5503 1970-01-01 00:00:00.000000 port_ocean-0.1.0.dev5/PKG-INFO
```

### Comparing `port_ocean-0.1.0.dev4/README.md` & `port_ocean-0.1.0.dev5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,117 @@
-<img align="right" width="100" height="74" src="https://user-images.githubusercontent.com/8277210/183290025-d7b24277-dfb4-4ce1-bece-7fe0ecd5efd4.svg" />
+# Ocean <img src="./assets/OceanSymbol.svg" alt="Ocean" width="100" height="100" align="right">
 
-# Ocean
 [![Lint](https://github.com/port-labs/port-ocean/actions/workflows/lint.yml/badge.svg)](https://github.com/port-labs/port-ocean/actions/workflows/lint.yml)
 
-Ocean is a solution developed by Port to address the challenges faced while integrating various third-party systems with our developer portal product. This framework provides a standardized approach for implementing integrations, simplifying the process and allowing platform engineers to focus on the core functionality of the third-party system.
+Ocean is a solution created by Port to tackle the difficulties encountered when merging different third-party systems with our developer portal product. This framework offers a uniform method for executing integrations, streamlining the process and enabling platform engineers to prioritize the essential features of the third-party system.
+
+
+
+## Prerequisites
+
+- Python 3.11
+
+
 
 ## Installation
-`pip install port-ocean[cli]` or `poetry add port-ocean[cli]`
+```
+pip install port-ocean[cli]
+```
+
+Or
+
+```sh
+poetry add port-ocean[cli]
+```
+
+[]()
 
 ## Run Integration
-1. source the integration venv `. .venv/bin/activate`
-2. `ocean sail ./path/to/integration`
+
+1. source the integration venv 
+
+   ```sh
+   . .venv/bin/activate
+   ```
+
+2. Run
+
+   ```sh
+   ocean sail ./path/to/integration
+   ```
+
+   
 
 ## Local Development (Framework)
 1. Clone the repository
-2. Install dependencies: `make install` or `make install/all` for installing integrations dependencies as well
-3. source the integration venv `. .venv/bin/activate`
+
+2. Install dependencies:
+
+   ```sh
+   make install
+   ```
+
+   Or (For installing integrations dependencies as well)
+
+   ```sh
+   make install/all
+   ```
+
+3. source the integration venv
+
+   ```sh
+   . .venv/bin/activate
+   ```
+
+   
 
 
 ## Local Development (Integration)
 1. Clone the repository
-2. For new integration run `make new` and follow the instructions
-3. Install dependencies: `cd DESIRED_INTEGRATION_FOLDER && make install`
-4. source the integration venv `. .venv/bin/activate`
-5. Run integration: `make run`
- 
-## Export Architecture
-![image](./assets/IntegrationFrameworkExportArchitecture.svg)
 
-## Real-Time updates Architecture
-![image](./assets/IntergationFrameworkRealTimeUpdatesArchitecture.svg)
+2. For new integration run
+
+   ```sh
+   make new
+   ```
+
+   and follow the instructions
+
+3. Install dependencies
+
+4. ```sh
+   cd DESIRED_INTEGRATION_FOLDER && make install
+   ```
+
+5. source the integration venv
 
-## Self Service Architecture
-![image](./assets/IntegrationFrameworkSelfServiceArchitecture.svg)
+   ```sh
+   . .venv/bin/activate
+   ```
+
+6. Run the integration
+
+   ```sh
+   make run
+   ```
+
+   Or
+
+   ```sh
+   ocean sail
+   ```
+
+   
+
+# Export Architecture
+
+![image](./assets/ExportArchitecture.svg)
+
+## Real-Time updates Architecture
+![image](./assets/RealTimeUpdatesArchitecture.svg)
 
 ## Folder Structure
 The Integration Framework follows a specific folder structure within the mono repository. This structure ensures proper organization and easy identification of integration modules. The suggested folder structure is as follows:
 
 ```
 port-ocean/
 ├── port_ocean (framework)/
@@ -51,42 +126,40 @@
 ├── ...
 └── ...
 ```
 
 - The `framework` folder contains the core logic for managing the integration lifecycle.
 - Each integration is represented by a separate folder inside the `integrations` directory.
 - Inside each integration folder, you'll find a `main.py` file that implements the core functionality of the integration for the specific third-party system.
-- The `requirements.txt` file inside each integration folder lists the required dependencies for that integration.
+- The `pyproject.toml` file inside each integration folder lists the required dependencies for that integration.
 
 ## Integration Lifecycle
 
-![image](./assets/IntegrationFrameworkLifecycleOfIntegration.svg)
+![image](./assets/LifecycleOfIntegration.svg)
 
 ## Configuration
-The Integration Framework utilizes a `config.yaml` file for configuration. This file specifies the integrations to be used within an array. Each integration has a unique identifier and type, which are used during initialization to update Port accordingly.
+The Integration Framework utilizes a `config.yaml` file for its configuration. This file defines both the framework configuration and the integration configuration within it. Each integration is identified by its type and unique identifier, which are utilized during initialization to appropriately update Port.
 
 Example `config.yaml`:
 ```yaml
 # This is an example configuration file for the integration service.
 # Please copy this file to config.yaml file in the integration folder and edit it to your needs.
 
 port:
   clientId: PORT_CLIENT_ID # Can be loaded via environment variable: PORT_CLIENT_ID
   clientSecret: PORT_CLIENT_SECRET # Can be loaded via environment variable: PORT_CLIENT_SECRET
   baseUrl: https://api.getport.io/v1
 # The trigger channel to use for the integration service.
 triggerChannel:
-  type: KAFKA
-  brokers: "localhost:9092"
-  kafkaSecurityEnabled: false
+  type: KAFKA / WEBHOOK
 integration:
   # The name of the integration.
   identifier: "my_integration"
   # The type of the integration.
-  type: "Git"
+  type: "PagerDuty"
   config:
     my_git_token: "random"
     some_other_integration_config: "Very important information"
 ```
 
 ## Contributing
 We welcome contributions to the Integration Framework project. If you have any suggestions, bug reports, or would like to contribute new features, please follow our guidelines outlined in the `CONTRIBUTING.md` file.
```

### Comparing `port_ocean-0.1.0.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile` & `port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml` & `port_ocean-0.1.0.dev5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev4/port_ocean/cli/download_git_folder.py` & `port_ocean-0.1.0.dev5/port_ocean/cli/download_git_folder.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev4/port_ocean/cli/list_integrations.py` & `port_ocean-0.1.0.dev5/port_ocean/cli/list_integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev4/port_ocean/clients/port/types.py` & `port_ocean-0.1.0.dev5/port_ocean/clients/port/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev4/port_ocean/config/integration.py` & `port_ocean-0.1.0.dev5/port_ocean/config/integration.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-import warnings
 from typing import Any
 
 from pydantic import BaseModel, Field
 from pydantic import BaseSettings
 
 from port_ocean.config.base import BaseOceanSettings
 from port_ocean.core.trigger_channel.settings import (
     HttpTriggerChannelSettings,
     KafkaTriggerChannelSettings,
 )
 
-warnings.filterwarnings("ignore", category=FutureWarning)
-
 
 class PortSettings(BaseSettings):
     client_id: str = Field(alias="clientId")
     client_secret: str = Field(alias="clientSecret")
-    base_url: str = Field(alias="baseUrl")
+    base_url: str = Field(alias="baseUrl", default="https://api.getport.io/v1")
 
 
 class IntegrationSettings(BaseSettings):
     identifier: str
     type: str
     config: dict[str, Any]
```

### Comparing `port_ocean-0.1.0.dev4/port_ocean/consumers/kafka_consumer.py` & `port_ocean-0.1.0.dev5/port_ocean/consumers/kafka_consumer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import asyncio
 import json
 import signal
+import sys
 from typing import Any, Callable, Awaitable
 
 from confluent_kafka import Consumer, KafkaException, Message  # type: ignore
 from loguru import logger
 from pydantic import BaseModel
 
 from port_ocean.consumers.base_consumer import BaseConsumer
 
 
 class KafkaConsumerConfig(BaseModel):
     brokers: str
     username: str | None = None
     password: str | None = None
+    group_name: str | None = None
     security_protocol: str
     authentication_mechanism: str
     kafka_security_enabled: bool
 
 
 class KafkaConsumer(BaseConsumer):
     def __init__(
         self,
         msg_process: Callable[[dict[Any, Any], str], Awaitable[None]],
         config: KafkaConsumerConfig,
-        org_id: str | None = None,
+        org_id: str,
     ) -> None:
         self.running = False
         self.org_id = org_id
 
         signal.signal(signal.SIGINT, self.exit_gracefully)
         signal.signal(signal.SIGTERM, self.exit_gracefully)
 
@@ -36,15 +38,15 @@
         if config.kafka_security_enabled:
             kafka_config = {
                 "bootstrap.servers": config.brokers,
                 "security.protocol": config.security_protocol,
                 "sasl.mechanism": config.authentication_mechanism,
                 "sasl.username": config.username,
                 "sasl.password": config.password,
-                "group.id": config.username,
+                "group.id": f"{self.org_id}.{config.group_name}",
                 "enable.auto.commit": "false",
             }
         else:
             kafka_config = {
                 "bootstrap.servers": config.brokers,
                 "group.id": "no-security",
                 "enable.auto.commit": "false",
@@ -56,15 +58,18 @@
         message = json.loads(raw_msg.value().decode())
         topic = raw_msg.topic()
 
         async def try_wrapper() -> None:
             try:
                 await self.msg_process(message, topic)
             except Exception as e:
-                logger.error(f"Failed to process message: {str(e)}")
+                _type, _, tb = sys.exc_info()
+                logger.opt(exception=(_type, None, tb)).error(
+                    f"Failed to process message: {str(e)}"
+                )
 
         asyncio.run(try_wrapper())
 
     def start(self) -> None:
         try:
             logger.info("Start consumer...")
 
@@ -96,13 +101,13 @@
                                 f" from topic {msg.topic()}, partition {msg.partition()}, offset {msg.offset()}: {str(process_error)}"
                             )
                         finally:
                             self.consumer.commit(asynchronous=False)
                 except Exception as message_error:
                     logger.error(str(message_error))
         finally:
-            self.consumer.close()
+            self.exit_gracefully()
 
     def exit_gracefully(self, *_: Any) -> None:
         logger.info("Exiting gracefully...")
         self.running = False
         self.consumer.close()
```

### Comparing `port_ocean-0.1.0.dev4/port_ocean/context/event.py` & `port_ocean-0.1.0.dev5/port_ocean/context/event.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dataclasses import dataclass, field
 from typing import AsyncIterator, Literal, Any, TYPE_CHECKING, Optional
 from uuid import uuid4
 
 from loguru import logger
 from werkzeug.local import LocalStack, LocalProxy
 
-from port_ocean.errors import EventContextNotFoundError
+from port_ocean.exceptions.context import EventContextNotFoundError
 from port_ocean.utils import get_time
 
 if TYPE_CHECKING:
     from port_ocean.core.handlers.port_app_config.models import PortAppConfig
 
 TriggerType = Literal["manual", "machine", "request"]
 
@@ -83,17 +83,14 @@
             trigger_type=trigger_type,
             attributes=attributes,
             _parent_event=parent,
         )
     )
 
     start_time = get_time(seconds_precision=False)
-    logger.bind(
-        event_id=event.id, event_type=event.event_type, parent_id=event.parent_id
-    ).info("Event started")
     with logger.contextualize(
         event_trigger_type=event.trigger_type,
         event_kind=event.event_type,
         event_id=event.id,
     ):
         logger.info("Event started")
         try:
```

### Comparing `port_ocean-0.1.0.dev4/port_ocean/context/ocean.py` & `port_ocean-0.1.0.dev5/port_ocean/context/ocean.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from port_ocean.config.integration import IntegrationConfiguration
 from port_ocean.core.models import Entity
 from port_ocean.core.types import (
     RESYNC_EVENT_LISTENER,
     START_EVENT_LISTENER,
     RawEntityDiff,
 )
-from port_ocean.errors import PortOceanContextNotFoundError
+from port_ocean.exceptions.context import PortOceanContextNotFoundError
 
 if TYPE_CHECKING:
     from port_ocean.core.integrations.base import BaseIntegration
     from port_ocean.ocean import Ocean
 
 
 @dataclass
@@ -98,16 +98,16 @@
         await self.integration.unregister(entities, user_agent_type)
 
     async def sync(
         self, entities: list[Entity], user_agent_type: UserAgentType
     ) -> None:
         await self.integration.sync(entities, user_agent_type)
 
-    async def sync_all(self) -> None:
-        await self.integration.sync_all(trigger_type="manual")
+    async def sync_raw_all(self) -> None:
+        await self.integration.sync_raw_all(trigger_type="manual")
 
 
 _port_ocean_context_stack: LocalStack[PortOceanContext] = LocalStack()
 
 
 def initialize_port_ocean_context(ocean_app: "Ocean") -> None:
     """
```

### Comparing `port_ocean-0.1.0.dev4/port_ocean/core/handlers/manipulation/base.py` & `port_ocean-0.1.0.dev5/port_ocean/core/handlers/manipulation/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from abc import abstractmethod
 from dataclasses import dataclass, field
 
+from loguru import logger
+
 from port_ocean.core.base import BaseWithContext
 from port_ocean.core.handlers.port_app_config.models import ResourceConfig
 from port_ocean.core.models import Entity
 from port_ocean.core.types import RawEntityDiff, EntityDiff
 
 
 @dataclass
@@ -12,11 +14,17 @@
     deleted: list[Entity] = field(default_factory=list)
     modified: list[Entity] = field(default_factory=list)
     created: list[Entity] = field(default_factory=list)
 
 
 class BaseManipulation(BaseWithContext):
     @abstractmethod
-    async def parse_items(
+    async def _parse_items(
         self, mapping: ResourceConfig, raw_data: RawEntityDiff
     ) -> EntityDiff:
         pass
+
+    async def parse_items(
+        self, mapping: ResourceConfig, raw_data: RawEntityDiff
+    ) -> EntityDiff:
+        with logger.contextualize(kind=mapping.kind):
+            return await self._parse_items(mapping, raw_data)
```

### Comparing `port_ocean-0.1.0.dev4/port_ocean/core/handlers/manipulation/jq_manipulation.py` & `port_ocean-0.1.0.dev5/port_ocean/core/handlers/manipulation/jq_manipulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from functools import lru_cache
 from typing import Any
 
 import pyjq as jq  # type: ignore
+
 from port_ocean.core.handlers.manipulation.base import BaseManipulation
 from port_ocean.core.handlers.port_app_config.models import ResourceConfig
 from port_ocean.core.models import Entity
 from port_ocean.core.types import RawEntityDiff, EntityDiff
-from port_ocean.exceptions.base import ManipulationHandlerException
+from port_ocean.exceptions.core import ManipulationHandlerException
 
 
 class JQManipulation(BaseManipulation):
     @lru_cache
     def _compile(self, pattern: str) -> Any:
         return jq.compile(pattern)
 
@@ -40,15 +41,15 @@
                     result[key] = self._search_as_object(data, value)
                 else:
                     result[key] = self._search(data, value)
             except Exception:
                 result[key] = None
         return result
 
-    def _parse_items(
+    def _calculate_entities(
         self, mapping: ResourceConfig, raw_data: list[dict[str, Any]]
     ) -> list[Entity]:
         entities = []
         for data in raw_data:
             should_run = self._search_as_bool(data, mapping.selector.query)
 
             if should_run and mapping.port.entity:
@@ -60,19 +61,21 @@
             Entity.parse_obj(entity_data)
             for entity_data in filter(
                 lambda entity: entity.get("identifier") and entity.get("blueprint"),
                 entities,
             )
         ]
 
-    async def parse_items(
+    async def _parse_items(
         self, mapping: ResourceConfig, raw_results: RawEntityDiff
     ) -> EntityDiff:
-        entities_before: list[Entity] = self._parse_items(
+        entities_before: list[Entity] = self._calculate_entities(
             mapping, raw_results["before"]
         )
-        entities_after: list[Entity] = self._parse_items(mapping, raw_results["after"])
+        entities_after: list[Entity] = self._calculate_entities(
+            mapping, raw_results["after"]
+        )
 
         return {
             "before": entities_before,
             "after": entities_after,
         }
```

### Comparing `port_ocean-0.1.0.dev4/port_ocean/core/handlers/port_app_config/base.py` & `port_ocean-0.1.0.dev5/port_ocean/core/handlers/port_app_config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev4/port_ocean/core/handlers/port_app_config/models.py` & `port_ocean-0.1.0.dev5/port_ocean/core/handlers/port_app_config/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev4/port_ocean/core/handlers/transport/base.py` & `port_ocean-0.1.0.dev5/port_ocean/core/handlers/transport/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 from port_ocean.clients.port.types import UserAgentType
 from port_ocean.core.base import BaseWithContext
 from port_ocean.core.models import Entity
 from port_ocean.core.types import EntityDiff
 
 
 class BaseTransport(BaseWithContext):
-    DEFAULT_USER_AGENT_TYPE = UserAgentType.exporter
-
     @abstractmethod
-    async def update_diff(
+    async def apply_diff(
         self,
         entities: EntityDiff,
-        user_agent: UserAgentType | None = None,
+        user_agent: UserAgentType,
     ) -> None:
         pass
 
     @abstractmethod
-    async def upsert(
-        self, entities: list[Entity], user_agent_type: UserAgentType
+    async def delete_diff(
+        self,
+        entities: EntityDiff,
+        user_agent: UserAgentType,
     ) -> None:
         pass
 
     @abstractmethod
-    async def delete(
+    async def upsert(
         self, entities: list[Entity], user_agent_type: UserAgentType
     ) -> None:
         pass
 
     @abstractmethod
-    async def delete_non_existing(
-        self, entities: list[Entity], user_agent: UserAgentType
+    async def delete(
+        self, entities: list[Entity], user_agent_type: UserAgentType
     ) -> None:
         pass
```

### Comparing `port_ocean-0.1.0.dev4/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py` & `port_ocean-0.1.0.dev5/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev4/port_ocean/core/handlers/transport/port/validate_entity_relations.py` & `port_ocean-0.1.0.dev5/port_ocean/core/handlers/transport/port/get_related_entities.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 import asyncio
 from itertools import groupby
 
 from port_ocean.clients.port.client import PortClient
-from port_ocean.core.handlers.manipulation.base import EntityPortDiff
-from port_ocean.core.handlers.transport.port.get_required_entities import (
-    get_required_entities,
-)
+from port_ocean.core.models import Entity
 
 
-async def validate_entity_relations(
-    diff: EntityPortDiff, port_client: PortClient
-) -> None:
-    modified_or_created_entities = diff.modified + diff.created
-    entities_with_relations = [
-        entity for entity in modified_or_created_entities if entity.relations
-    ]
+async def get_related_entities(
+    entities: list[Entity], port_client: PortClient
+) -> list[Entity]:
+    entities_with_relations = [entity for entity in entities if entity.relations]
     blueprint_identifier_to_entity = dict(
         groupby(
             entities_with_relations,
             key=lambda x: x.blueprint,
         )
     )
     blueprints = await asyncio.gather(
@@ -35,17 +29,16 @@
                 for blueprint in blueprints
                 if blueprint.identifier == entity.blueprint
             ),
         )
         for entity in entities_with_relations
     ]
 
-    required_entities = get_required_entities(
-        entity_to_blueprint, diff.deleted, modified_or_created_entities
-    )
+    related_entities = []
+    for entity, blueprint in entity_to_blueprint:
+        for relation_name, relation in entity.relations.items():
+            relation_blueprint = blueprint.relations[relation_name].target
+            related_entities.append(
+                Entity(identifier=relation, blueprint=relation_blueprint)
+            )
 
-    await asyncio.gather(
-        *[
-            port_client.validate_entity_exist(item.identifier, item.blueprint)
-            for item in required_entities
-        ]
-    )
+    return related_entities
```

### Comparing `port_ocean-0.1.0.dev4/port_ocean/core/integrations/mixins/events.py` & `port_ocean-0.1.0.dev5/port_ocean/core/integrations/mixins/events.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev4/port_ocean/core/integrations/mixins/handler.py` & `port_ocean-0.1.0.dev5/port_ocean/core/integrations/mixins/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Callable
 
 from loguru import logger
+
 from port_ocean.context.ocean import PortOceanContext, ocean
 from port_ocean.core.handlers import BaseManipulation, BasePortAppConfig, BaseTransport
 from port_ocean.core.handlers.manipulation.jq_manipulation import JQManipulation
 from port_ocean.core.handlers.port_app_config.api import APIPortAppConfig
 from port_ocean.core.handlers.transport.port.transport import HttpPortTransport
-from port_ocean.exceptions.base import IntegrationNotStartedException
+from port_ocean.exceptions.core import IntegrationNotStartedException
 
 
 class HandlerMixin:
     ManipulationHandlerClass: Callable[
         [PortOceanContext], BaseManipulation
     ] = JQManipulation
```

### Comparing `port_ocean-0.1.0.dev4/port_ocean/core/integrations/mixins/sync.py` & `port_ocean-0.1.0.dev5/port_ocean/core/integrations/mixins/sync.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import asyncio
 from itertools import chain
 from typing import Any, Awaitable
 
 from loguru import logger
 
 from port_ocean.clients.port.types import UserAgentType
+from port_ocean.context.event import TriggerType, event_context
+from port_ocean.context.ocean import ocean
 from port_ocean.core.handlers.port_app_config.models import ResourceConfig
 from port_ocean.core.integrations.mixins.events import EventsMixin
 from port_ocean.core.integrations.mixins.handler import HandlerMixin
 from port_ocean.core.models import Entity
 from port_ocean.core.types import RawEntityDiff, EntityDiff, RESYNC_EVENT_LISTENER
 from port_ocean.core.utils import validate_result, zip_and_sum
-from port_ocean.exceptions.base import RawObjectValidationException
+from port_ocean.exceptions.core import RawObjectValidationException
 from port_ocean.utils import get_function_location
 
 
 class SyncMixin(HandlerMixin, EventsMixin):
     def __init__(self) -> None:
         HandlerMixin.__init__(self)
         EventsMixin.__init__(self)
@@ -35,16 +37,20 @@
         logger.info("Finished unregistering change")
 
     async def sync(
         self,
         entities: list[Entity],
         user_agent_type: UserAgentType,
     ) -> None:
+        entities_at_port = await ocean.port_client.search_entities(user_agent_type)
+
         await self.transport.upsert(entities, user_agent_type)
-        await self.transport.delete_non_existing(entities, user_agent_type)
+        await self.transport.delete_diff(
+            {"before": entities_at_port, "after": entities}, user_agent_type
+        )
 
         logger.info("Finished syncing change")
 
 
 class SyncRawMixin(HandlerMixin, EventsMixin):
     def __init__(self) -> None:
         HandlerMixin.__init__(self)
@@ -60,15 +66,15 @@
         return await asyncio.gather(
             *[
                 self.manipulation.parse_items(mapping, results)
                 for mapping, results in raw_diff
             ]
         )
 
-    async def _validate_raw_data_wrapper(
+    async def _resync_function_wrapper(
         self, fn: RESYNC_EVENT_LISTENER, kind: str
     ) -> Any:
         results = await fn(kind)
         try:
             return validate_result(results)
         except RawObjectValidationException as error:
             raise RawObjectValidationException(
@@ -78,36 +84,34 @@
     async def _get_resource_raw_results(
         self, resource_config: ResourceConfig
     ) -> tuple[ResourceConfig, list[dict[Any, Any]]]:
         logger.info(f"Fetching {resource_config.kind} resync results")
         tasks: list[Awaitable[list[dict[Any, Any]]]] = []
         with logger.contextualize(kind=resource_config.kind):
             if self.__class__._on_resync != SyncRawMixin._on_resync:
-                tasks.append(self._on_resync(resource_config.kind))
+                tasks.append(
+                    self._resync_function_wrapper(self._on_resync, resource_config.kind)
+                )
 
             fns = [
                 *self.event_strategy["resync"][resource_config.kind],
                 *self.event_strategy["resync"][None],
             ]
 
-            for resync_function in fns:
-                tasks.append(
-                    self._validate_raw_data_wrapper(
-                        resync_function, resource_config.kind
-                    )
-                )
+            tasks.extend(
+                [
+                    self._resync_function_wrapper(resync_function, resource_config.kind)
+                    for resync_function in fns
+                ]
+            )
 
             logger.info(f"Found {len(tasks)} resync tasks for {resource_config.kind}")
+
             results: list[dict[Any, Any]] = list(
-                chain.from_iterable(
-                    [
-                        validate_result(task_result)
-                        for task_result in await asyncio.gather(*tasks)
-                    ]
-                )
+                chain.from_iterable(await asyncio.gather(*tasks))
             )
 
             logger.info(f"Triggered {len(tasks)} tasks for {resource_config.kind}")
             return resource_config, results
 
     async def _register_resource_raw(
         self,
@@ -125,15 +129,14 @@
                     },
                 )
             ]
         )
 
         entities_after: list[Entity] = objects_diff[0]["after"]
         await self.transport.upsert(entities_after, user_agent_type)
-        logger.info("Finished registering change")
         return entities_after
 
     async def _unregister_resource_raw(
         self,
         resource: ResourceConfig,
         results: list[dict[Any, Any]],
         user_agent_type: UserAgentType,
@@ -151,14 +154,39 @@
         )
 
         entities_after: list[Entity] = objects_diff[0]["before"]
         await self.transport.delete(entities_after, user_agent_type)
         logger.info("Finished unregistering change")
         return entities_after
 
+    async def _register_in_batches(
+        self,
+        resource_config: ResourceConfig,
+        user_agent_type: UserAgentType,
+        batch_work_size: int | None,
+    ) -> list[Entity]:
+        resource, results = await self._get_resource_raw_results(resource_config)
+
+        tasks = []
+
+        batch_size = batch_work_size or len(results) or 1
+        batches = [
+            results[i : i + batch_size] for i in range(0, len(results), batch_size)
+        ]
+        for batch in batches:
+            logger.info(f"Creating task for registering batch of {len(batch)} entities")
+            tasks.append(self._register_resource_raw(resource, batch, user_agent_type))
+
+        registered_entities_results = await asyncio.gather(*tasks)
+        entities: list[Entity] = sum(registered_entities_results, [])
+        logger.info(
+            f"Finished registering change for {len(results)} raw results for kind: {resource_config.kind}"
+        )
+        return entities
+
     async def register_raw(
         self,
         kind: str,
         results: list[dict[Any, Any]],
         user_agent_type: UserAgentType,
     ) -> list[Entity]:
         logger.info(f"Registering state for {kind}")
@@ -215,10 +243,37 @@
             entities_before, entities_after = zip_and_sum(
                 (
                     (entities_change["before"], entities_change["after"])
                     for entities_change in objects_diff
                 )
             )
 
-            await self.transport.update_diff(
+            await self.transport.apply_diff(
                 {"before": entities_before, "after": entities_after}, user_agent_type
             )
+
+    async def sync_raw_all(
+        self,
+        _: dict[Any, Any] | None = None,
+        trigger_type: TriggerType = "machine",
+        user_agent_type: UserAgentType = UserAgentType.exporter,
+    ) -> None:
+        logger.info("Resync was triggered")
+
+        async with event_context("resync", trigger_type=trigger_type):
+            app_config = await self.port_app_config_handler.get_port_app_config()
+
+            entities_at_port = await ocean.port_client.search_entities(user_agent_type)
+
+            created_entities = await asyncio.gather(
+                *(
+                    self._register_in_batches(
+                        resource, user_agent_type, ocean.config.batch_work_size
+                    )
+                    for resource in app_config.resources
+                )
+            )
+            flat_created_entities: list[Entity] = sum(created_entities, [])
+            await self.transport.delete_diff(
+                {"before": entities_at_port, "after": flat_created_entities},
+                user_agent_type,
+            )
```

### Comparing `port_ocean-0.1.0.dev4/port_ocean/core/models.py` & `port_ocean-0.1.0.dev5/port_ocean/core/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev4/port_ocean/core/trigger_channel/factory.py` & `port_ocean-0.1.0.dev5/port_ocean/core/trigger_channel/factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from port_ocean.core.trigger_channel.kafka import (
     KafkaTriggerChannel,
 )
 from port_ocean.core.trigger_channel.settings import (
     HttpTriggerChannelSettings,
     KafkaTriggerChannelSettings,
 )
-from port_ocean.exceptions.base import UnsupportedTriggerChannelException
+from port_ocean.exceptions.core import UnsupportedTriggerChannelException
 
 
 class TriggerChannelFactory(BaseWithContext):
     def __init__(
         self,
         context: PortOceanContext,
         installation_id: str,
@@ -62,14 +62,16 @@
                     config, KafkaTriggerChannelSettings
                 ), assert_message.format(type(config))
                 org_id = await self.context.port_client.get_org_id()
                 self._trigger_channel = KafkaTriggerChannel(
                     wrapped_events,
                     config,
                     org_id,
+                    self.context.config.integration.identifier,
+                    self.context.config.integration.type,
                 )
 
             case "webhook":
                 assert isinstance(
                     config, HttpTriggerChannelSettings
                 ), assert_message.format(type(config))
                 self._trigger_channel = HttpTriggerChannel(wrapped_events, config)
```

### Comparing `port_ocean-0.1.0.dev4/port_ocean/core/trigger_channel/http.py` & `port_ocean-0.1.0.dev5/port_ocean/core/trigger_channel/http.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev4/port_ocean/core/trigger_channel/settings.py` & `port_ocean-0.1.0.dev5/port_ocean/core/trigger_channel/settings.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev4/port_ocean/core/types.py` & `port_ocean-0.1.0.dev5/port_ocean/core/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev4/port_ocean/core/utils.py` & `port_ocean-0.1.0.dev5/port_ocean/core/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Any, TypeVar
 
 from port_ocean.core.handlers.manipulation.base import EntityPortDiff
 from port_ocean.core.models import Entity
-from port_ocean.exceptions.base import RawObjectValidationException
+from port_ocean.exceptions.core import RawObjectValidationException
 
 
 def is_valid_diff_item(item: Any) -> bool:
     return isinstance(item, list) and all([isinstance(i, dict) for i in item] or [True])
 
 
 def validate_result(result: Any) -> list[dict[Any, Any]]:
```

### Comparing `port_ocean-0.1.0.dev4/port_ocean/middlewares.py` & `port_ocean-0.1.0.dev5/port_ocean/middlewares.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Callable, Awaitable
 
 from fastapi import Request, Response
 from loguru import logger
 
+from port_ocean.exceptions.api import BaseAPIException, InternalServerException
 from .context.event import event_context
 from .context.ocean import ocean
-from .exceptions.api.base import BaseAPIException, InternalServerException
 from .utils import get_time, get_uuid
 
 
 async def _handle_silently(
     call_next: Callable[[Request], Awaitable[Response]], request: Request
 ) -> Response:
     response: Response
```

### Comparing `port_ocean-0.1.0.dev4/port_ocean/ocean.py` & `port_ocean-0.1.0.dev5/port_ocean/ocean.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from port_ocean.config.integration import IntegrationConfiguration
 from port_ocean.context.ocean import (
     PortOceanContext,
     ocean,
     initialize_port_ocean_context,
 )
 from port_ocean.core.integrations.base import BaseIntegration
-from port_ocean.logger_setup import setup_logger
+from port_ocean.logger_setup import setup_logger, LogLevelType
 from port_ocean.middlewares import request_handler
 
 
 def _get_base_integration_class_from_module(
     module: ModuleType,
 ) -> Type[BaseIntegration]:
     for name, obj in getmembers(module):
@@ -53,15 +53,15 @@
 
 
 def _include_target_channel_router(app: FastAPI, _ocean: PortOceanContext) -> None:
     target_channel_router = APIRouter()
 
     @target_channel_router.post("/resync")
     async def resync() -> None:
-        await _ocean.integration.sync_all()
+        await _ocean.integration.sync_raw_all()
 
     app.include_router(target_channel_router)
 
 
 class Ocean:
     def __init__(
         self,
@@ -81,15 +81,16 @@
             ).dict()
         self.integration_router = integration_router or APIRouter()
 
         self.port_client = PortClient(
             base_url=self.config.port.base_url,
             client_id=self.config.port.client_id,
             client_secret=self.config.port.client_secret,
-            user_agent_id=self.config.integration.identifier,
+            integration_identifier=self.config.integration.identifier,
+            integration_type=self.config.integration.type,
         )
         self.integration = (
             integration_class(ocean) if integration_class else BaseIntegration(ocean)
         )
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         self.fast_api_app.include_router(self.integration_router, prefix="/integration")
@@ -103,16 +104,16 @@
             except Exception as e:
                 logger.error(f"Failed to start integration with error: {e}")
                 sys.exit("Server stopped")
 
         await self.fast_api_app(scope, receive, send)
 
 
-def run(path: str) -> None:
-    setup_logger()
+def run(path: str, log_level: LogLevelType = "DEBUG") -> None:
+    setup_logger(log_level)
     sys.path.append(".")
     try:
         integration_path = f"{path}/integration.py" if path else "integration.py"
         module = _load_module(integration_path)
         integration_class = _get_base_integration_class_from_module(module)
     except Exception:
         integration_class = None
```

### Comparing `port_ocean-0.1.0.dev4/port_ocean/utils.py` & `port_ocean-0.1.0.dev5/port_ocean/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev4/pyproject.toml` & `port_ocean-0.1.0.dev5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "port-ocean"
-version = "0.1.0.dev4"
+version = "0.1.0.dev5"
 description = "Port Ocean is a CLI tool for managing your Port projects."
 readme = "README.md"
 authors = ["Daniel Sinai <daniel@getport.io>", "Yair Siman-Tov <yair@getport.io>"]
 packages = [
     { include = "port_ocean", from = "." }
 ]
 
@@ -30,33 +30,36 @@
 urllib3 = "^1.26.16"
 six = "^1.16.0"
 
 # CLI
 click = { version = "^8.1.3", optional = true }
 rich = { version = "^13.4.1", optional = true }
 cookiecutter = { version = "^2.1.1", optional = true }
+toml = { version = "^0.10.2", optional = true }
 
 [tool.poetry.extras]
-cli = ["click", "rich", "cookiecutter"]
+cli = ["click", "rich", "cookiecutter", "toml"]
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2"
 black = "^23.3.0"
 mypy = "^1.3.0"
 pylint = "^2.17.4"
 types-requests = "^2.31.0.1"
 types-pyyaml = "^6.0.12.10"
 ruff = "^0.0.272"
+types-toml = "^0.10.8.6"
 
 
 [tool.mypy]
 exclude = [
     'port_ocean/cli/cookiecutter',
     'venv',
+    '.venv',
     'integrations'
 ]
 plugins = [
     "pydantic.mypy"
 ]
 
 follow_imports = "silent"
@@ -69,15 +72,15 @@
 # for strict mypy: (this is the tricky one :-))
 disallow_untyped_defs = true
 
 
 [tool.ruff]
 # Never enforce `E501` (line length violations).
 ignore = ["E501"]
-exclude = ['venv', 'integrations']
+exclude = ['venv', '.venv', 'integrations']
 
 [tool.pydantic-mypy]
 init_forbid_extra = true
 init_typed = true
 warn_required_dynamic_aliases = true
 warn_untyped_fields = true
```

### Comparing `port_ocean-0.1.0.dev4/PKG-INFO` & `port_ocean-0.1.0.dev5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-ocean
-Version: 0.1.0.dev4
+Version: 0.1.0.dev5
 Summary: Port Ocean is a CLI tool for managing your Port projects.
 Author: Daniel Sinai
 Author-email: daniel@getport.io
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cli
@@ -16,54 +16,130 @@
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: pyjq (>=2.6.0,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.4.1,<14.0.0) ; extra == "cli"
 Requires-Dist: six (>=1.16.0,<2.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "cli"
 Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Requires-Dist: werkzeug (>=2.3.4,<3.0.0)
 Description-Content-Type: text/markdown
 
-<img align="right" width="100" height="74" src="https://user-images.githubusercontent.com/8277210/183290025-d7b24277-dfb4-4ce1-bece-7fe0ecd5efd4.svg" />
+# Ocean <img src="./assets/OceanSymbol.svg" alt="Ocean" width="100" height="100" align="right">
 
-# Ocean
 [![Lint](https://github.com/port-labs/port-ocean/actions/workflows/lint.yml/badge.svg)](https://github.com/port-labs/port-ocean/actions/workflows/lint.yml)
 
-Ocean is a solution developed by Port to address the challenges faced while integrating various third-party systems with our developer portal product. This framework provides a standardized approach for implementing integrations, simplifying the process and allowing platform engineers to focus on the core functionality of the third-party system.
+Ocean is a solution created by Port to tackle the difficulties encountered when merging different third-party systems with our developer portal product. This framework offers a uniform method for executing integrations, streamlining the process and enabling platform engineers to prioritize the essential features of the third-party system.
+
+
+
+## Prerequisites
+
+- Python 3.11
+
+
 
 ## Installation
-`pip install port-ocean[cli]` or `poetry add port-ocean[cli]`
+```
+pip install port-ocean[cli]
+```
+
+Or
+
+```sh
+poetry add port-ocean[cli]
+```
+
+[]()
 
 ## Run Integration
-1. source the integration venv `. .venv/bin/activate`
-2. `ocean sail ./path/to/integration`
+
+1. source the integration venv 
+
+   ```sh
+   . .venv/bin/activate
+   ```
+
+2. Run
+
+   ```sh
+   ocean sail ./path/to/integration
+   ```
+
+   
 
 ## Local Development (Framework)
 1. Clone the repository
-2. Install dependencies: `make install` or `make install/all` for installing integrations dependencies as well
-3. source the integration venv `. .venv/bin/activate`
+
+2. Install dependencies:
+
+   ```sh
+   make install
+   ```
+
+   Or (For installing integrations dependencies as well)
+
+   ```sh
+   make install/all
+   ```
+
+3. source the integration venv
+
+   ```sh
+   . .venv/bin/activate
+   ```
+
+   
 
 
 ## Local Development (Integration)
 1. Clone the repository
-2. For new integration run `make new` and follow the instructions
-3. Install dependencies: `cd DESIRED_INTEGRATION_FOLDER && make install`
-4. source the integration venv `. .venv/bin/activate`
-5. Run integration: `make run`
- 
-## Export Architecture
-![image](./assets/IntegrationFrameworkExportArchitecture.svg)
 
-## Real-Time updates Architecture
-![image](./assets/IntergationFrameworkRealTimeUpdatesArchitecture.svg)
+2. For new integration run
+
+   ```sh
+   make new
+   ```
+
+   and follow the instructions
+
+3. Install dependencies
+
+4. ```sh
+   cd DESIRED_INTEGRATION_FOLDER && make install
+   ```
+
+5. source the integration venv
 
-## Self Service Architecture
-![image](./assets/IntegrationFrameworkSelfServiceArchitecture.svg)
+   ```sh
+   . .venv/bin/activate
+   ```
+
+6. Run the integration
+
+   ```sh
+   make run
+   ```
+
+   Or
+
+   ```sh
+   ocean sail
+   ```
+
+   
+
+# Export Architecture
+
+![image](./assets/ExportArchitecture.svg)
+
+## Real-Time updates Architecture
+![image](./assets/RealTimeUpdatesArchitecture.svg)
 
 ## Folder Structure
 The Integration Framework follows a specific folder structure within the mono repository. This structure ensures proper organization and easy identification of integration modules. The suggested folder structure is as follows:
 
 ```
 port-ocean/
 ├── port_ocean (framework)/
@@ -78,42 +154,40 @@
 ├── ...
 └── ...
 ```
 
 - The `framework` folder contains the core logic for managing the integration lifecycle.
 - Each integration is represented by a separate folder inside the `integrations` directory.
 - Inside each integration folder, you'll find a `main.py` file that implements the core functionality of the integration for the specific third-party system.
-- The `requirements.txt` file inside each integration folder lists the required dependencies for that integration.
+- The `pyproject.toml` file inside each integration folder lists the required dependencies for that integration.
 
 ## Integration Lifecycle
 
-![image](./assets/IntegrationFrameworkLifecycleOfIntegration.svg)
+![image](./assets/LifecycleOfIntegration.svg)
 
 ## Configuration
-The Integration Framework utilizes a `config.yaml` file for configuration. This file specifies the integrations to be used within an array. Each integration has a unique identifier and type, which are used during initialization to update Port accordingly.
+The Integration Framework utilizes a `config.yaml` file for its configuration. This file defines both the framework configuration and the integration configuration within it. Each integration is identified by its type and unique identifier, which are utilized during initialization to appropriately update Port.
 
 Example `config.yaml`:
 ```yaml
 # This is an example configuration file for the integration service.
 # Please copy this file to config.yaml file in the integration folder and edit it to your needs.
 
 port:
   clientId: PORT_CLIENT_ID # Can be loaded via environment variable: PORT_CLIENT_ID
   clientSecret: PORT_CLIENT_SECRET # Can be loaded via environment variable: PORT_CLIENT_SECRET
   baseUrl: https://api.getport.io/v1
 # The trigger channel to use for the integration service.
 triggerChannel:
-  type: KAFKA
-  brokers: "localhost:9092"
-  kafkaSecurityEnabled: false
+  type: KAFKA / WEBHOOK
 integration:
   # The name of the integration.
   identifier: "my_integration"
   # The type of the integration.
-  type: "Git"
+  type: "PagerDuty"
   config:
     my_git_token: "random"
     some_other_integration_config: "Very important information"
 ```
 
 ## Contributing
 We welcome contributions to the Integration Framework project. If you have any suggestions, bug reports, or would like to contribute new features, please follow our guidelines outlined in the `CONTRIBUTING.md` file.
```

