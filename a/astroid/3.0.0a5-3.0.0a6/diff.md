# Comparing `tmp/astroid-3.0.0a5.tar.gz` & `tmp/astroid-3.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroid-3.0.0a5.tar", last modified: Tue Jun 13 07:54:08 2023, max compression
+gzip compressed data, was "astroid-3.0.0a6.tar", last modified: Tue Jul  4 20:09:59 2023, max compression
```

## Comparing `astroid-3.0.0a5.tar` & `astroid-3.0.0a6.tar`

### file list

```diff
@@ -1,151 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:54:08.648510 astroid-3.0.0a5/
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-06-13 07:53:44.000000 astroid-3.0.0a5/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-06-13 07:53:44.000000 astroid-3.0.0a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 07:53:44.000000 astroid-3.0.0a5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-13 07:54:08.648510 astroid-3.0.0a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-13 07:53:44.000000 astroid-3.0.0a5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:54:08.624509 astroid-3.0.0a5/astroid/
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/__pkginfo__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/_backport_stdlib_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/astroid_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    26966 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/bases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:54:08.640510 astroid-3.0.0a5/astroid/brain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)    35841 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_builtin_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_ctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_curses.py
--rw-r--r--   0 runner    (1001) docker     (123)    22150 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_dateutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_fstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_gi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_hashlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_mechanize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    23777 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_namedtuple_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_nose.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_numpy_core_einsumfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_numpy_core_fromnumeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_numpy_core_function_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_numpy_core_multiarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_numpy_core_numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_numpy_core_numerictypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_numpy_core_umath.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_numpy_ma.py
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_numpy_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_numpy_random_mtrand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_pkg_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_re.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_responses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2286 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_scipy_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_six.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_threading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    14690 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_unittest.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18824 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/filter_statements.py
--rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    45357 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/inference_tip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:54:08.640510 astroid-3.0.0a5/astroid/interpreter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/interpreter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:54:08.640510 astroid-3.0.0a5/astroid/interpreter/_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/interpreter/_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/interpreter/_import/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/interpreter/_import/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/interpreter/dunder_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    34584 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/interpreter/objectmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    18176 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    23616 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/modutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/node_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:54:08.640510 astroid-3.0.0a5/astroid/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/nodes/_base_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/nodes/as_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/nodes/const.py
--rw-r--r--   0 runner    (1001) docker     (123)   132674 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/nodes/node_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    28138 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/nodes/node_ng.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:54:08.644510 astroid-3.0.0a5/astroid/nodes/scoped_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/nodes/scoped_nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/nodes/scoped_nodes/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)   101119 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/nodes/scoped_nodes/scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/nodes/scoped_nodes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/nodes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    32620 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    25341 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/raw_building.py
--rw-r--r--   0 runner    (1001) docker     (123)    69315 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/rebuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:54:08.628509 astroid-3.0.0a5/astroid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-13 07:54:08.000000 astroid-3.0.0a5/astroid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-13 07:54:08.000000 astroid-3.0.0a5/astroid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:54:08.000000 astroid-3.0.0a5/astroid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 07:54:08.000000 astroid-3.0.0a5/astroid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 07:54:08.000000 astroid-3.0.0a5/astroid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-13 07:53:44.000000 astroid-3.0.0a5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-13 07:53:44.000000 astroid-3.0.0a5/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-13 07:53:44.000000 astroid-3.0.0a5/requirements_full.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-13 07:53:44.000000 astroid-3.0.0a5/requirements_minimal.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-13 07:54:08.648510 astroid-3.0.0a5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:54:08.648510 astroid-3.0.0a5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    34673 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15619 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_filter_statements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_group_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)   223086 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_inference_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)    34833 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    22658 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_modutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    62072 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    54462 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_nodes_lineno.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_nodes_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    27699 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_object_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_python3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_raw_building.py
--rw-r--r--   0 runner    (1001) docker     (123)    15110 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_regrtest.py
--rw-r--r--   0 runner    (1001) docker     (123)    92790 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_stdlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:59.811851 astroid-3.0.0a6/
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-07-04 20:09:38.000000 astroid-3.0.0a6/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-07-04 20:09:38.000000 astroid-3.0.0a6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 20:09:38.000000 astroid-3.0.0a6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-04 20:09:59.811851 astroid-3.0.0a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-04 20:09:38.000000 astroid-3.0.0a6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:59.795851 astroid-3.0.0a6/astroid/
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/__pkginfo__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/_backport_stdlib_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/astroid_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27153 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/bases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:59.803851 astroid-3.0.0a6/astroid/brain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37079 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_builtin_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_curses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22134 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_dateutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_fstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_gi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_hashlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_mechanize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23766 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_namedtuple_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_nose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_numpy_core_einsumfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_numpy_core_fromnumeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_numpy_core_function_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_numpy_core_multiarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_numpy_core_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_numpy_core_numerictypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_numpy_core_umath.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_numpy_ma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_numpy_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_numpy_random_mtrand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_pkg_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_responses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2286 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_scipy_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_six.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15608 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18802 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/filter_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11915 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/inference_tip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:59.803851 astroid-3.0.0a6/astroid/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/interpreter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:59.803851 astroid-3.0.0a6/astroid/interpreter/_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/interpreter/_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/interpreter/_import/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/interpreter/_import/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/interpreter/dunder_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34584 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/interpreter/objectmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18185 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23616 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/modutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/node_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:59.803851 astroid-3.0.0a6/astroid/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24111 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/nodes/_base_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25825 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/nodes/as_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/nodes/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)   167768 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/nodes/node_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27207 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/nodes/node_ng.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:59.807851 astroid-3.0.0a6/astroid/nodes/scoped_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/nodes/scoped_nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/nodes/scoped_nodes/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104648 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/nodes/scoped_nodes/scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/nodes/scoped_nodes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/nodes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31226 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25314 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/raw_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72666 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/rebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:59.795851 astroid-3.0.0a6/astroid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-04 20:09:59.000000 astroid-3.0.0a6/astroid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-04 20:09:59.000000 astroid-3.0.0a6/astroid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 20:09:59.000000 astroid-3.0.0a6/astroid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-04 20:09:59.000000 astroid-3.0.0a6/astroid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 20:09:59.000000 astroid-3.0.0a6/astroid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-04 20:09:38.000000 astroid-3.0.0a6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 20:09:38.000000 astroid-3.0.0a6/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-04 20:09:38.000000 astroid-3.0.0a6/requirements_full.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-04 20:09:38.000000 astroid-3.0.0a6/requirements_minimal.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-04 20:09:59.811851 astroid-3.0.0a6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:59.811851 astroid-3.0.0a6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34680 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15619 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_filter_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_group_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)   223536 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_inference_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34833 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19631 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22658 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_modutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63115 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55531 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_nodes_lineno.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_nodes_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27843 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_object_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14780 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_python3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_raw_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15110 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_regrtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93424 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_type_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tox.ini
```

### Comparing `astroid-3.0.0a5/CONTRIBUTORS.txt` & `astroid-3.0.0a6/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/LICENSE` & `astroid-3.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/PKG-INFO` & `astroid-3.0.0a6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroid
-Version: 3.0.0a5
+Version: 3.0.0a6
 Summary: An abstract syntax tree for Python with inference support.
 License: LGPL-2.1-or-later
 Project-URL: Docs, https://pylint.readthedocs.io/projects/astroid/en/latest/
 Project-URL: Source Code, https://github.com/pylint-dev/astroid
 Project-URL: Bug tracker, https://github.com/pylint-dev/astroid/issues
 Project-URL: Discord server, https://discord.gg/Egy6P8AMB5
 Keywords: static code analysis,python,abstract syntax tree
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
```

### Comparing `astroid-3.0.0a5/README.rst` & `astroid-3.0.0a6/README.rst`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/__init__.py` & `astroid-3.0.0a6/astroid/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 It mimics the class defined in the python's _ast module with some
 additional methods and attributes. New nodes instances are not fully
 compatible with python's _ast.
 
 Instance attributes are added by a
 builder object, which can either generate extended ast (let's call
 them astroid ;) by visiting an existent ast tree or by inspecting living
-object. Methods are added by monkey patching ast classes.
+object.
 
 Main modules are:
 
 * nodes and scoped_nodes for more information about methods and
   attributes added to different node classes
 
 * the manager contains a high level object to get astroid trees from
@@ -36,15 +36,15 @@
 
 # isort: off
 # We have an isort: off on '__version__' because of a circular import in nodes.
 from astroid.nodes import node_classes, scoped_nodes
 
 # isort: on
 
-from astroid import inference, raw_building
+from astroid import raw_building
 from astroid.__pkginfo__ import __version__, version
 from astroid.astroid_manager import MANAGER
 from astroid.bases import BaseInstance, BoundMethod, Instance, UnboundMethod
 from astroid.brain.helpers import register_module_extender
 from astroid.builder import extract_node, parse
 from astroid.const import BRAIN_MODULES_DIRECTORY, PY310_PLUS, Context
 from astroid.exceptions import (
@@ -53,31 +53,28 @@
     AstroidError,
     AstroidImportError,
     AstroidIndexError,
     AstroidSyntaxError,
     AstroidTypeError,
     AstroidValueError,
     AttributeInferenceError,
-    BinaryOperationError,
     DuplicateBasesError,
     InconsistentMroError,
     InferenceError,
     InferenceOverwriteError,
     MroError,
     NameInferenceError,
     NoDefault,
     NotFoundError,
-    OperationError,
     ParentMissingError,
     ResolveError,
     StatementMissing,
     SuperArgumentTypeError,
     SuperError,
     TooManyLevelsError,
-    UnaryOperationError,
     UnresolvableName,
     UseInferenceDefault,
 )
 from astroid.inference_tip import _inference_tip_cached, inference_tip
 from astroid.objects import ExceptionInstance
 
 # isort: off
```

### Comparing `astroid-3.0.0a5/astroid/_ast.py` & `astroid-3.0.0a6/astroid/_ast.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/_backport_stdlib_names.py` & `astroid-3.0.0a6/astroid/_backport_stdlib_names.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/arguments.py` & `astroid-3.0.0a6/astroid/arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 
 from __future__ import annotations
 
 from astroid import nodes
 from astroid.bases import Instance
 from astroid.context import CallContext, InferenceContext
 from astroid.exceptions import InferenceError, NoDefault
-from astroid.helpers import safe_infer
 from astroid.typing import InferenceResult
-from astroid.util import Uninferable, UninferableBase
+from astroid.util import Uninferable, UninferableBase, safe_infer
 
 
 class CallSite:
     """Class for understanding arguments passed into a call site.
 
     It needs a call context, which contains the arguments and the
     keyword arguments that were passed into a given call site.
@@ -82,16 +81,20 @@
         For instance, unpacking a dictionary with integer keys is invalid
         (**{1:2}), because the keys must be strings, which will make this
         method to return True. Other cases where this might return True if
         objects which can't be inferred were passed.
         """
         return len(self.keyword_arguments) != len(self._unpacked_kwargs)
 
-    def _unpack_keywords(self, keywords, context: InferenceContext | None = None):
-        values = {}
+    def _unpack_keywords(
+        self,
+        keywords: list[tuple[str | None, nodes.NodeNG]],
+        context: InferenceContext | None = None,
+    ):
+        values: dict[str | None, InferenceResult] = {}
         context = context or InferenceContext()
         context.extra_context = self.argument_context_map
         for name, value in keywords:
             if name is None:
                 # Then it's an unpacking operation (**)
                 inferred = safe_infer(value, context=context)
                 if not isinstance(inferred, nodes.Dict):
@@ -203,15 +206,15 @@
                 # context.boundnode is None when an instance method is called with
                 # the class, e.g. MyClass.method(obj, ...). In this case, self
                 # is the first argument.
                 if boundnode is None and funcnode.type == "method" and positional:
                     return positional[0].infer(context=context)
                 if boundnode is None:
                     # XXX can do better ?
-                    boundnode = funcnode.parent.frame(future=True)
+                    boundnode = funcnode.parent.frame()
 
                 if isinstance(boundnode, nodes.ClassDef):
                     # Verify that we're accessing a method
                     # of the metaclass through a class, as in
                     # `cls.metaclass_method`. In this case, the
                     # first argument is always the class.
                     method_scope = funcnode.parent.scope()
```

### Comparing `astroid-3.0.0a5/astroid/astroid_manager.py` & `astroid-3.0.0a6/astroid/astroid_manager.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/bases.py` & `astroid-3.0.0a6/astroid/bases.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 inference utils.
 """
 from __future__ import annotations
 
 import collections
 import collections.abc
 from collections.abc import Iterable, Iterator
-from typing import TYPE_CHECKING, Any, ClassVar, Literal
+from typing import TYPE_CHECKING, Any, Literal
 
-from astroid import nodes
+from astroid import decorators, nodes
 from astroid.const import PY310_PLUS
 from astroid.context import (
     CallContext,
     InferenceContext,
     bind_context_to_node,
     copy_context,
 )
@@ -24,20 +24,19 @@
     AstroidTypeError,
     AttributeInferenceError,
     InferenceError,
     NameInferenceError,
 )
 from astroid.interpreter import objectmodel
 from astroid.typing import (
-    InferBinaryOp,
     InferenceErrorInfo,
     InferenceResult,
     SuccessfulInferenceResult,
 )
-from astroid.util import Uninferable, UninferableBase
+from astroid.util import Uninferable, UninferableBase, safe_infer
 
 if TYPE_CHECKING:
     from astroid.constraint import Constraint
 
 
 PROPERTIES = {"builtins.property", "abc.abstractproperty"}
 if PY310_PLUS:
@@ -65,16 +64,14 @@
     "DynamicClassAttribute",
 }
 
 
 def _is_property(
     meth: nodes.FunctionDef | UnboundMethod, context: InferenceContext | None = None
 ) -> bool:
-    from astroid import helpers  # pylint: disable=import-outside-toplevel
-
     decoratornames = meth.decoratornames(context=context)
     if PROPERTIES.intersection(decoratornames):
         return True
     stripped = {
         name.split(".")[-1]
         for name in decoratornames
         if not isinstance(name, UninferableBase)
@@ -82,15 +79,15 @@
     if any(name in stripped for name in POSSIBLE_PROPERTIES):
         return True
 
     # Lookup for subclasses of *property*
     if not meth.decorators:
         return False
     for decorator in meth.decorators.nodes or ():
-        inferred = helpers.safe_infer(decorator, context=context)
+        inferred = safe_infer(decorator, context=context)
         if inferred is None or isinstance(inferred, UninferableBase):
             continue
         if isinstance(inferred, nodes.ClassDef):
             for base_class in inferred.bases:
                 if not isinstance(base_class, nodes.Name):
                     continue
                 module, _ = base_class.lookup(base_class.name)
@@ -145,15 +142,15 @@
     def infer(  # type: ignore[return]
         self, context: InferenceContext | None = None, **kwargs: Any
     ) -> collections.abc.Generator[InferenceResult, None, InferenceErrorInfo | None]:
         yield self
 
 
 def _infer_stmts(
-    stmts: Iterator[InferenceResult],
+    stmts: Iterable[InferenceResult],
     context: InferenceContext | None,
     frame: nodes.NodeNG | BaseInstance | None = None,
 ) -> collections.abc.Generator[InferenceResult, None, None]:
     """Return an iterator on statements inferred by each statement in *stmts*."""
     inferred = False
     constraint_failed = False
     if context is not None:
@@ -239,15 +236,15 @@
         return "Instance of"
 
     def getattr(
         self,
         name: str,
         context: InferenceContext | None = None,
         lookupclass: bool = True,
-    ) -> list[SuccessfulInferenceResult]:
+    ) -> list[InferenceResult]:
         try:
             values = self._proxied.instance_attr(name, context)
         except AttributeInferenceError as exc:
             if self.special_attributes and name in self.special_attributes:
                 return [self.special_attributes.lookup(name)]
 
             if lookupclass:
@@ -342,15 +339,24 @@
     """A special node representing a class instance."""
 
     special_attributes = objectmodel.InstanceModel()
 
     def __init__(self, proxied: nodes.ClassDef | None) -> None:
         super().__init__(proxied)
 
-    infer_binary_op: ClassVar[InferBinaryOp[Instance]]
+    @decorators.yes_if_nothing_inferred
+    def infer_binary_op(
+        self,
+        opnode: nodes.AugAssign | nodes.BinOp,
+        operator: str,
+        other: InferenceResult,
+        context: InferenceContext,
+        method: SuccessfulInferenceResult,
+    ) -> Generator[InferenceResult, None, None]:
+        return method.infer_call_result(self, context)
 
     def __repr__(self) -> str:
         return "<Instance of {}.{} at 0x{}>".format(
             self._proxied.root().name, self._proxied.name, id(self)
         )
 
     def __str__(self) -> str:
@@ -426,15 +432,15 @@
 
     special_attributes: objectmodel.BoundMethodModel | objectmodel.UnboundMethodModel = (
         objectmodel.UnboundMethodModel()
     )
 
     def __repr__(self) -> str:
         assert self._proxied.parent, "Expected a parent node"
-        frame = self._proxied.parent.frame(future=True)
+        frame = self._proxied.parent.frame()
         return "<{} {} of {} at 0x{}".format(
             self.__class__.__name__, self._proxied.name, frame.qname(), id(self)
         )
 
     def implicit_parameters(self) -> Literal[0, 1]:
         return 0
 
@@ -468,15 +474,15 @@
         to determine which class the method was called from
         """
 
         # If we're unbound method __new__ of a builtin, the result is an
         # instance of the class given as first argument.
         if self._proxied.name == "__new__":
             assert self._proxied.parent, "Expected a parent node"
-            qname = self._proxied.parent.frame(future=True).qname()
+            qname = self._proxied.parent.frame().qname()
             # Avoid checking builtins.type: _infer_type_new_call() does more validation
             if qname.startswith("builtins.") and qname != "builtins.type":
                 return self._infer_builtin_new(caller, context or InferenceContext())
         return self._proxied.infer_call_result(caller, context)
 
     def _infer_builtin_new(
         self,
```

### Comparing `astroid-3.0.0a5/astroid/brain/brain_argparse.py` & `astroid-3.0.0a6/astroid/brain/brain_argparse.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_attrs.py` & `astroid-3.0.0a6/astroid/brain/brain_attrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 """
 Astroid hook for the attrs library
 
 Without this hook pylint reports unsupported-assignment-operation
 for attrs classes
 """
-from astroid.helpers import safe_infer
 from astroid.manager import AstroidManager
 from astroid.nodes.node_classes import AnnAssign, Assign, AssignName, Call, Unknown
 from astroid.nodes.scoped_nodes import ClassDef
+from astroid.util import safe_infer
 
 ATTRIB_NAMES = frozenset(
     (
         "attr.Factory",
         "attr.ib",
         "attrib",
         "attr.attrib",
```

### Comparing `astroid-3.0.0a5/astroid/brain/brain_boto3.py` & `astroid-3.0.0a6/astroid/brain/brain_boto3.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_builtin_inference.py` & `astroid-3.0.0a6/astroid/brain/brain_builtin_inference.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,31 +3,59 @@
 # Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Astroid hooks for various builtins."""
 
 from __future__ import annotations
 
 import itertools
-from collections.abc import Callable, Iterable, Iterator
+from collections.abc import Callable, Iterable
 from functools import partial
-from typing import Any
+from typing import TYPE_CHECKING, Any, Iterator, NoReturn, Type, Union, cast
 
-from astroid import arguments, bases, helpers, inference_tip, nodes, objects, util
+from astroid import arguments, helpers, inference_tip, nodes, objects, util
 from astroid.builder import AstroidBuilder
 from astroid.context import InferenceContext
 from astroid.exceptions import (
     AstroidTypeError,
     AttributeInferenceError,
     InferenceError,
     MroError,
     UseInferenceDefault,
 )
 from astroid.manager import AstroidManager
 from astroid.nodes import scoped_nodes
-from astroid.typing import InferenceResult, SuccessfulInferenceResult
+from astroid.typing import (
+    ConstFactoryResult,
+    InferenceResult,
+    SuccessfulInferenceResult,
+)
+
+if TYPE_CHECKING:
+    from astroid.bases import Instance
+
+ContainerObjects = Union[
+    objects.FrozenSet,
+    objects.DictItems,
+    objects.DictKeys,
+    objects.DictValues,
+]
+
+BuiltContainers = Union[
+    Type[tuple],
+    Type[list],
+    Type[set],
+    Type[frozenset],
+]
+
+CopyResult = Union[
+    nodes.Dict,
+    nodes.List,
+    nodes.Set,
+    objects.FrozenSet,
+]
 
 OBJECT_DUNDER_NEW = "object.__new__"
 
 STR_CLASS = """
 class whatever(object):
     def join(self, iterable):
         return {rvalue}
@@ -105,14 +133,18 @@
     def center(self, width, fillchar=None):
         return {rvalue}
     def ljust(self, width, fillchar=None):
         return {rvalue}
 """
 
 
+def _use_default() -> NoReturn:  # pragma: no cover
+    raise UseInferenceDefault()
+
+
 def _extend_string_class(class_node, code, rvalue):
     """Function to extend builtin str/unicode class."""
     code = code.format(rvalue=rvalue)
     fake = AstroidBuilder(AstroidManager()).string_build(code)["whatever"]
     for method in fake.mymethods():
         method.parent = class_node
         method.lineno = None
@@ -171,15 +203,17 @@
 def register_builtin_transform(transform, builtin_name) -> None:
     """Register a new transform function for the given *builtin_name*.
 
     The transform function must accept two parameters, a node and
     an optional context.
     """
 
-    def _transform_wrapper(node, context: InferenceContext | None = None):
+    def _transform_wrapper(
+        node: nodes.Call, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Iterator:
         result = transform(node, context=context)
         if result:
             if not result.parent:
                 # Let the transformation function determine
                 # the parent for its result. Otherwise,
                 # we set it to be the node we transformed from.
                 result.parent = node
@@ -228,56 +262,60 @@
             raise UseInferenceDefault
         transformed = transform(inferred)
     if not transformed or isinstance(transformed, util.UninferableBase):
         raise UseInferenceDefault
     return transformed
 
 
-def _container_generic_transform(  # pylint: disable=inconsistent-return-statements
+def _container_generic_transform(
     arg: SuccessfulInferenceResult,
     context: InferenceContext | None,
     klass: type[nodes.BaseContainer],
-    iterables: tuple[type[nodes.NodeNG] | type[bases.Proxy], ...],
-    build_elts: type[Iterable[Any]],
+    iterables: tuple[type[nodes.BaseContainer] | type[ContainerObjects], ...],
+    build_elts: BuiltContainers,
 ) -> nodes.BaseContainer | None:
+    elts: Iterable | str | bytes
+
     if isinstance(arg, klass):
         return arg
     if isinstance(arg, iterables):
+        arg = cast(Union[nodes.BaseContainer, ContainerObjects], arg)
         if all(isinstance(elt, nodes.Const) for elt in arg.elts):
-            elts = [elt.value for elt in arg.elts]
+            elts = [cast(nodes.Const, elt).value for elt in arg.elts]
         else:
             # TODO: Does not handle deduplication for sets.
             elts = []
             for element in arg.elts:
                 if not element:
                     continue
-                inferred = helpers.safe_infer(element, context=context)
+                inferred = util.safe_infer(element, context=context)
                 if inferred:
                     evaluated_object = nodes.EvaluatedObject(
                         original=element, value=inferred
                     )
                     elts.append(evaluated_object)
     elif isinstance(arg, nodes.Dict):
         # Dicts need to have consts as strings already.
-        if not all(isinstance(elt[0], nodes.Const) for elt in arg.items):
-            raise UseInferenceDefault()
-        elts = [item[0].value for item in arg.items]
+        elts = [
+            item[0].value if isinstance(item[0], nodes.Const) else _use_default()
+            for item in arg.items
+        ]
     elif isinstance(arg, nodes.Const) and isinstance(arg.value, (str, bytes)):
         elts = arg.value
     else:
-        return
+        return None
     return klass.from_elements(elts=build_elts(elts))
 
 
 def _infer_builtin_container(
     node: nodes.Call,
     context: InferenceContext | None,
     klass: type[nodes.BaseContainer],
-    iterables: tuple[type[nodes.NodeNG] | type[bases.Proxy], ...],
-    build_elts: type[Iterable[Any]],
+    iterables: tuple[type[nodes.NodeNG] | type[ContainerObjects], ...],
+    build_elts: BuiltContainers,
 ) -> nodes.BaseContainer:
     transform_func = partial(
         _container_generic_transform,
         context=context,
         klass=klass,
         iterables=iterables,
         build_elts=build_elts,
@@ -376,14 +414,15 @@
     call = arguments.CallSite.from_call(node, context=context)
     if call.has_invalid_arguments() or call.has_invalid_keywords():
         raise UseInferenceDefault
 
     args = call.positional_arguments
     kwargs = list(call.keyword_arguments.items())
 
+    items: list[tuple[InferenceResult, InferenceResult]]
     if not args and not kwargs:
         # dict()
         return nodes.Dict(
             lineno=node.lineno,
             col_offset=node.col_offset,
             parent=node.parent,
             end_lineno=node.end_lineno,
@@ -647,15 +686,15 @@
 
 def infer_slice(node, context: InferenceContext | None = None):
     """Understand `slice` calls."""
     args = node.args
     if not 0 < len(args) <= 3:
         raise UseInferenceDefault
 
-    infer_func = partial(helpers.safe_infer, context=context)
+    infer_func = partial(util.safe_infer, context=context)
     args = [infer_func(arg) for arg in args]
     for arg in args:
         if not arg or isinstance(arg, util.UninferableBase):
             raise UseInferenceDefault
         if not isinstance(arg, nodes.Const):
             raise UseInferenceDefault
         if not isinstance(arg.value, (type(None), int)):
@@ -672,15 +711,17 @@
         end_lineno=node.end_lineno,
         end_col_offset=node.end_col_offset,
     )
     slice_node.postinit(*args)
     return slice_node
 
 
-def _infer_object__new__decorator(node, context: InferenceContext | None = None):
+def _infer_object__new__decorator(
+    node: nodes.ClassDef, context: InferenceContext | None = None, **kwargs: Any
+) -> Iterator[Instance]:
     # Instantiate class immediately
     # since that's what @object.__new__ does
     return iter((node.instantiate_class(),))
 
 
 def _infer_object__new__decorator_check(node) -> bool:
     """Predicate before inference_tip.
@@ -921,18 +962,18 @@
                 return _build_dict_with_elements([])
 
         elements_with_value = [(element, default) for element in elements]
         return _build_dict_with_elements(elements_with_value)
     if isinstance(inferred_values, nodes.Const) and isinstance(
         inferred_values.value, (str, bytes)
     ):
-        elements = [
+        elements_with_value = [
             (nodes.Const(element), default) for element in inferred_values.value
         ]
-        return _build_dict_with_elements(elements)
+        return _build_dict_with_elements(elements_with_value)
     if isinstance(inferred_values, nodes.Dict):
         keys = inferred_values.itered()
         for key in keys:
             if not isinstance(key, accepted_iterable_elements):
                 # Fallback to an empty dict
                 return _build_dict_with_elements([])
 
@@ -940,70 +981,81 @@
         return _build_dict_with_elements(elements_with_value)
 
     # Fallback to an empty dictionary
     return _build_dict_with_elements([])
 
 
 def _infer_copy_method(
-    node: nodes.Call, context: InferenceContext | None = None
-) -> Iterator[nodes.NodeNG]:
+    node: nodes.Call, context: InferenceContext | None = None, **kwargs: Any
+) -> Iterator[CopyResult]:
     assert isinstance(node.func, nodes.Attribute)
     inferred_orig, inferred_copy = itertools.tee(node.func.expr.infer(context=context))
     if all(
         isinstance(
             inferred_node, (nodes.Dict, nodes.List, nodes.Set, objects.FrozenSet)
         )
         for inferred_node in inferred_orig
     ):
-        return inferred_copy
+        return cast(Iterator[CopyResult], inferred_copy)
 
-    raise UseInferenceDefault()
+    raise UseInferenceDefault
 
 
 def _is_str_format_call(node: nodes.Call) -> bool:
     """Catch calls to str.format()."""
     if not isinstance(node.func, nodes.Attribute) or not node.func.attrname == "format":
         return False
 
     if isinstance(node.func.expr, nodes.Name):
-        value = helpers.safe_infer(node.func.expr)
+        value = util.safe_infer(node.func.expr)
     else:
         value = node.func.expr
 
     return isinstance(value, nodes.Const) and isinstance(value.value, str)
 
 
 def _infer_str_format_call(
-    node: nodes.Call, context: InferenceContext | None = None
-) -> Iterator[nodes.Const | util.UninferableBase]:
+    node: nodes.Call, context: InferenceContext | None = None, **kwargs: Any
+) -> Iterator[ConstFactoryResult | util.UninferableBase]:
     """Return a Const node based on the template and passed arguments."""
     call = arguments.CallSite.from_call(node, context=context)
+    assert isinstance(node.func, (nodes.Attribute, nodes.AssignAttr, nodes.DelAttr))
+
+    value: nodes.Const
     if isinstance(node.func.expr, nodes.Name):
-        value: nodes.Const | None = helpers.safe_infer(node.func.expr)
-        if value is None:
+        if not (inferred := util.safe_infer(node.func.expr)) or not isinstance(
+            inferred, nodes.Const
+        ):
             return iter([util.Uninferable])
-    else:
+        value = inferred
+    elif isinstance(node.func.expr, nodes.Const):
         value = node.func.expr
+    else:  # pragma: no cover
+        return iter([util.Uninferable])
 
     format_template = value.value
 
     # Get the positional arguments passed
-    inferred_positional = [
-        helpers.safe_infer(i, context) for i in call.positional_arguments
-    ]
-    if not all(isinstance(i, nodes.Const) for i in inferred_positional):
-        return iter([util.Uninferable])
+    inferred_positional: list[nodes.Const] = []
+    for i in call.positional_arguments:
+        one_inferred = util.safe_infer(i, context)
+        if not isinstance(one_inferred, nodes.Const):
+            return iter([util.Uninferable])
+        inferred_positional.append(one_inferred)
+
     pos_values: list[str] = [i.value for i in inferred_positional]
 
     # Get the keyword arguments passed
-    inferred_keyword = {
-        k: helpers.safe_infer(v, context) for k, v in call.keyword_arguments.items()
-    }
-    if not all(isinstance(i, nodes.Const) for i in inferred_keyword.values()):
-        return iter([util.Uninferable])
+    inferred_keyword: dict[str, nodes.Const] = {}
+    for k, v in call.keyword_arguments.items():
+        one_inferred = util.safe_infer(v, context)
+        if not isinstance(one_inferred, nodes.Const):
+            return iter([util.Uninferable])
+        inferred_keyword[k] = one_inferred
+
     keyword_values: dict[str, str] = {k: v.value for k, v in inferred_keyword.items()}
 
     try:
         formatted_string = format_template.format(*pos_values, **keyword_values)
     except (AttributeError, IndexError, KeyError, TypeError, ValueError):
         # AttributeError: named field in format string was not found in the arguments
         # IndexError: there are too few arguments to interpolate
@@ -1047,9 +1099,11 @@
     nodes.Call,
     inference_tip(_infer_copy_method),
     lambda node: isinstance(node.func, nodes.Attribute)
     and node.func.attrname == "copy",
 )
 
 AstroidManager().register_transform(
-    nodes.Call, inference_tip(_infer_str_format_call), _is_str_format_call
+    nodes.Call,
+    inference_tip(_infer_str_format_call),
+    _is_str_format_call,
 )
```

### Comparing `astroid-3.0.0a5/astroid/brain/brain_collections.py` & `astroid-3.0.0a6/astroid/brain/brain_collections.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_crypt.py` & `astroid-3.0.0a6/astroid/brain/brain_crypt.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_ctypes.py` & `astroid-3.0.0a6/astroid/brain/brain_ctypes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_curses.py` & `astroid-3.0.0a6/astroid/brain/brain_curses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_dataclasses.py` & `astroid-3.0.0a6/astroid/brain/brain_dataclasses.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 """
 
 from __future__ import annotations
 
 from collections.abc import Iterator
 from typing import Literal, Tuple, Union
 
-from astroid import bases, context, helpers, nodes
+from astroid import bases, context, nodes
 from astroid.builder import parse
 from astroid.const import PY39_PLUS, PY310_PLUS
 from astroid.exceptions import AstroidSyntaxError, InferenceError, UseInferenceDefault
 from astroid.inference_tip import inference_tip
 from astroid.manager import AstroidManager
 from astroid.typing import InferenceResult
-from astroid.util import Uninferable, UninferableBase
+from astroid.util import Uninferable, UninferableBase, safe_infer
 
 _FieldDefaultReturn = Union[
     None,
     Tuple[Literal["default"], nodes.NodeNG],
     Tuple[Literal["default_factory"], nodes.Call],
 ]
 
@@ -478,15 +478,15 @@
 ) -> bool:
     """Return True if node is calling dataclasses field or Field
     from an AnnAssign statement directly in the body of a ClassDef.
 
     If check_scope is False, skips checking the statement and body.
     """
     if check_scope:
-        stmt = node.statement(future=True)
+        stmt = node.statement()
         scope = stmt.scope()
         if not (
             isinstance(stmt, nodes.AnnAssign)
             and stmt.value is not None
             and isinstance(scope, nodes.ClassDef)
             and is_decorated_with_dataclass(scope)
         ):
@@ -557,15 +557,15 @@
     )
 
 
 def _is_keyword_only_sentinel(node: nodes.NodeNG) -> bool:
     """Return True if node is the KW_ONLY sentinel."""
     if not PY310_PLUS:
         return False
-    inferred = helpers.safe_infer(node)
+    inferred = safe_infer(node)
     return (
         isinstance(inferred, bases.Instance)
         and inferred.qname() == "dataclasses._KW_ONLY_TYPE"
     )
 
 
 def _is_init_var(node: nodes.NodeNG) -> bool:
```

### Comparing `astroid-3.0.0a5/astroid/brain/brain_dateutil.py` & `astroid-3.0.0a6/astroid/brain/brain_dateutil.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_fstrings.py` & `astroid-3.0.0a6/astroid/brain/brain_fstrings.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_functools.py` & `astroid-3.0.0a6/astroid/brain/brain_functools.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 
 from __future__ import annotations
 
 from collections.abc import Iterator
 from functools import partial
 from itertools import chain
 
-from astroid import BoundMethod, arguments, extract_node, helpers, nodes, objects
+from astroid import BoundMethod, arguments, extract_node, nodes, objects
 from astroid.context import InferenceContext
 from astroid.exceptions import InferenceError, UseInferenceDefault
 from astroid.inference_tip import inference_tip
 from astroid.interpreter import objectmodel
 from astroid.manager import AstroidManager
 from astroid.nodes.node_classes import AssignName, Attribute, Call, Name
 from astroid.nodes.scoped_nodes import FunctionDef
 from astroid.typing import InferenceResult, SuccessfulInferenceResult
-from astroid.util import UninferableBase
+from astroid.util import UninferableBase, safe_infer
 
 LRU_CACHE = "functools.lru_cache"
 
 
 class LruWrappedModel(objectmodel.FunctionModel):
     """Special attribute model for functions decorated with functools.lru_cache.
 
@@ -46,15 +46,15 @@
 
         class CacheInfoBoundMethod(BoundMethod):
             def infer_call_result(
                 self,
                 caller: SuccessfulInferenceResult | None,
                 context: InferenceContext | None = None,
             ) -> Iterator[InferenceResult]:
-                res = helpers.safe_infer(cache_info)
+                res = safe_infer(cache_info)
                 assert res is not None
                 yield res
 
         return CacheInfoBoundMethod(proxy=self._instance, bound=self._instance)
 
     @property
     def attr_cache_clear(self):
```

### Comparing `astroid-3.0.0a5/astroid/brain/brain_gi.py` & `astroid-3.0.0a6/astroid/brain/brain_gi.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_hashlib.py` & `astroid-3.0.0a6/astroid/brain/brain_hashlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_http.py` & `astroid-3.0.0a6/astroid/brain/brain_http.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_hypothesis.py` & `astroid-3.0.0a6/astroid/brain/brain_hypothesis.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_io.py` & `astroid-3.0.0a6/astroid/brain/brain_io.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_mechanize.py` & `astroid-3.0.0a6/astroid/brain/brain_mechanize.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_multiprocessing.py` & `astroid-3.0.0a6/astroid/brain/brain_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_namedtuple_enum.py` & `astroid-3.0.0a6/astroid/brain/brain_namedtuple_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,15 +402,15 @@
             break
         dunder_members = {}
         target_names = set()
         for local, values in node.locals.items():
             if any(not isinstance(value, nodes.AssignName) for value in values):
                 continue
 
-            stmt = values[0].statement(future=True)
+            stmt = values[0].statement()
             if isinstance(stmt, nodes.Assign):
                 if isinstance(stmt.targets[0], nodes.Tuple):
                     targets = stmt.targets[0].itered()
                 else:
                     targets = stmt.targets
             elif isinstance(stmt, nodes.AnnAssign):
                 targets = [stmt.target]
```

### Comparing `astroid-3.0.0a5/astroid/brain/brain_nose.py` & `astroid-3.0.0a6/astroid/brain/brain_nose.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_numpy_core_einsumfunc.py` & `astroid-3.0.0a6/astroid/brain/brain_numpy_core_einsumfunc.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_numpy_core_fromnumeric.py` & `astroid-3.0.0a6/astroid/brain/brain_numpy_core_fromnumeric.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_numpy_core_function_base.py` & `astroid-3.0.0a6/astroid/brain/brain_numpy_core_function_base.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_numpy_core_multiarray.py` & `astroid-3.0.0a6/astroid/brain/brain_numpy_core_multiarray.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_numpy_core_numeric.py` & `astroid-3.0.0a6/astroid/brain/brain_numpy_core_numeric.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_numpy_core_numerictypes.py` & `astroid-3.0.0a6/astroid/brain/brain_numpy_core_numerictypes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_numpy_core_umath.py` & `astroid-3.0.0a6/astroid/brain/brain_numpy_core_umath.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_numpy_ma.py` & `astroid-3.0.0a6/astroid/brain/brain_numpy_ma.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_numpy_ndarray.py` & `astroid-3.0.0a6/astroid/brain/brain_numpy_ndarray.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_numpy_random_mtrand.py` & `astroid-3.0.0a6/astroid/brain/brain_numpy_random_mtrand.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_numpy_utils.py` & `astroid-3.0.0a6/astroid/brain/brain_numpy_utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_pathlib.py` & `astroid-3.0.0a6/astroid/brain/brain_pathlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_pkg_resources.py` & `astroid-3.0.0a6/astroid/brain/brain_pkg_resources.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_pytest.py` & `astroid-3.0.0a6/astroid/brain/brain_pytest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_qt.py` & `astroid-3.0.0a6/astroid/brain/brain_qt.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_random.py` & `astroid-3.0.0a6/astroid/brain/brain_random.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 # For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
 # Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 from __future__ import annotations
 
 import random
 
-from astroid import helpers
 from astroid.context import InferenceContext
 from astroid.exceptions import UseInferenceDefault
 from astroid.inference_tip import inference_tip
 from astroid.manager import AstroidManager
 from astroid.nodes.node_classes import (
     Attribute,
     Call,
     Const,
     EvaluatedObject,
     List,
     Name,
     Set,
     Tuple,
 )
+from astroid.util import safe_infer
 
 ACCEPTED_ITERABLES_FOR_SAMPLE = (List, Set, Tuple)
 
 
 def _clone_node_with_lineno(node, parent, lineno):
     if isinstance(node, EvaluatedObject):
         node = node.original
@@ -47,21 +47,21 @@
     return new_node
 
 
 def infer_random_sample(node, context: InferenceContext | None = None):
     if len(node.args) != 2:
         raise UseInferenceDefault
 
-    inferred_length = helpers.safe_infer(node.args[1], context=context)
+    inferred_length = safe_infer(node.args[1], context=context)
     if not isinstance(inferred_length, Const):
         raise UseInferenceDefault
     if not isinstance(inferred_length.value, int):
         raise UseInferenceDefault
 
-    inferred_sequence = helpers.safe_infer(node.args[0], context=context)
+    inferred_sequence = safe_infer(node.args[0], context=context)
     if not inferred_sequence:
         raise UseInferenceDefault
 
     if not isinstance(inferred_sequence, ACCEPTED_ITERABLES_FOR_SAMPLE):
         raise UseInferenceDefault
 
     if inferred_length.value > len(inferred_sequence.elts):
```

### Comparing `astroid-3.0.0a5/astroid/brain/brain_re.py` & `astroid-3.0.0a6/astroid/brain/brain_re.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_regex.py` & `astroid-3.0.0a6/astroid/brain/brain_regex.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_responses.py` & `astroid-3.0.0a6/astroid/brain/brain_responses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_scipy_signal.py` & `astroid-3.0.0a6/astroid/brain/brain_scipy_signal.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_signal.py` & `astroid-3.0.0a6/astroid/brain/brain_signal.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_six.py` & `astroid-3.0.0a6/astroid/brain/brain_six.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_sqlalchemy.py` & `astroid-3.0.0a6/astroid/brain/brain_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_ssl.py` & `astroid-3.0.0a6/astroid/brain/brain_ssl.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_subprocess.py` & `astroid-3.0.0a6/astroid/brain/brain_subprocess.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_threading.py` & `astroid-3.0.0a6/astroid/brain/brain_threading.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_type.py` & `astroid-3.0.0a6/astroid/brain/brain_type.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_typing.py` & `astroid-3.0.0a6/astroid/brain/brain_typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 # For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
 # Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Astroid hooks for typing.py support."""
 
 from __future__ import annotations
 
+import textwrap
 import typing
 from collections.abc import Iterator
 from functools import partial
 from typing import Final
 
 from astroid import context, extract_node, inference_tip
-from astroid.builder import _extract_single_node
-from astroid.const import PY39_PLUS
+from astroid.brain.helpers import register_module_extender
+from astroid.builder import AstroidBuilder, _extract_single_node
+from astroid.const import PY39_PLUS, PY312_PLUS
 from astroid.exceptions import (
     AttributeInferenceError,
     InferenceError,
     UseInferenceDefault,
 )
 from astroid.manager import AstroidManager
 from astroid.nodes.node_classes import (
@@ -227,15 +229,16 @@
 
     MutableSet = _alias(collections.abc.MutableSet, T)
 
     :param node: call node
     """
     return (
         isinstance(node.func, Name)
-        and node.func.name == "_alias"
+        # TODO: remove _DeprecatedGenericAlias when Py3.14 min
+        and node.func.name in {"_alias", "_DeprecatedGenericAlias"}
         and (
             # _alias function works also for builtins object such as list and dict
             isinstance(node.args[0], (Attribute, Name))
         )
     )
 
 
@@ -269,14 +272,16 @@
     """
     Infers the call to _alias function
     Insert ClassDef, with same name as aliased class,
     in mro to simulate _GenericAlias.
 
     :param node: call node
     :param context: inference context
+
+    # TODO: evaluate if still necessary when Py3.12 is minimum
     """
     if (
         not isinstance(node.parent, Assign)
         or not len(node.parent.targets) == 1
         or not isinstance(node.parent.targets[0], AssignName)
     ):
         raise UseInferenceDefault
@@ -411,14 +416,37 @@
         or len(node.args) != 2
     ):
         raise UseInferenceDefault
 
     return node.args[1].infer(context=ctx)
 
 
+def _typing_transform():
+    return AstroidBuilder(AstroidManager()).string_build(
+        textwrap.dedent(
+            """
+    class Generic:
+        @classmethod
+        def __class_getitem__(cls, item):  return cls
+    class ParamSpec: ...
+    class ParamSpecArgs: ...
+    class ParamSpecKwargs: ...
+    class TypeAlias: ...
+    class Type:
+        @classmethod
+        def __class_getitem__(cls, item):  return cls
+    class TypeVar:
+        @classmethod
+        def __class_getitem__(cls, item):  return cls
+    class TypeVarTuple: ...
+    """
+        )
+    )
+
+
 AstroidManager().register_transform(
     Call,
     inference_tip(infer_typing_typevar_or_newtype),
     looks_like_typing_typevar_or_newtype,
 )
 AstroidManager().register_transform(
     Subscript, inference_tip(infer_typing_attr), _looks_like_typing_subscript
@@ -438,7 +466,10 @@
 
 AstroidManager().register_transform(
     Call, inference_tip(infer_typing_alias), _looks_like_typing_alias
 )
 AstroidManager().register_transform(
     Call, inference_tip(infer_special_alias), _looks_like_special_alias
 )
+
+if PY312_PLUS:
+    register_module_extender(AstroidManager(), "typing", _typing_transform)
```

### Comparing `astroid-3.0.0a5/astroid/brain/brain_unittest.py` & `astroid-3.0.0a6/astroid/brain/brain_unittest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/brain_uuid.py` & `astroid-3.0.0a6/astroid/brain/brain_uuid.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/brain/helpers.py` & `astroid-3.0.0a6/astroid/brain/helpers.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/builder.py` & `astroid-3.0.0a6/astroid/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,15 @@
         """Visit a AssAttr node.
 
         This adds name to locals and handle members definition.
         """
         from astroid import objects  # pylint: disable=import-outside-toplevel
 
         try:
-            frame = node.frame(future=True)
+            frame = node.frame()
             for inferred in node.expr.infer():
                 if isinstance(inferred, util.UninferableBase):
                     continue
                 try:
                     # pylint: disable=unidiomatic-typecheck # We want a narrow check on the
                     # parent type, not all of its subclasses
                     if (
@@ -264,15 +264,15 @@
                 values = iattrs.setdefault(node.attrname, [])
                 if node in values:
                     continue
                 # get assign in __init__ first XXX useful ?
                 if (
                     frame.name == "__init__"
                     and values
-                    and values[0].frame(future=True).name != "__init__"
+                    and values[0].frame().name != "__init__"
                 ):
                     values.insert(0, node)
                 else:
                     values.append(node)
         except InferenceError:
             pass
```

### Comparing `astroid-3.0.0a5/astroid/const.py` & `astroid-3.0.0a6/astroid/const.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import sys
 from pathlib import Path
 
 PY38 = sys.version_info[:2] == (3, 8)
 PY39_PLUS = sys.version_info >= (3, 9)
 PY310_PLUS = sys.version_info >= (3, 10)
 PY311_PLUS = sys.version_info >= (3, 11)
+PY312_PLUS = sys.version_info >= (3, 12)
 
 WIN32 = sys.platform == "win32"
 
 IS_PYPY = sys.implementation.name == "pypy"
 IS_JYTHON = sys.implementation.name == "jython"
 
 # pylint: disable-next=no-member
```

### Comparing `astroid-3.0.0a5/astroid/constraint.py` & `astroid-3.0.0a6/astroid/constraint.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 
 """Classes representing different types of constraints on inference values."""
 from __future__ import annotations
 
 import sys
 from abc import ABC, abstractmethod
 from collections.abc import Iterator
-from typing import Union
+from typing import TYPE_CHECKING, Union
 
-from astroid import bases, nodes, util
+from astroid import nodes, util
 from astroid.typing import InferenceResult
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
+if TYPE_CHECKING:
+    from astroid import bases
+
 _NameNodes = Union[nodes.AssignAttr, nodes.Attribute, nodes.AssignName, nodes.Name]
 
 
 class Constraint(ABC):
     """Represents a single constraint on a variable."""
 
     def __init__(self, node: nodes.NodeNG, negate: bool) -> None:
```

### Comparing `astroid-3.0.0a5/astroid/context.py` & `astroid-3.0.0a6/astroid/context.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/decorators.py` & `astroid-3.0.0a6/astroid/decorators.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/exceptions.py` & `astroid-3.0.0a6/astroid/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 # For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
 # Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """This module contains exceptions used in the astroid library."""
 
 from __future__ import annotations
 
-from collections.abc import Iterator
+from collections.abc import Iterable, Iterator
 from typing import TYPE_CHECKING, Any
 
-from astroid import util
 from astroid.typing import InferenceResult, SuccessfulInferenceResult
 
 if TYPE_CHECKING:
     from astroid import arguments, bases, nodes, objects
     from astroid.context import InferenceContext
 
 __all__ = (
@@ -22,31 +21,28 @@
     "AstroidError",
     "AstroidImportError",
     "AstroidIndexError",
     "AstroidSyntaxError",
     "AstroidTypeError",
     "AstroidValueError",
     "AttributeInferenceError",
-    "BinaryOperationError",
     "DuplicateBasesError",
     "InconsistentMroError",
     "InferenceError",
     "InferenceOverwriteError",
     "MroError",
     "NameInferenceError",
     "NoDefault",
     "NotFoundError",
-    "OperationError",
     "ParentMissingError",
     "ResolveError",
     "StatementMissing",
     "SuperArgumentTypeError",
     "SuperError",
     "TooManyLevelsError",
-    "UnaryOperationError",
     "UnresolvableName",
     "UseInferenceDefault",
 )
 
 
 class AstroidError(Exception):
     """Base exception class for all astroid related exceptions.
@@ -184,15 +180,15 @@
         cls: ClassDef node whose MRO resolution failed.
         context: InferenceContext object.
     """
 
     def __init__(
         self,
         message: str,
-        mros: list[nodes.ClassDef],
+        mros: Iterable[Iterable[nodes.ClassDef]],
         cls: nodes.ClassDef,
         context: InferenceContext | None = None,
         **kws: Any,
     ) -> None:
         self.mros = mros
         self.cls = cls
         self.context = context
@@ -412,16 +408,11 @@
 
     def __init__(self, target: nodes.NodeNG) -> None:
         super(ParentMissingError, self).__init__(
             message=f"Statement not found on {target!r}"
         )
 
 
-# Backwards-compatibility aliases
-OperationError = util.BadOperationMessage
-UnaryOperationError = util.BadUnaryOperationMessage
-BinaryOperationError = util.BadBinaryOperationMessage
-
 SuperArgumentTypeError = SuperError
 UnresolvableName = NameInferenceError
 NotFoundError = AttributeInferenceError
 AstroidBuildingException = AstroidBuildingError
```

### Comparing `astroid-3.0.0a5/astroid/filter_statements.py` & `astroid-3.0.0a6/astroid/filter_statements.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,27 @@
 
 This method gets used in LocalsDictnodes.NodeNG._scope_lookup.
 It is not considered public.
 """
 
 from __future__ import annotations
 
+from typing import TYPE_CHECKING
+
 from astroid import nodes
-from astroid.nodes import node_classes
 from astroid.typing import SuccessfulInferenceResult
 
+if TYPE_CHECKING:
+    from astroid.nodes import _base_nodes
+
 
 def _get_filtered_node_statements(
     base_node: nodes.NodeNG, stmt_nodes: list[nodes.NodeNG]
 ) -> list[tuple[nodes.NodeNG, nodes.Statement]]:
-    statements = [(node, node.statement(future=True)) for node in stmt_nodes]
+    statements = [(node, node.statement()) for node in stmt_nodes]
     # Next we check if we have ExceptHandlers that are parent
     # of the underlying variable, in which case the last one survives
     if len(statements) > 1 and all(
         isinstance(stmt, nodes.ExceptHandler) for _, stmt in statements
     ):
         statements = [
             (node, stmt) for node, stmt in statements if stmt.parent_of(base_node)
@@ -40,15 +44,15 @@
     for parent in node.node_ancestors():
         if isinstance(parent, nodes.If):
             return parent
     return None
 
 
 def _filter_stmts(
-    base_node: node_classes.LookupMixIn,
+    base_node: _base_nodes.LookupMixIn,
     stmts: list[SuccessfulInferenceResult],
     frame: nodes.LocalsDictNodeNG,
     offset: int,
 ) -> list[nodes.NodeNG]:
     """Filter the given list of statements to remove ignorable statements.
 
     If base_node is not a frame itself and the name is found in the inner
@@ -79,24 +83,20 @@
         # For more information why this is important,
         # see Pylint issue #295.
         # For example, for 'b', the statement is the same
         # as the frame / scope:
         #
         # def test(b=1):
         #     ...
-        if (
-            base_node.parent
-            and base_node.statement(future=True) is myframe
-            and myframe.parent
-        ):
+        if base_node.parent and base_node.statement() is myframe and myframe.parent:
             myframe = myframe.parent.frame()
 
     mystmt: nodes.Statement | None = None
     if base_node.parent:
-        mystmt = base_node.statement(future=True)
+        mystmt = base_node.statement()
 
     # line filtering if we are in the same frame
     #
     # take care node may be missing lineno information (this is the case for
     # nodes inserted for living objects)
     if myframe is frame and mystmt and mystmt.fromlineno is not None:
         assert mystmt.fromlineno is not None, mystmt
```

### Comparing `astroid-3.0.0a5/astroid/helpers.py` & `astroid-3.0.0a6/astroid/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,42 @@
 # For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
 # Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Various helper utilities."""
 
 from __future__ import annotations
 
+import warnings
 from collections.abc import Generator
 
 from astroid import bases, manager, nodes, objects, raw_building, util
 from astroid.context import CallContext, InferenceContext
 from astroid.exceptions import (
     AstroidTypeError,
     AttributeInferenceError,
     InferenceError,
     MroError,
     _NonDeducibleTypeHierarchy,
 )
 from astroid.nodes import scoped_nodes
 from astroid.typing import InferenceResult
+from astroid.util import safe_infer as real_safe_infer
+
+
+def safe_infer(
+    node: nodes.NodeNG | bases.Proxy | util.UninferableBase,
+    context: InferenceContext | None = None,
+) -> InferenceResult | None:
+    # When removing, also remove the real_safe_infer alias
+    warnings.warn(
+        "Import safe_infer from astroid.util; this shim in astroid.helpers will be removed.",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+    return real_safe_infer(node, context=context)
 
 
 def _build_proxy_class(cls_name: str, builtins: nodes.Module) -> nodes.ClassDef:
     proxy = raw_building.build_class(cls_name)
     proxy.parent = builtins
     return proxy
 
@@ -151,47 +166,22 @@
         or its type's mro doesn't work
     """
     if not isinstance(node, nodes.ClassDef):
         raise TypeError(f"{node} needs to be a ClassDef node")
     return _object_type_is_subclass(node, class_or_seq, context=context)
 
 
-def safe_infer(
-    node: nodes.NodeNG | bases.Proxy | util.UninferableBase,
-    context: InferenceContext | None = None,
-) -> InferenceResult | None:
-    """Return the inferred value for the given node.
-
-    Return None if inference failed or if there is some ambiguity (more than
-    one node has been inferred).
-    """
-    if isinstance(node, util.UninferableBase):
-        return node
-    try:
-        inferit = node.infer(context=context)
-        value = next(inferit)
-    except (InferenceError, StopIteration):
-        return None
-    try:
-        next(inferit)
-        return None  # None if there is ambiguity on the inferred node
-    except InferenceError:
-        return None  # there is some kind of ambiguity
-    except StopIteration:
-        return value
-
-
 def has_known_bases(klass, context: InferenceContext | None = None) -> bool:
     """Return whether all base classes of a class could be inferred."""
     try:
         return klass._all_bases_known
     except AttributeError:
         pass
     for base in klass.bases:
-        result = safe_infer(base, context=context)
+        result = real_safe_infer(base, context=context)
         # TODO: check for A->B->A->B pattern in class structure too?
         if (
             not isinstance(result, scoped_nodes.ClassDef)
             or result is klass
             or not has_known_bases(result, context=context)
         ):
             klass._all_bases_known = False
@@ -258,19 +248,19 @@
         or if multiple nodes are inferred or if the code executed in python
         would result in a infinite recursive check for length
     :rtype int: Integer length of node
     """
     # pylint: disable=import-outside-toplevel; circular import
     from astroid.objects import FrozenSet
 
-    inferred_node = safe_infer(node, context=context)
+    inferred_node = real_safe_infer(node, context=context)
 
     # prevent self referential length calls from causing a recursion error
     # see https://github.com/pylint-dev/astroid/issues/777
-    node_frame = node.frame(future=True)
+    node_frame = node.frame()
     if (
         isinstance(node_frame, scoped_nodes.FunctionDef)
         and node_frame.name == "__len__"
         and isinstance(inferred_node, bases.Proxy)
         and inferred_node._proxied == node_frame.parent
     ):
         message = (
@@ -320,7 +310,29 @@
         and result_of_len.is_subtype_of("builtins.int")
     ):
         # Fake a result as we don't know the arguments of the instance call.
         return 0
     raise AstroidTypeError(
         f"'{result_of_len}' object cannot be interpreted as an integer"
     )
+
+
+def _higher_function_scope(node: nodes.NodeNG) -> nodes.FunctionDef | None:
+    """Search for the first function which encloses the given
+    scope.
+
+    This can be used for looking up in that function's
+    scope, in case looking up in a lower scope for a particular
+    name fails.
+
+    :param node: A scope node.
+    :returns:
+        ``None``, if no parent function scope was found,
+        otherwise an instance of :class:`astroid.nodes.scoped_nodes.Function`,
+        which encloses the given node.
+    """
+    current = node
+    while current.parent and not isinstance(current.parent, nodes.FunctionDef):
+        current = current.parent
+    if current and current.parent:
+        return current.parent
+    return None
```

### Comparing `astroid-3.0.0a5/astroid/inference_tip.py` & `astroid-3.0.0a6/astroid/inference_tip.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/interpreter/_import/spec.py` & `astroid-3.0.0a6/astroid/interpreter/_import/spec.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/interpreter/_import/util.py` & `astroid-3.0.0a6/astroid/interpreter/_import/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,20 +74,16 @@
             # For tree a > b > c.py
             # >>> from importlib.machinery import PathFinder
             # >>> PathFinder.find_spec('a.b', ['a'])
             # KeyError: 'a'
 
             # Repair last_submodule_search_locations
             if last_submodule_search_locations:
-                # TODO: py38: remove except
-                try:
-                    # pylint: disable=unsubscriptable-object
-                    last_item = last_submodule_search_locations[-1]
-                except TypeError:
-                    last_item = last_submodule_search_locations._recalculate()[-1]
+                # pylint: disable=unsubscriptable-object
+                last_item = last_submodule_search_locations[-1]
                 # e.g. for failure example above, add 'a/b' and keep going
                 # so that find_spec('a.b.c', path=['a', 'a/b']) succeeds
                 assumed_location = pathlib.Path(last_item) / component
                 last_submodule_search_locations.append(str(assumed_location))
             continue
 
         # Update last_submodule_search_locations for next iteration
```

### Comparing `astroid-3.0.0a5/astroid/interpreter/dunder_lookup.py` & `astroid-3.0.0a6/astroid/interpreter/dunder_lookup.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/interpreter/objectmodel.py` & `astroid-3.0.0a6/astroid/interpreter/objectmodel.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/manager.py` & `astroid-3.0.0a6/astroid/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 class AstroidManager:
     """Responsible to build astroid from files or modules.
 
     Use the Borg (singleton) pattern.
     """
 
     name = "astroid loader"
-    brain: AstroidManagerBrain = {
+    brain: ClassVar[AstroidManagerBrain] = {
         "astroid_cache": {},
         "_mod_file_cache": {},
         "_failed_import_hooks": [],
         "always_load_extensions": False,
         "optimize_ast": False,
         "extension_package_whitelist": set(),
         "_transform": TransformVisitor(),
@@ -430,15 +430,15 @@
         """Clear the underlying caches, bootstrap the builtins module and
         re-register transforms.
         """
         # import here because of cyclic imports
         # pylint: disable=import-outside-toplevel
         from astroid.inference_tip import clear_inference_tip_cache
         from astroid.interpreter.objectmodel import ObjectModel
-        from astroid.nodes.node_classes import LookupMixIn
+        from astroid.nodes._base_nodes import LookupMixIn
         from astroid.nodes.scoped_nodes import ClassDef
 
         clear_inference_tip_cache()
         _invalidate_cache()  # inference context cache
 
         self.astroid_cache.clear()
         # NB: not a new TransformVisitor()
```

### Comparing `astroid-3.0.0a5/astroid/mixins.py` & `astroid-3.0.0a6/astroid/mixins.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/modutils.py` & `astroid-3.0.0a6/astroid/modutils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/node_classes.py` & `astroid-3.0.0a6/astroid/node_classes.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,15 +44,14 @@
     If,
     IfExp,
     Import,
     ImportFrom,
     JoinedStr,
     Keyword,
     List,
-    LookupMixIn,
     Match,
     MatchAs,
     MatchCase,
     MatchClass,
     MatchMapping,
     MatchOr,
     MatchSequence,
```

### Comparing `astroid-3.0.0a5/astroid/nodes/__init__.py` & `astroid-3.0.0a6/astroid/nodes/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,18 +7,14 @@
 .. seealso::
     :doc:`ast documentation <green_tree_snakes:nodes>`
 
 All nodes inherit from :class:`~astroid.nodes.node_classes.NodeNG`.
 """
 
 # Nodes not present in the builtin ast module:  DictUnpack, Unknown, and EvaluatedObject.
-
-# This is the only node we re-export from the private _base_nodes module. This
-# is because it was originally part of the public API and hasn't been deprecated.
-from astroid.nodes._base_nodes import Statement
 from astroid.nodes.node_classes import (
     CONST_CLS,
     AnnAssign,
     Arguments,
     Assert,
     Assign,
     AssignAttr,
@@ -67,26 +63,30 @@
     MatchSingleton,
     MatchStar,
     MatchValue,
     Name,
     NamedExpr,
     NodeNG,
     Nonlocal,
+    ParamSpec,
     Pass,
     Pattern,
     Raise,
     Return,
     Set,
     Slice,
     Starred,
     Subscript,
     TryExcept,
     TryFinally,
     TryStar,
     Tuple,
+    TypeAlias,
+    TypeVar,
+    TypeVarTuple,
     UnaryOp,
     Unknown,
     While,
     With,
     Yield,
     YieldFrom,
     are_exclusive,
@@ -107,18 +107,15 @@
     SetComp,
     builtin_lookup,
     function_to_method,
     get_wrapping_class,
 )
 from astroid.nodes.utils import Position
 
-_BaseContainer = BaseContainer  # TODO Remove for astroid 3.0
-
 ALL_NODE_CLASSES = (
-    _BaseContainer,
     BaseContainer,
     AnnAssign,
     Arguments,
     Assert,
     Assign,
     AssignAttr,
     AssignName,
@@ -176,27 +173,31 @@
     MatchStar,
     MatchValue,
     Module,
     Name,
     NamedExpr,
     NodeNG,
     Nonlocal,
+    ParamSpec,
+    TypeVarTuple,
     Pass,
     Pattern,
     Raise,
     Return,
     Set,
     SetComp,
     Slice,
     Starred,
     Subscript,
     TryExcept,
     TryFinally,
     TryStar,
     Tuple,
+    TypeAlias,
+    TypeVar,
     UnaryOp,
     Unknown,
     While,
     With,
     Yield,
     YieldFrom,
 )
@@ -211,14 +212,15 @@
     "AssignName",
     "AsyncFor",
     "AsyncFunctionDef",
     "AsyncWith",
     "Attribute",
     "AugAssign",
     "Await",
+    "BaseContainer",
     "BinOp",
     "BoolOp",
     "Break",
     "builtin_lookup",
     "Call",
     "ClassDef",
     "CONST_CLS",
@@ -267,28 +269,31 @@
     "MatchStar",
     "MatchValue",
     "Module",
     "Name",
     "NamedExpr",
     "NodeNG",
     "Nonlocal",
+    "ParamSpec",
     "Pass",
     "Position",
     "Raise",
     "Return",
     "Set",
     "SetComp",
     "Slice",
     "Starred",
-    "Statement",
     "Subscript",
     "TryExcept",
     "TryFinally",
     "TryStar",
     "Tuple",
+    "TypeAlias",
+    "TypeVar",
+    "TypeVarTuple",
     "UnaryOp",
     "Unknown",
     "unpack_infer",
     "While",
     "With",
     "Yield",
     "YieldFrom",
```

### Comparing `astroid-3.0.0a5/astroid/nodes/as_string.py` & `astroid-3.0.0a6/astroid/nodes/as_string.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,14 +174,15 @@
         decorate = node.decorators.accept(self) if node.decorators else ""
         args = [n.accept(self) for n in node.bases]
         if node._metaclass and not node.has_metaclass_hack():
             args.append("metaclass=" + node._metaclass.accept(self))
         args += [n.accept(self) for n in node.keywords]
         args_str = f"({', '.join(args)})" if args else ""
         docs = self._docs_dedent(node.doc_node)
+        # TODO: handle type_params
         return "\n\n{}class {}{}:{}\n{}\n".format(
             decorate, node.name, args_str, docs, self._stmt_list(node.body)
         )
 
     def visit_compare(self, node) -> str:
         """return an astroid.Compare node as string"""
         rhs_str = " ".join(
@@ -326,14 +327,15 @@
         """return a (possibly async) function definition node as string"""
         decorate = node.decorators.accept(self) if node.decorators else ""
         docs = self._docs_dedent(node.doc_node)
         trailer = ":"
         if node.returns:
             return_annotation = " -> " + node.returns.as_string()
             trailer = return_annotation + ":"
+        # TODO: handle type_params
         def_format = "\n%s%s %s(%s)%s%s\n%s"
         return def_format % (
             decorate,
             keyword,
             node.name,
             node.args.accept(self),
             trailer,
@@ -427,14 +429,18 @@
         value = node.value.accept(self)
         return f"{target} := {value}"
 
     def visit_nonlocal(self, node) -> str:
         """return an astroid.Nonlocal node as string"""
         return f"nonlocal {', '.join(node.names)}"
 
+    def visit_paramspec(self, node: nodes.ParamSpec) -> str:
+        """return an astroid.ParamSpec node as string"""
+        return node.name.accept(self)
+
     def visit_pass(self, node) -> str:
         """return an astroid.Pass node as string"""
         return "pass"
 
     def visit_raise(self, node) -> str:
         """return an astroid.Raise node as string"""
         if node.exc:
@@ -513,14 +519,26 @@
 
     def visit_tuple(self, node) -> str:
         """return an astroid.Tuple node as string"""
         if len(node.elts) == 1:
             return f"({node.elts[0].accept(self)}, )"
         return f"({', '.join(child.accept(self) for child in node.elts)})"
 
+    def visit_typealias(self, node: nodes.TypeAlias) -> str:
+        """return an astroid.TypeAlias node as string"""
+        return node.name.accept(self) if node.name else "_"
+
+    def visit_typevar(self, node: nodes.TypeVar) -> str:
+        """return an astroid.TypeVar node as string"""
+        return node.name.accept(self) if node.name else "_"
+
+    def visit_typevartuple(self, node: nodes.TypeVarTuple) -> str:
+        """return an astroid.TypeVarTuple node as string"""
+        return "*" + node.name.accept(self) if node.name else ""
+
     def visit_unaryop(self, node) -> str:
         """return an astroid.UnaryOp node as string"""
         if node.op == "not":
             operator = "not "
         else:
             operator = node.op
         return f"{operator}{self._precedence_parens(node, node.operand)}"
```

### Comparing `astroid-3.0.0a5/astroid/nodes/const.py` & `astroid-3.0.0a6/astroid/nodes/const.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/nodes/node_classes.py` & `astroid-3.0.0a6/astroid/nodes/node_classes.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,71 +3,76 @@
 # Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Module for some node classes. More nodes in scoped_nodes.py"""
 
 from __future__ import annotations
 
 import abc
+import ast
 import itertools
+import operator
 import sys
 import typing
+import warnings
 from collections.abc import Generator, Iterable, Iterator, Mapping
-from functools import cached_property, lru_cache
+from functools import cached_property
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
-    ClassVar,
     Literal,
     Optional,
-    TypeVar,
     Union,
 )
 
-from astroid import decorators, util
+from astroid import decorators, protocols, util
 from astroid.bases import Instance, _infer_stmts
 from astroid.const import _EMPTY_OBJECT_MARKER, Context
-from astroid.context import InferenceContext
+from astroid.context import CallContext, InferenceContext, copy_context
 from astroid.exceptions import (
+    AstroidBuildingError,
+    AstroidError,
     AstroidIndexError,
     AstroidTypeError,
     AstroidValueError,
+    AttributeInferenceError,
     InferenceError,
+    NameInferenceError,
     NoDefault,
     ParentMissingError,
+    _NonDeducibleTypeHierarchy,
 )
+from astroid.interpreter import dunder_lookup
 from astroid.manager import AstroidManager
 from astroid.nodes import _base_nodes
 from astroid.nodes.const import OP_PRECEDENCE
 from astroid.nodes.node_ng import NodeNG
 from astroid.typing import (
     ConstFactoryResult,
-    InferBinaryOp,
     InferenceErrorInfo,
     InferenceResult,
     SuccessfulInferenceResult,
 )
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
-
 if TYPE_CHECKING:
     from astroid import nodes
     from astroid.nodes import LocalsDictNodeNG
 
 
 def _is_const(value) -> bool:
     return isinstance(value, tuple(CONST_CLS))
 
 
-_NodesT = TypeVar("_NodesT", bound=NodeNG)
-_BadOpMessageT = TypeVar("_BadOpMessageT", bound=util.BadOperationMessage)
+_NodesT = typing.TypeVar("_NodesT", bound=NodeNG)
+_BadOpMessageT = typing.TypeVar("_BadOpMessageT", bound=util.BadOperationMessage)
 
 AssignedStmtsPossibleNode = Union["List", "Tuple", "AssignName", "AssignAttr", None]
 AssignedStmtsCall = Callable[
     [
         _NodesT,
         AssignedStmtsPossibleNode,
         Optional[InferenceContext],
@@ -333,54 +338,71 @@
 
         :returns: The name of the type.
         """
 
     def get_children(self):
         yield from self.elts
 
+    @decorators.raise_if_nothing_inferred
+    def _infer(
+        self,
+        context: InferenceContext | None = None,
+        **kwargs: Any,
+    ) -> Iterator[Self]:
+        has_starred_named_expr = any(
+            isinstance(e, (Starred, NamedExpr)) for e in self.elts
+        )
+        if has_starred_named_expr:
+            values = self._infer_sequence_helper(context)
+            new_seq = type(self)(
+                lineno=self.lineno,
+                col_offset=self.col_offset,
+                parent=self.parent,
+                end_lineno=self.end_lineno,
+                end_col_offset=self.end_col_offset,
+            )
+            new_seq.postinit(values)
 
-# TODO: Move into _base_nodes. Blocked by import of _infer_stmts from bases.
-class LookupMixIn(NodeNG):
-    """Mixin to look up a name in the right scope."""
-
-    @lru_cache  # noqa
-    def lookup(self, name: str) -> tuple[LocalsDictNodeNG, list[NodeNG]]:
-        """Lookup where the given variable is assigned.
-
-        The lookup starts from self's scope. If self is not a frame itself
-        and the name is found in the inner frame locals, statements will be
-        filtered to remove ignorable statements according to self's location.
-
-        :param name: The name of the variable to find assignments for.
-
-        :returns: The scope node and the list of assignments associated to the
-            given name according to the scope where it has been found (locals,
-            globals or builtin).
-        """
-        return self.scope().scope_lookup(self, name)
-
-    def ilookup(self, name):
-        """Lookup the inferred values of the given variable.
-
-        :param name: The variable name to find values for.
-        :type name: str
+            yield new_seq
+        else:
+            yield self
 
-        :returns: The inferred values of the statements returned from
-            :meth:`lookup`.
-        :rtype: iterable
-        """
-        frame, stmts = self.lookup(name)
-        context = InferenceContext()
-        return _infer_stmts(stmts, context, frame)
+    def _infer_sequence_helper(
+        self, context: InferenceContext | None = None
+    ) -> list[SuccessfulInferenceResult]:
+        """Infer all values based on BaseContainer.elts."""
+        values = []
+
+        for elt in self.elts:
+            if isinstance(elt, Starred):
+                starred = util.safe_infer(elt.value, context)
+                if not starred:
+                    raise InferenceError(node=self, context=context)
+                if not hasattr(starred, "elts"):
+                    raise InferenceError(node=self, context=context)
+                # TODO: fresh context?
+                values.extend(starred._infer_sequence_helper(context))
+            elif isinstance(elt, NamedExpr):
+                value = util.safe_infer(elt.value, context)
+                if not value:
+                    raise InferenceError(node=self, context=context)
+                values.append(value)
+            else:
+                values.append(elt)
+        return values
 
 
 # Name classes
 
 
-class AssignName(_base_nodes.NoChildrenNode, LookupMixIn, _base_nodes.ParentAssignNode):
+class AssignName(
+    _base_nodes.NoChildrenNode,
+    _base_nodes.LookupMixIn,
+    _base_nodes.ParentAssignNode,
+):
     """Variation of :class:`ast.Assign` representing assignment to a name.
 
     An :class:`AssignName` is the name of something that is assigned to.
     This includes variables defined in a function signature or in a loop.
 
     >>> import astroid
     >>> node = astroid.extract_node('variable = range(10)')
@@ -390,16 +412,14 @@
     [<AssignName.variable l.1 at 0x7effe1db8748>, <Call l.1 at 0x7effe1db8630>]
     >>> list(node.get_children())[0].as_string()
     'variable'
     """
 
     _other_fields = ("name",)
 
-    infer_lhs: ClassVar[InferLHS[AssignName]]
-
     def __init__(
         self,
         name: str,
         lineno: int,
         col_offset: int,
         parent: NodeNG,
         *,
@@ -413,21 +433,66 @@
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    assigned_stmts: ClassVar[AssignedStmtsCall[AssignName]]
+    assigned_stmts = protocols.assend_assigned_stmts
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
+    @decorators.raise_if_nothing_inferred
+    @decorators.path_wrapper
+    def _infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[InferenceResult, None, InferenceErrorInfo | None]:
+        """Infer an AssignName: need to inspect the RHS part of the
+        assign node.
+        """
+        if isinstance(self.parent, AugAssign):
+            return self.parent.infer(context)
+
+        stmts = list(self.assigned_stmts(context=context))
+        return _infer_stmts(stmts, context)
+
+    @decorators.raise_if_nothing_inferred
+    def infer_lhs(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[InferenceResult, None, InferenceErrorInfo | None]:
+        """Infer a Name: use name lookup rules.
+
+        Same implementation as Name._infer."""
+        # pylint: disable=import-outside-toplevel
+        from astroid.constraint import get_constraints
+        from astroid.helpers import _higher_function_scope
+
+        frame, stmts = self.lookup(self.name)
+        if not stmts:
+            # Try to see if the name is enclosed in a nested function
+            # and use the higher (first function) scope for searching.
+            parent_function = _higher_function_scope(self.scope())
+            if parent_function:
+                _, stmts = parent_function.lookup(self.name)
+
+            if not stmts:
+                raise NameInferenceError(
+                    name=self.name, scope=self.scope(), context=context
+                )
+        context = copy_context(context)
+        context.lookupname = self.name
+        context.constraints[self.name] = get_constraints(self, frame)
+
+        return _infer_stmts(stmts, context, frame)
+
 
-class DelName(_base_nodes.NoChildrenNode, LookupMixIn, _base_nodes.ParentAssignNode):
+class DelName(
+    _base_nodes.NoChildrenNode, _base_nodes.LookupMixIn, _base_nodes.ParentAssignNode
+):
     """Variation of :class:`ast.Delete` representing deletion of a name.
 
     A :class:`DelName` is the name of something that is deleted.
 
     >>> import astroid
     >>> node = astroid.extract_node("del variable #@")
     >>> list(node.get_children())
@@ -456,15 +521,15 @@
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
 
-class Name(_base_nodes.NoChildrenNode, LookupMixIn):
+class Name(_base_nodes.LookupMixIn, _base_nodes.NoChildrenNode):
     """Class representing an :class:`ast.Name` node.
 
     A :class:`Name` node is something that is named, but not covered by
     :class:`AssignName` or :class:`DelName`.
 
     >>> import astroid
     >>> node = astroid.extract_node('range(10)')
@@ -501,14 +566,46 @@
 
     def _get_name_nodes(self):
         yield self
 
         for child_node in self.get_children():
             yield from child_node._get_name_nodes()
 
+    @decorators.path_wrapper
+    def _infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[InferenceResult, None, InferenceErrorInfo | None]:
+        """Infer a Name: use name lookup rules
+
+        Same implementation as AssignName._infer_lhs."""
+        # pylint: disable=import-outside-toplevel
+        from astroid.constraint import get_constraints
+        from astroid.helpers import _higher_function_scope
+
+        frame, stmts = self.lookup(self.name)
+        if not stmts:
+            # Try to see if the name is enclosed in a nested function
+            # and use the higher (first function) scope for searching.
+            parent_function = _higher_function_scope(self.scope())
+            if parent_function:
+                _, stmts = parent_function.lookup(self.name)
+
+            if not stmts:
+                raise NameInferenceError(
+                    name=self.name, scope=self.scope(), context=context
+                )
+        context = copy_context(context)
+        context.lookupname = self.name
+        context.constraints[self.name] = get_constraints(self, frame)
+
+        return _infer_stmts(stmts, context, frame)
+
+
+DEPRECATED_ARGUMENT_DEFAULT = "DEPRECATED_ARGUMENT_DEFAULT"
+
 
 class Arguments(_base_nodes.AssignTypeNode):
     """Class representing an :class:`ast.arguments` node.
 
     An :class:`Arguments` node represents that arguments in a
     function definition.
 
@@ -656,15 +753,15 @@
         if type_comment_kwonlyargs is None:
             type_comment_kwonlyargs = []
         self.type_comment_kwonlyargs = type_comment_kwonlyargs
         if type_comment_posonlyargs is None:
             type_comment_posonlyargs = []
         self.type_comment_posonlyargs = type_comment_posonlyargs
 
-    assigned_stmts: ClassVar[AssignedStmtsCall[Arguments]]
+    assigned_stmts = protocols.arguments_assigned_stmts
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
     def _infer_name(self, frame, name):
         if self.parent is frame:
             return name
@@ -832,34 +929,36 @@
         :returns: Whether the given name is defined in the arguments,
         """
         if name == self.vararg:
             return True
         if name == self.kwarg:
             return True
         return (
-            self.find_argname(name, rec=True)[1] is not None
+            self.find_argname(name)[1] is not None
             or self.kwonlyargs
-            and _find_arg(name, self.kwonlyargs, rec=True)[1] is not None
+            and _find_arg(name, self.kwonlyargs)[1] is not None
         )
 
-    def find_argname(self, argname, rec=False):
+    def find_argname(self, argname, rec=DEPRECATED_ARGUMENT_DEFAULT):
         """Get the index and :class:`AssignName` node for given name.
 
         :param argname: The name of the argument to search for.
         :type argname: str
 
-        :param rec: Whether or not to include arguments in unpacked tuples
-            in the search.
-        :type rec: bool
-
         :returns: The index and node for the argument.
         :rtype: tuple(str or None, AssignName or None)
         """
+        if rec != DEPRECATED_ARGUMENT_DEFAULT:  # pragma: no cover
+            warnings.warn(
+                "The rec argument will be removed in astroid 3.1.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
         if self.arguments:
-            return _find_arg(argname, self.arguments, rec)
+            return _find_arg(argname, self.arguments)
         return None, None
 
     def get_children(self):
         yield from self.posonlyargs or ()
 
         for elt in self.posonlyargs_annotations:
             if elt is not None:
@@ -885,23 +984,29 @@
         if self.kwargannotation is not None:
             yield self.kwargannotation
 
         for elt in self.kwonlyargs_annotations:
             if elt is not None:
                 yield elt
 
+    @decorators.raise_if_nothing_inferred
+    def _infer(
+        self: nodes.Arguments, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[InferenceResult, None, None]:
+        # pylint: disable-next=import-outside-toplevel
+        from astroid.protocols import _arguments_infer_argname
+
+        if context is None or context.lookupname is None:
+            raise InferenceError(node=self, context=context)
+        return _arguments_infer_argname(self, context.lookupname, context)
+
 
-def _find_arg(argname, args, rec=False):
+def _find_arg(argname, args):
     for i, arg in enumerate(args):
-        if isinstance(arg, Tuple):
-            if rec:
-                found = _find_arg(argname, arg.elts)
-                if found[0] is not None:
-                    return found
-        elif arg.name == argname:
+        if arg.name == argname:
             return i, arg
     return None, None
 
 
 def _format_args(
     args, defaults=None, annotations=None, skippable_names: set[str] | None = None
 ) -> str:
@@ -930,35 +1035,66 @@
 
             if defaults is not None and i >= default_offset:
                 if defaults[i - default_offset] is not None:
                     values[-1] += default_sep + defaults[i - default_offset].as_string()
     return ", ".join(values)
 
 
-class AssignAttr(_base_nodes.ParentAssignNode):
+def _infer_attribute(
+    node: nodes.AssignAttr | nodes.Attribute,
+    context: InferenceContext | None = None,
+    **kwargs: Any,
+) -> Generator[InferenceResult, None, InferenceErrorInfo]:
+    """Infer an AssignAttr/Attribute node by using getattr on the associated object."""
+    # pylint: disable=import-outside-toplevel
+    from astroid.constraint import get_constraints
+    from astroid.nodes import ClassDef
+
+    for owner in node.expr.infer(context):
+        if isinstance(owner, util.UninferableBase):
+            yield owner
+            continue
+
+        context = copy_context(context)
+        old_boundnode = context.boundnode
+        try:
+            context.boundnode = owner
+            if isinstance(owner, (ClassDef, Instance)):
+                frame = owner if isinstance(owner, ClassDef) else owner._proxied
+                context.constraints[node.attrname] = get_constraints(node, frame=frame)
+            yield from owner.igetattr(node.attrname, context)
+        except (
+            AttributeInferenceError,
+            InferenceError,
+            AttributeError,
+        ):
+            pass
+        finally:
+            context.boundnode = old_boundnode
+    return InferenceErrorInfo(node=node, context=context)
+
+
+class AssignAttr(_base_nodes.LookupMixIn, _base_nodes.ParentAssignNode):
     """Variation of :class:`ast.Assign` representing assignment to an attribute.
 
     >>> import astroid
     >>> node = astroid.extract_node('self.attribute = range(10)')
     >>> node
     <Assign l.1 at 0x7effe1d521d0>
     >>> list(node.get_children())
     [<AssignAttr.attribute l.1 at 0x7effe1d52320>, <Call l.1 at 0x7effe1d522e8>]
     >>> list(node.get_children())[0].as_string()
     'self.attribute'
     """
 
+    expr: NodeNG
+
     _astroid_fields = ("expr",)
     _other_fields = ("attrname",)
 
-    infer_lhs: ClassVar[InferLHS[AssignAttr]]
-
-    expr: NodeNG
-    """What has the attribute that is being assigned to."""
-
     def __init__(
         self,
         attrname: str,
         lineno: int,
         col_offset: int,
         parent: NodeNG,
         *,
@@ -975,22 +1111,43 @@
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
     def postinit(self, expr: NodeNG) -> None:
         self.expr = expr
 
-    assigned_stmts: ClassVar[AssignedStmtsCall[AssignAttr]]
+    assigned_stmts = protocols.assend_assigned_stmts
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
     def get_children(self):
         yield self.expr
 
+    @decorators.raise_if_nothing_inferred
+    @decorators.path_wrapper
+    def _infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[InferenceResult, None, InferenceErrorInfo | None]:
+        """Infer an AssignAttr: need to inspect the RHS part of the
+        assign node.
+        """
+        if isinstance(self.parent, AugAssign):
+            return self.parent.infer(context)
+
+        stmts = list(self.assigned_stmts(context=context))
+        return _infer_stmts(stmts, context)
+
+    @decorators.raise_if_nothing_inferred
+    @decorators.path_wrapper
+    def infer_lhs(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[InferenceResult, None, InferenceErrorInfo | None]:
+        return _infer_attribute(self, context, **kwargs)
+
 
 class Assert(_base_nodes.Statement):
     """Class representing an :class:`ast.Assert` node.
 
     An :class:`Assert` node represents an assert statement.
 
     >>> import astroid
@@ -1048,28 +1205,31 @@
         value: NodeNG,
         type_annotation: NodeNG | None,
     ) -> None:
         self.targets = targets
         self.value = value
         self.type_annotation = type_annotation
 
-    assigned_stmts: ClassVar[AssignedStmtsCall[Assign]]
+    assigned_stmts = protocols.assign_assigned_stmts
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
     def get_children(self):
         yield from self.targets
 
         yield self.value
 
     @cached_property
     def _assign_nodes_in_scope(self) -> list[nodes.Assign]:
         return [self, *self.value._assign_nodes_in_scope]
 
+    def _get_yield_nodes_skip_functions(self):
+        yield from self.value._get_yield_nodes_skip_functions()
+
     def _get_yield_nodes_skip_lambdas(self):
         yield from self.value._get_yield_nodes_skip_lambdas()
 
 
 class AnnAssign(_base_nodes.AssignTypeNode, _base_nodes.Statement):
     """Class representing an :class:`ast.AnnAssign` node.
 
@@ -1104,28 +1264,30 @@
         value: NodeNG | None,
     ) -> None:
         self.target = target
         self.annotation = annotation
         self.value = value
         self.simple = simple
 
-    assigned_stmts: ClassVar[AssignedStmtsCall[AnnAssign]]
+    assigned_stmts = protocols.assign_annassigned_stmts
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
     def get_children(self):
         yield self.target
         yield self.annotation
 
         if self.value is not None:
             yield self.value
 
 
-class AugAssign(_base_nodes.AssignTypeNode, _base_nodes.Statement):
+class AugAssign(
+    _base_nodes.AssignTypeNode, _base_nodes.OperatorNode, _base_nodes.Statement
+):
     """Class representing an :class:`ast.AugAssign` node.
 
     An :class:`AugAssign` is an assignment paired with an operator.
 
     >>> import astroid
     >>> node = astroid.extract_node('variable += 1')
     >>> node
@@ -1165,24 +1327,19 @@
             parent=parent,
         )
 
     def postinit(self, target: Name | Attribute | Subscript, value: NodeNG) -> None:
         self.target = target
         self.value = value
 
-    assigned_stmts: ClassVar[AssignedStmtsCall[AugAssign]]
+    assigned_stmts = protocols.assign_assigned_stmts
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
-    # This is set by inference.py
-    _infer_augassign: ClassVar[
-        InferBinaryOperation[AugAssign, util.BadBinaryOperationMessage]
-    ]
-
     def type_errors(self, context: InferenceContext | None = None):
         """Get a list of type errors which can occur during inference.
 
         Each TypeError is represented by a :class:`BadBinaryOperationMessage` ,
         which holds the original exception.
 
         :returns: The list of possible type errors.
@@ -1198,21 +1355,63 @@
         except InferenceError:
             return []
 
     def get_children(self):
         yield self.target
         yield self.value
 
+    def _get_yield_nodes_skip_functions(self):
+        """An AugAssign node can contain a Yield node in the value"""
+        yield from self.value._get_yield_nodes_skip_functions()
+        yield from super()._get_yield_nodes_skip_functions()
+
     def _get_yield_nodes_skip_lambdas(self):
         """An AugAssign node can contain a Yield node in the value"""
         yield from self.value._get_yield_nodes_skip_lambdas()
         yield from super()._get_yield_nodes_skip_lambdas()
 
+    def _infer_augassign(
+        self, context: InferenceContext | None = None
+    ) -> Generator[InferenceResult | util.BadBinaryOperationMessage, None, None]:
+        """Inference logic for augmented binary operations."""
+        context = context or InferenceContext()
+
+        rhs_context = context.clone()
+
+        lhs_iter = self.target.infer_lhs(context=context)
+        rhs_iter = self.value.infer(context=rhs_context)
+
+        for lhs, rhs in itertools.product(lhs_iter, rhs_iter):
+            if any(isinstance(value, util.UninferableBase) for value in (rhs, lhs)):
+                # Don't know how to process this.
+                yield util.Uninferable
+                return
+
+            try:
+                yield from self._infer_binary_operation(
+                    left=lhs,
+                    right=rhs,
+                    binary_opnode=self,
+                    context=context,
+                    flow_factory=self._get_aug_flow,
+                )
+            except _NonDeducibleTypeHierarchy:
+                yield util.Uninferable
+
+    @decorators.raise_if_nothing_inferred
+    @decorators.path_wrapper
+    def _infer(
+        self: nodes.AugAssign, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[InferenceResult, None, None]:
+        return self._filter_operation_errors(
+            self._infer_augassign, context, util.BadBinaryOperationMessage
+        )
+
 
-class BinOp(NodeNG):
+class BinOp(_base_nodes.OperatorNode):
     """Class representing an :class:`ast.BinOp` node.
 
     A :class:`BinOp` node is an application of a binary operator.
 
     >>> import astroid
     >>> node = astroid.extract_node('a + b')
     >>> node
@@ -1249,17 +1448,14 @@
             parent=parent,
         )
 
     def postinit(self, left: NodeNG, right: NodeNG) -> None:
         self.left = left
         self.right = right
 
-    # This is set by inference.py
-    _infer_binop: ClassVar[InferBinaryOperation[BinOp, util.BadBinaryOperationMessage]]
-
     def type_errors(self, context: InferenceContext | None = None):
         """Get a list of type errors which can occur during inference.
 
         Each TypeError is represented by a :class:`BadBinaryOperationMessage`,
         which holds the original exception.
 
         :returns: The list of possible type errors.
@@ -1282,14 +1478,51 @@
     def op_precedence(self):
         return OP_PRECEDENCE[self.op]
 
     def op_left_associative(self) -> bool:
         # 2**3**4 == 2**(3**4)
         return self.op != "**"
 
+    def _infer_binop(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[InferenceResult, None, None]:
+        """Binary operation inference logic."""
+        left = self.left
+        right = self.right
+
+        # we use two separate contexts for evaluating lhs and rhs because
+        # 1. evaluating lhs may leave some undesired entries in context.path
+        #    which may not let us infer right value of rhs
+        context = context or InferenceContext()
+        lhs_context = copy_context(context)
+        rhs_context = copy_context(context)
+        lhs_iter = left.infer(context=lhs_context)
+        rhs_iter = right.infer(context=rhs_context)
+        for lhs, rhs in itertools.product(lhs_iter, rhs_iter):
+            if any(isinstance(value, util.UninferableBase) for value in (rhs, lhs)):
+                # Don't know how to process this.
+                yield util.Uninferable
+                return
+
+            try:
+                yield from self._infer_binary_operation(
+                    lhs, rhs, self, context, self._get_binop_flow
+                )
+            except _NonDeducibleTypeHierarchy:
+                yield util.Uninferable
+
+    @decorators.yes_if_nothing_inferred
+    @decorators.path_wrapper
+    def _infer(
+        self: nodes.BinOp, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[InferenceResult, None, None]:
+        return self._filter_operation_errors(
+            self._infer_binop, context, util.BadBinaryOperationMessage
+        )
+
 
 class BoolOp(NodeNG):
     """Class representing an :class:`ast.BoolOp` node.
 
     A :class:`BoolOp` is an application of a boolean operator.
 
     >>> import astroid
@@ -1351,14 +1584,68 @@
 
     def get_children(self):
         yield from self.values
 
     def op_precedence(self):
         return OP_PRECEDENCE[self.op]
 
+    @decorators.raise_if_nothing_inferred
+    @decorators.path_wrapper
+    def _infer(
+        self: nodes.BoolOp, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[InferenceResult, None, InferenceErrorInfo | None]:
+        """Infer a boolean operation (and / or / not).
+
+        The function will calculate the boolean operation
+        for all pairs generated through inference for each component
+        node.
+        """
+        values = self.values
+        if self.op == "or":
+            predicate = operator.truth
+        else:
+            predicate = operator.not_
+
+        try:
+            inferred_values = [value.infer(context=context) for value in values]
+        except InferenceError:
+            yield util.Uninferable
+            return None
+
+        for pair in itertools.product(*inferred_values):
+            if any(isinstance(item, util.UninferableBase) for item in pair):
+                # Can't infer the final result, just yield Uninferable.
+                yield util.Uninferable
+                continue
+
+            bool_values = [item.bool_value() for item in pair]
+            if any(isinstance(item, util.UninferableBase) for item in bool_values):
+                # Can't infer the final result, just yield Uninferable.
+                yield util.Uninferable
+                continue
+
+            # Since the boolean operations are short circuited operations,
+            # this code yields the first value for which the predicate is True
+            # and if no value respected the predicate, then the last value will
+            # be returned (or Uninferable if there was no last value).
+            # This is conforming to the semantics of `and` and `or`:
+            #   1 and 0 -> 1
+            #   0 and 1 -> 0
+            #   1 or 0 -> 1
+            #   0 or 1 -> 1
+            value = util.Uninferable
+            for value, bool_value in zip(pair, bool_values):
+                if predicate(bool_value):
+                    yield value
+                    break
+            else:
+                yield value
+
+        return InferenceErrorInfo(node=self, context=context)
+
 
 class Break(_base_nodes.NoChildrenNode, _base_nodes.Statement):
     """Class representing an :class:`ast.Break` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('break')
     >>> node
@@ -1408,14 +1695,72 @@
     def get_children(self):
         yield self.func
 
         yield from self.args
 
         yield from self.keywords
 
+    @decorators.raise_if_nothing_inferred
+    @decorators.path_wrapper
+    def _infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[InferenceResult, None, InferenceErrorInfo]:
+        """Infer a Call node by trying to guess what the function returns."""
+        callcontext = copy_context(context)
+        callcontext.boundnode = None
+        if context is not None:
+            callcontext.extra_context = self._populate_context_lookup(context.clone())
+
+        for callee in self.func.infer(context):
+            if isinstance(callee, util.UninferableBase):
+                yield callee
+                continue
+            try:
+                if hasattr(callee, "infer_call_result"):
+                    callcontext.callcontext = CallContext(
+                        args=self.args, keywords=self.keywords, callee=callee
+                    )
+                    yield from callee.infer_call_result(
+                        caller=self, context=callcontext
+                    )
+            except InferenceError:
+                continue
+        return InferenceErrorInfo(node=self, context=context)
+
+    def _populate_context_lookup(self, context: InferenceContext | None):
+        """Allows context to be saved for later for inference inside a function."""
+        context_lookup: dict[InferenceResult, InferenceContext] = {}
+        if context is None:
+            return context_lookup
+        for arg in self.args:
+            if isinstance(arg, Starred):
+                context_lookup[arg.value] = context
+            else:
+                context_lookup[arg] = context
+        keywords = self.keywords if self.keywords is not None else []
+        for keyword in keywords:
+            context_lookup[keyword.value] = context
+        return context_lookup
+
+
+COMPARE_OPS: dict[str, Callable[[Any, Any], bool]] = {
+    "==": operator.eq,
+    "!=": operator.ne,
+    "<": operator.lt,
+    "<=": operator.le,
+    ">": operator.gt,
+    ">=": operator.ge,
+    "in": lambda a, b: a in b,
+    "not in": lambda a, b: a not in b,
+}
+UNINFERABLE_OPS = {
+    "is",
+    "is not",
+}
+
 
 class Compare(NodeNG):
     """Class representing an :class:`ast.Compare` node.
 
     A :class:`Compare` node indicates a comparison.
 
     >>> import astroid
@@ -1457,14 +1802,96 @@
         :returns: The last child.
         :rtype: NodeNG
         """
         # XXX maybe if self.ops:
         return self.ops[-1][1]
         # return self.left
 
+    # TODO: move to util?
+    @staticmethod
+    def _to_literal(node: SuccessfulInferenceResult) -> Any:
+        # Can raise SyntaxError or ValueError from ast.literal_eval
+        # Can raise AttributeError from node.as_string() as not all nodes have a visitor
+        # Is this the stupidest idea or the simplest idea?
+        return ast.literal_eval(node.as_string())
+
+    def _do_compare(
+        self,
+        left_iter: Iterable[InferenceResult],
+        op: str,
+        right_iter: Iterable[InferenceResult],
+    ) -> bool | util.UninferableBase:
+        """
+        If all possible combinations are either True or False, return that:
+        >>> _do_compare([1, 2], '<=', [3, 4])
+        True
+        >>> _do_compare([1, 2], '==', [3, 4])
+        False
+
+        If any item is uninferable, or if some combinations are True and some
+        are False, return Uninferable:
+        >>> _do_compare([1, 3], '<=', [2, 4])
+        util.Uninferable
+        """
+        retval: bool | None = None
+        if op in UNINFERABLE_OPS:
+            return util.Uninferable
+        op_func = COMPARE_OPS[op]
+
+        for left, right in itertools.product(left_iter, right_iter):
+            if isinstance(left, util.UninferableBase) or isinstance(
+                right, util.UninferableBase
+            ):
+                return util.Uninferable
+
+            try:
+                left, right = self._to_literal(left), self._to_literal(right)
+            except (SyntaxError, ValueError, AttributeError):
+                return util.Uninferable
+
+            try:
+                expr = op_func(left, right)
+            except TypeError as exc:
+                raise AstroidTypeError from exc
+
+            if retval is None:
+                retval = expr
+            elif retval != expr:
+                return util.Uninferable
+                # (or both, but "True | False" is basically the same)
+
+        assert retval is not None
+        return retval  # it was all the same value
+
+    def _infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[nodes.Const | util.UninferableBase, None, None]:
+        """Chained comparison inference logic."""
+        retval: bool | util.UninferableBase = True
+
+        ops = self.ops
+        left_node = self.left
+        lhs = list(left_node.infer(context=context))
+        # should we break early if first element is uninferable?
+        for op, right_node in ops:
+            # eagerly evaluate rhs so that values can be re-used as lhs
+            rhs = list(right_node.infer(context=context))
+            try:
+                retval = self._do_compare(lhs, op, rhs)
+            except AstroidTypeError:
+                retval = util.Uninferable
+                break
+            if retval is not True:
+                break  # short-circuit
+            lhs = rhs  # continue
+        if retval is util.Uninferable:
+            yield retval  # type: ignore[misc]
+        else:
+            yield Const(retval)
+
 
 class Comprehension(NodeNG):
     """Class representing an :class:`ast.comprehension` node.
 
     A :class:`Comprehension` indicates the loop inside any type of
     comprehension including generator expressions.
 
@@ -1502,15 +1929,15 @@
         is_async: bool,
     ) -> None:
         self.target = target
         self.iter = iter
         self.ifs = ifs
         self.is_async = is_async
 
-    assigned_stmts: ClassVar[AssignedStmtsCall[Comprehension]]
+    assigned_stmts = protocols.for_assigned_stmts
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
     def assign_type(self):
         """The type of assignment that this node performs.
 
@@ -1523,15 +1950,15 @@
         self, lookup_node, node, stmts, mystmt: _base_nodes.Statement | None
     ):
         """method used in filter_stmts"""
         if self is mystmt:
             if isinstance(lookup_node, (Const, Name)):
                 return [lookup_node], True
 
-        elif self.statement(future=True) is mystmt:
+        elif self.statement() is mystmt:
             # original node's statement is the assignment, only keeps
             # current node (gen exp, list comp)
 
             return [node], True
 
         return stmts, False
 
@@ -1599,16 +2026,16 @@
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
         Instance.__init__(self, None)
 
-    infer_unary_op: ClassVar[InferUnaryOp[Const]]
-    infer_binary_op: ClassVar[InferBinaryOp[Const]]
+    infer_unary_op = protocols.const_infer_unary_op
+    infer_binary_op = protocols.const_infer_binary_op
 
     def __getattr__(self, name):
         # This is needed because of Proxy's __getattr__ method.
         # Calling object.__new__ on this class without calling
         # __init__ would result in an infinite loop otherwise
         # since __getattr__ is called when an attribute doesn't
         # exist and self._proxied indirectly calls self.value
@@ -1688,14 +2115,19 @@
         """Determine the boolean value of this node.
 
         :returns: The boolean value of this node.
         :rtype: bool
         """
         return bool(self.value)
 
+    def _infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Iterator[Const]:
+        yield self
+
 
 class Continue(_base_nodes.NoChildrenNode, _base_nodes.Statement):
     """Class representing an :class:`ast.Continue` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('continue')
     >>> node
@@ -1860,24 +2292,22 @@
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    def postinit(
-        self, items: list[tuple[SuccessfulInferenceResult, SuccessfulInferenceResult]]
-    ) -> None:
+    def postinit(self, items: list[tuple[InferenceResult, InferenceResult]]) -> None:
         """Do some setup after initialisation.
 
         :param items: The key-value pairs contained in the dictionary.
         """
         self.items = items
 
-    infer_unary_op: ClassVar[InferUnaryOp[Dict]]
+    infer_unary_op = protocols.dict_infer_unary_op
 
     def pytype(self) -> Literal["builtins.dict"]:
         """Get the name of the type that this node represents.
 
         :returns: The name of the type.
         """
         return "builtins.dict"
@@ -1921,21 +2351,18 @@
         :param index: The node to use as a subscript index.
 
         :raises AstroidTypeError: When the given index cannot be used as a
             subscript index, or if this node is not subscriptable.
         :raises AstroidIndexError: If the given index does not exist in the
             dictionary.
         """
-        # pylint: disable-next=import-outside-toplevel; circular import
-        from astroid.helpers import safe_infer
-
         for key, value in self.items:
             # TODO(cpopa): no support for overriding yet, {1:2, **{1: 3}}.
             if isinstance(key, DictUnpack):
-                inferred_value = safe_infer(value, context)
+                inferred_value = util.safe_infer(value, context)
                 if not isinstance(inferred_value, Dict):
                     continue
 
                 try:
                     return inferred_value.getitem(index, context)
                 except (AstroidTypeError, AstroidIndexError):
                     continue
@@ -1953,14 +2380,80 @@
         """Determine the boolean value of this node.
 
         :returns: The boolean value of this node.
         :rtype: bool
         """
         return bool(self.items)
 
+    def _infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Iterator[nodes.Dict]:
+        if not any(isinstance(k, DictUnpack) for k, _ in self.items):
+            yield self
+        else:
+            items = self._infer_map(context)
+            new_seq = type(self)(
+                lineno=self.lineno,
+                col_offset=self.col_offset,
+                parent=self.parent,
+                end_lineno=self.end_lineno,
+                end_col_offset=self.end_col_offset,
+            )
+            new_seq.postinit(list(items.items()))
+            yield new_seq
+
+    @staticmethod
+    def _update_with_replacement(
+        lhs_dict: dict[SuccessfulInferenceResult, SuccessfulInferenceResult],
+        rhs_dict: dict[SuccessfulInferenceResult, SuccessfulInferenceResult],
+    ) -> dict[SuccessfulInferenceResult, SuccessfulInferenceResult]:
+        """Delete nodes that equate to duplicate keys.
+
+        Since an astroid node doesn't 'equal' another node with the same value,
+        this function uses the as_string method to make sure duplicate keys
+        don't get through
+
+        Note that both the key and the value are astroid nodes
+
+        Fixes issue with DictUnpack causing duplicate keys
+        in inferred Dict items
+
+        :param lhs_dict: Dictionary to 'merge' nodes into
+        :param rhs_dict: Dictionary with nodes to pull from
+        :return : merged dictionary of nodes
+        """
+        combined_dict = itertools.chain(lhs_dict.items(), rhs_dict.items())
+        # Overwrite keys which have the same string values
+        string_map = {key.as_string(): (key, value) for key, value in combined_dict}
+        # Return to dictionary
+        return dict(string_map.values())
+
+    def _infer_map(
+        self, context: InferenceContext | None
+    ) -> dict[SuccessfulInferenceResult, SuccessfulInferenceResult]:
+        """Infer all values based on Dict.items."""
+        values: dict[SuccessfulInferenceResult, SuccessfulInferenceResult] = {}
+        for name, value in self.items:
+            if isinstance(name, DictUnpack):
+                double_starred = util.safe_infer(value, context)
+                if not double_starred:
+                    raise InferenceError
+                if not isinstance(double_starred, Dict):
+                    raise InferenceError(node=self, context=context)
+                unpack_items = double_starred._infer_map(context)
+                values = self._update_with_replacement(values, unpack_items)
+            else:
+                key = util.safe_infer(name, context=context)
+                safe_value = util.safe_infer(value, context=context)
+                if any(not elem for elem in (key, safe_value)):
+                    raise InferenceError(node=self, context=context)
+                # safe_value is SuccessfulInferenceResult as bool(Uninferable) == False
+                values = self._update_with_replacement(values, {key: safe_value})
+        return values
+
 
 class Expr(_base_nodes.Statement):
     """Class representing an :class:`ast.Expr` node.
 
     An :class:`Expr` is any expression that does not have its value used or
     stored.
 
@@ -1979,14 +2472,18 @@
 
     def postinit(self, value: NodeNG) -> None:
         self.value = value
 
     def get_children(self):
         yield self.value
 
+    def _get_yield_nodes_skip_functions(self):
+        if not self.value.is_function:
+            yield from self.value._get_yield_nodes_skip_functions()
+
     def _get_yield_nodes_skip_lambdas(self):
         if not self.value.is_lambda:
             yield from self.value._get_yield_nodes_skip_lambdas()
 
 
 class EmptyNode(_base_nodes.NoChildrenNode):
     """Holds an arbitrary object in the :attr:`LocalsDictNodeNG.locals`."""
@@ -2009,14 +2506,29 @@
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
     def has_underlying_object(self) -> bool:
         return self.object is not None and self.object is not _EMPTY_OBJECT_MARKER
 
+    @decorators.raise_if_nothing_inferred
+    @decorators.path_wrapper
+    def _infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[InferenceResult, None, None]:
+        if not self.has_underlying_object():
+            yield util.Uninferable
+        else:
+            try:
+                yield from AstroidManager().infer_ast_from_something(
+                    self.object, context=context
+                )
+            except AstroidError:
+                yield util.Uninferable
+
 
 class ExceptHandler(
     _base_nodes.MultiLineBlockNode, _base_nodes.AssignTypeNode, _base_nodes.Statement
 ):
     """Class representing an :class:`ast.ExceptHandler`. node.
 
     An :class:`ExceptHandler` is an ``except`` block on a try-except.
@@ -2042,15 +2554,15 @@
 
     name: AssignName | None
     """The name that the caught exception is assigned to."""
 
     body: list[NodeNG]
     """The contents of the block."""
 
-    assigned_stmts: ClassVar[AssignedStmtsCall[ExceptHandler]]
+    assigned_stmts = protocols.excepthandler_assigned_stmts
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
     def postinit(
         self,
         type: NodeNG | None,  # pylint: disable = redefined-builtin
@@ -2140,15 +2652,15 @@
     ) -> None:
         self.target = target
         self.iter = iter
         self.body = body
         self.orelse = orelse
         self.type_annotation = type_annotation
 
-    assigned_stmts: ClassVar[AssignedStmtsCall[For]]
+    assigned_stmts = protocols.for_assigned_stmts
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
     @cached_property
     def blockstart_tolineno(self):
         """The line on which the beginning of this block ends.
@@ -2281,24 +2793,57 @@
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
+    @decorators.raise_if_nothing_inferred
+    @decorators.path_wrapper
+    def _infer(
+        self,
+        context: InferenceContext | None = None,
+        asname: bool = True,
+        **kwargs: Any,
+    ) -> Generator[InferenceResult, None, None]:
+        """Infer a ImportFrom node: return the imported module/object."""
+        context = context or InferenceContext()
+        name = context.lookupname
+        if name is None:
+            raise InferenceError(node=self, context=context)
+        if asname:
+            try:
+                name = self.real_name(name)
+            except AttributeInferenceError as exc:
+                # See https://github.com/pylint-dev/pylint/issues/4692
+                raise InferenceError(node=self, context=context) from exc
+        try:
+            module = self.do_import_module()
+        except AstroidBuildingError as exc:
+            raise InferenceError(node=self, context=context) from exc
+
+        try:
+            context = copy_context(context)
+            context.lookupname = name
+            stmts = module.getattr(name, ignore_locals=module is self.root())
+            return _infer_stmts(stmts, context)
+        except AttributeInferenceError as error:
+            raise InferenceError(
+                str(error), target=self, attribute=name, context=context
+            ) from error
+
 
 class Attribute(NodeNG):
     """Class representing an :class:`ast.Attribute` node."""
 
+    expr: NodeNG
+
     _astroid_fields = ("expr",)
     _other_fields = ("attrname",)
 
-    expr: NodeNG
-    """The name that this node represents."""
-
     def __init__(
         self,
         attrname: str,
         lineno: int,
         col_offset: int,
         parent: NodeNG,
         *,
@@ -2318,14 +2863,21 @@
 
     def postinit(self, expr: NodeNG) -> None:
         self.expr = expr
 
     def get_children(self):
         yield self.expr
 
+    @decorators.raise_if_nothing_inferred
+    @decorators.path_wrapper
+    def _infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[InferenceResult, None, InferenceErrorInfo]:
+        return _infer_attribute(self, context, **kwargs)
+
 
 class Global(_base_nodes.NoChildrenNode, _base_nodes.Statement):
     """Class representing an :class:`ast.Global` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('global a_global')
     >>> node
@@ -2369,14 +2921,29 @@
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
     def _infer_name(self, frame, name):
         return name
 
+    @decorators.raise_if_nothing_inferred
+    @decorators.path_wrapper
+    def _infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[InferenceResult, None, None]:
+        if context is None or context.lookupname is None:
+            raise InferenceError(node=self, context=context)
+        try:
+            # pylint: disable-next=no-member
+            return _infer_stmts(self.root().getattr(context.lookupname), context)
+        except AttributeInferenceError as error:
+            raise InferenceError(
+                str(error), target=self, attribute=context.lookupname, context=context
+            ) from error
+
 
 class If(_base_nodes.MultiLineWithElseBlockNode, _base_nodes.Statement):
     """Class representing an :class:`ast.If` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('if condition: print(True)')
     >>> node
@@ -2427,14 +2994,19 @@
 
         yield from self.body
         yield from self.orelse
 
     def has_elif_block(self):
         return len(self.orelse) == 1 and isinstance(self.orelse[0], If)
 
+    def _get_yield_nodes_skip_functions(self):
+        """An If node can contain a Yield node in the test"""
+        yield from self.test._get_yield_nodes_skip_functions()
+        yield from super()._get_yield_nodes_skip_functions()
+
     def _get_yield_nodes_skip_lambdas(self):
         """An If node can contain a Yield node in the test"""
         yield from self.test._get_yield_nodes_skip_lambdas()
         yield from super()._get_yield_nodes_skip_lambdas()
 
 
 class IfExp(NodeNG):
@@ -2467,14 +3039,48 @@
         yield self.orelse
 
     def op_left_associative(self) -> Literal[False]:
         # `1 if True else 2 if False else 3` is parsed as
         # `1 if True else (2 if False else 3)`
         return False
 
+    @decorators.raise_if_nothing_inferred
+    def _infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[InferenceResult, None, None]:
+        """Support IfExp inference.
+
+        If we can't infer the truthiness of the condition, we default
+        to inferring both branches. Otherwise, we infer either branch
+        depending on the condition.
+        """
+        both_branches = False
+        # We use two separate contexts for evaluating lhs and rhs because
+        # evaluating lhs may leave some undesired entries in context.path
+        # which may not let us infer right value of rhs.
+
+        context = context or InferenceContext()
+        lhs_context = copy_context(context)
+        rhs_context = copy_context(context)
+        try:
+            test = next(self.test.infer(context=context.clone()))
+        except (InferenceError, StopIteration):
+            both_branches = True
+        else:
+            if not isinstance(test, util.UninferableBase):
+                if test.bool_value():
+                    yield from self.body.infer(context=lhs_context)
+                else:
+                    yield from self.orelse.infer(context=rhs_context)
+            else:
+                both_branches = True
+        if both_branches:
+            yield from self.body.infer(context=lhs_context)
+            yield from self.orelse.infer(context=rhs_context)
+
 
 class Import(_base_nodes.ImportNode):
     """Class representing an :class:`ast.Import` node.
     >>> import astroid
     >>> node = astroid.extract_node('import astroid')
     >>> node
     <Import l.1 at 0x7f23b2e4e5c0>
@@ -2519,14 +3125,36 @@
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
+    @decorators.raise_if_nothing_inferred
+    @decorators.path_wrapper
+    def _infer(
+        self,
+        context: InferenceContext | None = None,
+        asname: bool = True,
+        **kwargs: Any,
+    ) -> Generator[nodes.Module, None, None]:
+        """Infer an Import node: return the imported module/object."""
+        context = context or InferenceContext()
+        name = context.lookupname
+        if name is None:
+            raise InferenceError(node=self, context=context)
+
+        try:
+            if asname:
+                yield self.do_import_module(self.real_name(name))
+            else:
+                yield self.do_import_module(name)
+        except AstroidBuildingError as exc:
+            raise InferenceError(node=self, context=context) from exc
+
 
 class Keyword(NodeNG):
     """Class representing an :class:`ast.keyword` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('function(a_kwarg=True)')
     >>> node
@@ -2612,21 +3240,21 @@
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    assigned_stmts: ClassVar[AssignedStmtsCall[List]]
+    assigned_stmts = protocols.sequence_assigned_stmts
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
-    infer_unary_op: ClassVar[InferUnaryOp[List]]
-    infer_binary_op: ClassVar[InferBinaryOp[List]]
+    infer_unary_op = protocols.list_infer_unary_op
+    infer_binary_op = protocols.tl_infer_binary_op
 
     def pytype(self) -> Literal["builtins.list"]:
         """Get the name of the type that this node represents.
 
         :returns: The name of the type.
         """
         return "builtins.list"
@@ -2692,14 +3320,53 @@
             parent=parent,
         )
 
     def _infer_name(self, frame, name):
         return name
 
 
+class ParamSpec(_base_nodes.AssignTypeNode):
+    """Class representing a :class:`ast.ParamSpec` node.
+
+    >>> import astroid
+    >>> node = astroid.extract_node('type Alias[**P] = Callable[P, int]')
+    >>> node.type_params[0]
+    <ParamSpec l.1 at 0x7f23b2e4e198>
+    """
+
+    _astroid_fields = ("name",)
+
+    name: AssignName
+
+    def __init__(
+        self,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
+        *,
+        end_lineno: int | None,
+        end_col_offset: int | None,
+    ) -> None:
+        super().__init__(
+            lineno=lineno,
+            col_offset=col_offset,
+            end_lineno=end_lineno,
+            end_col_offset=end_col_offset,
+            parent=parent,
+        )
+
+    def postinit(self, *, name: AssignName) -> None:
+        self.name = name
+
+    def _infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Iterator[ParamSpec]:
+        yield self
+
+
 class Pass(_base_nodes.NoChildrenNode, _base_nodes.Statement):
     """Class representing an :class:`ast.Pass` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('pass')
     >>> node
     <Pass l.1 at 0x7f23b2e9e748>
@@ -2783,15 +3450,15 @@
 
     >>> import astroid
     >>> node = astroid.extract_node('{1, 2, 3}')
     >>> node
     <Set.set l.1 at 0x7f23b2e71d68>
     """
 
-    infer_unary_op: ClassVar[InferUnaryOp[Set]]
+    infer_unary_op = protocols.set_infer_unary_op
 
     def pytype(self) -> Literal["builtins.set"]:
         """Get the name of the type that this node represents.
 
         :returns: The name of the type.
         """
         return "builtins.set"
@@ -2876,14 +3543,19 @@
 
         if self.upper is not None:
             yield self.upper
 
         if self.step is not None:
             yield self.step
 
+    def _infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Iterator[Slice]:
+        yield self
+
 
 class Starred(_base_nodes.ParentAssignNode):
     """Class representing an :class:`ast.Starred` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('*args')
     >>> node
@@ -2916,15 +3588,15 @@
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
     def postinit(self, value: NodeNG) -> None:
         self.value = value
 
-    assigned_stmts: ClassVar[AssignedStmtsCall[Starred]]
+    assigned_stmts = protocols.starred_assigned_stmts
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
     def get_children(self):
         yield self.value
 
@@ -2934,19 +3606,18 @@
 
     >>> import astroid
     >>> node = astroid.extract_node('things[1:3]')
     >>> node
     <Subscript l.1 at 0x7f23b2e71f60>
     """
 
+    _SUBSCRIPT_SENTINEL = object()
     _astroid_fields = ("value", "slice")
     _other_fields = ("ctx",)
 
-    infer_lhs: ClassVar[InferLHS[Subscript]]
-
     value: NodeNG
     """What is being indexed."""
 
     slice: NodeNG
     """The slice being used to lookup."""
 
     def __init__(
@@ -2975,14 +3646,82 @@
         self.value = value
         self.slice = slice
 
     def get_children(self):
         yield self.value
         yield self.slice
 
+    def _infer_subscript(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[InferenceResult, None, InferenceErrorInfo | None]:
+        """Inference for subscripts.
+
+        We're understanding if the index is a Const
+        or a slice, passing the result of inference
+        to the value's `getitem` method, which should
+        handle each supported index type accordingly.
+        """
+        from astroid import helpers  # pylint: disable=import-outside-toplevel
+
+        found_one = False
+        for value in self.value.infer(context):
+            if isinstance(value, util.UninferableBase):
+                yield util.Uninferable
+                return None
+            for index in self.slice.infer(context):
+                if isinstance(index, util.UninferableBase):
+                    yield util.Uninferable
+                    return None
+
+                # Try to deduce the index value.
+                index_value = self._SUBSCRIPT_SENTINEL
+                if value.__class__ == Instance:
+                    index_value = index
+                elif index.__class__ == Instance:
+                    instance_as_index = helpers.class_instance_as_index(index)
+                    if instance_as_index:
+                        index_value = instance_as_index
+                else:
+                    index_value = index
+
+                if index_value is self._SUBSCRIPT_SENTINEL:
+                    raise InferenceError(node=self, context=context)
+
+                try:
+                    assigned = value.getitem(index_value, context)
+                except (
+                    AstroidTypeError,
+                    AstroidIndexError,
+                    AstroidValueError,
+                    AttributeInferenceError,
+                    AttributeError,
+                ) as exc:
+                    raise InferenceError(node=self, context=context) from exc
+
+                # Prevent inferring if the inferred subscript
+                # is the same as the original subscripted object.
+                if self is assigned or isinstance(assigned, util.UninferableBase):
+                    yield util.Uninferable
+                    return None
+                yield from assigned.infer(context)
+                found_one = True
+
+        if found_one:
+            return InferenceErrorInfo(node=self, context=context)
+        return None
+
+    @decorators.raise_if_nothing_inferred
+    @decorators.path_wrapper
+    def _infer(self, context: InferenceContext | None = None, **kwargs: Any):
+        return self._infer_subscript(context, **kwargs)
+
+    @decorators.raise_if_nothing_inferred
+    def infer_lhs(self, context: InferenceContext | None = None, **kwargs: Any):
+        return self._infer_subscript(context, **kwargs)
+
 
 class TryExcept(_base_nodes.MultiLineWithElseBlockNode, _base_nodes.Statement):
     """Class representing an :class:`ast.TryExcept` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('''
         try:
@@ -3282,21 +4021,21 @@
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    assigned_stmts: ClassVar[AssignedStmtsCall[Tuple]]
+    assigned_stmts = protocols.sequence_assigned_stmts
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
-    infer_unary_op: ClassVar[InferUnaryOp[Tuple]]
-    infer_binary_op: ClassVar[InferBinaryOp[Tuple]]
+    infer_unary_op = protocols.tuple_infer_unary_op
+    infer_binary_op = protocols.tl_infer_binary_op
 
     def pytype(self) -> Literal["builtins.tuple"]:
         """Get the name of the type that this node represents.
 
         :returns: The name of the type.
         """
         return "builtins.tuple"
@@ -3306,15 +4045,152 @@
 
         :param index: The node to use as a subscript index.
         :type index: Const or Slice
         """
         return _container_getitem(self, self.elts, index, context=context)
 
 
-class UnaryOp(NodeNG):
+class TypeAlias(_base_nodes.AssignTypeNode):
+    """Class representing a :class:`ast.TypeAlias` node.
+
+    >>> import astroid
+    >>> node = astroid.extract_node('type Point = tuple[float, float]')
+    >>> node
+    <TypeAlias l.1 at 0x7f23b2e4e198>
+    """
+
+    _astroid_fields = ("name", "type_params", "value")
+
+    name: AssignName
+    type_params: list[TypeVar | ParamSpec | TypeVarTuple]
+    value: NodeNG
+
+    def __init__(
+        self,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
+        *,
+        end_lineno: int | None,
+        end_col_offset: int | None,
+    ) -> None:
+        super().__init__(
+            lineno=lineno,
+            col_offset=col_offset,
+            end_lineno=end_lineno,
+            end_col_offset=end_col_offset,
+            parent=parent,
+        )
+
+    def postinit(
+        self,
+        *,
+        name: AssignName,
+        type_params: list[TypeVar | ParamSpec | TypeVarTuple],
+        value: NodeNG,
+    ) -> None:
+        self.name = name
+        self.type_params = type_params
+        self.value = value
+
+    def _infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Iterator[TypeAlias]:
+        yield self
+
+
+class TypeVar(_base_nodes.AssignTypeNode):
+    """Class representing a :class:`ast.TypeVar` node.
+
+    >>> import astroid
+    >>> node = astroid.extract_node('type Point[T] = tuple[float, float]')
+    >>> node.type_params[0]
+    <TypeVar l.1 at 0x7f23b2e4e198>
+    """
+
+    _astroid_fields = ("name", "bound")
+
+    name: AssignName
+    bound: NodeNG | None
+
+    def __init__(
+        self,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
+        *,
+        end_lineno: int | None,
+        end_col_offset: int | None,
+    ) -> None:
+        super().__init__(
+            lineno=lineno,
+            col_offset=col_offset,
+            end_lineno=end_lineno,
+            end_col_offset=end_col_offset,
+            parent=parent,
+        )
+
+    def postinit(self, *, name: AssignName, bound: NodeNG | None) -> None:
+        self.name = name
+        self.bound = bound
+
+    def _infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Iterator[TypeVar]:
+        yield self
+
+
+class TypeVarTuple(_base_nodes.AssignTypeNode):
+    """Class representing a :class:`ast.TypeVarTuple` node.
+
+    >>> import astroid
+    >>> node = astroid.extract_node('type Alias[*Ts] = tuple[*Ts]')
+    >>> node.type_params[0]
+    <TypeVarTuple l.1 at 0x7f23b2e4e198>
+    """
+
+    _astroid_fields = ("name",)
+
+    name: AssignName
+
+    def __init__(
+        self,
+        lineno: int,
+        col_offset: int,
+        parent: NodeNG,
+        *,
+        end_lineno: int | None,
+        end_col_offset: int | None,
+    ) -> None:
+        super().__init__(
+            lineno=lineno,
+            col_offset=col_offset,
+            end_lineno=end_lineno,
+            end_col_offset=end_col_offset,
+            parent=parent,
+        )
+
+    def postinit(self, *, name: AssignName) -> None:
+        self.name = name
+
+    def _infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Iterator[TypeVarTuple]:
+        yield self
+
+
+UNARY_OP_METHOD = {
+    "+": "__pos__",
+    "-": "__neg__",
+    "~": "__invert__",
+    "not": None,  # XXX not '__nonzero__'
+}
+
+
+class UnaryOp(_base_nodes.OperatorNode):
     """Class representing an :class:`ast.UnaryOp` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('-5')
     >>> node
     <UnaryOp l.1 at 0x7f23b2e4e198>
     """
@@ -3345,27 +4221,22 @@
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
     def postinit(self, operand: NodeNG) -> None:
         self.operand = operand
 
-    # This is set by inference.py
-    _infer_unaryop: ClassVar[
-        InferBinaryOperation[UnaryOp, util.BadUnaryOperationMessage]
-    ]
-
     def type_errors(self, context: InferenceContext | None = None):
         """Get a list of type errors which can occur during inference.
 
-        Each TypeError is represented by a :class:`BadBinaryOperationMessage`,
+        Each TypeError is represented by a :class:`BadUnaryOperationMessage`,
         which holds the original exception.
 
         :returns: The list of possible type errors.
-        :rtype: list(BadBinaryOperationMessage)
+        :rtype: list(BadUnaryOperationMessage)
         """
         try:
             results = self._infer_unaryop(context=context)
             return [
                 result
                 for result in results
                 if isinstance(result, util.BadUnaryOperationMessage)
@@ -3378,14 +4249,89 @@
 
     def op_precedence(self):
         if self.op == "not":
             return OP_PRECEDENCE[self.op]
 
         return super().op_precedence()
 
+    def _infer_unaryop(
+        self: nodes.UnaryOp, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[
+        InferenceResult | util.BadUnaryOperationMessage, None, InferenceErrorInfo
+    ]:
+        """Infer what an UnaryOp should return when evaluated."""
+        from astroid.nodes import ClassDef  # pylint: disable=import-outside-toplevel
+
+        for operand in self.operand.infer(context):
+            try:
+                yield operand.infer_unary_op(self.op)
+            except TypeError as exc:
+                # The operand doesn't support this operation.
+                yield util.BadUnaryOperationMessage(operand, self.op, exc)
+            except AttributeError as exc:
+                meth = UNARY_OP_METHOD[self.op]
+                if meth is None:
+                    # `not node`. Determine node's boolean
+                    # value and negate its result, unless it is
+                    # Uninferable, which will be returned as is.
+                    bool_value = operand.bool_value()
+                    if not isinstance(bool_value, util.UninferableBase):
+                        yield const_factory(not bool_value)
+                    else:
+                        yield util.Uninferable
+                else:
+                    if not isinstance(operand, (Instance, ClassDef)):
+                        # The operation was used on something which
+                        # doesn't support it.
+                        yield util.BadUnaryOperationMessage(operand, self.op, exc)
+                        continue
+
+                    try:
+                        try:
+                            methods = dunder_lookup.lookup(operand, meth)
+                        except AttributeInferenceError:
+                            yield util.BadUnaryOperationMessage(operand, self.op, exc)
+                            continue
+
+                        meth = methods[0]
+                        inferred = next(meth.infer(context=context), None)
+                        if (
+                            isinstance(inferred, util.UninferableBase)
+                            or not inferred.callable()
+                        ):
+                            continue
+
+                        context = copy_context(context)
+                        context.boundnode = operand
+                        context.callcontext = CallContext(args=[], callee=inferred)
+
+                        call_results = inferred.infer_call_result(self, context=context)
+                        result = next(call_results, None)
+                        if result is None:
+                            # Failed to infer, return the same type.
+                            yield operand
+                        else:
+                            yield result
+                    except AttributeInferenceError as inner_exc:
+                        # The unary operation special method was not found.
+                        yield util.BadUnaryOperationMessage(operand, self.op, inner_exc)
+                    except InferenceError:
+                        yield util.Uninferable
+
+    @decorators.raise_if_nothing_inferred
+    @decorators.path_wrapper
+    def _infer(
+        self: nodes.UnaryOp, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[InferenceResult, None, InferenceErrorInfo]:
+        """Infer what an UnaryOp should return when evaluated."""
+        yield from self._filter_operation_errors(
+            self._infer_unaryop, context, util.BadUnaryOperationMessage
+        )
+        return InferenceErrorInfo(node=self, context=context)
+
 
 class While(_base_nodes.MultiLineWithElseBlockNode, _base_nodes.Statement):
     """Class representing an :class:`ast.While` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('''
     while condition():
@@ -3437,14 +4383,19 @@
 
     def get_children(self):
         yield self.test
 
         yield from self.body
         yield from self.orelse
 
+    def _get_yield_nodes_skip_functions(self):
+        """A While node can contain a Yield node in the test"""
+        yield from self.test._get_yield_nodes_skip_functions()
+        yield from super()._get_yield_nodes_skip_functions()
+
     def _get_yield_nodes_skip_lambdas(self):
         """A While node can contain a Yield node in the test"""
         yield from self.test._get_yield_nodes_skip_lambdas()
         yield from super()._get_yield_nodes_skip_lambdas()
 
 
 class With(
@@ -3521,15 +4472,15 @@
         """
         if items is not None:
             self.items = items
         if body is not None:
             self.body = body
         self.type_annotation = type_annotation
 
-    assigned_stmts: ClassVar[AssignedStmtsCall[With]]
+    assigned_stmts = protocols.with_assigned_stmts
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
     @cached_property
     def blockstart_tolineno(self):
         """The line on which the beginning of this block ends.
@@ -3572,14 +4523,17 @@
     def postinit(self, value: NodeNG | None) -> None:
         self.value = value
 
     def get_children(self):
         if self.value is not None:
             yield self.value
 
+    def _get_yield_nodes_skip_functions(self):
+        yield self
+
     def _get_yield_nodes_skip_lambdas(self):
         yield self
 
 
 class YieldFrom(Yield):  # TODO value is required, not optional
     """Class representing an :class:`ast.YieldFrom` node."""
 
@@ -3794,41 +4748,47 @@
             parent=parent,
         )
 
     def postinit(self, target: NodeNG, value: NodeNG) -> None:
         self.target = target
         self.value = value
 
-    assigned_stmts: ClassVar[AssignedStmtsCall[NamedExpr]]
+    assigned_stmts = protocols.named_expr_assigned_stmts
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
     def frame(
         self, *, future: Literal[None, True] = None
     ) -> nodes.FunctionDef | nodes.Module | nodes.ClassDef | nodes.Lambda:
         """The first parent frame node.
 
         A frame node is a :class:`Module`, :class:`FunctionDef`,
         or :class:`ClassDef`.
 
         :returns: The first parent frame node.
         """
+        if future is not None:
+            warnings.warn(
+                "The future arg will be removed in astroid 4.0.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
         if not self.parent:
             raise ParentMissingError(target=self)
 
         # For certain parents NamedExpr evaluate to the scope of the parent
         if isinstance(self.parent, (Arguments, Keyword, Comprehension)):
             if not self.parent.parent:
                 raise ParentMissingError(target=self.parent)
             if not self.parent.parent.parent:
                 raise ParentMissingError(target=self.parent.parent)
-            return self.parent.parent.parent.frame(future=True)
+            return self.parent.parent.parent.frame()
 
-        return self.parent.frame(future=True)
+        return self.parent.frame()
 
     def scope(self) -> LocalsDictNodeNG:
         """The first parent node defining a new scope.
         These can be Module, FunctionDef, ClassDef, Lambda, or GeneratorExp nodes.
 
         :returns: The first parent scope node.
         """
@@ -3852,15 +4812,15 @@
 
         .. seealso:: :meth:`scope`
 
         :param name: The name that is being defined.
 
         :param stmt: The statement that defines the given name.
         """
-        self.frame(future=True).set_local(name, stmt)
+        self.frame().set_local(name, stmt)
 
 
 class Unknown(_base_nodes.AssignTypeNode):
     """This node represents a node in a constructed AST where
     introspection is not possible.  At the moment, it's only used in
     the args attribute of FunctionDef nodes where function signature
     introspection failed.
@@ -3900,19 +4860,21 @@
     with the resulting class acting as the non-evaluated node.
     """
 
     name = "EvaluatedObject"
     _astroid_fields = ("original",)
     _other_fields = ("value",)
 
-    def __init__(self, original: NodeNG, value: NodeNG | util.UninferableBase) -> None:
-        self.original: NodeNG = original
+    def __init__(
+        self, original: SuccessfulInferenceResult, value: InferenceResult
+    ) -> None:
+        self.original: SuccessfulInferenceResult = original
         """The original node that has already been evaluated"""
 
-        self.value: NodeNG | util.UninferableBase = value
+        self.value: InferenceResult = value
         """The inferred value"""
 
         super().__init__(
             lineno=self.original.lineno,
             col_offset=self.original.col_offset,
             parent=self.original.parent,
             end_lineno=self.original.end_lineno,
@@ -4187,25 +5149,15 @@
         patterns: list[Pattern],
         rest: AssignName | None,
     ) -> None:
         self.keys = keys
         self.patterns = patterns
         self.rest = rest
 
-    assigned_stmts: ClassVar[
-        Callable[
-            [
-                MatchMapping,
-                AssignName,
-                InferenceContext | None,
-                None,
-            ],
-            Generator[NodeNG, None, None],
-        ]
-    ]
+    assigned_stmts = protocols.match_mapping_assigned_stmts
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
 
 class MatchClass(Pattern):
     """Class representing a :class:`ast.MatchClass` node.
@@ -4294,25 +5246,15 @@
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
     def postinit(self, *, name: AssignName | None) -> None:
         self.name = name
 
-    assigned_stmts: ClassVar[
-        Callable[
-            [
-                MatchStar,
-                AssignName,
-                InferenceContext | None,
-                None,
-            ],
-            Generator[NodeNG, None, None],
-        ]
-    ]
+    assigned_stmts = protocols.match_star_assigned_stmts
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
 
 class MatchAs(_base_nodes.AssignTypeNode, Pattern):
     """Class representing a :class:`ast.MatchAs` node.
@@ -4365,25 +5307,15 @@
         *,
         pattern: Pattern | None,
         name: AssignName | None,
     ) -> None:
         self.pattern = pattern
         self.name = name
 
-    assigned_stmts: ClassVar[
-        Callable[
-            [
-                MatchAs,
-                AssignName,
-                InferenceContext | None,
-                None,
-            ],
-            Generator[NodeNG, None, None],
-        ]
-    ]
+    assigned_stmts = protocols.match_as_assigned_stmts
     """Returns the assigned statement (non inferred) according to the assignment type.
     See astroid/protocols.py for actual implementation.
     """
 
 
 class MatchOr(Pattern):
     """Class representing a :class:`ast.MatchOr` node.
```

### Comparing `astroid-3.0.0a5/astroid/nodes/node_ng.py` & `astroid-3.0.0a6/astroid/nodes/node_ng.py`

 * *Files 4% similar despite different names*

```diff
@@ -284,72 +284,50 @@
         :param node: The node to check if it is the child.
         :type node: NodeNG
 
         :returns: Whether this node is the parent of the given node.
         """
         return any(self is parent for parent in node.node_ancestors())
 
-    @overload
-    def statement(self, *, future: None = ...) -> nodes.Statement | nodes.Module:
-        ...
-
-    @overload
-    def statement(self, *, future: Literal[True]) -> nodes.Statement:
-        ...
-
-    def statement(
-        self, *, future: Literal[None, True] = None
-    ) -> nodes.Statement | nodes.Module:
+    def statement(self, *, future: Literal[None, True] = None) -> nodes.Statement:
         """The first parent node, including self, marked as statement node.
 
-        TODO: Deprecate the future parameter and only raise StatementMissing and return
-        nodes.Statement
-
-        :raises AttributeError: If self has no parent attribute
-        :raises StatementMissing: If self has no parent attribute and future is True
+        :raises StatementMissing: If self has no parent attribute.
         """
-        if self.is_statement:
-            return cast("nodes.Statement", self)
-        if not self.parent:
-            if future:
-                raise StatementMissing(target=self)
+        if future is not None:
             warnings.warn(
-                "In astroid 3.0.0 NodeNG.statement() will return either a nodes.Statement "
-                "or raise a StatementMissing exception. AttributeError will no longer be raised. "
-                "This behaviour can already be triggered "
-                "by passing 'future=True' to a statement() call.",
+                "The future arg will be removed in astroid 4.0.",
                 DeprecationWarning,
                 stacklevel=2,
             )
-            raise AttributeError(f"{self} object has no attribute 'parent'")
-        return self.parent.statement(future=future)
+        if self.is_statement:
+            return cast("nodes.Statement", self)
+        if not self.parent:
+            raise StatementMissing(target=self)
+        return self.parent.statement()
 
     def frame(
         self, *, future: Literal[None, True] = None
     ) -> nodes.FunctionDef | nodes.Module | nodes.ClassDef | nodes.Lambda:
         """The first parent frame node.
 
         A frame node is a :class:`Module`, :class:`FunctionDef`,
         :class:`ClassDef` or :class:`Lambda`.
 
         :returns: The first parent frame node.
+        :raises ParentMissingError: If self has no parent attribute.
         """
-        if self.parent is None:
-            if future:
-                raise ParentMissingError(target=self)
+        if future is not None:
             warnings.warn(
-                "In astroid 3.0.0 NodeNG.frame() will return either a Frame node, "
-                "or raise ParentMissingError. AttributeError will no longer be raised. "
-                "This behaviour can already be triggered "
-                "by passing 'future=True' to a frame() call.",
+                "The future arg will be removed in astroid 4.0.",
                 DeprecationWarning,
                 stacklevel=2,
             )
-            raise AttributeError(f"{self} object has no attribute 'parent'")
-
+        if self.parent is None:
+            raise ParentMissingError(target=self)
         return self.parent.frame(future=future)
 
     def scope(self) -> nodes.LocalsDictNodeNG:
         """The first parent node defining a new scope.
 
         These can be Module, FunctionDef, ClassDef, Lambda, or GeneratorExp nodes.
 
@@ -584,14 +562,17 @@
     def _get_name_nodes(self):
         for child_node in self.get_children():
             yield from child_node._get_name_nodes()
 
     def _get_return_nodes_skip_functions(self):
         yield from ()
 
+    def _get_yield_nodes_skip_functions(self):
+        yield from ()
+
     def _get_yield_nodes_skip_lambdas(self):
         yield from ()
 
     def _infer_name(self, frame, name):
         # overridden for ImportFrom, Import, Global, TryExcept, TryStar and Arguments
         pass
```

### Comparing `astroid-3.0.0a5/astroid/nodes/scoped_nodes/__init__.py` & `astroid-3.0.0a6/astroid/nodes/scoped_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/nodes/scoped_nodes/mixin.py` & `astroid-3.0.0a6/astroid/nodes/scoped_nodes/mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,58 +5,57 @@
 """This module contains mixin classes for scoped nodes."""
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, TypeVar, overload
 
 from astroid.filter_statements import _filter_stmts
-from astroid.nodes import node_classes, scoped_nodes
+from astroid.nodes import _base_nodes, node_classes, scoped_nodes
 from astroid.nodes.scoped_nodes.utils import builtin_lookup
 from astroid.typing import InferenceResult, SuccessfulInferenceResult
 
 if TYPE_CHECKING:
     from astroid import nodes
 
 _T = TypeVar("_T")
 
 
-class LocalsDictNodeNG(node_classes.LookupMixIn):
+class LocalsDictNodeNG(_base_nodes.LookupMixIn):
     """this class provides locals handling common to Module, FunctionDef
     and ClassDef nodes, including a dict like interface for direct access
     to locals information
     """
 
     # attributes below are set by the builder module or by raw factories
-
-    locals: dict[str, list[InferenceResult]] = {}
+    locals: dict[str, list[InferenceResult]]
     """A map of the name of a local variable to the node defining the local."""
 
     def qname(self) -> str:
         """Get the 'qualified' name of the node.
 
         For example: module.name, module.class.name ...
 
         :returns: The qualified name.
         :rtype: str
         """
         # pylint: disable=no-member; github.com/pylint-dev/astroid/issues/278
         if self.parent is None or isinstance(self.parent, node_classes.Unknown):
             return self.name
-        return f"{self.parent.frame(future=True).qname()}.{self.name}"
+        return f"{self.parent.frame().qname()}.{self.name}"
 
     def scope(self: _T) -> _T:
         """The first parent node defining a new scope.
 
         :returns: The first parent scope node.
         :rtype: Module or FunctionDef or ClassDef or Lambda or GenExpr
         """
         return self
 
     def scope_lookup(
-        self, node: node_classes.LookupMixIn, name: str, offset: int = 0
+        self, node: _base_nodes.LookupMixIn, name: str, offset: int = 0
     ) -> tuple[LocalsDictNodeNG, list[nodes.NodeNG]]:
         """Lookup where the given variable is assigned.
 
         :param node: The node to look for assignments up to.
             Any assignments after the given node are ignored.
 
         :param name: The name of the variable to find assignments for.
@@ -66,15 +65,15 @@
         :returns: This scope node and the list of assignments associated to the
             given name according to the scope where it has been found (locals,
             globals or builtin).
         """
         raise NotImplementedError
 
     def _scope_lookup(
-        self, node: node_classes.LookupMixIn, name: str, offset: int = 0
+        self, node: _base_nodes.LookupMixIn, name: str, offset: int = 0
     ) -> tuple[LocalsDictNodeNG, list[nodes.NodeNG]]:
         """XXX method for interfacing the scope lookup"""
         try:
             stmts = _filter_stmts(node, self.locals[name], self, offset)
         except KeyError:
             stmts = ()
         if stmts:
```

### Comparing `astroid-3.0.0a5/astroid/nodes/scoped_nodes/scoped_nodes.py` & `astroid-3.0.0a6/astroid/nodes/scoped_nodes/scoped_nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 import io
 import itertools
 import os
 import warnings
 from collections.abc import Generator, Iterable, Iterator, Sequence
 from functools import cached_property, lru_cache
-from typing import TYPE_CHECKING, ClassVar, Literal, NoReturn, TypeVar, overload
+from typing import TYPE_CHECKING, Any, ClassVar, Literal, NoReturn, TypeVar
 
-from astroid import bases, util
+from astroid import bases, protocols, util
 from astroid.const import IS_PYPY, PY38, PY39_PLUS, PYPY_7_3_11_PLUS
 from astroid.context import (
     CallContext,
     InferenceContext,
     bind_context_to_node,
     copy_context,
 )
@@ -30,28 +30,35 @@
     AstroidBuildingError,
     AstroidTypeError,
     AttributeInferenceError,
     DuplicateBasesError,
     InconsistentMroError,
     InferenceError,
     MroError,
+    ParentMissingError,
     StatementMissing,
     TooManyLevelsError,
 )
 from astroid.interpreter.dunder_lookup import lookup
 from astroid.interpreter.objectmodel import ClassModel, FunctionModel, ModuleModel
 from astroid.manager import AstroidManager
 from astroid.nodes import Arguments, Const, NodeNG, Unknown, _base_nodes, node_classes
 from astroid.nodes.scoped_nodes.mixin import ComprehensionScope, LocalsDictNodeNG
 from astroid.nodes.scoped_nodes.utils import builtin_lookup
 from astroid.nodes.utils import Position
-from astroid.typing import InferBinaryOp, InferenceResult, SuccessfulInferenceResult
+from astroid.typing import (
+    InferBinaryOp,
+    InferenceErrorInfo,
+    InferenceResult,
+    SuccessfulInferenceResult,
+)
 
 if TYPE_CHECKING:
-    from astroid import nodes
+    from astroid import nodes, objects
+    from astroid.nodes._base_nodes import LookupMixIn
 
 
 ITER_METHODS = ("__iter__", "__getitem__")
 EXCEPTION_BASE_CLASSES = frozenset({"Exception", "BaseException"})
 BUILTIN_DESCRIPTORS = frozenset(
     {"classmethod", "staticmethod", "builtins.classmethod", "builtins.staticmethod"}
 )
@@ -130,18 +137,18 @@
     # Found multiple Generics in mro, remove entry from inferred_bases
     # and the corresponding one from bases_mro
     inferred_bases.pop(position_in_inferred_bases)
     bases_mro.pop(position_in_inferred_bases)
 
 
 def clean_duplicates_mro(
-    sequences: Iterable[Iterable[ClassDef]],
+    sequences: list[list[ClassDef]],
     cls: ClassDef,
     context: InferenceContext | None,
-) -> Iterable[Iterable[ClassDef]]:
+) -> list[list[ClassDef]]:
     for sequence in sequences:
         seen = set()
         for node in sequence:
             lineno_and_qname = (node.lineno, node.qname())
             if lineno_and_qname in seen:
                 raise DuplicateBasesError(
                     message="Duplicates found in MROs {mros} for {cls!r}.",
@@ -192,15 +199,21 @@
     Python 2 only.
     """
 
     special_attributes = ModuleModel()
     """The names of special attributes that this module has."""
 
     # names of module attributes available through the global scope
-    scope_attrs = {"__name__", "__doc__", "__file__", "__path__", "__package__"}
+    scope_attrs: ClassVar[set[str]] = {
+        "__name__",
+        "__doc__",
+        "__file__",
+        "__path__",
+        "__package__",
+    }
     """The names of module attributes available through the global scope."""
 
     _other_fields = (
         "name",
         "file",
         "path",
         "package",
@@ -231,15 +244,15 @@
 
         self.package = package
         """Whether the node represents a package or a module."""
 
         self.pure_python = pure_python
         """Whether the ast was built from source."""
 
-        self.globals: dict[str, list[SuccessfulInferenceResult]]
+        self.globals: dict[str, list[InferenceResult]]
         """A map of the name of a global variable to the node defining the global."""
 
         self.locals = self.globals = {}
         """A map of the name of a local variable to the node defining the local."""
 
         self.body: list[node_classes.NodeNG] = []
         """The contents of the module."""
@@ -281,15 +294,15 @@
         :param lineno: Unused.
 
         :returns: The range of line numbers that this node belongs to.
         """
         return self.fromlineno, self.tolineno
 
     def scope_lookup(
-        self, node: node_classes.LookupMixIn, name: str, offset: int = 0
+        self, node: LookupMixIn, name: str, offset: int = 0
     ) -> tuple[LocalsDictNodeNG, list[node_classes.NodeNG]]:
         """Lookup where the given variable is assigned.
 
         :param node: The node to look for assignments up to.
             Any assignments after the given node are ignored.
 
         :param name: The name of the variable to find assignments for.
@@ -373,42 +386,26 @@
         If so, the module contains a complete representation,
         including the code.
 
         :returns: Whether the module has been built from a .py file.
         """
         return self.file is not None and self.file.endswith(".py")
 
-    @overload
-    def statement(self, *, future: None = ...) -> Module:
-        ...
-
-    @overload
-    def statement(self, *, future: Literal[True]) -> NoReturn:
-        ...
-
-    def statement(self, *, future: Literal[None, True] = None) -> Module | NoReturn:
+    def statement(self, *, future: Literal[None, True] = None) -> NoReturn:
         """The first parent node, including self, marked as statement node.
 
-        When called on a :class:`Module` with the future parameter this raises an error.
-
-        TODO: Deprecate the future parameter and only raise StatementMissing
-
-        :raises StatementMissing: If no self has no parent attribute and future is True
+        When called on a :class:`Module` this raises a StatementMissing.
         """
-        if future:
-            raise StatementMissing(target=self)
-        warnings.warn(
-            "In astroid 3.0.0 NodeNG.statement() will return either a nodes.Statement "
-            "or raise a StatementMissing exception. nodes.Module will no longer be "
-            "considered a statement. This behaviour can already be triggered "
-            "by passing 'future=True' to a statement() call.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self
+        if future is not None:
+            warnings.warn(
+                "The future arg will be removed in astroid 4.0.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+        raise StatementMissing(target=self)
 
     def previous_sibling(self):
         """The previous sibling statement.
 
         :returns: The previous sibling statement node.
         :rtype: NodeNG or None
         """
@@ -457,15 +454,19 @@
                 absmodname, use_cache=use_cache
             )
         except AstroidBuildingError:
             # we only want to import a sub module or package of this module,
             # skip here
             if relative_only:
                 raise
-        return AstroidManager().ast_from_module_name(modname)
+            # Don't repeat the same operation, e.g. for missing modules
+            # like "_winapi" or "nt" on POSIX systems.
+            if modname == absmodname:
+                raise
+        return AstroidManager().ast_from_module_name(modname, use_cache=use_cache)
 
     def relative_to_absolute_name(self, modname: str, level: int | None) -> str:
         """Get the absolute module name for a relative import.
 
         The relative import can be implicit or explicit.
 
         :param modname: The module name to convert.
@@ -586,14 +587,19 @@
         A frame node is a :class:`Module`, :class:`FunctionDef`,
         :class:`ClassDef` or :class:`Lambda`.
 
         :returns: The node itself.
         """
         return self
 
+    def _infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[Module, None, None]:
+        yield self
+
 
 class GeneratorExp(ComprehensionScope):
     """Class representing an :class:`ast.GeneratorExp` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('(thing for thing in things if thing)')
     >>> node
@@ -884,15 +890,15 @@
     @property
     def type(self) -> Literal["method", "function"]:
         """Whether this is a method or function.
 
         :returns: 'method' if this is a method, 'function' otherwise.
         """
         if self.args.arguments and self.args.arguments[0].name == "self":
-            if isinstance(self.parent.scope(), ClassDef):
+            if self.parent and isinstance(self.parent.scope(), ClassDef):
                 return "method"
         return "function"
 
     def __init__(
         self,
         lineno: int,
         col_offset: int,
@@ -950,15 +956,15 @@
         of the collections of variable-length arguments ("args", "kwargs",
         etc.), as well as positional-only and keyword-only arguments.
 
         :returns: The names of the arguments.
         :rtype: list(str)
         """
         if self.args.arguments:  # maybe None with builtin functions
-            names = _rec_get_names(self.args.arguments)
+            names = [elt.name for elt in self.args.arguments]
         else:
             names = []
         if self.args.vararg:
             names.append(self.args.vararg)
         names += [elt.name for elt in self.args.kwonlyargs]
         if self.args.kwarg:
             names.append(self.args.kwarg)
@@ -969,15 +975,15 @@
         caller: SuccessfulInferenceResult | None,
         context: InferenceContext | None = None,
     ) -> Iterator[InferenceResult]:
         """Infer what the function returns when called."""
         return self.body.infer(context)
 
     def scope_lookup(
-        self, node: node_classes.LookupMixIn, name: str, offset: int = 0
+        self, node: LookupMixIn, name: str, offset: int = 0
     ) -> tuple[LocalsDictNodeNG, list[NodeNG]]:
         """Lookup where the given names is assigned.
 
         :param node: The node to look for assignments up to.
             Any assignments after the given node are ignored.
 
         :param name: The name to find assignments for.
@@ -987,15 +993,17 @@
         :returns: This scope node and the list of assignments associated to the
             given name according to the scope where it has been found (locals,
             globals or builtin).
         """
         if (self.args.defaults and node in self.args.defaults) or (
             self.args.kw_defaults and node in self.args.kw_defaults
         ):
-            frame = self.parent.frame(future=True)
+            if not self.parent:
+                raise ParentMissingError(target=self)
+            frame = self.parent.frame()
             # line offset to avoid that def func(f=func) resolve the default
             # value to the defined function
             offset = -1
         else:
             # check this is not used in function decorators
             frame = self
         return frame._scope_lookup(node, name, offset)
@@ -1033,14 +1041,23 @@
             found_attrs = self.instance_attrs[name]
         if name in self.special_attributes:
             found_attrs.append(self.special_attributes.lookup(name))
         if found_attrs:
             return found_attrs
         raise AttributeInferenceError(target=self, attribute=name)
 
+    def _infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[Lambda, None, None]:
+        yield self
+
+    def _get_yield_nodes_skip_functions(self):
+        """A Lambda node can contain a Yield node in the body."""
+        yield from self.body._get_yield_nodes_skip_functions()
+
 
 class FunctionDef(
     _base_nodes.MultiLineBlockNode,
     _base_nodes.FilterStmtsBaseNode,
     _base_nodes.Statement,
     LocalsDictNodeNG,
 ):
@@ -1051,15 +1068,22 @@
     ... def my_func(arg):
     ...     return arg + 1
     ... ''')
     >>> node
     <FunctionDef.my_func l.2 at 0x7f23b2e71e10>
     """
 
-    _astroid_fields = ("decorators", "args", "returns", "doc_node", "body")
+    _astroid_fields = (
+        "decorators",
+        "args",
+        "returns",
+        "type_params",
+        "doc_node",
+        "body",
+    )
     _multi_line_block_fields = ("body",)
     returns = None
 
     decorators: node_classes.Decorators | None
     """The decorators that are applied to this method or function."""
 
     doc_node: Const | None
@@ -1095,16 +1119,14 @@
         "type_comment_returns",
         "type_comment_args",
     )
     _type = None
 
     name = "<functiondef>"
 
-    is_lambda = True
-
     special_attributes = FunctionModel()
     """The names of special attributes that this function has."""
 
     def __init__(
         self,
         name: str,
         lineno: int,
@@ -1119,38 +1141,45 @@
 
         self.locals = {}
         """A map of the name of a local variable to the node defining it."""
 
         self.body: list[NodeNG] = []
         """The contents of the function body."""
 
+        self.type_params: list[
+            nodes.TypeVar | nodes.ParamSpec | nodes.TypeVarTuple
+        ] = []
+        """PEP 695 (Python 3.12+) type params, e.g. first 'T' in def func[T]() -> T: ..."""
+
         self.instance_attrs: dict[str, list[NodeNG]] = {}
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
         if parent and not isinstance(parent, Unknown):
-            frame = parent.frame(future=True)
+            frame = parent.frame()
             frame.set_local(name, self)
 
     def postinit(
         self,
         args: Arguments,
         body: list[NodeNG],
         decorators: node_classes.Decorators | None = None,
         returns=None,
         type_comment_returns=None,
         type_comment_args=None,
         *,
         position: Position | None = None,
         doc_node: Const | None = None,
+        type_params: list[nodes.TypeVar | nodes.ParamSpec | nodes.TypeVarTuple]
+        | None = None,
     ):
         """Do some setup after initialisation.
 
         :param args: The arguments that the function takes.
 
         :param body: The contents of the function body.
 
@@ -1160,35 +1189,37 @@
             The return type annotation passed via a type comment.
         :params type_comment_args:
             The args type annotation passed via a type comment.
         :params position:
             Position of function keyword(s) and name.
         :param doc_node:
             The doc node associated with this node.
+        :param type_params:
+            The type_params associated with this node.
         """
         self.args = args
         self.body = body
         self.decorators = decorators
         self.returns = returns
         self.type_comment_returns = type_comment_returns
         self.type_comment_args = type_comment_args
         self.position = position
         self.doc_node = doc_node
+        self.type_params = type_params or []
 
     @cached_property
     def extra_decorators(self) -> list[node_classes.Call]:
         """The extra decorators that this function can have.
 
         Additional decorators are considered when they are used as
         assignments, as in ``method = staticmethod(method)``.
         The property will return all the callables that are used for
         decoration.
         """
-        frame = self.parent.frame(future=True)
-        if not isinstance(frame, ClassDef):
+        if not self.parent or not isinstance(frame := self.parent.frame(), ClassDef):
             return []
 
         decorators: list[node_classes.Call] = []
         for assign in frame._assign_nodes_in_scope:
             if isinstance(assign.value, node_classes.Call) and isinstance(
                 assign.value.func, node_classes.Name
             ):
@@ -1206,15 +1237,15 @@
                     except KeyError:
                         continue
                     else:
                         # Must be a function and in the same frame as the
                         # original method.
                         if (
                             isinstance(meth, FunctionDef)
-                            and assign_node.frame(future=True) == frame
+                            and assign_node.frame() == frame
                         ):
                             decorators.append(assign.value)
         return decorators
 
     def pytype(self) -> Literal["builtins.instancemethod", "builtins.function"]:
         """Get the name of the type that this node represents.
 
@@ -1242,15 +1273,15 @@
         of the collections of variable-length arguments ("args", "kwargs",
         etc.), as well as positional-only and keyword-only arguments.
 
         :returns: The names of the arguments.
         :rtype: list(str)
         """
         if self.args.arguments:  # maybe None with builtin functions
-            names = _rec_get_names(self.args.arguments)
+            names = [elt.name for elt in self.args.arguments]
         else:
             names = []
         if self.args.vararg:
             names.append(self.args.vararg)
         names += [elt.name for elt in self.args.kwonlyargs]
         if self.args.kwarg:
             names.append(self.args.kwarg)
@@ -1277,15 +1308,18 @@
 
         Possible values are: method, function, staticmethod, classmethod.
         """
         for decorator in self.extra_decorators:
             if decorator.func.name in BUILTIN_DESCRIPTORS:
                 return decorator.func.name
 
-        frame = self.parent.frame(future=True)
+        if not self.parent:
+            raise ParentMissingError(target=self)
+
+        frame = self.parent.frame()
         type_name = "function"
         if isinstance(frame, ClassDef):
             if self.name == "__new__":
                 return "classmethod"
             if self.name == "__init_subclass__":
                 return "classmethod"
             if self.name == "__class_getitem__":
@@ -1391,16 +1425,18 @@
     def is_method(self) -> bool:
         """Check if this function node represents a method.
 
         :returns: Whether this is a method.
         """
         # check we are defined in a ClassDef, because this is usually expected
         # (e.g. pylint...) when is_method() return True
-        return self.type != "function" and isinstance(
-            self.parent.frame(future=True), ClassDef
+        return (
+            self.type != "function"
+            and self.parent is not None
+            and isinstance(self.parent.frame(), ClassDef)
         )
 
     def decoratornames(self, context: InferenceContext | None = None) -> set[str]:
         """Get the qualified names of each of the decorators on this function.
 
         :param context:
             An inference context that can be passed to inference functions
@@ -1463,15 +1499,58 @@
         return False
 
     def is_generator(self) -> bool:
         """Check if this is a generator function.
 
         :returns: Whether this is a generator function.
         """
-        return bool(next(self._get_yield_nodes_skip_lambdas(), False))
+        yields_without_lambdas = set(self._get_yield_nodes_skip_lambdas())
+        yields_without_functions = set(self._get_yield_nodes_skip_functions())
+        # Want an intersecting member that is neither in a lambda nor a function
+        return bool(yields_without_lambdas & yields_without_functions)
+
+    def _infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[objects.Property | FunctionDef, None, InferenceErrorInfo]:
+        from astroid import objects  # pylint: disable=import-outside-toplevel
+
+        if not self.decorators or not bases._is_property(self):
+            yield self
+            return InferenceErrorInfo(node=self, context=context)
+
+        # When inferring a property, we instantiate a new `objects.Property` object,
+        # which in turn, because it inherits from `FunctionDef`, sets itself in the locals
+        # of the wrapping frame. This means that every time we infer a property, the locals
+        # are mutated with a new instance of the property. To avoid this, we detect this
+        # scenario and avoid passing the `parent` argument to the constructor.
+        if not self.parent:
+            raise ParentMissingError(target=self)
+        parent_frame = self.parent.frame()
+        property_already_in_parent_locals = self.name in parent_frame.locals and any(
+            isinstance(val, objects.Property) for val in parent_frame.locals[self.name]
+        )
+        # We also don't want to pass parent if the definition is within a Try node
+        if isinstance(
+            self.parent,
+            (node_classes.TryExcept, node_classes.TryFinally, node_classes.If),
+        ):
+            property_already_in_parent_locals = True
+
+        prop_func = objects.Property(
+            function=self,
+            name=self.name,
+            lineno=self.lineno,
+            parent=self.parent if not property_already_in_parent_locals else None,
+            col_offset=self.col_offset,
+        )
+        if property_already_in_parent_locals:
+            prop_func.parent = self.parent
+        prop_func.postinit(body=[], args=self.args, doc_node=self.doc_node)
+        yield prop_func
+        return InferenceErrorInfo(node=self, context=context)
 
     def infer_yield_result(self, context: InferenceContext | None = None):
         """Infer what the function yields when called
 
         :returns: What the function yields
         :rtype: iterable(NodeNG or Uninferable) or None
         """
@@ -1596,30 +1675,31 @@
 
         if self.returns is not None:
             yield self.returns
 
         yield from self.body
 
     def scope_lookup(
-        self, node: node_classes.LookupMixIn, name: str, offset: int = 0
+        self, node: LookupMixIn, name: str, offset: int = 0
     ) -> tuple[LocalsDictNodeNG, list[nodes.NodeNG]]:
         """Lookup where the given name is assigned."""
         if name == "__class__":
             # __class__ is an implicit closure reference created by the compiler
             # if any methods in a class body refer to either __class__ or super.
             # In our case, we want to be able to look it up in the current scope
             # when `__class__` is being used.
-            frame = self.parent.frame(future=True)
-            if isinstance(frame, ClassDef):
+            if self.parent and isinstance(frame := self.parent.frame(), ClassDef):
                 return self, [frame]
 
         if (self.args.defaults and node in self.args.defaults) or (
             self.args.kw_defaults and node in self.args.kw_defaults
         ):
-            frame = self.parent.frame(future=True)
+            if not self.parent:
+                raise ParentMissingError(target=self)
+            frame = self.parent.frame()
             # line offset to avoid that def func(f=func) resolve the default
             # value to the defined function
             offset = -1
         else:
             # check this is not used in function decorators
             frame = self
         return frame._scope_lookup(node, name, offset)
@@ -1650,26 +1730,14 @@
     >>> node
     <AsyncFunctionDef.func l.2 at 0x7f23b2e416d8>
     >>> node.body[0]
     <AsyncFor l.3 at 0x7f23b2e417b8>
     """
 
 
-def _rec_get_names(args, names: list[str] | None = None) -> list[str]:
-    """return a list of all argument names"""
-    if names is None:
-        names = []
-    for arg in args:
-        if isinstance(arg, node_classes.Tuple):
-            _rec_get_names(arg.elts, names)
-        else:
-            names.append(arg.name)
-    return names
-
-
 def _is_metaclass(klass, seen=None, context: InferenceContext | None = None) -> bool:
     """Return if the given class can be
     used as a metaclass.
     """
     if klass.name == "type":
         return True
     if seen is None:
@@ -1738,24 +1806,24 @@
     We consider that a class wraps a node if the class
     is a parent for the said node.
 
     :returns: The class that wraps the given node
     :rtype: ClassDef or None
     """
 
-    klass = node.frame(future=True)
+    klass = node.frame()
     while klass is not None and not isinstance(klass, ClassDef):
         if klass.parent is None:
             klass = None
         else:
-            klass = klass.parent.frame(future=True)
+            klass = klass.parent.frame()
     return klass
 
 
-class ClassDef(
+class ClassDef(  # pylint: disable=too-many-instance-attributes
     _base_nodes.FilterStmtsBaseNode, LocalsDictNodeNG, _base_nodes.Statement
 ):
     """Class representing an :class:`ast.ClassDef` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('''
     class Thing:
@@ -1766,15 +1834,22 @@
     <ClassDef.Thing l.2 at 0x7f23b2e9e748>
     """
 
     # some of the attributes below are set by the builder module or
     # by a raw factories
 
     # a dictionary of class instances attributes
-    _astroid_fields = ("decorators", "bases", "keywords", "doc_node", "body")  # name
+    _astroid_fields = (
+        "decorators",
+        "bases",
+        "keywords",
+        "doc_node",
+        "body",
+        "type_params",
+    )  # name
 
     decorators = None
     """The decorators that are applied to this class.
 
     :type: Decorators or None
     """
     special_attributes = ClassModel()
@@ -1833,28 +1908,35 @@
 
         self.doc_node: Const | None = None
         """The doc node associated with this node."""
 
         self.is_dataclass: bool = False
         """Whether this class is a dataclass."""
 
+        self.type_params: list[
+            nodes.TypeVar | nodes.ParamSpec | nodes.TypeVarTuple
+        ] = []
+        """PEP 695 (Python 3.12+) type params, e.g. class MyClass[T]: ..."""
+
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
         if parent and not isinstance(parent, Unknown):
-            parent.frame(future=True).set_local(name, self)
+            parent.frame().set_local(name, self)
 
         for local_name, node in self.implicit_locals():
             self.add_local_node(node, local_name)
 
-    infer_binary_op: ClassVar[InferBinaryOp[ClassDef]]
+    infer_binary_op: ClassVar[
+        InferBinaryOp[ClassDef]
+    ] = protocols.instance_class_infer_binary_op
 
     def implicit_parameters(self) -> Literal[1]:
         return 1
 
     def implicit_locals(self):
         """Get implicitly defined class definition locals.
 
@@ -1874,24 +1956,27 @@
         decorators: node_classes.Decorators | None,
         newstyle: bool | None = None,
         metaclass: NodeNG | None = None,
         keywords: list[node_classes.Keyword] | None = None,
         *,
         position: Position | None = None,
         doc_node: Const | None = None,
+        type_params: list[nodes.TypeVar | nodes.ParamSpec | nodes.TypeVarTuple]
+        | None = None,
     ) -> None:
         if keywords is not None:
             self.keywords = keywords
         self.bases = bases
         self.body = body
         self.decorators = decorators
         self._newstyle = newstyle
         self._metaclass = metaclass
         self.position = position
         self.doc_node = doc_node
+        self.type_params = type_params or []
 
     def _newstyle_impl(self, context: InferenceContext | None = None):
         if context is None:
             context = InferenceContext()
         if self._newstyle is not None:
             return self._newstyle
         for base in self.ancestors(recurs=False, context=context):
@@ -2076,15 +2161,15 @@
             context = bind_context_to_node(context, self)
             context.callcontext.callee = dunder_call
             yield from dunder_call.infer_call_result(caller, context)
         else:
             yield self.instantiate_class()
 
     def scope_lookup(
-        self, node: node_classes.LookupMixIn, name: str, offset: int = 0
+        self, node: LookupMixIn, name: str, offset: int = 0
     ) -> tuple[LocalsDictNodeNG, list[nodes.NodeNG]]:
         """Lookup where the given name is assigned.
 
         :param node: The node to look for assignments up to.
             Any assignments after the given node are ignored.
 
         :param name: The name to find assignments for.
@@ -2115,16 +2200,17 @@
             # name = ...
             # class A(name):
             #     def name(self): ...
             #
             # import name
             # class A(name.Name):
             #     def name(self): ...
-
-            frame = self.parent.frame(future=True)
+            if not self.parent:
+                raise ParentMissingError(target=self)
+            frame = self.parent.frame()
             # line offset to avoid that class A(A) resolve the ancestor to
             # the defined class
             offset = -1
         else:
             frame = self
         return frame._scope_lookup(node, name, offset)
 
@@ -2149,15 +2235,16 @@
         """
         # FIXME: should be possible to choose the resolution order
         # FIXME: inference make infinite loops possible here
         yielded = {self}
         if context is None:
             context = InferenceContext()
         if not self.bases and self.qname() != "builtins.object":
-            yield builtin_lookup("object")[1][0]
+            # This should always be a ClassDef (which we don't assert for)
+            yield builtin_lookup("object")[1][0]  # type: ignore[misc]
             return
 
         for stmt in self.bases:
             with context.restore_path():
                 try:
                     for baseobj in stmt.infer(context):
                         if not isinstance(baseobj, ClassDef):
@@ -2289,15 +2376,15 @@
         return bases.Instance(self)
 
     def getattr(
         self,
         name: str,
         context: InferenceContext | None = None,
         class_context: bool = True,
-    ) -> list[SuccessfulInferenceResult]:
+    ) -> list[InferenceResult]:
         """Get an attribute from this class, using Python's attribute semantic.
 
         This method doesn't look in the :attr:`instance_attrs` dictionary
         since it is done by an :class:`Instance` proxy at inference time.
         It may return an :class:`Uninferable` object if
         the attribute has not been
         found, but a ``__getattr__`` or ``__getattribute__`` method is defined.
@@ -2316,15 +2403,15 @@
 
         :raises AttributeInferenceError: If the attribute cannot be inferred.
         """
         if not name:
             raise AttributeInferenceError(target=self, attribute=name, context=context)
 
         # don't modify the list in self.locals!
-        values: list[SuccessfulInferenceResult] = list(self.locals.get(name, []))
+        values: list[InferenceResult] = list(self.locals.get(name, []))
         for classnode in self.ancestors(recurs=True, context=context):
             values += classnode.locals.get(name, [])
 
         if name in self.special_attributes and class_context and not values:
             result = [self.special_attributes.lookup(name)]
             if name == "__bases__":
                 # Need special treatment, since they are mutable
@@ -2334,15 +2421,15 @@
 
         if class_context:
             values += self._metaclass_lookup_attribute(name, context)
 
         # Remove AnnAssigns without value, which are not attributes in the purest sense.
         for value in values.copy():
             if isinstance(value, node_classes.AssignName):
-                stmt = value.statement(future=True)
+                stmt = value.statement()
                 if isinstance(stmt, node_classes.AnnAssign) and stmt.value is None:
                     values.pop(values.index(value))
 
         if not values:
             raise AttributeInferenceError(target=self, attribute=name, context=context)
 
         return values
@@ -2823,15 +2910,15 @@
                 # old style classes. For these we can't retrieve the .mro,
                 # although in Python it's possible, since the class we are
                 # currently working is in fact new style.
                 # So, we fallback to ancestors here.
                 ancestors = list(base.ancestors(context=context))
                 bases_mro.append(ancestors)
 
-        unmerged_mro = [[self], *bases_mro, inferred_bases]
+        unmerged_mro: list[list[ClassDef]] = [[self], *bases_mro, inferred_bases]
         unmerged_mro = clean_duplicates_mro(unmerged_mro, self, context)
         clean_typing_generic_mro(unmerged_mro)
         return _c3_merge(unmerged_mro, self, context)
 
     def mro(self, context: InferenceContext | None = None) -> list[ClassDef]:
         """Get the method resolution order, using C3 linearization.
 
@@ -2871,7 +2958,12 @@
 
         A frame node is a :class:`Module`, :class:`FunctionDef`,
         :class:`ClassDef` or :class:`Lambda`.
 
         :returns: The node itself.
         """
         return self
+
+    def _infer(
+        self, context: InferenceContext | None = None, **kwargs: Any
+    ) -> Generator[ClassDef, None, None]:
+        yield self
```

### Comparing `astroid-3.0.0a5/astroid/nodes/scoped_nodes/utils.py` & `astroid-3.0.0a6/astroid/nodes/scoped_nodes/utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/objects.py` & `astroid-3.0.0a6/astroid/objects.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/protocols.py` & `astroid-3.0.0a6/astroid/protocols.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 from __future__ import annotations
 
 import collections
 import itertools
 import operator as operator_mod
 from collections.abc import Callable, Generator, Iterator, Sequence
-from typing import Any, TypeVar
+from typing import TYPE_CHECKING, Any, TypeVar
 
-from astroid import arguments, bases, decorators, helpers, nodes, objects, util
+from astroid import bases, decorators, nodes, util
 from astroid.const import Context
 from astroid.context import InferenceContext, copy_context
 from astroid.exceptions import (
     AstroidIndexError,
     AstroidTypeError,
     AttributeInferenceError,
     InferenceError,
@@ -27,55 +27,19 @@
 from astroid.nodes import node_classes
 from astroid.typing import (
     ConstFactoryResult,
     InferenceResult,
     SuccessfulInferenceResult,
 )
 
-_TupleListNodeT = TypeVar("_TupleListNodeT", nodes.Tuple, nodes.List)
-
-
-def _reflected_name(name) -> str:
-    return "__r" + name[2:]
-
-
-def _augmented_name(name) -> str:
-    return "__i" + name[2:]
-
+if TYPE_CHECKING:
+    _TupleListNodeT = TypeVar("_TupleListNodeT", nodes.Tuple, nodes.List)
 
 _CONTEXTLIB_MGR = "contextlib.contextmanager"
-BIN_OP_METHOD = {
-    "+": "__add__",
-    "-": "__sub__",
-    "/": "__truediv__",
-    "//": "__floordiv__",
-    "*": "__mul__",
-    "**": "__pow__",
-    "%": "__mod__",
-    "&": "__and__",
-    "|": "__or__",
-    "^": "__xor__",
-    "<<": "__lshift__",
-    ">>": "__rshift__",
-    "@": "__matmul__",
-}
-
-REFLECTED_BIN_OP_METHOD = {
-    key: _reflected_name(value) for (key, value) in BIN_OP_METHOD.items()
-}
-AUGMENTED_OP_METHOD = {
-    key + "=": _augmented_name(value) for (key, value) in BIN_OP_METHOD.items()
-}
 
-UNARY_OP_METHOD = {
-    "+": "__pos__",
-    "-": "__neg__",
-    "~": "__invert__",
-    "not": None,  # XXX not '__nonzero__'
-}
 _UNARY_OPERATORS: dict[str, Callable[[Any], Any]] = {
     "+": operator_mod.pos,
     "-": operator_mod.neg,
     "~": operator_mod.invert,
     "not": operator_mod.not_,
 }
 
@@ -89,19 +53,33 @@
         value = obj
     else:
         func = _UNARY_OPERATORS[op]
         value = func(obj)
     return nodes.const_factory(value)
 
 
-nodes.Tuple.infer_unary_op = lambda self, op: _infer_unary_op(tuple(self.elts), op)
-nodes.List.infer_unary_op = lambda self, op: _infer_unary_op(self.elts, op)
-nodes.Set.infer_unary_op = lambda self, op: _infer_unary_op(set(self.elts), op)
-nodes.Const.infer_unary_op = lambda self, op: _infer_unary_op(self.value, op)
-nodes.Dict.infer_unary_op = lambda self, op: _infer_unary_op(dict(self.items), op)
+def tuple_infer_unary_op(self, op):
+    return _infer_unary_op(tuple(self.elts), op)
+
+
+def list_infer_unary_op(self, op):
+    return _infer_unary_op(self.elts, op)
+
+
+def set_infer_unary_op(self, op):
+    return _infer_unary_op(set(self.elts), op)
+
+
+def const_infer_unary_op(self, op):
+    return _infer_unary_op(self.value, op)
+
+
+def dict_infer_unary_op(self, op):
+    return _infer_unary_op(dict(self.items), op)
+
 
 # Binary operations
 
 BIN_OP_IMPL = {
     "+": lambda a, b: a + b,
     "-": lambda a, b: a - b,
     "/": lambda a, b: a / b,
@@ -153,30 +131,30 @@
     elif isinstance(self.value, str) and operator == "%":
         # TODO(cpopa): implement string interpolation later on.
         yield util.Uninferable
     else:
         yield not_implemented
 
 
-nodes.Const.infer_binary_op = const_infer_binary_op
-
-
 def _multiply_seq_by_int(
     self: _TupleListNodeT,
     opnode: nodes.AugAssign | nodes.BinOp,
-    other: nodes.Const,
+    value: int,
     context: InferenceContext,
 ) -> _TupleListNodeT:
     node = self.__class__(parent=opnode)
+    if value > 1e8:
+        node.elts = [util.Uninferable]
+        return node
     filtered_elts = (
-        helpers.safe_infer(elt, context) or util.Uninferable
+        util.safe_infer(elt, context) or util.Uninferable
         for elt in self.elts
         if not isinstance(elt, util.UninferableBase)
     )
-    node.elts = list(filtered_elts) * other.value
+    node.elts = list(filtered_elts) * value
     return node
 
 
 def _filter_uninferable_nodes(
     elts: Sequence[InferenceResult], context: InferenceContext
 ) -> Iterator[SuccessfulInferenceResult]:
     for elt in elts:
@@ -201,14 +179,16 @@
 ) -> Generator[_TupleListNodeT | nodes.Const | util.UninferableBase, None, None]:
     """Infer a binary operation on a tuple or list.
 
     The instance on which the binary operation is performed is a tuple
     or list. This refers to the left-hand side of the operation, so:
     'tuple() + 1' or '[] + A()'
     """
+    from astroid import helpers  # pylint: disable=import-outside-toplevel
+
     # For tuples and list the boundnode is no longer the tuple or list instance
     context.boundnode = None
     not_implemented = nodes.Const(NotImplemented)
     if isinstance(other, self.__class__) and operator == "+":
         node = self.__class__(parent=opnode)
         node.elts = list(
             itertools.chain(
@@ -217,48 +197,43 @@
             )
         )
         yield node
     elif isinstance(other, nodes.Const) and operator == "*":
         if not isinstance(other.value, int):
             yield not_implemented
             return
-        yield _multiply_seq_by_int(self, opnode, other, context)
+        yield _multiply_seq_by_int(self, opnode, other.value, context)
     elif isinstance(other, bases.Instance) and operator == "*":
         # Verify if the instance supports __index__.
         as_index = helpers.class_instance_as_index(other)
         if not as_index:
             yield util.Uninferable
+        elif not isinstance(as_index.value, int):  # pragma: no cover
+            # already checked by class_instance_as_index() but faster than casting
+            raise AssertionError("Please open a bug report.")
         else:
-            yield _multiply_seq_by_int(self, opnode, as_index, context)
+            yield _multiply_seq_by_int(self, opnode, as_index.value, context)
     else:
         yield not_implemented
 
 
-nodes.Tuple.infer_binary_op = tl_infer_binary_op
-nodes.List.infer_binary_op = tl_infer_binary_op
-
-
 @decorators.yes_if_nothing_inferred
 def instance_class_infer_binary_op(
-    self: bases.Instance | nodes.ClassDef,
+    self: nodes.ClassDef,
     opnode: nodes.AugAssign | nodes.BinOp,
     operator: str,
     other: InferenceResult,
     context: InferenceContext,
     method: SuccessfulInferenceResult,
 ) -> Generator[InferenceResult, None, None]:
     return method.infer_call_result(self, context)
 
 
-bases.Instance.infer_binary_op = instance_class_infer_binary_op
-nodes.ClassDef.infer_binary_op = instance_class_infer_binary_op
-
-
 # assignment ##################################################################
-
+# pylint: disable-next=pointless-string-statement
 """The assigned_stmts method is responsible to return the assigned statement
 (e.g. not inferred) according to the assignment type.
 
 The `assign_path` argument is used to record the lhs path of the original node.
 For instance if we want assigned statements for 'c' in 'a, (b,c)', assign_path
 will be [1, 1] once arrived to the Assign node.
 
@@ -333,18 +308,14 @@
         "node": self,
         "unknown": node,
         "assign_path": assign_path,
         "context": context,
     }
 
 
-nodes.For.assigned_stmts = for_assigned_stmts
-nodes.Comprehension.assigned_stmts = for_assigned_stmts
-
-
 def sequence_assigned_stmts(
     self: nodes.Tuple | nodes.List,
     node: node_classes.AssignedStmtsPossibleNode = None,
     context: InferenceContext | None = None,
     assign_path: list[int] | None = None,
 ) -> Any:
     if assign_path is None:
@@ -361,36 +332,30 @@
 
     assign_path.insert(0, index)
     return self.parent.assigned_stmts(
         node=self, context=context, assign_path=assign_path
     )
 
 
-nodes.Tuple.assigned_stmts = sequence_assigned_stmts
-nodes.List.assigned_stmts = sequence_assigned_stmts
-
-
 def assend_assigned_stmts(
     self: nodes.AssignName | nodes.AssignAttr,
     node: node_classes.AssignedStmtsPossibleNode = None,
     context: InferenceContext | None = None,
     assign_path: list[int] | None = None,
 ) -> Any:
     return self.parent.assigned_stmts(node=self, context=context)
 
 
-nodes.AssignName.assigned_stmts = assend_assigned_stmts
-nodes.AssignAttr.assigned_stmts = assend_assigned_stmts
-
-
 def _arguments_infer_argname(
     self, name: str | None, context: InferenceContext
 ) -> Generator[InferenceResult, None, None]:
     # arguments information may be missing, in which case we can't do anything
     # more
+    from astroid import arguments  # pylint: disable=import-outside-toplevel
+
     if not (self.arguments or self.vararg or self.kwarg):
         yield util.Uninferable
         return
 
     functype = self.parent.type
     # first argument of instance/class method
     if (
@@ -445,40 +410,39 @@
 
 def arguments_assigned_stmts(
     self: nodes.Arguments,
     node: node_classes.AssignedStmtsPossibleNode = None,
     context: InferenceContext | None = None,
     assign_path: list[int] | None = None,
 ) -> Any:
+    from astroid import arguments  # pylint: disable=import-outside-toplevel
+
     try:
         node_name = node.name  # type: ignore[union-attr]
     except AttributeError:
         # Added to handle edge cases where node.name is not defined.
         # https://github.com/pylint-dev/astroid/pull/1644#discussion_r901545816
         node_name = None  # pragma: no cover
 
     if context and context.callcontext:
         callee = context.callcontext.callee
         while hasattr(callee, "_proxied"):
             callee = callee._proxied
     else:
         return _arguments_infer_argname(self, node_name, context)
-    if node and getattr(callee, "name", None) == node.frame(future=True).name:
+    if node and getattr(callee, "name", None) == node.frame().name:
         # reset call context/name
         callcontext = context.callcontext
         context = copy_context(context)
         context.callcontext = None
         args = arguments.CallSite(callcontext, context=context)
         return args.infer_argument(self.parent, node_name, context)
     return _arguments_infer_argname(self, node_name, context)
 
 
-nodes.Arguments.assigned_stmts = arguments_assigned_stmts
-
-
 @decorators.raise_if_nothing_inferred
 def assign_assigned_stmts(
     self: nodes.AugAssign | nodes.Assign | nodes.AnnAssign,
     node: node_classes.AssignedStmtsPossibleNode = None,
     context: InferenceContext | None = None,
     assign_path: list[int] | None = None,
 ) -> Any:
@@ -506,19 +470,14 @@
     for inferred in assign_assigned_stmts(self, node, context, assign_path):
         if inferred is None:
             yield util.Uninferable
         else:
             yield inferred
 
 
-nodes.Assign.assigned_stmts = assign_assigned_stmts
-nodes.AnnAssign.assigned_stmts = assign_annassigned_stmts
-nodes.AugAssign.assigned_stmts = assign_assigned_stmts
-
-
 def _resolve_assignment_parts(parts, assign_path, context):
     """Recursive function to resolve multiple assignments."""
     assign_path = assign_path[:]
     index = assign_path.pop(0)
     for part in parts:
         assigned = None
         if isinstance(part, nodes.Dict):
@@ -558,30 +517,29 @@
 @decorators.raise_if_nothing_inferred
 def excepthandler_assigned_stmts(
     self: nodes.ExceptHandler,
     node: node_classes.AssignedStmtsPossibleNode = None,
     context: InferenceContext | None = None,
     assign_path: list[int] | None = None,
 ) -> Any:
+    from astroid import objects  # pylint: disable=import-outside-toplevel
+
     for assigned in node_classes.unpack_infer(self.type):
         if isinstance(assigned, nodes.ClassDef):
             assigned = objects.ExceptionInstance(assigned)
 
         yield assigned
     return {
         "node": self,
         "unknown": node,
         "assign_path": assign_path,
         "context": context,
     }
 
 
-nodes.ExceptHandler.assigned_stmts = excepthandler_assigned_stmts
-
-
 def _infer_context_manager(self, mgr, context):
     try:
         inferred = next(mgr.infer(context=context))
     except StopIteration as e:
         raise InferenceError(node=mgr) from e
     if isinstance(inferred, bases.Generator):
         # Check if it is decorated with contextlib.contextmanager.
@@ -692,17 +650,14 @@
         "node": self,
         "unknown": node,
         "assign_path": assign_path,
         "context": context,
     }
 
 
-nodes.With.assigned_stmts = with_assigned_stmts
-
-
 @decorators.raise_if_nothing_inferred
 def named_expr_assigned_stmts(
     self: nodes.NamedExpr,
     node: node_classes.AssignedStmtsPossibleNode,
     context: InferenceContext | None = None,
     assign_path: list[int] | None = None,
 ) -> Any:
@@ -714,17 +669,14 @@
             "Cannot infer NamedExpr node {node!r}",
             node=self,
             assign_path=assign_path,
             context=context,
         )
 
 
-nodes.NamedExpr.assigned_stmts = named_expr_assigned_stmts
-
-
 @decorators.yes_if_nothing_inferred
 def starred_assigned_stmts(  # noqa: C901
     self: nodes.Starred,
     node: node_classes.AssignedStmtsPossibleNode = None,
     context: InferenceContext | None = None,
     assign_path: list[int] | None = None,
 ) -> Any:
@@ -751,15 +703,15 @@
             ):
                 lookups.append((index, len(itered)))
                 break
             if isinstance(element, nodes.Tuple):
                 lookups.append((index, len(element.itered())))
                 _determine_starred_iteration_lookups(starred, element, lookups)
 
-    stmt = self.statement(future=True)
+    stmt = self.statement()
     if not isinstance(stmt, (nodes.Assign, nodes.For)):
         raise InferenceError(
             "Statement {stmt!r} enclosing {node!r} must be an Assign or For node.",
             node=self,
             stmt=stmt,
             unknown=node,
             context=context,
@@ -914,51 +866,42 @@
             unpacked.postinit(elts=found_element or [])
             yield unpacked
             return
 
         yield util.Uninferable
 
 
-nodes.Starred.assigned_stmts = starred_assigned_stmts
-
-
 @decorators.yes_if_nothing_inferred
 def match_mapping_assigned_stmts(
     self: nodes.MatchMapping,
     node: nodes.AssignName,
     context: InferenceContext | None = None,
     assign_path: None = None,
 ) -> Generator[nodes.NodeNG, None, None]:
     """Return empty generator (return -> raises StopIteration) so inferred value
     is Uninferable.
     """
     return
     yield
 
 
-nodes.MatchMapping.assigned_stmts = match_mapping_assigned_stmts
-
-
 @decorators.yes_if_nothing_inferred
 def match_star_assigned_stmts(
     self: nodes.MatchStar,
     node: nodes.AssignName,
     context: InferenceContext | None = None,
     assign_path: None = None,
 ) -> Generator[nodes.NodeNG, None, None]:
     """Return empty generator (return -> raises StopIteration) so inferred value
     is Uninferable.
     """
     return
     yield
 
 
-nodes.MatchStar.assigned_stmts = match_star_assigned_stmts
-
-
 @decorators.yes_if_nothing_inferred
 def match_as_assigned_stmts(
     self: nodes.MatchAs,
     node: nodes.AssignName,
     context: InferenceContext | None = None,
     assign_path: None = None,
 ) -> Generator[nodes.NodeNG, None, None]:
@@ -967,10 +910,7 @@
     """
     if (
         isinstance(self.parent, nodes.MatchCase)
         and isinstance(self.parent.parent, nodes.Match)
         and self.pattern is None
     ):
         yield self.parent.parent.subject
-
-
-nodes.MatchAs.assigned_stmts = match_as_assigned_stmts
```

### Comparing `astroid-3.0.0a5/astroid/raw_building.py` & `astroid-3.0.0a6/astroid/raw_building.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     types.WrapperDescriptorType,
     types.MethodDescriptorType,
     types.ClassMethodDescriptorType,
 ]
 
 # the keys of CONST_CLS eg python builtin types
 _CONSTANTS = tuple(node_classes.CONST_CLS)
-_BUILTINS = vars(builtins)
 TYPE_NONE = type(None)
 TYPE_NOTIMPLEMENTED = type(NotImplemented)
 TYPE_ELLIPSIS = type(...)
 
 
 def _attach_local_node(parent, node, name: str) -> None:
     node.name = name  # needed by add_local_node
```

### Comparing `astroid-3.0.0a5/astroid/rebuilder.py` & `astroid-3.0.0a6/astroid/rebuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 from collections.abc import Callable, Generator
 from io import StringIO
 from tokenize import TokenInfo, generate_tokens
 from typing import TYPE_CHECKING, Final, TypeVar, Union, cast, overload
 
 from astroid import nodes
 from astroid._ast import ParserModule, get_parser_module, parse_function_type_comment
-from astroid.const import IS_PYPY, PY38, PY39_PLUS, Context
+from astroid.const import IS_PYPY, PY38, PY39_PLUS, PY312_PLUS, Context
 from astroid.manager import AstroidManager
 from astroid.nodes import NodeNG
 from astroid.nodes.utils import Position
-from astroid.typing import SuccessfulInferenceResult
+from astroid.typing import InferenceResult
 
 REDIRECT: Final[dict[str, str]] = {
     "arguments": "Arguments",
     "comprehension": "Comprehension",
     "ListCompFor": "Comprehension",
     "GenExprFor": "Comprehension",
     "excepthandler": "ExceptHandler",
@@ -380,14 +380,20 @@
         def visit(self, node: ast.Nonlocal, parent: NodeNG) -> nodes.Nonlocal:
             ...
 
         @overload
         def visit(self, node: ast.Constant, parent: NodeNG) -> nodes.Const:
             ...
 
+        if sys.version_info >= (3, 12):
+
+            @overload
+            def visit(self, node: ast.ParamSpec, parent: NodeNG) -> nodes.ParamSpec:
+                ...
+
         @overload
         def visit(self, node: ast.Pass, parent: NodeNG) -> nodes.Pass:
             ...
 
         @overload
         def visit(self, node: ast.Raise, parent: NodeNG) -> nodes.Raise:
             ...
@@ -428,14 +434,30 @@
             def visit(self, node: ast.TryStar, parent: NodeNG) -> nodes.TryStar:
                 ...
 
         @overload
         def visit(self, node: ast.Tuple, parent: NodeNG) -> nodes.Tuple:
             ...
 
+        if sys.version_info >= (3, 12):
+
+            @overload
+            def visit(self, node: ast.TypeAlias, parent: NodeNG) -> nodes.TypeAlias:
+                ...
+
+            @overload
+            def visit(self, node: ast.TypeVar, parent: NodeNG) -> nodes.TypeVar:
+                ...
+
+            @overload
+            def visit(
+                self, node: ast.TypeVarTuple, parent: NodeNG
+            ) -> nodes.TypeVarTuple:
+                ...
+
         @overload
         def visit(self, node: ast.UnaryOp, parent: NodeNG) -> nodes.UnaryOp:
             ...
 
         @overload
         def visit(self, node: ast.While, parent: NodeNG) -> nodes.While:
             ...
@@ -866,14 +888,17 @@
             [
                 self.visit(kwd, newnode)
                 for kwd in node.keywords
                 if kwd.arg != "metaclass"
             ],
             position=self._get_position_info(node, newnode),
             doc_node=self.visit(doc_ast_node, newnode),
+            type_params=[self.visit(param, newnode) for param in node.type_params]
+            if PY312_PLUS
+            else [],
         )
         return newnode
 
     def visit_continue(self, node: ast.Continue, parent: NodeNG) -> nodes.Continue:
         """Visit a Continue node by returning a fresh instance of it."""
         return nodes.Continue(
             lineno=node.lineno,
@@ -990,15 +1015,15 @@
         newnode = nodes.Dict(
             lineno=node.lineno,
             col_offset=node.col_offset,
             end_lineno=node.end_lineno,
             end_col_offset=node.end_col_offset,
             parent=parent,
         )
-        items: list[tuple[SuccessfulInferenceResult, SuccessfulInferenceResult]] = list(
+        items: list[tuple[InferenceResult, InferenceResult]] = list(
             self._visit_dict_items(node, parent, newnode)
         )
         newnode.postinit(items)
         return newnode
 
     def visit_dictcomp(self, node: ast.DictComp, parent: NodeNG) -> nodes.DictComp:
         """Visit a DictComp node by returning a fresh instance of it."""
@@ -1166,14 +1191,17 @@
             body=[self.visit(child, newnode) for child in node.body],
             decorators=decorators,
             returns=returns,
             type_comment_returns=type_comment_returns,
             type_comment_args=type_comment_args,
             position=self._get_position_info(node, newnode),
             doc_node=self.visit(doc_ast_node, newnode),
+            type_params=[self.visit(param, newnode) for param in node.type_params]
+            if PY312_PLUS
+            else [],
         )
         self._global_names.pop()
         return newnode
 
     def visit_functiondef(
         self, node: ast.FunctionDef, parent: NodeNG
     ) -> nodes.FunctionDef:
@@ -1473,14 +1501,28 @@
             lineno=node.lineno,
             col_offset=node.col_offset,
             end_lineno=node.end_lineno,
             end_col_offset=node.end_col_offset,
             parent=parent,
         )
 
+    def visit_paramspec(self, node: ast.ParamSpec, parent: NodeNG) -> nodes.ParamSpec:
+        """Visit a ParamSpec node by returning a fresh instance of it."""
+        newnode = nodes.ParamSpec(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
+        # Add AssignName node for 'node.name'
+        # https://bugs.python.org/issue43994
+        newnode.postinit(name=self.visit_assignname(node, newnode, node.name))
+        return newnode
+
     def visit_pass(self, node: ast.Pass, parent: NodeNG) -> nodes.Pass:
         """Visit a Pass node by returning a fresh instance of it."""
         return nodes.Pass(
             lineno=node.lineno,
             col_offset=node.col_offset,
             end_lineno=node.end_lineno,
             end_col_offset=node.end_col_offset,
@@ -1665,14 +1707,63 @@
             end_lineno=node.end_lineno,
             end_col_offset=node.end_col_offset,
             parent=parent,
         )
         newnode.postinit([self.visit(child, newnode) for child in node.elts])
         return newnode
 
+    def visit_typealias(self, node: ast.TypeAlias, parent: NodeNG) -> nodes.TypeAlias:
+        """Visit a TypeAlias node by returning a fresh instance of it."""
+        newnode = nodes.TypeAlias(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
+        newnode.postinit(
+            name=self.visit(node.name, newnode),
+            type_params=[self.visit(p, newnode) for p in node.type_params],
+            value=self.visit(node.value, newnode),
+        )
+        return newnode
+
+    def visit_typevar(self, node: ast.TypeVar, parent: NodeNG) -> nodes.TypeVar:
+        """Visit a TypeVar node by returning a fresh instance of it."""
+        newnode = nodes.TypeVar(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
+        # Add AssignName node for 'node.name'
+        # https://bugs.python.org/issue43994
+        newnode.postinit(
+            name=self.visit_assignname(node, newnode, node.name),
+            bound=self.visit(node.bound, newnode),
+        )
+        return newnode
+
+    def visit_typevartuple(
+        self, node: ast.TypeVarTuple, parent: NodeNG
+    ) -> nodes.TypeVarTuple:
+        """Visit a TypeVarTuple node by returning a fresh instance of it."""
+        newnode = nodes.TypeVarTuple(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+            parent=parent,
+        )
+        # Add AssignName node for 'node.name'
+        # https://bugs.python.org/issue43994
+        newnode.postinit(name=self.visit_assignname(node, newnode, node.name))
+        return newnode
+
     def visit_unaryop(self, node: ast.UnaryOp, parent: NodeNG) -> nodes.UnaryOp:
         """Visit a UnaryOp node by returning a fresh instance of it."""
         newnode = nodes.UnaryOp(
             op=self._parser_module.unary_op_classes[node.op.__class__],
             lineno=node.lineno,
             col_offset=node.col_offset,
             end_lineno=node.end_lineno,
```

### Comparing `astroid-3.0.0a5/astroid/scoped_nodes.py` & `astroid-3.0.0a6/astroid/scoped_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/test_utils.py` & `astroid-3.0.0a6/astroid/test_utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/transforms.py` & `astroid-3.0.0a6/astroid/transforms.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/astroid/typing.py` & `astroid-3.0.0a6/astroid/typing.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     Protocol,
     TypedDict,
     TypeVar,
     Union,
 )
 
 if TYPE_CHECKING:
+    from collections.abc import Iterator
+
     from astroid import bases, exceptions, nodes, transforms, util
     from astroid.context import InferenceContext
     from astroid.interpreter._import import spec
 
 
 class InferenceErrorInfo(TypedDict):
     """Store additional Inference error information
@@ -80,15 +82,15 @@
 
 class InferFn(Protocol, Generic[_SuccessfulInferenceResultT_contra]):
     def __call__(
         self,
         node: _SuccessfulInferenceResultT_contra,
         context: InferenceContext | None = None,
         **kwargs: Any,
-    ) -> Generator[InferenceResult, None, None]:
+    ) -> Iterator[InferenceResult]:
         ...  # pragma: no cover
 
 
 class TransformFn(Protocol, Generic[_SuccessfulInferenceResultT]):
     def __call__(
         self,
         node: _SuccessfulInferenceResultT,
```

### Comparing `astroid-3.0.0a5/astroid.egg-info/PKG-INFO` & `astroid-3.0.0a6/astroid.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroid
-Version: 3.0.0a5
+Version: 3.0.0a6
 Summary: An abstract syntax tree for Python with inference support.
 License: LGPL-2.1-or-later
 Project-URL: Docs, https://pylint.readthedocs.io/projects/astroid/en/latest/
 Project-URL: Source Code, https://github.com/pylint-dev/astroid
 Project-URL: Bug tracker, https://github.com/pylint-dev/astroid/issues
 Project-URL: Discord server, https://discord.gg/Egy6P8AMB5
 Keywords: static code analysis,python,abstract syntax tree
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
```

### Comparing `astroid-3.0.0a5/astroid.egg-info/SOURCES.txt` & `astroid-3.0.0a6/astroid.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 astroid/const.py
 astroid/constraint.py
 astroid/context.py
 astroid/decorators.py
 astroid/exceptions.py
 astroid/filter_statements.py
 astroid/helpers.py
-astroid/inference.py
 astroid/inference_tip.py
 astroid/manager.py
 astroid/mixins.py
 astroid/modutils.py
 astroid/node_classes.py
 astroid/objects.py
 astroid/protocols.py
@@ -51,14 +50,15 @@
 astroid/brain/brain_boto3.py
 astroid/brain/brain_builtin_inference.py
 astroid/brain/brain_collections.py
 astroid/brain/brain_crypt.py
 astroid/brain/brain_ctypes.py
 astroid/brain/brain_curses.py
 astroid/brain/brain_dataclasses.py
+astroid/brain/brain_datetime.py
 astroid/brain/brain_dateutil.py
 astroid/brain/brain_fstrings.py
 astroid/brain/brain_functools.py
 astroid/brain/brain_gi.py
 astroid/brain/brain_hashlib.py
 astroid/brain/brain_http.py
 astroid/brain/brain_hypothesis.py
@@ -134,8 +134,9 @@
 tests/test_protocols.py
 tests/test_python3.py
 tests/test_raw_building.py
 tests/test_regrtest.py
 tests/test_scoped_nodes.py
 tests/test_stdlib.py
 tests/test_transforms.py
+tests/test_type_params.py
 tests/test_utils.py
```

### Comparing `astroid-3.0.0a5/pyproject.toml` & `astroid-3.0.0a6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Quality Assurance",
     "Topic :: Software Development :: Testing",
 ]
 requires-python = ">=3.8.0"
```

### Comparing `astroid-3.0.0a5/tests/resources.py` & `astroid-3.0.0a6/tests/resources.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/tests/test_builder.py` & `astroid-3.0.0a6/tests/test_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -752,25 +752,26 @@
         module = self.module
         self.assertEqual(module.name, "data.module")
         assert isinstance(module.doc_node, nodes.Const)
         self.assertEqual(module.doc_node.value, "test module for astroid\n")
         self.assertEqual(module.fromlineno, 0)
         self.assertIsNone(module.parent)
         self.assertEqual(module.frame(), module)
-        self.assertEqual(module.frame(future=True), module)
+        self.assertEqual(module.frame(), module)
         self.assertEqual(module.root(), module)
         self.assertEqual(module.file, os.path.abspath(resources.find("data/module.py")))
         self.assertEqual(module.pure_python, 1)
         self.assertEqual(module.package, 0)
         self.assertFalse(module.is_statement)
-        with pytest.warns(DeprecationWarning) as records:
-            self.assertEqual(module.statement(), module)
-            assert len(records) == 1
         with self.assertRaises(StatementMissing):
-            module.statement(future=True)
+            with pytest.warns(DeprecationWarning) as records:
+                self.assertEqual(module.statement(future=True), module)
+                assert len(records) == 1
+        with self.assertRaises(StatementMissing):
+            module.statement()
 
     def test_module_locals(self) -> None:
         """Test the 'locals' dictionary of an astroid module."""
         module = self.module
         _locals = module.locals
         self.assertIs(_locals, module.globals)
         keys = sorted(_locals.keys())
@@ -796,16 +797,16 @@
         self.assertEqual(function.name, "global_access")
         assert isinstance(function.doc_node, nodes.Const)
         self.assertEqual(function.doc_node.value, "function test")
         self.assertEqual(function.fromlineno, 11)
         self.assertTrue(function.parent)
         self.assertEqual(function.frame(), function)
         self.assertEqual(function.parent.frame(), module)
-        self.assertEqual(function.frame(future=True), function)
-        self.assertEqual(function.parent.frame(future=True), module)
+        self.assertEqual(function.frame(), function)
+        self.assertEqual(function.parent.frame(), module)
         self.assertEqual(function.root(), module)
         self.assertEqual([n.name for n in function.args.args], ["key", "val"])
         self.assertEqual(function.type, "function")
 
     def test_function_locals(self) -> None:
         """Test the 'locals' dictionary of an astroid function."""
         _locals = self.module["global_access"].locals
@@ -820,16 +821,16 @@
         self.assertEqual(klass.name, "YO")
         assert isinstance(klass.doc_node, nodes.Const)
         self.assertEqual(klass.doc_node.value, "hehe\n    haha")
         self.assertEqual(klass.fromlineno, 25)
         self.assertTrue(klass.parent)
         self.assertEqual(klass.frame(), klass)
         self.assertEqual(klass.parent.frame(), module)
-        self.assertEqual(klass.frame(future=True), klass)
-        self.assertEqual(klass.parent.frame(future=True), module)
+        self.assertEqual(klass.frame(), klass)
+        self.assertEqual(klass.parent.frame(), module)
         self.assertEqual(klass.root(), module)
         self.assertEqual(klass.basenames, [])
         self.assertTrue(klass.newstyle)
 
     def test_class_locals(self) -> None:
         """Test the 'locals' dictionary of an astroid class."""
         module = self.module
```

### Comparing `astroid-3.0.0a5/tests/test_constraint.py` & `astroid-3.0.0a6/tests/test_constraint.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/tests/test_decorators.py` & `astroid-3.0.0a6/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/tests/test_filter_statements.py` & `astroid-3.0.0a6/tests/test_filter_statements.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,11 +7,9 @@
 from astroid.nodes import EmptyNode
 
 
 def test_empty_node() -> None:
     enum_mod = extract_node("import enum")
     empty = EmptyNode(parent=enum_mod)
     empty.is_statement = True
-    filtered_statements = _filter_stmts(
-        empty, [empty.statement(future=True)], empty.frame(future=True), 0
-    )
+    filtered_statements = _filter_stmts(empty, [empty.statement()], empty.frame(), 0)
     assert filtered_statements[0] is empty
```

### Comparing `astroid-3.0.0a5/tests/test_group_exceptions.py` & `astroid-3.0.0a6/tests/test_group_exceptions.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/tests/test_helpers.py` & `astroid-3.0.0a6/tests/test_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,8 +259,18 @@
         builtin_type = self._extract("type")
         self.assertTrue(helpers.is_supertype(builtin_type, cls_a))
         self.assertTrue(helpers.is_subtype(cls_a, builtin_type))
 
 
 def test_uninferable_for_safe_infer() -> None:
     uninfer = util.Uninferable
-    assert helpers.safe_infer(util.Uninferable) == uninfer
+    assert util.safe_infer(util.Uninferable) == uninfer
+
+
+def test_safe_infer_shim() -> None:
+    with pytest.warns(DeprecationWarning) as records:
+        helpers.safe_infer(nodes.Unknown())
+
+    assert (
+        "Import safe_infer from astroid.util; this shim in astroid.helpers will be removed."
+        in records[0].message.args[0]
+    )
```

### Comparing `astroid-3.0.0a5/tests/test_inference.py` & `astroid-3.0.0a6/tests/test_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
 # Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Tests for the astroid inference capabilities."""
 
 from __future__ import annotations
 
+import sys
 import textwrap
 import unittest
 from abc import ABCMeta
 from collections.abc import Callable
 from functools import partial
 from pathlib import Path
 from typing import Any
@@ -17,34 +18,32 @@
 
 import pytest
 
 from astroid import (
     Slice,
     Uninferable,
     arguments,
-    helpers,
     manager,
     nodes,
     objects,
     test_utils,
     util,
 )
 from astroid import decorators as decoratorsmod
 from astroid.arguments import CallSite
 from astroid.bases import BoundMethod, Instance, UnboundMethod, UnionType
 from astroid.builder import AstroidBuilder, _extract_single_node, extract_node, parse
-from astroid.const import IS_PYPY, PY39_PLUS, PY310_PLUS
+from astroid.const import IS_PYPY, PY39_PLUS, PY310_PLUS, PY312_PLUS
 from astroid.context import CallContext, InferenceContext
 from astroid.exceptions import (
     AstroidTypeError,
     AttributeInferenceError,
     InferenceError,
     NotFoundError,
 )
-from astroid.inference import infer_end as inference_infer_end
 from astroid.objects import ExceptionInstance
 
 from . import resources
 
 try:
     import six  # type: ignore[import]  # pylint: disable=unused-import
 
@@ -66,15 +65,15 @@
 
 class InferenceUtilsTest(unittest.TestCase):
     def test_path_wrapper(self) -> None:
         def infer_default(self: Any, *args: InferenceContext) -> None:
             raise InferenceError
 
         infer_default = decoratorsmod.path_wrapper(infer_default)
-        infer_end = decoratorsmod.path_wrapper(inference_infer_end)
+        infer_end = decoratorsmod.path_wrapper(Slice._infer)
         with self.assertRaises(InferenceError):
             next(infer_default(1))
         self.assertEqual(next(infer_end(1)), 1)
 
 
 def _assertInferElts(
     node_type: ABCMeta,
@@ -311,24 +310,24 @@
 
     def test_unbound_method_inference(self) -> None:
         inferred = self.ast["m_unbound"].infer()
         meth1 = next(inferred)
         self.assertIsInstance(meth1, UnboundMethod)
         self.assertEqual(meth1.name, "meth1")
         self.assertEqual(meth1.parent.frame().name, "C")
-        self.assertEqual(meth1.parent.frame(future=True).name, "C")
+        self.assertEqual(meth1.parent.frame().name, "C")
         self.assertRaises(StopIteration, partial(next, inferred))
 
     def test_bound_method_inference(self) -> None:
         inferred = self.ast["m_bound"].infer()
         meth1 = next(inferred)
         self.assertIsInstance(meth1, BoundMethod)
         self.assertEqual(meth1.name, "meth1")
         self.assertEqual(meth1.parent.frame().name, "C")
-        self.assertEqual(meth1.parent.frame(future=True).name, "C")
+        self.assertEqual(meth1.parent.frame().name, "C")
         self.assertRaises(StopIteration, partial(next, inferred))
 
     def test_args_default_inference1(self) -> None:
         optarg = test_utils.get_name_node(self.ast["C"]["meth1"], "optarg")
         inferred = optarg.infer()
         obj1 = next(inferred)
         self.assertIsInstance(obj1, nodes.Const)
@@ -984,15 +983,20 @@
         """
         ast = parse(code, __name__)
         inferred = list(ast.igetattr("osp"))
         self.assertEqual(len(inferred), 1)
         self.assertIsInstance(inferred[0], nodes.Module)
         self.assertEqual(inferred[0].name, "os.path")
         inferred = list(ast.igetattr("e"))
-        self.assertEqual(len(inferred), 1)
+        if PY312_PLUS and sys.platform.startswith("win"):
+            # There are two os.path.exists exported, likely due to
+            # https://github.com/python/cpython/pull/101324
+            self.assertEqual(len(inferred), 2)
+        else:
+            self.assertEqual(len(inferred), 1)
         self.assertIsInstance(inferred[0], nodes.FunctionDef)
         self.assertEqual(inferred[0].name, "exists")
 
     def test_do_import_module_performance(self) -> None:
         import_node = extract_node("import importlib")
         import_node.modname = ""
         import_node.do_import_module()
@@ -4020,15 +4024,15 @@
                 return self
         flow = AttributeDict()
         flow['app'] = AttributeDict()
         flow['app']['config'] = AttributeDict()
         flow['app']['config']['doffing'] = AttributeDict() #@
         """
         )
-        self.assertIsInstance(helpers.safe_infer(ast_node.targets[0]), Instance)
+        self.assertIsInstance(util.safe_infer(ast_node.targets[0]), Instance)
 
     def test_classmethod_inferred_by_context(self) -> None:
         ast_node = extract_node(
             """
         class Super(object):
            def instance(cls):
               return cls()
@@ -6311,14 +6315,28 @@
     inferred = next(node.infer())
     assert isinstance(inferred, ExceptionInstance)
     index = inferred.getattr("index")
     assert len(index) == 1
     assert isinstance(index[0], nodes.AssignAttr)
 
 
+def test_infer_assign_attr() -> None:
+    code = """
+    class Counter:
+        def __init__(self):
+            self.count = 0
+
+        def increment(self):
+            self.count += 1  #@
+    """
+    node = extract_node(code)
+    inferred = next(node.infer())
+    assert inferred.value == 1
+
+
 @pytest.mark.parametrize(
     "code,instance_name",
     [
         (
             """
         class A:
             def __enter__(self):
@@ -6489,15 +6507,15 @@
         a = "foo"
     inst = Foo()
 
     b = tuple([inst.a]) #@
     inst.a = b
     """
     )
-    helpers.safe_infer(node.targets[0])
+    util.safe_infer(node.targets[0])
 
 
 def test_inferaugassign_picking_parent_instead_of_stmt() -> None:
     code = """
     from collections import namedtuple
     SomeClass = namedtuple('SomeClass', ['name'])
     items = [SomeClass(name='some name')]
@@ -6641,15 +6659,15 @@
     test_dict = {"proxy" : {"auth" : "", "bla" : "f"}}
 
     foo = test_dict['proxy']
     replace(a, **test_dict['proxy']) # This fails
     """
     node = extract_node(code)
     # Reproduces only with safe_infer()
-    assert helpers.safe_infer(node) is None
+    assert util.safe_infer(node) is None
 
 
 @pytest.mark.skipif(
     not PY39_PLUS,
     reason="Exact inference with dataclasses (replace function) in python3.9",
 )
 def test_dataclasses_subscript_inference_recursion_error_39():
@@ -6664,15 +6682,15 @@
     a = ProxyConfig("")
     test_dict = {"proxy" : {"auth" : "", "bla" : "f"}}
 
     foo = test_dict['proxy']
     replace(a, **test_dict['proxy']) # This fails
     """
     node = extract_node(code)
-    infer_val = helpers.safe_infer(node)
+    infer_val = util.safe_infer(node)
     assert isinstance(infer_val, Instance)
     assert infer_val.pytype() == ".ProxyConfig"
 
 
 def test_self_reference_infer_does_not_trigger_recursion_error() -> None:
     # Prevents https://github.com/pylint-dev/pylint/issues/1285
     code = """
```

### Comparing `astroid-3.0.0a5/tests/test_inference_calls.py` & `astroid-3.0.0a6/tests/test_inference_calls.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/tests/test_lookup.py` & `astroid-3.0.0a6/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/tests/test_manager.py` & `astroid-3.0.0a6/tests/test_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,33 +317,33 @@
         self.assertEqual(ast.name, "unittest")
         self.assertIn("unittest", self.manager.astroid_cache)
 
     def test_ast_from_class(self) -> None:
         ast = self.manager.ast_from_class(int)
         self.assertEqual(ast.name, "int")
         self.assertEqual(ast.parent.frame().name, "builtins")
-        self.assertEqual(ast.parent.frame(future=True).name, "builtins")
+        self.assertEqual(ast.parent.frame().name, "builtins")
 
         ast = self.manager.ast_from_class(object)
         self.assertEqual(ast.name, "object")
         self.assertEqual(ast.parent.frame().name, "builtins")
-        self.assertEqual(ast.parent.frame(future=True).name, "builtins")
+        self.assertEqual(ast.parent.frame().name, "builtins")
         self.assertIn("__setattr__", ast)
 
     def test_ast_from_class_with_module(self) -> None:
         """Check if the method works with the module name."""
         ast = self.manager.ast_from_class(int, int.__module__)
         self.assertEqual(ast.name, "int")
         self.assertEqual(ast.parent.frame().name, "builtins")
-        self.assertEqual(ast.parent.frame(future=True).name, "builtins")
+        self.assertEqual(ast.parent.frame().name, "builtins")
 
         ast = self.manager.ast_from_class(object, object.__module__)
         self.assertEqual(ast.name, "object")
         self.assertEqual(ast.parent.frame().name, "builtins")
-        self.assertEqual(ast.parent.frame(future=True).name, "builtins")
+        self.assertEqual(ast.parent.frame().name, "builtins")
         self.assertIn("__setattr__", ast)
 
     def test_ast_from_class_attr_error(self) -> None:
         """Give a wrong class at the ast_from_class method."""
         self.assertRaises(AstroidBuildingError, self.manager.ast_from_class, None)
 
     def test_failed_import_hooks(self) -> None:
@@ -405,15 +405,15 @@
         second_built = second_manager.ast_from_module_name("builtins")
         self.assertIs(built, second_built)
 
 
 class ClearCacheTest(unittest.TestCase):
     def test_clear_cache_clears_other_lru_caches(self) -> None:
         lrus = (
-            astroid.nodes.node_classes.LookupMixIn.lookup,
+            astroid.nodes._base_nodes.LookupMixIn.lookup,
             astroid.modutils._cache_normalize_path_,
             util.is_namespace,
             astroid.interpreter.objectmodel.ObjectModel.attributes,
             ClassDef._metaclass_lookup_attribute,
         )
 
         # Get a baseline for the size of the cache after simply calling bootstrap()
```

### Comparing `astroid-3.0.0a5/tests/test_modutils.py` & `astroid-3.0.0a6/tests/test_modutils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/tests/test_nodes.py` & `astroid-3.0.0a6/tests/test_nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     builder,
     nodes,
     parse,
     test_utils,
     transforms,
     util,
 )
-from astroid.const import PY310_PLUS, Context
+from astroid.const import PY310_PLUS, PY312_PLUS, Context
 from astroid.context import InferenceContext
 from astroid.exceptions import (
     AstroidBuildingError,
     AstroidSyntaxError,
     AttributeInferenceError,
     ParentMissingError,
     StatementMissing,
@@ -275,14 +275,41 @@
 
     @staticmethod
     def test_as_string_unknown() -> None:
         assert nodes.Unknown().as_string() == "Unknown.Unknown()"
         assert nodes.Unknown(lineno=1, col_offset=0).as_string() == "Unknown.Unknown()"
 
 
+@pytest.mark.skipif(not PY312_PLUS, reason="Uses 3.12 type param nodes")
+class AsStringTypeParamNodes(unittest.TestCase):
+    @staticmethod
+    def test_as_string_type_alias() -> None:
+        ast = abuilder.string_build("type Point = tuple[float, float]")
+        type_alias = ast.body[0]
+        assert type_alias.as_string().strip() == "Point"
+
+    @staticmethod
+    def test_as_string_type_var() -> None:
+        ast = abuilder.string_build("type Point[T] = tuple[float, float]")
+        type_var = ast.body[0].type_params[0]
+        assert type_var.as_string().strip() == "T"
+
+    @staticmethod
+    def test_as_string_type_var_tuple() -> None:
+        ast = abuilder.string_build("type Alias[*Ts] = tuple[*Ts]")
+        type_var_tuple = ast.body[0].type_params[0]
+        assert type_var_tuple.as_string().strip() == "*Ts"
+
+    @staticmethod
+    def test_as_string_param_spec() -> None:
+        ast = abuilder.string_build("type Alias[**P] = Callable[P, int]")
+        param_spec = ast.body[0].type_params[0]
+        assert param_spec.as_string().strip() == "P"
+
+
 class _NodeTest(unittest.TestCase):
     """Test transformation of If Node."""
 
     CODE = ""
 
     @property
     def astroid(self) -> Module:
@@ -537,27 +564,27 @@
     def _test(self, value: Any) -> None:
         node = nodes.const_factory(value)
         self.assertIsInstance(node._proxied, nodes.ClassDef)
         self.assertEqual(node._proxied.name, value.__class__.__name__)
         self.assertIs(node.value, value)
         self.assertTrue(node._proxied.parent)
         self.assertEqual(node._proxied.root().name, value.__class__.__module__)
-        with self.assertRaises(AttributeError):
+        with self.assertRaises(StatementMissing):
             with pytest.warns(DeprecationWarning) as records:
-                node.statement()
+                node.statement(future=True)
                 assert len(records) == 1
         with self.assertRaises(StatementMissing):
-            node.statement(future=True)
+            node.statement()
 
-        with self.assertRaises(AttributeError):
+        with self.assertRaises(ParentMissingError):
             with pytest.warns(DeprecationWarning) as records:
-                node.frame()
+                node.frame(future=True)
                 assert len(records) == 1
         with self.assertRaises(ParentMissingError):
-            node.frame(future=True)
+            node.frame()
 
     def test_none(self) -> None:
         self._test(None)
 
     def test_bool(self) -> None:
         self._test(True)
 
@@ -637,43 +664,43 @@
                 pass
 
             COMPREHENSION = [y for i in (1, 2) if (y := i ** 2)]
         """
         )
         function = module.body[0]
         assert function.args.frame() == function
-        assert function.args.frame(future=True) == function
+        assert function.args.frame() == function
 
         function_two = module.body[1]
         assert function_two.args.args[0].frame() == function_two
-        assert function_two.args.args[0].frame(future=True) == function_two
+        assert function_two.args.args[0].frame() == function_two
+        assert function_two.args.args[1].frame() == function_two
         assert function_two.args.args[1].frame() == function_two
-        assert function_two.args.args[1].frame(future=True) == function_two
         assert function_two.args.defaults[0].frame() == module
-        assert function_two.args.defaults[0].frame(future=True) == module
+        assert function_two.args.defaults[0].frame() == module
 
         inherited_class = module.body[3]
         assert inherited_class.keywords[0].frame() == inherited_class
-        assert inherited_class.keywords[0].frame(future=True) == inherited_class
+        assert inherited_class.keywords[0].frame() == inherited_class
+        assert inherited_class.keywords[0].value.frame() == module
         assert inherited_class.keywords[0].value.frame() == module
-        assert inherited_class.keywords[0].value.frame(future=True) == module
 
         lambda_assignment = module.body[4].value
         assert lambda_assignment.args.args[0].frame() == lambda_assignment
-        assert lambda_assignment.args.args[0].frame(future=True) == lambda_assignment
+        assert lambda_assignment.args.args[0].frame() == lambda_assignment
+        assert lambda_assignment.args.defaults[0].frame() == module
         assert lambda_assignment.args.defaults[0].frame() == module
-        assert lambda_assignment.args.defaults[0].frame(future=True) == module
 
         lambda_named_expr = module.body[5].args.defaults[0]
         assert lambda_named_expr.value.args.defaults[0].frame() == module
-        assert lambda_named_expr.value.args.defaults[0].frame(future=True) == module
+        assert lambda_named_expr.value.args.defaults[0].frame() == module
 
         comprehension = module.body[6].value
         assert comprehension.generators[0].ifs[0].frame() == module
-        assert comprehension.generators[0].ifs[0].frame(future=True) == module
+        assert comprehension.generators[0].ifs[0].frame() == module
 
     @staticmethod
     def test_scope() -> None:
         """Test if the scope of NamedExpr is correctly set for certain types
         of parent nodes.
         """
         module = builder.parse(
@@ -1885,30 +1912,32 @@
 
 
 @pytest.mark.parametrize(
     "node",
     [
         node
         for node in astroid.nodes.ALL_NODE_CLASSES
-        if node.__name__
-        not in ["_BaseContainer", "BaseContainer", "NodeNG", "const_factory"]
+        if node.__name__ not in ["BaseContainer", "NodeNG", "const_factory"]
     ],
 )
 @pytest.mark.filterwarnings("error")
 def test_str_repr_no_warnings(node):
     parameters = inspect.signature(node.__init__).parameters
 
     args = {}
     for name, param_type in parameters.items():
         if name == "self":
             continue
 
         if "int" in param_type.annotation:
             args[name] = random.randint(0, 50)
-        elif "NodeNG" in param_type.annotation:
+        elif (
+            "NodeNG" in param_type.annotation
+            or "SuccessfulInferenceResult" in param_type.annotation
+        ):
             args[name] = nodes.Unknown()
         elif "str" in param_type.annotation:
             args[name] = ""
         else:
             args[name] = None
 
     test_node = node(**args)
```

### Comparing `astroid-3.0.0a5/tests/test_nodes_lineno.py` & `astroid-3.0.0a6/tests/test_nodes_lineno.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import textwrap
 
 import pytest
 
 import astroid
 from astroid import builder, nodes
-from astroid.const import IS_PYPY, PY38, PY39_PLUS, PY310_PLUS
+from astroid.const import IS_PYPY, PY38, PY39_PLUS, PY310_PLUS, PY312_PLUS
 
 
 @pytest.mark.skipif(
     not (PY38 and IS_PYPY),
     reason="end_lineno and end_col_offset were added in PY38",
 )
 class TestEndLinenoNotSet:
@@ -973,46 +973,70 @@
         assert isinstance(ast_nodes, list) and len(ast_nodes) == 2
 
         s1 = ast_nodes[0]
         assert isinstance(s1, nodes.JoinedStr)
         assert isinstance(s1.values[0], nodes.Const)
         assert (s1.lineno, s1.col_offset) == (1, 0)
         assert (s1.end_lineno, s1.end_col_offset) == (1, 29)
-        assert (s1.values[0].lineno, s1.values[0].col_offset) == (1, 0)
-        assert (s1.values[0].end_lineno, s1.values[0].end_col_offset) == (1, 29)
+        if PY312_PLUS:
+            assert (s1.values[0].lineno, s1.values[0].col_offset) == (1, 2)
+            assert (s1.values[0].end_lineno, s1.values[0].end_col_offset) == (1, 15)
+        else:
+            # Bug in Python 3.11
+            # https://github.com/python/cpython/issues/81639
+            assert (s1.values[0].lineno, s1.values[0].col_offset) == (1, 0)
+            assert (s1.values[0].end_lineno, s1.values[0].end_col_offset) == (1, 29)
 
         s2 = s1.values[1]
         assert isinstance(s2, nodes.FormattedValue)
-        assert (s2.lineno, s2.col_offset) == (1, 0)
-        assert (s2.end_lineno, s2.end_col_offset) == (1, 29)
+        if PY312_PLUS:
+            assert (s2.lineno, s2.col_offset) == (1, 15)
+            assert (s2.end_lineno, s2.end_col_offset) == (1, 28)
+        else:
+            assert (s2.lineno, s2.col_offset) == (1, 0)
+            assert (s2.end_lineno, s2.end_col_offset) == (1, 29)
+
         assert isinstance(s2.value, nodes.Const)  # 42.1234
         if PY39_PLUS:
             assert (s2.value.lineno, s2.value.col_offset) == (1, 16)
             assert (s2.value.end_lineno, s2.value.end_col_offset) == (1, 23)
         else:
             # Bug in Python 3.8
             # https://bugs.python.org/issue44885
             assert (s2.value.lineno, s2.value.col_offset) == (1, 1)
             assert (s2.value.end_lineno, s2.value.end_col_offset) == (1, 8)
-        assert isinstance(s2.format_spec, nodes.JoinedStr)  # '02d'
-        assert (s2.format_spec.lineno, s2.format_spec.col_offset) == (1, 0)
-        assert (s2.format_spec.end_lineno, s2.format_spec.end_col_offset) == (1, 29)
+        assert isinstance(s2.format_spec, nodes.JoinedStr)  # ':02d'
+        if PY312_PLUS:
+            assert (s2.format_spec.lineno, s2.format_spec.col_offset) == (1, 23)
+            assert (s2.format_spec.end_lineno, s2.format_spec.end_col_offset) == (1, 27)
+        else:
+            assert (s2.format_spec.lineno, s2.format_spec.col_offset) == (1, 0)
+            assert (s2.format_spec.end_lineno, s2.format_spec.end_col_offset) == (1, 29)
 
         s3 = ast_nodes[1]
         assert isinstance(s3, nodes.JoinedStr)
         assert isinstance(s3.values[0], nodes.Const)
         assert (s3.lineno, s3.col_offset) == (2, 0)
         assert (s3.end_lineno, s3.end_col_offset) == (2, 17)
-        assert (s3.values[0].lineno, s3.values[0].col_offset) == (2, 0)
-        assert (s3.values[0].end_lineno, s3.values[0].end_col_offset) == (2, 17)
+        if PY312_PLUS:
+            assert (s3.values[0].lineno, s3.values[0].col_offset) == (2, 2)
+            assert (s3.values[0].end_lineno, s3.values[0].end_col_offset) == (2, 15)
+        else:
+            assert (s3.values[0].lineno, s3.values[0].col_offset) == (2, 0)
+            assert (s3.values[0].end_lineno, s3.values[0].end_col_offset) == (2, 17)
 
         s4 = s3.values[1]
         assert isinstance(s4, nodes.FormattedValue)
-        assert (s4.lineno, s4.col_offset) == (2, 0)
-        assert (s4.end_lineno, s4.end_col_offset) == (2, 17)
+        if PY312_PLUS:
+            assert (s4.lineno, s4.col_offset) == (2, 9)
+            assert (s4.end_lineno, s4.end_col_offset) == (2, 16)
+        else:
+            assert (s4.lineno, s4.col_offset) == (2, 0)
+            assert (s4.end_lineno, s4.end_col_offset) == (2, 17)
+
         assert isinstance(s4.value, nodes.Name)  # 'name'
         if PY39_PLUS:
             assert (s4.value.lineno, s4.value.col_offset) == (2, 10)
             assert (s4.value.end_lineno, s4.value.end_col_offset) == (2, 14)
         else:
             # Bug in Python 3.8
             # https://bugs.python.org/issue44885
```

### Comparing `astroid-3.0.0a5/tests/test_nodes_position.py` & `astroid-3.0.0a6/tests/test_nodes_position.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/tests/test_object_model.py` & `astroid-3.0.0a6/tests/test_object_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -585,14 +585,18 @@
         self.assertIsInstance(annotations, astroid.Dict)
 
         self.assertIsInstance(annotations.getitem(astroid.Const("a")), astroid.Const)
         self.assertEqual(annotations.getitem(astroid.Const("a")).value, 1)
         self.assertEqual(annotations.getitem(astroid.Const("b")).value, 2)
         self.assertEqual(annotations.getitem(astroid.Const("c")).value, 3)
 
+    def test_is_not_lambda(self):
+        ast_node = builder.extract_node("def func(): pass")
+        self.assertIs(ast_node.is_lambda, False)
+
 
 class TestContextManagerModel:
     def test_model(self) -> None:
         """We use a generator to test this model."""
         ast_nodes = builder.extract_node(
             """
         def test():
```

### Comparing `astroid-3.0.0a5/tests/test_objects.py` & `astroid-3.0.0a6/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/tests/test_protocols.py` & `astroid-3.0.0a6/tests/test_protocols.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,14 +275,21 @@
         parsed = extract_node("15 ** 20220609")
         assert parsed.inferred() == [Uninferable]
 
         # Test a pathological case (more realistic: None as naive inference result)
         parsed = extract_node("None ** 2")
         assert parsed.inferred() == [Uninferable]
 
+    @staticmethod
+    def test_uninferable_list_multiplication() -> None:
+        """Attempting to calculate the result is prohibitively expensive."""
+        parsed = extract_node("[0] * 123456789")
+        element = parsed.inferred()[0].elts[0]
+        assert element.value is Uninferable
+
 
 def test_named_expr_inference() -> None:
     code = """
     if (a := 2) == 2:
         a #@
```

### Comparing `astroid-3.0.0a5/tests/test_python3.py` & `astroid-3.0.0a6/tests/test_python3.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/tests/test_raw_building.py` & `astroid-3.0.0a6/tests/test_raw_building.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import _io
 import pytest
 
 import tests.testdata.python3.data.fake_module_with_broken_getattr as fm_getattr
 import tests.testdata.python3.data.fake_module_with_warnings as fm
 from astroid.builder import AstroidBuilder
-from astroid.const import IS_PYPY
+from astroid.const import IS_PYPY, PY312_PLUS
 from astroid.raw_building import (
     attach_dummy_node,
     build_class,
     build_from_import,
     build_function,
     build_module,
 )
@@ -82,23 +82,24 @@
     def test_build_from_import(self) -> None:
         names = ["exceptions, inference, inspector"]
         node = build_from_import("astroid", names)
         self.assertEqual(len(names), len(node.names))
 
     @unittest.skipIf(IS_PYPY, "Only affects CPython")
     def test_io_is__io(self):
-        # _io module calls itself io. This leads
+        # _io module calls itself io before Python 3.12. This leads
         # to cyclic dependencies when astroid tries to resolve
         # what io.BufferedReader is. The code that handles this
         # is in astroid.raw_building.imported_member, which verifies
         # the true name of the module.
         builder = AstroidBuilder()
         module = builder.inspect_build(_io)
         buffered_reader = module.getattr("BufferedReader")[0]
-        self.assertEqual(buffered_reader.root().name, "io")
+        expected = "_io" if PY312_PLUS else "io"
+        self.assertEqual(buffered_reader.root().name, expected)
 
     def test_build_function_deepinspect_deprecation(self) -> None:
         # Tests https://github.com/pylint-dev/astroid/issues/1717
         # When astroid deep inspection of modules raises
         # attribute errors when getting all attributes
         # Create a mock module to simulate a Cython module
         m = types.ModuleType("test")
```

### Comparing `astroid-3.0.0a5/tests/test_regrtest.py` & `astroid-3.0.0a6/tests/test_regrtest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/tests/test_scoped_nodes.py` & `astroid-3.0.0a6/tests/test_scoped_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,37 +4,39 @@
 
 """Tests for specific behaviour of astroid scoped nodes (i.e. module, class and
 function).
 """
 
 from __future__ import annotations
 
-import datetime
+import difflib
 import os
 import sys
 import textwrap
 import unittest
 from functools import partial
 from typing import Any
+from unittest.mock import patch
 
 import pytest
 
 from astroid import (
     MANAGER,
     builder,
     extract_node,
     nodes,
     objects,
     parse,
     test_utils,
     util,
 )
 from astroid.bases import BoundMethod, Generator, Instance, UnboundMethod
-from astroid.const import IS_PYPY, PY38
+from astroid.const import IS_PYPY, PY38, WIN32
 from astroid.exceptions import (
+    AstroidBuildingError,
     AttributeInferenceError,
     DuplicateBasesError,
     InconsistentMroError,
     InferenceError,
     MroError,
     NameInferenceError,
     NoDefault,
@@ -240,14 +242,27 @@
             self.assertEqual(m.name, "package")
             inferred = list(astroid.igetattr("pouet"))
             self.assertEqual(len(inferred), 1)
             self.assertEqual(inferred[0].name, "package.subpackage")
         finally:
             del sys.path[0]
 
+    @patch(
+        "astroid.nodes.scoped_nodes.scoped_nodes.AstroidManager.ast_from_module_name"
+    )
+    def test_import_unavailable_module(self, mock) -> None:
+        unavailable_modname = "posixpath" if WIN32 else "ntpath"
+        module = builder.parse(f"import {unavailable_modname}")
+        mock.side_effect = AstroidBuildingError
+
+        with pytest.raises(AstroidBuildingError):
+            module.import_module(unavailable_modname)
+
+        mock.assert_called_once()
+
     def test_file_stream_in_memory(self) -> None:
         data = """irrelevant_variable is irrelevant"""
         astroid = builder.parse(data, "in_memory")
         with astroid.stream() as stream:
             self.assertEqual(stream.read().decode(), data)
 
     def test_file_stream_physical(self) -> None:
@@ -364,15 +379,15 @@
         # self.assertIsInstance(func.mularg_class('args'), nodes.Tuple)
         # self.assertIsInstance(func.mularg_class('kwargs'), nodes.Dict)
         # self.assertIsNone(func.mularg_class('base'))
 
     def test_navigation(self) -> None:
         function = self.module["global_access"]
         self.assertEqual(function.statement(), function)
-        self.assertEqual(function.statement(future=True), function)
+        self.assertEqual(function.statement(), function)
         l_sibling = function.previous_sibling()
         # check taking parent if child is not a stmt
         self.assertIsInstance(l_sibling, nodes.Assign)
         child = function.args.args[0]
         self.assertIs(l_sibling, child.previous_sibling())
         r_sibling = function.next_sibling()
         self.assertIsInstance(r_sibling, nodes.ClassDef)
@@ -525,14 +540,18 @@
 
         code_with_kwonly_args = "def f(a, b, *args, c=None, d=None, **kwargs): pass"
         astroid = builder.parse(code_with_kwonly_args, __name__)
         self.assertEqual(
             astroid["f"].argnames(), ["a", "b", "args", "c", "d", "kwargs"]
         )
 
+    def test_argnames_lambda(self) -> None:
+        lambda_node = extract_node("lambda a, b, c, *args, **kwargs: ...")
+        self.assertEqual(lambda_node.argnames(), ["a", "b", "c", "args", "kwargs"])
+
     def test_positional_only_argnames(self) -> None:
         code = "def f(a, b, /, c=None, *args, d, **kwargs): pass"
         astroid = builder.parse(code, __name__)
         self.assertEqual(
             astroid["f"].argnames(), ["a", "b", "c", "args", "d", "kwargs"]
         )
 
@@ -1045,15 +1064,15 @@
             self.assertRaises(AttributeInferenceError, inst.getattr, "__name__")
             self.assertEqual(len(inst.getattr("__dict__")), 1)
             self.assertEqual(len(inst.getattr("__doc__")), 1)
 
     def test_navigation(self) -> None:
         klass = self.module["YO"]
         self.assertEqual(klass.statement(), klass)
-        self.assertEqual(klass.statement(future=True), klass)
+        self.assertEqual(klass.statement(), klass)
         l_sibling = klass.previous_sibling()
         self.assertTrue(isinstance(l_sibling, nodes.FunctionDef), l_sibling)
         self.assertEqual(l_sibling.name, "global_access")
         r_sibling = klass.next_sibling()
         self.assertIsInstance(r_sibling, nodes.ClassDef)
         self.assertEqual(r_sibling.name, "YOUPI")
 
@@ -2133,16 +2152,16 @@
         self.assertTrue(module["Getattr"].has_dynamic_getattr())
         self.assertTrue(module["Getattribute"].has_dynamic_getattr())
         self.assertTrue(module["ParentGetattr"].has_dynamic_getattr())
 
         # Test that objects analyzed through the live introspection
         # aren't considered to have dynamic getattr implemented.
         astroid_builder = builder.AstroidBuilder()
-        module = astroid_builder.module_build(datetime)
-        self.assertFalse(module["timedelta"].has_dynamic_getattr())
+        module = astroid_builder.module_build(difflib)
+        self.assertFalse(module["SequenceMatcher"].has_dynamic_getattr())
 
     def test_duplicate_bases_namedtuple(self) -> None:
         module = builder.parse(
             """
         import collections
         _A = collections.namedtuple('A', 'a')
 
@@ -2805,41 +2824,41 @@
                     pass
 
             VAR = lambda y = (named_expr := "walrus"): print(y)
         """
         )
         function = module.body[0]
         assert function.frame() == function
-        assert function.frame(future=True) == function
+        assert function.frame() == function
+        assert function.body[0].frame() == function
         assert function.body[0].frame() == function
-        assert function.body[0].frame(future=True) == function
 
         class_node = module.body[1]
         assert class_node.frame() == class_node
-        assert class_node.frame(future=True) == class_node
+        assert class_node.frame() == class_node
         assert class_node.body[0].frame() == class_node
-        assert class_node.body[0].frame(future=True) == class_node
+        assert class_node.body[0].frame() == class_node
+        assert class_node.body[1].frame() == class_node.body[1]
         assert class_node.body[1].frame() == class_node.body[1]
-        assert class_node.body[1].frame(future=True) == class_node.body[1]
 
         lambda_assignment = module.body[2].value
         assert lambda_assignment.args.args[0].frame() == lambda_assignment
-        assert lambda_assignment.args.args[0].frame(future=True) == lambda_assignment
+        assert lambda_assignment.args.args[0].frame() == lambda_assignment
 
         assert module.frame() == module
-        assert module.frame(future=True) == module
+        assert module.frame() == module
 
     @staticmethod
     def test_non_frame_node():
         """Test if the frame of non frame nodes is set correctly."""
         module = builder.parse(
             """
             VAR_ONE = 1
 
             VAR_TWO = [x for x in range(1)]
         """
         )
         assert module.body[0].frame() == module
-        assert module.body[0].frame(future=True) == module
+        assert module.body[0].frame() == module
 
         assert module.body[1].value.locals["x"][0].frame() == module
-        assert module.body[1].value.locals["x"][0].frame(future=True) == module
+        assert module.body[1].value.locals["x"][0].frame() == module
```

### Comparing `astroid-3.0.0a5/tests/test_stdlib.py` & `astroid-3.0.0a6/tests/test_stdlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/tests/test_transforms.py` & `astroid-3.0.0a6/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a5/tests/test_utils.py` & `astroid-3.0.0a6/tests/test_utils.py`

 * *Files identical despite different names*

