# Comparing `tmp/propan-0.1.5.0.tar.gz` & `tmp/propan-0.1.5.1.tar.gz`

## Comparing `propan-0.1.5.0.tar` & `propan-0.1.5.1.tar`

### file list

```diff
@@ -1,190 +1,190 @@
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.5.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.5.0/SECURITY.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.5.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.5.0/.github/dependantbot.yml
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.5.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 propan-0.1.5.0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.5.0/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.5.0/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 propan-0.1.5.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/kafka/1_direct.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/nats/1_basic.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/redis/pattern.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/scheduling/rocketry.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/serialization/gen_py_code.sh
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/serialization/message.proto
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/serialization/protobuf.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/serialization/requirements.txt
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/sqs/1_basic.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/__about__.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/__main__.py
--rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/_compat.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/py.typed
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/types.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/__init__.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/channels.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/info.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/main.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/message.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/security.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/servers.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/subscription.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/utils.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/bindings/__init__.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/bindings/amqp.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/bindings/kafka.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/bindings/main.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/bindings/nats.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/bindings/redis.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/bindings/sqs.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/__init__.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/constants.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/exceptions.py
--rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/_model/__init__.py
--rw-r--r--   0        0        0    19850 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/_model/broker_usecase.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/_model/routing.py
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/_model/schemas.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/_model/utils.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/kafka/__init__.py
--rw-r--r--   0        0        0    13299 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/kafka/kafka_broker.py
--rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/kafka/kafka_broker.pyi
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/kafka/routing.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/kafka/routing.pyi
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/kafka/schemas.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/nats/consts.py
--rw-r--r--   0        0        0     9155 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/nats/nats_js_broker.pyi
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/nats/routing.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/nats/routing.pyi
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/rabbit/logging.py
--rw-r--r--   0        0        0    13869 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0    11093 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/rabbit/routing.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/rabbit/routing.pyi
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/rabbit/utils.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/redis/routing.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/redis/routing.pyi
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/sqs/__init__.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/sqs/routing.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/sqs/routing.pyi
--rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/sqs/schema.py
--rw-r--r--   0        0        0    13265 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/sqs/sqs_broker.py
--rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/sqs/sqs_broker.pyi
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/__init__.py
--rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/app.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/main.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/docs/__init__.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/docs/app.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/docs/gen.py
--rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/docs/serving.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/async_app/kafka.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/async_app/sqs.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/kafka/__init__.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/kafka/router.py
--rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/kafka/router.pyi
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/nats/__init__.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/nats/router.py
--rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/nats/router.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/sqs/__init__.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/sqs/router.py
--rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/sqs/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/log/__init__.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/log/formatter.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/log/logging.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/test/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/test/kafka.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/test/nats.py
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/test/rabbit.py
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/test/redis.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/test/sqs.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/test/utils.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/utils/__init__.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/utils/classes.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/utils/functions.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/utils/no_cast.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/utils/context/main.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.5.0/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.5.0/scripts/publish.sh
--rwxr-xr-x   0        0        0      407 2020-02-02 00:00:00.000000 propan-0.1.5.0/scripts/test-cov.sh
--rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.5.0/scripts/test.sh
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.5.0/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.5.0/LICENSE
--rw-r--r--   0        0        0    14822 2020-02-02 00:00:00.000000 propan-0.1.5.0/README.md
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 propan-0.1.5.0/pyproject.toml
--rw-r--r--   0        0        0    19171 2020-02-02 00:00:00.000000 propan-0.1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 propan-0.1.5.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.5.1/SECURITY.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.5.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.5.1/.github/dependantbot.yml
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.5.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.5.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 propan-0.1.5.1/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.5.1/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.5.1/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 propan-0.1.5.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/kafka/1_direct.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/nats/1_basic.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/redis/pattern.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/scheduling/rocketry.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/serialization/gen_py_code.sh
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/serialization/message.proto
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/serialization/protobuf.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/serialization/requirements.txt
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/sqs/1_basic.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/__about__.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/__main__.py
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/_compat.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/py.typed
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/types.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/__init__.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/channels.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/info.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/main.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/message.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/security.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/servers.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/subscription.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/utils.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/bindings/__init__.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/bindings/amqp.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/bindings/kafka.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/bindings/main.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/bindings/nats.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/bindings/redis.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/bindings/sqs.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/__init__.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/constants.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/exceptions.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/_model/__init__.py
+-rw-r--r--   0        0        0    19850 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/_model/broker_usecase.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/_model/routing.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/_model/schemas.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/_model/utils.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/kafka/__init__.py
+-rw-r--r--   0        0        0    13299 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/kafka/kafka_broker.pyi
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/kafka/routing.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/kafka/routing.pyi
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/kafka/schemas.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/nats/consts.py
+-rw-r--r--   0        0        0     9155 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/nats/nats_js_broker.pyi
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/nats/routing.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/nats/routing.pyi
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/rabbit/logging.py
+-rw-r--r--   0        0        0    13869 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0    11093 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/rabbit/routing.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/rabbit/routing.pyi
+-rw-r--r--   0        0        0     7479 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/rabbit/utils.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/redis/routing.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/redis/routing.pyi
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/sqs/__init__.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/sqs/routing.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/sqs/routing.pyi
+-rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/sqs/schema.py
+-rw-r--r--   0        0        0    13265 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/sqs/sqs_broker.py
+-rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/sqs/sqs_broker.pyi
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/__init__.py
+-rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/app.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/main.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/docs/__init__.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/docs/app.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/docs/gen.py
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/docs/serving.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/async_app/kafka.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/async_app/sqs.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/kafka/__init__.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/kafka/router.py
+-rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/kafka/router.pyi
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/nats/__init__.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/nats/router.py
+-rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/nats/router.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/sqs/__init__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/sqs/router.py
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/sqs/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/log/__init__.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/log/formatter.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/log/logging.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/test/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/test/kafka.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/test/nats.py
+-rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/test/redis.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/test/sqs.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/test/utils.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/utils/__init__.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/utils/classes.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/utils/functions.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/utils/no_cast.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/utils/context/main.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.5.1/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.5.1/scripts/publish.sh
+-rwxr-xr-x   0        0        0      407 2020-02-02 00:00:00.000000 propan-0.1.5.1/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.5.1/scripts/test.sh
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.5.1/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.5.1/LICENSE
+-rw-r--r--   0        0        0    14954 2020-02-02 00:00:00.000000 propan-0.1.5.1/README.md
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 propan-0.1.5.1/pyproject.toml
+-rw-r--r--   0        0        0    19303 2020-02-02 00:00:00.000000 propan-0.1.5.1/PKG-INFO
```

### Comparing `propan-0.1.5.0/CONTRIBUTING.md` & `propan-0.1.5.1/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,17 @@
 ```
 
 There are some *pytest marks* at project:
 
 * **slow**
 * **rabbit**
 * **nats**
+* **sqs**
+* **kafka**
+* **redis**
 * **all**
 
 Default *pytest* calling runs "not slow" tests.
 
 To run all tests use:
 
 ```bash
@@ -98,14 +101,15 @@
   redis:
     image: redis
     ports:
       - 6379:6379
 
   nats:
     image: nats
+    command: -js
     ports:
       - 4222:4222
       - 8222:8222  # management
   
   kafka:
     image: bitnami/kafka
     ports:
```

### Comparing `propan-0.1.5.0/SECURITY.md` & `propan-0.1.5.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/.github/PULL_REQUEST_TEMPLATE.md` & `propan-0.1.5.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/.github/ISSUE_TEMPLATE/bug_report.md` & `propan-0.1.5.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/.github/ISSUE_TEMPLATE/config.yml` & `propan-0.1.5.1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/.github/workflows/documentation.yml` & `propan-0.1.5.1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/.github/workflows/publish_coverage.yml` & `propan-0.1.5.1/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/.github/workflows/publish_pypi.yml` & `propan-0.1.5.1/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/.github/workflows/tests.yml` & `propan-0.1.5.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/3_lifespan_events.py` & `propan-0.1.5.1/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/4_cli_attributes_promotion.py` & `propan-0.1.5.1/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/5_publishing.py` & `propan-0.1.5.1/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/6_arguments_casting.py` & `propan-0.1.5.1/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/7_handler_errors_processing.py` & `propan-0.1.5.1/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/dependencies/1_dependency_injection.py` & `propan-0.1.5.1/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.5.1/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.5.1/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.5.1/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.5.1/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/dependencies/7_annotated.py` & `propan-0.1.5.1/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.5.1/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.5.1/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.5.1/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.5.1/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/http_frameworks_integrations/quart.py` & `propan-0.1.5.1/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.5.1/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.5.1/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/rabbit/direct.py` & `propan-0.1.5.1/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/rabbit/fanout.py` & `propan-0.1.5.1/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/rabbit/header.py` & `propan-0.1.5.1/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/rabbit/topic.py` & `propan-0.1.5.1/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/redis/direct.py` & `propan-0.1.5.1/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/redis/pattern.py` & `propan-0.1.5.1/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/examples/serialization/protobuf.py` & `propan-0.1.5.1/examples/serialization/protobuf.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/__about__.py` & `propan-0.1.5.1/propan/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Simple and fast framework to create message brokers based microservices"""
 
 from unittest.mock import Mock
 
-__version__ = "0.1.5.0"
+__version__ = "0.1.5.1"
 
 
 INSTALL_MESSAGE = (
     "You should specify using broker!\n"
     "Install it using one of the following commands:\n"
     'pip install "propan[async-rabbit]"\n'
     'pip install "propan[async-nats]"\n'
```

### Comparing `propan-0.1.5.0/propan/__init__.py` & `propan-0.1.5.1/propan/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/_compat.py` & `propan-0.1.5.1/propan/_compat.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/annotations.py` & `propan-0.1.5.1/propan/annotations.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/types.py` & `propan-0.1.5.1/propan/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/asyncapi/__init__.py` & `propan-0.1.5.1/propan/asyncapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/asyncapi/channels.py` & `propan-0.1.5.1/propan/asyncapi/channels.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/asyncapi/info.py` & `propan-0.1.5.1/propan/asyncapi/info.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/asyncapi/main.py` & `propan-0.1.5.1/propan/asyncapi/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/asyncapi/message.py` & `propan-0.1.5.1/propan/asyncapi/message.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/asyncapi/security.py` & `propan-0.1.5.1/propan/asyncapi/security.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/asyncapi/subscription.py` & `propan-0.1.5.1/propan/asyncapi/subscription.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/asyncapi/bindings/amqp.py` & `propan-0.1.5.1/propan/asyncapi/bindings/amqp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/asyncapi/bindings/kafka.py` & `propan-0.1.5.1/propan/asyncapi/bindings/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/asyncapi/bindings/main.py` & `propan-0.1.5.1/propan/asyncapi/bindings/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/asyncapi/bindings/redis.py` & `propan-0.1.5.1/propan/asyncapi/bindings/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/push_back_watcher.py` & `propan-0.1.5.1/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/_model/broker_usecase.py` & `propan-0.1.5.1/propan/brokers/_model/broker_usecase.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/_model/routing.py` & `propan-0.1.5.1/propan/brokers/_model/routing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/_model/schemas.py` & `propan-0.1.5.1/propan/brokers/_model/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/_model/utils.py` & `propan-0.1.5.1/propan/brokers/_model/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/kafka/kafka_broker.py` & `propan-0.1.5.1/propan/brokers/kafka/kafka_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/kafka/kafka_broker.pyi` & `propan-0.1.5.1/propan/brokers/kafka/kafka_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/kafka/routing.pyi` & `propan-0.1.5.1/propan/brokers/kafka/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/kafka/schemas.py` & `propan-0.1.5.1/propan/brokers/kafka/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/nats/nats_broker.py` & `propan-0.1.5.1/propan/brokers/nats/nats_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.5.1/propan/brokers/nats/nats_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.5.1/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/nats/nats_js_broker.pyi` & `propan-0.1.5.1/propan/brokers/nats/nats_js_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/nats/routing.pyi` & `propan-0.1.5.1/propan/brokers/nats/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/nats/schemas.py` & `propan-0.1.5.1/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/rabbit/logging.py` & `propan-0.1.5.1/propan/brokers/rabbit/logging.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-from typing import Optional
-
-import aio_pika
+from typing import Any, Optional
 
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.rabbit.schemas import RabbitExchange, RabbitQueue
 from propan.types import AnyDict
 
 
 class RabbitLoggingMixin:
     _max_queue_len: int
     _max_exchange_len: int
 
     def _get_log_context(
         self,
-        message: Optional[PropanMessage[aio_pika.message.IncomingMessage]],
+        message: Optional[PropanMessage[Any]],
         queue: RabbitQueue,
         exchange: Optional[RabbitExchange] = None,
     ) -> AnyDict:
         context = {
             "queue": queue.name,
             "exchange": exchange.name if exchange else "default",
             **super()._get_log_context(message),
```

### Comparing `propan-0.1.5.0/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.5.1/propan/brokers/rabbit/rabbit_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.5.1/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/rabbit/routing.pyi` & `propan-0.1.5.1/propan/brokers/rabbit/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/rabbit/schemas.py` & `propan-0.1.5.1/propan/brokers/rabbit/schemas.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 from dataclasses import dataclass, field
-from typing import Any, Dict, Optional
+from enum import Enum, unique
+from typing import Any, Dict, Optional, Union
 
-from aio_pika.abc import ExchangeType, TimeoutType
 from fast_depends.core import CallModel
 from pydantic import Field
+from typing_extensions import TypeAlias
 
 from propan.asyncapi.bindings import (
     AsyncAPIChannelBinding,
     AsyncAPIOperationBinding,
     amqp,
 )
 from propan.asyncapi.channels import AsyncAPIChannel
 from propan.asyncapi.message import AsyncAPICorrelationId, AsyncAPIMessage
 from propan.asyncapi.subscription import AsyncAPISubscription
 from propan.brokers._model.schemas import BaseHandler, NameRequired, Queue
 from propan.types import DecoratedCallable
 
-__all__ = (
-    "RabbitQueue",
-    "RabbitExchange",
-    "Handler",
-    "ExchangeType",
-)
+
+@unique
+class ExchangeType(str, Enum):
+    FANOUT = "fanout"
+    DIRECT = "direct"
+    TOPIC = "topic"
+    HEADERS = "headers"
+    X_DELAYED_MESSAGE = "x-delayed-message"
+    X_CONSISTENT_HASH = "x-consistent-hash"
+    X_MODULUS_HASH = "x-modulus-hash"
+
+
+TimeoutType: TypeAlias = Optional[Union[int, float]]
 
 
 class RabbitQueue(Queue):
     name: str = ""
     durable: bool = False
     exclusive: bool = False
     passive: bool = False
@@ -75,15 +83,15 @@
             auto_delete=auto_delete,
             arguments=arguments,
             timeout=timeout,
         )
 
 
 class RabbitExchange(NameRequired):
-    type: ExchangeType = ExchangeType.DIRECT
+    type: str = ExchangeType.DIRECT.value
     durable: bool = False
     auto_delete: bool = False
     internal: bool = False
     passive: bool = False
     arguments: Optional[Dict[str, Any]] = None
     timeout: TimeoutType = None
     robust: bool = True
@@ -92,15 +100,15 @@
     bind_arguments: Optional[Dict[str, Any]] = Field(default=None, exclude=True)
     routing_key: str = Field(default="", exclude=True)
 
     def __hash__(self) -> int:
         return sum(
             (
                 hash(self.name),
-                hash(self.type.value),
+                hash(self.type),
                 int(self.durable),
                 int(self.auto_delete),
             )
         )
 
     def __init__(
         self,
@@ -115,15 +123,15 @@
         robust: bool = True,
         bind_to: Optional["RabbitExchange"] = None,
         bind_arguments: Optional[Dict[str, Any]] = None,
         routing_key: str = "",
     ):
         super().__init__(
             name=name,
-            type=type,
+            type=type.value,
             durable=durable,
             auto_delete=auto_delete,
             routing_key=routing_key,
             bind_to=bind_to,
             bind_arguments=bind_arguments,
             robust=robust,
             internal=internal,
@@ -161,15 +169,18 @@
                     description=self.description,
                     bindings=AsyncAPIOperationBinding(
                         amqp=amqp.AsyncAPIAmqpOperationBinding(
                             cc=None
                             if (
                                 self.exchange
                                 and self.exchange.type
-                                in (ExchangeType.FANOUT, ExchangeType.HEADERS)
+                                in (
+                                    ExchangeType.FANOUT.value,
+                                    ExchangeType.HEADERS.value,
+                                )
                             )
                             else self.queue.name,
                             replyTo=reply_to,
                         ),
                     ),
                     message=AsyncAPIMessage(
                         title=message_title,
@@ -183,27 +194,30 @@
                     amqp=amqp.AsyncAPIAmqpChannelBinding(
                         **{
                             "is": "routingKey",  # type: ignore
                             "queue": None
                             if (
                                 self.exchange
                                 and self.exchange.type
-                                in (ExchangeType.FANOUT, ExchangeType.HEADERS)
+                                in (
+                                    ExchangeType.FANOUT.value,
+                                    ExchangeType.HEADERS.value,
+                                )
                             )
                             else amqp.AsyncAPIAmqpQueue(
                                 name=self.queue.name,
                                 durable=self.queue.durable,
                                 exclusive=self.queue.exclusive,
                                 autoDelete=self.queue.auto_delete,
                             ),
                             "exchange": (
                                 amqp.AsyncAPIAmqpExchange(type="default")
                                 if self.exchange is None
                                 else amqp.AsyncAPIAmqpExchange(
-                                    type=self.exchange.type.value,  # type: ignore
+                                    type=self.exchange.type,  # type: ignore
                                     name=self.exchange.name,
                                     durable=self.exchange.durable,
                                     autoDelete=self.exchange.auto_delete,
                                 )
                             ),
                         }
                     )
```

### Comparing `propan-0.1.5.0/propan/brokers/rabbit/utils.py` & `propan-0.1.5.1/propan/brokers/rabbit/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/redis/redis_broker.py` & `propan-0.1.5.1/propan/brokers/redis/redis_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.5.1/propan/brokers/redis/redis_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/redis/routing.pyi` & `propan-0.1.5.1/propan/brokers/redis/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/redis/schemas.py` & `propan-0.1.5.1/propan/brokers/redis/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/sqs/routing.pyi` & `propan-0.1.5.1/propan/brokers/sqs/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/sqs/schema.py` & `propan-0.1.5.1/propan/brokers/sqs/schema.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/sqs/sqs_broker.py` & `propan-0.1.5.1/propan/brokers/sqs/sqs_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/brokers/sqs/sqs_broker.pyi` & `propan-0.1.5.1/propan/brokers/sqs/sqs_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/cli/app.py` & `propan-0.1.5.1/propan/cli/app.py`

 * *Files 19% similar despite different names*

```diff
@@ -60,37 +60,44 @@
         self.title = title
         self.version = version
         self.description = description
         self.license = license
         self.contact = contact
 
     def set_broker(self, broker: Runnable) -> None:
+        """Set already existed App object broker
+        Usefull then you create/init broker in `on_startup` hook"""
         self.broker = broker
 
     def on_startup(
         self, func: Callable[P_HookParams, T_HookReturn]
     ) -> Callable[P_HookParams, T_HookReturn]:
+        """Add hook running BEFORE broker connected
+        This hook also takes an extra CLI options as a kwargs"""
         self._on_startup_calling.append(apply_types(func))
         return func
 
     def on_shutdown(
         self, func: Callable[P_HookParams, T_HookReturn]
     ) -> Callable[P_HookParams, T_HookReturn]:
+        """Add hook running BEFORE broker disconnected"""
         self._on_shutdown_calling.append(apply_types(func))
         return func
 
     def after_startup(
         self, func: Callable[P_HookParams, T_HookReturn]
     ) -> Callable[P_HookParams, T_HookReturn]:
+        """Add hook running AFTER broker connected"""
         self._after_startup_calling.append(apply_types(func))
         return func
 
     def after_shutdown(
         self, func: Callable[P_HookParams, T_HookReturn]
     ) -> Callable[P_HookParams, T_HookReturn]:
+        """Add hook running AFTER broker disconnected"""
         self._after_shutdown_calling.append(apply_types(func))
         return func
 
     def _log(self, level: int, message: str) -> None:
         if self.logger is not None:
             self.logger.log(level, message)
 
@@ -110,14 +117,29 @@
         # AsyncAPI args,
         title: str = "Propan",
         version: str = "0.1.0",
         description: str = "",
         license: Optional[AsyncAPILicense] = None,
         contact: Optional[AsyncAPIContact] = None,
     ):
+        """Asyncronous Propan Application class
+
+        stores and run broker, control hooks
+
+        Args:
+            broker: async broker to run (may be `None`, then specify by `set_broker`)
+            logger: logger object to log startup/shutdown messages (`None` to disable)
+
+        AsyncAPI Args:
+            title: application title
+            version: application version
+            description: application description
+            license: application license
+            contact: application contact
+        """
         super().__init__(
             broker=broker,
             logger=logger,
             title=title,
             version=version,
             description=description,
             license=license,
@@ -127,32 +149,74 @@
         self._stop_event = None
 
         set_exit(lambda *_: self.__exit())
 
     def on_startup(
         self, func: Callable[P_HookParams, T_HookReturn]
     ) -> Callable[P_HookParams, Awaitable[T_HookReturn]]:
+        """Add hook running BEFORE broker connected
+
+        This hook also takes an extra CLI options as a kwargs
+
+        Args:
+            func: async or sync func to call as a hook
+
+        Returns:
+            Async version of the func argument
+        """
         return super().on_startup(to_async(func))
 
     def on_shutdown(
         self, func: Callable[P_HookParams, Awaitable[T_HookReturn]]
     ) -> AsyncFunc:
+        """Add hook running BEFORE broker disconnected
+
+        Args:
+            func: async or sync func to call as a hook
+
+        Returns:
+            Async version of the func argument
+        """
         return super().on_shutdown(to_async(func))
 
     def after_startup(
         self, func: Callable[P_HookParams, Awaitable[T_HookReturn]]
     ) -> AsyncFunc:
+        """Add hook running AFTER broker connected
+
+        Args:
+            func: async or sync func to call as a hook
+
+        Returns:
+            Async version of the func argument
+        """
         return super().after_startup(to_async(func))
 
     def after_shutdown(
         self, func: Callable[P_HookParams, Awaitable[T_HookReturn]]
     ) -> AsyncFunc:
+        """Add hook running AFTER broker disconnected
+
+        Args:
+            func: async or sync func to call as a hook
+
+        Returns:
+            Async version of the func argument
+        """
         return super().after_shutdown(to_async(func))
 
     async def run(self, log_level: int = logging.INFO) -> None:
+        """Run Propan Application
+
+        Args:
+            log_level: force application log level
+
+        Returns:
+            Block an event loop until stopped
+        """
         self._init_async_cycle()
         async with anyio.create_task_group() as tg:
             tg.start_soon(self._start, log_level)
             await self._stop(log_level)
             tg.cancel_scope.cancel()
 
     def _init_async_cycle(self) -> None:
```

### Comparing `propan-0.1.5.0/propan/cli/main.py` & `propan-0.1.5.1/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/cli/docs/app.py` & `propan-0.1.5.1/propan/cli/docs/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/cli/docs/gen.py` & `propan-0.1.5.1/propan/cli/docs/gen.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/cli/docs/serving.py` & `propan-0.1.5.1/propan/cli/docs/serving.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/cli/startproject/core.py` & `propan-0.1.5.1/propan/cli/startproject/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/cli/startproject/async_app/app.py` & `propan-0.1.5.1/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/cli/startproject/async_app/core.py` & `propan-0.1.5.1/propan/cli/startproject/async_app/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/cli/startproject/async_app/kafka.py` & `propan-0.1.5.1/propan/cli/startproject/async_app/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/cli/startproject/async_app/nats.py` & `propan-0.1.5.1/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.5.1/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/cli/startproject/async_app/redis.py` & `propan-0.1.5.1/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/cli/startproject/async_app/sqs.py` & `propan-0.1.5.1/propan/cli/startproject/async_app/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/cli/supervisors/basereload.py` & `propan-0.1.5.1/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/cli/supervisors/multiprocess.py` & `propan-0.1.5.1/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/cli/supervisors/utils.py` & `propan-0.1.5.1/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/cli/supervisors/watchfiles.py` & `propan-0.1.5.1/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/cli/utils/imports.py` & `propan-0.1.5.1/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/cli/utils/logs.py` & `propan-0.1.5.1/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/cli/utils/parser.py` & `propan-0.1.5.1/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/fastapi/__init__.py` & `propan-0.1.5.1/propan/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/fastapi/core/route.py` & `propan-0.1.5.1/propan/fastapi/core/route.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/fastapi/core/router.py` & `propan-0.1.5.1/propan/fastapi/core/router.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/fastapi/kafka/router.pyi` & `propan-0.1.5.1/propan/fastapi/kafka/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/fastapi/nats/router.pyi` & `propan-0.1.5.1/propan/fastapi/nats/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/fastapi/rabbit/router.pyi` & `propan-0.1.5.1/propan/fastapi/rabbit/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/fastapi/redis/router.pyi` & `propan-0.1.5.1/propan/fastapi/redis/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/fastapi/sqs/router.pyi` & `propan-0.1.5.1/propan/fastapi/sqs/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/log/formatter.py` & `propan-0.1.5.1/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/log/logging.py` & `propan-0.1.5.1/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/test/__init__.py` & `propan-0.1.5.1/propan/test/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/test/kafka.py` & `propan-0.1.5.1/propan/test/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/test/nats.py` & `propan-0.1.5.1/propan/test/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/test/rabbit.py` & `propan-0.1.5.1/propan/test/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/test/redis.py` & `propan-0.1.5.1/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/test/sqs.py` & `propan-0.1.5.1/propan/test/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/test/utils.py` & `propan-0.1.5.1/propan/test/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/utils/functions.py` & `propan-0.1.5.1/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/utils/context/main.py` & `propan-0.1.5.1/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/propan/utils/context/types.py` & `propan-0.1.5.1/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/LICENSE` & `propan-0.1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/README.md` & `propan-0.1.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     <a href="https://github.com/Lancetnik/Propan/blob/main/LICENSE" target="_blank">
         <img alt="GitHub" src="https://img.shields.io/github/license/Lancetnik/Propan?color=%23007ec6">
     </a>
 </p>
 
 # Propan
 
-**Propan** - just *~~an another one HTTP~~* a **declarative Python MQ framework**. It's following by <a href="https://FastAPI.tiangolo.com/ru/" target="_blank">*FastAPI*</a>, simplify Message Brokers around code writing and provides a helpful development toolkit, which existed only in HTTP-frameworks world until now.
+**Propan** - just *~~an another one HTTP~~* a **declarative Python Messaging Framework**. It's inspired by <a href="https://FastAPI.tiangolo.com/ru/" target="_blank">*FastAPI*</a>, simplify Message Brokers around code writing and provides a helpful development toolkit, which existed only in HTTP-frameworks world until now.
 
 It's designed to create reactive microservices around <a href="https://microservices.io/patterns/communication-style/messaging.html" target="_blank">Messaging Architecture</a>.
 
 It is a modern, high-level framework on top of popular specific Python brokers libraries, based on <a href="https://docs.pydantic.dev/" target="_blank">*pydantic*</a> and <a href="https://FastAPI.tiangolo.com/ru/" target="_blank">*FastAPI*</a>, <a href="https://docs.pytest.org/en/latest/" target="_blank">*pytest*</a> concepts.
 
 ---
 
@@ -66,37 +66,37 @@
 |-------------------|:-------------------------------------------------------:|:-------------------------------------------:|
 | **RabbitMQ**      | :heavy_check_mark: **stable** :heavy_check_mark:        | :hammer_and_wrench: WIP :hammer_and_wrench: |
 | **Redis**         | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag:                        |
 | **Nats**          | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag:                        |
 | **Kafka**         | :warning: **beta** :warning:                            | :mag: planning :mag:                        |
 | **SQS**           | :warning: **beta** :warning:                            | :mag: planning :mag:                        |
 | **NatsJS**        | :warning: **beta** :warning:                            | :mag: planning :mag:                        |
+| **ZeroMQ**        | :hammer_and_wrench: WIP :hammer_and_wrench:             | :mag: planning :mag:                        |
 | **MQTT**          | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 | **Redis Streams** | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 | **Pulsar**        | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 | **ActiveMQ**      | :mag: planning :mag:                                    | :mag: planning :mag:                        |
-| **ZeroMQ**        | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 
 ---
 
 ### ⭐ Support the project ⭐
 
 If you are interested in this project, please give me feedback by:
 
 - giving the [repository](https://github.com/Lancetnik/Propan) a star
 
-- tweet about <a href="https://twitter.com/PropanFramework" target="_blank">**Propan**</a> and let me and others know why you use it.
+- tweet about <a href="https://twitter.com/compose/tweet?text=I'm like @PropanFramework because... https://github.com/Lancetnik/Propan" class="external-link" target="_blank">**Propan**</a> and let me and others know why you use it
 
-- joining <a href="https://discord.gg/ChhMXJpvz7" target="_blank">Discord server</a>.
+- joining <a href="https://discord.gg/ChhMXJpvz7" target="_blank">Discord server</a>
 
-Your support helps me to stay in touch with you and encourages us to
+Your support helps me to stay in touch with you and encourages to
 continue developing and improving the library. Thank you for your
 support!
 
-Really, share information about this project with overs. The bigger community we have - the better project will be!
+Really, share information about this project with others. The bigger community we have - the better project will be!
 
 ---
 
 ## Declarative?
 
 With declarative tools you can define **what you need to get**. With traditional imperative tools you must write **what you need to do**.
 
@@ -132,15 +132,14 @@
 
 It is not a bad way, but it can be much easier.
 
 ```python
 from propan import PropanApp, RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
-
 app = PropanApp(broker)
 
 @broker.handle("test_queue")
 async def base_handler(body):
     print(body)
 ```
 
@@ -259,15 +258,17 @@
 
 @broker.handle("ping")
 async def base_handler():
     return "pong"
 
 @app.after_startup
 async def self_ping():
-    assert (await broker.publish("", "ping")) == "pong"
+    assert (
+        await broker.publish("", "ping", callback=True)
+    ) == "pong"
 ```
 
 ---
 
 ## Project Documentation
 
 **Propan** automatically generates documentation for your project according to the <a href="https://www.asyncapi.com/" target="_blank">**AsyncAPI**</a> specification. You can work with both generated artifacts and place a Web view of your documentation on resources available to related teams.
@@ -374,26 +375,25 @@
 
 ```python
 from fastapi import Depends, FastAPI
 from pydantic import BaseModel
 from propan.fastapi import RabbitRouter
 
 router = RabbitRouter("amqp://guest:guest@localhost:5672")
-
 app = FastAPI(lifespan=router.lifespan_context)
 
 class Incoming(BaseModel):
-    m: dict
+    username: str
 
 def call():
     return True
 
 @router.event("test")
-async def hello(m: Incoming, d = Depends(call)) -> dict:
-    return { "response": "Hello, Propan!" }
+async def hello(m: Incoming, d = Depends(call)):
+    return { "response": f"Hello, {m.username}!" }
 
 app.include_router(router)
 ```
 
 ## Examples
 
 To see more framework usages go to [**examples/**](https://github.com/Lancetnik/Propan/tree/main/examples)
```

#### html2text {}

```diff
@@ -1,143 +1,144 @@
                                  [Propan_logo]
           [Tests_coverage] [Coverage] [Package_version] [downloads]
                      [Supported_Python_versions] [GitHub]
-# Propan **Propan** - just *~~an another one HTTP~~* a **declarative Python MQ
-framework**. It's following by *FastAPI*, simplify Message Brokers around code
-writing and provides a helpful development toolkit, which existed only in HTTP-
-frameworks world until now. It's designed to create reactive microservices
-around Messaging_Architecture. It is a modern, high-level framework on top of
-popular specific Python brokers libraries, based on *pydantic* and *FastAPI*,
-*pytest* concepts. --- **Documentation**: https://lancetnik.github.io/Propan/ -
--- ### The key features are * **Simple**: Designed to be easy to use and learn.
-* **Intuitive**: Great editor support. Autocompletion everywhere. *
-[**Dependencies management**](#dependencies): Minimization of code duplication.
-Access to dependencies at any level of the call stack. * [**Integrations**]
-(#http-frameworks-integrations): **Propan** is fully compatible with any_HTTP
-framework you want * **MQ independent**: Single interface to popular MQ: *
-**Redis** (based on redis-py) * **RabbitMQ** (based on aio-pika) * **Kafka**
-(based on aiokafka) * **SQS** (based on aiobotocore) * **Nats** (based on nats-
-py) * **RPC**: The framework supports RPC requests over MQ, which will allow
-performing long operations on remote services asynchronously. * [**Great to
-develop**](#cli-power): CLI tool provides great development experience: *
-framework-independent way to manage the project environment * application code
-*hot reload* * robust application templates * [**Documentation**](#project-
-documentation): **Propan** automatically generates and presents an interactive
-**AsyncAPI** documentation for your project * **Testability**: **Propan**
-allows you to test your app without external dependencies: you do not have to
-set up a Message Broker, you can use a virtual one! ### Supported MQ brokers |
-| async | sync | |-------------------|:----------------------------------------
----------------:|:-------------------------------------------:| | **RabbitMQ**
-| :heavy_check_mark: **stable** :heavy_check_mark: | :hammer_and_wrench: WIP :
-hammer_and_wrench: | | **Redis** | :heavy_check_mark: **stable** :
-heavy_check_mark: | :mag: planning :mag: | | **Nats** | :heavy_check_mark:
-**stable** :heavy_check_mark: | :mag: planning :mag: | | **Kafka** | :warning:
-**beta** :warning: | :mag: planning :mag: | | **SQS** | :warning: **beta** :
-warning: | :mag: planning :mag: | | **NatsJS** | :warning: **beta** :warning: |
-:mag: planning :mag: | | **MQTT** | :mag: planning :mag: | :mag: planning :mag:
-| | **Redis Streams** | :mag: planning :mag: | :mag: planning :mag: | |
-**Pulsar** | :mag: planning :mag: | :mag: planning :mag: | | **ActiveMQ** | :
-mag: planning :mag: | :mag: planning :mag: | | **ZeroMQ** | :mag: planning :
-mag: | :mag: planning :mag: | --- ### â­ Support the project â­ If you are
-interested in this project, please give me feedback by: - giving the
-[repository](https://github.com/Lancetnik/Propan) a star - tweet about
-**Propan** and let me and others know why you use it. - joining Discord_server.
-Your support helps me to stay in touch with you and encourages us to continue
-developing and improving the library. Thank you for your support! Really, share
-information about this project with overs. The bigger community we have - the
-better project will be! --- ## Declarative? With declarative tools you can
-define **what you need to get**. With traditional imperative tools you must
-write **what you need to do**. Take a look at classic imperative tools, such as
-aio-pika, pika, redis-py, nats-py, etc. This is the **Quickstart** with the
-*aio-pika*: ```python import asyncio import aio_pika async def main():
-connection = await aio_pika.connect_robust( "amqp://guest:guest@127.0.0.1/" )
-queue_name = "test_queue" async with connection: channel = await
-connection.channel() queue = await channel.declare_queue(queue_name) async with
-queue.iterator() as queue_iter: async for message in queue_iter: async with
-message.process(): print(message.body) asyncio.run(main()) ``` **aio-pika** is
-a great tool with a really easy learning curve. But it's still imperative. You
-need to *connect*, declare *channel*, *queues*, *exchanges* by yourself. Also,
-you need to manage *connection*, *message*, *queue* context to avoid any
-troubles. It is not a bad way, but it can be much easier. ```python from propan
-import PropanApp, RabbitBroker broker = RabbitBroker("amqp://guest:
-guest@localhost:5672/") app = PropanApp(broker) @broker.handle("test_queue")
-async def base_handler(body): print(body) ``` This is the **Propan**
-declarative way to write the same code. That is so much easier, isn't it? --
-- ## Quickstart Install using `pip`: ```shell pip install "propan[async-
-rabbit]" # or pip install "propan[async-nats]" # or pip install "propan[async-
-redis]" # or pip install "propan[async-kafka]" # or pip install "propan[async-
-sqs]" ``` ### Basic usage Create an application with the following code at
-`serve.py`: ```python from propan import PropanApp from propan import
-RabbitBroker # from propan import RedisBroker # from propan import NatsBroker #
-from propan import SQSBroker # from propan import KafkaBroker broker =
-RabbitBroker("amqp://guest:guest@localhost:5672/") # broker = NatsBroker("nats:
-//localhost:4222") # broker = RedisBroker("redis://localhost:6379") # broker =
-SQSBroker("http://localhost:9324", ...) # broker = KafkaBroker("localhost:
-9092") app = PropanApp(broker) @broker.handle("test") async def base_handler
-(body): print(body) ``` And just run it: ```shell propan run serve:app --
-workers 3 ``` --- ## Type casting Propan uses `pydantic` to cast incoming
-function arguments to types according to their annotation. ```python from
-pydantic import BaseModel from propan import PropanApp, RabbitBroker broker =
-RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp(broker)
-class SimpleMessage(BaseModel): key: int @broker.handle("test2") async def
-second_handler(body: SimpleMessage): assert isinstance(body.key, int) ``` --
-- ## Dependencies **Propan** a has dependencies management policy close to
-`pytest fixtures`. You can specify in functions arguments which dependencies
-you would to use. Framework passes them from the global Context object. Also,
-you can specify your own dependencies, call dependencies functions (like
-`FastAPI Depends`) and [more](https://github.com/Lancetnik/Propan/tree/main/
-examples/dependencies). ```python from propan import PropanApp, RabbitBroker,
-Context, Depends rabbit_broker = RabbitBroker("amqp://guest:guest@localhost:
-5672/") app = PropanApp(rabbit_broker) async def dependency(user_id: int) -
-> bool: return True @rabbit_broker.handle("test") async def base_handler
-(user_id: int, dep: bool = Depends(dependency), broker: RabbitBroker = Context
-()): assert dep is True assert broker is rabbit_broker ``` --- ## RPC over MQ
-Also, **Propan** allows you to use **RPC** requests over your broker with a
-simple way: ```python from propan import PropanApp, RabbitBroker broker =
-RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp
-(rabbit_broker) @broker.handle("ping") async def base_handler(): return "pong"
-@app.after_startup async def self_ping(): assert (await broker.publish("",
-"ping")) == "pong" ``` --- ## Project Documentation **Propan** automatically
-generates documentation for your project according to the **AsyncAPI**
-specification. You can work with both generated artifacts and place a Web view
-of your documentation on resources available to related teams. The availability
-of such documentation significantly simplifies the integration of services: you
-can immediately see what channels and message format the application works
-with. And most importantly, it doesn't cost you anything - **Propan** has
-already done everything for you! ![HTML-page](https://lancetnik.github.io/
-Propan/assets/img/docs-html-short.png) --- ## CLI power **Propan** has its own
-CLI tool that provided the following features: * project generation *
-multiprocessing workers * project hot reloading * documentation generating and
-hosting * custom command line arguments passing ### Context passing For
-example: pass your current *.env* project setting to context ```bash propan run
-serve:app --env=.env.dev ``` ```python from propan import PropanApp,
-RabbitBroker from propan.annotations import ContextRepo from pydantic import
-BaseSettings broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
-PropanApp(broker) class Settings(BaseSettings): ... @app.on_startup async def
-setup(env: str, context: ContextRepo): settings = Settings(_env_file=env)
-context.set_global("settings", settings) ``` ### Project template Also,
-**Propan CLI** is able to generate a production-ready application template:
-```bash propan create async rabbit [projectname] ``` *Notice: project template
-require* `pydantic[dotenv]` *installation.* Run the created project: ```bash #
-Run rabbimq first docker compose --file [projectname]/docker-compose.yaml up -
-d # Run project propan run [projectname].app.serve:app --env=.env --reload ```
-Now you can enjoy a new development experience! --- ## HTTP Frameworks
-integrations ### Any Framework You can use **Propan** `MQBrokers` without
-`PropanApp`. Just *start* and *stop* them according to your application
-lifespan. ```python from propan import NatsBroker from sanic import Sanic app =
-Sanic("MyHelloWorldApp") broker = NatsBroker("nats://localhost:4222")
-@broker.handle("test") async def base_handler(body): print(body)
-@app.after_server_start async def start_broker(app, loop): await broker.start()
-@app.after_server_stop async def stop_broker(app, loop): await broker.close()
-``` ### FastAPI Plugin Also, **Propan** can be used as part of **FastAPI**.
-Just import a **PropanRouter** you need and declare the message handler using
-the `@event` decorator. This decorator is similar to the decorator `@handle`
-for the corresponding brokers. ```python from fastapi import Depends, FastAPI
-from pydantic import BaseModel from propan.fastapi import RabbitRouter router =
-RabbitRouter("amqp://guest:guest@localhost:5672") app = FastAPI
-(lifespan=router.lifespan_context) class Incoming(BaseModel): m: dict def call
-(): return True @router.event("test") async def hello(m: Incoming, d = Depends
-(call)) -> dict: return { "response": "Hello, Propan!" } app.include_router
-(router) ``` ## Examples To see more framework usages go to [**examples/**]
-(https://github.com/Lancetnik/Propan/tree/main/examples) ## Contributors Thanks
-for all of these amazing peoples made the project better! [https://
-contrib.rocks/image?repo=Lancetnik/Propan]
+# Propan **Propan** - just *~~an another one HTTP~~* a **declarative Python
+Messaging Framework**. It's inspired by *FastAPI*, simplify Message Brokers
+around code writing and provides a helpful development toolkit, which existed
+only in HTTP-frameworks world until now. It's designed to create reactive
+microservices around Messaging_Architecture. It is a modern, high-level
+framework on top of popular specific Python brokers libraries, based on
+*pydantic* and *FastAPI*, *pytest* concepts. --- **Documentation**: https://
+lancetnik.github.io/Propan/ --- ### The key features are * **Simple**: Designed
+to be easy to use and learn. * **Intuitive**: Great editor support.
+Autocompletion everywhere. * [**Dependencies management**](#dependencies):
+Minimization of code duplication. Access to dependencies at any level of the
+call stack. * [**Integrations**](#http-frameworks-integrations): **Propan** is
+fully compatible with any_HTTP_framework you want * **MQ independent**: Single
+interface to popular MQ: * **Redis** (based on redis-py) * **RabbitMQ** (based
+on aio-pika) * **Kafka** (based on aiokafka) * **SQS** (based on aiobotocore) *
+**Nats** (based on nats-py) * **RPC**: The framework supports RPC requests over
+MQ, which will allow performing long operations on remote services
+asynchronously. * [**Great to develop**](#cli-power): CLI tool provides great
+development experience: * framework-independent way to manage the project
+environment * application code *hot reload* * robust application templates *
+[**Documentation**](#project-documentation): **Propan** automatically generates
+and presents an interactive **AsyncAPI** documentation for your project *
+**Testability**: **Propan** allows you to test your app without external
+dependencies: you do not have to set up a Message Broker, you can use a virtual
+one! ### Supported MQ brokers | | async | sync | |-------------------|:--------
+-----------------------------------------------:|:-----------------------------
+--------------:| | **RabbitMQ** | :heavy_check_mark: **stable** :
+heavy_check_mark: | :hammer_and_wrench: WIP :hammer_and_wrench: | | **Redis** |
+:heavy_check_mark: **stable** :heavy_check_mark: | :mag: planning :mag: | |
+**Nats** | :heavy_check_mark: **stable** :heavy_check_mark: | :mag: planning :
+mag: | | **Kafka** | :warning: **beta** :warning: | :mag: planning :mag: | |
+**SQS** | :warning: **beta** :warning: | :mag: planning :mag: | | **NatsJS** |
+:warning: **beta** :warning: | :mag: planning :mag: | | **ZeroMQ** | :
+hammer_and_wrench: WIP :hammer_and_wrench: | :mag: planning :mag: | | **MQTT**
+| :mag: planning :mag: | :mag: planning :mag: | | **Redis Streams** | :mag:
+planning :mag: | :mag: planning :mag: | | **Pulsar** | :mag: planning :mag: | :
+mag: planning :mag: | | **ActiveMQ** | :mag: planning :mag: | :mag: planning :
+mag: | --- ### â­ Support the project â­ If you are interested in this
+project, please give me feedback by: - giving the [repository](https://
+github.com/Lancetnik/Propan) a star - tweet about **Propan** and let me and
+others know why you use it - joining Discord_server Your support helps me to
+stay in touch with you and encourages to continue developing and improving the
+library. Thank you for your support! Really, share information about this
+project with others. The bigger community we have - the better project will be!
+--- ## Declarative? With declarative tools you can define **what you need to
+get**. With traditional imperative tools you must write **what you need to
+do**. Take a look at classic imperative tools, such as aio-pika, pika, redis-
+py, nats-py, etc. This is the **Quickstart** with the *aio-pika*: ```python
+import asyncio import aio_pika async def main(): connection = await
+aio_pika.connect_robust( "amqp://guest:guest@127.0.0.1/" ) queue_name =
+"test_queue" async with connection: channel = await connection.channel() queue
+= await channel.declare_queue(queue_name) async with queue.iterator() as
+queue_iter: async for message in queue_iter: async with message.process():
+print(message.body) asyncio.run(main()) ``` **aio-pika** is a great tool with a
+really easy learning curve. But it's still imperative. You need to *connect*,
+declare *channel*, *queues*, *exchanges* by yourself. Also, you need to manage
+*connection*, *message*, *queue* context to avoid any troubles. It is not a bad
+way, but it can be much easier. ```python from propan import PropanApp,
+RabbitBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
+PropanApp(broker) @broker.handle("test_queue") async def base_handler(body):
+print(body) ``` This is the **Propan** declarative way to write the same code.
+That is so much easier, isn't it? --- ## Quickstart Install using `pip`:
+```shell pip install "propan[async-rabbit]" # or pip install "propan[async-
+nats]" # or pip install "propan[async-redis]" # or pip install "propan[async-
+kafka]" # or pip install "propan[async-sqs]" ``` ### Basic usage Create an
+application with the following code at `serve.py`: ```python from propan import
+PropanApp from propan import RabbitBroker # from propan import RedisBroker #
+from propan import NatsBroker # from propan import SQSBroker # from propan
+import KafkaBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
+# broker = NatsBroker("nats://localhost:4222") # broker = RedisBroker("redis://
+localhost:6379") # broker = SQSBroker("http://localhost:9324", ...) # broker =
+KafkaBroker("localhost:9092") app = PropanApp(broker) @broker.handle("test")
+async def base_handler(body): print(body) ``` And just run it: ```shell propan
+run serve:app --workers 3 ``` --- ## Type casting Propan uses `pydantic` to
+cast incoming function arguments to types according to their annotation.
+```python from pydantic import BaseModel from propan import PropanApp,
+RabbitBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
+PropanApp(broker) class SimpleMessage(BaseModel): key: int @broker.handle
+("test2") async def second_handler(body: SimpleMessage): assert isinstance
+(body.key, int) ``` --- ## Dependencies **Propan** a has dependencies
+management policy close to `pytest fixtures`. You can specify in functions
+arguments which dependencies you would to use. Framework passes them from the
+global Context object. Also, you can specify your own dependencies, call
+dependencies functions (like `FastAPI Depends`) and [more](https://github.com/
+Lancetnik/Propan/tree/main/examples/dependencies). ```python from propan import
+PropanApp, RabbitBroker, Context, Depends rabbit_broker = RabbitBroker("amqp://
+guest:guest@localhost:5672/") app = PropanApp(rabbit_broker) async def
+dependency(user_id: int) -> bool: return True @rabbit_broker.handle("test")
+async def base_handler(user_id: int, dep: bool = Depends(dependency), broker:
+RabbitBroker = Context()): assert dep is True assert broker is rabbit_broker
+``` --- ## RPC over MQ Also, **Propan** allows you to use **RPC** requests over
+your broker with a simple way: ```python from propan import PropanApp,
+RabbitBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
+PropanApp(rabbit_broker) @broker.handle("ping") async def base_handler():
+return "pong" @app.after_startup async def self_ping(): assert ( await
+broker.publish("", "ping", callback=True) ) == "pong" ``` --- ## Project
+Documentation **Propan** automatically generates documentation for your project
+according to the **AsyncAPI** specification. You can work with both generated
+artifacts and place a Web view of your documentation on resources available to
+related teams. The availability of such documentation significantly simplifies
+the integration of services: you can immediately see what channels and message
+format the application works with. And most importantly, it doesn't cost you
+anything - **Propan** has already done everything for you! ![HTML-page](https:/
+/lancetnik.github.io/Propan/assets/img/docs-html-short.png) --- ## CLI power
+**Propan** has its own CLI tool that provided the following features: * project
+generation * multiprocessing workers * project hot reloading * documentation
+generating and hosting * custom command line arguments passing ### Context
+passing For example: pass your current *.env* project setting to context
+```bash propan run serve:app --env=.env.dev ``` ```python from propan import
+PropanApp, RabbitBroker from propan.annotations import ContextRepo from
+pydantic import BaseSettings broker = RabbitBroker("amqp://guest:
+guest@localhost:5672/") app = PropanApp(broker) class Settings(BaseSettings):
+... @app.on_startup async def setup(env: str, context: ContextRepo): settings =
+Settings(_env_file=env) context.set_global("settings", settings) ``` ###
+Project template Also, **Propan CLI** is able to generate a production-ready
+application template: ```bash propan create async rabbit [projectname] ```
+*Notice: project template require* `pydantic[dotenv]` *installation.* Run the
+created project: ```bash # Run rabbimq first docker compose --file
+[projectname]/docker-compose.yaml up -d # Run project propan run
+[projectname].app.serve:app --env=.env --reload ``` Now you can enjoy a new
+development experience! --- ## HTTP Frameworks integrations ### Any Framework
+You can use **Propan** `MQBrokers` without `PropanApp`. Just *start* and *stop*
+them according to your application lifespan. ```python from propan import
+NatsBroker from sanic import Sanic app = Sanic("MyHelloWorldApp") broker =
+NatsBroker("nats://localhost:4222") @broker.handle("test") async def
+base_handler(body): print(body) @app.after_server_start async def start_broker
+(app, loop): await broker.start() @app.after_server_stop async def stop_broker
+(app, loop): await broker.close() ``` ### FastAPI Plugin Also, **Propan** can
+be used as part of **FastAPI**. Just import a **PropanRouter** you need and
+declare the message handler using the `@event` decorator. This decorator is
+similar to the decorator `@handle` for the corresponding brokers. ```python
+from fastapi import Depends, FastAPI from pydantic import BaseModel from
+propan.fastapi import RabbitRouter router = RabbitRouter("amqp://guest:
+guest@localhost:5672") app = FastAPI(lifespan=router.lifespan_context) class
+Incoming(BaseModel): username: str def call(): return True @router.event
+("test") async def hello(m: Incoming, d = Depends(call)): return { "response":
+f"Hello, {m.username}!" } app.include_router(router) ``` ## Examples To see
+more framework usages go to [**examples/**](https://github.com/Lancetnik/
+Propan/tree/main/examples) ## Contributors Thanks for all of these amazing
+peoples made the project better! [https://contrib.rocks/image?repo=Lancetnik/
+Propan]
```

### Comparing `propan-0.1.5.0/pyproject.toml` & `propan-0.1.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.0/PKG-INFO` & `propan-0.1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.5.0
+Version: 0.1.5.1
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
@@ -118,15 +118,15 @@
     <a href="https://github.com/Lancetnik/Propan/blob/main/LICENSE" target="_blank">
         <img alt="GitHub" src="https://img.shields.io/github/license/Lancetnik/Propan?color=%23007ec6">
     </a>
 </p>
 
 # Propan
 
-**Propan** - just *~~an another one HTTP~~* a **declarative Python MQ framework**. It's following by <a href="https://FastAPI.tiangolo.com/ru/" target="_blank">*FastAPI*</a>, simplify Message Brokers around code writing and provides a helpful development toolkit, which existed only in HTTP-frameworks world until now.
+**Propan** - just *~~an another one HTTP~~* a **declarative Python Messaging Framework**. It's inspired by <a href="https://FastAPI.tiangolo.com/ru/" target="_blank">*FastAPI*</a>, simplify Message Brokers around code writing and provides a helpful development toolkit, which existed only in HTTP-frameworks world until now.
 
 It's designed to create reactive microservices around <a href="https://microservices.io/patterns/communication-style/messaging.html" target="_blank">Messaging Architecture</a>.
 
 It is a modern, high-level framework on top of popular specific Python brokers libraries, based on <a href="https://docs.pydantic.dev/" target="_blank">*pydantic*</a> and <a href="https://FastAPI.tiangolo.com/ru/" target="_blank">*FastAPI*</a>, <a href="https://docs.pytest.org/en/latest/" target="_blank">*pytest*</a> concepts.
 
 ---
 
@@ -160,37 +160,37 @@
 |-------------------|:-------------------------------------------------------:|:-------------------------------------------:|
 | **RabbitMQ**      | :heavy_check_mark: **stable** :heavy_check_mark:        | :hammer_and_wrench: WIP :hammer_and_wrench: |
 | **Redis**         | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag:                        |
 | **Nats**          | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag:                        |
 | **Kafka**         | :warning: **beta** :warning:                            | :mag: planning :mag:                        |
 | **SQS**           | :warning: **beta** :warning:                            | :mag: planning :mag:                        |
 | **NatsJS**        | :warning: **beta** :warning:                            | :mag: planning :mag:                        |
+| **ZeroMQ**        | :hammer_and_wrench: WIP :hammer_and_wrench:             | :mag: planning :mag:                        |
 | **MQTT**          | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 | **Redis Streams** | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 | **Pulsar**        | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 | **ActiveMQ**      | :mag: planning :mag:                                    | :mag: planning :mag:                        |
-| **ZeroMQ**        | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 
 ---
 
 ### ⭐ Support the project ⭐
 
 If you are interested in this project, please give me feedback by:
 
 - giving the [repository](https://github.com/Lancetnik/Propan) a star
 
-- tweet about <a href="https://twitter.com/PropanFramework" target="_blank">**Propan**</a> and let me and others know why you use it.
+- tweet about <a href="https://twitter.com/compose/tweet?text=I'm like @PropanFramework because... https://github.com/Lancetnik/Propan" class="external-link" target="_blank">**Propan**</a> and let me and others know why you use it
 
-- joining <a href="https://discord.gg/ChhMXJpvz7" target="_blank">Discord server</a>.
+- joining <a href="https://discord.gg/ChhMXJpvz7" target="_blank">Discord server</a>
 
-Your support helps me to stay in touch with you and encourages us to
+Your support helps me to stay in touch with you and encourages to
 continue developing and improving the library. Thank you for your
 support!
 
-Really, share information about this project with overs. The bigger community we have - the better project will be!
+Really, share information about this project with others. The bigger community we have - the better project will be!
 
 ---
 
 ## Declarative?
 
 With declarative tools you can define **what you need to get**. With traditional imperative tools you must write **what you need to do**.
 
@@ -226,15 +226,14 @@
 
 It is not a bad way, but it can be much easier.
 
 ```python
 from propan import PropanApp, RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
-
 app = PropanApp(broker)
 
 @broker.handle("test_queue")
 async def base_handler(body):
     print(body)
 ```
 
@@ -353,15 +352,17 @@
 
 @broker.handle("ping")
 async def base_handler():
     return "pong"
 
 @app.after_startup
 async def self_ping():
-    assert (await broker.publish("", "ping")) == "pong"
+    assert (
+        await broker.publish("", "ping", callback=True)
+    ) == "pong"
 ```
 
 ---
 
 ## Project Documentation
 
 **Propan** automatically generates documentation for your project according to the <a href="https://www.asyncapi.com/" target="_blank">**AsyncAPI**</a> specification. You can work with both generated artifacts and place a Web view of your documentation on resources available to related teams.
@@ -468,26 +469,25 @@
 
 ```python
 from fastapi import Depends, FastAPI
 from pydantic import BaseModel
 from propan.fastapi import RabbitRouter
 
 router = RabbitRouter("amqp://guest:guest@localhost:5672")
-
 app = FastAPI(lifespan=router.lifespan_context)
 
 class Incoming(BaseModel):
-    m: dict
+    username: str
 
 def call():
     return True
 
 @router.event("test")
-async def hello(m: Incoming, d = Depends(call)) -> dict:
-    return { "response": "Hello, Propan!" }
+async def hello(m: Incoming, d = Depends(call)):
+    return { "response": f"Hello, {m.username}!" }
 
 app.include_router(router)
 ```
 
 ## Examples
 
 To see more framework usages go to [**examples/**](https://github.com/Lancetnik/Propan/tree/main/examples)
```

