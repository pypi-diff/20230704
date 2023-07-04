# Comparing `tmp/rotki-pysqlcipher3-2023.5.1.tar.gz` & `tmp/rotki-pysqlcipher3-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotki-pysqlcipher3-2023.5.1.tar", last modified: Sat May 27 21:42:31 2023, max compression
+gzip compressed data, was "rotki-pysqlcipher3-2023.7.1.tar", last modified: Tue Jul  4 12:26:10 2023, max compression
```

## Comparing `rotki-pysqlcipher3-2023.5.1.tar` & `rotki-pysqlcipher3-2023.7.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 21:42:31.424942 rotki-pysqlcipher3-2023.5.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-05-27 21:42:31.424942 rotki-pysqlcipher3-2023.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4976 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 21:42:31.408942 rotki-pysqlcipher3-2023.5.1/lib/
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3156 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/dbapi2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2825 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/dump.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 21:42:31.412942 rotki-pysqlcipher3-2023.5.1/lib/test/
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 21:42:31.412942 rotki-pysqlcipher3-2023.5.1/lib/test/python2/
--rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/test/python2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    29889 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/test/python2/dbapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     1756 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/test/python2/dump.py
--rw-r--r--   0 runner    (1001) docker     (122)     7945 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/test/python2/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     6579 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/test/python2/hooks.py
--rw-r--r--   0 runner    (1001) docker     (122)     9692 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/test/python2/regression.py
--rw-r--r--   0 runner    (1001) docker     (122)     3792 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/test/python2/sqlcipher.py
--rw-r--r--   0 runner    (1001) docker     (122)     7359 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/test/python2/transactions.py
--rw-r--r--   0 runner    (1001) docker     (122)    14836 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/test/python2/types.py
--rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/test/python2/userfunctions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 21:42:31.416942 rotki-pysqlcipher3-2023.5.1/lib/test/python3/
--rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/test/python3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    31420 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/test/python3/dbapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     2852 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/test/python3/dump.py
--rw-r--r--   0 runner    (1001) docker     (122)     9632 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/test/python3/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     9426 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/test/python3/hooks.py
--rw-r--r--   0 runner    (1001) docker     (122)    12932 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/test/python3/regression.py
--rw-r--r--   0 runner    (1001) docker     (122)     3792 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/test/python3/sqlcipher.py
--rw-r--r--   0 runner    (1001) docker     (122)     7350 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/test/python3/transactions.py
--rw-r--r--   0 runner    (1001) docker     (122)    14447 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/test/python3/types.py
--rw-r--r--   0 runner    (1001) docker     (122)    15035 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/lib/test/python3/userfunctions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 21:42:31.416942 rotki-pysqlcipher3-2023.5.1/rotki_pysqlcipher3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-05-27 21:42:31.000000 rotki-pysqlcipher3-2023.5.1/rotki_pysqlcipher3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1736 2023-05-27 21:42:31.000000 rotki-pysqlcipher3-2023.5.1/rotki_pysqlcipher3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-27 21:42:31.000000 rotki-pysqlcipher3-2023.5.1/rotki_pysqlcipher3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-27 21:42:31.000000 rotki-pysqlcipher3-2023.5.1/rotki_pysqlcipher3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-27 21:42:31.424942 rotki-pysqlcipher3-2023.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     7142 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 21:42:31.408942 rotki-pysqlcipher3-2023.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 21:42:31.420942 rotki-pysqlcipher3-2023.5.1/src/python2/
--rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python2/backup.h
--rw-r--r--   0 runner    (1001) docker     (122)    12932 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python2/cache.c
--rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python2/cache.h
--rw-r--r--   0 runner    (1001) docker     (122)    50435 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python2/connection.c
--rw-r--r--   0 runner    (1001) docker     (122)     5149 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python2/connection.h
--rw-r--r--   0 runner    (1001) docker     (122)    35338 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python2/cursor.c
--rw-r--r--   0 runner    (1001) docker     (122)     2579 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python2/cursor.h
--rw-r--r--   0 runner    (1001) docker     (122)     4357 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python2/microprotocols.c
--rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python2/microprotocols.h
--rw-r--r--   0 runner    (1001) docker     (122)    15264 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python2/module.c
--rw-r--r--   0 runner    (1001) docker     (122)     2018 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python2/module.h
--rw-r--r--   0 runner    (1001) docker     (122)     4420 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python2/prepare_protocol.c
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python2/prepare_protocol.h
--rw-r--r--   0 runner    (1001) docker     (122)     8859 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python2/row.c
--rw-r--r--   0 runner    (1001) docker     (122)     1270 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python2/row.h
--rw-r--r--   0 runner    (1001) docker     (122)     1945 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python2/sqlitecompat.h
--rw-r--r--   0 runner    (1001) docker     (122)    18329 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python2/statement.c
--rw-r--r--   0 runner    (1001) docker     (122)     2174 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python2/statement.h
--rw-r--r--   0 runner    (1001) docker     (122)     3318 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python2/util.c
--rw-r--r--   0 runner    (1001) docker     (122)     1431 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python2/util.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 21:42:31.424942 rotki-pysqlcipher3-2023.5.1/src/python3/
--rw-r--r--   0 runner    (1001) docker     (122)    12485 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python3/cache.c
--rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python3/cache.h
--rw-r--r--   0 runner    (1001) docker     (122)    50947 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python3/connection.c
--rw-r--r--   0 runner    (1001) docker     (122)     4870 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python3/connection.h
--rw-r--r--   0 runner    (1001) docker     (122)    35359 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python3/cursor.c
--rw-r--r--   0 runner    (1001) docker     (122)     2596 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python3/cursor.h
--rw-r--r--   0 runner    (1001) docker     (122)     4445 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python3/microprotocols.c
--rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python3/microprotocols.h
--rw-r--r--   0 runner    (1001) docker     (122)    15501 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python3/module.c
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python3/module.h
--rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python3/prepare_protocol.c
--rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python3/prepare_protocol.h
--rw-r--r--   0 runner    (1001) docker     (122)     9449 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python3/row.c
--rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python3/row.h
--rw-r--r--   0 runner    (1001) docker     (122)    17401 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python3/statement.c
--rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python3/statement.h
--rw-r--r--   0 runner    (1001) docker     (122)     5237 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python3/util.c
--rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-05-27 21:42:21.000000 rotki-pysqlcipher3-2023.5.1/src/python3/util.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:26:10.426508 rotki-pysqlcipher3-2023.7.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-07-04 12:26:10.426508 rotki-pysqlcipher3-2023.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4976 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:26:10.398506 rotki-pysqlcipher3-2023.7.1/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3156 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/dbapi2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2825 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/dump.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:26:10.398506 rotki-pysqlcipher3-2023.7.1/lib/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:26:10.402506 rotki-pysqlcipher3-2023.7.1/lib/test/python2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/test/python2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29889 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/test/python2/dbapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1756 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/test/python2/dump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7945 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/test/python2/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6579 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/test/python2/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9692 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/test/python2/regression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3792 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/test/python2/sqlcipher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7359 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/test/python2/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14836 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/test/python2/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/test/python2/userfunctions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:26:10.410507 rotki-pysqlcipher3-2023.7.1/lib/test/python3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/test/python3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31420 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/test/python3/dbapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2852 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/test/python3/dump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9632 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/test/python3/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9426 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/test/python3/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12932 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/test/python3/regression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3792 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/test/python3/sqlcipher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7350 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/test/python3/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14447 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/test/python3/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15035 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/lib/test/python3/userfunctions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:26:10.410507 rotki-pysqlcipher3-2023.7.1/rotki_pysqlcipher3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-07-04 12:26:10.000000 rotki-pysqlcipher3-2023.7.1/rotki_pysqlcipher3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1736 2023-07-04 12:26:10.000000 rotki-pysqlcipher3-2023.7.1/rotki_pysqlcipher3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-04 12:26:10.000000 rotki-pysqlcipher3-2023.7.1/rotki_pysqlcipher3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-04 12:26:10.000000 rotki-pysqlcipher3-2023.7.1/rotki_pysqlcipher3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-04 12:26:10.426508 rotki-pysqlcipher3-2023.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     7223 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:26:10.398506 rotki-pysqlcipher3-2023.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:26:10.418507 rotki-pysqlcipher3-2023.7.1/src/python2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python2/backup.h
+-rw-r--r--   0 runner    (1001) docker     (122)    12932 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python2/cache.c
+-rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python2/cache.h
+-rw-r--r--   0 runner    (1001) docker     (122)    50435 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python2/connection.c
+-rw-r--r--   0 runner    (1001) docker     (122)     5149 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python2/connection.h
+-rw-r--r--   0 runner    (1001) docker     (122)    35338 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python2/cursor.c
+-rw-r--r--   0 runner    (1001) docker     (122)     2579 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python2/cursor.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4357 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python2/microprotocols.c
+-rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python2/microprotocols.h
+-rw-r--r--   0 runner    (1001) docker     (122)    15264 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python2/module.c
+-rw-r--r--   0 runner    (1001) docker     (122)     2018 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python2/module.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4420 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python2/prepare_protocol.c
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python2/prepare_protocol.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8859 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python2/row.c
+-rw-r--r--   0 runner    (1001) docker     (122)     1270 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python2/row.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1945 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python2/sqlitecompat.h
+-rw-r--r--   0 runner    (1001) docker     (122)    18329 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python2/statement.c
+-rw-r--r--   0 runner    (1001) docker     (122)     2174 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python2/statement.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3318 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python2/util.c
+-rw-r--r--   0 runner    (1001) docker     (122)     1431 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python2/util.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 12:26:10.426508 rotki-pysqlcipher3-2023.7.1/src/python3/
+-rw-r--r--   0 runner    (1001) docker     (122)    12485 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python3/cache.c
+-rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python3/cache.h
+-rw-r--r--   0 runner    (1001) docker     (122)    50947 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python3/connection.c
+-rw-r--r--   0 runner    (1001) docker     (122)     4870 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python3/connection.h
+-rw-r--r--   0 runner    (1001) docker     (122)    35359 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python3/cursor.c
+-rw-r--r--   0 runner    (1001) docker     (122)     2596 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python3/cursor.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4445 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python3/microprotocols.c
+-rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python3/microprotocols.h
+-rw-r--r--   0 runner    (1001) docker     (122)    15501 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python3/module.c
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python3/module.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python3/prepare_protocol.c
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python3/prepare_protocol.h
+-rw-r--r--   0 runner    (1001) docker     (122)     9449 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python3/row.c
+-rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python3/row.h
+-rw-r--r--   0 runner    (1001) docker     (122)    17401 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python3/statement.c
+-rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python3/statement.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5237 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python3/util.c
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-07-04 12:26:00.000000 rotki-pysqlcipher3-2023.7.1/src/python3/util.h
```

### Comparing `rotki-pysqlcipher3-2023.5.1/LICENSE` & `rotki-pysqlcipher3-2023.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/PKG-INFO` & `rotki-pysqlcipher3-2023.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotki-pysqlcipher3
-Version: 2023.5.1
+Version: 2023.7.1
 Summary: DB-API 2.0 interface for SQLCIPHER 4.x
 Home-page: https://github.com/rotki/pysqlcipher3
 Author: Rotki Solutions GmbH
 Author-email: info@rotki.com
 License: zlib/libpng
 Platform: ALL
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rotki-pysqlcipher3-2023.5.1/README.rst` & `rotki-pysqlcipher3-2023.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/__init__.py` & `rotki-pysqlcipher3-2023.7.1/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/dbapi2.py` & `rotki-pysqlcipher3-2023.7.1/lib/dbapi2.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/dump.py` & `rotki-pysqlcipher3-2023.7.1/lib/dump.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/test/__init__.py` & `rotki-pysqlcipher3-2023.7.1/lib/test/__init__.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/test/python2/__init__.py` & `rotki-pysqlcipher3-2023.7.1/lib/test/python2/__init__.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/test/python2/dbapi.py` & `rotki-pysqlcipher3-2023.7.1/lib/test/python2/dbapi.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/test/python2/dump.py` & `rotki-pysqlcipher3-2023.7.1/lib/test/python2/dump.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/test/python2/factory.py` & `rotki-pysqlcipher3-2023.7.1/lib/test/python2/factory.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/test/python2/hooks.py` & `rotki-pysqlcipher3-2023.7.1/lib/test/python2/hooks.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/test/python2/regression.py` & `rotki-pysqlcipher3-2023.7.1/lib/test/python2/regression.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/test/python2/sqlcipher.py` & `rotki-pysqlcipher3-2023.7.1/lib/test/python2/sqlcipher.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/test/python2/transactions.py` & `rotki-pysqlcipher3-2023.7.1/lib/test/python2/transactions.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/test/python2/types.py` & `rotki-pysqlcipher3-2023.7.1/lib/test/python2/types.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/test/python2/userfunctions.py` & `rotki-pysqlcipher3-2023.7.1/lib/test/python2/userfunctions.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/test/python3/__init__.py` & `rotki-pysqlcipher3-2023.7.1/lib/test/python3/__init__.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/test/python3/dbapi.py` & `rotki-pysqlcipher3-2023.7.1/lib/test/python3/dbapi.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/test/python3/dump.py` & `rotki-pysqlcipher3-2023.7.1/lib/test/python3/dump.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/test/python3/factory.py` & `rotki-pysqlcipher3-2023.7.1/lib/test/python3/factory.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/test/python3/hooks.py` & `rotki-pysqlcipher3-2023.7.1/lib/test/python3/hooks.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/test/python3/regression.py` & `rotki-pysqlcipher3-2023.7.1/lib/test/python3/regression.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/test/python3/sqlcipher.py` & `rotki-pysqlcipher3-2023.7.1/lib/test/python3/sqlcipher.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/test/python3/transactions.py` & `rotki-pysqlcipher3-2023.7.1/lib/test/python3/transactions.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/test/python3/types.py` & `rotki-pysqlcipher3-2023.7.1/lib/test/python3/types.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/lib/test/python3/userfunctions.py` & `rotki-pysqlcipher3-2023.7.1/lib/test/python3/userfunctions.py`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/rotki_pysqlcipher3.egg-info/PKG-INFO` & `rotki-pysqlcipher3-2023.7.1/rotki_pysqlcipher3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotki-pysqlcipher3
-Version: 2023.5.1
+Version: 2023.7.1
 Summary: DB-API 2.0 interface for SQLCIPHER 4.x
 Home-page: https://github.com/rotki/pysqlcipher3
 Author: Rotki Solutions GmbH
 Author-email: info@rotki.com
 License: zlib/libpng
 Platform: ALL
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rotki-pysqlcipher3-2023.5.1/rotki_pysqlcipher3.egg-info/SOURCES.txt` & `rotki-pysqlcipher3-2023.7.1/rotki_pysqlcipher3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/setup.py` & `rotki-pysqlcipher3-2023.7.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: ISO-8859-1 -*-
 # setup.py: the distutils script
 #
+# Copyright (C) 2022 Rotki Solutions GmbH <info@rotki.com>
 # Copyright (C) 2015 David Riggleman <davidriggleman@gmail.com>
 # Copyright (C) 2013 Kali Kaneko <kali@futeisha.org> (sqlcipher support)
 # Copyright (C) 2005-2010 Gerhard Häring <gh@ghaering.de>
 #
 # This file is part of pysqlcipher.
 #
 # This software is provided 'as-is', without any express or implied
@@ -29,15 +30,15 @@
 from distutils import log
 from distutils.command.build_ext import build_ext
 from setuptools import Extension
 
 # If you need to change anything, it should be enough to change setup.cfg.
 
 PACKAGE_NAME = "pysqlcipher3"
-VERSION = '2023.5.1'
+VERSION = '2023.7.1'
 LONG_DESCRIPTION = \
 """Python interface to SQLCipher
 
 pysqlcipher3 is an interface to the SQLite 3.x embedded relational
 database engine. It is almost fully compliant with the Python database API
 version 2.0. At the same time, it also exposes the unique features of
 SQLCipher. This build has SQLCipher 4.x statically linked."""
@@ -127,15 +128,15 @@
 
             # Configure the linker
             ext.extra_link_args.append("libcrypto.lib")
             ext.extra_link_args.append("User32.lib")
             ext.extra_link_args.append("advapi32.lib")
             ext.extra_link_args.append(f'/LIBPATH:{openssl_lib_path}')
         else:
-            ext.extra_link_args.append("-lcrypto")
+            ext.extra_link_args.append("/usr/local/ssl/lib/libcrypto.a")
 
         build_ext.build_extension(self, ext)
 
     def __setattr__(self, k, v):
         # Make sure we don't link against the SQLite
         # library, no matter what setup.cfg says
         if k == "libraries":
```

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python2/backup.h` & `rotki-pysqlcipher3-2023.7.1/src/python2/backup.h`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python2/cache.c` & `rotki-pysqlcipher3-2023.7.1/src/python2/cache.c`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python2/cache.h` & `rotki-pysqlcipher3-2023.7.1/src/python2/cache.h`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python2/connection.c` & `rotki-pysqlcipher3-2023.7.1/src/python2/connection.c`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python2/connection.h` & `rotki-pysqlcipher3-2023.7.1/src/python2/connection.h`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python2/cursor.c` & `rotki-pysqlcipher3-2023.7.1/src/python2/cursor.c`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python2/cursor.h` & `rotki-pysqlcipher3-2023.7.1/src/python2/cursor.h`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python2/microprotocols.c` & `rotki-pysqlcipher3-2023.7.1/src/python2/microprotocols.c`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python2/microprotocols.h` & `rotki-pysqlcipher3-2023.7.1/src/python2/microprotocols.h`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python2/module.c` & `rotki-pysqlcipher3-2023.7.1/src/python2/module.c`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python2/module.h` & `rotki-pysqlcipher3-2023.7.1/src/python2/module.h`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python2/prepare_protocol.c` & `rotki-pysqlcipher3-2023.7.1/src/python2/prepare_protocol.c`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python2/prepare_protocol.h` & `rotki-pysqlcipher3-2023.7.1/src/python2/prepare_protocol.h`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python2/row.c` & `rotki-pysqlcipher3-2023.7.1/src/python2/row.c`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python2/row.h` & `rotki-pysqlcipher3-2023.7.1/src/python2/row.h`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python2/sqlitecompat.h` & `rotki-pysqlcipher3-2023.7.1/src/python2/sqlitecompat.h`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python2/statement.c` & `rotki-pysqlcipher3-2023.7.1/src/python2/statement.c`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python2/statement.h` & `rotki-pysqlcipher3-2023.7.1/src/python2/statement.h`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python2/util.c` & `rotki-pysqlcipher3-2023.7.1/src/python2/util.c`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python2/util.h` & `rotki-pysqlcipher3-2023.7.1/src/python2/util.h`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python3/cache.c` & `rotki-pysqlcipher3-2023.7.1/src/python3/cache.c`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python3/cache.h` & `rotki-pysqlcipher3-2023.7.1/src/python3/cache.h`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python3/connection.c` & `rotki-pysqlcipher3-2023.7.1/src/python3/connection.c`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python3/connection.h` & `rotki-pysqlcipher3-2023.7.1/src/python3/connection.h`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python3/cursor.c` & `rotki-pysqlcipher3-2023.7.1/src/python3/cursor.c`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python3/cursor.h` & `rotki-pysqlcipher3-2023.7.1/src/python3/cursor.h`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python3/microprotocols.c` & `rotki-pysqlcipher3-2023.7.1/src/python3/microprotocols.c`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python3/microprotocols.h` & `rotki-pysqlcipher3-2023.7.1/src/python3/microprotocols.h`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python3/module.c` & `rotki-pysqlcipher3-2023.7.1/src/python3/module.c`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python3/module.h` & `rotki-pysqlcipher3-2023.7.1/src/python3/module.h`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python3/prepare_protocol.c` & `rotki-pysqlcipher3-2023.7.1/src/python3/prepare_protocol.c`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python3/prepare_protocol.h` & `rotki-pysqlcipher3-2023.7.1/src/python3/prepare_protocol.h`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python3/row.c` & `rotki-pysqlcipher3-2023.7.1/src/python3/row.c`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python3/row.h` & `rotki-pysqlcipher3-2023.7.1/src/python3/row.h`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python3/statement.c` & `rotki-pysqlcipher3-2023.7.1/src/python3/statement.c`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python3/statement.h` & `rotki-pysqlcipher3-2023.7.1/src/python3/statement.h`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python3/util.c` & `rotki-pysqlcipher3-2023.7.1/src/python3/util.c`

 * *Files identical despite different names*

### Comparing `rotki-pysqlcipher3-2023.5.1/src/python3/util.h` & `rotki-pysqlcipher3-2023.7.1/src/python3/util.h`

 * *Files identical despite different names*

