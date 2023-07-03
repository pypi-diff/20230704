# Comparing `tmp/vbcore-2.0.0rc4.tar.gz` & `tmp/vbcore-2.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbcore-2.0.0rc4.tar", last modified: Sun Jun  4 21:26:28 2023, max compression
+gzip compressed data, was "vbcore-2.1.0rc0.tar", last modified: Mon Jul  3 22:48:18 2023, max compression
```

## Comparing `vbcore-2.0.0rc4.tar` & `vbcore-2.1.0rc0.tar`

### file list

```diff
@@ -1,164 +1,204 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.746931 vbcore-2.0.0rc4/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      402 2023-06-04 21:26:28.746931 vbcore-2.0.0rc4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.731931 vbcore-2.0.0rc4/requirements/
--rw-rw-rw-   0 root         (0) root         (0)      222 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-all.in
--rw-rw-rw-   0 root         (0) root         (0)     5238 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-all.txt
--rw-rw-rw-   0 root         (0) root         (0)      245 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-build.in
--rw-rw-rw-   0 root         (0) root         (0)     2092 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-build.txt
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-crypto.in
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-crypto.txt
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-db.in
--rw-rw-rw-   0 root         (0) root         (0)      606 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-db.txt
--rw-rw-rw-   0 root         (0) root         (0)      419 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-dev.in
--rw-rw-rw-   0 root         (0) root         (0)     5559 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-extra.in
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-extra.txt
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-http.in
--rw-rw-rw-   0 root         (0) root         (0)     1142 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-http.txt
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-net.in
--rw-rw-rw-   0 root         (0) root         (0)      945 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-net.txt
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-scheduler.in
--rw-rw-rw-   0 root         (0) root         (0)      694 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-scheduler.txt
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-test.in
--rw-rw-rw-   0 root         (0) root         (0)     1754 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-04 21:26:28.746931 vbcore-2.0.0rc4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4745 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.734931 vbcore-2.0.0rc4/vbcore/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     1686 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/aio.py
--rw-rw-rw-   0 root         (0) root         (0)     4713 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/base.py
--rw-rw-rw-   0 root         (0) root         (0)     7460 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/batch.py
--rw-rw-rw-   0 root         (0) root         (0)     1396 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/configurator.py
--rw-rw-rw-   0 root         (0) root         (0)     7979 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/crc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.736931 vbcore-2.0.0rc4/vbcore/crypto/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/crypto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1266 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/crypto/argon.py
--rw-rw-rw-   0 root         (0) root         (0)      942 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/crypto/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1093 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/crypto/bcrypt.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/crypto/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1193 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/crypto/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1213 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/crypto/hashes.py
--rw-rw-rw-   0 root         (0) root         (0)     3369 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/csvfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.736931 vbcore-2.0.0rc4/vbcore/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.736931 vbcore-2.0.0rc4/vbcore/data/transformations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/data/transformations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.737931 vbcore-2.0.0rc4/vbcore/data/transformations/builders/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/data/transformations/builders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/data/transformations/builders/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2026 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/data/transformations/builders/csv.py
--rw-rw-rw-   0 root         (0) root         (0)     5586 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/data/transformations/builders/dicttoxml.py
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/data/transformations/builders/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     5880 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/data/transformations/builders/html.py
--rw-rw-rw-   0 root         (0) root         (0)     1908 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/data/transformations/builders/json.py
--rw-rw-rw-   0 root         (0) root         (0)     2230 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/data/transformations/builders/xml.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/data/transformations/builders/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.738931 vbcore-2.0.0rc4/vbcore/datastruct/
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/datastruct/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1108 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/datastruct/buffer.py
--rw-rw-rw-   0 root         (0) root         (0)     6012 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/datastruct/cache.py
--rw-rw-rw-   0 root         (0) root         (0)     2767 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/datastruct/dictionaries.py
--rw-rw-rw-   0 root         (0) root         (0)     2772 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/datastruct/lazy.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/datastruct/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     1156 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/datastruct/orderer_set.py
--rw-rw-rw-   0 root         (0) root         (0)     4400 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/date_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.740931 vbcore-2.0.0rc4/vbcore/db/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15794 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/db/events.py
--rw-rw-rw-   0 root         (0) root         (0)     4935 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/db/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2866 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/db/listener.py
--rw-rw-rw-   0 root         (0) root         (0)     2861 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/db/mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     6775 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/db/mysql_dumper.py
--rw-rw-rw-   0 root         (0) root         (0)     1826 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/db/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     4076 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/db/sqla.py
--rw-rw-rw-   0 root         (0) root         (0)     5471 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/db/support.py
--rw-rw-rw-   0 root         (0) root         (0)     2318 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/db/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.740931 vbcore-2.0.0rc4/vbcore/dictutils/
--rw-rw-rw-   0 root         (0) root         (0)      210 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/dictutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15745 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/dictutils/flatter_dict.py
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/dictutils/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     1032 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2190 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/enums.py
--rw-rw-rw-   0 root         (0) root         (0)      730 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3883 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3901 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/files.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.741931 vbcore-2.0.0rc4/vbcore/http/
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2938 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/http/batch.py
--rw-rw-rw-   0 root         (0) root         (0)     8176 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/http/client.py
--rw-rw-rw-   0 root         (0) root         (0)     3880 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/http/gql.py
--rw-rw-rw-   0 root         (0) root         (0)     3367 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/http/headers.py
--rw-rw-rw-   0 root         (0) root         (0)     2632 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/http/httpcode.py
--rw-rw-rw-   0 root         (0) root         (0)     4012 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/http/httpdumper.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/http/methods.py
--rw-rw-rw-   0 root         (0) root         (0)     6063 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/http/proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     1894 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/http/rpc.py
--rw-rw-rw-   0 root         (0) root         (0)     2128 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/http/useragent.py
--rw-rw-rw-   0 root         (0) root         (0)     4631 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/importer.py
--rw-rw-rw-   0 root         (0) root         (0)     6034 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.742931 vbcore-2.0.0rc4/vbcore/jsonschema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/jsonschema/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.742931 vbcore-2.0.0rc4/vbcore/jsonschema/schemas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/jsonschema/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2118 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/jsonschema/schemas/jsonrpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7052 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/jsonschema/support.py
--rw-rw-rw-   0 root         (0) root         (0)     2533 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/lambdas.py
--rw-rw-rw-   0 root         (0) root         (0)     2524 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/loggers.py
--rw-rw-rw-   0 root         (0) root         (0)     4108 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/misc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.743931 vbcore-2.0.0rc4/vbcore/net/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/net/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/net/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     5873 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/net/sendmail.py
--rw-rw-rw-   0 root         (0) root         (0)     3541 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/net/sftp.py
--rw-rw-rw-   0 root         (0) root         (0)     1566 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/net/socks_smtp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.743931 vbcore-2.0.0rc4/vbcore/rule_engine/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/rule_engine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/rule_engine/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3220 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/rule_engine/engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.743931 vbcore-2.0.0rc4/vbcore/standalone/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/standalone/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3335 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/standalone/scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)     9057 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/standalone/wsgi_gunicorn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.744931 vbcore-2.0.0rc4/vbcore/stringutils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/stringutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1226 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/stringutils/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     2158 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/stringutils/notations.py
--rw-rw-rw-   0 root         (0) root         (0)     4449 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.745931 vbcore-2.0.0rc4/vbcore/tester/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tester/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16074 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tester/asserter.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tester/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1455 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tester/fetchmail.py
--rw-rw-rw-   0 root         (0) root         (0)     1963 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tester/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     7405 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tester/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.745931 vbcore-2.0.0rc4/vbcore/tester/plugins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tester/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tester/plugins/fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tester/plugins/startup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.746931 vbcore-2.0.0rc4/vbcore/tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5840 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tools/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      948 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tools/crypto.py
--rw-rw-rw-   0 root         (0) root         (0)     2227 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tools/database.py
--rw-rw-rw-   0 root         (0) root         (0)      699 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tools/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.746931 vbcore-2.0.0rc4/vbcore/tools/initializer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tools/initializer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1104 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tools/initializer/init.py
--rw-rw-rw-   0 root         (0) root         (0)      765 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tools/scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/types.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/version.py
--rw-rw-rw-   0 root         (0) root         (0)     2877 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.735931 vbcore-2.0.0rc4/vbcore.egg-info/
--rw-r--r--   0 root         (0) root         (0)      402 2023-06-04 21:26:28.000000 vbcore-2.0.0rc4/vbcore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3800 2023-06-04 21:26:28.000000 vbcore-2.0.0rc4/vbcore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 21:26:28.000000 vbcore-2.0.0rc4/vbcore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-06-04 21:26:28.000000 vbcore-2.0.0rc4/vbcore.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 21:26:28.000000 vbcore-2.0.0rc4/vbcore.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      584 2023-06-04 21:26:28.000000 vbcore-2.0.0rc4/vbcore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-04 21:26:28.000000 vbcore-2.0.0rc4/vbcore.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.827467 vbcore-2.1.0rc0/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      402 2023-07-03 22:48:18.827467 vbcore-2.1.0rc0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.806467 vbcore-2.1.0rc0/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)      222 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-all.in
+-rw-rw-rw-   0 root         (0) root         (0)     5202 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-all.txt
+-rw-rw-rw-   0 root         (0) root         (0)      245 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-build.in
+-rw-rw-rw-   0 root         (0) root         (0)     2093 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-build.txt
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-crypto.in
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-crypto.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-db.in
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-db.txt
+-rw-rw-rw-   0 root         (0) root         (0)      384 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-dev.in
+-rw-rw-rw-   0 root         (0) root         (0)     5233 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-extra.in
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-extra.txt
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-http.in
+-rw-rw-rw-   0 root         (0) root         (0)     1142 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-http.txt
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-net.in
+-rw-rw-rw-   0 root         (0) root         (0)      945 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-net.txt
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-scheduler.in
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-scheduler.txt
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-test.in
+-rw-rw-rw-   0 root         (0) root         (0)     1755 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 22:48:18.827467 vbcore-2.1.0rc0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4745 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.809467 vbcore-2.1.0rc0/vbcore/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     4716 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7460 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/batch.py
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/configurator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.811467 vbcore-2.1.0rc0/vbcore/crypto/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/crypto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1266 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/crypto/argon.py
+-rw-rw-rw-   0 root         (0) root         (0)      942 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/crypto/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1093 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/crypto/bcrypt.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/crypto/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/crypto/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/crypto/hashes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4635 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/csvfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.811467 vbcore-2.1.0rc0/vbcore/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.812467 vbcore-2.1.0rc0/vbcore/data/transformations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/data/transformations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.813467 vbcore-2.1.0rc0/vbcore/data/transformations/builders/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/data/transformations/builders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/data/transformations/builders/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2026 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/data/transformations/builders/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)     5586 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/data/transformations/builders/dicttoxml.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/data/transformations/builders/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5880 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/data/transformations/builders/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/data/transformations/builders/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2230 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/data/transformations/builders/xml.py
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/data/transformations/builders/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.814467 vbcore-2.1.0rc0/vbcore/datastruct/
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/datastruct/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/datastruct/buffer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6158 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/datastruct/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     2904 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/datastruct/dictionaries.py
+-rw-rw-rw-   0 root         (0) root         (0)     2772 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/datastruct/lazy.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/datastruct/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/datastruct/orderer_set.py
+-rw-rw-rw-   0 root         (0) root         (0)     4400 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/date_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.815467 vbcore-2.1.0rc0/vbcore/db/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15840 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/db/events.py
+-rw-rw-rw-   0 root         (0) root         (0)     4935 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/db/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/db/listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     2997 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/db/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     6775 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/db/mysql_dumper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1826 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/db/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4942 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/db/sqla.py
+-rw-rw-rw-   0 root         (0) root         (0)     5600 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/db/support.py
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/db/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.816467 vbcore-2.1.0rc0/vbcore/dictutils/
+-rw-rw-rw-   0 root         (0) root         (0)      210 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/dictutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15745 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/dictutils/flatter_dict.py
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/dictutils/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2350 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3883 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3901 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.817467 vbcore-2.1.0rc0/vbcore/http/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2938 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/http/batch.py
+-rw-rw-rw-   0 root         (0) root         (0)     8181 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/http/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3880 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/http/gql.py
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/http/headers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2632 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/http/httpcode.py
+-rw-rw-rw-   0 root         (0) root         (0)     4012 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/http/httpdumper.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/http/methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     6063 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/http/proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1894 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/http/rpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2128 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/http/useragent.py
+-rw-rw-rw-   0 root         (0) root         (0)     4631 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/importer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5279 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.817467 vbcore-2.1.0rc0/vbcore/jsonschema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/jsonschema/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.818467 vbcore-2.1.0rc0/vbcore/jsonschema/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/jsonschema/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2118 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/jsonschema/schemas/jsonrpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7052 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/jsonschema/support.py
+-rw-rw-rw-   0 root         (0) root         (0)     2533 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/lambdas.py
+-rw-rw-rw-   0 root         (0) root         (0)     5111 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/loggers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5173 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/misc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.818467 vbcore-2.1.0rc0/vbcore/net/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/net/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/net/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5747 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/net/sendmail.py
+-rw-rw-rw-   0 root         (0) root         (0)     5984 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/net/sftp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/net/socks_smtp.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.819467 vbcore-2.1.0rc0/vbcore/rule_engine/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/rule_engine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/rule_engine/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3171 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/rule_engine/engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.819467 vbcore-2.1.0rc0/vbcore/standalone/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/standalone/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3310 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/standalone/scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)     8327 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/standalone/wsgi_gunicorn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.819467 vbcore-2.1.0rc0/vbcore/stringutils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/stringutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1226 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/stringutils/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2158 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/stringutils/notations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4449 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.820467 vbcore-2.1.0rc0/vbcore/tester/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tester/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16074 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tester/asserter.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tester/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tester/fetchmail.py
+-rw-rw-rw-   0 root         (0) root         (0)     1963 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tester/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     7405 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tester/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.821467 vbcore-2.1.0rc0/vbcore/tester/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tester/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tester/plugins/fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tester/plugins/startup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.822467 vbcore-2.1.0rc0/vbcore/tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6170 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      948 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/crypto.py
+-rw-rw-rw-   0 root         (0) root         (0)     2111 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.822467 vbcore-2.1.0rc0/vbcore/tools/initializer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.824467 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/.bumpversion.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/.dockerignore
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/.editorconfig
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/.flake8
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.824467 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/.git-hooks/
+-rwxrwxrwx   0 root         (0) root         (0)      179 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/.git-hooks/pre-commit
+-rwxrwxrwx   0 root         (0) root         (0)       30 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/.git-hooks/pre-push
+-rw-rw-rw-   0 root         (0) root         (0)     2205 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)    16254 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     4464 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.825466 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/devops/
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/devops/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)     2091 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/devops/gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.825466 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/devops/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/devops/scripts/build.sh
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/devops/scripts/dist-publish.sh
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/devops/scripts/fresh-install.sh
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/devops/scripts/test-builds.sh
+-rw-rw-rw-   0 root         (0) root         (0)      801 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/liccheck.ini
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.826467 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/requirements/requirements-build.in
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/requirements/requirements-dev.in
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/requirements/requirements-test.in
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/requirements/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)     3738 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.826467 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/skel/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/skel/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.826467 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/skel/entrypoints/
+-rw-rw-rw-   0 root         (0) root         (0)      419 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/skel/entrypoints/main.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/skel/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/skel/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/tox.ini
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1520 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/sendmail.py
+-rw-rw-rw-   0 root         (0) root         (0)     2745 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/sftp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/wsgi_gunicorn.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2877 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.810467 vbcore-2.1.0rc0/vbcore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      402 2023-07-03 22:48:18.000000 vbcore-2.1.0rc0/vbcore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5458 2023-07-03 22:48:18.000000 vbcore-2.1.0rc0/vbcore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 22:48:18.000000 vbcore-2.1.0rc0/vbcore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-03 22:48:18.000000 vbcore-2.1.0rc0/vbcore.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 22:48:18.000000 vbcore-2.1.0rc0/vbcore.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      590 2023-07-03 22:48:18.000000 vbcore-2.1.0rc0/vbcore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-03 22:48:18.000000 vbcore-2.1.0rc0/vbcore.egg-info/top_level.txt
```

### Comparing `vbcore-2.0.0rc4/requirements/requirements-all.txt` & `vbcore-2.1.0rc0/requirements/requirements-all.txt`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     #   -r requirements/requirements-extra.txt
     #   gql
 bcrypt==4.0.1
     # via
     #   -r requirements/requirements-crypto.txt
     #   -r requirements/requirements-net.txt
     #   paramiko
+bson==0.5.10
+    # via -r requirements/requirements.txt
 certifi==2023.5.7
     # via
     #   -r requirements/requirements-http.txt
     #   requests
 cffi==1.15.1
     # via
     #   -r requirements/requirements-crypto.txt
@@ -53,15 +55,15 @@
 charset-normalizer==2.1.1
     # via
     #   -r requirements/requirements-http.txt
     #   aiohttp
     #   requests
 click==8.1.3
     # via -r requirements/requirements.txt
-cryptography==40.0.2
+cryptography==41.0.1
     # via
     #   -r requirements/requirements-net.txt
     #   paramiko
 defusedxml==0.7.1
     # via -r requirements/requirements-extra.txt
 dnspython==2.3.0
     # via
@@ -97,15 +99,15 @@
     # via -r requirements/requirements-extra.txt
 multidict==6.0.4
     # via
     #   -r requirements/requirements-extra.txt
     #   -r requirements/requirements-http.txt
     #   aiohttp
     #   yarl
-paramiko==3.1.0
+paramiko==3.2.0
     # via -r requirements/requirements-net.txt
 ply==3.11
     # via
     #   -r requirements/requirements-extra.txt
     #   rule-engine
 psutil==5.9.5
     # via -r requirements/requirements.txt
@@ -118,70 +120,68 @@
     # via
     #   -r requirements/requirements-db.txt
     #   sqlalchemy-schemadisplay
 pynacl==1.5.0
     # via
     #   -r requirements/requirements-net.txt
     #   paramiko
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via
     #   -r requirements/requirements-db.txt
     #   pydot
 pyrsistent==0.19.3
     # via
     #   -r requirements/requirements-extra.txt
     #   jsonschema
 pysocks==1.7.1
     # via -r requirements/requirements-net.txt
 python-dateutil==2.8.2
     # via
     #   -r requirements/requirements-extra.txt
     #   -r requirements/requirements.txt
+    #   bson
     #   rule-engine
 python-decouple==3.8
     # via -r requirements/requirements.txt
 python-dotenv==1.0.0
     # via -r requirements/requirements.txt
 pytz==2023.3
     # via
     #   -r requirements/requirements-scheduler.txt
     #   apscheduler
-pytz-deprecation-shim==0.1.0.post0
-    # via
-    #   -r requirements/requirements-scheduler.txt
-    #   tzlocal
 pyyaml==6.0
     # via -r requirements/requirements.txt
-requests==2.30.0
+requests==2.31.0
     # via -r requirements/requirements-http.txt
-rule-engine==3.5.1
+rule-engine==3.6.0
     # via -r requirements/requirements-extra.txt
 six==1.16.0
     # via
     #   -r requirements/requirements-scheduler.txt
     #   -r requirements/requirements.txt
     #   apscheduler
+    #   bson
     #   python-dateutil
-sqlalchemy==1.4.48
+sqlalchemy==2.0.17
     # via -r requirements/requirements-db.txt
 sqlalchemy-schemadisplay==1.3
     # via -r requirements/requirements-db.txt
-tzdata==2023.3
+typing-extensions==4.7.0
     # via
-    #   -r requirements/requirements-scheduler.txt
-    #   pytz-deprecation-shim
-tzlocal==4.3
+    #   -r requirements/requirements-db.txt
+    #   sqlalchemy
+tzlocal==5.0.1
     # via
     #   -r requirements/requirements-scheduler.txt
     #   apscheduler
 ua-parser==0.16.1
     # via
     #   -r requirements/requirements-http.txt
     #   user-agents
-urllib3==2.0.2
+urllib3==2.0.3
     # via
     #   -r requirements/requirements-http.txt
     #   requests
 user-agents==2.2.0
     # via -r requirements/requirements-http.txt
 xmltodict==0.13.0
     # via -r requirements/requirements-extra.txt
```

### Comparing `vbcore-2.0.0rc4/requirements/requirements-build.txt` & `vbcore-2.1.0rc0/requirements/requirements-build.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,107 +2,107 @@
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-build.txt --resolver=backtracking requirements/requirements-build.in
 #
 bleach==6.0.0
     # via readme-renderer
-cachetools==5.3.0
+cachetools==5.3.1
     # via tox
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via cryptography
 chardet==5.1.0
     # via tox
 charset-normalizer==2.1.1
     # via
     #   -r requirements/requirements-build.in
     #   requests
 colorama==0.4.6
     # via tox
-cryptography==40.0.2
+cryptography==41.0.1
     # via secretstorage
 distlib==0.3.6
     # via virtualenv
-docutils==0.20
+docutils==0.20.1
     # via readme-renderer
-filelock==3.12.0
+filelock==3.12.2
     # via
     #   tox
     #   virtualenv
 idna==3.4
     # via requests
-importlib-metadata==6.6.0
+importlib-metadata==6.7.0
     # via
     #   keyring
     #   twine
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
-keyring==23.13.1
+keyring==24.2.0
     # via twine
-markdown-it-py==2.2.0
+markdown-it-py==3.0.0
     # via rich
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 packaging==23.1
     # via
     #   pyproject-api
     #   tox
 pkginfo==1.9.6
     # via twine
-platformdirs==3.5.1
+platformdirs==3.8.0
     # via
     #   tox
     #   virtualenv
-pluggy==1.0.0
+pluggy==1.2.0
     # via tox
 pycparser==2.21
     # via cffi
 pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
-pyproject-api==1.5.1
+pyproject-api==1.5.2
     # via tox
-readme-renderer==37.3
+readme-renderer==40.0
     # via twine
-requests==2.30.0
+requests==2.31.0
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.3.5
+rich==13.4.2
     # via twine
 secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via bleach
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
-tox==4.5.1
+tox==4.6.3
     # via -r requirements/requirements-build.in
 twine==4.0.2
     # via -r requirements/requirements-build.in
-urllib3==2.0.2
+urllib3==2.0.3
     # via
     #   requests
     #   twine
-virtualenv==20.23.0
+virtualenv==20.23.1
     # via tox
 webencodings==0.5.1
     # via bleach
 wheel==0.40.0
     # via -r requirements/requirements-build.in
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `vbcore-2.0.0rc4/requirements/requirements-crypto.txt` & `vbcore-2.1.0rc0/requirements/requirements-crypto.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/requirements/requirements-db.txt` & `vbcore-2.1.0rc0/requirements/requirements-db.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 #
 #    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-db.txt --resolver=backtracking requirements/requirements-db.in
 #
 greenlet==2.0.2
     # via sqlalchemy
 pydot==1.4.2
     # via sqlalchemy-schemadisplay
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via pydot
-sqlalchemy==1.4.48
+sqlalchemy==2.0.17
     # via -r requirements/requirements-db.in
 sqlalchemy-schemadisplay==1.3
     # via -r requirements/requirements-db.in
+typing-extensions==4.7.0
+    # via sqlalchemy
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `vbcore-2.0.0rc4/requirements/requirements-dev.txt` & `vbcore-2.1.0rc0/requirements/requirements-dev.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-dev.txt --resolver=backtracking requirements/requirements-dev.in
 #
-astroid==2.15.4
+astroid==2.15.5
     # via pylint
 attrs==23.1.0
     # via
     #   -c requirements/requirements-test.txt
     #   flake8-bugbear
-autoflake==2.1.1
+autoflake==2.2.0
     # via -r requirements/requirements-dev.in
 bandit==1.7.5
     # via -r requirements/requirements-dev.in
 black==23.3.0
     # via -r requirements/requirements-dev.in
 build==0.10.0
     # via pip-tools
@@ -42,36 +42,32 @@
     # via
     #   -c requirements/requirements-build.txt
     #   radon
 coloredlogs==15.0.1
     # via -r requirements/requirements-dev.in
 configparser==5.3.0
     # via liccheck
-cryptography==40.0.2
+cryptography==41.0.1
     # via
     #   -c requirements/requirements-build.txt
     #   types-paramiko
 dill==0.3.6
     # via pylint
-dparse==0.6.2
+dparse==0.6.3
     # via safety
 flake8==6.0.0
     # via
     #   -r requirements/requirements-dev.in
     #   flake8-bugbear
-flake8-bugbear==23.5.9
+flake8-bugbear==23.6.5
     # via -r requirements/requirements-dev.in
 gitdb==4.0.10
     # via gitpython
 gitpython==3.1.31
     # via bandit
-greenlet==2.0.2
-    # via
-    #   -c requirements/requirements-all.txt
-    #   sqlalchemy
 humanfriendly==10.0
     # via coloredlogs
 idna==3.4
     # via
     #   -c requirements/requirements-test.txt
     #   requests
 isort==5.12.0
@@ -80,31 +76,28 @@
     #   pylint
 lazy-object-proxy==1.9.0
     # via astroid
 liccheck==0.9.1
     # via -r requirements/requirements-dev.in
 mando==0.7.1
     # via radon
-markdown-it-py==2.2.0
+markdown-it-py==3.0.0
     # via
     #   -c requirements/requirements-build.txt
     #   rich
 mccabe==0.7.0
     # via
     #   flake8
     #   pylint
 mdurl==0.1.2
     # via
     #   -c requirements/requirements-build.txt
     #   markdown-it-py
 mypy==0.991
-    # via
-    #   -r requirements/requirements-dev.in
-    #   sqlalchemy
-    #   sqlalchemy-stubs
+    # via -r requirements/requirements-dev.in
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
 packaging==23.1
     # via
     #   -c requirements/requirements-test.txt
@@ -112,19 +105,19 @@
     #   build
     #   dparse
     #   safety
 pathspec==0.11.1
     # via black
 pbr==5.11.1
     # via stevedore
-pip-tools==6.13.0
+pip-tools==6.14.0
     # via -r requirements/requirements-dev.in
-pipdeptree==2.7.1
+pipdeptree==2.9.3
     # via -r requirements/requirements-dev.in
-platformdirs==3.5.1
+platformdirs==3.8.0
     # via
     #   -c requirements/requirements-build.txt
     #   black
     #   pylint
 pycodestyle==2.10.0
     # via flake8
 pycparser==2.21
@@ -145,88 +138,81 @@
     # via build
 pyyaml==6.0
     # via
     #   -c requirements/requirements-test.txt
     #   bandit
 radon==6.0.1
     # via -r requirements/requirements-dev.in
-requests==2.30.0
+requests==2.31.0
     # via
     #   -c requirements/requirements-test.txt
     #   safety
-rich==13.3.5
+rich==13.4.2
     # via
     #   -c requirements/requirements-build.txt
     #   bandit
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.32
     # via safety
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 safety==2.3.4
     # via -r requirements/requirements-dev.in
 semantic-version==2.10.0
     # via liccheck
 six==1.16.0
     # via
     #   -c requirements/requirements-build.txt
     #   mando
 smmap==5.0.0
     # via gitdb
-sqlalchemy[mypy]==1.4.48
-    # via -r requirements/requirements-dev.in
-sqlalchemy-stubs==0.4
-    # via -r requirements/requirements-dev.in
-sqlalchemy2-stubs==0.0.2a34
-    # via sqlalchemy
-stevedore==5.0.0
+stevedore==5.1.0
     # via bandit
 toml==0.10.2
-    # via
-    #   dparse
-    #   liccheck
+    # via liccheck
 tomli==2.0.1
     # via
     #   -c requirements/requirements-test.txt
     #   autoflake
     #   black
     #   build
+    #   dparse
     #   mypy
+    #   pip-tools
     #   pylint
     #   pyproject-hooks
 tomlkit==0.11.8
     # via pylint
 types-backports==0.1.3
     # via -r requirements/requirements-dev.in
 types-chardet==5.0.4.6
     # via -r requirements/requirements-dev.in
-types-paramiko==3.0.0.10
+types-paramiko==3.2.0.0
     # via -r requirements/requirements-dev.in
 types-python-dateutil==2.8.19.13
     # via -r requirements/requirements-dev.in
 types-pytz==2023.3.0.0
     # via -r requirements/requirements-dev.in
-types-pyyaml==6.0.12.9
+types-pyyaml==6.0.12.10
     # via -r requirements/requirements-dev.in
-types-requests==2.30.0.0
+types-requests==2.31.0.1
     # via -r requirements/requirements-dev.in
-types-setuptools==67.7.0.2
+types-setuptools==68.0.0.0
     # via -r requirements/requirements-dev.in
 types-toml==0.10.8.6
     # via -r requirements/requirements-dev.in
 types-urllib3==1.26.25.13
     # via types-requests
 types-xmltodict==0.13.0.2
     # via -r requirements/requirements-dev.in
-typing-extensions==4.5.0
+typing-extensions==4.7.0
     # via
+    #   -c requirements/requirements-all.txt
     #   astroid
     #   mypy
-    #   sqlalchemy-stubs
-    #   sqlalchemy2-stubs
-urllib3==2.0.2
+urllib3==2.0.3
     # via
     #   -c requirements/requirements-test.txt
     #   requests
 wheel==0.40.0
     # via
     #   -c requirements/requirements-build.txt
     #   pip-tools
```

### Comparing `vbcore-2.0.0rc4/requirements/requirements-extra.txt` & `vbcore-2.1.0rc0/requirements/requirements-extra.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     # via rule-engine
 pyrsistent==0.19.3
     # via jsonschema
 python-dateutil==2.8.2
     # via
     #   -c requirements/requirements.txt
     #   rule-engine
-rule-engine==3.5.1
+rule-engine==3.6.0
     # via -r requirements/requirements-extra.in
 six==1.16.0
     # via
     #   -c requirements/requirements-build.txt
     #   python-dateutil
 xmltodict==0.13.0
     # via -r requirements/requirements-extra.in
```

### Comparing `vbcore-2.0.0rc4/requirements/requirements-http.txt` & `vbcore-2.1.0rc0/requirements/requirements-http.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,19 +30,19 @@
     #   -c requirements/requirements-build.txt
     #   requests
     #   yarl
 multidict==6.0.4
     # via
     #   aiohttp
     #   yarl
-requests==2.30.0
+requests==2.31.0
     # via -r requirements/requirements-http.in
 ua-parser==0.16.1
     # via user-agents
-urllib3==2.0.2
+urllib3==2.0.3
     # via
     #   -c requirements/requirements-build.txt
     #   requests
 user-agents==2.2.0
     # via -r requirements/requirements-http.in
 yarl==1.9.2
     # via aiohttp
```

### Comparing `vbcore-2.0.0rc4/requirements/requirements-net.txt` & `vbcore-2.1.0rc0/requirements/requirements-net.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 bcrypt==4.0.1
     # via paramiko
 cffi==1.15.1
     # via
     #   -c requirements/requirements-build.txt
     #   cryptography
     #   pynacl
-cryptography==40.0.2
+cryptography==41.0.1
     # via
     #   -c requirements/requirements-build.txt
     #   paramiko
 dnspython==2.3.0
     # via email-validator
 email-validator==2.0.0.post2
     # via -r requirements/requirements-net.in
 idna==3.4
     # via
     #   -c requirements/requirements-build.txt
     #   email-validator
-paramiko==3.1.0
+paramiko==3.2.0
     # via -r requirements/requirements-net.in
 pycparser==2.21
     # via
     #   -c requirements/requirements-build.txt
     #   cffi
 pynacl==1.5.0
     # via paramiko
```

### Comparing `vbcore-2.0.0rc4/requirements/requirements-scheduler.txt` & `vbcore-2.1.0rc0/requirements/requirements.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-scheduler.txt --resolver=backtracking requirements/requirements-scheduler.in
+#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements.txt --resolver=backtracking requirements/requirements.in
 #
-apscheduler==3.10.1
-    # via -r requirements/requirements-scheduler.in
-pytz==2023.3
-    # via apscheduler
-pytz-deprecation-shim==0.1.0.post0
-    # via tzlocal
+bson==0.5.10
+    # via -r requirements/requirements.in
+click==8.1.3
+    # via -r requirements/requirements.in
+psutil==5.9.5
+    # via -r requirements/requirements.in
+python-dateutil==2.8.2
+    # via
+    #   -r requirements/requirements.in
+    #   bson
+python-decouple==3.8
+    # via -r requirements/requirements.in
+python-dotenv==1.0.0
+    # via -r requirements/requirements.in
+pyyaml==6.0
+    # via -r requirements/requirements.in
 six==1.16.0
     # via
     #   -c requirements/requirements-build.txt
-    #   apscheduler
-tzdata==2023.3
-    # via pytz-deprecation-shim
-tzlocal==4.3
-    # via apscheduler
-
-# The following packages are considered to be unsafe in a requirements file:
-# setuptools
+    #   bson
+    #   python-dateutil
```

### Comparing `vbcore-2.0.0rc4/requirements/requirements-test.txt` & `vbcore-2.1.0rc0/requirements/requirements-test.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,61 +12,61 @@
     # via
     #   -c requirements/requirements-build.txt
     #   requests
 charset-normalizer==2.1.1
     # via
     #   -c requirements/requirements-build.txt
     #   requests
-coverage[toml]==7.2.5
+coverage[toml]==7.2.7
     # via
     #   -r requirements/requirements-test.in
     #   pytest-cov
 exceptiongroup==1.1.1
     # via
     #   hypothesis
     #   pytest
-hypothesis==6.75.2
+hypothesis==6.80.0
     # via -r requirements/requirements-test.in
 idna==3.4
     # via
     #   -c requirements/requirements-build.txt
     #   requests
 iniconfig==2.0.0
     # via pytest
 packaging==23.1
     # via
     #   -c requirements/requirements-build.txt
     #   pytest
-pluggy==1.0.0
+pluggy==1.2.0
     # via
     #   -c requirements/requirements-build.txt
     #   pytest
-pytest==7.3.1
+pytest==7.4.0
     # via
     #   -r requirements/requirements-test.in
     #   pytest-cov
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via -r requirements/requirements-test.in
 pyyaml==6.0
     # via
     #   -c requirements/requirements-all.txt
     #   responses
-requests==2.30.0
+requests==2.31.0
     # via
     #   -c requirements/requirements-build.txt
     #   responses
 responses==0.23.1
     # via -r requirements/requirements-test.in
 sortedcontainers==2.4.0
     # via hypothesis
 tomli==2.0.1
     # via
     #   -c requirements/requirements-build.txt
     #   coverage
     #   pytest
-types-pyyaml==6.0.12.9
+types-pyyaml==6.0.12.10
     # via responses
-urllib3==2.0.2
+urllib3==2.0.3
     # via
     #   -c requirements/requirements-build.txt
     #   requests
     #   responses
```

### Comparing `vbcore-2.0.0rc4/setup.py` & `vbcore-2.1.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/aio.py` & `vbcore-2.1.0rc0/vbcore/aio.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/base.py` & `vbcore-2.1.0rc0/vbcore/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 if t.TYPE_CHECKING:
     # prevent mypy issue
 
     # noinspection PyPep8Naming
     from dataclasses import dataclass as Data
 else:
     # TODO at the moment this is not used because pycharm issue
-    Data = dataclasses.dataclass(frozen=True, kw_only=False)
+    Data = dataclasses.dataclass(frozen=True, kw_only=True)
 
 
-class LoggerMixin(t.Generic[LogClass], ABC):
+class LoggerMixin(ABC, t.Generic[LogClass]):
     @classmethod
     @abstractmethod
     def logger(cls, name: OptStr = None) -> LogClass:
         """returns the logger instance"""
 
     @cached_property
     def log(self) -> LogClass:
@@ -110,19 +110,19 @@
 
     >>> class MyStaticClass(metaclass=Static):
     ...     pass
     ...
     >>> MyStaticClass()
     Traceback (most recent call last):
         ...
-    TypeError: Can't instantiate Static class MyStaticClass
+    TypeError: can not instantiate Static class MyStaticClass
     """
 
     def __call__(cls):
-        raise TypeError(f"Can't instantiate Static class {cls.__name__}")
+        raise TypeError(f"can not instantiate Static class {cls.__name__}")
 
 
 class Decorator:
     def __call__(self, function: t.Callable) -> t.Any:
         @functools.wraps(function)
         def decorated(*args, **kwargs):
             return self.perform(function, *args, **kwargs)
```

### Comparing `vbcore-2.0.0rc4/vbcore/batch.py` & `vbcore-2.1.0rc0/vbcore/batch.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/configurator.py` & `vbcore-2.1.0rc0/vbcore/configurator.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/crypto/argon.py` & `vbcore-2.1.0rc0/vbcore/crypto/argon.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/crypto/base.py` & `vbcore-2.1.0rc0/vbcore/crypto/base.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/crypto/bcrypt.py` & `vbcore-2.1.0rc0/vbcore/crypto/bcrypt.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/crypto/factory.py` & `vbcore-2.1.0rc0/vbcore/crypto/factory.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/crypto/hashes.py` & `vbcore-2.1.0rc0/vbcore/crypto/hashes.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/data/transformations/builders/base.py` & `vbcore-2.1.0rc0/vbcore/data/transformations/builders/base.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/data/transformations/builders/csv.py` & `vbcore-2.1.0rc0/vbcore/data/transformations/builders/csv.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/data/transformations/builders/dicttoxml.py` & `vbcore-2.1.0rc0/vbcore/data/transformations/builders/dicttoxml.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/data/transformations/builders/factory.py` & `vbcore-2.1.0rc0/vbcore/data/transformations/builders/factory.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/data/transformations/builders/html.py` & `vbcore-2.1.0rc0/vbcore/data/transformations/builders/html.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/data/transformations/builders/json.py` & `vbcore-2.1.0rc0/vbcore/data/transformations/builders/json.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/data/transformations/builders/xml.py` & `vbcore-2.1.0rc0/vbcore/data/transformations/builders/xml.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/data/transformations/builders/yaml.py` & `vbcore-2.1.0rc0/vbcore/data/transformations/builders/yaml.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from dataclasses import dataclass
 
 import yaml
 
 from vbcore.base import BaseDTO
-from vbcore.types import OptAny, OptInt, OptStr
+from vbcore.types import OptAny, OptInt
 
 from .base import DictBuilder, RecordType
 
 
 # pylint: disable=too-many-instance-attributes
 @dataclass(frozen=True)
 class YAMLBuilderOptions(BaseDTO):
     default_flow_style: bool = False
     indent: OptInt = None
     width: OptInt = None
-    encoding: OptStr = None
+    encoding: str = "utf-8"
     sort_keys: bool = True
     default_style: OptAny = None
     canonical: OptAny = None
     allow_unicode: OptAny = None
     line_break: OptAny = None
     explicit_start: OptAny = None
     explicit_end: OptAny = None
@@ -27,15 +27,15 @@
 
 
 class YAMLBuilder(DictBuilder[YAMLBuilderOptions]):
     def to_dict(self, data: str) -> RecordType:
         return yaml.safe_load(data)
 
     def to_self(self, data: RecordType) -> str:
-        return yaml.safe_dump(
+        bytes_data = yaml.safe_dump(
             data,
             default_style=self.options.default_style,
             default_flow_style=self.options.default_flow_style,
             canonical=self.options.canonical,
             indent=self.options.indent,
             width=self.options.width,
             allow_unicode=self.options.allow_unicode,
@@ -43,7 +43,8 @@
             encoding=self.options.encoding,
             explicit_start=self.options.explicit_start,
             explicit_end=self.options.explicit_end,
             version=self.options.version,
             tags=self.options.tags,
             sort_keys=self.options.sort_keys,
         )
+        return bytes_data.decode(encoding=self.options.encoding)
```

### Comparing `vbcore-2.0.0rc4/vbcore/datastruct/buffer.py` & `vbcore-2.1.0rc0/vbcore/datastruct/buffer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,42 @@
 import typing as t
+from collections import deque
 
 T = t.TypeVar("T")
 
 
 class BufferManager(t.Generic[T]):
     def __init__(self, max_size: int = 0) -> None:
-        self._max_size = max_size
-        self._buffer: t.List[T] = []
-
-    @property
-    def buffer(self) -> t.List[T]:
-        return self._buffer
+        self.max_size = max_size
+        self._buffer: t.Deque[T] = deque(maxlen=max_size or None)
 
     @property
     def size(self) -> int:
-        return len(self.buffer)
+        return len(self._buffer)
 
     @property
     def is_full(self) -> bool:
-        return 0 < self._max_size <= self.size
+        return 0 < self.max_size <= self.size
 
     @property
     def is_empty(self) -> bool:
         return self.size == 0
 
     def pre_flush_hook(self) -> None:
         """Derived class can hook at flush time, so it can handle buffered data"""
 
     def clear(self) -> None:
-        self.buffer.clear()
+        self._buffer.clear()
 
-    def load(self, record: T) -> int:
+    def load(self, record: T) -> None:
         self._buffer.append(record)
         if self.is_full:
             self.flush()
-        return self.size
 
-    def loads(self, records: t.Iterable[T]) -> int:
+    def loads(self, records: t.Iterable[T]) -> None:
         for record in records:
             self.load(record)
-        return self.size
 
     def flush(self) -> None:
         if not self.is_empty:
             self.pre_flush_hook()
             self.clear()
```

### Comparing `vbcore-2.0.0rc4/vbcore/datastruct/cache.py` & `vbcore-2.1.0rc0/vbcore/datastruct/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,22 @@
 
         if len(self) > self.maxsize:
             oldest = next(iter(self))
             del self[oldest]
 
     def set(self, key, value):
         # pylint: disable=unnecessary-dunder-call
-        return self.__setitem__(key, value)
+        self[key] = value
+        return self[key]
+
+    def get(self, key, default=None):
+        try:
+            return self[key]
+        except AttributeError:
+            return default
 
 
 # based on: https://github.com/mailgun/expiringdict
 class ExpiringCache(OrderedDict):
     """
     Dictionary with auto-expiring values for caching purposes.
     Expiration happens on any access, object is locked during cleanup from expired
```

### Comparing `vbcore-2.0.0rc4/vbcore/datastruct/dictionaries.py` & `vbcore-2.1.0rc0/vbcore/datastruct/dictionaries.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 
 class HashableDict(dict):
     def __hash__(self):
         return hash(tuple(sorted(self.items())))
 
 
 class IDict(dict):
-    def patch(self: D, __dict: D, **kwargs) -> D:
-        super().update(__dict, **kwargs)
+    def patch(self: D, __dict: t.Optional[D] = None, **kwargs) -> D:
+        if __dict:
+            super().update(__dict)
+        else:
+            super().update(**kwargs)
         return self
 
     def get_namespace(
         self: D,
         prefix: str,
         lowercase: bool = True,
         trim: bool = True,
@@ -24,18 +27,19 @@
         Returns a dictionary containing a subset of configuration options
         that match the specified prefix.
 
         :param prefix: a configuration prefix
         :param lowercase: a flag indicating if the keys should be lowercase
         :param trim: a flag indicating if the keys should include the namespace
         """
+        _prefix = f"{prefix}_"
         data: D = self.__class__()
         for k, v in self.items():
-            if k.startswith(prefix):
-                key = k[len(prefix) :] if trim else k
+            if k.startswith(_prefix):
+                key = k[len(_prefix) :] if trim else k
                 data[key.lower() if lowercase else key] = v
         return data
 
 
 class ObjectDict(IDict):
     def __init__(self: OD, seq=None, **kwargs):
         super().__init__()
@@ -81,16 +85,17 @@
 class BDict(dict):
     @classmethod
     def from_dict(cls, data: dict) -> "BDict":
         return cls(**data)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.inverse = {v: k for k, v in self.items()}
+        # pylint: disable=invalid-name
+        self.T = {v: k for k, v in self.items()}
 
     def __setitem__(self, key, value):
         super().__setitem__(key, value)
-        self.inverse[value] = key
+        self.T[value] = key
 
     def __delitem__(self, key):
         super().__delitem__(key)
-        del self.inverse[self[key]]
+        del self.T[self[key]]
```

### Comparing `vbcore-2.0.0rc4/vbcore/datastruct/lazy.py` & `vbcore-2.1.0rc0/vbcore/datastruct/lazy.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/datastruct/orderer_set.py` & `vbcore-2.1.0rc0/vbcore/datastruct/orderer_set.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/date_helper.py` & `vbcore-2.1.0rc0/vbcore/date_helper.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/db/events.py` & `vbcore-2.1.0rc0/vbcore/db/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import collections
 import re
 import sys
 import typing as t
 from dataclasses import dataclass
 
 from sqlalchemy import exc as sqla_exc
-from sqlalchemy.engine.interfaces import ExceptionContext
+from sqlalchemy.engine import ExceptionContext
 from sqlalchemy.exc import DBAPIError
 
 from vbcore.db.exceptions import (
     DBConnectionError,
     DBConstraintError,
     DBDataError,
     DBDeadlock,
@@ -472,15 +472,16 @@
             and not context.connection.closed
             and not context.connection.invalidated
             and ROLLBACK_CAUSE_KEY in context.connection.info
         ):
             dbe.cause = context.connection.info.pop(ROLLBACK_CAUSE_KEY)  # type: ignore
 
         if isinstance(dbe, DBConnectionError):
-            context.is_disconnect = True
+            # noinspection PyDunderSlots
+            context.is_disconnect = True  # type: ignore
 
             if hasattr(context, "is_pre_ping") and context.is_pre_ping:
                 # if this is a pre-ping, need to integrate
                 # with the built-in pre-ping handler that doesn't know
                 # about DBConnectionError, just needs the updated status
                 return None
         return dbe
```

### Comparing `vbcore-2.0.0rc4/vbcore/db/exceptions.py` & `vbcore-2.1.0rc0/vbcore/db/exceptions.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/db/listener.py` & `vbcore-2.1.0rc0/vbcore/db/listener.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/db/mixins.py` & `vbcore-2.1.0rc0/vbcore/db/mixins.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import typing as t
 from functools import cached_property, partial
 
 import sqlalchemy as sa
-from sqlalchemy.ext.declarative import declared_attr
+from sqlalchemy.orm import Mapped, mapped_column
 
 from vbcore import json
 from vbcore.crypto.base import Hasher
 from vbcore.crypto.factory import CryptoFactory
+from vbcore.misc import get_uuid
 from vbcore.types import StrDict
-from vbcore.uuid import get_uuid
 
 if t.TYPE_CHECKING:
     hybrid_property = property  # pylint: disable=C0103
 else:
     from sqlalchemy.ext.hybrid import hybrid_property
 
 
@@ -47,30 +47,28 @@
 class StandardUuidMixin(BaseMixin):
     id = Column.uuid()
     created_at = Column.date_created()
     updated_at = Column.date_updated()
 
 
 class CatalogMixin(BaseMixin):
-    @declared_attr
-    def __table_args__(self) -> tuple:
-        return (sa.UniqueConstraint("code", "type_id"),)
-
-    id = sa.Column(sa.Integer, primary_key=True)
-    type_id = sa.Column(sa.Integer)
-    code = sa.Column(sa.String(100))
-    description = sa.Column(sa.Text())
-    order_id = sa.Column(sa.Integer, index=True)
+    __table_args__ = (sa.UniqueConstraint("code", "type_id"),)
+
+    id: Mapped[int] = mapped_column(sa.Integer, primary_key=True)
+    type_id: Mapped[int] = mapped_column(sa.Integer, nullable=True)
+    code: Mapped[str] = mapped_column(sa.String(100), nullable=False)
+    order_id: Mapped[str] = mapped_column(sa.Integer, nullable=True, index=True)
+    description: Mapped[str] = mapped_column(sa.Text(), nullable=True)
 
 
 class UserMixin(StandardMixin):
     _hasher_type: str = "ARGON2"
-    _password = sa.Column("password", sa.String(128), nullable=False)
+    _password: Mapped[str] = mapped_column("password", sa.String(128), nullable=False)
 
-    email = sa.Column(sa.String(255), unique=True, nullable=False)
+    email: Mapped[str] = mapped_column(sa.String(255), unique=True, nullable=False)
 
     @cached_property
     def hasher_instance(self) -> Hasher:
         return CryptoFactory.instance(self._hasher_type)
 
     @hybrid_property
     def password(self):
@@ -82,15 +80,15 @@
 
     def check_password(self, password):
         return self.hasher_instance.verify(self._password, password)
 
 
 class ExtraMixin(BaseMixin):
     _json_class = json
-    _extra: str = sa.Column(sa.Text())  # type: ignore
+    _extra: Mapped[str] = mapped_column(sa.Text())  # type: ignore
 
     @property
     def extra(self) -> t.Dict[str, t.Any]:
         return self._json_class.loads(self._extra) if self._extra else {}
 
     @extra.setter
     def extra(self, value: t.Optional[StrDict]):
```

### Comparing `vbcore-2.0.0rc4/vbcore/db/mysql_dumper.py` & `vbcore-2.1.0rc0/vbcore/db/mysql_dumper.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/db/schema.py` & `vbcore-2.1.0rc0/vbcore/db/schema.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/db/support.py` & `vbcore-2.1.0rc0/vbcore/db/support.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 from vbcore.db.events import ErrorsHandler
 from vbcore.db.sqla import Model
 from vbcore.db.views import DDLViewCompiler
 from vbcore.files import FileHandler
 from vbcore.types import StrTuple
 
+SynchronizeSessionArgument = t.Literal[False, "auto", "evaluate", "fetch"]
+
 
 class SQLASupport:
     def __init__(self, model: t.Type[Model], session: Session, commit: bool = True):
         """
         @param model: a model class
         @param session: a session object
         @param commit: enable auto commit
@@ -83,15 +85,15 @@
         @param kwargs: filters used to fetch record or create
         @return updated object and is_created flag
         """
         defaults = defaults or {}
         with self.session.begin_nested():
             try:
                 query = self.fetch().with_for_update()
-                obj = query.filter_by(**kwargs).one()
+                obj = query.filter_by(**kwargs).one()  # type: ignore
             except NoResultError:
                 params = self._prepare_params(defaults, **kwargs)
                 obj, created = self._create_object(kwargs, params, lock=True)
                 if created:
                     return obj, created
 
             for k, v in defaults.items():
@@ -102,15 +104,17 @@
 
         return obj, False
 
     def fetch(self, *args, fields: tuple = (), **kwargs) -> Query:
         columns = fields or (self.model,)
         return self.session.query(*columns).filter(*args).filter_by(**kwargs)
 
-    def delete(self, *args, synchronize: str = "evaluate", **kwargs) -> int:
+    def delete(
+        self, *args, synchronize: SynchronizeSessionArgument = "evaluate", **kwargs
+    ) -> int:
         row_count = self.fetch(*args, **kwargs).delete(synchronize)
         if self._commit:
             self.session.commit()
         return row_count
 
     def bulk_insert(self, records: t.Iterable[Model]) -> None:
         self.session.add_all(records)
```

### Comparing `vbcore-2.0.0rc4/vbcore/db/views.py` & `vbcore-2.1.0rc0/vbcore/db/views.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/dictutils/flatter_dict.py` & `vbcore-2.1.0rc0/vbcore/dictutils/flatter_dict.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/dispatcher.py` & `vbcore-2.1.0rc0/vbcore/dispatcher.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/enums.py` & `vbcore-2.1.0rc0/vbcore/enums.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 import enum
+from typing import List
 
 from vbcore.datastruct import ObjectDict
 from vbcore.types import CoupleStr
 
 
+class EnumMixin:
+    __members__: dict
+
+    @classmethod
+    def items(cls) -> List[str]:
+        return list(cls.__members__.keys())
+
+
 class IntEnum(enum.IntEnum):
     @classmethod
     def to_list(cls):
         return [
             ObjectDict(id=getattr(cls, m).value, label=getattr(cls, m).name)
             for m in cls.__members__
         ]
```

### Comparing `vbcore-2.0.0rc4/vbcore/factory.py` & `vbcore-2.1.0rc0/vbcore/factory.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/files.py` & `vbcore-2.1.0rc0/vbcore/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,19 +53,19 @@
 
 
 class FileHandler:
     def __init__(
         self,
         filename: OptStr = None,
         encoding: OptStr = None,
-        supporter_encodings: t.Sequence[str] = (),
+        supported_encodings: t.Sequence[str] = (),
     ):
         self.filename = filename
         self.encoding = encoding or "utf-8"
-        self.supporter_encodings = supporter_encodings
+        self.supported_encodings = supported_encodings
 
     def open(self, filename: OptStr = None, **kwargs) -> t.IO:
         encoding = kwargs.pop("encoding", self.encoding)
         return open(filename or self.filename, encoding=encoding, **kwargs)
 
     def open_binary(self, filename: OptStr = None, **kwargs) -> t.IO:
         return open(filename or self.filename, mode="rb", **kwargs)
@@ -99,15 +99,15 @@
 
     def check_encoding(
         self, filename: OptStr = None, extra_supported: t.Sequence[str] = ()
     ):
         encoding = self.detect_encoding(filename)
         supported_encodings = [
             self.encoding,
-            *self.supporter_encodings,
+            *self.supported_encodings,
             *extra_supported,
         ]
         if encoding.encoding not in supported_encodings:
             raise VBEncodingError(
                 filename,
                 encoding.encoding,
                 supported_encodings,
```

### Comparing `vbcore-2.0.0rc4/vbcore/http/batch.py` & `vbcore-2.1.0rc0/vbcore/http/batch.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/http/client.py` & `vbcore-2.1.0rc0/vbcore/http/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 import typing as t
 
 from requests import auth, exceptions as http_exc, request as send_request, Response
 
 from vbcore.datastruct import ObjectDict
 from vbcore.http.headers import HeaderEnum
-from vbcore.uuid import get_uuid
+from vbcore.misc import get_uuid
+from vbcore.types import OptStr
 
-from ..types import OptStr
 from . import httpcode
 from .httpdumper import LazyHTTPDumper
 from .methods import HttpMethod
 
 HTTPStatusError = (http_exc.HTTPError,)
 NetworkError = (http_exc.ConnectionError, http_exc.Timeout)
 all_errors = (*HTTPStatusError, *NetworkError)
```

### Comparing `vbcore-2.0.0rc4/vbcore/http/gql.py` & `vbcore-2.1.0rc0/vbcore/http/gql.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/http/headers.py` & `vbcore-2.1.0rc0/vbcore/http/headers.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/http/httpcode.py` & `vbcore-2.1.0rc0/vbcore/http/httpcode.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/http/httpdumper.py` & `vbcore-2.1.0rc0/vbcore/http/httpdumper.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/http/proxy.py` & `vbcore-2.1.0rc0/vbcore/http/proxy.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/http/rpc.py` & `vbcore-2.1.0rc0/vbcore/http/rpc.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/http/useragent.py` & `vbcore-2.1.0rc0/vbcore/http/useragent.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/importer.py` & `vbcore-2.1.0rc0/vbcore/importer.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/json.py` & `vbcore-2.1.0rc0/vbcore/json.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 import datetime
 import json
+import traceback
 import uuid
 from collections import Counter, defaultdict, deque, OrderedDict
 from decimal import Decimal
 from enum import Enum
 from types import SimpleNamespace
 from typing import Any, Callable, Optional, Type, Union
 
+from bson.objectid import InvalidId, ObjectId
+
 from vbcore.types import CoupleStr, OptInt
 
 OptCallableHook = Optional[Callable[[Any], Any]]
 
 JSONDecodeError = json.JSONDecodeError
 
 
-try:
-    # noinspection PyUnresolvedReferences
-    from bson import ObjectId
-    from bson.errors import InvalidId
-except ImportError:  # pragma: no cover
-    ObjectId = str
-    InvalidId = ValueError
-
-
 class SetsEncoderMixin(json.JSONEncoder):
     def default(self, o, *_, **__):
         if isinstance(o, (set, frozenset)):
             return list(o)
         return super().default(o)
 
 
@@ -64,28 +58,21 @@
 
 class CollectionsEncoderMixin(json.JSONEncoder):
     def default(self, o, *_, **__):
         if isinstance(o, deque):
             return list(o)
         if isinstance(o, (defaultdict, OrderedDict, Counter)):
             return dict(o)
-        try:
-            # check for namedtuple compliant
-            # noinspection PyProtectedMember
-            return o._asdict()
-        except AttributeError:
-            pass
-
         return super().default(o)
 
 
-class HexUUIDMixin(json.JSONEncoder):
+class UUIDMixin(json.JSONEncoder):
     def default(self, o, *_, **__):
         if isinstance(o, uuid.UUID):
-            return o.hex
+            return str(o)
         return super().default(o)
 
 
 class ObjectIdMixin(json.JSONEncoder):
     def default(self, o, *_, **__):
         if isinstance(o, ObjectId):
             return {"$oid": str(o)}
@@ -104,75 +91,59 @@
 
 
 class JsonEncoder(
     BuiltinEncoderMixin,
     DateTimeEncoderMixin,
     NamespaceEncoderMixin,
     CollectionsEncoderMixin,
-    HexUUIDMixin,
+    UUIDMixin,
     ObjectIdMixin,
     DictableMixin,
 ):
     """
     Extends all encoders provided with this module
     """
 
     def default(self, o, *_, **__):
         return super().default(o)
 
 
 class JsonDecoderMixin:
-    @classmethod
-    def custom_object_hook(cls, data: dict) -> dict:
+    def custom_object_hook(self, data: dict) -> dict:
         return data
 
-    @classmethod
-    def custom_field_hook(cls, value):
-        return value
-
 
 class JsonISODateDecoder(JsonDecoderMixin):
     ISO_FORMAT = "%Y-%m-%dT%H:%M:%S"
 
-    @classmethod
-    def custom_field_hook(cls, value):
-        if isinstance(value, str):
+    def custom_object_hook(self, data: dict):
+        if "$datetime" in data:
             try:
-                return datetime.datetime.strptime(value, cls.ISO_FORMAT)
+                return datetime.datetime.strptime(data["$datetime"], self.ISO_FORMAT)
             except (TypeError, ValueError):
-                return value
+                traceback.print_exc()
 
-        return super().custom_object_hook(value)
+        return super().custom_object_hook(data)
 
 
 class JsonObjectIdDecoder(JsonDecoderMixin):
-    @classmethod
-    def custom_object_hook(cls, data: dict):
+    def custom_object_hook(self, data: dict):
         if "$oid" in data:
             try:
                 return ObjectId(data["$oid"])
             except (TypeError, InvalidId):
-                return data
+                traceback.print_exc()
 
         return super().custom_object_hook(data)
 
 
 class BaseJsonDecoder(json.JSONDecoder, JsonDecoderMixin):
     def __init__(self, *args, **kwargs):
         super().__init__(object_hook=self.custom_object_hook, *args, **kwargs)
 
-    @classmethod
-    def custom_object_hook(cls, data: dict) -> dict:
-        # noinspection PyBroadException
-        try:
-            data = super().custom_object_hook(data)
-            return {k: super().custom_field_hook(v) for k, v in data.items()}
-        except Exception:  # pylint: disable=broad-except
-            return data
-
 
 class JsonDecoder(
     BaseJsonDecoder,
     JsonObjectIdDecoder,
     JsonISODateDecoder,
 ):
     """
```

### Comparing `vbcore-2.0.0rc4/vbcore/jsonschema/schemas/jsonrpc.py` & `vbcore-2.1.0rc0/vbcore/jsonschema/schemas/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/jsonschema/support.py` & `vbcore-2.1.0rc0/vbcore/jsonschema/support.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/lambdas.py` & `vbcore-2.1.0rc0/vbcore/lambdas.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/misc.py` & `vbcore-2.1.0rc0/vbcore/misc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import functools
 import math
 import re
 import signal
 import sys
 import typing as t
+import uuid
 from threading import Lock
 
+from vbcore.types import OptStr
+
 
 class Printer:
     function = print
     thread_lock = Lock()
 
     @classmethod
     def safe(cls, *args, **kwargs):
@@ -110,32 +113,37 @@
     @classmethod
     def handle_terminate(cls, signum, frame, callback: t.Callable = lambda: None):
         Printer.error(f"received signal: {signum} at frame: {frame}")
         callback()
         sys.exit(signum)
 
     @classmethod
-    def register(cls, handler: t.Callable, *signals):
+    def register(cls, handler: t.Callable, *signals: int):
         for s in signals:
             try:
-                sig = getattr(signal, s)
-                signal.signal(sig, handler)
+                signal.signal(s, handler)
             except Exception as exc:  # pylint: disable=broad-except
                 Printer.error(f"unable to register signal {s}: {exc}")
 
 
 class MemoryUsage:
     @classmethod
     def sizeof_fmt(cls, num: float, units: t.Sequence[str] = ()) -> str:
         _units = units or ("B", "KB", "MB", "GB")
-        for unit in _units[:-1]:
+
+        if abs(num) < 1000.0:
+            return f"{num} {_units[0]}"
+
+        num /= 1000.0
+        for unit in _units[1:-1]:
             if abs(num) < 1000.0:
                 return f"{num:.2f} {unit}"
             num /= 1000.0
-        return f"{num:.2f} {units[-1]}"
+
+        return f"{num:.2f} {_units[-1]}"
 
     @classmethod
     def sizeof(cls, value: float) -> float:
         return sys.int_info.bits_per_digit * math.ceil(
             sys.getsizeof(value) / sys.int_info.sizeof_digit
         )
 
@@ -159,7 +167,44 @@
 
 class CommonRegex:
     EMAIL_REGEX = re.compile(r"(^[a-zA-Z0-9_.-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$)")
 
     @classmethod
     def is_valid_email(cls, email: str) -> bool:
         return bool(re.fullmatch(cls.EMAIL_REGEX, email))
+
+
+def get_uuid(
+    ver: int = 4,
+    hex_: bool = True,
+    name: OptStr = None,
+    ns: t.Optional[uuid.UUID] = None,
+) -> t.Union[str, uuid.UUID]:
+    if ver == 1:
+        _uuid = uuid.uuid1()
+    elif ver == 3:
+        _uuid = uuid.uuid3(ns or uuid.NAMESPACE_DNS, name)
+    elif ver == 4:
+        _uuid = uuid.uuid4()
+    elif ver == 5:
+        _uuid = uuid.uuid5(ns or uuid.NAMESPACE_DNS, name)
+    else:
+        raise TypeError(f"invalid uuid version {ver}")
+
+    return _uuid.hex if hex_ else _uuid
+
+
+def check_uuid(
+    u: t.Union[str, uuid.UUID],
+    ver: int = 4,
+    raise_exc: bool = False,
+) -> bool:
+    try:
+        if isinstance(u, uuid.UUID):
+            return True
+
+        _uuid = uuid.UUID(u, version=ver)
+        return u == (str(_uuid) if "-" in u else _uuid.hex)
+    except (ValueError, TypeError, AttributeError) as exc:
+        if raise_exc:
+            raise ValueError(f"'{u}' is an invalid UUID{ver}") from exc
+        return False
```

### Comparing `vbcore-2.0.0rc4/vbcore/net/helpers.py` & `vbcore-2.1.0rc0/vbcore/net/helpers.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/net/sendmail.py` & `vbcore-2.1.0rc0/vbcore/net/sendmail.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,73 +1,69 @@
-import dataclasses
-import logging
 import os
 import smtplib
 import typing as t
+from dataclasses import dataclass
 from email.mime.application import MIMEApplication
 from email.mime.base import MIMEBase
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from email.utils import formatdate, make_msgid, parseaddr
 
 from email_validator import caching_resolver, validate_email, ValidatedEmail
 
 from vbcore.files import FileHandler
-from vbcore.misc import CommonRegex
-from vbcore.types import OptStr, StrList, StrTuple
-from vbcore.uuid import get_uuid
+from vbcore.misc import CommonRegex, get_uuid
+from vbcore.types import CoupleStr, OptStr, StrDict, StrList, StrTuple
 
 AddressType = t.Union[str, StrTuple]
-HeadersType = t.Dict[str, str]
 
 
-@dataclasses.dataclass
+@dataclass(frozen=True)
 class SMTPResponse:
     message_id: str
     response: t.Dict[str, t.Tuple[int, bytes]]
 
 
-@dataclasses.dataclass(frozen=True)
+@dataclass(frozen=True, kw_only=True)
 class SMTPParams:
     host: str
     port: int
     timeout: int = 10
     debug: bool = False
     is_ssl: bool = False
     is_tls: bool = False
     user: OptStr = None
     password: OptStr = None
-    sender: t.Optional[t.Union[str, t.Tuple[str, str]]] = None
+    sender: t.Optional[t.Union[str, CoupleStr]] = None
 
 
-@dataclasses.dataclass(frozen=True)
+@dataclass(frozen=True)
 class MessageData:
     subject: str
     priority: int = 3
     html: OptStr = None
     text: OptStr = None
-    headers: t.Optional[HeadersType] = None
     message_id: OptStr = None
+    headers: t.Optional[StrDict] = None
     attachments: t.Optional[StrList] = None
 
 
-@dataclasses.dataclass(frozen=True)
+@dataclass(frozen=True)
 class MessageAddresses:
     sender: str
     to: AddressType  # pylint: disable=invalid-name
     cc: AddressType = ()  # pylint: disable=invalid-name
     bcc: AddressType = ()
     reply_to: OptStr = None
 
 
 class SendMail:
     def __init__(self, params: SMTPParams, **kwargs):
         self.params = params
         self._smtp_args = kwargs
-        self._log = logging.getLogger(self.__module__)
 
     @classmethod
     def validate_email(cls, email: str, restricted: bool = True) -> ValidatedEmail:
         if restricted and not CommonRegex.is_valid_email(email):
             raise ValueError(f"invalid email: {email}")
         return validate_email(email, dns_resolver=caching_resolver())
 
@@ -145,18 +141,18 @@
         subject: str,
         to: AddressType,
         sender: OptStr = None,
         priority: int = 3,
         html: OptStr = None,
         text: OptStr = None,
         reply_to: OptStr = None,
+        message_id: OptStr = None,
         cc: t.Optional[AddressType] = (),
         bcc: t.Optional[AddressType] = (),
-        headers: t.Optional[HeadersType] = None,
-        message_id: OptStr = None,
+        headers: t.Optional[StrDict] = None,
         attachments: t.Optional[StrList] = None,
         **kwargs,
     ) -> SMTPResponse:
         _sender = sender or str(self.params.sender) or self.params.user
         message = self.message(
             MessageAddresses(
                 to=to,
```

### Comparing `vbcore-2.0.0rc4/vbcore/net/socks_smtp.py` & `vbcore-2.1.0rc0/vbcore/net/socks_smtp.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/rule_engine/base.py` & `vbcore-2.1.0rc0/vbcore/rule_engine/base.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/rule_engine/engine.py` & `vbcore-2.1.0rc0/vbcore/rule_engine/engine.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import typing as t
-from collections import OrderedDict
 
 from rule_engine import Context, resolve_item, Rule
 
+from ..types import StrDict
 from .base import RuleInfo, RuleType
 
 
 class RuleEngine:
     def __init__(
         self,
         context: t.Optional[Context] = None,
@@ -70,25 +70,25 @@
                 result = self.evaluate(rule.rule, data)
             else:
                 result = self.matches(rule.rule, data)
             yield rule, result
 
     def which_matches(self, rules: t.List[RuleInfo], data: dict) -> t.List[RuleInfo]:
         cursor = self.apply(rules, data)
-        return [match[0] for match in filter(lambda x: x[1] is True, cursor)]
+        return [match[0] for match in filter(lambda x: bool(x[1]) is True, cursor)]
 
     def first_match(self, rules: t.List[RuleInfo], data: dict) -> t.Optional[RuleInfo]:
         for result in self.apply(rules, data):
             if result[1] is True:
                 return result[0]
         return None
 
     def perform_on_match(
         self, rules: t.List[RuleInfo], data: dict, *args, **kwargs
-    ) -> t.OrderedDict[str, t.Any]:
-        results: t.OrderedDict[str, t.Any] = OrderedDict()
+    ) -> StrDict:
+        results: StrDict = {}
         for rule, result in self.apply(rules, data):
             if rule.evaluate is True or result is True:
                 results[rule.id] = rule.action.perform(
                     data, *args, rule=rule, rule_result=result, **kwargs
                 )
         return results
```

### Comparing `vbcore-2.0.0rc4/vbcore/standalone/scheduler.py` & `vbcore-2.1.0rc0/vbcore/standalone/scheduler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-import logging
 import typing as t
 from io import StringIO
 
 from apscheduler import events as scheduler_events
 from apscheduler.job import Job
 from apscheduler.schedulers.base import BaseScheduler
 from apscheduler.schedulers.blocking import BlockingScheduler
 
+from vbcore.base import BaseLoggerMixin
 from vbcore.datastruct.lazy import Dumper, LazyDump
-from vbcore.uuid import get_uuid
+from vbcore.misc import get_uuid
+from vbcore.types import OptDict, StrDict
 
 
-class APScheduler:
+class APScheduler(BaseLoggerMixin):
     def __init__(
         self,
         *args,
         scheduler: t.Type[BaseScheduler] = BlockingScheduler,
-        gconfig: dict = None,
+        gconfig: StrDict = None,
         events_to_listen: int = None,
         auto_start: bool = False,
         **kwargs,
     ):
-        self.logger = logging.getLogger(self.__module__)
         super().__init__(*args, **kwargs)
         self._scheduler = scheduler(gconfig or {})
         self._events = events_to_listen or scheduler_events.EVENT_ALL
         self._scheduler.add_listener(self.event_listener, self._events)
         if auto_start:
             self._scheduler.start()
 
     @classmethod
     def factory(
         cls, config: dict, scheduler_class: t.Optional[t.Type[BaseScheduler]] = None
     ) -> "APScheduler":
         instance = cls(scheduler=scheduler_class, **config["SCHEDULER"])
         instance.load_jobs(config["JOBS"])
-        instance.logger.info("%s", LazyDump(instance.dump_jobs))
+        instance.log.info("%s", LazyDump(instance.dump_jobs))
         return instance
 
     @property
     def scheduler(self) -> BaseScheduler:
         return self._scheduler
 
     def dump_jobs(self) -> str:
@@ -53,25 +53,23 @@
             return f"{repr(event)}-<{event.job_id}>-<{event.jobstore}>"
         return repr(event)
 
     def event_listener(self, event):
         if not event.code & self._events:
             return
 
-        self.logger.debug(
-            "received event %s", Dumper(event, callback=self.repr_job_event)
-        )
+        self.log.debug("received event %s", Dumper(event, callback=self.repr_job_event))
         if event.code == scheduler_events.EVENT_JOB_ERROR:
-            self.logger.error("An error occurred when executing job: %s", event.job_id)
-            self.logger.exception(event.exception)
-            self.logger.error(event.traceback)
+            self.log.error("An error occurred when executing job: %s", event.job_id)
+            self.log.exception(event.exception)
+            self.log.error(event.traceback)
         elif event.code == scheduler_events.EVENT_JOB_ADDED:
-            self.logger.info("successfully added job: %s", event.job_id)
+            self.log.info("successfully added job: %s", event.job_id)
         elif event.code == scheduler_events.EVENT_JOB_EXECUTED:
-            self.logger.info(
+            self.log.info(
                 "successfully executed job: %s, returned value: %s",
                 event.job_id,
                 event.retval,
             )
 
     @classmethod
     def get_id(cls) -> str:
@@ -81,22 +79,22 @@
         for config in jobs_config:
             self.add_job(**config)
 
     def add_job(
         self,
         task: t.Union[t.Callable, str],
         *args,
-        params: t.Optional[dict] = None,
+        params: OptDict = None,
         **kwargs,
     ) -> Job:
         job_id = self.get_id()
         job = self._scheduler.add_job(
             task, args=args, kwargs=params, id=job_id, **kwargs
         )
-        self.logger.debug("added job '%s' with id '%s'", task, job_id)
+        self.log.debug("added job '%s' with id '%s'", task, job_id)
         return job
 
     def __del__(self):
         try:
             self._scheduler.shutdown()
         except AttributeError:
             pass  # pragma: no cover
```

### Comparing `vbcore-2.0.0rc4/vbcore/standalone/wsgi_gunicorn.py` & `vbcore-2.1.0rc0/vbcore/standalone/wsgi_gunicorn.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 import typing as t
-from dataclasses import MISSING
-from functools import partial
 from multiprocessing import cpu_count
 
 from decouple import Choices, Csv, UndefinedValueError
 from gunicorn import util
 from gunicorn.app.base import BaseApplication  # type: ignore
 
 from vbcore.configurator import config, load_dotenv
+from vbcore.enums import EnumMixin, StrEnum
 from vbcore.importer import Importer
+from vbcore.types import MISSING
 
 # Supported env vars:
 #  - GU_BIND
 #  - GU_PID_FILE
 #  - GU_PROC_NAME
 #  - GU_TIMEOUT
 #  - GU_BACKLOG
@@ -27,32 +27,32 @@
 #  - GU_WORKER_CONNECTIONS
 #  - GU_LOG_LEVEL
 #  - GU_ACCESS_LOG_FORMAT
 
 LOG_LEVELS = ["debug", "info", "warning", "error"]
 
 
+class WorkerType(EnumMixin, StrEnum):
+    DEFAULT = "gthread"
+    UVICORN = "uvicorn.workers.UvicornWorker"
+    MEINHELD = "meinheld.gmeinheld.MeinheldWorker"
+
+
 # pylint: disable=too-many-public-methods
 class GUnicornServer(BaseApplication):
-    custom_worker = {
-        None: "gthread",
-        "uvicorn": "uvicorn.workers.UvicornWorker",
-        "meinheld": "meinheld.gmeinheld.MeinheldWorker",
-    }
-
     def __init__(
         self,
         app: t.Union[str, t.Callable],
-        worker_class: t.Optional[str] = None,
+        worker_type: t.Optional[WorkerType] = None,
         **kwargs,
     ):
         load_dotenv()
+        self.worker_type = worker_type or WorkerType.DEFAULT
         self.application = app
         self.options = kwargs
-        self.worker_class = self.custom_worker.get(worker_class, worker_class)
         super().__init__()
 
     def from_env_config(
         self, conf_key: str, opt_key: str, default: t.Any = MISSING, **kwargs
     ):
         _default = self.options.get(opt_key, default)
         if default == _default == MISSING:
@@ -76,16 +76,16 @@
         self.from_env_config("GU_KEEP_ALIVE", "keepalive", 5, cast=int)
         self.from_env_config("GU_CHDIR", "chdir", util.getcwd())
         self.from_env_config("GU_USER", "user", os.geteuid())
         self.from_env_config("GU_GROUP", "group", os.getegid())
         self.from_env_config(
             "GU_FORWARDED_ALLOW_IPS", "forwarded_allow_ips", "127.0.0.1"
         )
-        self.from_env_config("GU_WORKER_CLASS", "worker_class", self.worker_class)
-        self.from_env_config("GU_THREADS", "threads", 4, cast=int)
+        self.from_env_config("GU_WORKER_CLASS", "worker_class", self.worker_type.value)
+        self.from_env_config("GU_THREADS", "threads", cpu_count() * 2 + 1, cast=int)
         self.from_env_config("GU_WORKERS", "workers", cpu_count(), cast=int)
         self.from_env_config(
             "GU_WORKER_CONNECTIONS", "worker_connections", 1000, cast=int
         )
         self.from_env_config(
             "GU_LOG_LEVEL", "loglevel", "info", cast=Choices(LOG_LEVELS)
         )
@@ -121,15 +121,16 @@
         self.load_default_config()
         self.load_config()
 
     def load_config(self):
         self.set_hooks()
         self.set_default_config()
         for key, value in self.options.items():
-            self.cfg.set(key.lower(), value)
+            if value is not MISSING:
+                self.cfg.set(key.lower(), value)
         self.load_from_env()
 
     def load(self):
         if isinstance(self.application, str):
             return Importer.from_module(self.application)
         return self.application
 
@@ -262,32 +263,7 @@
     @classmethod
     def nworkers_changed(cls, server, new_value, old_value):
         _ = server, new_value, old_value
 
     @classmethod
     def on_exit(cls, server):
         _ = server
-
-
-def cli_gu_options(func: t.Callable) -> t.Callable:
-    import click  # pylint: disable=import-outside-toplevel
-
-    str_option = partial(click.option, required=False)
-    int_option = partial(click.option, required=False, type=click.INT)
-
-    @str_option("-b", "--bind", multiple=True)
-    @int_option("-w", "--workers")
-    @int_option("-t", "--threads")
-    @str_option("-W", "--worker-class")
-    @int_option("-T", "--timeout")
-    @int_option("--backlog")
-    @int_option("--keepalive")
-    @str_option("--pidfile")
-    @str_option("--proc-name")
-    @str_option("--chdir")
-    @str_option("-u", "--user")
-    @str_option("-g", "--group")
-    def wrapper(**kwargs):
-        without_blanks = {k: v for k, v in kwargs.items() if v}
-        return func(**without_blanks)
-
-    return wrapper
```

### Comparing `vbcore-2.0.0rc4/vbcore/stringutils/misc.py` & `vbcore-2.1.0rc0/vbcore/stringutils/misc.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/stringutils/notations.py` & `vbcore-2.1.0rc0/vbcore/stringutils/notations.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/system.py` & `vbcore-2.1.0rc0/vbcore/system.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/tester/asserter.py` & `vbcore-2.1.0rc0/vbcore/tester/asserter.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/tester/fetchmail.py` & `vbcore-2.1.0rc0/vbcore/tester/fetchmail.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/tester/helpers.py` & `vbcore-2.1.0rc0/vbcore/tester/helpers.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/tester/http.py` & `vbcore-2.1.0rc0/vbcore/tester/http.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/tools/cli.py` & `vbcore-2.1.0rc0/vbcore/tools/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import typing as t
 from functools import partial
 
 import click
 
 from vbcore.date_helper import DateFmt, DateTimeFmt
+from vbcore.types import OptFloat, OptInt
 
 
 def option_as_dict(ctx, param, value):
     _ = ctx, param
     option = {}
     for opt in value:
         tokens = opt.split("=", 2)
@@ -59,40 +60,52 @@
     ):
         return Cli.option(*args, type=click.Choice(values, case_sensitive), **kwargs)
 
     @classmethod
     def integer(
         cls,
         *args,
-        min_val: t.Optional[int] = None,
-        max_val: t.Optional[int] = None,
+        min_val: OptInt = None,
+        max_val: OptInt = None,
         min_open: bool = False,
         max_open: bool = False,
         clamp: bool = False,
         **kwargs,
     ):
-        opt_type = click.IntRange(
-            min=min_val, max=max_val, min_open=min_open, max_open=max_open, clamp=clamp
-        )
+        opt_type = click.INT
+        if min_val is not None or max_val is not None:
+            opt_type = click.IntRange(
+                min=min_val,
+                max=max_val,
+                min_open=min_open,
+                max_open=max_open,
+                clamp=clamp,
+            )
         return Cli.option(*args, **kwargs, type=opt_type)
 
     @classmethod
     def decimal(
         cls,
         *args,
-        min_val: t.Optional[float] = None,
-        max_val: t.Optional[float] = None,
+        min_val: OptFloat = None,
+        max_val: OptFloat = None,
         min_open: bool = False,
         max_open: bool = False,
         clamp: bool = False,
         **kwargs,
     ):
-        opt_type = click.FloatRange(
-            min=min_val, max=max_val, min_open=min_open, max_open=max_open, clamp=clamp
-        )
+        opt_type = click.FLOAT
+        if min_val is not None or max_val is not None:
+            opt_type = click.FloatRange(
+                min=min_val,
+                max=max_val,
+                min_open=min_open,
+                max_open=max_open,
+                clamp=clamp,
+            )
         return Cli.option(*args, **kwargs, type=opt_type)
 
     @classmethod
     def debug(cls):
         return partial(cls.flag, "-D", "--debug")
```

### Comparing `vbcore-2.0.0rc4/vbcore/tools/crypto.py` & `vbcore-2.1.0rc0/vbcore/tools/crypto.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore/tools/database.py` & `vbcore-2.1.0rc0/vbcore/tools/database.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,32 @@
 import click
 
+from vbcore.datastruct.lazy import LazyImporter
 from vbcore.db.mysql_dumper import cli_wrapper as mysql_dump_cli_wrapper
-from vbcore.loggers import Loggers
-from vbcore.tools.cli import Cli, CliOpt, CliOutputDir, CliReqOpt
-
-try:
-    from vbcore.db.schema import db_to_schema, dump_model_ddl, model_to_uml
-except ImportError:  # pragma: no cover
-    db_to_schema = dump_model_ddl = model_to_uml = None
+from vbcore.loggers import Log
+from vbcore.tools.cli import Cli, CliOpt, CliOutputDir, CliOutputFile, CliReqOpt
 
+db_to_schema, dump_model_ddl, model_to_uml = LazyImporter.import_many(
+    "vbcore.db.schema:db_to_schema",
+    "vbcore.db.schema:dump_model_ddl",
+    "vbcore.db.schema:model_to_uml",
+    message="you must install vbcore[db]",
+)
 
 DIALECTS = ["sqlite", "mysql", "oracle", "postgresql", "mssql"]
 
 main = click.Group(name="database", help="tools for database")
 
-# enabling default logging config
-logger = Loggers()
-
-
-def check_dependency(label):
-    if label is None:
-        Cli.abort("you must install vbcore[db]")
-
 
 @main.command(name="schema")
 @CliOpt.string("-m", "--from-models", help="module of sqlalchemy models")
 @CliOpt.string("-d", "--from-database", help="database url connection")
-@CliReqOpt.string("-f", "--file", help="output png filename")
+@CliReqOpt.string("-f", "--file", type=CliOutputFile(), help="output png filename")
 def dump_schema(from_models, from_database, file):
     """Create png schema of database"""
-    check_dependency(model_to_uml or db_to_schema)
-
     if from_models:
         graph = model_to_uml(from_models)
     elif from_database:
         graph = db_to_schema(from_database)
     else:
         raise click.UsageError("One of -m or -d are required")
 
@@ -44,25 +36,24 @@
         Cli.abort(f"{str(exc)}\ntry to install 'graphviz'")
 
 
 @main.command(name="dump-ddl")
 @CliOpt.choice("--dialect", default="sqlite", values=DIALECTS)
 @CliReqOpt.string("-m", "--metadata", help="metadata module")
 def dump_ddl(dialect, metadata):
-    """Dumps the create table statements for a given metadata"""
-    check_dependency(dump_model_ddl)
+    """Dumps the CREATE table statements for a given metadata"""
     dump_model_ddl(metadata, dialect)
 
 
 @main.command(name="mysql-backup")
 @Cli.argument("db_url")
 @CliOpt.string("--folder", default=".", type=CliOutputDir())
 @CliOpt.multi("-i", "--ignore-database")
 @CliOpt.boolean("-t", "--add-datetime", default=True)
 @CliOpt.flag("-a", "--as-archive")
 @CliOpt.string("-d", "--db-prefix")
 @CliOpt.string("--datetime-format")
 @CliOpt.string("--file-prefix")
 def mysql_backup(**kwargs):
     """perform the backup of mysql databases"""
-    with logger.execution_time():
+    with Log.execution_time():
         mysql_dump_cli_wrapper(**kwargs)
```

### Comparing `vbcore-2.0.0rc4/vbcore/tools/entrypoint.py` & `vbcore-2.1.0rc0/vbcore/tools/entrypoint.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 import sys
 
 import click
 
+from vbcore.loggers import SetupLoggers
 from vbcore.tools.cli import Cli
 from vbcore.tools.crypto import main as main_crypto
 from vbcore.tools.database import main as main_database
 from vbcore.tools.initializer.init import main as main_init
 from vbcore.tools.scheduler import main as main_scheduler
+from vbcore.tools.sendmail import sendmail as main_sendmail
+from vbcore.tools.sftp import main as main_sftp
+from vbcore.tools.wsgi_gunicorn import main as main_gunicorn
 from vbcore.version import __version__
 
+SetupLoggers()
+
 main = click.Group()
 
 
 @main.command(name="version")
 def dump_version():
     """dump python and vbcore version"""
     Cli.print(f"vbcore version: {__version__}")
     Cli.print(f"python version: {sys.version}")
 
 
 main.add_command(main_database)
 main.add_command(main_crypto)
 main.add_command(main_init)
 main.add_command(main_scheduler)
+main.add_command(main_sendmail)
+main.add_command(main_sftp)
+main.add_command(main_gunicorn)
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `vbcore-2.0.0rc4/vbcore/tools/initializer/init.py` & `vbcore-2.1.0rc0/vbcore/tools/initializer/init.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     except OSError as e:
         Cli.abort(f"Unable to create new app. Error: {e}")
 
 
 def init_app(name: str):
     copy_skeleton(name)
     init_file = Path(os.path.join(name, "__init__.py"))
-    init_file.write_text("from .version import *\n", encoding="utf-8")
+    init_file.write_text("", encoding="utf-8")
 
     for root, _, files in os.walk("."):
         for f in files:
             replace_in_file(os.path.join(root, f), "{skeleton}", name)
 
 
 @click.command(name="init")
```

### Comparing `vbcore-2.0.0rc4/vbcore/yaml.py` & `vbcore-2.1.0rc0/vbcore/yaml.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc4/vbcore.egg-info/requires.txt` & `vbcore-2.1.0rc0/vbcore.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+bson
 click
 python-dateutil
 python-decouple
 python-dotenv
 pyyaml
 psutil
 
 [all]
+bson
 click
 python-dateutil
 python-decouple
 python-dotenv
 pyyaml
 psutil
-sqlalchemy<2
+sqlalchemy
 sqlalchemy_schemadisplay
 argon2-cffi
 bcrypt
 aiohttp
 requests
 user_agents
 email_validator
@@ -32,15 +34,15 @@
 xmltodict
 
 [crypto]
 argon2-cffi
 bcrypt
 
 [db]
-sqlalchemy<2
+sqlalchemy
 sqlalchemy_schemadisplay
 
 [extra]
 chardet
 jsonschema
 rule_engine
 gql
```

