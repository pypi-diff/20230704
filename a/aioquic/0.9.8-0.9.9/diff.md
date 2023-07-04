# Comparing `tmp/aioquic-0.9.8.tar.gz` & `tmp/aioquic-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aioquic-0.9.8.tar", last modified: Mon Mar  8 19:44:51 2021, max compression
+gzip compressed data, was "dist/aioquic-0.9.9.tar", last modified: Tue Mar  9 08:21:32 2021, max compression
```

## Comparing `aioquic-0.9.8.tar` & `aioquic-0.9.9.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-08 19:44:51.000000 aioquic-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2021-03-08 19:44:49.000000 aioquic-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-08 19:44:49.000000 aioquic-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5652 2021-03-08 19:44:51.000000 aioquic-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3799 2021-03-08 19:44:49.000000 aioquic-0.9.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-08 19:44:51.000000 aioquic-0.9.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      604 2021-03-08 19:44:49.000000 aioquic-0.9.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      544 2021-03-08 19:44:49.000000 aioquic-0.9.8/docs/asyncio.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5850 2021-03-08 19:44:49.000000 aioquic-0.9.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2021-03-08 19:44:49.000000 aioquic-0.9.8/docs/design.rst
--rw-r--r--   0 runner    (1001) docker     (121)      753 2021-03-08 19:44:49.000000 aioquic-0.9.8/docs/h3.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1141 2021-03-08 19:44:49.000000 aioquic-0.9.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-03-08 19:44:49.000000 aioquic-0.9.8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)      913 2021-03-08 19:44:49.000000 aioquic-0.9.8/docs/quic.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-08 19:44:51.000000 aioquic-0.9.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2950 2021-03-08 19:44:49.000000 aioquic-0.9.8/examples/demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     5029 2021-03-08 19:44:49.000000 aioquic-0.9.8/examples/doq_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4574 2021-03-08 19:44:49.000000 aioquic-0.9.8/examples/doq_server.py
--rw-r--r--   0 runner    (1001) docker     (121)    16731 2021-03-08 19:44:49.000000 aioquic-0.9.8/examples/http3_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    16160 2021-03-08 19:44:49.000000 aioquic-0.9.8/examples/http3_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     7072 2021-03-08 19:44:49.000000 aioquic-0.9.8/examples/httpx_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    18440 2021-03-08 19:44:49.000000 aioquic-0.9.8/examples/interop.py
--rw-r--r--   0 runner    (1001) docker     (121)      794 2021-03-08 19:44:49.000000 aioquic-0.9.8/examples/quic_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     3132 2021-03-08 19:44:49.000000 aioquic-0.9.8/examples/siduck_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-08 19:44:51.000000 aioquic-0.9.8/examples/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2021-03-08 19:44:49.000000 aioquic-0.9.8/examples/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (121)      711 2021-03-08 19:44:49.000000 aioquic-0.9.8/examples/templates/logs.html
--rw-r--r--   0 runner    (1001) docker     (121)      439 2021-03-08 19:44:51.000000 aioquic-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2244 2021-03-08 19:44:49.000000 aioquic-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-08 19:44:51.000000 aioquic-0.9.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-08 19:44:51.000000 aioquic-0.9.8/src/aioquic/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13884 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/_buffer.c
--rw-r--r--   0 runner    (1001) docker     (121)    15344 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/_crypto.c
--rw-r--r--   0 runner    (1001) docker     (121)      227 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/about.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-08 19:44:51.000000 aioquic-0.9.8/src/aioquic/asyncio/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3421 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/asyncio/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      865 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/asyncio/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     8687 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/asyncio/protocol.py
--rw-r--r--   0 runner    (1001) docker     (121)     8402 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/asyncio/server.py
--rw-r--r--   0 runner    (1001) docker     (121)      732 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-08 19:44:51.000000 aioquic-0.9.8/src/aioquic/h0/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/h0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2594 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/h0/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-08 19:44:51.000000 aioquic-0.9.8/src/aioquic/h3/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/h3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27319 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/h3/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1404 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/h3/events.py
--rw-r--r--   0 runner    (1001) docker     (121)      179 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/h3/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-08 19:44:51.000000 aioquic-0.9.8/src/aioquic/quic/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/quic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3876 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/quic/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)   112071 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/quic/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     7671 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/quic/crypto.py
--rw-r--r--   0 runner    (1001) docker     (121)     2374 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/quic/events.py
--rw-r--r--   0 runner    (1001) docker     (121)     8885 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/quic/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)    15760 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/quic/packet.py
--rw-r--r--   0 runner    (1001) docker     (121)    11886 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/quic/packet_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3133 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/quic/rangeset.py
--rw-r--r--   0 runner    (1001) docker     (121)    17177 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/quic/recovery.py
--rw-r--r--   0 runner    (1001) docker     (121)     1988 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/quic/retry.py
--rw-r--r--   0 runner    (1001) docker     (121)     8918 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/quic/stream.py
--rw-r--r--   0 runner    (1001) docker     (121)    66399 2021-03-08 19:44:49.000000 aioquic-0.9.8/src/aioquic/tls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-08 19:44:51.000000 aioquic-0.9.8/src/aioquic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5652 2021-03-08 19:44:51.000000 aioquic-0.9.8/src/aioquic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2610 2021-03-08 19:44:51.000000 aioquic-0.9.8/src/aioquic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-08 19:44:51.000000 aioquic-0.9.8/src/aioquic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       89 2021-03-08 19:44:51.000000 aioquic-0.9.8/src/aioquic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-03-08 19:44:51.000000 aioquic-0.9.8/src/aioquic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-08 19:44:51.000000 aioquic-0.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/initial_client.bin
--rw-r--r--   0 runner    (1001) docker     (121)      202 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/initial_server.bin
--rw-r--r--   0 runner    (1001) docker     (121)     5656 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/pycacert.pem
--rw-r--r--   0 runner    (1001) docker     (121)      125 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/retry.bin
--rw-r--r--   0 runner    (1001) docker     (121)      125 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/retry_draft_29.bin
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/short_header.bin
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/ssl_cert.pem
--rw-r--r--   0 runner    (1001) docker     (121)     3716 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/ssl_cert_with_chain.pem
--rw-r--r--   0 runner    (1001) docker     (121)     4607 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/ssl_combined.pem
--rw-r--r--   0 runner    (1001) docker     (121)     2484 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/ssl_key.pem
--rw-r--r--   0 runner    (1001) docker     (121)    13460 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/test_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)      843 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/test_asyncio_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     6742 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/test_buffer.py
--rw-r--r--   0 runner    (1001) docker     (121)    95551 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)    14192 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (121)    13046 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/test_crypto_draft_29.py
--rw-r--r--   0 runner    (1001) docker     (121)     7086 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/test_h0.py
--rw-r--r--   0 runner    (1001) docker     (121)    45118 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/test_h3.py
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)    17131 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/test_packet.py
--rw-r--r--   0 runner    (1001) docker     (121)    20903 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/test_packet_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     6909 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/test_rangeset.py
--rw-r--r--   0 runner    (1001) docker     (121)     8307 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/test_recovery.py
--rw-r--r--   0 runner    (1001) docker     (121)     1227 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (121)    20063 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (121)    51865 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/test_tls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1538 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/tls_certificate.bin
--rw-r--r--   0 runner    (1001) docker     (121)      392 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/tls_certificate_verify.bin
--rw-r--r--   0 runner    (1001) docker     (121)      258 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/tls_client_hello.bin
--rw-r--r--   0 runner    (1001) docker     (121)      306 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/tls_client_hello_with_alpn.bin
--rw-r--r--   0 runner    (1001) docker     (121)      481 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/tls_client_hello_with_psk.bin
--rw-r--r--   0 runner    (1001) docker     (121)      286 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/tls_client_hello_with_sni.bin
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/tls_encrypted_extensions.bin
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/tls_encrypted_extensions_with_alpn.bin
--rw-r--r--   0 runner    (1001) docker     (121)      116 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/tls_encrypted_extensions_with_alpn_and_early_data.bin
--rw-r--r--   0 runner    (1001) docker     (121)       36 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/tls_finished.bin
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/tls_new_session_ticket.bin
--rw-r--r--   0 runner    (1001) docker     (121)       64 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/tls_new_session_ticket_with_unknown_extension.bin
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/tls_server_hello.bin
--rw-r--r--   0 runner    (1001) docker     (121)      161 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/tls_server_hello_with_psk.bin
--rw-r--r--   0 runner    (1001) docker     (121)      162 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/tls_server_hello_with_unknown_extension.bin
--rw-r--r--   0 runner    (1001) docker     (121)     2295 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-03-08 19:44:49.000000 aioquic-0.9.8/tests/version_negotiation.bin
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-09 08:21:32.000000 aioquic-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1508 2021-03-09 08:21:29.000000 aioquic-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-09 08:21:29.000000 aioquic-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5652 2021-03-09 08:21:32.000000 aioquic-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3799 2021-03-09 08:21:29.000000 aioquic-0.9.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-09 08:21:32.000000 aioquic-0.9.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2021-03-09 08:21:29.000000 aioquic-0.9.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2021-03-09 08:21:29.000000 aioquic-0.9.9/docs/asyncio.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5850 2021-03-09 08:21:29.000000 aioquic-0.9.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1191 2021-03-09 08:21:29.000000 aioquic-0.9.9/docs/design.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      753 2021-03-09 08:21:29.000000 aioquic-0.9.9/docs/h3.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1141 2021-03-09 08:21:29.000000 aioquic-0.9.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-03-09 08:21:29.000000 aioquic-0.9.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      913 2021-03-09 08:21:29.000000 aioquic-0.9.9/docs/quic.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-09 08:21:32.000000 aioquic-0.9.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     2950 2021-03-09 08:21:29.000000 aioquic-0.9.9/examples/demo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5029 2021-03-09 08:21:29.000000 aioquic-0.9.9/examples/doq_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4574 2021-03-09 08:21:29.000000 aioquic-0.9.9/examples/doq_server.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16731 2021-03-09 08:21:29.000000 aioquic-0.9.9/examples/http3_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16146 2021-03-09 08:21:29.000000 aioquic-0.9.9/examples/http3_server.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7072 2021-03-09 08:21:29.000000 aioquic-0.9.9/examples/httpx_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18440 2021-03-09 08:21:29.000000 aioquic-0.9.9/examples/interop.py
+-rw-r--r--   0 runner    (1001) docker     (121)      794 2021-03-09 08:21:29.000000 aioquic-0.9.9/examples/quic_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3132 2021-03-09 08:21:29.000000 aioquic-0.9.9/examples/siduck_client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-09 08:21:32.000000 aioquic-0.9.9/examples/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     1125 2021-03-09 08:21:29.000000 aioquic-0.9.9/examples/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (121)      711 2021-03-09 08:21:29.000000 aioquic-0.9.9/examples/templates/logs.html
+-rw-r--r--   0 runner    (1001) docker     (121)      439 2021-03-09 08:21:32.000000 aioquic-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2244 2021-03-09 08:21:29.000000 aioquic-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-09 08:21:32.000000 aioquic-0.9.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-09 08:21:32.000000 aioquic-0.9.9/src/aioquic/
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13884 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (121)    15344 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/_crypto.c
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/about.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-09 08:21:32.000000 aioquic-0.9.9/src/aioquic/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3421 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/asyncio/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      865 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/asyncio/compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8687 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/asyncio/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8402 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/asyncio/server.py
+-rw-r--r--   0 runner    (1001) docker     (121)      732 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-09 08:21:32.000000 aioquic-0.9.9/src/aioquic/h0/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/h0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2594 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/h0/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-09 08:21:32.000000 aioquic-0.9.9/src/aioquic/h3/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/h3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27248 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/h3/connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1404 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/h3/events.py
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/h3/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-09 08:21:32.000000 aioquic-0.9.9/src/aioquic/quic/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/quic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3876 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/quic/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)   113708 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/quic/connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7671 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/quic/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2374 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/quic/events.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8885 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/quic/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15792 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/quic/packet.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11886 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/quic/packet_builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3133 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/quic/rangeset.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17177 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/quic/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1988 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/quic/retry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8918 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/quic/stream.py
+-rw-r--r--   0 runner    (1001) docker     (121)    66399 2021-03-09 08:21:29.000000 aioquic-0.9.9/src/aioquic/tls.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-09 08:21:32.000000 aioquic-0.9.9/src/aioquic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5652 2021-03-09 08:21:32.000000 aioquic-0.9.9/src/aioquic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2610 2021-03-09 08:21:32.000000 aioquic-0.9.9/src/aioquic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-09 08:21:32.000000 aioquic-0.9.9/src/aioquic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2021-03-09 08:21:32.000000 aioquic-0.9.9/src/aioquic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2021-03-09 08:21:32.000000 aioquic-0.9.9/src/aioquic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-09 08:21:32.000000 aioquic-0.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1280 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/initial_client.bin
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/initial_server.bin
+-rw-r--r--   0 runner    (1001) docker     (121)     5656 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/pycacert.pem
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/retry.bin
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/retry_draft_29.bin
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/short_header.bin
+-rw-r--r--   0 runner    (1001) docker     (121)     2122 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/ssl_cert.pem
+-rw-r--r--   0 runner    (1001) docker     (121)     3716 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/ssl_cert_with_chain.pem
+-rw-r--r--   0 runner    (1001) docker     (121)     4607 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/ssl_combined.pem
+-rw-r--r--   0 runner    (1001) docker     (121)     2484 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/ssl_key.pem
+-rw-r--r--   0 runner    (1001) docker     (121)    13460 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (121)      843 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/test_asyncio_compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6742 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/test_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    99387 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14192 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13046 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/test_crypto_draft_29.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7086 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/test_h0.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45017 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/test_h3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1234 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17131 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/test_packet.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20903 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/test_packet_builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6909 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/test_rangeset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8307 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/test_recovery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1227 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20063 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51865 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/test_tls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1538 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/tls_certificate.bin
+-rw-r--r--   0 runner    (1001) docker     (121)      392 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/tls_certificate_verify.bin
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/tls_client_hello.bin
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/tls_client_hello_with_alpn.bin
+-rw-r--r--   0 runner    (1001) docker     (121)      481 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/tls_client_hello_with_psk.bin
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/tls_client_hello_with_sni.bin
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/tls_encrypted_extensions.bin
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/tls_encrypted_extensions_with_alpn.bin
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/tls_encrypted_extensions_with_alpn_and_early_data.bin
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/tls_finished.bin
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/tls_new_session_ticket.bin
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/tls_new_session_ticket_with_unknown_extension.bin
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/tls_server_hello.bin
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/tls_server_hello_with_psk.bin
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/tls_server_hello_with_unknown_extension.bin
+-rw-r--r--   0 runner    (1001) docker     (121)     2295 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2021-03-09 08:21:29.000000 aioquic-0.9.9/tests/version_negotiation.bin
```

### Comparing `aioquic-0.9.8/LICENSE` & `aioquic-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/PKG-INFO` & `aioquic-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aioquic
-Version: 0.9.8
+Version: 0.9.9
 Summary: An implementation of QUIC and HTTP/3
 Home-page: https://github.com/aiortc/aioquic
 Author: Jeremy Lainé
 Author-email: jeremy.laine@m4x.org
 License: BSD
 Description: aioquic
         =======
```

### Comparing `aioquic-0.9.8/README.rst` & `aioquic-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/docs/Makefile` & `aioquic-0.9.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/docs/asyncio.rst` & `aioquic-0.9.9/docs/asyncio.rst`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/docs/conf.py` & `aioquic-0.9.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/docs/design.rst` & `aioquic-0.9.9/docs/design.rst`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/docs/h3.rst` & `aioquic-0.9.9/docs/h3.rst`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/docs/index.rst` & `aioquic-0.9.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/docs/quic.rst` & `aioquic-0.9.9/docs/quic.rst`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/examples/demo.py` & `aioquic-0.9.9/examples/demo.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/examples/doq_client.py` & `aioquic-0.9.9/examples/doq_client.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/examples/doq_server.py` & `aioquic-0.9.9/examples/doq_server.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/examples/http3_client.py` & `aioquic-0.9.9/examples/http3_client.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/examples/http3_server.py` & `aioquic-0.9.9/examples/http3_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,17 +319,17 @@
             and event.stream_id in self._handlers
         ):
             handler = self._handlers[event.stream_id]
             handler.http_event_received(event)
 
     def quic_event_received(self, event: QuicEvent) -> None:
         if isinstance(event, ProtocolNegotiated):
-            if event.alpn_protocol.startswith("h3-"):
+            if event.alpn_protocol in H3_ALPN:
                 self._http = H3Connection(self._quic)
-            elif event.alpn_protocol.startswith("hq-"):
+            elif event.alpn_protocol in H0_ALPN:
                 self._http = H0Connection(self._quic)
         elif isinstance(event, DatagramFrameReceived):
             if event.data == b"quack":
                 self._quic.send_datagram_frame(b"quack-ack")
 
         #  pass event to the HTTP layer
         if self._http is not None:
```

### Comparing `aioquic-0.9.8/examples/httpx_client.py` & `aioquic-0.9.9/examples/httpx_client.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/examples/interop.py` & `aioquic-0.9.9/examples/interop.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/examples/quic_logger.py` & `aioquic-0.9.9/examples/quic_logger.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/examples/siduck_client.py` & `aioquic-0.9.9/examples/siduck_client.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/examples/templates/index.html` & `aioquic-0.9.9/examples/templates/index.html`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/examples/templates/logs.html` & `aioquic-0.9.9/examples/templates/logs.html`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/setup.py` & `aioquic-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/src/aioquic/_buffer.c` & `aioquic-0.9.9/src/aioquic/_buffer.c`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/src/aioquic/_crypto.c` & `aioquic-0.9.9/src/aioquic/_crypto.c`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/src/aioquic/asyncio/client.py` & `aioquic-0.9.9/src/aioquic/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/src/aioquic/asyncio/compat.py` & `aioquic-0.9.9/src/aioquic/asyncio/compat.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/src/aioquic/asyncio/protocol.py` & `aioquic-0.9.9/src/aioquic/asyncio/protocol.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/src/aioquic/asyncio/server.py` & `aioquic-0.9.9/src/aioquic/asyncio/server.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/src/aioquic/buffer.py` & `aioquic-0.9.9/src/aioquic/buffer.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/src/aioquic/h0/connection.py` & `aioquic-0.9.9/src/aioquic/h0/connection.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/src/aioquic/h3/connection.py` & `aioquic-0.9.9/src/aioquic/h3/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,34 +19,34 @@
 
 logger = logging.getLogger("http3")
 
 H3_ALPN = ["h3", "h3-32", "h3-31", "h3-30", "h3-29"]
 
 
 class ErrorCode(IntEnum):
-    HTTP_NO_ERROR = 0x100
-    HTTP_GENERAL_PROTOCOL_ERROR = 0x101
-    HTTP_INTERNAL_ERROR = 0x102
-    HTTP_STREAM_CREATION_ERROR = 0x103
-    HTTP_CLOSED_CRITICAL_STREAM = 0x104
-    HTTP_FRAME_UNEXPECTED = 0x105
-    HTTP_FRAME_ERROR = 0x106
-    HTTP_EXCESSIVE_LOAD = 0x107
-    HTTP_ID_ERROR = 0x108
-    HTTP_SETTINGS_ERROR = 0x109
-    HTTP_MISSING_SETTINGS = 0x10A
-    HTTP_REQUEST_REJECTED = 0x10B
-    HTTP_REQUEST_CANCELLED = 0x10C
-    HTTP_REQUEST_INCOMPLETE = 0x10D
-    HTTP_EARLY_RESPONSE = 0x10E
-    HTTP_CONNECT_ERROR = 0x10F
-    HTTP_VERSION_FALLBACK = 0x110
-    HTTP_QPACK_DECOMPRESSION_FAILED = 0x200
-    HTTP_QPACK_ENCODER_STREAM_ERROR = 0x201
-    HTTP_QPACK_DECODER_STREAM_ERROR = 0x202
+    H3_NO_ERROR = 0x100
+    H3_GENERAL_PROTOCOL_ERROR = 0x101
+    H3_INTERNAL_ERROR = 0x102
+    H3_STREAM_CREATION_ERROR = 0x103
+    H3_CLOSED_CRITICAL_STREAM = 0x104
+    H3_FRAME_UNEXPECTED = 0x105
+    H3_FRAME_ERROR = 0x106
+    H3_EXCESSIVE_LOAD = 0x107
+    H3_ID_ERROR = 0x108
+    H3_SETTINGS_ERROR = 0x109
+    H3_MISSING_SETTINGS = 0x10A
+    H3_REQUEST_REJECTED = 0x10B
+    H3_REQUEST_CANCELLED = 0x10C
+    H3_REQUEST_INCOMPLETE = 0x10D
+    H3_MESSAGE_ERROR = 0x10E
+    H3_CONNECT_ERROR = 0x10F
+    H3_VERSION_FALLBACK = 0x110
+    QPACK_DECOMPRESSION_FAILED = 0x200
+    QPACK_ENCODER_STREAM_ERROR = 0x201
+    QPACK_DECODER_STREAM_ERROR = 0x202
 
 
 class FrameType(IntEnum):
     DATA = 0x0
     HEADERS = 0x1
     PRIORITY = 0x2
     CANCEL_PUSH = 0x3
@@ -81,38 +81,38 @@
     """
     Base class for protocol errors.
 
     These errors are not exposed to the API user, they are handled
     in :meth:`H3Connection.handle_event`.
     """
 
-    error_code = ErrorCode.HTTP_GENERAL_PROTOCOL_ERROR
+    error_code = ErrorCode.H3_GENERAL_PROTOCOL_ERROR
 
     def __init__(self, reason_phrase: str = ""):
         self.reason_phrase = reason_phrase
 
 
 class QpackDecompressionFailed(ProtocolError):
-    error_code = ErrorCode.HTTP_QPACK_DECOMPRESSION_FAILED
+    error_code = ErrorCode.QPACK_DECOMPRESSION_FAILED
 
 
 class QpackDecoderStreamError(ProtocolError):
-    error_code = ErrorCode.HTTP_QPACK_DECODER_STREAM_ERROR
+    error_code = ErrorCode.QPACK_DECODER_STREAM_ERROR
 
 
 class QpackEncoderStreamError(ProtocolError):
-    error_code = ErrorCode.HTTP_QPACK_ENCODER_STREAM_ERROR
+    error_code = ErrorCode.QPACK_ENCODER_STREAM_ERROR
 
 
 class StreamCreationError(ProtocolError):
-    error_code = ErrorCode.HTTP_STREAM_CREATION_ERROR
+    error_code = ErrorCode.H3_STREAM_CREATION_ERROR
 
 
 class FrameUnexpected(ProtocolError):
-    error_code = ErrorCode.HTTP_FRAME_UNEXPECTED
+    error_code = ErrorCode.H3_FRAME_UNEXPECTED
 
 
 def encode_frame(frame_type: int, frame_data: bytes) -> bytes:
     frame_length = len(frame_data)
     buf = Buffer(capacity=frame_length + 16)
     buf.push_uint_var(frame_type)
     buf.push_uint_var(frame_length)
```

### Comparing `aioquic-0.9.8/src/aioquic/h3/events.py` & `aioquic-0.9.9/src/aioquic/h3/events.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/src/aioquic/quic/configuration.py` & `aioquic-0.9.9/src/aioquic/quic/configuration.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/src/aioquic/quic/connection.py` & `aioquic-0.9.9/src/aioquic/quic/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,22 +10,24 @@
 from .. import tls
 from ..buffer import UINT_VAR_MAX, Buffer, BufferReadError, size_uint_var
 from . import events
 from .configuration import QuicConfiguration
 from .crypto import CryptoError, CryptoPair, KeyUnavailableError
 from .logger import QuicLoggerTrace
 from .packet import (
+    CONNECTION_ID_MAX_SIZE,
     NON_ACK_ELICITING_FRAME_TYPES,
     PACKET_TYPE_HANDSHAKE,
     PACKET_TYPE_INITIAL,
     PACKET_TYPE_ONE_RTT,
     PACKET_TYPE_RETRY,
     PACKET_TYPE_ZERO_RTT,
     PROBING_FRAME_TYPES,
     RETRY_INTEGRITY_TAG_SIZE,
+    STATELESS_RESET_TOKEN_SIZE,
     QuicErrorCode,
     QuicFrameType,
     QuicProtocolVersion,
     QuicStreamFrame,
     QuicTransportParameters,
     get_retry_integrity_tag,
     get_spin_bit,
@@ -67,24 +69,27 @@
         None,
         None,
         "SERVER_HANDSHAKE_TRAFFIC_SECRET",
         "SERVER_TRAFFIC_SECRET_0",
     ],
 ]
 STREAM_FLAGS = 0x07
+STREAM_COUNT_MAX = 0x1000000000000000
 
 NetworkAddress = Any
 
 # frame sizes
 ACK_FRAME_CAPACITY = 64  # FIXME: this is arbitrary!
 APPLICATION_CLOSE_FRAME_CAPACITY = 1 + 8 + 8  # + reason length
 CONNECTION_LIMIT_FRAME_CAPACITY = 1 + 8
 HANDSHAKE_DONE_FRAME_CAPACITY = 1
 MAX_STREAM_DATA_FRAME_CAPACITY = 1 + 8 + 8
-NEW_CONNECTION_ID_FRAME_CAPACITY = 1 + 8 + 8 + 1 + 20 + 16
+NEW_CONNECTION_ID_FRAME_CAPACITY = (
+    1 + 8 + 8 + 1 + CONNECTION_ID_MAX_SIZE + STATELESS_RESET_TOKEN_SIZE
+)
 PATH_CHALLENGE_FRAME_CAPACITY = 1 + 8
 PATH_RESPONSE_FRAME_CAPACITY = 1 + 8
 PING_FRAME_CAPACITY = 1
 RESET_STREAM_CAPACITY = 1 + 8 + 8 + 8
 RETIRE_CONNECTION_ID_CAPACITY = 1 + 8
 STREAMS_BLOCKED_CAPACITY = 1 + 8
 TRANSPORT_CLOSE_FRAME_CAPACITY = 1 + 8 + 8 + 8  # + reason length
@@ -628,15 +633,15 @@
         :param now: The current time.
         """
         # end of closing period or idle timeout
         if now >= self._close_at:
             if self._close_event is None:
                 self._close_event = events.ConnectionTerminated(
                     error_code=QuicErrorCode.INTERNAL_ERROR,
-                    frame_type=None,
+                    frame_type=QuicFrameType.PADDING,
                     reason_phrase="Idle timeout",
                 )
             self._close_end()
             return
 
         # loss detection timeout
         if self._loss_at is not None and now >= self._loss_at:
@@ -733,15 +738,15 @@
                 common = [
                     x for x in self._configuration.supported_versions if x in versions
                 ]
                 if not common:
                     self._logger.error("Could not find a common protocol version")
                     self._close_event = events.ConnectionTerminated(
                         error_code=QuicErrorCode.INTERNAL_ERROR,
-                        frame_type=None,
+                        frame_type=QuicFrameType.PADDING,
                         reason_phrase="Could not find a common protocol version",
                     )
                     self._close_end()
                     return
                 self._packet_number = 0
                 self._version = QuicProtocolVersion(common[0])
                 self._version_negotiation_count += 1
@@ -849,15 +854,15 @@
             if header.is_long_header:
                 reserved_mask = 0x0C
             else:
                 reserved_mask = 0x18
             if plain_header[0] & reserved_mask:
                 self.close(
                     error_code=QuicErrorCode.PROTOCOL_VIOLATION,
-                    frame_type=None,
+                    frame_type=QuicFrameType.PADDING,
                     reason_phrase="Reserved bits must be zero",
                 )
                 return
 
             # raise expected packet number
             if packet_number > space.expected_packet_number:
                 space.expected_packet_number = packet_number + 1
@@ -1589,14 +1594,20 @@
     ) -> None:
         """
         Handle a MAX_STREAMS_BIDI frame.
 
         This raises number of bidirectional streams we can initiate to the peer.
         """
         max_streams = buf.pull_uint_var()
+        if max_streams > STREAM_COUNT_MAX:
+            raise QuicConnectionError(
+                error_code=QuicErrorCode.FRAME_ENCODING_ERROR,
+                frame_type=frame_type,
+                reason_phrase="Maximum Streams cannot exceed 2^60",
+            )
 
         # log frame
         if self._quic_logger is not None:
             context.quic_logger_frames.append(
                 self._quic_logger.encode_connection_limit_frame(
                     frame_type=frame_type, maximum=max_streams
                 )
@@ -1612,14 +1623,20 @@
     ) -> None:
         """
         Handle a MAX_STREAMS_UNI frame.
 
         This raises number of unidirectional streams we can initiate to the peer.
         """
         max_streams = buf.pull_uint_var()
+        if max_streams > STREAM_COUNT_MAX:
+            raise QuicConnectionError(
+                error_code=QuicErrorCode.FRAME_ENCODING_ERROR,
+                frame_type=frame_type,
+                reason_phrase="Maximum Streams cannot exceed 2^60",
+            )
 
         # log frame
         if self._quic_logger is not None:
             context.quic_logger_frames.append(
                 self._quic_logger.encode_connection_limit_frame(
                     frame_type=frame_type, maximum=max_streams
                 )
@@ -1636,15 +1653,21 @@
         """
         Handle a NEW_CONNECTION_ID frame.
         """
         sequence_number = buf.pull_uint_var()
         retire_prior_to = buf.pull_uint_var()
         length = buf.pull_uint8()
         connection_id = buf.pull_bytes(length)
-        stateless_reset_token = buf.pull_bytes(16)
+        stateless_reset_token = buf.pull_bytes(STATELESS_RESET_TOKEN_SIZE)
+        if not connection_id or len(connection_id) > CONNECTION_ID_MAX_SIZE:
+            raise QuicConnectionError(
+                error_code=QuicErrorCode.FRAME_ENCODING_ERROR,
+                frame_type=frame_type,
+                reason_phrase="Length must be greater than 0 and less than 20",
+            )
 
         # log frame
         if self._quic_logger is not None:
             context.quic_logger_frames.append(
                 self._quic_logger.encode_new_connection_id_frame(
                     connection_id=connection_id,
                     retire_prior_to=retire_prior_to,
@@ -1654,15 +1677,15 @@
             )
 
         # sanity check
         if retire_prior_to > sequence_number:
             raise QuicConnectionError(
                 error_code=QuicErrorCode.PROTOCOL_VIOLATION,
                 frame_type=frame_type,
-                reason_phrase="retire_prior_to is greater than the sequence_number",
+                reason_phrase="Retire Prior To is greater than Sequence Number",
             )
 
         # determine which CIDs to retire
         change_cid = False
         retire = list(
             filter(
                 lambda c: c.sequence_number < retire_prior_to, self._peer_cid_available
@@ -2005,14 +2028,20 @@
     def _handle_streams_blocked_frame(
         self, context: QuicReceiveContext, frame_type: int, buf: Buffer
     ) -> None:
         """
         Handle a STREAMS_BLOCKED frame.
         """
         limit = buf.pull_uint_var()
+        if limit > STREAM_COUNT_MAX:
+            raise QuicConnectionError(
+                error_code=QuicErrorCode.FRAME_ENCODING_ERROR,
+                frame_type=frame_type,
+                reason_phrase="Maximum Streams cannot exceed 2^60",
+            )
 
         # log frame
         if self._quic_logger is not None:
             context.quic_logger_frames.append(
                 self._quic_logger.encode_streams_blocked_frame(
                     is_unidirectional=frame_type == QuicFrameType.STREAMS_BLOCKED_UNI,
                     limit=limit,
@@ -2110,14 +2139,15 @@
         self, context: QuicReceiveContext, plain: bytes
     ) -> Tuple[bool, bool]:
         """
         Handle a QUIC packet payload.
         """
         buf = Buffer(data=plain)
 
+        frame_found = False
         is_ack_eliciting = False
         is_probing = None
         while not buf.eof():
             frame_type = buf.pull_uint_var()
 
             # check frame type is known
             try:
@@ -2144,22 +2174,31 @@
                 raise QuicConnectionError(
                     error_code=QuicErrorCode.FRAME_ENCODING_ERROR,
                     frame_type=frame_type,
                     reason_phrase="Failed to parse frame",
                 )
 
             # update ACK only / probing flags
+            frame_found = True
+
             if frame_type not in NON_ACK_ELICITING_FRAME_TYPES:
                 is_ack_eliciting = True
 
             if frame_type not in PROBING_FRAME_TYPES:
                 is_probing = False
             elif is_probing is None:
                 is_probing = True
 
+        if not frame_found:
+            raise QuicConnectionError(
+                error_code=QuicErrorCode.PROTOCOL_VIOLATION,
+                frame_type=QuicFrameType.PADDING,
+                reason_phrase="Packet contains no frames",
+            )
+
         return is_ack_eliciting, bool(is_probing)
 
     def _replenish_connection_ids(self) -> None:
         """
         Generate new connection IDs.
         """
         while len(self._host_cids) < min(8, self._remote_active_connection_id_limit):
```

### Comparing `aioquic-0.9.8/src/aioquic/quic/crypto.py` & `aioquic-0.9.9/src/aioquic/quic/crypto.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/src/aioquic/quic/events.py` & `aioquic-0.9.9/src/aioquic/quic/events.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/src/aioquic/quic/logger.py` & `aioquic-0.9.9/src/aioquic/quic/logger.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/src/aioquic/quic/packet.py` & `aioquic-0.9.9/src/aioquic/quic/packet.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 CONNECTION_ID_MAX_SIZE = 20
 PACKET_NUMBER_MAX_SIZE = 4
 RETRY_AEAD_KEY_DRAFT_29 = binascii.unhexlify("ccce187ed09a09d05728155a6cb96be1")
 RETRY_AEAD_KEY_VERSION_1 = binascii.unhexlify("be0c690b9f66575a1d766b54e368c84e")
 RETRY_AEAD_NONCE_DRAFT_29 = binascii.unhexlify("e54930f97f2136f0530a8c1c")
 RETRY_AEAD_NONCE_VERSION_1 = binascii.unhexlify("461599d35d632bf2239825bb")
 RETRY_INTEGRITY_TAG_SIZE = 16
+STATELESS_RESET_TOKEN_SIZE = 16
 
 
 class QuicErrorCode(IntEnum):
     NO_ERROR = 0x0
     INTERNAL_ERROR = 0x1
     CONNECTION_REFUSED = 0x2
     FLOW_CONTROL_ERROR = 0x3
```

### Comparing `aioquic-0.9.8/src/aioquic/quic/packet_builder.py` & `aioquic-0.9.9/src/aioquic/quic/packet_builder.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/src/aioquic/quic/rangeset.py` & `aioquic-0.9.9/src/aioquic/quic/rangeset.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/src/aioquic/quic/recovery.py` & `aioquic-0.9.9/src/aioquic/quic/recovery.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/src/aioquic/quic/retry.py` & `aioquic-0.9.9/src/aioquic/quic/retry.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/src/aioquic/quic/stream.py` & `aioquic-0.9.9/src/aioquic/quic/stream.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/src/aioquic/tls.py` & `aioquic-0.9.9/src/aioquic/tls.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/src/aioquic.egg-info/PKG-INFO` & `aioquic-0.9.9/src/aioquic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aioquic
-Version: 0.9.8
+Version: 0.9.9
 Summary: An implementation of QUIC and HTTP/3
 Home-page: https://github.com/aiortc/aioquic
 Author: Jeremy Lainé
 Author-email: jeremy.laine@m4x.org
 License: BSD
 Description: aioquic
         =======
```

### Comparing `aioquic-0.9.8/src/aioquic.egg-info/SOURCES.txt` & `aioquic-0.9.9/src/aioquic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/tests/initial_client.bin` & `aioquic-0.9.9/tests/initial_client.bin`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/tests/pycacert.pem` & `aioquic-0.9.9/tests/pycacert.pem`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/tests/ssl_cert.pem` & `aioquic-0.9.9/tests/ssl_cert.pem`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/tests/ssl_cert_with_chain.pem` & `aioquic-0.9.9/tests/ssl_cert_with_chain.pem`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/tests/ssl_combined.pem` & `aioquic-0.9.9/tests/ssl_combined.pem`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/tests/ssl_key.pem` & `aioquic-0.9.9/tests/ssl_key.pem`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/tests/test_asyncio.py` & `aioquic-0.9.9/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/tests/test_asyncio_compat.py` & `aioquic-0.9.9/tests/test_asyncio_compat.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/tests/test_buffer.py` & `aioquic-0.9.9/tests/test_buffer.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/tests/test_connection.py` & `aioquic-0.9.9/tests/test_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from unittest import TestCase, skipIf
 
 from aioquic import tls
 from aioquic.buffer import UINT_VAR_MAX, Buffer, encode_uint_var
 from aioquic.quic import events
 from aioquic.quic.configuration import QuicConfiguration
 from aioquic.quic.connection import (
+    STREAM_COUNT_MAX,
     QuicConnection,
     QuicConnectionError,
     QuicNetworkPath,
     QuicReceiveContext,
 )
 from aioquic.quic.crypto import CryptoPair
 from aioquic.quic.logger import QuicLogger
@@ -902,15 +903,15 @@
         for datagram in builder.flush()[0]:
             client.receive_datagram(datagram, SERVER_ADDR, now=time.time())
         self.assertEqual(drop(client), 1)
         self.assertEqual(
             client._close_event,
             events.ConnectionTerminated(
                 error_code=QuicErrorCode.PROTOCOL_VIOLATION,
-                frame_type=None,
+                frame_type=QuicFrameType.PADDING,
                 reason_phrase="Reserved bits must be zero",
             ),
         )
 
     def test_receive_datagram_wrong_version(self):
         client = create_standalone_client(self)
 
@@ -1209,14 +1210,30 @@
             client._handle_max_streams_bidi_frame(
                 client_receive_context(client),
                 QuicFrameType.MAX_STREAMS_BIDI,
                 Buffer(data=encode_uint_var(127)),
             )
             self.assertEqual(client._remote_max_streams_bidi, 129)
 
+            # client receives invalid MAX_STREAMS_BIDI
+            with self.assertRaises(QuicConnectionError) as cm:
+                client._handle_max_streams_bidi_frame(
+                    client_receive_context(client),
+                    QuicFrameType.MAX_STREAMS_BIDI,
+                    Buffer(data=encode_uint_var(STREAM_COUNT_MAX + 1)),
+                )
+            self.assertEqual(
+                cm.exception.error_code,
+                QuicErrorCode.FRAME_ENCODING_ERROR,
+            )
+            self.assertEqual(cm.exception.frame_type, QuicFrameType.MAX_STREAMS_BIDI)
+            self.assertEqual(
+                cm.exception.reason_phrase, "Maximum Streams cannot exceed 2^60"
+            )
+
     def test_handle_max_streams_uni_frame(self):
         with client_and_server() as (client, server):
             self.assertEqual(client._remote_max_streams_uni, 128)
 
             # client receives MAX_STREAMS_UNI raising limit
             client._handle_max_streams_uni_frame(
                 client_receive_context(client),
@@ -1229,14 +1246,30 @@
             client._handle_max_streams_uni_frame(
                 client_receive_context(client),
                 QuicFrameType.MAX_STREAMS_UNI,
                 Buffer(data=encode_uint_var(127)),
             )
             self.assertEqual(client._remote_max_streams_uni, 129)
 
+            # client receives invalid MAX_STREAMS_UNI
+            with self.assertRaises(QuicConnectionError) as cm:
+                client._handle_max_streams_uni_frame(
+                    client_receive_context(client),
+                    QuicFrameType.MAX_STREAMS_UNI,
+                    Buffer(data=encode_uint_var(STREAM_COUNT_MAX + 1)),
+                )
+            self.assertEqual(
+                cm.exception.error_code,
+                QuicErrorCode.FRAME_ENCODING_ERROR,
+            )
+            self.assertEqual(cm.exception.frame_type, QuicFrameType.MAX_STREAMS_UNI)
+            self.assertEqual(
+                cm.exception.reason_phrase, "Maximum Streams cannot exceed 2^60"
+            )
+
     def test_handle_new_connection_id_duplicate(self):
         with client_and_server() as (client, server):
             buf = Buffer(capacity=100)
             buf.push_uint_var(7)  # sequence_number
             buf.push_uint_var(0)  # retire_prior_to
             buf.push_uint_var(8)
             buf.push_bytes(bytes(8))
@@ -1298,14 +1331,41 @@
             )
 
             self.assertEqual(client._peer_cid.sequence_number, 2)
             self.assertEqual(
                 sequence_numbers(client._peer_cid_available), [3, 4, 5, 6, 7, 8]
             )
 
+    def test_handle_new_connection_id_with_connection_id_invalid(self):
+        with client_and_server() as (client, server):
+            buf = Buffer(capacity=100)
+            buf.push_uint_var(8)  # sequence_number
+            buf.push_uint_var(2)  # retire_prior_to
+            buf.push_uint_var(21)
+            buf.push_bytes(bytes(21))
+            buf.push_bytes(bytes(16))
+            buf.seek(0)
+
+            # client receives NEW_CONNECTION_ID
+            with self.assertRaises(QuicConnectionError) as cm:
+                client._handle_new_connection_id_frame(
+                    client_receive_context(client),
+                    QuicFrameType.NEW_CONNECTION_ID,
+                    buf,
+                )
+            self.assertEqual(
+                cm.exception.error_code,
+                QuicErrorCode.FRAME_ENCODING_ERROR,
+            )
+            self.assertEqual(cm.exception.frame_type, QuicFrameType.NEW_CONNECTION_ID)
+            self.assertEqual(
+                cm.exception.reason_phrase,
+                "Length must be greater than 0 and less than 20",
+            )
+
     def test_handle_new_connection_id_with_retire_prior_to_invalid(self):
         with client_and_server() as (client, server):
             buf = Buffer(capacity=100)
             buf.push_uint_var(8)  # sequence_number
             buf.push_uint_var(9)  # retire_prior_to
             buf.push_uint_var(8)
             buf.push_bytes(bytes(8))
@@ -1322,15 +1382,15 @@
             self.assertEqual(
                 cm.exception.error_code,
                 QuicErrorCode.PROTOCOL_VIOLATION,
             )
             self.assertEqual(cm.exception.frame_type, QuicFrameType.NEW_CONNECTION_ID)
             self.assertEqual(
                 cm.exception.reason_phrase,
-                "retire_prior_to is greater than the sequence_number",
+                "Retire Prior To is greater than Sequence Number",
             )
 
     def test_handle_new_token_frame(self):
         with client_and_server() as (client, server):
             # client receives NEW_TOKEN
             client._handle_new_token_frame(
                 client_receive_context(client),
@@ -1798,14 +1858,30 @@
             # client receives STREAMS_BLOCKED_UNI: 0
             client._handle_streams_blocked_frame(
                 client_receive_context(client),
                 QuicFrameType.STREAMS_BLOCKED_UNI,
                 Buffer(data=b"\x00"),
             )
 
+            # client receives invalid STREAMS_BLOCKED_UNI
+            with self.assertRaises(QuicConnectionError) as cm:
+                client._handle_streams_blocked_frame(
+                    client_receive_context(client),
+                    QuicFrameType.STREAMS_BLOCKED_UNI,
+                    Buffer(data=encode_uint_var(STREAM_COUNT_MAX + 1)),
+                )
+            self.assertEqual(
+                cm.exception.error_code,
+                QuicErrorCode.FRAME_ENCODING_ERROR,
+            )
+            self.assertEqual(cm.exception.frame_type, QuicFrameType.STREAMS_BLOCKED_UNI)
+            self.assertEqual(
+                cm.exception.reason_phrase, "Maximum Streams cannot exceed 2^60"
+            )
+
     def test_parse_transport_parameters(self):
         client = create_standalone_client(self)
 
         data = encode_transport_parameters(
             QuicTransportParameters(
                 original_destination_connection_id=client.original_destination_connection_id
             )
@@ -1857,14 +1933,23 @@
             )
             self.assertEqual(cm.exception.frame_type, QuicFrameType.CRYPTO)
             self.assertEqual(
                 cm.exception.reason_phrase,
                 "original_destination_connection_id is not allowed for clients",
             )
 
+    def test_payload_received_empty(self):
+        with client_and_server() as (client, server):
+            # client receives empty payload
+            with self.assertRaises(QuicConnectionError) as cm:
+                client._payload_received(client_receive_context(client), b"")
+            self.assertEqual(cm.exception.error_code, QuicErrorCode.PROTOCOL_VIOLATION)
+            self.assertEqual(cm.exception.frame_type, QuicFrameType.PADDING)
+            self.assertEqual(cm.exception.reason_phrase, "Packet contains no frames")
+
     def test_payload_received_padding_only(self):
         with client_and_server() as (client, server):
             # client receives padding only
             is_ack_eliciting, is_probing = client._payload_received(
                 client_receive_context(client), b"\x00" * 1200
             )
             self.assertFalse(is_ack_eliciting)
@@ -2203,15 +2288,15 @@
             now=time.time(),
         )
         self.assertEqual(drop(client), 0)
 
         event = client.next_event()
         self.assertEqual(type(event), events.ConnectionTerminated)
         self.assertEqual(event.error_code, QuicErrorCode.INTERNAL_ERROR)
-        self.assertEqual(event.frame_type, None)
+        self.assertEqual(event.frame_type, QuicFrameType.PADDING)
         self.assertEqual(
             event.reason_phrase, "Could not find a common protocol version"
         )
 
     def test_version_negotiation_ignore(self):
         client = create_standalone_client(self)
```

### Comparing `aioquic-0.9.8/tests/test_crypto.py` & `aioquic-0.9.9/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/tests/test_crypto_draft_29.py` & `aioquic-0.9.9/tests/test_crypto_draft_29.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/tests/test_h0.py` & `aioquic-0.9.9/tests/test_h0.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/tests/test_h3.py` & `aioquic-0.9.9/tests/test_h3.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,15 @@
                 data=encode_uint_var(StreamType.CONTROL)
                 + encode_frame(FrameType.HEADERS, b""),
                 end_stream=False,
             )
         )
         self.assertEqual(
             quic_server.closed,
-            (ErrorCode.HTTP_FRAME_UNEXPECTED, "Invalid frame type on control stream"),
+            (ErrorCode.H3_FRAME_UNEXPECTED, "Invalid frame type on control stream"),
         )
 
     def test_handle_control_frame_max_push_id_from_server(self):
         """
         A client should not receive MAX_PUSH_ID on the control stream.
         """
         quic_client = FakeQuicConnection(
@@ -203,15 +203,15 @@
                 data=encode_uint_var(StreamType.CONTROL)
                 + encode_frame(FrameType.MAX_PUSH_ID, b""),
                 end_stream=False,
             )
         )
         self.assertEqual(
             quic_client.closed,
-            (ErrorCode.HTTP_FRAME_UNEXPECTED, "Servers must not send MAX_PUSH_ID"),
+            (ErrorCode.H3_FRAME_UNEXPECTED, "Servers must not send MAX_PUSH_ID"),
         )
 
     def test_handle_control_stream_duplicate(self):
         """
         We must only receive a single control stream.
         """
         quic_server = FakeQuicConnection(
@@ -231,15 +231,15 @@
             StreamDataReceived(
                 stream_id=6, data=encode_uint_var(StreamType.CONTROL), end_stream=False
             )
         )
         self.assertEqual(
             quic_server.closed,
             (
-                ErrorCode.HTTP_STREAM_CREATION_ERROR,
+                ErrorCode.H3_STREAM_CREATION_ERROR,
                 "Only one control stream is allowed",
             ),
         )
 
     def test_handle_push_frame_wrong_frame_type(self):
         """
         We should not received SETTINGS on a push stream.
@@ -256,15 +256,15 @@
                 + encode_uint_var(0)  # push ID
                 + encode_frame(FrameType.SETTINGS, b""),
                 end_stream=False,
             )
         )
         self.assertEqual(
             quic_client.closed,
-            (ErrorCode.HTTP_FRAME_UNEXPECTED, "Invalid frame type on push stream"),
+            (ErrorCode.H3_FRAME_UNEXPECTED, "Invalid frame type on push stream"),
         )
 
     def test_handle_qpack_decoder_duplicate(self):
         """
         We must only receive a single QPACK decoder stream.
         """
         quic_client = FakeQuicConnection(
@@ -288,15 +288,15 @@
                 data=encode_uint_var(StreamType.QPACK_DECODER),
                 end_stream=False,
             )
         )
         self.assertEqual(
             quic_client.closed,
             (
-                ErrorCode.HTTP_STREAM_CREATION_ERROR,
+                ErrorCode.H3_STREAM_CREATION_ERROR,
                 "Only one QPACK decoder stream is allowed",
             ),
         )
 
     def test_handle_qpack_decoder_stream_error(self):
         """
         Receiving garbage on the QPACK decoder stream triggers an exception.
@@ -309,17 +309,15 @@
         h3_client.handle_event(
             StreamDataReceived(
                 stream_id=11,
                 data=encode_uint_var(StreamType.QPACK_DECODER) + b"\x00",
                 end_stream=False,
             )
         )
-        self.assertEqual(
-            quic_client.closed, (ErrorCode.HTTP_QPACK_DECODER_STREAM_ERROR, "")
-        )
+        self.assertEqual(quic_client.closed, (ErrorCode.QPACK_DECODER_STREAM_ERROR, ""))
 
     def test_handle_qpack_encoder_duplicate(self):
         """
         We must only receive a single QPACK encoder stream.
         """
         quic_client = FakeQuicConnection(
             configuration=QuicConfiguration(is_client=True)
@@ -342,15 +340,15 @@
                 data=encode_uint_var(StreamType.QPACK_ENCODER),
                 end_stream=False,
             )
         )
         self.assertEqual(
             quic_client.closed,
             (
-                ErrorCode.HTTP_STREAM_CREATION_ERROR,
+                ErrorCode.H3_STREAM_CREATION_ERROR,
                 "Only one QPACK encoder stream is allowed",
             ),
         )
 
     def test_handle_qpack_encoder_stream_error(self):
         """
         Receiving garbage on the QPACK encoder stream triggers an exception.
@@ -363,17 +361,15 @@
         h3_client.handle_event(
             StreamDataReceived(
                 stream_id=7,
                 data=encode_uint_var(StreamType.QPACK_ENCODER) + b"\x00",
                 end_stream=False,
             )
         )
-        self.assertEqual(
-            quic_client.closed, (ErrorCode.HTTP_QPACK_ENCODER_STREAM_ERROR, "")
-        )
+        self.assertEqual(quic_client.closed, (ErrorCode.QPACK_ENCODER_STREAM_ERROR, ""))
 
     def test_handle_request_frame_bad_headers(self):
         """
         We should not receive HEADERS which cannot be decoded.
         """
         quic_server = FakeQuicConnection(
             configuration=QuicConfiguration(is_client=False)
@@ -381,17 +377,15 @@
         h3_server = H3Connection(quic_server)
 
         h3_server.handle_event(
             StreamDataReceived(
                 stream_id=0, data=encode_frame(FrameType.HEADERS, b""), end_stream=False
             )
         )
-        self.assertEqual(
-            quic_server.closed, (ErrorCode.HTTP_QPACK_DECOMPRESSION_FAILED, "")
-        )
+        self.assertEqual(quic_server.closed, (ErrorCode.QPACK_DECOMPRESSION_FAILED, ""))
 
     def test_handle_request_frame_data_before_headers(self):
         """
         We should not receive DATA before receiving headers.
         """
         quic_server = FakeQuicConnection(
             configuration=QuicConfiguration(is_client=False)
@@ -402,15 +396,15 @@
             StreamDataReceived(
                 stream_id=0, data=encode_frame(FrameType.DATA, b""), end_stream=False
             )
         )
         self.assertEqual(
             quic_server.closed,
             (
-                ErrorCode.HTTP_FRAME_UNEXPECTED,
+                ErrorCode.H3_FRAME_UNEXPECTED,
                 "DATA frame is not allowed in this state",
             ),
         )
 
     def test_handle_request_frame_headers_after_trailers(self):
         """
         We should not receive HEADERS after receiving trailers.
@@ -444,15 +438,15 @@
             StreamDataReceived(
                 stream_id=0, data=encode_frame(FrameType.HEADERS, b""), end_stream=False
             )
         )
         self.assertEqual(
             quic_server.closed,
             (
-                ErrorCode.HTTP_FRAME_UNEXPECTED,
+                ErrorCode.H3_FRAME_UNEXPECTED,
                 "HEADERS frame is not allowed in this state",
             ),
         )
 
     def test_handle_request_frame_push_promise_from_client(self):
         """
         A server should not receive PUSH_PROMISE on a request stream.
@@ -467,15 +461,15 @@
                 stream_id=0,
                 data=encode_frame(FrameType.PUSH_PROMISE, b""),
                 end_stream=False,
             )
         )
         self.assertEqual(
             quic_server.closed,
-            (ErrorCode.HTTP_FRAME_UNEXPECTED, "Clients must not send PUSH_PROMISE"),
+            (ErrorCode.H3_FRAME_UNEXPECTED, "Clients must not send PUSH_PROMISE"),
         )
 
     def test_handle_request_frame_wrong_frame_type(self):
         quic_server = FakeQuicConnection(
             configuration=QuicConfiguration(is_client=False)
         )
         h3_server = H3Connection(quic_server)
@@ -485,15 +479,15 @@
                 stream_id=0,
                 data=encode_frame(FrameType.SETTINGS, b""),
                 end_stream=False,
             )
         )
         self.assertEqual(
             quic_server.closed,
-            (ErrorCode.HTTP_FRAME_UNEXPECTED, "Invalid frame type on request stream"),
+            (ErrorCode.H3_FRAME_UNEXPECTED, "Invalid frame type on request stream"),
         )
 
     def test_request(self):
         with h3_client_and_server() as (quic_client, quic_server):
             h3_client = H3Connection(quic_client)
             h3_server = H3Connection(quic_server)
```

### Comparing `aioquic-0.9.8/tests/test_logger.py` & `aioquic-0.9.9/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/tests/test_packet.py` & `aioquic-0.9.9/tests/test_packet.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/tests/test_packet_builder.py` & `aioquic-0.9.9/tests/test_packet_builder.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/tests/test_rangeset.py` & `aioquic-0.9.9/tests/test_rangeset.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/tests/test_recovery.py` & `aioquic-0.9.9/tests/test_recovery.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/tests/test_retry.py` & `aioquic-0.9.9/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/tests/test_stream.py` & `aioquic-0.9.9/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/tests/test_tls.py` & `aioquic-0.9.9/tests/test_tls.py`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/tests/tls_certificate.bin` & `aioquic-0.9.9/tests/tls_certificate.bin`

 * *Files identical despite different names*

### Comparing `aioquic-0.9.8/tests/utils.py` & `aioquic-0.9.9/tests/utils.py`

 * *Files identical despite different names*

