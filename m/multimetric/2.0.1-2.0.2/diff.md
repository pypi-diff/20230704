# Comparing `tmp/multimetric-2.0.1.tar.gz` & `tmp/multimetric-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimetric-2.0.1.tar", last modified: Mon Jul  3 14:17:11 2023, max compression
+gzip compressed data, was "multimetric-2.0.2.tar", last modified: Tue Jul  4 15:25:41 2023, max compression
```

## Comparing `multimetric-2.0.1.tar` & `multimetric-2.0.2.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:17:11.352872 multimetric-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-03 14:16:55.000000 multimetric-2.0.1/LICENSE.Zlib
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-03 14:16:55.000000 multimetric-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-07-03 14:17:11.352872 multimetric-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-07-03 14:16:55.000000 multimetric-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:17:11.348872 multimetric-2.0.1/multimetric/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:17:11.348872 multimetric-2.0.1/multimetric/cls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/base_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/base_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:17:11.348872 multimetric-2.0.1/multimetric/cls/calc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/calc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/calc/halstead.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/calc/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/calc/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/calc/tiobe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:17:11.348872 multimetric-2.0.1/multimetric/cls/importer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/importer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/importer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/importer/filtered.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:17:11.348872 multimetric-2.0.1/multimetric/cls/importer/mods/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/importer/mods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/importer/mods/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/importer/mods/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/importer/pick.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:17:11.348872 multimetric-2.0.1/multimetric/cls/metric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/metric/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/metric/cyclomatic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/metric/fanout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/metric/loc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/metric/operands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/metric/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:17:11.348872 multimetric-2.0.1/multimetric/cls/stats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/stats/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-03 14:16:55.000000 multimetric-2.0.1/multimetric/cls/tokentree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:17:11.348872 multimetric-2.0.1/multimetric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-07-03 14:17:11.000000 multimetric-2.0.1/multimetric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-03 14:17:11.000000 multimetric-2.0.1/multimetric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:17:11.000000 multimetric-2.0.1/multimetric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-03 14:17:11.000000 multimetric-2.0.1/multimetric.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 14:17:11.000000 multimetric-2.0.1/multimetric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 14:17:11.000000 multimetric-2.0.1/multimetric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 14:16:55.000000 multimetric-2.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-03 14:17:11.352872 multimetric-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-03 14:17:11.000000 multimetric-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:17:11.352872 multimetric-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_c.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_calc_halstead.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_calc_maintenance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_coffeescript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_cornercases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_cpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_csharp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_dart.py
--rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_go.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_groovy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_haskell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_import_cornercases.py
--rw-r--r--   0 runner    (1001) docker     (123)    14523 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_import_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_import_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_java.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_javascript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_julia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_kotlin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_lisp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_lua.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_objective_c.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_perl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_php.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_rust.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_tcl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_typescript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-03 14:16:55.000000 multimetric-2.0.1/tests/test_zig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:25:41.690904 multimetric-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-04 15:25:22.000000 multimetric-2.0.2/LICENSE.Zlib
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-04 15:25:22.000000 multimetric-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-07-04 15:25:41.690904 multimetric-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-07-04 15:25:22.000000 multimetric-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:25:41.674903 multimetric-2.0.2/multimetric/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:25:41.678903 multimetric-2.0.2/multimetric/cls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/base_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/base_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:25:41.678903 multimetric-2.0.2/multimetric/cls/calc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/calc/halstead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/calc/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/calc/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/calc/tiobe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:25:41.678903 multimetric-2.0.2/multimetric/cls/importer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/importer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/importer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/importer/filtered.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:25:41.678903 multimetric-2.0.2/multimetric/cls/importer/mods/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/importer/mods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/importer/mods/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/importer/mods/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/importer/pick.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:25:41.682904 multimetric-2.0.2/multimetric/cls/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/metric/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/metric/cyclomatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/metric/fanout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/metric/loc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/metric/operands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/metric/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:25:41.682904 multimetric-2.0.2/multimetric/cls/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/stats/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-04 15:25:22.000000 multimetric-2.0.2/multimetric/cls/tokentree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:25:41.678903 multimetric-2.0.2/multimetric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-07-04 15:25:41.000000 multimetric-2.0.2/multimetric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-04 15:25:41.000000 multimetric-2.0.2/multimetric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:25:41.000000 multimetric-2.0.2/multimetric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-04 15:25:41.000000 multimetric-2.0.2/multimetric.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-04 15:25:41.000000 multimetric-2.0.2/multimetric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 15:25:41.000000 multimetric-2.0.2/multimetric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-04 15:25:22.000000 multimetric-2.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-04 15:25:41.690904 multimetric-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-04 15:25:41.000000 multimetric-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:25:41.690904 multimetric-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_calc_halstead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_calc_maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_coffeescript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_cornercases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_csharp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_dart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_groovy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_haskell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_import_cornercases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14523 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_import_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_import_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_javascript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_julia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_kotlin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_lisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_lua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_objective_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_perl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_php.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_rust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_tcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_typescript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-04 15:25:22.000000 multimetric-2.0.2/tests/test_zig.py
```

### Comparing `multimetric-2.0.1/LICENSE.Zlib` & `multimetric-2.0.2/LICENSE.Zlib`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/PKG-INFO` & `multimetric-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimetric
-Version: 2.0.1
+Version: 2.0.2
 Summary: Calculate code metrics in various languages
 Home-page: https://github.com/priv-kweihmann/multimetric
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `multimetric-2.0.1/README.md` & `multimetric-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/multimetric/__main__.py` & `multimetric-2.0.2/multimetric/__main__.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/multimetric/cls/base.py` & `multimetric-2.0.2/multimetric/cls/base.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/multimetric/cls/calc/halstead.py` & `multimetric-2.0.2/multimetric/cls/calc/halstead.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/multimetric/cls/calc/maintenance.py` & `multimetric-2.0.2/multimetric/cls/calc/maintenance.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/multimetric/cls/calc/pylint.py` & `multimetric-2.0.2/multimetric/cls/calc/pylint.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/multimetric/cls/calc/tiobe.py` & `multimetric-2.0.2/multimetric/cls/calc/tiobe.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/multimetric/cls/importer/base.py` & `multimetric-2.0.2/multimetric/cls/importer/base.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/multimetric/cls/importer/mods/csv.py` & `multimetric-2.0.2/multimetric/cls/importer/mods/csv.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/multimetric/cls/importer/mods/json.py` & `multimetric-2.0.2/multimetric/cls/importer/mods/json.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/multimetric/cls/importer/pick.py` & `multimetric-2.0.2/multimetric/cls/importer/pick.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/multimetric/cls/metric/comments.py` & `multimetric-2.0.2/multimetric/cls/metric/comments.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/multimetric/cls/metric/cyclomatic.py` & `multimetric-2.0.2/multimetric/cls/metric/cyclomatic.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/multimetric/cls/metric/fanout.py` & `multimetric-2.0.2/multimetric/cls/metric/fanout.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/multimetric/cls/metric/loc.py` & `multimetric-2.0.2/multimetric/cls/metric/loc.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/multimetric/cls/metric/operands.py` & `multimetric-2.0.2/multimetric/cls/metric/operands.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/multimetric/cls/metric/operators.py` & `multimetric-2.0.2/multimetric/cls/metric/operators.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/multimetric/cls/modules.py` & `multimetric-2.0.2/multimetric/cls/modules.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/multimetric/cls/stats/stats.py` & `multimetric-2.0.2/multimetric/cls/stats/stats.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/multimetric/cls/tokentree.py` & `multimetric-2.0.2/multimetric/cls/tokentree.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/multimetric.egg-info/PKG-INFO` & `multimetric-2.0.2/multimetric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimetric
-Version: 2.0.1
+Version: 2.0.2
 Summary: Calculate code metrics in various languages
 Home-page: https://github.com/priv-kweihmann/multimetric
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `multimetric-2.0.1/multimetric.egg-info/SOURCES.txt` & `multimetric-2.0.2/multimetric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/setup.py` & `multimetric-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 requirements = []
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="multimetric",
-    version="2.0.1",
+    version="2.0.2",
     author="Konrad Weihmann",
     author_email="kweihmann@outlook.com",
     description="Calculate code metrics in various languages",
     long_description=_long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/priv-kweihmann/multimetric",
     packages=setuptools.find_packages(exclude='tests'),
```

### Comparing `multimetric-2.0.1/tests/conftest.py` & `multimetric-2.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_bash.py` & `multimetric-2.0.2/tests/test_bash.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_c.py` & `multimetric-2.0.2/tests/test_c.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_calc_halstead.py` & `multimetric-2.0.2/tests/test_calc_halstead.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_calc_maintenance.py` & `multimetric-2.0.2/tests/test_calc_maintenance.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_coffeescript.py` & `multimetric-2.0.2/tests/test_coffeescript.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_cornercases.py` & `multimetric-2.0.2/tests/test_cornercases.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_cpp.py` & `multimetric-2.0.2/tests/test_cpp.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_csharp.py` & `multimetric-2.0.2/tests/test_csharp.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_dart.py` & `multimetric-2.0.2/tests/test_dart.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_format.py` & `multimetric-2.0.2/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_go.py` & `multimetric-2.0.2/tests/test_go.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_groovy.py` & `multimetric-2.0.2/tests/test_groovy.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_haskell.py` & `multimetric-2.0.2/tests/test_haskell.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_import_cornercases.py` & `multimetric-2.0.2/tests/test_import_cornercases.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_import_csv.py` & `multimetric-2.0.2/tests/test_import_csv.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_import_json.py` & `multimetric-2.0.2/tests/test_import_json.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_integration.py` & `multimetric-2.0.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_java.py` & `multimetric-2.0.2/tests/test_java.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_javascript.py` & `multimetric-2.0.2/tests/test_javascript.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_julia.py` & `multimetric-2.0.2/tests/test_julia.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_kotlin.py` & `multimetric-2.0.2/tests/test_kotlin.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_lisp.py` & `multimetric-2.0.2/tests/test_lisp.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_lua.py` & `multimetric-2.0.2/tests/test_lua.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_objective_c.py` & `multimetric-2.0.2/tests/test_objective_c.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_perl.py` & `multimetric-2.0.2/tests/test_perl.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_php.py` & `multimetric-2.0.2/tests/test_php.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_python.py` & `multimetric-2.0.2/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_rust.py` & `multimetric-2.0.2/tests/test_rust.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_statistics.py` & `multimetric-2.0.2/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_tcl.py` & `multimetric-2.0.2/tests/test_tcl.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_typescript.py` & `multimetric-2.0.2/tests/test_typescript.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.1/tests/test_zig.py` & `multimetric-2.0.2/tests/test_zig.py`

 * *Files identical despite different names*

