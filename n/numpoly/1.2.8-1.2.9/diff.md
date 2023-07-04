# Comparing `tmp/numpoly-1.2.8.tar.gz` & `tmp/numpoly-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpoly-1.2.8.tar", last modified: Sat Jun  3 10:46:43 2023, max compression
+gzip compressed data, was "numpoly-1.2.9.tar", last modified: Mon Jul  3 19:54:22 2023, max compression
```

## Comparing `numpoly-1.2.8.tar` & `numpoly-1.2.9.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-03 10:46:43.866494 numpoly-1.2.8/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1327 2023-06-03 10:46:31.000000 numpoly-1.2.8/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2023-06-03 10:46:31.000000 numpoly-1.2.8/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5415 2023-06-03 10:46:43.866494 numpoly-1.2.8/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4942 2023-06-03 10:46:31.000000 numpoly-1.2.8/README.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-03 10:46:43.850494 numpoly-1.2.8/numpoly/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1866 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6695 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/align.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-03 10:46:43.858494 numpoly-1.2.8/numpoly/array_function/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2847 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2218 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/absolute.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2272 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/add.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2278 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/all.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2628 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/allclose.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2620 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/amax.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2623 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/amin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2387 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/any.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4039 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/apply_along_axis.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2575 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/apply_over_axes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1919 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/argmax.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1895 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/argmin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1705 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/around.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5205 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/array_repr.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1651 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/array_split.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2159 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/array_str.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1102 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/atleast_1d.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1211 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/atleast_2d.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1443 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/atleast_3d.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1826 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/broadcast_arrays.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2007 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/ceil.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4633 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/choose.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1309 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/common_type.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2223 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/concatenate.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3191 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/copyto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1606 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/count_nonzero.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2302 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/cumsum.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1380 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/det.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1299 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/diag.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2369 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/diagonal.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3148 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/diff.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2873 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/divmod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1553 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/dsplit.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2043 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/dstack.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1945 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/ediff1d.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2356 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/equal.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      989 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/expand_dims.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1979 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/floor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3401 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/floor_divide.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1797 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/full.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2442 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/full_like.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2888 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/greater.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2961 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/greater_equal.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1639 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/hsplit.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1854 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/hstack.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      540 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/inner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3051 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/isclose.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2428 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/isfinite.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2854 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/less.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2926 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/less_equal.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4067 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/load.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5295 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/loadtxt.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2448 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/logical_and.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2443 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/logical_or.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2072 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/matmul.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3084 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/maximum.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2653 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/mean.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3074 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/minimum.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1221 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/moveaxis.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3191 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/multiply.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1770 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/negative.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1130 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/nonzero.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2408 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/not_equal.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1256 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/ones.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1991 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/ones_like.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1384 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/outer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1841 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/positive.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3227 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/power.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4276 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/prod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2600 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/remainder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1663 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/repeat.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2494 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/reshape.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1792 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/result_type.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1873 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/rint.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1749 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/roots.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2377 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/save.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3858 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/savetxt.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2391 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/savez.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2440 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/savez_compressed.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2798 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/split.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1798 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/square.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2174 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/stack.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2264 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/subtract.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2759 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/sum.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1772 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/tile.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1129 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/transpose.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3314 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/true_divide.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1653 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/vsplit.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1946 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/vstack.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2050 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/where.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1263 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/zeros.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1998 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/array_function/zeros_like.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    25098 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/baseclass.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-03 10:46:43.862494 numpoly-1.2.8/numpoly/construct/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      421 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/construct/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1836 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/construct/aspolynomial.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8780 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/construct/clean.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3155 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/construct/compose.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3054 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/construct/from_attributes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1648 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/construct/from_roots.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3744 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/construct/monomial.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5072 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/construct/polynomial.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2988 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/construct/symbols.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1331 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/construct/variable.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3348 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/dispatch.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4787 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/option.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-03 10:46:43.862494 numpoly-1.2.8/numpoly/poly_function/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      740 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/poly_function/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3526 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/poly_function/call.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1378 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/poly_function/decompose.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4150 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/poly_function/derivative.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-03 10:46:43.862494 numpoly-1.2.8/numpoly/poly_function/divide/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      160 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/poly_function/divide/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2221 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/poly_function/divide/divide.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6469 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/poly_function/divide/divmod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2462 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/poly_function/divide/remainder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      828 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/poly_function/isconstant.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1800 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/poly_function/lead_coefficient.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2039 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/poly_function/lead_exponent.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2303 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/poly_function/set_dimensions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2363 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/poly_function/sortable_proxy.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      929 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/poly_function/tonumpy.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1152 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/sympy_.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-03 10:46:43.862494 numpoly-1.2.8/numpoly/utils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      187 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/utils/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2730 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/utils/bindex.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2289 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/utils/cross_truncation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4192 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/utils/glexindex.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2090 2023-06-03 10:46:31.000000 numpoly-1.2.8/numpoly/utils/glexsort.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-03 10:46:43.850494 numpoly-1.2.8/numpoly.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5415 2023-06-03 10:46:43.000000 numpoly-1.2.8/numpoly.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4641 2023-06-03 10:46:43.000000 numpoly-1.2.8/numpoly.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-03 10:46:43.000000 numpoly-1.2.8/numpoly.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      204 2023-06-03 10:46:43.000000 numpoly-1.2.8/numpoly.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2023-06-03 10:46:43.000000 numpoly-1.2.8/numpoly.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1061 2023-06-03 10:46:31.000000 numpoly-1.2.8/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-03 10:46:43.866494 numpoly-1.2.8/setup.cfg
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-03 10:46:43.866494 numpoly-1.2.8/test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      546 2023-06-03 10:46:31.000000 numpoly-1.2.8/test/test_align.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    40655 2023-06-03 10:46:31.000000 numpoly-1.2.8/test/test_array_function.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2144 2023-06-03 10:46:31.000000 numpoly-1.2.8/test/test_baseclass.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3786 2023-06-03 10:46:31.000000 numpoly-1.2.8/test/test_construct.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      165 2023-06-03 10:46:31.000000 numpoly-1.2.8/test/test_dispatch.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1481 2023-06-03 10:46:31.000000 numpoly-1.2.8/test/test_option.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7286 2023-06-03 10:46:31.000000 numpoly-1.2.8/test/test_poly_function.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2870 2023-06-03 10:46:31.000000 numpoly-1.2.8/test/test_save_load.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5326 2023-06-03 10:46:31.000000 numpoly-1.2.8/test/test_utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-03 19:54:22.305624 numpoly-1.2.9/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1327 2023-07-03 19:54:08.000000 numpoly-1.2.9/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2023-07-03 19:54:08.000000 numpoly-1.2.9/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5415 2023-07-03 19:54:22.305624 numpoly-1.2.9/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4942 2023-07-03 19:54:08.000000 numpoly-1.2.9/README.rst
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-03 19:54:22.285624 numpoly-1.2.9/numpoly/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1866 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6695 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/align.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-03 19:54:22.301624 numpoly-1.2.9/numpoly/array_function/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2847 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2218 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/absolute.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2272 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/add.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2278 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/all.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2628 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/allclose.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2620 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/amax.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2623 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/amin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2387 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/any.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4039 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/apply_along_axis.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2575 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/apply_over_axes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1919 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/argmax.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1895 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/argmin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1705 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/around.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5205 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/array_repr.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1651 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/array_split.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2159 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/array_str.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1102 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/atleast_1d.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1211 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/atleast_2d.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1443 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/atleast_3d.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1826 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/broadcast_arrays.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2007 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/ceil.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4633 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/choose.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1309 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/common_type.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2223 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/concatenate.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3191 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/copyto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1606 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/count_nonzero.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2302 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/cumsum.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1380 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/det.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1299 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/diag.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2369 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/diagonal.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3148 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/diff.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2873 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/divmod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1553 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/dsplit.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2043 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/dstack.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1945 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/ediff1d.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2356 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/equal.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      989 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/expand_dims.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1979 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/floor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3401 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/floor_divide.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1797 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/full.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2442 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/full_like.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2888 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/greater.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2961 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/greater_equal.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1639 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/hsplit.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1854 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/hstack.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      540 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/inner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3051 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/isclose.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2428 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/isfinite.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2854 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/less.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2926 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/less_equal.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4067 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/load.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5295 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/loadtxt.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2448 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/logical_and.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2443 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/logical_or.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2072 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/matmul.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3084 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/maximum.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2653 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/mean.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3074 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/minimum.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1221 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/moveaxis.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3191 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/multiply.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1770 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/negative.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1130 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/nonzero.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2408 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/not_equal.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1256 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/ones.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1991 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/ones_like.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1384 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/outer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1841 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/positive.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3227 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/power.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4276 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/prod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2600 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/remainder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1663 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/repeat.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2494 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/reshape.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1792 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/result_type.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1873 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/rint.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1749 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/roots.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2377 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/save.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3858 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/savetxt.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2391 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/savez.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2440 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/savez_compressed.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2798 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/split.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1798 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/square.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2174 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/stack.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2264 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/subtract.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2759 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/sum.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1772 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/tile.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1129 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/transpose.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3314 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/true_divide.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1653 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/vsplit.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1946 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/vstack.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2050 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/where.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1263 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/zeros.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1998 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/array_function/zeros_like.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    25174 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/baseclass.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-03 19:54:22.301624 numpoly-1.2.9/numpoly/construct/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      421 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/construct/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1836 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/construct/aspolynomial.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8780 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/construct/clean.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3155 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/construct/compose.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3054 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/construct/from_attributes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1648 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/construct/from_roots.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3744 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/construct/monomial.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5072 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/construct/polynomial.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2988 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/construct/symbols.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1331 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/construct/variable.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3348 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/dispatch.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4787 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/option.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-03 19:54:22.301624 numpoly-1.2.9/numpoly/poly_function/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      740 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/poly_function/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3526 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/poly_function/call.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1378 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/poly_function/decompose.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4150 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/poly_function/derivative.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-03 19:54:22.301624 numpoly-1.2.9/numpoly/poly_function/divide/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      160 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/poly_function/divide/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2221 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/poly_function/divide/divide.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6469 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/poly_function/divide/divmod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2462 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/poly_function/divide/remainder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      828 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/poly_function/isconstant.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1800 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/poly_function/lead_coefficient.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2039 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/poly_function/lead_exponent.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2303 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/poly_function/set_dimensions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2363 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/poly_function/sortable_proxy.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      929 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/poly_function/tonumpy.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1152 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/sympy_.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-03 19:54:22.305624 numpoly-1.2.9/numpoly/utils/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      187 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/utils/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2730 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/utils/bindex.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2289 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/utils/cross_truncation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4192 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/utils/glexindex.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2090 2023-07-03 19:54:08.000000 numpoly-1.2.9/numpoly/utils/glexsort.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-03 19:54:22.289624 numpoly-1.2.9/numpoly.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5415 2023-07-03 19:54:22.000000 numpoly-1.2.9/numpoly.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4641 2023-07-03 19:54:22.000000 numpoly-1.2.9/numpoly.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-03 19:54:22.000000 numpoly-1.2.9/numpoly.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      204 2023-07-03 19:54:22.000000 numpoly-1.2.9/numpoly.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2023-07-03 19:54:22.000000 numpoly-1.2.9/numpoly.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1061 2023-07-03 19:54:08.000000 numpoly-1.2.9/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-07-03 19:54:22.305624 numpoly-1.2.9/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-03 19:54:22.305624 numpoly-1.2.9/test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      546 2023-07-03 19:54:08.000000 numpoly-1.2.9/test/test_align.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    40655 2023-07-03 19:54:08.000000 numpoly-1.2.9/test/test_array_function.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2144 2023-07-03 19:54:08.000000 numpoly-1.2.9/test/test_baseclass.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3786 2023-07-03 19:54:08.000000 numpoly-1.2.9/test/test_construct.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      165 2023-07-03 19:54:08.000000 numpoly-1.2.9/test/test_dispatch.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1481 2023-07-03 19:54:08.000000 numpoly-1.2.9/test/test_option.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7286 2023-07-03 19:54:08.000000 numpoly-1.2.9/test/test_poly_function.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2870 2023-07-03 19:54:08.000000 numpoly-1.2.9/test/test_save_load.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5326 2023-07-03 19:54:08.000000 numpoly-1.2.9/test/test_utils.py
```

### Comparing `numpoly-1.2.8/LICENSE` & `numpoly-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/PKG-INFO` & `numpoly-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numpoly
-Version: 1.2.8
+Version: 1.2.9
 Summary: Polynomials as a numpy datatype
 License: BSD-2-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
```

### Comparing `numpoly-1.2.8/README.rst` & `numpoly-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/__init__.py` & `numpoly-1.2.9/numpoly/__init__.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/align.py` & `numpoly-1.2.9/numpoly/align.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/__init__.py` & `numpoly-1.2.9/numpoly/array_function/__init__.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/absolute.py` & `numpoly-1.2.9/numpoly/array_function/absolute.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/add.py` & `numpoly-1.2.9/numpoly/array_function/add.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/all.py` & `numpoly-1.2.9/numpoly/array_function/all.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/allclose.py` & `numpoly-1.2.9/numpoly/array_function/allclose.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/amax.py` & `numpoly-1.2.9/numpoly/array_function/amax.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/amin.py` & `numpoly-1.2.9/numpoly/array_function/amin.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/any.py` & `numpoly-1.2.9/numpoly/array_function/any.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/apply_along_axis.py` & `numpoly-1.2.9/numpoly/array_function/apply_along_axis.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/apply_over_axes.py` & `numpoly-1.2.9/numpoly/array_function/apply_over_axes.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/argmax.py` & `numpoly-1.2.9/numpoly/array_function/argmax.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/argmin.py` & `numpoly-1.2.9/numpoly/array_function/argmin.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/around.py` & `numpoly-1.2.9/numpoly/array_function/around.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/array_repr.py` & `numpoly-1.2.9/numpoly/array_function/array_repr.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/array_split.py` & `numpoly-1.2.9/numpoly/array_function/array_split.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/array_str.py` & `numpoly-1.2.9/numpoly/array_function/array_str.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/atleast_1d.py` & `numpoly-1.2.9/numpoly/array_function/atleast_1d.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/atleast_2d.py` & `numpoly-1.2.9/numpoly/array_function/atleast_2d.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/atleast_3d.py` & `numpoly-1.2.9/numpoly/array_function/atleast_3d.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/broadcast_arrays.py` & `numpoly-1.2.9/numpoly/array_function/broadcast_arrays.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/ceil.py` & `numpoly-1.2.9/numpoly/array_function/ceil.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/choose.py` & `numpoly-1.2.9/numpoly/array_function/choose.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/common_type.py` & `numpoly-1.2.9/numpoly/array_function/common_type.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/concatenate.py` & `numpoly-1.2.9/numpoly/array_function/concatenate.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/copyto.py` & `numpoly-1.2.9/numpoly/array_function/copyto.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/count_nonzero.py` & `numpoly-1.2.9/numpoly/array_function/count_nonzero.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/cumsum.py` & `numpoly-1.2.9/numpoly/array_function/cumsum.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/det.py` & `numpoly-1.2.9/numpoly/array_function/det.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/diag.py` & `numpoly-1.2.9/numpoly/array_function/diag.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/diagonal.py` & `numpoly-1.2.9/numpoly/array_function/diagonal.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/diff.py` & `numpoly-1.2.9/numpoly/array_function/diff.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/divmod.py` & `numpoly-1.2.9/numpoly/array_function/divmod.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/dsplit.py` & `numpoly-1.2.9/numpoly/array_function/dsplit.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/dstack.py` & `numpoly-1.2.9/numpoly/array_function/dstack.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/ediff1d.py` & `numpoly-1.2.9/numpoly/array_function/ediff1d.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/equal.py` & `numpoly-1.2.9/numpoly/array_function/equal.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/expand_dims.py` & `numpoly-1.2.9/numpoly/array_function/expand_dims.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/floor.py` & `numpoly-1.2.9/numpoly/array_function/floor.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/floor_divide.py` & `numpoly-1.2.9/numpoly/array_function/floor_divide.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/full.py` & `numpoly-1.2.9/numpoly/array_function/full.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/full_like.py` & `numpoly-1.2.9/numpoly/array_function/full_like.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/greater.py` & `numpoly-1.2.9/numpoly/array_function/greater.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/greater_equal.py` & `numpoly-1.2.9/numpoly/array_function/greater_equal.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/hsplit.py` & `numpoly-1.2.9/numpoly/array_function/hsplit.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/hstack.py` & `numpoly-1.2.9/numpoly/array_function/hstack.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/inner.py` & `numpoly-1.2.9/numpoly/array_function/inner.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/isclose.py` & `numpoly-1.2.9/numpoly/array_function/isclose.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/isfinite.py` & `numpoly-1.2.9/numpoly/array_function/isfinite.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/less.py` & `numpoly-1.2.9/numpoly/array_function/less.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/less_equal.py` & `numpoly-1.2.9/numpoly/array_function/less_equal.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/load.py` & `numpoly-1.2.9/numpoly/array_function/load.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/loadtxt.py` & `numpoly-1.2.9/numpoly/array_function/loadtxt.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/logical_and.py` & `numpoly-1.2.9/numpoly/array_function/logical_and.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/logical_or.py` & `numpoly-1.2.9/numpoly/array_function/logical_or.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/matmul.py` & `numpoly-1.2.9/numpoly/array_function/matmul.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/maximum.py` & `numpoly-1.2.9/numpoly/array_function/maximum.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/mean.py` & `numpoly-1.2.9/numpoly/array_function/mean.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/minimum.py` & `numpoly-1.2.9/numpoly/array_function/minimum.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/moveaxis.py` & `numpoly-1.2.9/numpoly/array_function/moveaxis.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/multiply.py` & `numpoly-1.2.9/numpoly/array_function/multiply.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/negative.py` & `numpoly-1.2.9/numpoly/array_function/negative.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/nonzero.py` & `numpoly-1.2.9/numpoly/array_function/nonzero.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/not_equal.py` & `numpoly-1.2.9/numpoly/array_function/not_equal.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/ones.py` & `numpoly-1.2.9/numpoly/array_function/ones.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/ones_like.py` & `numpoly-1.2.9/numpoly/array_function/ones_like.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/outer.py` & `numpoly-1.2.9/numpoly/array_function/outer.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/positive.py` & `numpoly-1.2.9/numpoly/array_function/positive.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/power.py` & `numpoly-1.2.9/numpoly/array_function/power.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/prod.py` & `numpoly-1.2.9/numpoly/array_function/prod.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/remainder.py` & `numpoly-1.2.9/numpoly/array_function/remainder.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/repeat.py` & `numpoly-1.2.9/numpoly/array_function/repeat.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/reshape.py` & `numpoly-1.2.9/numpoly/array_function/reshape.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/result_type.py` & `numpoly-1.2.9/numpoly/array_function/result_type.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/rint.py` & `numpoly-1.2.9/numpoly/array_function/rint.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/roots.py` & `numpoly-1.2.9/numpoly/array_function/roots.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/save.py` & `numpoly-1.2.9/numpoly/array_function/save.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/savetxt.py` & `numpoly-1.2.9/numpoly/array_function/savetxt.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/savez.py` & `numpoly-1.2.9/numpoly/array_function/savez.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/savez_compressed.py` & `numpoly-1.2.9/numpoly/array_function/savez_compressed.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/split.py` & `numpoly-1.2.9/numpoly/array_function/split.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/square.py` & `numpoly-1.2.9/numpoly/array_function/square.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/stack.py` & `numpoly-1.2.9/numpoly/array_function/stack.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/subtract.py` & `numpoly-1.2.9/numpoly/array_function/subtract.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/sum.py` & `numpoly-1.2.9/numpoly/array_function/sum.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/tile.py` & `numpoly-1.2.9/numpoly/array_function/tile.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/transpose.py` & `numpoly-1.2.9/numpoly/array_function/transpose.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/true_divide.py` & `numpoly-1.2.9/numpoly/array_function/true_divide.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/vsplit.py` & `numpoly-1.2.9/numpoly/array_function/vsplit.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/vstack.py` & `numpoly-1.2.9/numpoly/array_function/vstack.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/where.py` & `numpoly-1.2.9/numpoly/array_function/where.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/zeros.py` & `numpoly-1.2.9/numpoly/array_function/zeros.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/array_function/zeros_like.py` & `numpoly-1.2.9/numpoly/array_function/zeros_like.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/baseclass.py` & `numpoly-1.2.9/numpoly/baseclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -636,19 +636,20 @@
                         [q1-3, q0*q1**2]])
             >>> poly[0]
             polynomial([-4*q0+1, q0**2])
             >>> poly[:, 1]
             polynomial([q0**2, q0*q1**2])
 
         """
-        return numpoly.polynomial_from_attributes(
-            exponents=self.exponents,
-            coefficients=[coeff[index] for coeff in self.coefficients],
-            names=self.names,
-        )
+        with numpoly.global_options(retain_names=True):
+            return numpoly.polynomial_from_attributes(
+                exponents=self.exponents,
+                coefficients=[coeff[index] for coeff in self.coefficients],
+                names=self.names,
+            )
 
     # def __setitem__(self, index, other):
     #     other = numpoly.aspolynomial(other)
     #     difference =  set(other.names).difference(self.names)
     #     assert not difference, (
     #         "polynomial does not contain indeterminants: %s" % difference)
     #     assert self.ndim >= other.ndim
```

### Comparing `numpoly-1.2.8/numpoly/construct/aspolynomial.py` & `numpoly-1.2.9/numpoly/construct/aspolynomial.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/construct/clean.py` & `numpoly-1.2.9/numpoly/construct/clean.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/construct/compose.py` & `numpoly-1.2.9/numpoly/construct/compose.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/construct/from_attributes.py` & `numpoly-1.2.9/numpoly/construct/from_attributes.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/construct/from_roots.py` & `numpoly-1.2.9/numpoly/construct/from_roots.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/construct/monomial.py` & `numpoly-1.2.9/numpoly/construct/monomial.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/construct/polynomial.py` & `numpoly-1.2.9/numpoly/construct/polynomial.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/construct/symbols.py` & `numpoly-1.2.9/numpoly/construct/symbols.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/construct/variable.py` & `numpoly-1.2.9/numpoly/construct/variable.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/dispatch.py` & `numpoly-1.2.9/numpoly/dispatch.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/option.py` & `numpoly-1.2.9/numpoly/option.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/poly_function/__init__.py` & `numpoly-1.2.9/numpoly/poly_function/__init__.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/poly_function/call.py` & `numpoly-1.2.9/numpoly/poly_function/call.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/poly_function/decompose.py` & `numpoly-1.2.9/numpoly/poly_function/decompose.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/poly_function/derivative.py` & `numpoly-1.2.9/numpoly/poly_function/derivative.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/poly_function/divide/divide.py` & `numpoly-1.2.9/numpoly/poly_function/divide/divide.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/poly_function/divide/divmod.py` & `numpoly-1.2.9/numpoly/poly_function/divide/divmod.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/poly_function/divide/remainder.py` & `numpoly-1.2.9/numpoly/poly_function/divide/remainder.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/poly_function/isconstant.py` & `numpoly-1.2.9/numpoly/poly_function/isconstant.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/poly_function/lead_coefficient.py` & `numpoly-1.2.9/numpoly/poly_function/lead_coefficient.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/poly_function/lead_exponent.py` & `numpoly-1.2.9/numpoly/poly_function/lead_exponent.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/poly_function/set_dimensions.py` & `numpoly-1.2.9/numpoly/poly_function/set_dimensions.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/poly_function/sortable_proxy.py` & `numpoly-1.2.9/numpoly/poly_function/sortable_proxy.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/poly_function/tonumpy.py` & `numpoly-1.2.9/numpoly/poly_function/tonumpy.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/sympy_.py` & `numpoly-1.2.9/numpoly/sympy_.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/utils/bindex.py` & `numpoly-1.2.9/numpoly/utils/bindex.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/utils/cross_truncation.py` & `numpoly-1.2.9/numpoly/utils/cross_truncation.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/utils/glexindex.py` & `numpoly-1.2.9/numpoly/utils/glexindex.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly/utils/glexsort.py` & `numpoly-1.2.9/numpoly/utils/glexsort.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/numpoly.egg-info/PKG-INFO` & `numpoly-1.2.9/numpoly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numpoly
-Version: 1.2.8
+Version: 1.2.9
 Summary: Polynomials as a numpy datatype
 License: BSD-2-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
```

### Comparing `numpoly-1.2.8/numpoly.egg-info/SOURCES.txt` & `numpoly-1.2.9/numpoly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/pyproject.toml` & `numpoly-1.2.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.9.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "numpoly"
-version = "1.2.8"
+version = "1.2.9"
 description = "Polynomials as a numpy datatype"
 license = {text = "BSD-2-Clause"}
 readme = "README.rst"
 classifiers = [
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Mathematics",
```

### Comparing `numpoly-1.2.8/test/test_align.py` & `numpoly-1.2.9/test/test_align.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/test/test_array_function.py` & `numpoly-1.2.9/test/test_array_function.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/test/test_baseclass.py` & `numpoly-1.2.9/test/test_baseclass.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/test/test_construct.py` & `numpoly-1.2.9/test/test_construct.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/test/test_option.py` & `numpoly-1.2.9/test/test_option.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/test/test_poly_function.py` & `numpoly-1.2.9/test/test_poly_function.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/test/test_save_load.py` & `numpoly-1.2.9/test/test_save_load.py`

 * *Files identical despite different names*

### Comparing `numpoly-1.2.8/test/test_utils.py` & `numpoly-1.2.9/test/test_utils.py`

 * *Files identical despite different names*

