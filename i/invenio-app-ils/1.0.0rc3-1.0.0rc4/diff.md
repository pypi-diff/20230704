# Comparing `tmp/invenio-app-ils-1.0.0rc3.tar.gz` & `tmp/invenio-app-ils-1.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-app-ils-1.0.0rc3.tar", last modified: Fri Mar 10 14:18:05 2023, max compression
+gzip compressed data, was "dist/invenio-app-ils-1.0.0rc4.tar", last modified: Tue Jul  4 15:45:12 2023, max compression
```

## Comparing `invenio-app-ils-1.0.0rc3.tar` & `invenio-app-ils-1.0.0rc4.tar`

### file list

```diff
@@ -1,788 +1,790 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/docker/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/docker/backend/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docker/backend/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/docker/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docker/frontend/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/docker/frontend/conf.d/
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docker/frontend/conf.d/default.conf
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docker/frontend/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docker/frontend/test.crt
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docker/frontend/test.key
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/docker/lb/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docker/lb/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docker/lb/haproxy.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docker/lb/haproxy_cert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docker-compose.full.yml
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docker-services.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/jsonresolvers/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/jsonresolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/jsonresolvers/order_order_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/jsonresolvers/order_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/loaders/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/loaders/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/loaders/jsonschemas/order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/mappings/os-v1/acq_orders/
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/mappings/os-v1/acq_orders/order-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/mappings/os-v2/acq_orders/
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/mappings/os-v2/acq_orders/order-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/mappings/v7/acq_orders/
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/mappings/v7/acq_orders/order-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/schemas/acq_orders/
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/schemas/acq_orders/order-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/jsonresolvers/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/jsonresolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/jsonresolvers/loan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/loaders/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/loaders/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/loaders/schemas/json/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/loaders/schemas/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/loaders/schemas/json/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/loaders/schemas/json/bulk_extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/loaders/schemas/json/loan_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/loaders/schemas/json/loan_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/loaders/schemas/json/loan_update_dates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/notifications/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/notifications/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/notifications/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/receivers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/serializers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/serializers/custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/serializers/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/stats/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/stats/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/bulk_extend.html
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/cancel.html
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/checkin.html
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/checkout.html
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/extend.html
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/overdue_reminder.html
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/request.html
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/request_no_items.html
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/will_expire_in_reminder.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/transitions/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/transitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/transitions/transitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    57138 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/closures/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/closures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/closures/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/closures/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    40830 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/demo_data/
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/demo_data/documents.json
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/demo_data/items.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/jsonresolvers/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/jsonresolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/jsonresolvers/document_request_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/jsonresolvers/document_request_patron.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/loaders/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/loaders/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/loaders/jsonschemas/document_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_decline.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_document.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/mappings/os-v1/document_requests/
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/mappings/os-v1/document_requests/document_request-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/mappings/os-v2/document_requests/
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/mappings/os-v2/document_requests/document_request-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/mappings/v7/document_requests/
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/mappings/v7/document_requests/document_request-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/notifications/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/notifications/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/schemas/document_requests/
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/schemas/document_requests/document_request-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_accept.html
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_decline_in_catalog.html
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_decline_not_found.html
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_decline_other.html
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_decline_user_cancel.html
--rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/jsonresolvers/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/jsonresolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/jsonresolvers/document_circulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/jsonresolvers/document_eitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/jsonresolvers/document_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/jsonresolvers/document_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/jsonresolvers/document_stock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/loaders/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/loaders/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/loaders/jsonschemas/document.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/mappings/os-v1/documents/
--rw-r--r--   0 runner    (1001) docker     (123)    21341 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/mappings/os-v1/documents/document-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/mappings/os-v2/documents/
--rw-r--r--   0 runner    (1001) docker     (123)    21341 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/mappings/os-v2/documents/document-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/mappings/v7/documents/
--rw-r--r--   0 runner    (1001) docker     (123)    21341 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/mappings/v7/documents/document-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/schemas/documents/
--rw-r--r--   0 runner    (1001) docker     (123)    18138 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/schemas/documents/document-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/jsonresolvers/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/jsonresolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/jsonresolvers/eitem_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/jsonresolvers/eitem_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/loaders/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/loaders/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/loaders/jsonschemas/eitems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/mappings/os-v1/eitems/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/mappings/os-v1/eitems/eitem-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/mappings/os-v2/eitems/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/mappings/os-v2/eitems/eitem-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/mappings/v7/eitems/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/mappings/v7/eitems/eitem-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/schemas/eitems/
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/schemas/eitems/eitem-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/fetchers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/files/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/files/receivers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/files/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/jsonresolvers/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/jsonresolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/jsonresolvers/borrowing_request_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/jsonresolvers/borrowing_request_patron.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/jsonresolvers/borrowing_request_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/loaders/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/loaders/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/loaders/jsonschemas/borrowing_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/loaders/jsonschemas/patron_loan_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/loaders/jsonschemas/patron_loan_extension_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/mappings/os-v1/ill_borrowing_requests/
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/mappings/os-v1/ill_borrowing_requests/borrowing_request-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/mappings/os-v2/ill_borrowing_requests/
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/mappings/os-v2/ill_borrowing_requests/borrowing_request-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/mappings/v7/ill_borrowing_requests/
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/mappings/v7/ill_borrowing_requests/borrowing_request-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/notifications/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/notifications/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/schemas/ill_borrowing_requests/
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/schemas/ill_borrowing_requests/borrowing_request-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/serializers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/serializers/custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/serializers/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/templates/invenio_app_ils_ill/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_accept.html
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_decline.html
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_request.html
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/jsonresolvers/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/jsonresolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/jsonresolvers/internal_location.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/loaders/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/loaders/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/loaders/jsonschemas/internal_location.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/mappings/os-v1/internal_locations/
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/mappings/os-v1/internal_locations/internal_location-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/mappings/os-v2/internal_locations/
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/mappings/os-v2/internal_locations/internal_location-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/mappings/v7/internal_locations/
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/mappings/v7/internal_locations/internal_location-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/schemas/internal_locations/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/schemas/internal_locations/internal_location-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/jsonresolvers/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/jsonresolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/jsonresolvers/item_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/jsonresolvers/item_internal_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/jsonresolvers/item_loan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/loaders/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/loaders/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/loaders/jsonschemas/items.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/mappings/os-v1/items/
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/mappings/os-v1/items/item-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/mappings/os-v2/items/
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/mappings/os-v2/items/item-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/mappings/v7/items/
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/mappings/v7/items/item-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/schemas/items/
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/schemas/items/item-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/items/serializers/item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/literature/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/literature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/literature/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/literature/covers_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/literature/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/literature/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/literature/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/literature/serializers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/literature/serializers/custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/literature/serializers/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/loaders/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/loaders/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/loaders/jsonschemas/location.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/mappings/os-v1/locations/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/mappings/os-v1/locations/location-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/mappings/os-v2/locations/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/mappings/os-v2/locations/location-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/mappings/v7/locations/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/mappings/v7/locations/location-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/receivers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/schemas/locations/
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/schemas/locations/location-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/minters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/notifications/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/notifications/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/notifications/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/notifications/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/notifications/backends/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/notifications/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/notifications/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/notifications/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/notifications/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/anonymization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/mappings/os-v1/patrons/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/mappings/os-v1/patrons/patron-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/mappings/os-v2/patrons/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/mappings/os-v2/patrons/patron-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/mappings/v7/patrons/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/mappings/v7/patrons/patron-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/loaders/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/loaders/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/loaders/jsonschemas/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/mappings/os-v1/providers/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/mappings/os-v1/providers/provider-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/mappings/os-v2/providers/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/mappings/os-v2/providers/provider-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/mappings/v7/providers/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/mappings/v7/providers/provider-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/schemas/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/schemas/providers/provider-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/jsonresolvers/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/jsonresolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/jsonresolvers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/listeners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/loaders/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/loaders/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/loaders/schemas/changed_by.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/loaders/schemas/preserve_cover_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/loaders/schemas/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/metadata_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/receivers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/schemas/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records_relations/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records_relations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records_relations/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records_relations/indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records_relations/retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)    14889 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/records_relations/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/relations/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/relations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13996 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/relations/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/relations/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/search_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/jsonresolvers/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/jsonresolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/jsonresolvers/series_relations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/loaders/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/loaders/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/loaders/jsonschemas/series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/mappings/os-v1/series/
--rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/mappings/os-v1/series/series-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/mappings/os-v2/series/
--rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/mappings/os-v2/series/series-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/mappings/v7/series/
--rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/mappings/v7/series/series-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/schemas/series/
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/schemas/series/series-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/series/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/static/images/placeholder.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/static_pages/
--rw-r--r--   0 runner    (1001) docker     (123)    22084 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/static_pages/search_guide.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/aggregations/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/aggregations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/aggregations/aggr_file_download/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/aggregations/aggr_file_download/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/aggregations/aggr_file_download/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/aggregations/aggr_file_download/os-v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/aggregations/aggr_file_download/os-v1/aggr-file-download-v1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/aggregations/aggr_file_download/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/aggregations/aggr_file_download/os-v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/aggregations/aggr_file_download/os-v2/aggr-file-download-v1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/aggregations/aggr_file_download/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/aggregations/aggr_file_download/v7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/aggregations/aggr_file_download/v7/aggr-file-download-v1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/file_download/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/file_download/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/file_download/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/file_download/os-v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/file_download/os-v1/file-download-v1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/file_download/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/file_download/os-v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/file_download/os-v2/file-download-v1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/file_download/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/file_download/v7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/file_download/v7/file-download-v1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/templates/invenio_app_ils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/templates/invenio_app_ils/mail/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/templates/invenio_app_ils/mail/footer.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/templates/invenio_app_ils/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/templates/invenio_app_ils/notifications/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/templates/logged_out.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/translations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/translations/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/acq_mediums.json
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/acq_order_line_payment_modes.json
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/acq_order_line_purchase_types.json
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/acq_payment_modes.json
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/acq_recipients.json
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/affiliation_identifier_schemes.json
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/alternative_identifier_schemes.json
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/alternative_title_types.json
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/author_identifier_schemes.json
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/author_roles.json
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/author_types.json
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/conference_identifier_schemes.json
--rw-r--r--   0 runner    (1001) docker     (123)    20498 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/countries.json
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/currencies.json
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/docreq_payment_method.json
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/docreq_request_type.json
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/document_identifiers_materials.json
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/document_requests_mediums.json
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/document_subjects.json
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/eitem_sources.json
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/identifier_schemes.json
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/ill_item_types.json
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/ill_payment_modes.json
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/item_mediums.json
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/provider_types.json
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/series_identifier_schemes.json
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/series_url_access_restrictions.json
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/jsonresolvers/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/jsonresolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/jsonresolvers/licenses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/mappings/os-v1/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/mappings/os-v1/vocabularies/vocabulary-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/mappings/os-v2/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/mappings/os-v2/vocabularies/vocabulary-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/mappings/v7/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/mappings/v7/vocabularies/vocabulary-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/schemas/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/schemas/vocabularies/vocabulary-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/sources/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/sources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/sources/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/sources/opendefinition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-03-10 14:18:04.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26890 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 14:18:04.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-03-10 14:18:04.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 14:18:04.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-03-10 14:18:04.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-10 14:18:04.000000 invenio-app-ils-1.0.0rc3/invenio_app_ils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/run-tests.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      329 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/scripts/bootstrap
--rwxr-xr-x   0 runner    (1001) docker     (123)      270 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/scripts/build_assets
--rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/scripts/celery
--rwxr-xr-x   0 runner    (1001) docker     (123)      248 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/scripts/console
--rwxr-xr-x   0 runner    (1001) docker     (123)      341 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/scripts/update
--rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/tests/api/acquisition/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/acquisition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/acquisition/test_acq_orders_crud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/acquisition/test_acq_orders_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/acquisition/test_acq_providers_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/tests/api/circulation/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/circulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/circulation/test_expired_loans.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/circulation/test_loan_bulk_extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/circulation/test_loan_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/circulation/test_loan_default_durations.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/circulation/test_loan_document_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/circulation/test_loan_extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/circulation/test_loan_item_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/circulation/test_loan_item_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/circulation/test_loan_list_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/circulation/test_loan_patron_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/circulation/test_loan_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/circulation/test_loan_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/circulation/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/tests/api/document_requests/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/document_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/document_requests/test_document_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/document_requests/test_document_requests_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/document_requests/test_notifications_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/tests/api/ill/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ill/test_ill_brw_crud.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ill/test_ill_brw_reqs_patron_loan_create_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    10423 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ill/test_ill_brw_reqs_patron_loan_extension_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ill/test_ill_brw_reqs_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ill/test_ill_providers_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/documents/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/documents/test_document_crud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/documents/test_document_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/documents/test_document_resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/eitems/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/eitems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/eitems/test_eitems_crud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/eitems/test_eitems_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/eitems/test_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/items/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/items/test_apis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/items/test_items_crud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/items/test_items_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/items/test_items_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/records_relations/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/records_relations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/records_relations/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17969 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/records_relations/test_records_relations_parentchild.py
--rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/records_relations/test_records_relations_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    24820 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/records_relations/test_records_relations_siblings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/series/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/series/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/series/test_series_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/test_anonymization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/test_apis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10041 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/test_closures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/test_facets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/test_internal_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/test_metadata_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/test_notifications_mails.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/test_notifications_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/test_patrons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/test_record_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/test_record_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/test_resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/api/ils/test_vocabularies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/data/acq_orders.json
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/data/acq_providers.json
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/data/document_requests.json
--rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/data/documents.json
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/data/eitems.json
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/data/ill_borrowing_requests.json
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/data/ill_providers.json
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/data/internal_locations.json
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/data/items.json
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/data/loans.json
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/data/loans_most_loaned.json
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/data/locations.json
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/data/series.json
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/tests/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:05.000000 invenio-app-ils-1.0.0rc3/tests/templates/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/templates/notifications/blank.html
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/templates/notifications/title_body.html
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/templates/notifications/title_body_html.html
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/templates/notifications/title_body_html_ctx.html
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/templates/notifications/title_only.html
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/test_post_logout_redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-10 14:18:01.000000 invenio-app-ils-1.0.0rc3/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14161 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/docker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/docker/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docker/backend/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/docker/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docker/frontend/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/docker/frontend/conf.d/
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docker/frontend/conf.d/default.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docker/frontend/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docker/frontend/test.crt
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docker/frontend/test.key
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/docker/lb/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docker/lb/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docker/lb/haproxy.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docker/lb/haproxy_cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docker-compose.full.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docker-services.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/jsonresolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/jsonresolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/jsonresolvers/order_order_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/jsonresolvers/order_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/loaders/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/loaders/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/loaders/jsonschemas/order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/mappings/os-v1/acq_orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/mappings/os-v1/acq_orders/order-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/mappings/os-v2/acq_orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/mappings/os-v2/acq_orders/order-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/mappings/v7/acq_orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/mappings/v7/acq_orders/order-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/schemas/acq_orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/schemas/acq_orders/order-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/jsonresolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/jsonresolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/jsonresolvers/loan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/loaders/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/loaders/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/loaders/schemas/json/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/loaders/schemas/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/loaders/schemas/json/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/loaders/schemas/json/bulk_extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/loaders/schemas/json/loan_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/loaders/schemas/json/loan_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/loaders/schemas/json/loan_update_dates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/notifications/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/notifications/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/notifications/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/serializers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/serializers/custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/serializers/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/stats/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/stats/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/bulk_extend.html
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/cancel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/checkin.html
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/checkout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/extend.html
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/overdue_reminder.html
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/request.html
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/request_no_items.html
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/will_expire_in_reminder.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/transitions/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/transitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/transitions/transitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57138 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/closures/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/closures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/closures/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/closures/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40830 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/demo_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/demo_data/documents.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/demo_data/items.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/jsonresolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/jsonresolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/jsonresolvers/document_request_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/jsonresolvers/document_request_patron.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/loaders/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/loaders/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/loaders/jsonschemas/document_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_decline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/mappings/os-v1/document_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/mappings/os-v1/document_requests/document_request-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/mappings/os-v2/document_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/mappings/os-v2/document_requests/document_request-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/mappings/v7/document_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/mappings/v7/document_requests/document_request-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/notifications/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/notifications/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/schemas/document_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/schemas/document_requests/document_request-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_accept.html
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_decline_in_catalog.html
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_decline_not_found.html
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_decline_other.html
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_decline_user_cancel.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/jsonresolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/jsonresolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/jsonresolvers/document_circulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/jsonresolvers/document_eitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/jsonresolvers/document_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/jsonresolvers/document_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/jsonresolvers/document_stock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/loaders/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/loaders/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/loaders/jsonschemas/document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/mappings/os-v1/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)    21341 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/mappings/os-v1/documents/document-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/mappings/os-v2/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)    21341 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/mappings/os-v2/documents/document-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/mappings/v7/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)    21341 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/mappings/v7/documents/document-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/schemas/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)    18138 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/schemas/documents/document-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/jsonresolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/jsonresolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/jsonresolvers/eitem_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/jsonresolvers/eitem_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/loaders/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/loaders/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/loaders/jsonschemas/eitems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/mappings/os-v1/eitems/
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/mappings/os-v1/eitems/eitem-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/mappings/os-v2/eitems/
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/mappings/os-v2/eitems/eitem-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/mappings/v7/eitems/
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/mappings/v7/eitems/eitem-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/schemas/eitems/
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/schemas/eitems/eitem-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/fetchers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/files/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/files/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/jsonresolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/jsonresolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/jsonresolvers/borrowing_request_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/jsonresolvers/borrowing_request_patron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/jsonresolvers/borrowing_request_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/loaders/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/loaders/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/loaders/jsonschemas/borrowing_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/loaders/jsonschemas/patron_loan_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/loaders/jsonschemas/patron_loan_extension_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/mappings/os-v1/ill_borrowing_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/mappings/os-v1/ill_borrowing_requests/borrowing_request-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/mappings/os-v2/ill_borrowing_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/mappings/os-v2/ill_borrowing_requests/borrowing_request-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/mappings/v7/ill_borrowing_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/mappings/v7/ill_borrowing_requests/borrowing_request-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/notifications/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/notifications/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/schemas/ill_borrowing_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/schemas/ill_borrowing_requests/borrowing_request-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/serializers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/serializers/custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/serializers/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/templates/invenio_app_ils_ill/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_accept.html
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_decline.html
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_request.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/jsonresolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/jsonresolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/jsonresolvers/internal_location.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/loaders/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/loaders/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/loaders/jsonschemas/internal_location.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/mappings/os-v1/internal_locations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/mappings/os-v1/internal_locations/internal_location-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/mappings/os-v2/internal_locations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/mappings/os-v2/internal_locations/internal_location-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/mappings/v7/internal_locations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/mappings/v7/internal_locations/internal_location-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/schemas/internal_locations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/schemas/internal_locations/internal_location-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/jsonresolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/jsonresolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/jsonresolvers/item_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/jsonresolvers/item_internal_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/jsonresolvers/item_loan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/loaders/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/loaders/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/loaders/jsonschemas/items.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/mappings/os-v1/items/
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/mappings/os-v1/items/item-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/mappings/os-v2/items/
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/mappings/os-v2/items/item-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/mappings/v7/items/
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/mappings/v7/items/item-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/schemas/items/
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/schemas/items/item-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/items/serializers/item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/literature/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/literature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/literature/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/literature/covers_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/literature/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/literature/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/literature/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/literature/serializers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/literature/serializers/custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/literature/serializers/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/loaders/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/loaders/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/loaders/jsonschemas/location.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/mappings/os-v1/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/mappings/os-v1/locations/location-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/mappings/os-v2/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/mappings/os-v2/locations/location-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/mappings/v7/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/mappings/v7/locations/location-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/receivers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/schemas/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/schemas/locations/location-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/minters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/notifications/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/notifications/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/notifications/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/notifications/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/notifications/backends/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/notifications/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/notifications/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/notifications/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/notifications/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/anonymization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/mappings/os-v1/patrons/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/mappings/os-v1/patrons/patron-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/mappings/os-v2/patrons/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/mappings/os-v2/patrons/patron-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/mappings/v7/patrons/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/mappings/v7/patrons/patron-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/loaders/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/loaders/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/loaders/jsonschemas/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/mappings/os-v1/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/mappings/os-v1/providers/provider-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/mappings/os-v2/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/mappings/os-v2/providers/provider-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/mappings/v7/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/mappings/v7/providers/provider-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/schemas/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/schemas/providers/provider-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/jsonresolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/jsonresolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/jsonresolvers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/listeners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/loaders/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/loaders/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/loaders/schemas/changed_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/loaders/schemas/preserve_cover_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/loaders/schemas/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/metadata_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/receivers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/schemas/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records_relations/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records_relations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records_relations/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records_relations/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records_relations/retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14889 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/records_relations/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/relations/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/relations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13996 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/relations/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/relations/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/search_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/jsonresolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/jsonresolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/jsonresolvers/series_relations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/loaders/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/loaders/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/loaders/jsonschemas/series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/mappings/os-v1/series/
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/mappings/os-v1/series/series-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/mappings/os-v2/series/
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/mappings/os-v2/series/series-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/mappings/v7/series/
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/mappings/v7/series/series-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/schemas/series/
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/schemas/series/series-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/series/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/static/images/placeholder.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/static_pages/
+-rw-r--r--   0 runner    (1001) docker     (123)    22084 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/static_pages/search_guide.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/aggregations/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/aggregations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/aggregations/aggr_file_download/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/aggregations/aggr_file_download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/aggregations/aggr_file_download/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/aggregations/aggr_file_download/os-v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/aggregations/aggr_file_download/os-v1/aggr-file-download-v1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/aggregations/aggr_file_download/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/aggregations/aggr_file_download/os-v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/aggregations/aggr_file_download/os-v2/aggr-file-download-v1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/aggregations/aggr_file_download/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/aggregations/aggr_file_download/v7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/aggregations/aggr_file_download/v7/aggr-file-download-v1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/file_download/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/file_download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/file_download/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/file_download/os-v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/file_download/os-v1/file-download-v1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/file_download/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/file_download/os-v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/file_download/os-v2/file-download-v1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/file_download/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/file_download/v7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/file_download/v7/file-download-v1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/templates/invenio_app_ils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/templates/invenio_app_ils/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/templates/invenio_app_ils/mail/footer.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/templates/invenio_app_ils/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/templates/invenio_app_ils/notifications/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/templates/logged_out.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/translations/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/acq_mediums.json
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/acq_order_line_payment_modes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/acq_order_line_purchase_types.json
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/acq_payment_modes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/acq_recipients.json
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/affiliation_identifier_schemes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/alternative_identifier_schemes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/alternative_title_types.json
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/author_identifier_schemes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/author_roles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/author_types.json
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/conference_identifier_schemes.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20498 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/countries.json
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/currencies.json
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/docreq_payment_method.json
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/docreq_request_type.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/document_identifiers_materials.json
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/document_requests_mediums.json
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/document_subjects.json
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/eitem_sources.json
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/identifier_schemes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/ill_item_types.json
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/ill_payment_modes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/item_mediums.json
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/provider_types.json
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/series_identifier_schemes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/series_url_access_restrictions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/jsonresolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/jsonresolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/jsonresolvers/licenses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/mappings/os-v1/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/mappings/os-v1/vocabularies/vocabulary-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/mappings/os-v2/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/mappings/os-v2/vocabularies/vocabulary-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/mappings/v7/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/mappings/v7/vocabularies/vocabulary-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/schemas/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/schemas/vocabularies/vocabulary-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/sources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/sources/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/sources/opendefinition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14161 2023-07-04 15:45:11.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26919 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:45:11.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-07-04 15:45:11.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:45:11.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-04 15:45:11.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 15:45:11.000000 invenio-app-ils-1.0.0rc4/invenio_app_ils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/run-tests.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      329 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/scripts/bootstrap
+-rwxr-xr-x   0 runner    (1001) docker     (123)      270 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/scripts/build_assets
+-rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/scripts/celery
+-rwxr-xr-x   0 runner    (1001) docker     (123)      248 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/scripts/console
+-rwxr-xr-x   0 runner    (1001) docker     (123)      412 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/scripts/server
+-rwxr-xr-x   0 runner    (1001) docker     (123)      251 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/scripts/setup
+-rwxr-xr-x   0 runner    (1001) docker     (123)      341 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/scripts/update
+-rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/tests/api/acquisition/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/acquisition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/acquisition/test_acq_orders_crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/acquisition/test_acq_orders_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/acquisition/test_acq_providers_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/tests/api/circulation/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/circulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/circulation/test_expired_loans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/circulation/test_loan_bulk_extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/circulation/test_loan_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/circulation/test_loan_default_durations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/circulation/test_loan_document_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/circulation/test_loan_extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/circulation/test_loan_item_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/circulation/test_loan_item_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/circulation/test_loan_list_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/circulation/test_loan_patron_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/circulation/test_loan_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/circulation/test_loan_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/circulation/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/tests/api/document_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/document_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/document_requests/test_document_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/document_requests/test_document_requests_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/document_requests/test_notifications_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/tests/api/ill/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ill/test_ill_brw_crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ill/test_ill_brw_reqs_patron_loan_create_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10423 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ill/test_ill_brw_reqs_patron_loan_extension_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ill/test_ill_brw_reqs_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ill/test_ill_providers_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/documents/test_document_crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/documents/test_document_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/documents/test_document_resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/eitems/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/eitems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/eitems/test_eitems_crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/eitems/test_eitems_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/eitems/test_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/items/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/items/test_apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/items/test_items_crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/items/test_items_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/items/test_items_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/records_relations/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/records_relations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/records_relations/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17969 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/records_relations/test_records_relations_parentchild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/records_relations/test_records_relations_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24820 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/records_relations/test_records_relations_siblings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/series/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/series/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/series/test_series_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/test_anonymization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/test_apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10041 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/test_closures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/test_facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/test_internal_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/test_metadata_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/test_notifications_mails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/test_notifications_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/test_patrons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/test_record_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/test_record_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/test_resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/api/ils/test_vocabularies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/data/acq_orders.json
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/data/acq_providers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/data/document_requests.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/data/documents.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/data/eitems.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/data/ill_borrowing_requests.json
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/data/ill_providers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/data/internal_locations.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/data/items.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/data/loans.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/data/loans_most_loaned.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/data/locations.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/data/series.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/tests/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:12.000000 invenio-app-ils-1.0.0rc4/tests/templates/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/templates/notifications/blank.html
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/templates/notifications/title_body.html
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/templates/notifications/title_body_html.html
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/templates/notifications/title_body_html_ctx.html
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/templates/notifications/title_only.html
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/test_post_logout_redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-04 15:45:02.000000 invenio-app-ils-1.0.0rc4/tests/test_version.py
```

### Comparing `invenio-app-ils-1.0.0rc3/.editorconfig` & `invenio-app-ils-1.0.0rc4/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/CHANGES.rst` & `invenio-app-ils-1.0.0rc4/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
     invenio-app-ils is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 1.0.0rc4 (released 2023-07-04)
+
+- Fix docker-compose file
+
 Version 1.0.0rc3 (released 2023-03-10)
 
 - Remove ES v6 mappings
 
 Version 1.0.0rc2 (released 2023-03-07)
 
 - add opensearch docker image
```

### Comparing `invenio-app-ils-1.0.0rc3/CONTRIBUTING.rst` & `invenio-app-ils-1.0.0rc4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/LICENSE` & `invenio-app-ils-1.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/MANIFEST.in` & `invenio-app-ils-1.0.0rc4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/PKG-INFO` & `invenio-app-ils-1.0.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-app-ils
-Version: 1.0.0rc3
+Version: 1.0.0rc4
 Summary: Invenio Integrated Library System.
 Home-page: https://github.com/inveniosoftware/invenio-app-ils
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2018-2020 CERN.
@@ -36,14 +36,18 @@
         
             invenio-app-ils is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 1.0.0rc4 (released 2023-07-04)
+        
+        - Fix docker-compose file
+        
         Version 1.0.0rc3 (released 2023-03-10)
         
         - Remove ES v6 mappings
         
         Version 1.0.0rc2 (released 2023-03-07)
         
         - add opensearch docker image
```

### Comparing `invenio-app-ils-1.0.0rc3/README.rst` & `invenio-app-ils-1.0.0rc4/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/docker/backend/Dockerfile` & `invenio-app-ils-1.0.0rc4/docker/backend/Dockerfile`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/docker/frontend/Dockerfile` & `invenio-app-ils-1.0.0rc4/docker/frontend/Dockerfile`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/docker/frontend/conf.d/default.conf` & `invenio-app-ils-1.0.0rc4/docker/frontend/conf.d/default.conf`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/docker/frontend/nginx.conf` & `invenio-app-ils-1.0.0rc4/docker/frontend/nginx.conf`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/docker/frontend/test.crt` & `invenio-app-ils-1.0.0rc4/docker/frontend/test.crt`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/docker/frontend/test.key` & `invenio-app-ils-1.0.0rc4/docker/frontend/test.key`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/docker/lb/haproxy.cfg` & `invenio-app-ils-1.0.0rc4/docker/lb/haproxy.cfg`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/docker/lb/haproxy_cert.pem` & `invenio-app-ils-1.0.0rc4/docker/lb/haproxy_cert.pem`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/docker-compose.full.yml` & `invenio-app-ils-1.0.0rc4/docker-compose.full.yml`

 * *Files 7% similar despite different names*

```diff
@@ -29,27 +29,27 @@
       file: docker-services.yml
       service: backend
     command: uwsgi --module invenio_app.wsgi:application --socket 0.0.0.0:5000 --master --processes 2 --threads 2 --stats /tmp/stats.socket
     volumes:
       - static_data:/opt/invenio_app_ils/var/instance
     links:
       - cache
-      - es
+      - search
       - mq
       - db
   # Worker
   worker:
     extends:
       file: docker-services.yml
       service: backend
     command: "celery -A invenio_app.celery worker --loglevel=INFO"
     image: invenio_app_ils-worker
     links:
       - cache
-      - es
+      - search
       - mq
       - db
   # Monitoring
   flower:
     extends:
       file: docker-services.yml
       service: flower
@@ -64,13 +64,13 @@
     extends:
       file: docker-services.yml
       service: db
   mq:
     extends:
       file: docker-services.yml
       service: mq
-  es:
+  search:
     extends:
       file: docker-services.yml
-      service: es
+      service: search
 volumes:
   static_data:
```

### Comparing `invenio-app-ils-1.0.0rc3/docker-compose.yml` & `invenio-app-ils-1.0.0rc4/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/docker-services.yml` & `invenio-app-ils-1.0.0rc4/docker-services.yml`

 * *Files 19% similar despite different names*

```diff
@@ -46,28 +46,27 @@
       - "8080:8080"
   cache:
     image: redis:6
     read_only: true
     ports:
       - "6379:6379"
   db:
-    image: postgres:12.4
+    image: postgres:14
     environment:
       - "POSTGRES_USER=test"
       - "POSTGRES_PASSWORD=psw"
       - "POSTGRES_DB=ils"
     ports:
       - "5432:5432"
   mq:
     image: rabbitmq:3-management
     ports:
       - "15672:15672"
       - "5672:5672"
   search:
-    # to use ES7: docker.elastic.co/elasticsearch/elasticsearch-oss:7.9.1
     image: opensearchproject/opensearch:2.5.0
     environment:
       - bootstrap.memory_lock=true
       - compatibility.override_main_response_version=true
       - "OPENSEARCH_JAVA_OPTS=-Xms512m -Xmx512m"
       - "DISABLE_INSTALL_DEMO_CONFIG=true"
       - "DISABLE_SECURITY_PLUGIN=true"
@@ -76,21 +75,22 @@
       memlock:
         soft: -1
         hard: -1
     mem_limit: 1g
     ports:
       - "9200:9200"
       - "9300:9300"
-  # TODO: opensearch dashboards
-  kibana:
-    # to use ES6: docker.elastic.co/kibana/kibana-oss:6.8.8
-    # to use ES7: docker.elastic.co/kibana/kibana-oss:7.9.1
-    image: docker.elastic.co/kibana/kibana-oss:7.9.1
+  opensearch-dashboards:
+    image: opensearchproject/opensearch-dashboards:{{ dashboards_version }}
+    ports:
+      - "5601:5601"
+    expose:
+      - "5601"
     environment:
-      - "ELASTICSEARCH_URL=http://es:9200"
-      - "ES_JAVA_OPTS=-Xms512m -Xmx512m"
-    ports: ["5601:5601"]
+      # settings only for development. DO NOT use in production!
+      - 'OPENSEARCH_HOSTS=["http://search:9200"]'
+      - "DISABLE_SECURITY_DASHBOARDS_PLUGIN=true"
   flower:
     image: mher/flower:0.9.7
     command: --broker=amqp://guest:guest@mq:5672/ --broker_api=http://guest:guest@mq:15672/api/
     ports:
       - "5555:5555"
```

### Comparing `invenio-app-ils-1.0.0rc3/docs/Makefile` & `invenio-app-ils-1.0.0rc4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/docs/conf.py` & `invenio-app-ils-1.0.0rc4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/docs/index.rst` & `invenio-app-ils-1.0.0rc4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/docs/make.bat` & `invenio-app-ils-1.0.0rc4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/config.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/config.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/ext.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/jsonresolvers/order_order_lines.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/jsonresolvers/order_order_lines.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/jsonresolvers/order_provider.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/jsonresolvers/order_provider.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/loaders/jsonschemas/order.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/loaders/jsonschemas/order.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/mappings/os-v1/acq_orders/order-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/mappings/os-v1/acq_orders/order-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/mappings/os-v2/acq_orders/order-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/mappings/os-v2/acq_orders/order-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/mappings/v7/acq_orders/order-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/mappings/v7/acq_orders/order-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/schemas/acq_orders/order-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/schemas/acq_orders/order-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/acquisition/search.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/acquisition/search.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/config.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/config.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/indexer.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/jsonresolvers/loan.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/jsonresolvers/loan.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/loaders/__init__.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/loaders/schemas/json/base.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/loaders/schemas/json/base.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/loaders/schemas/json/bulk_extend.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/loaders/schemas/json/bulk_extend.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/loaders/schemas/json/loan_checkout.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/loaders/schemas/json/loan_checkout.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/loaders/schemas/json/loan_request.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/loaders/schemas/json/loan_request.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/loaders/schemas/json/loan_update_dates.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/loaders/schemas/json/loan_update_dates.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/notifications/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/notifications/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/notifications/messages.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/notifications/messages.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/notifications/tasks.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/notifications/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/receivers.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/receivers.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/search.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/search.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/serializers/__init__.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/serializers/csv.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/serializers/csv.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/serializers/custom_fields.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/serializers/custom_fields.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/serializers/json.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/serializers/json.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/serializers/response.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/serializers/response.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/stats/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/stats/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/stats/views.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/stats/views.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/tasks.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/bulk_extend.html` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/bulk_extend.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/cancel.html` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/cancel.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/checkin.html` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/checkin.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/checkout.html` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/checkout.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/extend.html` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/extend.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/overdue_reminder.html` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/overdue_reminder.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/request.html` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/request.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/request_no_items.html` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/request_no_items.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/will_expire_in_reminder.html` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/will_expire_in_reminder.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/transitions/transitions.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/transitions/transitions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/utils.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/circulation/views.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/circulation/views.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/cli.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/closures/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/closures/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/closures/tasks.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/closures/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/config.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/config.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/demo_data/documents.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/demo_data/documents.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/demo_data/items.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/demo_data/items.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/indexer.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/jsonresolvers/document_request_document.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/jsonresolvers/document_request_document.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/jsonresolvers/document_request_patron.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/jsonresolvers/document_request_patron.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/loaders/__init__.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/loaders/jsonschemas/document_request.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/loaders/jsonschemas/document_request.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_decline.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_decline.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_document.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_document.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_provider.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_provider.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/mappings/os-v1/document_requests/document_request-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/mappings/os-v1/document_requests/document_request-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/mappings/os-v2/document_requests/document_request-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/mappings/os-v2/document_requests/document_request-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/mappings/v7/document_requests/document_request-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/mappings/v7/document_requests/document_request-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/notifications/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/notifications/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/notifications/messages.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/notifications/messages.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/schemas/document_requests/document_request-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/schemas/document_requests/document_request-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/search.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/search.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_decline_in_catalog.html` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_decline_in_catalog.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/document_requests/views.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/document_requests/views.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/indexer.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/jsonresolvers/document_circulation.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/jsonresolvers/document_circulation.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/jsonresolvers/document_eitem.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/jsonresolvers/document_eitem.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/jsonresolvers/document_item.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/jsonresolvers/document_item.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/jsonresolvers/document_relations.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/jsonresolvers/document_relations.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/jsonresolvers/document_stock.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/jsonresolvers/document_stock.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/loaders/jsonschemas/document.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/loaders/jsonschemas/document.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/mappings/os-v1/documents/document-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/mappings/os-v1/documents/document-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/mappings/os-v2/documents/document-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/mappings/os-v2/documents/document-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/mappings/v7/documents/document-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/mappings/v7/documents/document-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/schemas/documents/document-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/schemas/documents/document-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/documents/search.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/documents/search.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/indexer.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/jsonresolvers/eitem_document.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/jsonresolvers/eitem_document.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/jsonresolvers/eitem_files.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/jsonresolvers/eitem_files.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/loaders/jsonschemas/eitems.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/loaders/jsonschemas/eitems.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/mappings/os-v1/eitems/eitem-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/mappings/os-v1/eitems/eitem-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/mappings/os-v2/eitems/eitem-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/mappings/os-v2/eitems/eitem-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/mappings/v7/eitems/eitem-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/mappings/v7/eitems/eitem-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/schemas/eitems/eitem-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/schemas/eitems/eitem-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/eitems/search.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/eitems/search.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/errors.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ext.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/facets.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/facets.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/fetchers.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/fetchers.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/files/receivers.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/files/receivers.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/files/views.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/files/views.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/config.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/config.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/errors.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/ext.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/jsonresolvers/borrowing_request_document.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/jsonresolvers/borrowing_request_document.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/jsonresolvers/borrowing_request_patron.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/jsonresolvers/borrowing_request_patron.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/jsonresolvers/borrowing_request_provider.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/jsonresolvers/borrowing_request_provider.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/loaders/__init__.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/loaders/jsonschemas/borrowing_request.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/loaders/jsonschemas/borrowing_request.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/loaders/jsonschemas/patron_loan_actions.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/loaders/jsonschemas/patron_loan_actions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/loaders/jsonschemas/patron_loan_extension_actions.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/loaders/jsonschemas/patron_loan_extension_actions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/mappings/os-v1/ill_borrowing_requests/borrowing_request-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/mappings/os-v1/ill_borrowing_requests/borrowing_request-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/mappings/os-v2/ill_borrowing_requests/borrowing_request-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/mappings/os-v2/ill_borrowing_requests/borrowing_request-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/mappings/v7/ill_borrowing_requests/borrowing_request-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/mappings/v7/ill_borrowing_requests/borrowing_request-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/notifications/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/notifications/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/notifications/messages.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/notifications/messages.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/schemas/ill_borrowing_requests/borrowing_request-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/schemas/ill_borrowing_requests/borrowing_request-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/search.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/search.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/serializers/__init__.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/serializers/csv.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/serializers/csv.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/serializers/custom_fields.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/serializers/custom_fields.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/serializers/json.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/serializers/json.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_accept.html` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_accept.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_decline.html` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_decline.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_request.html` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_request.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/ill/views.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/ill/views.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/indexer.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/indexer.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/jsonresolvers/internal_location.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/jsonresolvers/internal_location.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/loaders/__init__.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/loaders/jsonschemas/internal_location.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/loaders/jsonschemas/internal_location.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/mappings/os-v1/internal_locations/internal_location-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/mappings/os-v1/internal_locations/internal_location-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/mappings/os-v2/internal_locations/internal_location-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/mappings/os-v2/internal_locations/internal_location-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/mappings/v7/internal_locations/internal_location-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/mappings/v7/internal_locations/internal_location-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/schemas/internal_locations/internal_location-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/schemas/internal_locations/internal_location-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/internal_locations/search.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/internal_locations/search.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/items/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/items/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/items/indexer.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/items/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/items/jsonresolvers/item_document.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/items/jsonresolvers/item_document.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/items/jsonresolvers/item_internal_location.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/items/jsonresolvers/item_internal_location.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/items/jsonresolvers/item_loan.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/items/jsonresolvers/item_loan.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/items/loaders/jsonschemas/items.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/items/loaders/jsonschemas/items.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/items/mappings/os-v1/items/item-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/items/mappings/os-v1/items/item-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/items/mappings/os-v2/items/item-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/items/mappings/os-v2/items/item-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/items/mappings/v7/items/item-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/items/mappings/v7/items/item-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/items/schemas/items/item-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/items/schemas/items/item-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/items/search.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/items/search.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/items/serializers/__init__.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/items/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/items/serializers/item.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/items/serializers/item.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/literature/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/literature/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/literature/covers_builder.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/literature/covers_builder.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/literature/search.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/literature/search.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/literature/serializers/__init__.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/literature/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/literature/serializers/csv.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/literature/serializers/csv.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/literature/serializers/custom_fields.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/literature/serializers/custom_fields.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/literature/serializers/json.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/literature/serializers/json.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/indexer.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/loaders/jsonschemas/location.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/loaders/jsonschemas/location.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/mappings/os-v1/locations/location-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/mappings/os-v1/locations/location-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/mappings/os-v2/locations/location-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/mappings/os-v2/locations/location-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/mappings/v7/locations/location-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/mappings/v7/locations/location-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/receivers.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/receivers.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/locations/schemas/locations/location-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/locations/schemas/locations/location-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/minters.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/minters.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/notifications/admin.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/notifications/admin.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/notifications/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/notifications/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/notifications/backends/mail.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/notifications/backends/mail.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/notifications/messages.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/notifications/messages.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/notifications/models.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/notifications/models.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/notifications/tasks.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/notifications/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/notifications/views.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/notifications/views.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/anonymization.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/anonymization.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/cli.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/indexer.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/mappings/os-v1/patrons/patron-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/mappings/os-v1/patrons/patron-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/mappings/os-v2/patrons/patron-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/mappings/os-v2/patrons/patron-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/mappings/v7/patrons/patron-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/mappings/v7/patrons/patron-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/patrons/views.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/patrons/views.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/permissions.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/config.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/config.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/errors.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/ext.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/indexer.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/loaders/jsonschemas/provider.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/loaders/jsonschemas/provider.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/mappings/os-v1/providers/provider-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/mappings/os-v1/providers/provider-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/mappings/os-v2/providers/provider-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/mappings/os-v2/providers/provider-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/mappings/v7/providers/provider-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/mappings/v7/providers/provider-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/providers/schemas/providers/provider-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/providers/schemas/providers/provider-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/records/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/records/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/records/jsonresolvers/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/records/jsonresolvers/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/records/listeners.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/records/listeners.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/records/loaders/__init__.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/records/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/records/loaders/schemas/changed_by.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/records/loaders/schemas/changed_by.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/records/loaders/schemas/price.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/records/loaders/schemas/price.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/records/metadata_extensions.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/records/metadata_extensions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/records/permissions.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/records/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/records/schemas/json.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/records/schemas/json.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/records/serializers/__init__.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/records/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/records/views.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/records/views.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/records_relations/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/records_relations/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/records_relations/indexer.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/records_relations/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/records_relations/retriever.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/records_relations/retriever.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/records_relations/views.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/records_relations/views.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/relations/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/relations/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/search_permissions.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/search_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/series/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/series/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/series/indexer.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/series/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/series/jsonresolvers/series_relations.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/series/jsonresolvers/series_relations.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/series/loaders/jsonschemas/series.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/series/loaders/jsonschemas/series.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/series/mappings/os-v1/series/series-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/series/mappings/os-v1/series/series-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/series/mappings/os-v2/series/series-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/series/mappings/os-v2/series/series-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/series/mappings/v7/series/series-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/series/mappings/v7/series/series-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/series/schemas/series/series-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/series/schemas/series/series-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/series/search.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/series/search.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/static/images/placeholder.png` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/static/images/placeholder.png`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/static_pages/search_guide.html` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/static_pages/search_guide.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/aggregations/aggr_file_download/os-v1/aggr-file-download-v1.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/aggregations/aggr_file_download/os-v1/aggr-file-download-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/aggregations/aggr_file_download/os-v2/aggr-file-download-v1.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/aggregations/aggr_file_download/os-v2/aggr-file-download-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/aggregations/aggr_file_download/v7/aggr-file-download-v1.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/aggregations/aggr_file_download/v7/aggr-file-download-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/file_download/os-v1/file-download-v1.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/file_download/os-v1/file-download-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/file_download/os-v2/file-download-v1.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/file_download/os-v2/file-download-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/stats/file_download/v7/file-download-v1.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/stats/file_download/v7/file-download-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/views.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/views.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/api.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/cli.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/author_roles.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/author_roles.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/countries.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/countries.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/data/document_identifiers_materials.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/data/document_identifiers_materials.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/indexer.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/jsonresolvers/licenses.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/jsonresolvers/licenses.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/schemas/vocabularies/vocabulary-v1.0.0.json` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/schemas/vocabularies/vocabulary-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/search.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/search.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/sources/base.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/sources/base.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/sources/json.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/sources/json.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils/vocabularies/sources/opendefinition.py` & `invenio-app-ils-1.0.0rc4/invenio_app_ils/vocabularies/sources/opendefinition.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils.egg-info/PKG-INFO` & `invenio-app-ils-1.0.0rc4/invenio_app_ils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-app-ils
-Version: 1.0.0rc3
+Version: 1.0.0rc4
 Summary: Invenio Integrated Library System.
 Home-page: https://github.com/inveniosoftware/invenio-app-ils
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2018-2020 CERN.
@@ -36,14 +36,18 @@
         
             invenio-app-ils is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 1.0.0rc4 (released 2023-07-04)
+        
+        - Fix docker-compose file
+        
         Version 1.0.0rc3 (released 2023-03-10)
         
         - Remove ES v6 mappings
         
         Version 1.0.0rc2 (released 2023-03-07)
         
         - add opensearch docker image
```

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils.egg-info/SOURCES.txt` & `invenio-app-ils-1.0.0rc4/invenio_app_ils.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -459,14 +459,16 @@
 invenio_app_ils/vocabularies/sources/base.py
 invenio_app_ils/vocabularies/sources/json.py
 invenio_app_ils/vocabularies/sources/opendefinition.py
 scripts/bootstrap
 scripts/build_assets
 scripts/celery
 scripts/console
+scripts/server
+scripts/setup
 scripts/update
 tests/__init__.py
 tests/conftest.py
 tests/helpers.py
 tests/test_post_logout_redirect.py
 tests/test_version.py
 tests/api/__init__.py
```

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils.egg-info/entry_points.txt` & `invenio-app-ils-1.0.0rc4/invenio_app_ils.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/invenio_app_ils.egg-info/requires.txt` & `invenio-app-ils-1.0.0rc4/invenio_app_ils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/run-tests.sh` & `invenio-app-ils-1.0.0rc4/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/setup.cfg` & `invenio-app-ils-1.0.0rc4/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/acquisition/test_acq_orders_crud.py` & `invenio-app-ils-1.0.0rc4/tests/api/acquisition/test_acq_orders_crud.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/acquisition/test_acq_orders_permissions.py` & `invenio-app-ils-1.0.0rc4/tests/api/acquisition/test_acq_orders_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/acquisition/test_acq_providers_permissions.py` & `invenio-app-ils-1.0.0rc4/tests/api/acquisition/test_acq_providers_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/circulation/test_expired_loans.py` & `invenio-app-ils-1.0.0rc4/tests/api/circulation/test_expired_loans.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/circulation/test_loan_bulk_extend.py` & `invenio-app-ils-1.0.0rc4/tests/api/circulation/test_loan_bulk_extend.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/circulation/test_loan_checkout.py` & `invenio-app-ils-1.0.0rc4/tests/api/circulation/test_loan_checkout.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/circulation/test_loan_default_durations.py` & `invenio-app-ils-1.0.0rc4/tests/api/circulation/test_loan_default_durations.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/circulation/test_loan_document_resolver.py` & `invenio-app-ils-1.0.0rc4/tests/api/circulation/test_loan_document_resolver.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/circulation/test_loan_extend.py` & `invenio-app-ils-1.0.0rc4/tests/api/circulation/test_loan_extend.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/circulation/test_loan_item_permissions.py` & `invenio-app-ils-1.0.0rc4/tests/api/circulation/test_loan_item_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/circulation/test_loan_item_resolver.py` & `invenio-app-ils-1.0.0rc4/tests/api/circulation/test_loan_item_resolver.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/circulation/test_loan_list_permissions.py` & `invenio-app-ils-1.0.0rc4/tests/api/circulation/test_loan_list_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/circulation/test_loan_patron_resolver.py` & `invenio-app-ils-1.0.0rc4/tests/api/circulation/test_loan_patron_resolver.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/circulation/test_loan_request.py` & `invenio-app-ils-1.0.0rc4/tests/api/circulation/test_loan_request.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/circulation/test_loan_update.py` & `invenio-app-ils-1.0.0rc4/tests/api/circulation/test_loan_update.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/circulation/test_notifications.py` & `invenio-app-ils-1.0.0rc4/tests/api/circulation/test_notifications.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/conftest.py` & `invenio-app-ils-1.0.0rc4/tests/api/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/document_requests/test_document_requests.py` & `invenio-app-ils-1.0.0rc4/tests/api/document_requests/test_document_requests.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/document_requests/test_document_requests_permissions.py` & `invenio-app-ils-1.0.0rc4/tests/api/document_requests/test_document_requests_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/document_requests/test_notifications_filter.py` & `invenio-app-ils-1.0.0rc4/tests/api/document_requests/test_notifications_filter.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ill/test_ill_brw_crud.py` & `invenio-app-ils-1.0.0rc4/tests/api/ill/test_ill_brw_crud.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ill/test_ill_brw_reqs_patron_loan_create_action.py` & `invenio-app-ils-1.0.0rc4/tests/api/ill/test_ill_brw_reqs_patron_loan_create_action.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ill/test_ill_brw_reqs_patron_loan_extension_actions.py` & `invenio-app-ils-1.0.0rc4/tests/api/ill/test_ill_brw_reqs_patron_loan_extension_actions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ill/test_ill_brw_reqs_permissions.py` & `invenio-app-ils-1.0.0rc4/tests/api/ill/test_ill_brw_reqs_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ill/test_ill_providers_permissions.py` & `invenio-app-ils-1.0.0rc4/tests/api/ill/test_ill_providers_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/documents/test_document_crud.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/documents/test_document_crud.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/documents/test_document_permissions.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/documents/test_document_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/documents/test_document_resolvers.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/documents/test_document_resolvers.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/eitems/test_eitems_crud.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/eitems/test_eitems_crud.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/eitems/test_eitems_permissions.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/eitems/test_eitems_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/eitems/test_files.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/eitems/test_files.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/items/test_apis.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/items/test_apis.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/items/test_items_crud.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/items/test_items_crud.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/items/test_items_permissions.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/items/test_items_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/items/test_items_update.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/items/test_items_update.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/records_relations/helpers.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/records_relations/helpers.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/records_relations/test_records_relations_parentchild.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/records_relations/test_records_relations_parentchild.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/records_relations/test_records_relations_sequence.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/records_relations/test_records_relations_sequence.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/records_relations/test_records_relations_siblings.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/records_relations/test_records_relations_siblings.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/series/test_series_permissions.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/series/test_series_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/test_anonymization.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/test_anonymization.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/test_apis.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/test_apis.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/test_closures.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/test_closures.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/test_errors.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/test_errors.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/test_facets.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/test_facets.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/test_internal_locations.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/test_internal_locations.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/test_loaders.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/test_loaders.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/test_metadata_extensions.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/test_metadata_extensions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/test_notifications.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/test_notifications.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/test_notifications_mails.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/test_notifications_mails.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/test_notifications_permissions.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/test_notifications_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/test_patrons.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/test_patrons.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/test_record_delete.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/test_record_delete.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/test_record_permissions.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/test_record_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/test_resolvers.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/test_resolvers.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/test_stats.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/test_stats.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/test_tasks.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/test_tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/api/ils/test_vocabularies.py` & `invenio-app-ils-1.0.0rc4/tests/api/ils/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/conftest.py` & `invenio-app-ils-1.0.0rc4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/data/acq_orders.json` & `invenio-app-ils-1.0.0rc4/tests/data/acq_orders.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/data/document_requests.json` & `invenio-app-ils-1.0.0rc4/tests/data/document_requests.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/data/documents.json` & `invenio-app-ils-1.0.0rc4/tests/data/documents.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/data/eitems.json` & `invenio-app-ils-1.0.0rc4/tests/data/eitems.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/data/ill_borrowing_requests.json` & `invenio-app-ils-1.0.0rc4/tests/data/ill_borrowing_requests.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/data/items.json` & `invenio-app-ils-1.0.0rc4/tests/data/items.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/data/loans.json` & `invenio-app-ils-1.0.0rc4/tests/data/loans.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/data/loans_most_loaned.json` & `invenio-app-ils-1.0.0rc4/tests/data/loans_most_loaned.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/data/locations.json` & `invenio-app-ils-1.0.0rc4/tests/data/locations.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/data/series.json` & `invenio-app-ils-1.0.0rc4/tests/data/series.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/helpers.py` & `invenio-app-ils-1.0.0rc4/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-1.0.0rc3/tests/test_post_logout_redirect.py` & `invenio-app-ils-1.0.0rc4/tests/test_post_logout_redirect.py`

 * *Files identical despite different names*

