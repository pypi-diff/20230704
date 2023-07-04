# Comparing `tmp/pyglove-0.3.1.dev20230702.tar.gz` & `tmp/pyglove-0.3.1.dev20230703.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglove-0.3.1.dev20230702.tar", last modified: Sun Jul  2 08:06:38 2023, max compression
+gzip compressed data, was "pyglove-0.3.1.dev20230703.tar", last modified: Mon Jul  3 08:07:26 2023, max compression
```

## Comparing `pyglove-0.3.1.dev20230702.tar` & `pyglove-0.3.1.dev20230703.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:06:38.832692 pyglove-0.3.1.dev20230702/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-02 08:06:38.832692 pyglove-0.3.1.dev20230702/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-02 08:06:36.000000 pyglove-0.3.1.dev20230702/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:06:38.808692 pyglove-0.3.1.dev20230702/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:06:38.808692 pyglove-0.3.1.dev20230702/pyglove/core/
--rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:06:38.808692 pyglove-0.3.1.dev20230702/pyglove/core/detouring/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/detouring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/detouring/class_detour.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/detouring/class_detour_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:06:38.812692 pyglove-0.3.1.dev20230702/pyglove/core/geno/
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/geno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/geno/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/geno/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/geno/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/geno/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/geno/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/geno/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/geno/deduping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/geno/deduping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/geno/dna_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/geno/dna_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/geno/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/geno/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/geno/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/geno/random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/geno/space.py
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/geno/space_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/geno/sweeping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/geno/sweeping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:06:38.812692 pyglove-0.3.1.dev20230702/pyglove/core/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/hyper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/hyper/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/hyper/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/hyper/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/hyper/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/hyper/derived.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/hyper/derived_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/hyper/dynamic_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/hyper/dynamic_evaluation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/hyper/evolvable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/hyper/evolvable_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/hyper/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/hyper/iter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/hyper/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/hyper/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/hyper/object_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/hyper/object_template_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/logging_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:06:38.816692 pyglove-0.3.1.dev20230702/pyglove/core/object_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/object_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/object_utils/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/object_utils/codegen_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/object_utils/common_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/object_utils/common_traits_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/object_utils/docstr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/object_utils/docstr_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/object_utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/object_utils/formatting_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/object_utils/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/object_utils/hierarchical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/object_utils/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/object_utils/missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/object_utils/thread_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/object_utils/thread_local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/object_utils/value_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/object_utils/value_location_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:06:38.816692 pyglove-0.3.1.dev20230702/pyglove/core/patching/
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/patching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/patching/object_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/patching/object_factory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/patching/pattern_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/patching/pattern_based_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/patching/rule_based.py
--rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/patching/rule_based_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:06:38.820692 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    77681 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/boilerplate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22447 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/class_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/class_wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/compounding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/compounding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/contextual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/contextual_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    62550 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/dict_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/diff_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/flags_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23955 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/functor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29174 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/functor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28899 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    55862 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    35049 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    83341 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/origin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/pure_symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/symbolize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/symbolic/symbolize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:06:38.820692 pyglove-0.3.1.dev20230702/pyglove/core/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/tuning/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/tuning/backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/tuning/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/tuning/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/tuning/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/tuning/protocols_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/tuning/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/tuning/sample_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:06:38.824692 pyglove-0.3.1.dev20230702/pyglove/core/typing/
--rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/typing/annotation_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/typing/annotation_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/typing/callable_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/typing/callable_ext_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/typing/callable_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/typing/callable_signature_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    49538 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/typing/class_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/typing/class_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/typing/class_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/typing/class_schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/typing/custom_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/typing/key_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/typing/key_specs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/typing/pytype_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/typing/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/typing/type_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/typing/typed_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/typing/typed_missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    79567 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/typing/value_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)   103891 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/core/typing/value_specs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:06:38.824692 pyglove-0.3.1.dev20230702/pyglove/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:06:38.828692 pyglove-0.3.1.dev20230702/pyglove/ext/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/early_stopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/early_stopping/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/early_stopping/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/early_stopping/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/early_stopping/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:06:38.828692 pyglove-0.3.1.dev20230702/pyglove/ext/evolution/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/evolution/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/evolution/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/evolution/hill_climb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/evolution/hill_climb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/evolution/mutators.py
--rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/evolution/mutators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/evolution/neat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/evolution/neat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/evolution/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/evolution/nsga2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/evolution/recombinators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/evolution/recombinators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/evolution/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/evolution/regularized_evolution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/evolution/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/evolution/selectors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/evolution/where.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/evolution/where_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:06:38.832692 pyglove-0.3.1.dev20230702/pyglove/ext/mutfun/
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/mutfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/mutfun/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/mutfun/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/mutfun/basic_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/mutfun/basic_ops_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:06:38.832692 pyglove-0.3.1.dev20230702/pyglove/ext/scalars/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/scalars/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/scalars/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/scalars/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/scalars/maths_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/scalars/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/scalars/randoms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/scalars/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/pyglove/ext/scalars/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:06:38.808692 pyglove-0.3.1.dev20230702/pyglove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-02 08:06:38.000000 pyglove-0.3.1.dev20230702/pyglove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-02 08:06:38.000000 pyglove-0.3.1.dev20230702/pyglove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 08:06:38.000000 pyglove-0.3.1.dev20230702/pyglove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 08:06:38.000000 pyglove-0.3.1.dev20230702/pyglove.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-02 08:06:38.000000 pyglove-0.3.1.dev20230702/pyglove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 08:06:38.832692 pyglove-0.3.1.dev20230702/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-02 08:06:23.000000 pyglove-0.3.1.dev20230702/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:07:26.764699 pyglove-0.3.1.dev20230703/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-03 08:07:26.764699 pyglove-0.3.1.dev20230703/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-03 08:07:25.000000 pyglove-0.3.1.dev20230703/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:07:26.748699 pyglove-0.3.1.dev20230703/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:07:26.748699 pyglove-0.3.1.dev20230703/pyglove/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:07:26.748699 pyglove-0.3.1.dev20230703/pyglove/core/detouring/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/detouring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/detouring/class_detour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/detouring/class_detour_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:07:26.752699 pyglove-0.3.1.dev20230703/pyglove/core/geno/
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/geno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/geno/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/geno/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/geno/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/geno/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/geno/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/geno/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/geno/deduping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/geno/deduping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/geno/dna_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/geno/dna_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/geno/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/geno/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/geno/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/geno/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/geno/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/geno/space_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/geno/sweeping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/geno/sweeping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:07:26.752699 pyglove-0.3.1.dev20230703/pyglove/core/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/hyper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/hyper/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/hyper/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/hyper/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/hyper/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/hyper/derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/hyper/derived_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/hyper/dynamic_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/hyper/dynamic_evaluation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/hyper/evolvable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/hyper/evolvable_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/hyper/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/hyper/iter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/hyper/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/hyper/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/hyper/object_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/hyper/object_template_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/logging_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:07:26.752699 pyglove-0.3.1.dev20230703/pyglove/core/object_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/object_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/object_utils/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/object_utils/codegen_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/object_utils/common_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/object_utils/common_traits_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/object_utils/docstr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/object_utils/docstr_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/object_utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/object_utils/formatting_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/object_utils/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/object_utils/hierarchical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/object_utils/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/object_utils/missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/object_utils/thread_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/object_utils/thread_local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/object_utils/value_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/object_utils/value_location_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:07:26.752699 pyglove-0.3.1.dev20230703/pyglove/core/patching/
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/patching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/patching/object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/patching/object_factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/patching/pattern_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/patching/pattern_based_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/patching/rule_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/patching/rule_based_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:07:26.756699 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77862 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/boilerplate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22447 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/class_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/class_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/compounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/compounding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/contextual_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34189 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62550 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/dict_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/diff_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/flags_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23955 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/functor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29174 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/functor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28899 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55862 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35049 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83341 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/origin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/pure_symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/symbolize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/symbolic/symbolize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:07:26.756699 pyglove-0.3.1.dev20230703/pyglove/core/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/tuning/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/tuning/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/tuning/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/tuning/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/tuning/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/tuning/protocols_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/tuning/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/tuning/sample_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:07:26.760699 pyglove-0.3.1.dev20230703/pyglove/core/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/typing/annotation_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/typing/annotation_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/typing/callable_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/typing/callable_ext_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/typing/callable_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/typing/callable_signature_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49558 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/typing/class_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/typing/class_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/typing/class_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/typing/class_schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/typing/custom_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/typing/key_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/typing/key_specs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/typing/pytype_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/typing/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/typing/type_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/typing/typed_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/typing/typed_missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79584 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/typing/value_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103891 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/core/typing/value_specs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:07:26.760699 pyglove-0.3.1.dev20230703/pyglove/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:07:26.760699 pyglove-0.3.1.dev20230703/pyglove/ext/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/early_stopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/early_stopping/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/early_stopping/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/early_stopping/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/early_stopping/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:07:26.760699 pyglove-0.3.1.dev20230703/pyglove/ext/evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/evolution/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/evolution/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/evolution/hill_climb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/evolution/hill_climb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/evolution/mutators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/evolution/mutators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/evolution/neat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/evolution/neat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/evolution/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/evolution/nsga2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/evolution/recombinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/evolution/recombinators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/evolution/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/evolution/regularized_evolution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/evolution/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/evolution/selectors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/evolution/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/evolution/where_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:07:26.760699 pyglove-0.3.1.dev20230703/pyglove/ext/mutfun/
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/mutfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/mutfun/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/mutfun/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/mutfun/basic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/mutfun/basic_ops_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:07:26.764699 pyglove-0.3.1.dev20230703/pyglove/ext/scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/scalars/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/scalars/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/scalars/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/scalars/maths_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/scalars/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/scalars/randoms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/scalars/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/pyglove/ext/scalars/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:07:26.748699 pyglove-0.3.1.dev20230703/pyglove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-03 08:07:26.000000 pyglove-0.3.1.dev20230703/pyglove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-03 08:07:26.000000 pyglove-0.3.1.dev20230703/pyglove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:07:26.000000 pyglove-0.3.1.dev20230703/pyglove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 08:07:26.000000 pyglove-0.3.1.dev20230703/pyglove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 08:07:26.000000 pyglove-0.3.1.dev20230703/pyglove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 08:07:26.764699 pyglove-0.3.1.dev20230703/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-03 08:07:13.000000 pyglove-0.3.1.dev20230703/setup.py
```

### Comparing `pyglove-0.3.1.dev20230702/LICENSE` & `pyglove-0.3.1.dev20230703/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/PKG-INFO` & `pyglove-0.3.1.dev20230703/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.3.1.dev20230702
+Version: 0.3.1.dev20230703
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.3.1.dev20230702/README.md` & `pyglove-0.3.1.dev20230703/README.md`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/__init__.py` & `pyglove-0.3.1.dev20230703/pyglove/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/__init__.py` & `pyglove-0.3.1.dev20230703/pyglove/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/detouring/__init__.py` & `pyglove-0.3.1.dev20230703/pyglove/core/detouring/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/detouring/class_detour.py` & `pyglove-0.3.1.dev20230703/pyglove/core/detouring/class_detour.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/detouring/class_detour_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/detouring/class_detour_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/geno/__init__.py` & `pyglove-0.3.1.dev20230703/pyglove/core/geno/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/geno/base.py` & `pyglove-0.3.1.dev20230703/pyglove/core/geno/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/geno/base_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/geno/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/geno/categorical.py` & `pyglove-0.3.1.dev20230703/pyglove/core/geno/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/geno/categorical_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/geno/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/geno/custom.py` & `pyglove-0.3.1.dev20230703/pyglove/core/geno/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/geno/custom_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/geno/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/geno/deduping.py` & `pyglove-0.3.1.dev20230703/pyglove/core/geno/deduping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/geno/deduping_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/geno/deduping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/geno/dna_generator.py` & `pyglove-0.3.1.dev20230703/pyglove/core/geno/dna_generator.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/geno/dna_generator_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/geno/dna_generator_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/geno/numerical.py` & `pyglove-0.3.1.dev20230703/pyglove/core/geno/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/geno/numerical_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/geno/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/geno/random.py` & `pyglove-0.3.1.dev20230703/pyglove/core/geno/random.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/geno/random_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/geno/random_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/geno/space.py` & `pyglove-0.3.1.dev20230703/pyglove/core/geno/space.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/geno/space_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/geno/space_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/geno/sweeping.py` & `pyglove-0.3.1.dev20230703/pyglove/core/geno/sweeping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/geno/sweeping_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/geno/sweeping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/hyper/__init__.py` & `pyglove-0.3.1.dev20230703/pyglove/core/hyper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/hyper/base.py` & `pyglove-0.3.1.dev20230703/pyglove/core/hyper/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/hyper/categorical.py` & `pyglove-0.3.1.dev20230703/pyglove/core/hyper/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/hyper/categorical_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/hyper/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/hyper/custom.py` & `pyglove-0.3.1.dev20230703/pyglove/core/hyper/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/hyper/custom_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/hyper/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/hyper/derived.py` & `pyglove-0.3.1.dev20230703/pyglove/core/hyper/derived.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/hyper/derived_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/hyper/derived_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/hyper/dynamic_evaluation.py` & `pyglove-0.3.1.dev20230703/pyglove/core/hyper/dynamic_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/hyper/dynamic_evaluation_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/hyper/dynamic_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/hyper/evolvable.py` & `pyglove-0.3.1.dev20230703/pyglove/core/hyper/evolvable.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/hyper/evolvable_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/hyper/evolvable_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/hyper/iter.py` & `pyglove-0.3.1.dev20230703/pyglove/core/hyper/iter.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/hyper/iter_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/hyper/iter_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/hyper/numerical.py` & `pyglove-0.3.1.dev20230703/pyglove/core/hyper/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/hyper/numerical_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/hyper/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/hyper/object_template.py` & `pyglove-0.3.1.dev20230703/pyglove/core/hyper/object_template.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/hyper/object_template_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/hyper/object_template_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/logging.py` & `pyglove-0.3.1.dev20230703/pyglove/core/logging.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/logging_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/logging_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/object_utils/__init__.py` & `pyglove-0.3.1.dev20230703/pyglove/core/object_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/object_utils/codegen.py` & `pyglove-0.3.1.dev20230703/pyglove/core/object_utils/codegen.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/object_utils/codegen_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/object_utils/codegen_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/object_utils/common_traits.py` & `pyglove-0.3.1.dev20230703/pyglove/core/object_utils/common_traits.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/object_utils/common_traits_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/object_utils/common_traits_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/object_utils/docstr_utils.py` & `pyglove-0.3.1.dev20230703/pyglove/core/object_utils/docstr_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/object_utils/docstr_utils_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/object_utils/docstr_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/object_utils/formatting.py` & `pyglove-0.3.1.dev20230703/pyglove/core/object_utils/formatting.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/object_utils/formatting_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/object_utils/formatting_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/object_utils/hierarchical.py` & `pyglove-0.3.1.dev20230703/pyglove/core/object_utils/hierarchical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/object_utils/hierarchical_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/object_utils/hierarchical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/object_utils/missing.py` & `pyglove-0.3.1.dev20230703/pyglove/core/object_utils/missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/object_utils/missing_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/object_utils/missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/object_utils/thread_local.py` & `pyglove-0.3.1.dev20230703/pyglove/core/object_utils/thread_local.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/object_utils/thread_local_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/object_utils/thread_local_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/object_utils/value_location.py` & `pyglove-0.3.1.dev20230703/pyglove/core/object_utils/value_location.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/object_utils/value_location_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/object_utils/value_location_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/patching/__init__.py` & `pyglove-0.3.1.dev20230703/pyglove/core/patching/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/patching/object_factory.py` & `pyglove-0.3.1.dev20230703/pyglove/core/patching/object_factory.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/patching/object_factory_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/patching/object_factory_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/patching/pattern_based.py` & `pyglove-0.3.1.dev20230703/pyglove/core/patching/pattern_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/patching/pattern_based_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/patching/pattern_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/patching/rule_based.py` & `pyglove-0.3.1.dev20230703/pyglove/core/patching/rule_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/patching/rule_based_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/patching/rule_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/__init__.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/base.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -665,16 +665,18 @@
       path_value_pairs: Optional[Union[
           Dict[
               Union[object_utils.KeyPath, str, int],
               Any],
           Callable]] = None,  # pylint: disable=g-bare-generic
       raise_on_no_change: bool = True,
       skip_notification: Optional[bool] = None,
-      **kwargs) -> 'Symbolic':
+      **kwargs,
+  ) -> 'Symbolic':
     """Mutates the sub-nodes of current object. Please see `rebind`."""
+    assert Symbolic.DictType is not None
     if callable(path_value_pairs):
       path_value_pairs = get_rebind_dict(path_value_pairs, self)
     elif path_value_pairs is None:
       path_value_pairs = {}
     elif isinstance(path_value_pairs, Symbolic.DictType):
       # Rebind work on symbolic form, thus we get their symbol instead of
       # their evaluated value when building the rebind dict.
@@ -2126,14 +2128,15 @@
   Returns:
     Deserialized value, which is
     * pg.Dict for dict.
     * pg.List for list.
     * symbolic.Object for dict with '_type' property.
     * value itself.
   """
+  assert Symbolic.DictType is not None
   if isinstance(json_value, Symbolic):
     return json_value
 
   kwargs.update({
       'allow_partial': allow_partial,
       'root_path': root_path,
   })
@@ -2147,15 +2150,15 @@
                 f'besides \'{object_utils.JSONConvertible.TUPLE_MARKER}\'. '
                 f'Encountered: {json_value}', root_path))
       return tuple([
           from_json(v, allow_partial=allow_partial,
                     root_path=object_utils.KeyPath(i, root_path))
           for i, v in enumerate(json_value[1:])
       ])
-    return Symbolic.ListType(json_value, **kwargs)  # pylint: disable=not-callable
+    return Symbolic.ListType(json_value, **kwargs)  # pytype: disable=not-callable   # pylint: disable=not-callable
   elif isinstance(json_value, dict):
     if object_utils.JSONConvertible.TYPE_NAME_KEY not in json_value:
       return Symbolic.DictType.from_json(json_value, **kwargs)
     type_name = json_value[object_utils.JSONConvertible.TYPE_NAME_KEY]
     cls = object_utils.JSONConvertible.class_from_typename(type_name)
     if cls is None:
       raise TypeError(
@@ -2390,28 +2393,28 @@
       path: object_utils.KeyPath, field: pg_typing.Field, value: Any) -> Any:
     """Transform schema-less List and Dict to symbolic."""
     if isinstance(value, Symbolic):
       return value
     if isinstance(value, dict):
       value_spec = pg_typing.ensure_value_spec(
           field.value, pg_typing.Dict(), path)
-      value = Symbolic.DictType(   # pylint: disable=not-callable
+      value = Symbolic.DictType(   # pytype: disable=not-callable  # pylint: disable=not-callable
           value,
           value_spec=value_spec,
           allow_partial=allow_partial,
           root_path=path,
           # NOTE(daiyip): members are already checked and transformed
           # into final object, thus we simply pass through.
           # This prevents the Dict members from repeated validation
           # and transformation.
           pass_through=True)
     elif isinstance(value, list):
       value_spec = pg_typing.ensure_value_spec(
           field.value, pg_typing.List(pg_typing.Any()), path)
-      value = Symbolic.ListType(   # pylint: disable=not-callable
+      value = Symbolic.ListType(   # pytype: disable=not-callable  # pylint: disable=not-callable
           value,
           value_spec=value_spec,
           allow_partial=allow_partial,
           root_path=path)
     return value
 
   return _fn
```

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/base_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/boilerplate.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/boilerplate.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/boilerplate_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/boilerplate_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/class_wrapper.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/class_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/class_wrapper_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/class_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/compounding.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/compounding.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/compounding_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/compounding_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/contextual.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/contextual.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/contextual_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/contextual_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/dict.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,15 +432,15 @@
   def sym_keys(self) -> Iterator[str]:
     """Iterates the keys of symbolic attributes."""
     if self._value_spec is None or self._value_spec.schema is None:
       for key in super().__iter__():
         yield key
     else:
       traversed = set()
-      for key_spec in self._value_spec.schema.keys():
+      for key_spec in self._value_spec.schema.keys():  # pytype: disable=attribute-error
         if isinstance(key_spec, pg_typing.ConstStrKey) and key_spec in self:
           yield key_spec.text
           traversed.add(key_spec.text)
 
       if len(traversed) < len(self):
         for key in super().__iter__():
           if key not in traversed:
@@ -776,15 +776,15 @@
       hide_default_values: bool = False,
       exclude_keys: Optional[Sequence[str]] = None,
       **kwargs) -> object_utils.JSONValueType:
     """Converts current object to a dict with plain Python objects."""
     exclude_keys = set(exclude_keys or [])
     if self._value_spec and self._value_spec.schema:
       json_repr = dict()
-      matched_keys, _ = self._value_spec.schema.resolve(self.keys())
+      matched_keys, _ = self._value_spec.schema.resolve(self.keys())  # pytype: disable=attribute-error
       for key_spec, keys in matched_keys.items():
         # NOTE(daiyip): The key values of frozen field can safely be excluded
         # since they will be the same for a class.
         field = self._value_spec.schema[key_spec]
         if not field.frozen:
           for key in keys:
             if key not in exclude_keys:
@@ -857,15 +857,15 @@
     cls_name = cls_name or ''
     exclude_keys = exclude_keys or set()
     def _indent(text, indent):
       return ' ' * 2 * indent + text
 
     field_list = []
     if self._value_spec and self._value_spec.schema:
-      matched_keys, unmatched = self._value_spec.schema.resolve(self.keys())
+      matched_keys, unmatched = self._value_spec.schema.resolve(self.keys())  # pytype: disable=attribute-error
       assert not unmatched
       for key_spec, keys in matched_keys.items():
         for key in keys:
           if key not in exclude_keys:
             field = self._value_spec.schema[key_spec]
             v = self.sym_getattr(key)
             if pg_typing.MISSING_VALUE == v:
```

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/dict_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/dict_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/diff.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/diff.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/diff_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/diff_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/flags.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/flags.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/flags_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/flags_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/functor.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/functor.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/functor_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/functor_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/list.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/list.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/list_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/list_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/object.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/object.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/object_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/object_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/origin.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/origin.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/origin_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/origin_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/pure_symbolic.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/pure_symbolic.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/schema_utils.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/schema_utils_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/symbolize.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/symbolize.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/symbolic/symbolize_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/symbolic/symbolize_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/tuning/__init__.py` & `pyglove-0.3.1.dev20230703/pyglove/core/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/tuning/backend.py` & `pyglove-0.3.1.dev20230703/pyglove/core/tuning/backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/tuning/backend_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/tuning/backend_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/tuning/early_stopping.py` & `pyglove-0.3.1.dev20230703/pyglove/core/tuning/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/tuning/local_backend.py` & `pyglove-0.3.1.dev20230703/pyglove/core/tuning/local_backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/tuning/protocols.py` & `pyglove-0.3.1.dev20230703/pyglove/core/tuning/protocols.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/tuning/protocols_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/tuning/protocols_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/tuning/sample.py` & `pyglove-0.3.1.dev20230703/pyglove/core/tuning/sample.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/tuning/sample_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/tuning/sample_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/typing/__init__.py` & `pyglove-0.3.1.dev20230703/pyglove/core/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/typing/annotation_conversion.py` & `pyglove-0.3.1.dev20230703/pyglove/core/typing/annotation_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/typing/annotation_conversion_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/typing/annotation_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/typing/callable_ext.py` & `pyglove-0.3.1.dev20230703/pyglove/core/typing/callable_ext.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/typing/callable_ext_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/typing/callable_ext_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/typing/callable_signature.py` & `pyglove-0.3.1.dev20230703/pyglove/core/typing/callable_signature.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/typing/callable_signature_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/typing/callable_signature_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/typing/class_schema.py` & `pyglove-0.3.1.dev20230703/pyglove/core/typing/class_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -971,15 +971,15 @@
     if self._allow_nonconst_keys:
       for key_spec, field in self._fields.items():
         if key_spec.match(key):
           return field
     return None
 
   @property
-  def description(self) -> str:
+  def description(self) -> Optional[str]:
     """Returns the description for the schema."""
     return self._description
 
   def set_description(self, description: str) -> None:
     """Sets the description for the schema."""
     self._description = description
 
@@ -1122,15 +1122,15 @@
     """Validates whether dict object is conformed with the schema."""
     self.apply(
         copy.deepcopy(dict_obj),
         allow_partial=allow_partial,
         root_path=root_path)
 
   @property
-  def name(self) -> str:
+  def name(self) -> Optional[str]:
     """Name of this schema."""
     return self._name
 
   def set_name(self, name: str) -> None:
     """Sets the name of this schema."""
     self._name = name
```

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/typing/class_schema_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/typing/class_schema_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/typing/class_schema_utils.py` & `pyglove-0.3.1.dev20230703/pyglove/core/typing/class_schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/typing/class_schema_utils_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/typing/class_schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/typing/custom_typing.py` & `pyglove-0.3.1.dev20230703/pyglove/core/typing/custom_typing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/typing/key_specs.py` & `pyglove-0.3.1.dev20230703/pyglove/core/typing/key_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/typing/key_specs_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/typing/key_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/typing/pytype_support.py` & `pyglove-0.3.1.dev20230703/pyglove/core/typing/pytype_support.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/typing/type_conversion.py` & `pyglove-0.3.1.dev20230703/pyglove/core/typing/type_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/typing/type_conversion_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/typing/type_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/typing/typed_missing.py` & `pyglove-0.3.1.dev20230703/pyglove/core/typing/typed_missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/typing/typed_missing_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/typing/typed_missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/typing/value_specs.py` & `pyglove-0.3.1.dev20230703/pyglove/core/typing/value_specs.py`

 * *Files 0% similar despite different names*

```diff
@@ -482,15 +482,15 @@
 
   @property
   def min_value(self) -> typing.Optional[numbers.Number]:
     """Returns minimum value of acceptable values."""
     return self._min_value
 
   @property
-  def max_value(self) -> numbers.Number:
+  def max_value(self) -> typing.Optional[numbers.Number]:
     """Returns maximum value of acceptable values."""
     return self._max_value
 
   def _validate(self, path: object_utils.KeyPath,
                 value: numbers.Number) -> None:
     """Validates applied value."""
     if ((self._min_value is not None and value < self._min_value) or
```

### Comparing `pyglove-0.3.1.dev20230702/pyglove/core/typing/value_specs_test.py` & `pyglove-0.3.1.dev20230703/pyglove/core/typing/value_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/__init__.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/early_stopping/__init__.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/early_stopping/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/early_stopping/base.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/early_stopping/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/early_stopping/base_test.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/early_stopping/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/early_stopping/step_wise.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/early_stopping/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/early_stopping/step_wise_test.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/early_stopping/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/evolution/__init__.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/evolution/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/evolution/base.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/evolution/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/evolution/base_test.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/evolution/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/evolution/hill_climb.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/evolution/hill_climb.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/evolution/hill_climb_test.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/evolution/hill_climb_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/evolution/mutators.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/evolution/mutators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/evolution/mutators_test.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/evolution/mutators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/evolution/neat.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/evolution/neat.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/evolution/neat_test.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/evolution/neat_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/evolution/nsga2.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/evolution/nsga2.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/evolution/nsga2_test.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/evolution/nsga2_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/evolution/recombinators.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/evolution/recombinators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/evolution/recombinators_test.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/evolution/recombinators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/evolution/regularized_evolution.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/evolution/regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/evolution/regularized_evolution_test.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/evolution/regularized_evolution_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/evolution/selectors.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/evolution/selectors.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/evolution/selectors_test.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/evolution/selectors_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/evolution/where.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/evolution/where.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/evolution/where_test.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/evolution/where_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/mutfun/__init__.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/mutfun/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/mutfun/base.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/mutfun/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/mutfun/base_test.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/mutfun/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/mutfun/basic_ops.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/mutfun/basic_ops.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/mutfun/basic_ops_test.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/mutfun/basic_ops_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/scalars/__init__.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/scalars/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/scalars/base.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/scalars/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/scalars/base_test.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/scalars/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/scalars/maths.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/scalars/maths.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/scalars/maths_test.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/scalars/maths_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/scalars/randoms.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/scalars/randoms.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/scalars/randoms_test.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/scalars/randoms_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/scalars/step_wise.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/scalars/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove/ext/scalars/step_wise_test.py` & `pyglove-0.3.1.dev20230703/pyglove/ext/scalars/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/pyglove.egg-info/PKG-INFO` & `pyglove-0.3.1.dev20230703/pyglove.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.3.1.dev20230702
+Version: 0.3.1.dev20230703
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.3.1.dev20230702/pyglove.egg-info/SOURCES.txt` & `pyglove-0.3.1.dev20230703/pyglove.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230702/setup.py` & `pyglove-0.3.1.dev20230703/setup.py`

 * *Files identical despite different names*

