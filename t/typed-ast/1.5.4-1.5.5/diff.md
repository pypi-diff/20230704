# Comparing `tmp/typed_ast-1.5.4.tar.gz` & `tmp/typed_ast-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typed_ast-1.5.4.tar", last modified: Sat May 21 21:11:36 2022, max compression
+gzip compressed data, was "typed_ast-1.5.5.tar", last modified: Mon Jul  3 22:56:33 2023, max compression
```

## Comparing `typed_ast-1.5.4.tar` & `typed_ast-1.5.5.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 21:11:36.865009 typed_ast-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (121)    15191 2022-05-21 21:11:28.000000 typed_ast-1.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-05-21 21:11:28.000000 typed_ast-1.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-05-21 21:11:36.865009 typed_ast-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3609 2022-05-21 21:11:28.000000 typed_ast-1.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 21:11:36.857009 typed_ast-1.5.4/ast27/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 21:11:36.857009 typed_ast-1.5.4/ast27/Custom/
--rw-r--r--   0 runner    (1001) docker     (121)     8986 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Custom/typed_ast.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 21:11:36.857009 typed_ast-1.5.4/ast27/Grammar/
--rw-r--r--   0 runner    (1001) docker     (121)     6545 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Grammar/Grammar
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 21:11:36.857009 typed_ast-1.5.4/ast27/Include/
--rw-r--r--   0 runner    (1001) docker     (121)    22386 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Include/Python-ast.h
--rw-r--r--   0 runner    (1001) docker     (121)     1285 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Include/asdl.h
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Include/ast.h
--rw-r--r--   0 runner    (1001) docker     (121)      798 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Include/bitset.h
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Include/compile.h
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Include/errcode.h
--rw-r--r--   0 runner    (1001) docker     (121)     1988 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Include/graminit.h
--rw-r--r--   0 runner    (1001) docker     (121)     2032 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Include/grammar.h
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Include/node.h
--rw-r--r--   0 runner    (1001) docker     (121)     1845 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Include/parsetok.h
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Include/pgenheaders.h
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Include/pyarena.h
--rw-r--r--   0 runner    (1001) docker     (121)     2656 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Include/pycore_pyarena.h
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Include/token.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 21:11:36.857009 typed_ast-1.5.4/ast27/Parser/
--rw-r--r--   0 runner    (1001) docker     (121)     4839 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Parser/Python.asdl
--rw-r--r--   0 runner    (1001) docker     (121)     3404 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Parser/acceler.c
--rw-r--r--   0 runner    (1001) docker     (121)    11320 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Parser/asdl.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    41795 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Parser/asdl_c.py
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Parser/bitset.c
--rw-r--r--   0 runner    (1001) docker     (121)     6947 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Parser/grammar.c
--rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Parser/grammar1.c
--rw-r--r--   0 runner    (1001) docker     (121)     4568 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Parser/node.c
--rw-r--r--   0 runner    (1001) docker     (121)    11502 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Parser/parser.c
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Parser/parser.h
--rw-r--r--   0 runner    (1001) docker     (121)    11524 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Parser/parsetok.c
--rw-r--r--   0 runner    (1001) docker     (121)    26962 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Parser/spark.py
--rw-r--r--   0 runner    (1001) docker     (121)    52538 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Parser/tokenizer.c
--rw-r--r--   0 runner    (1001) docker     (121)     3024 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Parser/tokenizer.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 21:11:36.861009 typed_ast-1.5.4/ast27/Python/
--rw-r--r--   0 runner    (1001) docker     (121)   280357 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Python/Python-ast.c
--rw-r--r--   0 runner    (1001) docker     (121)     1449 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Python/asdl.c
--rw-r--r--   0 runner    (1001) docker     (121)   118113 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Python/ast.c
--rw-r--r--   0 runner    (1001) docker     (121)    45695 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Python/graminit.c
--rw-r--r--   0 runner    (1001) docker     (121)     9483 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast27/Python/mystrtoul.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 21:11:36.857009 typed_ast-1.5.4/ast3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 21:11:36.861009 typed_ast-1.5.4/ast3/Custom/
--rw-r--r--   0 runner    (1001) docker     (121)    10221 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Custom/typed_ast.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 21:11:36.861009 typed_ast-1.5.4/ast3/Grammar/
--rw-r--r--   0 runner    (1001) docker     (121)     7328 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Grammar/Grammar
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 21:11:36.861009 typed_ast-1.5.4/ast3/Include/
--rw-r--r--   0 runner    (1001) docker     (121)    23443 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Include/Python-ast.h
--rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Include/asdl.h
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Include/ast.h
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Include/bitset.h
--rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Include/errcode.h
--rw-r--r--   0 runner    (1001) docker     (121)     2063 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Include/graminit.h
--rw-r--r--   0 runner    (1001) docker     (121)     2323 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Include/grammar.h
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Include/node.h
--rw-r--r--   0 runner    (1001) docker     (121)     2899 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Include/parsetok.h
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Include/pgenheaders.h
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Include/pyarena.h
--rw-r--r--   0 runner    (1001) docker     (121)     2653 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Include/pycore_pyarena.h
--rw-r--r--   0 runner    (1001) docker     (121)     2569 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Include/token.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 21:11:36.861009 typed_ast-1.5.4/ast3/Parser/
--rw-r--r--   0 runner    (1001) docker     (121)     5466 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Parser/Python.asdl
--rw-r--r--   0 runner    (1001) docker     (121)     3401 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Parser/acceler.c
--rw-r--r--   0 runner    (1001) docker     (121)    12881 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Parser/asdl.py
--rw-r--r--   0 runner    (1001) docker     (121)    45012 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Parser/asdl_c.py
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Parser/bitset.c
--rw-r--r--   0 runner    (1001) docker     (121)     7665 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Parser/grammar.c
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Parser/grammar1.c
--rw-r--r--   0 runner    (1001) docker     (121)     4566 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Parser/node.c
--rw-r--r--   0 runner    (1001) docker     (121)    11577 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Parser/parser.c
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Parser/parser.h
--rw-r--r--   0 runner    (1001) docker     (121)    13272 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Parser/parsetok.c
--rw-r--r--   0 runner    (1001) docker     (121)    58106 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Parser/tokenizer.c
--rw-r--r--   0 runner    (1001) docker     (121)     3592 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Parser/tokenizer.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 21:11:36.865009 typed_ast-1.5.4/ast3/Python/
--rw-r--r--   0 runner    (1001) docker     (121)   282113 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Python/Python-ast.c
--rw-r--r--   0 runner    (1001) docker     (121)     1435 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Python/asdl.c
--rw-r--r--   0 runner    (1001) docker     (121)   175785 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Python/ast.c
--rw-r--r--   0 runner    (1001) docker     (121)    48037 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/Python/graminit.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 21:11:36.865009 typed_ast-1.5.4/ast3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     7516 2022-05-21 21:11:28.000000 typed_ast-1.5.4/ast3/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-21 21:11:36.865009 typed_ast-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4429 2022-05-21 21:11:28.000000 typed_ast-1.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 21:11:36.865009 typed_ast-1.5.4/typed_ast/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-21 21:11:28.000000 typed_ast-1.5.4/typed_ast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12630 2022-05-21 21:11:28.000000 typed_ast-1.5.4/typed_ast/ast27.py
--rw-r--r--   0 runner    (1001) docker     (121)    13761 2022-05-21 21:11:28.000000 typed_ast-1.5.4/typed_ast/ast3.py
--rw-r--r--   0 runner    (1001) docker     (121)     8632 2022-05-21 21:11:28.000000 typed_ast-1.5.4/typed_ast/conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 21:11:36.865009 typed_ast-1.5.4/typed_ast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-05-21 21:11:36.000000 typed_ast-1.5.4/typed_ast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1819 2022-05-21 21:11:36.000000 typed_ast-1.5.4/typed_ast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-21 21:11:36.000000 typed_ast-1.5.4/typed_ast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-05-21 21:11:36.000000 typed_ast-1.5.4/typed_ast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:56:33.786288 typed_ast-1.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-07-03 22:56:26.000000 typed_ast-1.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-03 22:56:26.000000 typed_ast-1.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-03 22:56:33.786288 typed_ast-1.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-03 22:56:26.000000 typed_ast-1.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:56:33.774288 typed_ast-1.5.5/ast27/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:56:33.774288 typed_ast-1.5.5/ast27/Custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Custom/typed_ast.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:56:33.774288 typed_ast-1.5.5/ast27/Grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Grammar/Grammar
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:56:33.778288 typed_ast-1.5.5/ast27/Include/
+-rw-r--r--   0 runner    (1001) docker     (123)    22386 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Include/Python-ast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Include/asdl.h
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Include/ast.h
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Include/bitset.h
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Include/compile.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Include/errcode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Include/graminit.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Include/grammar.h
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Include/node.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Include/parsetok.h
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Include/pgenheaders.h
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Include/pyarena.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Include/pycore_pyarena.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Include/token.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:56:33.778288 typed_ast-1.5.5/ast27/Parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Parser/Python.asdl
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Parser/acceler.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Parser/asdl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    41795 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Parser/asdl_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Parser/bitset.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Parser/grammar.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Parser/grammar1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Parser/node.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Parser/parser.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Parser/parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Parser/parsetok.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26962 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Parser/spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52538 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Parser/tokenizer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-03 22:56:26.000000 typed_ast-1.5.5/ast27/Parser/tokenizer.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:56:33.778288 typed_ast-1.5.5/ast27/Python/
+-rw-r--r--   0 runner    (1001) docker     (123)   280357 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast27/Python/Python-ast.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast27/Python/asdl.c
+-rw-r--r--   0 runner    (1001) docker     (123)   118113 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast27/Python/ast.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45695 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast27/Python/graminit.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast27/Python/mystrtoul.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:56:33.774288 typed_ast-1.5.5/ast3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:56:33.778288 typed_ast-1.5.5/ast3/Custom/
+-rw-r--r--   0 runner    (1001) docker     (123)    10221 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Custom/typed_ast.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:56:33.778288 typed_ast-1.5.5/ast3/Grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Grammar/Grammar
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:56:33.782288 typed_ast-1.5.5/ast3/Include/
+-rw-r--r--   0 runner    (1001) docker     (123)    23443 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Include/Python-ast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Include/asdl.h
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Include/ast.h
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Include/bitset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Include/errcode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Include/graminit.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Include/grammar.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Include/node.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Include/parsetok.h
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Include/pgenheaders.h
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Include/pyarena.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Include/pycore_pyarena.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Include/token.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:56:33.782288 typed_ast-1.5.5/ast3/Parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Parser/Python.asdl
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Parser/acceler.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12881 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Parser/asdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45012 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Parser/asdl_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Parser/bitset.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Parser/grammar.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Parser/grammar1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Parser/node.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Parser/parser.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Parser/parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13272 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Parser/parsetok.c
+-rw-r--r--   0 runner    (1001) docker     (123)    58106 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Parser/tokenizer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Parser/tokenizer.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:56:33.782288 typed_ast-1.5.5/ast3/Python/
+-rw-r--r--   0 runner    (1001) docker     (123)   282113 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Python/Python-ast.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Python/asdl.c
+-rw-r--r--   0 runner    (1001) docker     (123)   175785 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Python/ast.c
+-rw-r--r--   0 runner    (1001) docker     (123)    48037 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/Python/graminit.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:56:33.782288 typed_ast-1.5.5/ast3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-07-03 22:56:27.000000 typed_ast-1.5.5/ast3/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 22:56:33.786288 typed_ast-1.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-03 22:56:27.000000 typed_ast-1.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:56:33.786288 typed_ast-1.5.5/typed_ast/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 22:56:27.000000 typed_ast-1.5.5/typed_ast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12630 2023-07-03 22:56:27.000000 typed_ast-1.5.5/typed_ast/ast27.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-07-03 22:56:27.000000 typed_ast-1.5.5/typed_ast/ast3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-07-03 22:56:27.000000 typed_ast-1.5.5/typed_ast/conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:56:33.786288 typed_ast-1.5.5/typed_ast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-03 22:56:33.000000 typed_ast-1.5.5/typed_ast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-03 22:56:33.000000 typed_ast-1.5.5/typed_ast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:56:33.000000 typed_ast-1.5.5/typed_ast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 22:56:33.000000 typed_ast-1.5.5/typed_ast.egg-info/top_level.txt
```

### Comparing `typed_ast-1.5.4/LICENSE` & `typed_ast-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/PKG-INFO` & `typed_ast-1.5.5/typed_ast.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 Metadata-Version: 2.1
-Name: typed_ast
-Version: 1.5.4
+Name: typed-ast
+Version: 1.5.5
 Summary: a fork of Python 2 and 3 ast modules with type comment support
 Home-page: https://github.com/python/typed_ast
 Author: David Fisher
 License: Apache License 2.0
 Platform: POSIX
 Platform: Windows
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 7 - Inactive
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Requires-Python: >=3.6
 License-File: LICENSE
 
+===========
+End of life
+===========
+
+This project is no longer maintained.
+
+Use the standard library `ast` module instead.
+See https://github.com/python/typed_ast/issues/179.
+
+===========
+Description
+===========
+
 `typed_ast` is a Python 3 package that provides a Python 2.7 and Python 3
 parser similar to the standard `ast` library.  Unlike `ast` below Python 3.8,
 the parsers in
 `typed_ast` include PEP 484 type comments and are independent of the version of
 Python under which they are run.  The `typed_ast` parsers produce the standard
 Python AST (plus type comments), and are both fast and correct, as they are
 based on the CPython 2.7 and 3.7 parsers.
```

### Comparing `typed_ast-1.5.4/README.md` & `typed_ast-1.5.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# End of life
+
+This project is no longer maintained.
+
+Use the standard library `ast` module instead.
+See https://github.com/python/typed_ast/issues/179.
+
 # Typed AST
 
 [![Build Status](https://travis-ci.org/python/typed_ast.svg?branch=master)](https://travis-ci.org/python/typed_ast)
 [![Chat at https://gitter.im/python/typed_ast](https://badges.gitter.im/python/typed_ast.svg)](https://gitter.im/python/typed_ast)
 
 `typed_ast` is a Python 3 package that provides a Python 2.7 and Python 3
 parser similar to the standard `ast` library.  Unlike `ast` up to Python 3.7, the parsers in
```

### Comparing `typed_ast-1.5.4/ast27/Custom/typed_ast.c` & `typed_ast-1.5.5/ast27/Custom/typed_ast.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Grammar/Grammar` & `typed_ast-1.5.5/ast27/Grammar/Grammar`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Include/Python-ast.h` & `typed_ast-1.5.5/ast27/Include/Python-ast.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Include/asdl.h` & `typed_ast-1.5.5/ast27/Include/asdl.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Include/bitset.h` & `typed_ast-1.5.5/ast27/Include/bitset.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Include/errcode.h` & `typed_ast-1.5.5/ast27/Include/errcode.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Include/graminit.h` & `typed_ast-1.5.5/ast27/Include/graminit.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Include/grammar.h` & `typed_ast-1.5.5/ast27/Include/grammar.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Include/node.h` & `typed_ast-1.5.5/ast27/Include/node.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Include/parsetok.h` & `typed_ast-1.5.5/ast27/Include/parsetok.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Include/pycore_pyarena.h` & `typed_ast-1.5.5/ast27/Include/pycore_pyarena.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Include/token.h` & `typed_ast-1.5.5/ast27/Include/token.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Parser/Python.asdl` & `typed_ast-1.5.5/ast27/Parser/Python.asdl`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Parser/acceler.c` & `typed_ast-1.5.5/ast27/Parser/acceler.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Parser/asdl.py` & `typed_ast-1.5.5/ast27/Parser/asdl.py`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Parser/asdl_c.py` & `typed_ast-1.5.5/ast27/Parser/asdl_c.py`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Parser/bitset.c` & `typed_ast-1.5.5/ast27/Parser/bitset.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Parser/grammar.c` & `typed_ast-1.5.5/ast27/Parser/grammar.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Parser/grammar1.c` & `typed_ast-1.5.5/ast27/Parser/grammar1.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Parser/node.c` & `typed_ast-1.5.5/ast27/Parser/node.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Parser/parser.c` & `typed_ast-1.5.5/ast27/Parser/parser.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Parser/parser.h` & `typed_ast-1.5.5/ast27/Parser/parser.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Parser/parsetok.c` & `typed_ast-1.5.5/ast27/Parser/parsetok.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Parser/spark.py` & `typed_ast-1.5.5/ast27/Parser/spark.py`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Parser/tokenizer.c` & `typed_ast-1.5.5/ast27/Parser/tokenizer.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Parser/tokenizer.h` & `typed_ast-1.5.5/ast27/Parser/tokenizer.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Python/Python-ast.c` & `typed_ast-1.5.5/ast27/Python/Python-ast.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Python/asdl.c` & `typed_ast-1.5.5/ast27/Python/asdl.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Python/ast.c` & `typed_ast-1.5.5/ast27/Python/ast.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Python/graminit.c` & `typed_ast-1.5.5/ast27/Python/graminit.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast27/Python/mystrtoul.c` & `typed_ast-1.5.5/ast27/Python/mystrtoul.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Custom/typed_ast.c` & `typed_ast-1.5.5/ast3/Custom/typed_ast.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Grammar/Grammar` & `typed_ast-1.5.5/ast3/Grammar/Grammar`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Include/Python-ast.h` & `typed_ast-1.5.5/ast3/Include/Python-ast.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Include/asdl.h` & `typed_ast-1.5.5/ast3/Include/asdl.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Include/ast.h` & `typed_ast-1.5.5/ast3/Include/ast.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Include/bitset.h` & `typed_ast-1.5.5/ast3/Include/bitset.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Include/errcode.h` & `typed_ast-1.5.5/ast3/Include/errcode.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Include/graminit.h` & `typed_ast-1.5.5/ast3/Include/graminit.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Include/grammar.h` & `typed_ast-1.5.5/ast3/Include/grammar.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Include/node.h` & `typed_ast-1.5.5/ast3/Include/node.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Include/parsetok.h` & `typed_ast-1.5.5/ast3/Include/parsetok.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Include/pycore_pyarena.h` & `typed_ast-1.5.5/ast3/Include/pycore_pyarena.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Include/token.h` & `typed_ast-1.5.5/ast3/Include/token.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Parser/Python.asdl` & `typed_ast-1.5.5/ast3/Parser/Python.asdl`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Parser/acceler.c` & `typed_ast-1.5.5/ast3/Parser/acceler.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Parser/asdl.py` & `typed_ast-1.5.5/ast3/Parser/asdl.py`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Parser/asdl_c.py` & `typed_ast-1.5.5/ast3/Parser/asdl_c.py`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Parser/bitset.c` & `typed_ast-1.5.5/ast3/Parser/bitset.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Parser/grammar.c` & `typed_ast-1.5.5/ast3/Parser/grammar.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Parser/grammar1.c` & `typed_ast-1.5.5/ast3/Parser/grammar1.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Parser/node.c` & `typed_ast-1.5.5/ast3/Parser/node.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Parser/parser.c` & `typed_ast-1.5.5/ast3/Parser/parser.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Parser/parser.h` & `typed_ast-1.5.5/ast3/Parser/parser.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Parser/parsetok.c` & `typed_ast-1.5.5/ast3/Parser/parsetok.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Parser/tokenizer.c` & `typed_ast-1.5.5/ast3/Parser/tokenizer.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Parser/tokenizer.h` & `typed_ast-1.5.5/ast3/Parser/tokenizer.h`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Python/Python-ast.c` & `typed_ast-1.5.5/ast3/Python/Python-ast.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Python/asdl.c` & `typed_ast-1.5.5/ast3/Python/asdl.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Python/ast.c` & `typed_ast-1.5.5/ast3/Python/ast.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/Python/graminit.c` & `typed_ast-1.5.5/ast3/Python/graminit.c`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/ast3/tests/test_basics.py` & `typed_ast-1.5.5/ast3/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/setup.py` & `typed_ast-1.5.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,27 @@
         'ast3/Include/Python-ast.h',
         'ast3/Include/token.h',
         'ast3/Parser/parser.h',
         'ast3/Parser/tokenizer.h',
     ])
 
 long_description = """
+===========
+End of life
+===========
+
+This project is no longer maintained.
+
+Use the standard library `ast` module instead.
+See https://github.com/python/typed_ast/issues/179.
+
+===========
+Description
+===========
+
 `typed_ast` is a Python 3 package that provides a Python 2.7 and Python 3
 parser similar to the standard `ast` library.  Unlike `ast` below Python 3.8,
 the parsers in
 `typed_ast` include PEP 484 type comments and are independent of the version of
 Python under which they are run.  The `typed_ast` parsers produce the standard
 Python AST (plus type comments), and are both fast and correct, as they are
 based on the CPython 2.7 and 3.7 parsers.
@@ -107,24 +120,25 @@
        description = 'a fork of Python 2 and 3 ast modules with type comment support',
        long_description = long_description,
        author = 'David Fisher',
        url = 'https://github.com/python/typed_ast',
        license='Apache License 2.0',
        platforms = ['POSIX', 'Windows'],
        classifiers = [
-           'Development Status :: 5 - Production/Stable',
+           'Development Status :: 7 - Inactive',
            'Environment :: Console',
            'Intended Audience :: Developers',
            'Operating System :: POSIX',
            'Operating System :: Microsoft',
            'Programming Language :: Python :: 3.6',
            'Programming Language :: Python :: 3.7',
            'Programming Language :: Python :: 3.8',
            'Programming Language :: Python :: 3.9',
            'Programming Language :: Python :: 3.10',
+           'Programming Language :: Python :: 3.11',
            'Topic :: Software Development',
        ],
        python_requires=">=3.6",
        packages = ['typed_ast', 'typed_ast.tests'],
        package_dir={ 'typed_ast.tests': 'ast3/tests' },
        ext_package='typed_ast',
        ext_modules = [_ast27, _ast3])
```

### Comparing `typed_ast-1.5.4/typed_ast/ast27.py` & `typed_ast-1.5.5/typed_ast/ast27.py`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/typed_ast/ast3.py` & `typed_ast-1.5.5/typed_ast/ast3.py`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/typed_ast/conversions.py` & `typed_ast-1.5.5/typed_ast/conversions.py`

 * *Files identical despite different names*

### Comparing `typed_ast-1.5.4/typed_ast.egg-info/PKG-INFO` & `typed_ast-1.5.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 Metadata-Version: 2.1
-Name: typed-ast
-Version: 1.5.4
+Name: typed_ast
+Version: 1.5.5
 Summary: a fork of Python 2 and 3 ast modules with type comment support
 Home-page: https://github.com/python/typed_ast
 Author: David Fisher
 License: Apache License 2.0
 Platform: POSIX
 Platform: Windows
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 7 - Inactive
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Requires-Python: >=3.6
 License-File: LICENSE
 
+===========
+End of life
+===========
+
+This project is no longer maintained.
+
+Use the standard library `ast` module instead.
+See https://github.com/python/typed_ast/issues/179.
+
+===========
+Description
+===========
+
 `typed_ast` is a Python 3 package that provides a Python 2.7 and Python 3
 parser similar to the standard `ast` library.  Unlike `ast` below Python 3.8,
 the parsers in
 `typed_ast` include PEP 484 type comments and are independent of the version of
 Python under which they are run.  The `typed_ast` parsers produce the standard
 Python AST (plus type comments), and are both fast and correct, as they are
 based on the CPython 2.7 and 3.7 parsers.
```

### Comparing `typed_ast-1.5.4/typed_ast.egg-info/SOURCES.txt` & `typed_ast-1.5.5/typed_ast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

