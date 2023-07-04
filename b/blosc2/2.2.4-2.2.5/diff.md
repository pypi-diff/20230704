# Comparing `tmp/blosc2-2.2.4.tar.gz` & `tmp/blosc2-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blosc2-2.2.4.tar", last modified: Wed Jun 21 12:01:27 2023, max compression
+gzip compressed data, was "blosc2-2.2.5.tar", last modified: Tue Jul  4 06:08:53 2023, max compression
```

## Comparing `blosc2-2.2.4.tar` & `blosc2-2.2.5.tar`

### file list

```diff
@@ -1,1164 +1,1165 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.142870 blosc2-2.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 11:59:24.000000 blosc2-2.2.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.722863 blosc2-2.2.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-21 11:59:24.000000 blosc2-2.2.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.722863 blosc2-2.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-21 11:59:24.000000 blosc2-2.2.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-06-21 11:59:24.000000 blosc2-2.2.4/.github/workflows/cibuildwheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-21 11:59:24.000000 blosc2-2.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-21 11:59:24.000000 blosc2-2.2.4/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-21 11:59:24.000000 blosc2-2.2.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-21 11:59:24.000000 blosc2-2.2.4/ANNOUNCE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-21 11:59:24.000000 blosc2-2.2.4/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-21 11:59:24.000000 blosc2-2.2.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-21 11:59:24.000000 blosc2-2.2.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-06-21 12:01:27.142870 blosc2-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-06-21 11:59:24.000000 blosc2-2.2.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-21 11:59:24.000000 blosc2-2.2.4/README_DEVELOPERS.md
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-06-21 11:59:24.000000 blosc2-2.2.4/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-21 11:59:24.000000 blosc2-2.2.4/RELEASING.rst
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 11:59:24.000000 blosc2-2.2.4/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.726863 blosc2-2.2.4/bench/
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-21 11:59:24.000000 blosc2-2.2.4/bench/compress_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-21 11:59:24.000000 blosc2-2.2.4/bench/get_slice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.726863 blosc2-2.2.4/bench/ndarray/
--rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-06-21 11:59:24.000000 blosc2-2.2.4/bench/ndarray/compare_getslice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-21 11:59:24.000000 blosc2-2.2.4/bench/ndarray/copy_postfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-21 11:59:24.000000 blosc2-2.2.4/bench/ndarray/download_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.730863 blosc2-2.2.4/bench/ndarray/era5-pds/
--rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-06-21 11:59:24.000000 blosc2-2.2.4/bench/ndarray/era5-pds/measurements-i10k.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-06-21 11:59:24.000000 blosc2-2.2.4/bench/ndarray/era5-pds/measurements-i13k-always-split.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    16476 2023-06-21 11:59:24.000000 blosc2-2.2.4/bench/ndarray/era5-pds/measurements-i13k-never-split.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    16500 2023-06-21 11:59:24.000000 blosc2-2.2.4/bench/ndarray/era5-pds/measurements-i13k.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    16500 2023-06-21 11:59:24.000000 blosc2-2.2.4/bench/ndarray/era5-pds/measurements-m1.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-06-21 11:59:24.000000 blosc2-2.2.4/bench/ndarray/era5-pds/measurements-ryzen3.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    10749 2023-06-21 11:59:24.000000 blosc2-2.2.4/bench/ndarray/plot_transcode_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-06-21 11:59:24.000000 blosc2-2.2.4/bench/ndarray/transcode_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-06-21 11:59:24.000000 blosc2-2.2.4/bench/pack_compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-21 11:59:24.000000 blosc2-2.2.4/bench/pack_large.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-21 11:59:24.000000 blosc2-2.2.4/bench/pack_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-21 11:59:24.000000 blosc2-2.2.4/bench/set_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-21 11:59:24.000000 blosc2-2.2.4/bench/sum_postfilter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.734863 blosc2-2.2.4/blosc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-21 11:59:24.000000 blosc2-2.2.4/blosc2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-06-21 11:59:24.000000 blosc2-2.2.4/blosc2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    88179 2023-06-21 11:59:24.000000 blosc2-2.2.4/blosc2/blosc2_ext.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.746864 blosc2-2.2.4/blosc2/c-blosc2/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.746864 blosc2-2.2.4/blosc2/c-blosc2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.746864 blosc2-2.2.4/blosc2/c-blosc2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.746864 blosc2-2.2.4/blosc2/c-blosc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/.github/workflows/cmake.yml
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/.github/workflows/fuzz.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/ANNOUNCE.md
--rw-r--r--   0 runner    (1001) docker     (123)    17330 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/COMPILING_WITH_WHEELS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/DEVELOPING-GUIDE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/FAQ.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.750864 blosc2-2.2.4/blosc2/c-blosc2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/LICENSES/BITSHUFFLE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/LICENSES/FASTLZ.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/LICENSES/LZ4.txt
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/LICENSES/ZLIB.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/LICENSES/ZSTD.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16794 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15951 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/README_ARM.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/README_B2ND_METALAYER.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13926 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/README_CFRAME_FORMAT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/README_CHUNK_FORMAT.rst
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/README_FUZZER.md
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/README_SFRAME_FORMAT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/README_THREADED.rst
--rw-r--r--   0 runner    (1001) docker     (123)    26391 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/RELEASING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/ROADMAP.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/THANKS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/TODO-refactorization.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.754864 blosc2-2.2.4/blosc2/c-blosc2/bench/
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/Makefile.mingw
--rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/b2bench.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.754864 blosc2-2.2.4/blosc2/c-blosc2/bench/b2nd/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/b2nd/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/b2nd/bench_get_slice.c
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/b2nd/bench_zfp_getitem.c
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/create_frame.c
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/delta_schunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/plot-speeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/plot-sum_openmp-results.py
--rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/rainfall-grid-150x150.bin
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/read-grid-150x150.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.758864 blosc2-2.2.4/blosc2/c-blosc2/bench/results-corex/
--rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/results-corex/blosclz-cl1-sum_openmp-corex.out
--rw-r--r--   0 runner    (1001) docker     (123)    29803 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/results-corex/blosclz-suite-corex.out
--rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/results-corex/lz4-cl1-sum_openmp-corex.out
--rw-r--r--   0 runner    (1001) docker     (123)    29683 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/results-corex/lz4-suite-corex.out
--rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/results-corex/lz4hc-cl1-sum_openmp-corex.out
--rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/results-corex/zlib-cl1-sum_openmp-corex.out
--rw-r--r--   0 runner    (1001) docker     (123)    11248 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/results-corex/zstd-cl1-sum_openmp-corex.out
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/sframe_bench.c
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/sum_openmp.c
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/trunc_prec_schunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/bench/zero_runlen.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.778864 blosc2-2.2.4/blosc2/c-blosc2/blosc/
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    64356 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/b2nd.c
--rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/b2nd_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/b2nd_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)    21593 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/bitshuffle-altivec.c
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/bitshuffle-altivec.h
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/bitshuffle-avx2.c
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/bitshuffle-avx2.h
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/bitshuffle-generic.c
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/bitshuffle-generic.h
--rw-r--r--   0 runner    (1001) docker     (123)    49620 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/bitshuffle-neon.c
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/bitshuffle-neon.h
--rw-r--r--   0 runner    (1001) docker     (123)    15933 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/bitshuffle-sse2.c
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/bitshuffle-sse2.h
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/blosc-private.h
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/blosc2-stdio.c
--rw-r--r--   0 runner    (1001) docker     (123)   151464 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/blosc2.c
--rw-r--r--   0 runner    (1001) docker     (123)    24339 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/blosclz.c
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/blosclz.h
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/config.h.in
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/context.h
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/delta.c
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/delta.h
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/directories.c
--rw-r--r--   0 runner    (1001) docker     (123)    16723 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/fastcopy.c
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/fastcopy.h
--rw-r--r--   0 runner    (1001) docker     (123)   115804 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/frame.c
--rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/frame.h
--rw-r--r--   0 runner    (1001) docker     (123)    56502 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/schunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/sframe.c
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/sframe.h
--rw-r--r--   0 runner    (1001) docker     (123)    15715 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle-altivec.c
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle-altivec.h
--rw-r--r--   0 runner    (1001) docker     (123)    31648 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle-avx2.c
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle-avx2.h
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle-generic.c
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle-generic.h
--rw-r--r--   0 runner    (1001) docker     (123)    22000 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle-neon.c
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle-neon.h
--rw-r--r--   0 runner    (1001) docker     (123)    26157 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle-sse2.c
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle-sse2.h
--rw-r--r--   0 runner    (1001) docker     (123)    19569 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle.c
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle.h
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/stune.c
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/stune.h
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/timestamp.c
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/transpose-altivec.h
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/trunc-prec.c
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/trunc-prec.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.782864 blosc2-2.2.4/blosc2/c-blosc2/blosc/win32/
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/win32/pthread.c
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc/win32/pthread.h
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/blosc2.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.782864 blosc2-2.2.4/blosc2/c-blosc2/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/cmake/FindIPP.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/cmake/FindLZ4.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/cmake/FindSIMD.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/cmake/FindZLIB_NG.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/cmake/FindZSTD.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/cmake/toolchain-aarch64.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/cmake/toolchain-armhf.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/cmake/toolchain-armsf.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/code_of_conduct.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.798864 blosc2-2.2.4/blosc2/c-blosc2/compat/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    26736 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.11.1-blosclz.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    33610 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.11.1-lz4.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    32485 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.11.1-lz4hc.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.11.1-zlib.cdata
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.11.1-zstd.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    36256 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.14.0-blosclz.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    36267 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.14.0-lz4.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    36263 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.14.0-lz4hc.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    20530 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.14.0-zlib.cdata
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.14.0-zstd.cdata
--rw-r--r--   0 runner    (1001) docker     (123)   141205 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle4-memcpy.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    22760 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle8-nomemcpy.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    27787 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle4-memcpy.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    22760 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle8-nomemcpy.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    36349 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.3.0-blosclz.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    36267 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.3.0-lz4.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    31963 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.3.0-lz4hc.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    14956 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.3.0-zlib.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    36394 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.7.0-blosclz.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    36267 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.7.0-lz4.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    31963 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.7.0-lz4hc.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    14956 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.7.0-zlib.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    15763 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle4-memcpy.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle8-nomemcpy.cdata
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/compat/filegen.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.798864 blosc2-2.2.4/blosc2/c-blosc2/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.710863 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.798864 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6974 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test1.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    23072 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test16.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     8642 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test2.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    11457 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test4.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    14436 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test8.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.798864 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10706 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    16818 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.802864 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     4846 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.802864 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2262 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     7896 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle
--rwxr-xr-x   0 runner    (1001) docker     (123)     7574 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.802864 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3708 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     7910 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.802864 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5792 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    11472 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.802864 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8199 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    24719 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.802864 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1376 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     4233 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.806865 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2214 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     7559 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.806865 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3616 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    13037 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.806865 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4479 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    15834 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.710863 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.806865 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/Test/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10906 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test16.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2162 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test2.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2769 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test4.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     6545 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test8.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.810865 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     7713 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_bucle.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     4630 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     8365 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.810865 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2577 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.810865 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)      756 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2997 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.810865 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2268 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     4883 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_bucle.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2711 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     6813 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt_bucle.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2010 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     5787 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.814865 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3949 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     7649 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_bucle.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     4177 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     7353 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.814865 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)      656 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2212 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.814865 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle4_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)      770 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle4_neon/unshuffle4_neon.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.814865 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2279 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     5550 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_bucle.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2737 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     4987 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.818865 blosc2-2.2.4/blosc2/c-blosc2/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.818865 blosc2-2.2.4/blosc2/c-blosc2/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/_static/blosc-logo_256.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.818865 blosc2-2.2.4/blosc2/c-blosc2/doc/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/c-blosc2.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.818865 blosc2-2.2.4/blosc2/c-blosc2/doc/development/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/development/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/development/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/development/releasing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/development/roadmap.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.818865 blosc2-2.2.4/blosc2/c-blosc2/doc/format/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/format/cframe_format.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/format/chunk_format.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/format/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/format/sframe_format.rst
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.822865 blosc2-2.2.4/blosc2/c-blosc2/doc/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/reference/b2nd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/reference/blosc1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/reference/context.rst
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/reference/metalayers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/reference/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/reference/schunk.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/reference/utility.rst
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.830865 blosc2-2.2.4/blosc2/c-blosc2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.834865 blosc2-2.2.4/blosc2/c-blosc2/examples/b2nd/
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/b2nd/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/b2nd/example_empty_shape.c
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/b2nd/example_frame_generator.c
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/b2nd/example_oindex.c
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/b2nd/example_plainbuffer.c
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/b2nd/example_plugins_codecs.c
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/b2nd/example_plugins_filters.c
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/b2nd/example_print_meta.c
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/b2nd/example_serialize.c
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/compress_file.c
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/contexts.c
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/delta_schunk_ex.c
--rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/find_roots.c
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/frame_backed_schunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/frame_big.c
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/frame_metalayers.c
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/frame_offset.c
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/frame_roundtrip.c
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/frame_simple.c
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/frame_vlmetalayers.c
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/get_set_slice.c
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/instrument_codec.c
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/many_compressors.c
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/multithread.c
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/noinit.c
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/schunk_postfilter.c
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/schunk_simple.c
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/sframe_simple.c
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/simple.c
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/urcodecs.c
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/urfilters.c
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/win-dynamic-linking.c
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/examples/zstd_dict.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.838865 blosc2-2.2.4/blosc2/c-blosc2/images/
--rw-r--r--   0 runner    (1001) docker     (123)   116429 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/images/Complete-Write-Read-B2ND.png
--rw-r--r--   0 runner    (1001) docker     (123)   113029 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/images/Read-Partial-Slices-B2ND.png
--rw-r--r--   0 runner    (1001) docker     (123)   314966 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/images/b2nd-2level-parts.png
--rw-r--r--   0 runner    (1001) docker     (123)    45440 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/images/blosc2-pipeline.png
--rw-r--r--   0 runner    (1001) docker     (123)   491569 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/images/blosc2-pipeline.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.842865 blosc2-2.2.4/blosc2/c-blosc2/include/
--rw-r--r--   0 runner    (1001) docker     (123)    19739 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/include/b2nd.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.846865 blosc2-2.2.4/blosc2/c-blosc2/include/blosc2/
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/include/blosc2/blosc2-common.h
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/include/blosc2/blosc2-export.h
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/include/blosc2/blosc2-stdio.h
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/include/blosc2/codecs-registry.h
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/include/blosc2/filters-registry.h
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/include/blosc2/tuners-registry.h
--rw-r--r--   0 runner    (1001) docker     (123)    93824 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/include/blosc2.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.710863 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.846865 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)   113390 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.c
--rw-r--r--   0 runner    (1001) docker     (123)    43263 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.h
--rw-r--r--   0 runner    (1001) docker     (123)    70129 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.c
--rw-r--r--   0 runner    (1001) docker     (123)    20179 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.878866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/.shellcheckrc
--rw-r--r--   0 runner    (1001) docker     (123)    53620 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/FAQ.zlib
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/INDEX.md
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    13120 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/PORTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32.c
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32_p.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.882866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.882866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/adler32_neon.c
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/arm.h
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/armfeature.c
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/chunkset_neon.c
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/crc32_acle.c
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/ctzl.h
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/insert_string_acle.c
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/slide_neon.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.886866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/generic/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/generic/Makefile.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.886866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/adler32_power8.c
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/power.c
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/power.h
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/slide_hash_power8.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.890866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.c
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.h
--rw-r--r--   0 runner    (1001) docker     (123)    15189 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.c
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.h
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_detail.h
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.c
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.890866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.service
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.710863 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.710863 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.890866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      991 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/actions-runner
--rwxr-xr-x   0 runner    (1001) docker     (123)      740 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/entrypoint
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/qemu-user-static.service
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.898866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/INDEX.md
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_avx.c
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_ssse3.c
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_avx.c
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_sse.c
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_avx.c
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_sse.c
--rw-r--r--   0 runner    (1001) docker     (123)    16308 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.c
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.h
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/insert_string_sse.c
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_avx.c
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_sse.c
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/x86.c
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/x86.h
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset.c
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset_tpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.906866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.c
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-coverage.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-install-dirs.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-sanitizer.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-compare.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-redirect.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-compress.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-aarch64.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-arm.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-armhf.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-i686.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-x86_64.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64le.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-s390x.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-sparc64.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compare258.c
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compress.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    63492 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/configure
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32.c
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb.c
--rw-r--r--   0 runner    (1001) docker     (123)    13676 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl._h
--rw-r--r--   0 runner    (1001) docker     (123)    13676 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl.h
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_p.h
--rw-r--r--   0 runner    (1001) docker     (123)    26517 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl._h
--rw-r--r--   0 runner    (1001) docker     (123)    26517 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl.h
--rw-r--r--   0 runner    (1001) docker     (123)    69027 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.c
--rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.h
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_fast.c
--rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_medium.c
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_p.h
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_quick.c
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_slow.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.906866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/algorithm.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20502 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1950.txt
--rw-r--r--   0 runner    (1001) docker     (123)    36944 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1951.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25040 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1952.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/txtvsbin.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/fallback_builtins.h
--rw-r--r--   0 runner    (1001) docker     (123)    14849 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.c
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.h
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzguts.h
--rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzlib.c
--rw-r--r--   0 runner    (1001) docker     (123)    20278 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzread.c
--rw-r--r--   0 runner    (1001) docker     (123)    16106 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzwrite.c
--rw-r--r--   0 runner    (1001) docker     (123)    18689 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/infback.c
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.c
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.h
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl._h
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl.h
--rw-r--r--   0 runner    (1001) docker     (123)    48765 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.c
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.h
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate_p.h
--rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.c
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.h
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string.c
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string_tpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/match_tpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.918866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.918866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2002-0059/
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2002-0059/test.gz
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2003-0107.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.918866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2004-0797/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2004-0797/test.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.918866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-1849/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-1849/test.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.918866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-2096/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-2096/test.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.918866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/
--rw-r--r--   0 runner    (1001) docker     (123)    48192 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/default.txt
--rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/fixed.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.918866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-361/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-361/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.922866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-364/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-364/test.bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.922866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-382/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-382/defneg3.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.922866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-751/
--rw-r--r--   0 runner    (1001) docker     (123)   180001 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-751/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.922866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-979/
--rw-r--r--   0 runner    (1001) docker     (123)   106840 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-979/pigz-2.6.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.926866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/ignore
--rw-r--r--   0 runner    (1001) docker     (123)    14893 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-arm-linux-gnueabihf.abi
--rw-r--r--   0 runner    (1001) docker     (123)    90251 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-x86_64-linux-gnu.abi
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     4281 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.sh
--rw-r--r--   0 runner    (1001) docker     (123)    35507 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/adler32_test.c
--rw-r--r--   0 runner    (1001) docker     (123)    14167 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/crc32_test.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.926866 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)   123093 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/fireworks.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   419233 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/lcet10.txt
--rw-r--r--   0 runner    (1001) docker     (123)   102400 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/paper-100k.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_bi_valid.c
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_block_open.c
--rw-r--r--   0 runner    (1001) docker     (123)    33965 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/example.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.934867 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/checksum_fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/compress_fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_dict_fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_flush_fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_large_fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_small_fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/minigzip_fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/standalone_fuzz_target_runner.c
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/gh1235.c
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/hash_head_0.c
--rw-r--r--   0 runner    (1001) docker     (123)    26273 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/infcover.c
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/inflate_adler32.c
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minideflate.c
--rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minigzip.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.934867 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pigz/
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pigz/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pkgcheck.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/switchlevels.c
--rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/testCVEinputs.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.934867 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/codecov-upload.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      678 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/config.sub
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makecrct.c
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makefixed.c
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/maketrees.c
--rw-r--r--   0 runner    (1001) docker     (123)    31487 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.c
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.h
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_emit.h
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl._h
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl.h
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/uncompr.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.938867 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/
--rw-r--r--   0 runner    (1001) docker     (123)    17920 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/DLL_FAQ.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.a64
--rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.arm
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.msc
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/README-WIN32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng.def
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng1.rc
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib.def
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib1.rc
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlibcompat.def
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zbuild.h
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf-ng.h.in
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.in
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.included
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zendian.h
--rw-r--r--   0 runner    (1001) docker     (123)    94727 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.h
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.map
--rw-r--r--   0 runner    (1001) docker     (123)    94178 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.h
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.map
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.pc.cmakein
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.pc.in
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.c
--rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.h
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil_p.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.942867 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/BUCK
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.958867 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/allocations.h
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bits.h
--rw-r--r--   0 runner    (1001) docker     (123)    17522 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bitstream.h
--rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/compiler.h
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/cpu.h
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.c
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.h
--rw-r--r--   0 runner    (1001) docker     (123)    13308 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/entropy_common.c
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.c
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.h
--rw-r--r--   0 runner    (1001) docker     (123)    30110 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse.h
--rw-r--r--   0 runner    (1001) docker     (123)    12152 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/huf.h
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/mem.h
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.c
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.h
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/portability_macros.h
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.c
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.h
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.c
--rw-r--r--   0 runner    (1001) docker     (123)   212896 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.h
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_common.c
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_deps.h
--rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_trace.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.974867 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/clevels.h
--rw-r--r--   0 runner    (1001) docker     (123)    24096 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/fse_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.c
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.h
--rw-r--r--   0 runner    (1001) docker     (123)    57710 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/huf_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)   312776 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)    64416 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.c
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.h
--rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.c
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.h
--rw-r--r--   0 runner    (1001) docker     (123)    28499 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.c
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.h
--rw-r--r--   0 runner    (1001) docker     (123)    27872 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_cwksp.h
--rw-r--r--   0 runner    (1001) docker     (123)    34479 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.c
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.h
--rw-r--r--   0 runner    (1001) docker     (123)    36950 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.c
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.h
--rw-r--r--   0 runner    (1001) docker     (123)   101952 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.c
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.h
--rw-r--r--   0 runner    (1001) docker     (123)    28437 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.c
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.h
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm_geartab.h
--rw-r--r--   0 runner    (1001) docker     (123)    67459 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.c
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.h
--rw-r--r--   0 runner    (1001) docker     (123)    81334 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.978867 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/
--rw-r--r--   0 runner    (1001) docker     (123)    73701 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress_amd64.S
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.c
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.h
--rw-r--r--   0 runner    (1001) docker     (123)    99701 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)    99641 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.c
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.h
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_internal.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.982867 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/
--rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff.h
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_common.c
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_decompress.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.982867 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/
--rw-r--r--   0 runner    (1001) docker     (123)    42898 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.c
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.h
--rw-r--r--   0 runner    (1001) docker     (123)    54649 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.h
--rw-r--r--   0 runner    (1001) docker     (123)    28561 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/fastcover.c
--rw-r--r--   0 runner    (1001) docker     (123)    44008 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/zdict.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.714863 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.986868 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.sln
--rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.vcxproj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.994868 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)    14318 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_legacy.h
--rw-r--r--   0 runner    (1001) docker     (123)    69465 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.c
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.h
--rw-r--r--   0 runner    (1001) docker     (123)   125639 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.c
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.h
--rw-r--r--   0 runner    (1001) docker     (123)   111749 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.c
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.h
--rw-r--r--   0 runner    (1001) docker     (123)   132791 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.c
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.h
--rw-r--r--   0 runner    (1001) docker     (123)   153658 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.c
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.h
--rw-r--r--   0 runner    (1001) docker     (123)   163699 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.c
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.h
--rw-r--r--   0 runner    (1001) docker     (123)   182559 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.c
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.h
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/libzstd.mk
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/libzstd.pc.in
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/module.modulemap
--rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zdict.h
--rw-r--r--   0 runner    (1001) docker     (123)   171378 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd_errors.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.998868 blosc2-2.2.4/blosc2/c-blosc2/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.998868 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/codecs-registry.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.006868 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz-private.h
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.c
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.h
--rw-r--r--   0 runner    (1001) docker     (123)    23095 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.c
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.h
--rw-r--r--   0 runner    (1001) docker     (123)    19311 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.c
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.h
--rw-r--r--   0 runner    (1001) docker     (123)     9535 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/test_ndlz.c
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.c
--rw-r--r--   0 runner    (1001) docker     (123)   205061 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.010868 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    26699 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.c
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.010868 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/include/
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/include/bitstream.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.010868 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/macros.h
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/system.h
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/types.h
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/version.h
--rw-r--r--   0 runner    (1001) docker     (123)    34968 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.026868 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/bitstream.c
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/block1.h
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/block2.h
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/block3.h
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/block4.h
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1d.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1f.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1i.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1l.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2d.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2f.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2i.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2l.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3d.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3f.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3i.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3l.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4d.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4f.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4i.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4l.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1d.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1f.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1i.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1l.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2d.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2f.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2i.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2l.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3d.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3f.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3i.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3l.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4d.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4f.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4i.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4l.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.030868 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/
--rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/bitstream.c
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/inline.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.030868 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/share/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/share/omp.c
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/share/parallel.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.042868 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec.c
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec.h
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec1.c
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec2.c
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec3.c
--rw-r--r--   0 runner    (1001) docker     (123)     9466 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec4.c
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codecf.c
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/compress.c
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode.c
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode1.c
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode2.c
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode3.c
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode4.c
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decodef.c
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decodei.c
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode.c
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode1.c
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode2.c
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode3.c
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode4.c
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodef.c
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodei.c
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/ompcompress.c
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revcodecf.c
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode.c
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode1.c
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode2.c
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode3.c
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode4.c
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecodef.c
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode.c
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode1.c
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode2.c
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode3.c
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode4.c
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencodef.c
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/template.h
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsd.h
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsf.h
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsi.h
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsl.h
--rw-r--r--   0 runner    (1001) docker     (123)    32747 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/zfp.c
--rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_acc_float.c
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_prec_float.c
--rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_float.c
--rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_getitem.c
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/zfp-private.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.042868 blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.046868 blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/bytedelta/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/bytedelta/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.c
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.h
--rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/bytedelta/test_bytedelta.c
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/filters-registry.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.046868 blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndcell/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndcell/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndcell/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.c
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.h
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndcell/test_ndcell.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.050869 blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndmean/
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndmean/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndmean/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.c
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.h
--rw-r--r--   0 runner    (1001) docker     (123)    10410 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_mean.c
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_repart.c
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/plugin_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/plugin_utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.050869 blosc2-2.2.4/blosc2/c-blosc2/plugins/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/test_data/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/test_data/example_day_month_temp.b2nd
--rw-r--r--   0 runner    (1001) docker     (123)   141455 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/test_data/example_item_prices.b2nd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.050869 blosc2-2.2.4/blosc2/c-blosc2/plugins/tuners/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/tuners/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/plugins/tuners/tuners-registry.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.074869 blosc2-2.2.4/blosc2/c-blosc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.082869 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/cutest.h
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_append.c
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_copy.c
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_delete.c
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_full.c
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice.c
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice_buffer.c
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_insert.c
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_metalayers.c
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_open_offset.c
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_persistency.c
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_resize.c
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_roundtrip.c
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_save.c
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_serialize.c
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_set_slice_buffer.c
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze.c
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze_index.c
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_uninit.c
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_zeros.c
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_common.h
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/cutest.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.086869 blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.086869 blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/corpus/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/corpus/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    33187 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-blosclz.b2frame
--rw-r--r--   0 runner    (1001) docker     (123)    41393 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4.b2frame
--rw-r--r--   0 runner    (1001) docker     (123)    24087 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4hc.b2frame
--rw-r--r--   0 runner    (1001) docker     (123)    21570 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zlib.b2frame
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zstd.b2frame
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/fuzz_compress_chunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/fuzz_compress_frame.c
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_chunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_frame.c
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/generate_inputs_corpus.c
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/standalone.c
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/gcc-segfault-issue.c
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/print_versions.c
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_all.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_api.c
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_bitshuffle_leftovers.c
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_blosc1_compat.c
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_change_nthreads_append.c
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_common.h
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_compress_roundtrip.c
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_compress_roundtrip.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_compressor.c
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_contexts.c
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_copy.c
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_delete_chunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_delta.c
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_delta_schunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_dict_schunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_empty_buffer.c
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_fill_special.c
--rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_frame.c
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_frame_get_offsets.c
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_frame_offset.c
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_get_slice_buffer.c
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_getitem.c
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_getitem.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_getitem_delta.c
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_insert_chunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_lazychunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_lazychunk_memcpyed.c
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_maskout.c
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_maxout.c
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_noinit.c
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_nolock.c
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_nthreads.c
--rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_postfilter.c
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_prefilter.c
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_reorder_offsets.c
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_schunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_schunk_frame.c
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_schunk_header.c
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_set_slice_buffer.c
--rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_sframe.c
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_sframe_lazychunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.c
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.c
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.c
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.c
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.c
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_small_chunks.c
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_udio.c
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_update_chunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_urcodecs.c
--rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_urfilters.c
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-21 11:59:25.000000 blosc2-2.2.4/blosc2/c-blosc2/tests/test_zero_runlen.c
--rw-r--r--   0 runner    (1001) docker     (123)    46299 2023-06-21 11:59:24.000000 blosc2-2.2.4/blosc2/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-21 11:59:24.000000 blosc2-2.2.4/blosc2/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    21243 2023-06-21 11:59:24.000000 blosc2-2.2.4/blosc2/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    32418 2023-06-21 11:59:24.000000 blosc2-2.2.4/blosc2/schunk.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 12:01:26.000000 blosc2-2.2.4/blosc2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.734863 blosc2-2.2.4/blosc2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-06-21 12:01:26.000000 blosc2-2.2.4/blosc2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    53235 2023-06-21 12:01:26.000000 blosc2-2.2.4/blosc2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 12:01:26.000000 blosc2-2.2.4/blosc2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-21 12:01:26.000000 blosc2-2.2.4/blosc2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 12:01:26.000000 blosc2-2.2.4/blosc2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-21 11:59:24.000000 blosc2-2.2.4/code_of_conduct.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.086869 blosc2-2.2.4/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.090869 blosc2-2.2.4/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/_static/blosc-logo_128.png
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/_static/blosc-logo_256.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.090869 blosc2-2.2.4/doc/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.090869 blosc2-2.2.4/doc/development/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/development/code-of-conduct.rst
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/development/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/development/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.090869 blosc2-2.2.4/doc/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.094869 blosc2-2.2.4/doc/getting_started/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/tutorials/00.schunk-basics.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/tutorials/01.schunk-slicing_and_beyond.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    22039 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/tutorials/02.ndarray-basics.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    19380 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/tutorials/10.ucodecs-ufilters.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/tutorials/11.prefilters.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/tutorials/12.postfilters.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.094869 blosc2-2.2.4/doc/getting_started/tutorials/images/
--rw-r--r--   0 runner    (1001) docker     (123)    45440 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/tutorials/images/blosc2-pipeline.png
--rw-r--r--   0 runner    (1001) docker     (123)   491569 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/tutorials/images/blosc2-pipeline.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.102869 blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/
--rw-r--r--   0 runner    (1001) docker     (123)   107624 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/backward.png
--rw-r--r--   0 runner    (1001) docker     (123)    38548 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/backward.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/decoder.png
--rw-r--r--   0 runner    (1001) docker     (123)    31483 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/decoder.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/decoder2.png
--rw-r--r--   0 runner    (1001) docker     (123)    35540 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/decoder2.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/encoder.png
--rw-r--r--   0 runner    (1001) docker     (123)    23248 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/encoder.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/encoder2.png
--rw-r--r--   0 runner    (1001) docker     (123)    24481 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/encoder2.svg
--rw-r--r--   0 runner    (1001) docker     (123)   110817 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/forward.png
--rw-r--r--   0 runner    (1001) docker     (123)    41521 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/forward.svg
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/getting_started/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/python-blosc2.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.102869 blosc2-2.2.4/doc/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:26.714863 blosc2-2.2.4/doc/reference/autofiles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.110870 blosc2-2.2.4/doc/reference/autofiles/schunk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.114869 blosc2-2.2.4/doc/reference/autofiles/schunk/attributes/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.blocksize.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.cbytes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.chunkshape.rst
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.chunksize.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.contiguous.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.cparams.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.cratio.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.dparams.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.nbytes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.typesize.rst
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.urlpath.rst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/attributes/meta.rst
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/attributes/vlmeta.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.__getitem__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.__setitem__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.append_data.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.decompress_chunk.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.delete_chunk.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.filler.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.get_chunk.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.get_slice.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.insert_chunk.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.insert_data.rst
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.iterchunks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.iterchunks_info.rst
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.postfilter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.prefilter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.remove_postfilter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.remove_prefilter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.to_cframe.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.update_chunk.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.update_data.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.114869 blosc2-2.2.4/doc/reference/autofiles/top_level/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/top_level/blosc2.Codec.rst
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/top_level/blosc2.Filter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/top_level/blosc2.SplitMode.rst
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/autofiles/top_level/blosc2.nthreads.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/ndarray_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/schunk_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/reference/top_level.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.114869 blosc2-2.2.4/doc/release_notes/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 11:59:24.000000 blosc2-2.2.4/doc/release_notes/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.118870 blosc2-2.2.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/compress2_decompress2.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/compress_decompress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/filler.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/gil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.122870 blosc2-2.2.4/examples/ndarray/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/ndarray/asarray_.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/ndarray/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/ndarray/bytedelta_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/ndarray/copy_.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/ndarray/empty_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/ndarray/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/ndarray/getitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/ndarray/iterchunks_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/ndarray/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/ndarray/ndarray_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/ndarray/ndmean.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/ndarray/persistency.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/ndarray/resize_.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/ndarray/work_with_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/ndarray/zfp_codec.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/pack_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/pack_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/postfilter1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/postfilter2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/postfilter3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/prefilter.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/save_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/schunk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/schunk_roundtrip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2114 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/ucodecs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/ufilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-21 11:59:24.000000 blosc2-2.2.4/examples/vlmeta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.130870 blosc2-2.2.4/images/
--rw-r--r--   0 runner    (1001) docker     (123)   116429 2023-06-21 11:59:24.000000 blosc2-2.2.4/images/Complete-Write-Read-B2ND.png
--rw-r--r--   0 runner    (1001) docker     (123)    64898 2023-06-21 11:59:24.000000 blosc2-2.2.4/images/M1-i386-vs-arm64-pack.png
--rw-r--r--   0 runner    (1001) docker     (123)    62528 2023-06-21 11:59:24.000000 blosc2-2.2.4/images/M1-i386-vs-arm64-unpack.png
--rw-r--r--   0 runner    (1001) docker     (123)   113029 2023-06-21 11:59:24.000000 blosc2-2.2.4/images/Read-Partial-Slices-B2ND.png
--rw-r--r--   0 runner    (1001) docker     (123)   314966 2023-06-21 11:59:24.000000 blosc2-2.2.4/images/b2nd-2level-parts.png
--rw-r--r--   0 runner    (1001) docker     (123)    77813 2023-06-21 11:59:24.000000 blosc2-2.2.4/images/linspace-compress.png
--rw-r--r--   0 runner    (1001) docker     (123)    24888 2023-06-21 11:59:24.000000 blosc2-2.2.4/images/linspace-decompress.png
--rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-06-21 11:59:24.000000 blosc2-2.2.4/images/pack-array-cratios.png
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-21 11:59:24.000000 blosc2-2.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-21 11:59:24.000000 blosc2-2.2.4/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 11:59:24.000000 blosc2-2.2.4/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-21 11:59:24.000000 blosc2-2.2.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-21 11:59:24.000000 blosc2-2.2.4/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-21 11:59:24.000000 blosc2-2.2.4/requirements-runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 11:59:24.000000 blosc2-2.2.4/requirements-test-wheels.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-21 11:59:24.000000 blosc2-2.2.4/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 12:01:27.142870 blosc2-2.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-21 11:59:24.000000 blosc2-2.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.138870 blosc2-2.2.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:01:27.142870 blosc2-2.2.4/tests/ndarray/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/ndarray/persistency.cat
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/ndarray/test_auto_parts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/ndarray/test_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/ndarray/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/ndarray/test_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/ndarray/test_full.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/ndarray/test_getitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/ndarray/test_iterchunks_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/ndarray/test_lossy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/ndarray/test_metalayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/ndarray/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/ndarray/test_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/ndarray/test_persistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/ndarray/test_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/ndarray/test_setitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/ndarray/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/ndarray/test_squeeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/ndarray/test_struct_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/ndarray/test_zeros.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/test_bytes_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/test_comp_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/test_compress2.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/test_compression_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/test_compressors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/test_decompress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/test_iterchunks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/test_postfilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/test_prefilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/test_python_blosc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/test_schunk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/test_schunk_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/test_schunk_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/test_schunk_get_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/test_schunk_insert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/test_schunk_set_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/test_schunk_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/test_ucodecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/test_ufilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-21 11:59:24.000000 blosc2-2.2.4/tests/test_vlmeta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.818125 blosc2-2.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-04 06:06:47.000000 blosc2-2.2.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.430122 blosc2-2.2.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-04 06:06:47.000000 blosc2-2.2.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.430122 blosc2-2.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-04 06:06:47.000000 blosc2-2.2.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-07-04 06:06:47.000000 blosc2-2.2.5/.github/workflows/cibuildwheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-04 06:06:47.000000 blosc2-2.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-04 06:06:47.000000 blosc2-2.2.5/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-04 06:06:47.000000 blosc2-2.2.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-04 06:06:47.000000 blosc2-2.2.5/ANNOUNCE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-04 06:06:47.000000 blosc2-2.2.5/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-04 06:06:47.000000 blosc2-2.2.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-04 06:06:47.000000 blosc2-2.2.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-07-04 06:08:53.818125 blosc2-2.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-07-04 06:06:47.000000 blosc2-2.2.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-04 06:06:47.000000 blosc2-2.2.5/README_DEVELOPERS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-07-04 06:06:47.000000 blosc2-2.2.5/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-04 06:06:47.000000 blosc2-2.2.5/RELEASING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 06:06:47.000000 blosc2-2.2.5/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.430122 blosc2-2.2.5/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-04 06:06:47.000000 blosc2-2.2.5/bench/compress_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-04 06:06:47.000000 blosc2-2.2.5/bench/get_slice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.434122 blosc2-2.2.5/bench/ndarray/
+-rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-07-04 06:06:47.000000 blosc2-2.2.5/bench/ndarray/compare_getslice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-04 06:06:47.000000 blosc2-2.2.5/bench/ndarray/copy_postfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-04 06:06:47.000000 blosc2-2.2.5/bench/ndarray/download_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.434122 blosc2-2.2.5/bench/ndarray/era5-pds/
+-rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-07-04 06:06:47.000000 blosc2-2.2.5/bench/ndarray/era5-pds/measurements-i10k.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-07-04 06:06:47.000000 blosc2-2.2.5/bench/ndarray/era5-pds/measurements-i13k-always-split.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    16476 2023-07-04 06:06:47.000000 blosc2-2.2.5/bench/ndarray/era5-pds/measurements-i13k-never-split.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    16500 2023-07-04 06:06:47.000000 blosc2-2.2.5/bench/ndarray/era5-pds/measurements-i13k.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    16500 2023-07-04 06:06:47.000000 blosc2-2.2.5/bench/ndarray/era5-pds/measurements-m1.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-07-04 06:06:47.000000 blosc2-2.2.5/bench/ndarray/era5-pds/measurements-ryzen3.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    10749 2023-07-04 06:06:47.000000 blosc2-2.2.5/bench/ndarray/plot_transcode_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-04 06:06:47.000000 blosc2-2.2.5/bench/ndarray/transcode_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-04 06:06:47.000000 blosc2-2.2.5/bench/pack_compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-04 06:06:47.000000 blosc2-2.2.5/bench/pack_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-04 06:06:47.000000 blosc2-2.2.5/bench/pack_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-04 06:06:47.000000 blosc2-2.2.5/bench/set_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-04 06:06:47.000000 blosc2-2.2.5/bench/sum_postfilter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.438122 blosc2-2.2.5/blosc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-04 06:06:47.000000 blosc2-2.2.5/blosc2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-04 06:06:47.000000 blosc2-2.2.5/blosc2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88179 2023-07-04 06:06:47.000000 blosc2-2.2.5/blosc2/blosc2_ext.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.450122 blosc2-2.2.5/blosc2/c-blosc2/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.450122 blosc2-2.2.5/blosc2/c-blosc2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.450122 blosc2-2.2.5/blosc2/c-blosc2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.450122 blosc2-2.2.5/blosc2/c-blosc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/.github/workflows/cmake.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/.github/workflows/fuzz.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/ANNOUNCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/COMPILING_WITH_WHEELS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/DEVELOPING-GUIDE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/FAQ.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.454122 blosc2-2.2.5/blosc2/c-blosc2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/LICENSES/BITSHUFFLE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/LICENSES/FASTLZ.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/LICENSES/LZ4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/LICENSES/ZLIB.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/LICENSES/ZSTD.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16795 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15951 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/README_ARM.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/README_B2ND_METALAYER.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13926 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/README_CFRAME_FORMAT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/README_CHUNK_FORMAT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/README_FUZZER.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/README_SFRAME_FORMAT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/README_THREADED.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    27358 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/RELEASING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/ROADMAP.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/THANKS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/TODO-refactorization.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.458122 blosc2-2.2.5/blosc2/c-blosc2/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/Makefile.mingw
+-rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/b2bench.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.458122 blosc2-2.2.5/blosc2/c-blosc2/bench/b2nd/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/b2nd/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/b2nd/bench_get_slice.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/b2nd/bench_zfp_getitem.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/create_frame.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/delta_schunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/plot-speeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/plot-sum_openmp-results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/rainfall-grid-150x150.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/read-grid-150x150.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.462122 blosc2-2.2.5/blosc2/c-blosc2/bench/results-corex/
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/results-corex/blosclz-cl1-sum_openmp-corex.out
+-rw-r--r--   0 runner    (1001) docker     (123)    29803 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/results-corex/blosclz-suite-corex.out
+-rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/results-corex/lz4-cl1-sum_openmp-corex.out
+-rw-r--r--   0 runner    (1001) docker     (123)    29683 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/results-corex/lz4-suite-corex.out
+-rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/results-corex/lz4hc-cl1-sum_openmp-corex.out
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/results-corex/zlib-cl1-sum_openmp-corex.out
+-rw-r--r--   0 runner    (1001) docker     (123)    11248 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/results-corex/zstd-cl1-sum_openmp-corex.out
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/sframe_bench.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/sum_openmp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/trunc_prec_schunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/bench/zero_runlen.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.482123 blosc2-2.2.5/blosc2/c-blosc2/blosc/
+-rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    64356 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/b2nd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/b2nd_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/b2nd_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21593 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/bitshuffle-altivec.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/bitshuffle-altivec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/bitshuffle-avx2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/bitshuffle-avx2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/bitshuffle-generic.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/bitshuffle-generic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    49620 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/bitshuffle-neon.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/bitshuffle-neon.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15933 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/bitshuffle-sse2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/bitshuffle-sse2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/blosc-private.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/blosc2-stdio.c
+-rw-r--r--   0 runner    (1001) docker     (123)   151481 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/blosc2.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24339 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/blosclz.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/blosclz.h
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/config.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/context.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/delta.c
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/delta.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/directories.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16723 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/fastcopy.c
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/fastcopy.h
+-rw-r--r--   0 runner    (1001) docker     (123)   115804 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/frame.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/frame.h
+-rw-r--r--   0 runner    (1001) docker     (123)    56494 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/schunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/sframe.c
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/sframe.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15715 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle-altivec.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle-altivec.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31648 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle-avx2.c
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle-avx2.h
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle-generic.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle-generic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22000 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle-neon.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle-neon.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26157 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle-sse2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle-sse2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19569 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/stune.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/stune.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/timestamp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/transpose-altivec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/trunc-prec.c
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/trunc-prec.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.482123 blosc2-2.2.5/blosc2/c-blosc2/blosc/win32/
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/win32/pthread.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc/win32/pthread.h
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/blosc2.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.482123 blosc2-2.2.5/blosc2/c-blosc2/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/cmake/FindIPP.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/cmake/FindLZ4.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/cmake/FindSIMD.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/cmake/FindZLIB_NG.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/cmake/FindZSTD.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/cmake/toolchain-aarch64.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/cmake/toolchain-armhf.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/cmake/toolchain-armsf.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/code_of_conduct.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.498123 blosc2-2.2.5/blosc2/c-blosc2/compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26736 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.11.1-blosclz.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    33610 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.11.1-lz4.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    32485 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.11.1-lz4hc.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.11.1-zlib.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.11.1-zstd.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    36256 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.14.0-blosclz.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    36267 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.14.0-lz4.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    36263 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.14.0-lz4hc.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    20530 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.14.0-zlib.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.14.0-zstd.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)   141205 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle4-memcpy.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    22760 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle8-nomemcpy.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    27787 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle4-memcpy.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    22760 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle8-nomemcpy.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    36349 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.3.0-blosclz.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    36267 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.3.0-lz4.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    31963 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.3.0-lz4hc.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    14956 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.3.0-zlib.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    36394 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.7.0-blosclz.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    36267 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.7.0-lz4.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    31963 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.7.0-lz4hc.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    14956 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.7.0-zlib.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    15763 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle4-memcpy.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle8-nomemcpy.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/compat/filegen.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.498123 blosc2-2.2.5/blosc2/c-blosc2/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.414122 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.498123 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6974 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test1.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23072 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test16.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8642 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test2.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11457 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test4.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14436 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test8.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.498123 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10706 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16818 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.498123 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4846 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.502122 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2262 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7896 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7574 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.502122 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3708 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7910 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.502122 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5792 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11472 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.502122 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8199 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24719 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.502122 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1376 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4233 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.502122 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2214 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7559 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.506122 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3616 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13037 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.506122 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4479 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15834 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.414122 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.506122 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/Test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10906 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test16.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2162 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test2.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2769 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test4.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6545 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test8.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.510123 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7713 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_bucle.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4630 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8365 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.510123 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2577 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.510123 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      756 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2997 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.510123 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2268 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4883 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_bucle.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2711 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6813 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt_bucle.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2010 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5787 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.514123 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3949 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7649 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_bucle.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4177 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7353 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.514123 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      656 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2212 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.514123 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle4_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      770 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle4_neon/unshuffle4_neon.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.514123 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2279 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5550 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_bucle.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2737 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4987 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.518123 blosc2-2.2.5/blosc2/c-blosc2/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.518123 blosc2-2.2.5/blosc2/c-blosc2/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/_static/blosc-logo_256.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.518123 blosc2-2.2.5/blosc2/c-blosc2/doc/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/c-blosc2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.518123 blosc2-2.2.5/blosc2/c-blosc2/doc/development/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/development/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/development/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/development/releasing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/development/roadmap.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.522123 blosc2-2.2.5/blosc2/c-blosc2/doc/format/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/format/cframe_format.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/format/chunk_format.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/format/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/format/sframe_format.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.522123 blosc2-2.2.5/blosc2/c-blosc2/doc/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/reference/b2nd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/reference/blosc1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/reference/context.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/reference/metalayers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/reference/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/reference/schunk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/reference/utility.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.530123 blosc2-2.2.5/blosc2/c-blosc2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.534123 blosc2-2.2.5/blosc2/c-blosc2/examples/b2nd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/b2nd/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/b2nd/example_empty_shape.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/b2nd/example_frame_generator.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/b2nd/example_oindex.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/b2nd/example_plainbuffer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/b2nd/example_plugins_codecs.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/b2nd/example_plugins_filters.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/b2nd/example_print_meta.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/b2nd/example_serialize.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/compress_file.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/contexts.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/delta_schunk_ex.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/find_roots.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/frame_backed_schunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/frame_big.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/frame_metalayers.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/frame_offset.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/frame_roundtrip.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/frame_simple.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/frame_vlmetalayers.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/get_set_slice.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/instrument_codec.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/many_compressors.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/multithread.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/noinit.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/schunk_postfilter.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/schunk_simple.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/sframe_simple.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/simple.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/urcodecs.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/urfilters.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/win-dynamic-linking.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/examples/zstd_dict.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.538123 blosc2-2.2.5/blosc2/c-blosc2/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   116429 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/images/Complete-Write-Read-B2ND.png
+-rw-r--r--   0 runner    (1001) docker     (123)   113029 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/images/Read-Partial-Slices-B2ND.png
+-rw-r--r--   0 runner    (1001) docker     (123)   314966 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/images/b2nd-2level-parts.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45440 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/images/blosc2-pipeline.png
+-rw-r--r--   0 runner    (1001) docker     (123)   491569 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/images/blosc2-pipeline.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.542123 blosc2-2.2.5/blosc2/c-blosc2/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    19739 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/include/b2nd.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.546123 blosc2-2.2.5/blosc2/c-blosc2/include/blosc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/include/blosc2/blosc2-common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/include/blosc2/blosc2-export.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/include/blosc2/blosc2-stdio.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/include/blosc2/codecs-registry.h
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/include/blosc2/filters-registry.h
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/include/blosc2/tuners-registry.h
+-rw-r--r--   0 runner    (1001) docker     (123)    93839 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/include/blosc2.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.418122 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.546123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)   113390 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.c
+-rw-r--r--   0 runner    (1001) docker     (123)    43263 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.h
+-rw-r--r--   0 runner    (1001) docker     (123)    70129 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20179 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.574123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/.shellcheckrc
+-rw-r--r--   0 runner    (1001) docker     (123)    53620 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/FAQ.zlib
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/INDEX.md
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13120 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/PORTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32_p.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.574123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.578123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/adler32_neon.c
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/arm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/armfeature.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/chunkset_neon.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/crc32_acle.c
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/ctzl.h
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/insert_string_acle.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/slide_neon.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.578123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/generic/Makefile.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.578123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/adler32_power8.c
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/power.c
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/power.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/slide_hash_power8.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.582123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15189 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_detail.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.582123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.service
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.418122 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.418122 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.586123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      991 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/actions-runner
+-rwxr-xr-x   0 runner    (1001) docker     (123)      740 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/entrypoint
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/qemu-user-static.service
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.590123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/INDEX.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_avx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_ssse3.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_avx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_sse.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_avx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_sse.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16308 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.c
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/insert_string_sse.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_avx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_sse.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/x86.c
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/x86.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset_tpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.594123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-coverage.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-install-dirs.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-sanitizer.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-compare.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-redirect.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-compress.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-aarch64.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-arm.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-armhf.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-i686.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-x86_64.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64le.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-s390x.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-sparc64.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compare258.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compress.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    63492 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/configure
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13676 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl._h
+-rw-r--r--   0 runner    (1001) docker     (123)    13676 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl.h
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_p.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26517 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl._h
+-rw-r--r--   0 runner    (1001) docker     (123)    26517 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    69027 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_fast.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_medium.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_p.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_quick.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_slow.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.598123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/algorithm.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20502 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1950.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    36944 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1951.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25040 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1952.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/txtvsbin.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/fallback_builtins.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14849 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzguts.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzlib.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20278 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzread.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16106 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzwrite.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18689 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/infback.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.c
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl._h
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    48765 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate_p.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.h
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string_tpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/match_tpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.606123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.606123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2002-0059/
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2002-0059/test.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2003-0107.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.606123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2004-0797/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2004-0797/test.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.606123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-1849/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-1849/test.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.606123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-2096/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-2096/test.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.606123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/
+-rw-r--r--   0 runner    (1001) docker     (123)    48192 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/default.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/fixed.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.606123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-361/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-361/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.610123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-364/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-364/test.bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.610123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-382/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-382/defneg3.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.610123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-751/
+-rw-r--r--   0 runner    (1001) docker     (123)   180001 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-751/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.610123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-979/
+-rw-r--r--   0 runner    (1001) docker     (123)   106840 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-979/pigz-2.6.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.610123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/ignore
+-rw-r--r--   0 runner    (1001) docker     (123)    14893 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-arm-linux-gnueabihf.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    90251 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-x86_64-linux-gnu.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4281 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    35507 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/adler32_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14167 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/crc32_test.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.614123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   123093 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/fireworks.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   419233 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/lcet10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   102400 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/paper-100k.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_bi_valid.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_block_open.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33965 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/example.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.618123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/checksum_fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/compress_fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_dict_fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_flush_fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_large_fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_small_fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/minigzip_fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/standalone_fuzz_target_runner.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/gh1235.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/hash_head_0.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26273 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/infcover.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/inflate_adler32.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minideflate.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minigzip.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.618123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pigz/
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pigz/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pkgcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/switchlevels.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/testCVEinputs.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.622123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/codecov-upload.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      678 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/config.sub
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makecrct.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makefixed.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/maketrees.c
+-rw-r--r--   0 runner    (1001) docker     (123)    31487 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_emit.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl._h
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/uncompr.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.622123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/
+-rw-r--r--   0 runner    (1001) docker     (123)    17920 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/DLL_FAQ.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.a64
+-rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.arm
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.msc
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/README-WIN32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng.def
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng1.rc
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib.def
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib1.rc
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlibcompat.def
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zbuild.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf-ng.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.included
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zendian.h
+-rw-r--r--   0 runner    (1001) docker     (123)    94727 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.map
+-rw-r--r--   0 runner    (1001) docker     (123)    94178 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.map
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.pc.cmakein
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.pc.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil_p.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.626123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/BUCK
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.638123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/allocations.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bits.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17522 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bitstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/compiler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/cpu.h
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13308 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/entropy_common.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30110 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12152 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/huf.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/mem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/portability_macros.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.h
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.c
+-rw-r--r--   0 runner    (1001) docker     (123)   212896 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_common.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_deps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_trace.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.650123 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/clevels.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24096 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/fse_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57710 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/huf_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)   312776 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    64416 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28499 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27872 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_cwksp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34479 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36950 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.h
+-rw-r--r--   0 runner    (1001) docker     (123)   101952 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28437 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm_geartab.h
+-rw-r--r--   0 runner    (1001) docker     (123)    67459 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    81334 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.654124 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/
+-rw-r--r--   0 runner    (1001) docker     (123)    73701 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress_amd64.S
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.h
+-rw-r--r--   0 runner    (1001) docker     (123)    99701 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    99641 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.658124 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_common.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_decompress.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.662124 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)    42898 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.h
+-rw-r--r--   0 runner    (1001) docker     (123)    54649 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28561 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/fastcover.c
+-rw-r--r--   0 runner    (1001) docker     (123)    44008 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/zdict.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.422122 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.662124 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.sln
+-rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.vcxproj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.674124 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)    14318 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_legacy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    69465 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.h
+-rw-r--r--   0 runner    (1001) docker     (123)   125639 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.h
+-rw-r--r--   0 runner    (1001) docker     (123)   111749 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.h
+-rw-r--r--   0 runner    (1001) docker     (123)   132791 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.h
+-rw-r--r--   0 runner    (1001) docker     (123)   153658 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.h
+-rw-r--r--   0 runner    (1001) docker     (123)   163699 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.h
+-rw-r--r--   0 runner    (1001) docker     (123)   182559 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/libzstd.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/libzstd.pc.in
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/module.modulemap
+-rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zdict.h
+-rw-r--r--   0 runner    (1001) docker     (123)   171378 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd_errors.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.674124 blosc2-2.2.5/blosc2/c-blosc2/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.674124 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/codecs-registry.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.678124 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz-private.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.c
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23095 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19311 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9535 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/test_ndlz.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.c
+-rw-r--r--   0 runner    (1001) docker     (123)   205061 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.682124 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    26699 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.682124 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/include/bitstream.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.686124 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/macros.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/system.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/version.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34968 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.698124 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/bitstream.c
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/block1.h
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/block2.h
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/block3.h
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/block4.h
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1d.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1f.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1i.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1l.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2d.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2f.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2i.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2l.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3d.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3f.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3i.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3l.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4d.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4f.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4i.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4l.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1d.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1f.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1i.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1l.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2d.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2f.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2i.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2l.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3d.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3f.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3i.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3l.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4d.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4f.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4i.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4l.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.698124 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/
+-rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/bitstream.c
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/inline.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.698124 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/share/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/share/omp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/share/parallel.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.714124 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec.c
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec.h
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec1.c
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec3.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9466 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec4.c
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codecf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode3.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode4.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decodef.c
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decodei.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode3.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode4.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodef.c
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodei.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/ompcompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revcodecf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode.c
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode1.c
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode2.c
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode3.c
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode4.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecodef.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode.c
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode1.c
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode2.c
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode3.c
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode4.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencodef.c
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/template.h
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsd.h
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsi.h
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32747 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/zfp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_acc_float.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_prec_float.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_float.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_getitem.c
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/zfp-private.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.714124 blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.714124 blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/bytedelta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/bytedelta/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/bytedelta/test_bytedelta.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/filters-registry.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.714124 blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndcell/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndcell/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndcell/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.c
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndcell/test_ndcell.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.718124 blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndmean/
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndmean/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndmean/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.c
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10410 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_mean.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_repart.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/plugin_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/plugin_utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.718124 blosc2-2.2.5/blosc2/c-blosc2/plugins/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/test_data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/test_data/example_day_month_temp.b2nd
+-rw-r--r--   0 runner    (1001) docker     (123)   141455 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/test_data/example_item_prices.b2nd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.718124 blosc2-2.2.5/blosc2/c-blosc2/plugins/tuners/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/tuners/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/plugins/tuners/tuners-registry.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.742124 blosc2-2.2.5/blosc2/c-blosc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.754124 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/cutest.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_append.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_copy.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_delete.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_full.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_insert.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_metalayers.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_open_offset.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_persistency.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_resize.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_roundtrip.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_save.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_serialize.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_set_slice_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze_index.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_uninit.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_zeros.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/cutest.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.754124 blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.758124 blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/corpus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/corpus/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    33187 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-blosclz.b2frame
+-rw-r--r--   0 runner    (1001) docker     (123)    41393 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4.b2frame
+-rw-r--r--   0 runner    (1001) docker     (123)    24087 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4hc.b2frame
+-rw-r--r--   0 runner    (1001) docker     (123)    21570 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zlib.b2frame
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zstd.b2frame
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/fuzz_compress_chunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/fuzz_compress_frame.c
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_chunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_frame.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/generate_inputs_corpus.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/standalone.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/gcc-segfault-issue.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/print_versions.c
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_all.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_api.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_bitshuffle_leftovers.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_blosc1_compat.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_change_nthreads_append.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_compress_roundtrip.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_compress_roundtrip.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_compressor.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_contexts.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_copy.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_delete_chunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_delta.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_delta_schunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_dict_schunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_empty_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_fill_special.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_filters.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_frame.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_frame_get_offsets.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_frame_offset.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_get_slice_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_getitem.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_getitem.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_getitem_delta.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_insert_chunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_lazychunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_lazychunk_memcpyed.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_maskout.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_maxout.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_noinit.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_nolock.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_nthreads.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_postfilter.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_prefilter.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_reorder_offsets.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_schunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_schunk_frame.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_schunk_header.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_set_slice_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_sframe.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_sframe_lazychunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_small_chunks.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_udio.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_update_chunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_urcodecs.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_urfilters.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-04 06:06:48.000000 blosc2-2.2.5/blosc2/c-blosc2/tests/test_zero_runlen.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46299 2023-07-04 06:06:47.000000 blosc2-2.2.5/blosc2/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-04 06:06:47.000000 blosc2-2.2.5/blosc2/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21243 2023-07-04 06:06:47.000000 blosc2-2.2.5/blosc2/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32418 2023-07-04 06:06:47.000000 blosc2-2.2.5/blosc2/schunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 06:08:53.000000 blosc2-2.2.5/blosc2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.438122 blosc2-2.2.5/blosc2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-07-04 06:08:53.000000 blosc2-2.2.5/blosc2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    53272 2023-07-04 06:08:53.000000 blosc2-2.2.5/blosc2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 06:08:53.000000 blosc2-2.2.5/blosc2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-04 06:08:53.000000 blosc2-2.2.5/blosc2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 06:08:53.000000 blosc2-2.2.5/blosc2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-04 06:06:47.000000 blosc2-2.2.5/code_of_conduct.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.758124 blosc2-2.2.5/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.758124 blosc2-2.2.5/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/_static/blosc-logo_128.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/_static/blosc-logo_256.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.762124 blosc2-2.2.5/doc/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.762124 blosc2-2.2.5/doc/development/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/development/code-of-conduct.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/development/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/development/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.762124 blosc2-2.2.5/doc/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.766124 blosc2-2.2.5/doc/getting_started/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    11847 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/tutorials/00.schunk-basics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/tutorials/01.schunk-slicing_and_beyond.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    21986 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/tutorials/02.ndarray-basics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19380 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/tutorials/10.ucodecs-ufilters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/tutorials/11.prefilters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/tutorials/12.postfilters.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.766124 blosc2-2.2.5/doc/getting_started/tutorials/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    45440 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/tutorials/images/blosc2-pipeline.png
+-rw-r--r--   0 runner    (1001) docker     (123)   491569 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/tutorials/images/blosc2-pipeline.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.774124 blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/
+-rw-r--r--   0 runner    (1001) docker     (123)   107624 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/backward.png
+-rw-r--r--   0 runner    (1001) docker     (123)    38548 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/backward.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/decoder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31483 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/decoder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/decoder2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35540 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/decoder2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/encoder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23248 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/encoder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/encoder2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24481 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/encoder2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   110817 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/forward.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41521 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/forward.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/getting_started/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/python-blosc2.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.774124 blosc2-2.2.5/doc/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.422122 blosc2-2.2.5/doc/reference/autofiles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.782124 blosc2-2.2.5/doc/reference/autofiles/schunk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.786124 blosc2-2.2.5/doc/reference/autofiles/schunk/attributes/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.blocksize.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.cbytes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.chunkshape.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.chunksize.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.contiguous.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.cparams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.cratio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.dparams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.nbytes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.typesize.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.urlpath.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/attributes/meta.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/attributes/vlmeta.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.__getitem__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.__setitem__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.append_data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.decompress_chunk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.delete_chunk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.filler.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.get_chunk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.get_slice.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.insert_chunk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.insert_data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.iterchunks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.iterchunks_info.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.postfilter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.prefilter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.remove_postfilter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.remove_prefilter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.to_cframe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.update_chunk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.update_data.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.786124 blosc2-2.2.5/doc/reference/autofiles/top_level/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/top_level/blosc2.Codec.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/top_level/blosc2.Filter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/top_level/blosc2.SplitMode.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/autofiles/top_level/blosc2.nthreads.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/ndarray_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/schunk_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/reference/top_level.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.790125 blosc2-2.2.5/doc/release_notes/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-04 06:06:47.000000 blosc2-2.2.5/doc/release_notes/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.794124 blosc2-2.2.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/compress2_decompress2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/compress_decompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/filler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/gil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.798124 blosc2-2.2.5/examples/ndarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/ndarray/asarray_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/ndarray/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/ndarray/bytedelta_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/ndarray/copy_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/ndarray/empty_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/ndarray/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/ndarray/getitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/ndarray/iterchunks_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/ndarray/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/ndarray/ndarray_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/ndarray/ndmean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/ndarray/persistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/ndarray/resize_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/ndarray/work_with_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/ndarray/zfp_codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/pack_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/pack_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/postfilter1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/postfilter2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/postfilter3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/prefilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/save_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/schunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/schunk_roundtrip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2114 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/ucodecs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/ufilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-04 06:06:47.000000 blosc2-2.2.5/examples/vlmeta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.802125 blosc2-2.2.5/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   116429 2023-07-04 06:06:47.000000 blosc2-2.2.5/images/Complete-Write-Read-B2ND.png
+-rw-r--r--   0 runner    (1001) docker     (123)    64898 2023-07-04 06:06:47.000000 blosc2-2.2.5/images/M1-i386-vs-arm64-pack.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62528 2023-07-04 06:06:47.000000 blosc2-2.2.5/images/M1-i386-vs-arm64-unpack.png
+-rw-r--r--   0 runner    (1001) docker     (123)   113029 2023-07-04 06:06:47.000000 blosc2-2.2.5/images/Read-Partial-Slices-B2ND.png
+-rw-r--r--   0 runner    (1001) docker     (123)   314966 2023-07-04 06:06:47.000000 blosc2-2.2.5/images/b2nd-2level-parts.png
+-rw-r--r--   0 runner    (1001) docker     (123)    77813 2023-07-04 06:06:47.000000 blosc2-2.2.5/images/linspace-compress.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24888 2023-07-04 06:06:47.000000 blosc2-2.2.5/images/linspace-decompress.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-07-04 06:06:47.000000 blosc2-2.2.5/images/pack-array-cratios.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-04 06:06:47.000000 blosc2-2.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-04 06:06:47.000000 blosc2-2.2.5/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 06:06:47.000000 blosc2-2.2.5/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-04 06:06:47.000000 blosc2-2.2.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 06:06:47.000000 blosc2-2.2.5/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-04 06:06:47.000000 blosc2-2.2.5/requirements-runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-04 06:06:47.000000 blosc2-2.2.5/requirements-test-wheels.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-04 06:06:47.000000 blosc2-2.2.5/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 06:08:53.818125 blosc2-2.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-04 06:06:47.000000 blosc2-2.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.810124 blosc2-2.2.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:08:53.818125 blosc2-2.2.5/tests/ndarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/ndarray/persistency.cat
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/ndarray/test_auto_parts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/ndarray/test_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/ndarray/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/ndarray/test_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/ndarray/test_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/ndarray/test_getitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/ndarray/test_iterchunks_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/ndarray/test_lossy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/ndarray/test_metalayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/ndarray/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/ndarray/test_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/ndarray/test_persistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/ndarray/test_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/ndarray/test_setitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/ndarray/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/ndarray/test_squeeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/ndarray/test_struct_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/ndarray/test_zeros.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/test_bytes_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/test_comp_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/test_compress2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/test_compression_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/test_compressors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/test_decompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/test_iterchunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/test_postfilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/test_prefilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/test_python_blosc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/test_schunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/test_schunk_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/test_schunk_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/test_schunk_get_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/test_schunk_insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/test_schunk_set_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/test_schunk_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/test_ucodecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/test_ufilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-04 06:06:47.000000 blosc2-2.2.5/tests/test_vlmeta.py
```

### Comparing `blosc2-2.2.4/.github/workflows/build.yml` & `blosc2-2.2.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/.github/workflows/cibuildwheels.yml` & `blosc2-2.2.5/.github/workflows/cibuildwheels.yml`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/.gitignore` & `blosc2-2.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/ANNOUNCE.rst` & `blosc2-2.2.5/ANNOUNCE.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-Announcing Python-Blosc2 2.2.4
+Announcing Python-Blosc2 2.2.5
 ==============================
 
-This is a maintenance release, were we have added tutorials for a quick start.
-We have also added a new method `interchunks_info` for `SChunk` and `NDArray` classes.
-Finally, we have updated C-Blosc2 library to latest version (2.9.3).
+This is a maintenance release, where we have upgraded to latest C-Blosc2 2.10.0.
+This provides fixes for a bytedelta filter (see
+https://github.com/Blosc/c-blosc2/pull/532).  Hence, an upgrade is recommended
+for everybody, most especially, if you are using bytedelta.
 
 For more info, you can have a look at the release notes in:
 
 https://github.com/Blosc/python-blosc2/releases
 
 More docs and examples are available in the documentation site:
```

### Comparing `blosc2-2.2.4/CONTRIBUTING.rst` & `blosc2-2.2.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/LICENSE.txt` & `blosc2-2.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/PKG-INFO` & `blosc2-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blosc2
-Version: 2.2.4
+Version: 2.2.5
 Summary: Python wrapper for the C-Blosc2 library
 Author-email: Blosc Development Team <blosc@blosc.org>
 Maintainer-email: Blosc Development Team <blosc@blosc.org>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/Blosc/python-blosc2
 Project-URL: documentation, https://www.blosc.org/python-blosc2/python-blosc2.html
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `blosc2-2.2.4/README.rst` & `blosc2-2.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/RELEASE_NOTES.md` & `blosc2-2.2.5/RELEASE_NOTES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 # Release notes
 
-## Changes from 2.2.2 to 2.2.3
+## Changes from 2.2.4 to 2.2.5
+
+* Updated to latest C-Blosc2 2.10.0.
+
+* Use the new, fixed bytedelta filter introduced in C-Blosc2 2.10.0.
+
+* Some small fixes in tutorials.
+
+
+## Changes from 2.2.2 to 2.2.4
 
 * Added a new [section of tutorials](https://www.blosc.org/python-blosc2/getting_started/tutorials.html)
   for a quick get start.
 
 * Added a new [section on how to cite Blosc](https://github.com/Blosc/python-blosc2/tree/main#citing-blosc).
 
 * New method `interchunks_info` for `SChunk` and `NDArray` classes.
```

### Comparing `blosc2-2.2.4/RELEASING.rst` & `blosc2-2.2.5/RELEASING.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/bench/compress_numpy.py` & `blosc2-2.2.5/bench/compress_numpy.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/bench/get_slice.py` & `blosc2-2.2.5/bench/get_slice.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/bench/ndarray/compare_getslice.py` & `blosc2-2.2.5/bench/ndarray/compare_getslice.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/bench/ndarray/copy_postfilter.py` & `blosc2-2.2.5/bench/ndarray/copy_postfilter.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/bench/ndarray/download_data.py` & `blosc2-2.2.5/bench/ndarray/download_data.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/bench/ndarray/era5-pds/measurements-i10k.parquet` & `blosc2-2.2.5/bench/ndarray/era5-pds/measurements-i10k.parquet`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/bench/ndarray/era5-pds/measurements-i13k-always-split.parquet` & `blosc2-2.2.5/bench/ndarray/era5-pds/measurements-i13k-always-split.parquet`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/bench/ndarray/era5-pds/measurements-i13k-never-split.parquet` & `blosc2-2.2.5/bench/ndarray/era5-pds/measurements-i13k-never-split.parquet`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/bench/ndarray/era5-pds/measurements-i13k.parquet` & `blosc2-2.2.5/bench/ndarray/era5-pds/measurements-i13k.parquet`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/bench/ndarray/era5-pds/measurements-m1.parquet` & `blosc2-2.2.5/bench/ndarray/era5-pds/measurements-m1.parquet`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/bench/ndarray/era5-pds/measurements-ryzen3.parquet` & `blosc2-2.2.5/bench/ndarray/era5-pds/measurements-ryzen3.parquet`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/bench/ndarray/plot_transcode_data.ipynb` & `blosc2-2.2.5/bench/ndarray/plot_transcode_data.ipynb`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/bench/ndarray/transcode_data.py` & `blosc2-2.2.5/bench/ndarray/transcode_data.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/bench/pack_compress.py` & `blosc2-2.2.5/bench/pack_compress.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/bench/pack_large.py` & `blosc2-2.2.5/bench/pack_large.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/bench/pack_tensor.py` & `blosc2-2.2.5/bench/pack_tensor.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/bench/set_slice.py` & `blosc2-2.2.5/bench/set_slice.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/bench/sum_postfilter.py` & `blosc2-2.2.5/bench/sum_postfilter.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/CMakeLists.txt` & `blosc2-2.2.5/blosc2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/__init__.py` & `blosc2-2.2.5/blosc2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     NOFILTER = 0
     SHUFFLE = 1
     BITSHUFFLE = 2
     DELTA = 3
     TRUNC_PREC = 4
     NDCELL = 32
     NDMEAN = 33
-    BYTEDELTA = 34
+    BYTEDELTA = 35
 
 
 class SplitMode(Enum):
     """
     Available split modes.
     """
```

### Comparing `blosc2-2.2.4/blosc2/blosc2_ext.pyx` & `blosc2-2.2.5/blosc2/blosc2_ext.pyx`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/.github/ISSUE_TEMPLATE/bug_report.md` & `blosc2-2.2.5/blosc2/c-blosc2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/.github/workflows/cmake.yml` & `blosc2-2.2.5/blosc2/c-blosc2/.github/workflows/cmake.yml`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/.github/workflows/fuzz.yml` & `blosc2-2.2.5/blosc2/c-blosc2/.github/workflows/fuzz.yml`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/.readthedocs.yaml` & `blosc2-2.2.5/blosc2/c-blosc2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/ANNOUNCE.md` & `blosc2-2.2.5/blosc2/c-blosc2/ANNOUNCE.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-# Announcing C-Blosc2 2.9.3
+# Announcing C-Blosc2 2.10.0
 A fast, compressed and persistent binary data store library for C.
 
 ## What is new?
 
-This is a maintenance release with many improvements in documentation and code
-(thanks to Dimitri Papadopoulos). We also fixed several issues discovered
-by the fuzzer.
+This is a maintenance release with a couple of important fixes.  The first
+is bytedelta, which receives a new ID (35), whereas the previous one (34)
+is still available for backward compatibility.  The second is a fix for
+the filter pipeline, which e.g. allows to use several shuffle filters in a row
+(thanks to Tom Birch). There are also several fixes for helping integration
+of C-Blosc2 in other projects (thanks to Alex Huebel).
+
+Due to the important fixes, an upgrade is recommended for all users.
 
 For more info, please see the release notes in:
 
 https://github.com/Blosc/c-blosc2/blob/main/RELEASE_NOTES.md
 
 Also, there is blog post introducing the most relevant changes in Blosc2:
```

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/CMakeLists.txt` & `blosc2-2.2.5/blosc2/c-blosc2/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
     # Set the possible values of build type for cmake-gui
     set_property(CACHE CMAKE_BUILD_TYPE PROPERTY STRINGS
             "Debug" "Release" "MinSizeRel" "RelWithDebInfo")
 endif()
 
 # Propagate CMAKE_OSX_ARCHITECTURES env variable into CMAKE_SYSTEM_PROCESSOR
 if(DEFINED ENV{CMAKE_OSX_ARCHITECTURES})
-    if($ENV{CMAKE_OSX_ARCHITECTURES} STREQUAL "arm64")
+    if("$ENV{CMAKE_OSX_ARCHITECTURES}" STREQUAL "arm64")
         set(CMAKE_SYSTEM_PROCESSOR arm64)
     endif()
 endif()
 
 # Based on the target system's processor and the compiler being used,
 # set build variables indicating which hardware features can be targeted
 # by the compiler. Note we DO NOT check which hardware features are supported
```

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/COMPILING_WITH_WHEELS.rst` & `blosc2-2.2.5/blosc2/c-blosc2/COMPILING_WITH_WHEELS.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/CONTRIBUTING.rst` & `blosc2-2.2.5/blosc2/c-blosc2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/DEVELOPING-GUIDE.rst` & `blosc2-2.2.5/blosc2/c-blosc2/DEVELOPING-GUIDE.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/FAQ.md` & `blosc2-2.2.5/blosc2/c-blosc2/FAQ.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/LICENSE.txt` & `blosc2-2.2.5/blosc2/c-blosc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/LICENSES/BITSHUFFLE.txt` & `blosc2-2.2.5/blosc2/c-blosc2/LICENSES/BITSHUFFLE.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/LICENSES/FASTLZ.txt` & `blosc2-2.2.5/blosc2/c-blosc2/LICENSES/FASTLZ.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/LICENSES/LZ4.txt` & `blosc2-2.2.5/blosc2/c-blosc2/LICENSES/LZ4.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/LICENSES/ZLIB.txt` & `blosc2-2.2.5/blosc2/c-blosc2/LICENSES/ZLIB.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/LICENSES/ZSTD.txt` & `blosc2-2.2.5/blosc2/c-blosc2/LICENSES/ZSTD.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/README.rst` & `blosc2-2.2.5/blosc2/c-blosc2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 * **64-bit containers:** the first-class container in C-Blosc2 is the `super-chunk` or, for brevity, `schunk`, that is made by smaller chunks which are essentially C-Blosc1 32-bit containers.  The super-chunk can be backed or not by another container which is called a `frame` (see later).
 
 * **NDim containers (b2nd):** allow to store n-dimensional data that can efficiently read datasets in slices that can be n-dimensional too. To achieve this, a n-dimensional 2-level partitioning has been implemented.  This capabilities were formerly part of `Caterva <https://github.com/Blosc/caterva>`_, and now it is included in C-Blosc2 for convenience.  Caterva is now deprecated.
 
 * **More filters:** besides `shuffle` and `bitshuffle` already present in C-Blosc1, C-Blosc2 already implements:
 
-  - `bytedelta`: calculates the difference between bytes in a block that has been shuffle already.  We have `blogged about bytedelta <https://www.blosc.org/posts/bytedelta-enhance-compression-toolset/>`_.
+  - `bytedelta`: calculates the difference between bytes in a block that has been shuffled already.  We have `blogged about bytedelta <https://www.blosc.org/posts/bytedelta-enhance-compression-toolset/>`_.
 
   - `delta`: the stored blocks inside a chunk are diff'ed with respect to first block in the chunk.  The idea is that, in some situations, the diff will have more zeros than the original data, leading to better compression.
 
   - `trunc_prec`: it zeroes the least significant bits of the mantissa of float32 and float64 types.  When combined with the `shuffle` or `bitshuffle` filter, this leads to more contiguous zeros, which are compressed better.
 
 * **A filter pipeline:** the different filters can be pipelined so that the output of one can the input for the other.  A possible example is a `delta` followed by `shuffle`, or as described above, `trunc_prec` followed by `bitshuffle`.
```

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/README_ARM.rst` & `blosc2-2.2.5/blosc2/c-blosc2/README_ARM.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/README_B2ND_METALAYER.rst` & `blosc2-2.2.5/blosc2/c-blosc2/README_B2ND_METALAYER.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/README_CFRAME_FORMAT.rst` & `blosc2-2.2.5/blosc2/c-blosc2/README_CFRAME_FORMAT.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/README_CHUNK_FORMAT.rst` & `blosc2-2.2.5/blosc2/c-blosc2/README_CHUNK_FORMAT.rst`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
     +---------+--------+
     |  header | blocks |
     +---------+--------+
 
 Also, there are the so-called lazy chunks that do not have the actual compressed data,
 but only metainformation about how to read it. Lazy chunks typically appear when reading
-data from persistent media.  A lazy chunk has the header and bstarts sections in place
-and in addition, they have an additional trailer for allowing to read the data blocks::
+data from persistent media.  A lazy chunk has header and bstarts sections in place and
+in addition, an additional trailer for allowing to read the data blocks::
 
     +---------+---------+---------+
     |  header | bstarts | trailer |
     +---------+---------+---------+
 
 All these sections are described below.  Note that the bstarts section is described as
 part of the blocks section.
@@ -180,15 +180,15 @@
 The blocks section is composed of a list of offsets to the start of each block, an optional dictionary to aid in
 compression, and finally a list of compressed data streams::
 
     +=========+======+=========+
     | bstarts | dict | streams |
     +=========+======+=========+
 
-Each block is equal-sized as specified by the `blocksize` header field. The size of the last block that can be shorter
+Each block is equal-sized as specified by the `blocksize` header field. The size of the last block can be shorter
 or equal to the rest.
 
 **Block starts**
 
 The *block starts* section contains a list of offsets `int32 bstarts` that indicate where each block starts in the
 chunk. These offsets are relative to the start of the chunk and point to the start of one or more compressed
 data streams containing the contents of the block::
```

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/README_FUZZER.md` & `blosc2-2.2.5/blosc2/c-blosc2/README_FUZZER.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/README_SFRAME_FORMAT.rst` & `blosc2-2.2.5/blosc2/c-blosc2/README_SFRAME_FORMAT.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/README_THREADED.rst` & `blosc2-2.2.5/blosc2/c-blosc2/README_THREADED.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/RELEASE_NOTES.md` & `blosc2-2.2.5/blosc2/c-blosc2/RELEASE_NOTES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,33 @@
 Release notes for C-Blosc2
 ==========================
 
+
+Changes from 2.9.3 to 2.10.0
+===========================
+
+* bytedelta filter has been fixed. For backward compatibility, the old
+  bytedelta filter is still available as `BLOSC_FILTER_BYTEDELTA_BUGGY`
+  symbol, with the same ID (34) than before.  The new, fixed bytedelta
+  filter has received a new ID (35) and it can be used via the usual
+  `BLOSC_FILTER_BYTEDELTA` symbol. That means that old data written with
+  the buggy bytedelta filter should be decompressed without issues.
+  Thanks to @foody (Tom Birch) for the fix. See #531, #532 for more info.
+
+* Filter buffers are correctly cycled now.  Now it is possible to use e.g.
+  shuffle and bitshuffle filters in the pipeline.  Thanks to @foody (Tom Birch)
+  for the fix.  See #528 and PR #530.
+
+* Assorted fixes for allowing better inclusion in external projects.
+  Thanks to @ax3l (Axel Huebel). See #525, #527 and #529.
+
+* Minor fixes in the documentation.  Thanks to @ivilata (Ivan Vilata).
+  See #523.
+* 
+
 Changes from 2.9.2 to 2.9.3
 ===========================
 
 * Thanks to Dimitri Papadopoulos for an extensive set of improvements in
   documentation and code.
 
 * `load_lib` is now a private function. Before was public, but
```

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/RELEASING.rst` & `blosc2-2.2.5/blosc2/c-blosc2/RELEASING.rst`

 * *Files 2% similar despite different names*

```diff
@@ -89,16 +89,15 @@
 Post-release actions
 --------------------
 
 - Edit *VERSION* symbols in blosc/blosc2.h in master to increment the
   version to the next minor one (i.e. X.Y.Z --> X.Y.(Z+1).dev).
 
 - Create new headers for adding new features in ``RELEASE_NOTES.md``
-  and empty the release-specific information in ``ANNOUNCE.md`` and
-  add this place-holder instead:
+  and add this place-holder instead:
 
   #XXX version-specific blurb XXX#
 
 - Commit the changes::
 
   $ git commit -a -m"Post X.Y.Z release actions done"
   $ git push
```

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/ROADMAP.rst` & `blosc2-2.2.5/blosc2/c-blosc2/ROADMAP.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/THANKS.rst` & `blosc2-2.2.5/blosc2/c-blosc2/THANKS.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/CMakeLists.txt` & `blosc2-2.2.5/blosc2/c-blosc2/bench/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/Makefile` & `blosc2-2.2.5/blosc2/c-blosc2/bench/Makefile`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/Makefile.mingw` & `blosc2-2.2.5/blosc2/c-blosc2/bench/Makefile.mingw`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/b2bench.c` & `blosc2-2.2.5/blosc2/c-blosc2/bench/b2bench.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/b2nd/CMakeLists.txt` & `blosc2-2.2.5/blosc2/c-blosc2/bench/b2nd/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/b2nd/bench_get_slice.c` & `blosc2-2.2.5/blosc2/c-blosc2/bench/b2nd/bench_get_slice.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/b2nd/bench_zfp_getitem.c` & `blosc2-2.2.5/blosc2/c-blosc2/bench/b2nd/bench_zfp_getitem.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/create_frame.c` & `blosc2-2.2.5/blosc2/c-blosc2/bench/create_frame.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/delta_schunk.c` & `blosc2-2.2.5/blosc2/c-blosc2/bench/delta_schunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/plot-speeds.py` & `blosc2-2.2.5/blosc2/c-blosc2/bench/plot-speeds.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/plot-sum_openmp-results.py` & `blosc2-2.2.5/blosc2/c-blosc2/bench/plot-sum_openmp-results.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/rainfall-grid-150x150.bin` & `blosc2-2.2.5/blosc2/c-blosc2/bench/rainfall-grid-150x150.bin`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/read-grid-150x150.py` & `blosc2-2.2.5/blosc2/c-blosc2/bench/read-grid-150x150.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/results-corex/blosclz-cl1-sum_openmp-corex.out` & `blosc2-2.2.5/blosc2/c-blosc2/bench/results-corex/blosclz-cl1-sum_openmp-corex.out`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/results-corex/blosclz-suite-corex.out` & `blosc2-2.2.5/blosc2/c-blosc2/bench/results-corex/blosclz-suite-corex.out`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/results-corex/lz4-cl1-sum_openmp-corex.out` & `blosc2-2.2.5/blosc2/c-blosc2/bench/results-corex/lz4-cl1-sum_openmp-corex.out`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/results-corex/lz4-suite-corex.out` & `blosc2-2.2.5/blosc2/c-blosc2/bench/results-corex/lz4-suite-corex.out`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/results-corex/lz4hc-cl1-sum_openmp-corex.out` & `blosc2-2.2.5/blosc2/c-blosc2/bench/results-corex/lz4hc-cl1-sum_openmp-corex.out`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/results-corex/zlib-cl1-sum_openmp-corex.out` & `blosc2-2.2.5/blosc2/c-blosc2/bench/results-corex/zlib-cl1-sum_openmp-corex.out`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/results-corex/zstd-cl1-sum_openmp-corex.out` & `blosc2-2.2.5/blosc2/c-blosc2/bench/results-corex/zstd-cl1-sum_openmp-corex.out`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/sframe_bench.c` & `blosc2-2.2.5/blosc2/c-blosc2/bench/sframe_bench.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/sum_openmp.c` & `blosc2-2.2.5/blosc2/c-blosc2/bench/sum_openmp.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/trunc_prec_schunk.c` & `blosc2-2.2.5/blosc2/c-blosc2/bench/trunc_prec_schunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/bench/zero_runlen.c` & `blosc2-2.2.5/blosc2/c-blosc2/bench/zero_runlen.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/CMakeLists.txt` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     set(BLOSC_INCLUDE_DIRS ${BLOSC_INCLUDE_DIRS} ${LZ4_LOCAL_DIR})
 endif()
 
 if(NOT DEACTIVATE_ZLIB)
     if(ZLIB_NG_FOUND)
         set(BLOSC_INCLUDE_DIRS ${BLOSC_INCLUDE_DIRS} ${ZLIB_NG_INCLUDE_DIR})
     elseif(ZLIB_FOUND)
-        set(BLOSC_INCLUDE_DIRS ${BLOSC_INCLUDE_DIRS} ${ZLIB_INCLUDE_DIR})
+        set(BLOSC_INCLUDE_DIRS ${BLOSC_INCLUDE_DIRS} ${ZLIB_INCLUDE_DIRS})
     else()
         set(ZLIB_LOCAL_DIR ${INTERNAL_LIBS}/${ZLIB_NG_DIR})
         set(BLOSC_INCLUDE_DIRS ${BLOSC_INCLUDE_DIRS} ${ZLIB_LOCAL_DIR})
     endif()
 endif()
 
 if(NOT DEACTIVATE_ZSTD)
@@ -108,15 +108,15 @@
     source_group("LZ4" FILES ${LZ4_FILES})
 endif()
 
 if(NOT DEACTIVATE_ZLIB)
     if(ZLIB_NG_FOUND)
         set(LIBS ${LIBS} ${ZLIB_NG_LIBRARY})
     elseif(ZLIB_FOUND)
-        set(LIBS ${LIBS} ${ZLIB_LIBRARY})
+        set(LIBS ${LIBS} ${ZLIB_LIBRARIES})
     else()
         set(ZLIB_LOCAL_DIR ${INTERNAL_LIBS}/${ZLIB_NG_DIR})
         file(GLOB ZLIB_FILES ${ZLIB_LOCAL_DIR}/*.c)
         set(SOURCES ${SOURCES} ${ZLIB_FILES})
         source_group("Zlib" FILES ${ZLIB_FILES})
     endif()
 endif()
```

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/b2nd.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/b2nd.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/b2nd_utils.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/b2nd_utils.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/b2nd_utils.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/b2nd_utils.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/bitshuffle-altivec.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/bitshuffle-altivec.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/bitshuffle-altivec.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/bitshuffle-altivec.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/bitshuffle-avx2.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/bitshuffle-avx2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/bitshuffle-avx2.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/bitshuffle-avx2.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/bitshuffle-generic.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/bitshuffle-generic.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/bitshuffle-generic.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/bitshuffle-generic.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/bitshuffle-neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/bitshuffle-neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/bitshuffle-neon.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/bitshuffle-neon.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/bitshuffle-sse2.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/bitshuffle-sse2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/bitshuffle-sse2.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/bitshuffle-sse2.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/blosc-private.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/blosc-private.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/blosc2-stdio.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/blosc2-stdio.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/blosc2.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/blosc2.c`

 * *Files 1% similar despite different names*

```diff
@@ -903,14 +903,20 @@
       header->blosc2_flags |= BLOSC2_INSTR_CODEC;
     }
   }
 
   return 0;
 }
 
+void _cycle_buffers(uint8_t **src, uint8_t **dest, uint8_t **tmp) {
+  uint8_t *tmp2 = *src;
+  *src = *dest;
+  *dest = *tmp;
+  *tmp = tmp2;
+}
 
 uint8_t* pipeline_forward(struct thread_context* thread_context, const int32_t bsize,
                           const uint8_t* src, const int32_t offset,
                           uint8_t* dest, uint8_t* tmp, uint8_t* tmp2) {
   blosc2_context* context = thread_context->parent_context;
   uint8_t* _src = (uint8_t*)src + offset;
   uint8_t* _tmp = tmp;
@@ -944,33 +950,28 @@
       return NULL;
     }
 
     if (memcpyed) {
       // No more filters are required
       return _dest;
     }
-    // Cycle buffers
-    _src = _dest;
-    _dest = _tmp;
-    _tmp = _src;
+    _cycle_buffers(&_src, &_dest, &_tmp);
   }
 
   /* Process the filter pipeline */
   for (int i = 0; i < BLOSC2_MAX_FILTERS; i++) {
     int rc = BLOSC2_ERROR_SUCCESS;
     if (filters[i] <= BLOSC2_DEFINED_FILTERS_STOP) {
       switch (filters[i]) {
         case BLOSC_SHUFFLE:
           for (int j = 0; j <= filters_meta[i]; j++) {
             shuffle(typesize, bsize, _src, _dest);
             // Cycle filters when required
             if (j < filters_meta[i]) {
-              _src = _dest;
-              _dest = _tmp;
-              _tmp = _src;
+              _cycle_buffers(&_src, &_dest, &_tmp);
             }
           }
           break;
         case BLOSC_BITSHUFFLE:
           if (bitshuffle(typesize, bsize, _src, _dest, tmp2) < 0) {
             return NULL;
           }
@@ -1021,17 +1022,15 @@
 
       urfiltersuccess:;
 
     }
 
     // Cycle buffers when required
     if (filters[i] != BLOSC_NOFILTER) {
-      _src = _dest;
-      _dest = _tmp;
-      _tmp = _src;
+      _cycle_buffers(&_src, &_dest, &_tmp);
     }
   }
   return _src;
 }
 
 
 // Optimized version for detecting runs.  It compares 8 bytes values wherever possible.
@@ -1340,17 +1339,15 @@
     if (filters[i] <= BLOSC2_DEFINED_FILTERS_STOP) {
       switch (filters[i]) {
         case BLOSC_SHUFFLE:
           for (int j = 0; j <= filters_meta[i]; j++) {
             unshuffle(typesize, bsize, _src, _dest);
             // Cycle filters when required
             if (j < filters_meta[i]) {
-              _src = _dest;
-              _dest = _tmp;
-              _tmp = _src;
+              _cycle_buffers(&_src, &_dest, &_tmp);
             }
             // Check whether we have to copy the intermediate _dest buffer to final destination
             if (last_copy_filter && (filters_meta[i] % 2) == 1 && j == filters_meta[i]) {
               memcpy(dest + offset, _dest, (unsigned int) bsize);
             }
           }
           break;
@@ -1420,17 +1417,15 @@
       BLOSC_TRACE_ERROR("User-defined filter %d not found during decompression.", filters[i]);
       return BLOSC2_ERROR_FILTER_PIPELINE;
       urfiltersuccess:;
     }
 
     // Cycle buffers when required
     if ((filters[i] != BLOSC_NOFILTER) && (filters[i] != BLOSC_TRUNC_PREC)) {
-      _src = _dest;
-      _dest = _tmp;
-      _tmp = _src;
+      _cycle_buffers(&_src, &_dest, &_tmp);
     }
     if (last_filter_index == i) {
       break;
     }
   }
 
   /* Postfilter function */
```

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/blosclz.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/blosclz.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/blosclz.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/blosclz.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/context.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/context.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/delta.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/delta.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/delta.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/delta.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/directories.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/directories.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/fastcopy.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/fastcopy.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/fastcopy.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/fastcopy.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/frame.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/frame.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/frame.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/frame.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/schunk.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/schunk.c`

 * *Files 0% similar despite different names*

```diff
@@ -121,17 +121,17 @@
   schunk->version = 0;     /* pre-first version */
 
   // Get the storage with proper defaults
   schunk->storage = get_new_storage(storage, &BLOSC2_CPARAMS_DEFAULTS, &BLOSC2_DPARAMS_DEFAULTS, &BLOSC2_IO_DEFAULTS);
   // Update the (local variable) storage
   storage = schunk->storage;
 
-  char* btune_balance = getenv("BTUNE_BALANCE");
-  if (btune_balance != NULL) {
-    // If BTUNE_BALANCE passed, automatically use btune
+  char* tradeoff = getenv("BTUNE_TRADEOFF");
+  if (tradeoff != NULL) {
+    // If BTUNE_TRADEOFF passed, automatically use btune
     storage->cparams->tuner_id = BLOSC_BTUNE;
   }
 
   // ...and update internal properties
   update_schunk_properties(schunk);
 
   if (schunk->cctx->tuner_id < BLOSC_LAST_TUNER && schunk->cctx->tuner_id == BLOSC_STUNE) {
```

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/sframe.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/sframe.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/sframe.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/sframe.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle-altivec.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle-altivec.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle-altivec.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle-altivec.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle-avx2.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle-avx2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle-avx2.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle-avx2.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle-generic.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle-generic.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle-generic.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle-generic.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle-neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle-neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle-neon.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle-neon.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle-sse2.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle-sse2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle-sse2.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle-sse2.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/shuffle.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/shuffle.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/stune.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/stune.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/stune.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/stune.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/timestamp.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/timestamp.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/transpose-altivec.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/transpose-altivec.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/trunc-prec.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/trunc-prec.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/trunc-prec.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/trunc-prec.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/win32/pthread.c` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/win32/pthread.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/blosc/win32/pthread.h` & `blosc2-2.2.5/blosc2/c-blosc2/blosc/win32/pthread.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/cmake/FindIPP.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/cmake/FindIPP.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/cmake/FindSIMD.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/cmake/FindSIMD.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/cmake/FindZLIB_NG.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/cmake/FindZLIB_NG.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/cmake/toolchain-aarch64.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/cmake/toolchain-aarch64.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/cmake/toolchain-armhf.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/cmake/toolchain-armhf.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/cmake/toolchain-armsf.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/cmake/toolchain-armsf.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/cmake_uninstall.cmake.in` & `blosc2-2.2.5/blosc2/c-blosc2/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/CMakeLists.txt` & `blosc2-2.2.5/blosc2/c-blosc2/compat/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.11.1-blosclz.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.11.1-blosclz.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.11.1-lz4.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.11.1-lz4.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.11.1-lz4hc.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.11.1-lz4hc.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.11.1-zlib.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.11.1-zlib.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.11.1-zstd.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.11.1-zstd.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.14.0-blosclz.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.14.0-blosclz.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.14.0-lz4.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.14.0-lz4.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.14.0-lz4hc.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.14.0-lz4hc.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.14.0-zlib.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.14.0-zlib.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.14.0-zstd.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.14.0-zstd.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle4-memcpy.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle4-memcpy.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle8-nomemcpy.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle8-nomemcpy.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle4-memcpy.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle4-memcpy.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle8-nomemcpy.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle8-nomemcpy.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.3.0-blosclz.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.3.0-blosclz.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.3.0-lz4.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.3.0-lz4.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.3.0-lz4hc.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.3.0-lz4hc.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.3.0-zlib.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.3.0-zlib.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.7.0-blosclz.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.7.0-blosclz.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.7.0-lz4.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.7.0-lz4.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.7.0-lz4hc.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.7.0-lz4hc.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-1.7.0-zlib.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-1.7.0-zlib.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle4-memcpy.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle4-memcpy.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle8-nomemcpy.cdata` & `blosc2-2.2.5/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle8-nomemcpy.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/compat/filegen.c` & `blosc2-2.2.5/blosc2/c-blosc2/compat/filegen.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test1.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test1.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test16.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test16.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test2.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test4.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test8.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test8.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon_bucle.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon_bucle.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon_bucle.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon_bucle.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon_bucle.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon_bucle.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon_bucle.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon_bucle.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon_bucle.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test16.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test16.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test2.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test4.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test8.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test8.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_bucle.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx_bucle.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon_bucle.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon_bucle.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_bucle.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt_bucle.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx_bucle.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_bucle.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx_bucle.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon_bucle.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle4_neon/unshuffle4_neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle4_neon/unshuffle4_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_bucle.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx_bucle.c` & `blosc2-2.2.5/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/doc/_static/blosc-logo_256.png` & `blosc2-2.2.5/blosc2/c-blosc2/doc/_static/blosc-logo_256.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/doc/_static/css/custom.css` & `blosc2-2.2.5/blosc2/c-blosc2/doc/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/doc/conf.py` & `blosc2-2.2.5/blosc2/c-blosc2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/doc/reference/b2nd.rst` & `blosc2-2.2.5/blosc2/c-blosc2/doc/reference/b2nd.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Blosc2 NDim
 ===========
 
 It contains both the data and metalayer that stores the dimensional info for the array.
-Blosc2 NDim has an internal context managed that stores the different properties of each array.
+Blosc2 NDim has a managed internal context that stores the different properties of each array.
 
 Context
 -------
 
 .. doxygentypedef:: b2nd_context_t
 
 Creation
```

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/doc/reference/blosc1.rst` & `blosc2-2.2.5/blosc2/c-blosc2/doc/reference/blosc1.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/doc/reference/context.rst` & `blosc2-2.2.5/blosc2/c-blosc2/doc/reference/context.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/doc/reference/index.rst` & `blosc2-2.2.5/blosc2/c-blosc2/doc/reference/index.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/doc/reference/metalayers.rst` & `blosc2-2.2.5/blosc2/c-blosc2/doc/reference/metalayers.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/doc/reference/plugins.rst` & `blosc2-2.2.5/blosc2/c-blosc2/doc/reference/plugins.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/doc/reference/schunk.rst` & `blosc2-2.2.5/blosc2/c-blosc2/doc/reference/schunk.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/doc/reference/utility.rst` & `blosc2-2.2.5/blosc2/c-blosc2/doc/reference/utility.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/CMakeLists.txt` & `blosc2-2.2.5/blosc2/c-blosc2/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/README.rst` & `blosc2-2.2.5/blosc2/c-blosc2/examples/README.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/b2nd/CMakeLists.txt` & `blosc2-2.2.5/blosc2/c-blosc2/examples/b2nd/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/b2nd/example_empty_shape.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/b2nd/example_empty_shape.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/b2nd/example_frame_generator.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/b2nd/example_frame_generator.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/b2nd/example_oindex.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/b2nd/example_oindex.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/b2nd/example_plainbuffer.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/b2nd/example_plainbuffer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/b2nd/example_plugins_codecs.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/b2nd/example_plugins_codecs.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/b2nd/example_plugins_filters.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/b2nd/example_plugins_filters.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/b2nd/example_print_meta.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/b2nd/example_print_meta.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/b2nd/example_serialize.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/b2nd/example_serialize.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/compress_file.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/compress_file.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/contexts.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/contexts.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/delta_schunk_ex.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/delta_schunk_ex.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/find_roots.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/find_roots.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/frame_backed_schunk.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/frame_backed_schunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/frame_big.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/frame_big.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/frame_metalayers.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/frame_metalayers.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/frame_offset.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/frame_offset.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/frame_roundtrip.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/frame_roundtrip.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/frame_simple.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/frame_simple.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/frame_vlmetalayers.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/frame_vlmetalayers.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/get_set_slice.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/get_set_slice.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/instrument_codec.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/instrument_codec.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/many_compressors.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/many_compressors.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/multithread.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/multithread.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/noinit.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/noinit.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/schunk_postfilter.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/schunk_postfilter.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/schunk_simple.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/schunk_simple.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/sframe_simple.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/sframe_simple.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/simple.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/simple.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/urcodecs.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/urcodecs.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/urfilters.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/urfilters.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/win-dynamic-linking.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/win-dynamic-linking.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/examples/zstd_dict.c` & `blosc2-2.2.5/blosc2/c-blosc2/examples/zstd_dict.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/images/Complete-Write-Read-B2ND.png` & `blosc2-2.2.5/blosc2/c-blosc2/images/Complete-Write-Read-B2ND.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/images/Read-Partial-Slices-B2ND.png` & `blosc2-2.2.5/blosc2/c-blosc2/images/Read-Partial-Slices-B2ND.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/images/b2nd-2level-parts.png` & `blosc2-2.2.5/blosc2/c-blosc2/images/b2nd-2level-parts.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/images/blosc2-pipeline.png` & `blosc2-2.2.5/blosc2/c-blosc2/images/blosc2-pipeline.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/images/blosc2-pipeline.svg` & `blosc2-2.2.5/blosc2/c-blosc2/images/blosc2-pipeline.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/include/b2nd.h` & `blosc2-2.2.5/blosc2/c-blosc2/include/b2nd.h`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -194,16 +194,16 @@
 
 
 /**
  * Create an array, with @p fill_value being used as the default value for
  * uninitialized portions of the array.
  *
  * @param ctx The b2nd context for the new array.
- * @param fill_value Default value for uninitialized portions of the array.
  * @param array The memory pointer where the array will be created.
+ * @param fill_value Default value for uninitialized portions of the array.
  *
  * @return An error code.
  */
 BLOSC_EXPORT int b2nd_full(b2nd_context_t *ctx, b2nd_array_t **array, const void *fill_value);
 
 /**
  * @brief Free an array.
```

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/include/blosc2/blosc2-common.h` & `blosc2-2.2.5/blosc2/c-blosc2/include/blosc2/blosc2-common.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/include/blosc2/blosc2-export.h` & `blosc2-2.2.5/blosc2/c-blosc2/include/blosc2/blosc2-export.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/include/blosc2/blosc2-stdio.h` & `blosc2-2.2.5/blosc2/c-blosc2/include/blosc2/blosc2-stdio.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/include/blosc2/codecs-registry.h` & `blosc2-2.2.5/blosc2/c-blosc2/include/blosc2/codecs-registry.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/include/blosc2/filters-registry.h` & `blosc2-2.2.5/blosc2/c-blosc2/include/blosc2/filters-registry.h`

 * *Files 24% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 enum {
     BLOSC_FILTER_NDCELL = 32,
     BLOSC_FILTER_NDMEAN = 33,
-    BLOSC_FILTER_BYTEDELTA = 34,
+    BLOSC_FILTER_BYTEDELTA_BUGGY = 34, // buggy version. See #524
+    BLOSC_FILTER_BYTEDELTA = 35,  // fixed version
 };
 
 void register_filters(void);
 
 // For dynamically loaded filters
 typedef struct {
     char *forward;
```

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/include/blosc2/tuners-registry.h` & `blosc2-2.2.5/blosc2/c-blosc2/include/blosc2/tuners-registry.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/include/blosc2.h` & `blosc2-2.2.5/blosc2/c-blosc2/include/blosc2.h`

 * *Files 1% similar despite different names*

```diff
@@ -78,19 +78,19 @@
   #define blosc_cbuffer_versions blosc2_cbuffer_versions
   #define blosc_cbuffer_complib blosc2_cbuffer_complib
 #endif
 
 
 /* Version numbers */
 #define BLOSC2_VERSION_MAJOR    2    /* for major interface/format changes  */
-#define BLOSC2_VERSION_MINOR    9    /* for minor interface/format changes  */
-#define BLOSC2_VERSION_RELEASE  3    /* for tweaks, bug-fixes, or development */
+#define BLOSC2_VERSION_MINOR    10   /* for minor interface/format changes  */
+#define BLOSC2_VERSION_RELEASE  0    /* for tweaks, bug-fixes, or development */
 
-#define BLOSC2_VERSION_STRING   "2.9.3"  /* string version.  Sync with above! */
-#define BLOSC2_VERSION_DATE     "$Date:: 2023-06-21 #$"    /* date version */
+#define BLOSC2_VERSION_STRING   "2.10.0"  /* string version.  Sync with above! */
+#define BLOSC2_VERSION_DATE     "$Date:: 2023-07-04 #$"    /* date version */
 
 
 /* The maximum number of dimensions for Blosc2 NDim arrays */
 #define BLOSC2_MAX_DIM 8
 
 
 /* Tracing macros */
@@ -215,15 +215,15 @@
 enum {
   BLOSC2_DEFINED_FILTERS_START = 0,
   BLOSC2_DEFINED_FILTERS_STOP = 31,
   //!< Blosc-defined filters must be between 0 - 31.
   BLOSC2_GLOBAL_REGISTERED_FILTERS_START = 32,
   BLOSC2_GLOBAL_REGISTERED_FILTERS_STOP = 159,
   //!< Blosc-registered filters must be between 32 - 159.
-  BLOSC2_GLOBAL_REGISTERED_FILTERS = 3,
+  BLOSC2_GLOBAL_REGISTERED_FILTERS = 4,
   //!< Number of Blosc-registered filters at the moment.
   BLOSC2_USER_REGISTERED_FILTERS_START = 160,
   BLOSC2_USER_REGISTERED_FILTERS_STOP = 255,
   //!< User-defined filters must be between 128 - 255.
   BLOSC2_MAX_FILTERS = 6,
   //!< Maximum number of filters in the filter pipeline
   BLOSC2_MAX_UDFILTERS = 16,
@@ -1049,17 +1049,17 @@
   const char *name;
   //!< The IO identifier.
   void *params;
   //!< The IO parameters.
 } blosc2_io;
 
 static const blosc2_io BLOSC2_IO_DEFAULTS = {
-    .id = BLOSC2_IO_FILESYSTEM,
-    .name = "filesystem",
-    .params = NULL,
+  /* .id = */ BLOSC2_IO_FILESYSTEM,
+  /* .name = */ "filesystem",
+  /* .params = */ NULL,
 };
 
 
 /**
  * @brief Register a user-defined input/output callbacks in Blosc.
  *
  * @param io The callbacks API to register.
@@ -1239,29 +1239,29 @@
 /**
  * @brief Create a context for @a *_ctx() compression functions.
  *
  * @param cparams The blosc2_cparams struct with the compression parameters.
  *
  * @return A pointer to the new context. NULL is returned if this fails.
  *
- * @note This support the same environment variables than #blosc2_compress
+ * @note This supports the same environment variables than #blosc2_compress
  * for overriding the programmatic compression values.
  *
  * @sa #blosc2_compress
  */
 BLOSC_EXPORT blosc2_context* blosc2_create_cctx(blosc2_cparams cparams);
 
 /**
  * @brief Create a context for *_ctx() decompression functions.
  *
  * @param dparams The blosc2_dparams struct with the decompression parameters.
  *
  * @return A pointer to the new context. NULL is returned if this fails.
  *
- * @note This support the same environment variables than #blosc2_decompress
+ * @note This supports the same environment variables than #blosc2_decompress
  * for overriding the programmatic decompression values.
  *
  * @sa #blosc2_decompress
  *
  */
 BLOSC_EXPORT blosc2_context* blosc2_create_dctx(blosc2_dparams dparams);
 
@@ -1829,15 +1829,15 @@
 BLOSC_EXPORT int64_t blosc2_schunk_append_file(blosc2_schunk* schunk, const char* urlpath);
 
 /**
  * @brief Release resources from a super-chunk.
  *
  * @param schunk The super-chunk to be freed.
  *
- * @remark All the memory resources attached to the super-frame are freed.
+ * @remark All the memory resources attached to the super-chunk are freed.
  * If the super-chunk is on-disk, the data continues there for a later
  * re-opening.
  *
  * @return 0 if success.
  */
 BLOSC_EXPORT int blosc2_schunk_free(blosc2_schunk *schunk);
 
@@ -1912,15 +1912,15 @@
  * pointer.
  *
  * @param schunk The super-chunk from where the chunk will be decompressed.
  * @param nchunk The chunk to be decompressed (0 indexed).
  * @param dest The buffer where the decompressed data will be put.
  * @param nbytes The size of the area pointed by @p *dest.
  *
- * @warning You must make sure that you have space enough to store the
+ * @warning You must make sure that you have enough space to store the
  * uncompressed data.
  *
  * @return The size of the decompressed chunk or 0 if it is non-initialized. If some problem is
  * detected, a negative code is returned instead.
  */
 BLOSC_EXPORT int blosc2_schunk_decompress_chunk(blosc2_schunk *schunk, int64_t nchunk, void *dest, int32_t nbytes);
 
@@ -1976,15 +1976,15 @@
  * @brief Fill buffer with a schunk slice.
  *
  * @param schunk The super-chunk from where to extract a slice.
  * @param start Index (0-based) where the slice begins.
  * @param stop The first index (0-based) that is not in the selected slice.
  * @param buffer The buffer where the data will be stored.
  *
- * @warning You must make sure that you have space enough in buffer to store the
+ * @warning You must make sure that you have enough space in buffer to store the
  * uncompressed data.
  *
  * @return An error code.
  */
 BLOSC_EXPORT int blosc2_schunk_get_slice_buffer(blosc2_schunk *schunk, int64_t start, int64_t stop, void *buffer);
 
 /**
```

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/.shellcheckrc` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/.shellcheckrc`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/CMakeLists.txt` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/FAQ.zlib` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/FAQ.zlib`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/INDEX.md` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/INDEX.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/LICENSE.md` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/Makefile.in` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/Makefile.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/PORTING.md` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/PORTING.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/README.md` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32_p.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32_p.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/Makefile.in` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/Makefile.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/adler32_neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/adler32_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/armfeature.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/armfeature.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/chunkset_neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/chunkset_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/crc32_acle.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/crc32_acle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/insert_string_acle.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/insert_string_acle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/slide_neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/slide_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/Makefile.in` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/Makefile.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/adler32_power8.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/adler32_power8.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/slide_hash_power8.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/slide_hash_power8.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/Makefile.in` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/Makefile.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/README.md` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_detail.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_detail.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.Dockerfile` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.Dockerfile`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.service` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.service`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/actions-runner` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/actions-runner`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/entrypoint` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/Makefile.in` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/Makefile.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_avx.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_avx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_ssse3.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_ssse3.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_avx.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_avx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_sse.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_sse.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_avx.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_avx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_sse.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_sse.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/insert_string_sse.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/insert_string_sse.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_avx.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_avx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_sse.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_sse.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/x86.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/x86.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset_tpl.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset_tpl.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-coverage.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-coverage.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-install-dirs.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-install-dirs.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-sanitizer.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-sanitizer.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-compare.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-compare.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-redirect.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-redirect.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-compress.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-compress.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-tools.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-tools.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-aarch64.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-aarch64.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-arm.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-arm.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-armhf.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-armhf.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-i686.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-i686.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-x86_64.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-x86_64.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64le.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64le.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-s390x.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-s390x.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-sparc64.cmake` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-sparc64.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compare258.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compare258.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compress.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/configure` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/configure`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl._h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl._h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl._h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl._h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_fast.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_fast.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_medium.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_medium.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_p.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_p.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_quick.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_quick.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_slow.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_slow.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/algorithm.txt` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/algorithm.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1950.txt` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1950.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1951.txt` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1951.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1952.txt` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1952.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/txtvsbin.txt` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/txtvsbin.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/fallback_builtins.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/fallback_builtins.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzguts.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzguts.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzlib.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzlib.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzread.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzread.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzwrite.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzwrite.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/infback.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/infback.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl._h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl._h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate_p.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate_p.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string_tpl.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string_tpl.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/match_tpl.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/match_tpl.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2002-0059/test.gz` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2002-0059/test.gz`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/default.txt` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/default.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/fixed.txt` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/fixed.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-979/pigz-2.6.tar.gz` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-979/pigz-2.6.tar.gz`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/Makefile.in` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/Makefile.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/README.md` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-arm-linux-gnueabihf.abi` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-arm-linux-gnueabihf.abi`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-x86_64-linux-gnu.abi` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-x86_64-linux-gnu.abi`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.md` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.sh` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.sh`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/adler32_test.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/adler32_test.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/crc32_test.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/crc32_test.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/fireworks.jpg` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/fireworks.jpg`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/lcet10.txt` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/lcet10.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/paper-100k.pdf` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/paper-100k.pdf`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_bi_valid.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_bi_valid.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_block_open.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_block_open.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/example.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/example.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/checksum_fuzzer.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/checksum_fuzzer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/compress_fuzzer.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/compress_fuzzer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_dict_fuzzer.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_dict_fuzzer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_flush_fuzzer.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_flush_fuzzer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_large_fuzzer.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_large_fuzzer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_small_fuzzer.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_small_fuzzer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/minigzip_fuzzer.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/minigzip_fuzzer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/standalone_fuzz_target_runner.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/standalone_fuzz_target_runner.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/gh1235.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/gh1235.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/hash_head_0.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/hash_head_0.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/infcover.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/infcover.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/inflate_adler32.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/inflate_adler32.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minideflate.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minideflate.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minigzip.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minigzip.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pigz/CMakeLists.txt` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pigz/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pkgcheck.sh` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pkgcheck.sh`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/switchlevels.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/switchlevels.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/testCVEinputs.sh` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/testCVEinputs.sh`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/config.sub` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/config.sub`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makecrct.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makecrct.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makefixed.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makefixed.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/maketrees.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/maketrees.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_emit.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_emit.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl._h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl._h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/uncompr.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/uncompr.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/DLL_FAQ.txt` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/DLL_FAQ.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.a64` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.a64`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.arm` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.arm`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.msc` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.msc`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/README-WIN32.txt` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/README-WIN32.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng.def` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng.def`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng1.rc` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng1.rc`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib.def` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib.def`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib1.rc` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib1.rc`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlibcompat.def` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlibcompat.def`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zbuild.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zbuild.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf-ng.h.in` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf-ng.h.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.in` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.included` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.included`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zendian.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zendian.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.map` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.map`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.map` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.map`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil_p.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil_p.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/BUCK` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/BUCK`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/Makefile` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/Makefile`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/README.md` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/allocations.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/allocations.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bits.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bits.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bitstream.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bitstream.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/compiler.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/compiler.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/cpu.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/cpu.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/entropy_common.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/entropy_common.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse_decompress.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/huf.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/huf.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/mem.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/mem.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/portability_macros.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/portability_macros.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_common.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_common.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_deps.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_deps.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_internal.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_internal.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_trace.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_trace.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/clevels.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/clevels.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/fse_compress.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/fse_compress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/huf_compress.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/huf_compress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_internal.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_internal.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_cwksp.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_cwksp.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm_geartab.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm_geartab.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress_amd64.S` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress_amd64.S`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_internal.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_internal.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_common.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_common.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_compress.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_compress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_decompress.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_decompress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/fastcover.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/fastcover.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/zdict.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/zdict.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/Makefile` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/Makefile`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/README.md` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.sln` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.sln`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.vcxproj` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_legacy.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_legacy.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.c` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/libzstd.mk` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/libzstd.mk`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/module.modulemap` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/module.modulemap`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zdict.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zdict.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd_errors.h` & `blosc2-2.2.5/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd_errors.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/README.md` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/codecs-registry.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/codecs-registry.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/CMakeLists.txt` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/README.md` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz-private.h` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz-private.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.h` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.h` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.h` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/test_ndlz.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/test_ndlz.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.h` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/CMakeLists.txt` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/README.md` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.h` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/include/bitstream.h` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/include/bitstream.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/system.h` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/system.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/types.h` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/types.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/version.h` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/version.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp.h` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/bitstream.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/bitstream.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/share/omp.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/share/omp.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/share/parallel.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/share/parallel.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec2.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec3.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec3.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec4.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codecf.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codecf.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/compress.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/compress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode1.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode1.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode2.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode3.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode3.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode4.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decodef.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decodef.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decompress.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decompress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode1.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode1.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode2.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode3.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode3.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode4.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodef.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodef.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodei.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodei.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/ompcompress.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/ompcompress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode3.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode3.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode4.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecodef.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecodef.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode3.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode3.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode4.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencodef.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencodef.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsd.h` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsd.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsf.h` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsf.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/src/zfp.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/src/zfp.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_acc_float.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_acc_float.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_prec_float.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_prec_float.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_float.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_float.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_getitem.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_getitem.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/codecs/zfp/zfp-private.h` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/codecs/zfp/zfp-private.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/bytedelta/CMakeLists.txt` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/bytedelta/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.c`

 * *Files 24% similar despite different names*

```diff
@@ -42,14 +42,16 @@
   x = _mm_add_epi8(x, _mm_slli_epi64(x, 8));
   x = _mm_add_epi8(x, _mm_slli_epi64(x, 16));
   x = _mm_add_epi8(x, _mm_slli_epi64(x, 32));
   x = _mm_add_epi8(x, _mm_shuffle_epi8(x, _mm_setr_epi8(-1,-1,-1,-1,-1,-1,-1,-1,7,7,7,7,7,7,7,7)));
   return x;
 }
 
+uint8_t simd_get_last(bytes16 x) { return (_mm_extract_epi16(x, 7) >> 8) & 0xFF; }
+
 #elif defined(__aarch64__) || defined(_M_ARM64)
 // ARM v8 NEON code path
 #define CPU_HAS_SIMD 1
 #include <arm_neon.h>
 typedef uint8x16_t bytes16;
 bytes16 simd_zero() { return vdupq_n_u8(0); }
 bytes16 simd_set1(uint8_t v) { return vdupq_n_u8(v); }
@@ -68,14 +70,16 @@
   x = vaddq_u8(x, vextq_u8(zero, x, 16 - 1));
   x = vaddq_u8(x, vextq_u8(zero, x, 16 - 2));
   x = vaddq_u8(x, vextq_u8(zero, x, 16 - 4));
   x = vaddq_u8(x, vextq_u8(zero, x, 16 - 8));
   return x;
 }
 
+uint8_t simd_get_last(bytes16 x) { return vgetq_lane_u8(x, 15); }
+
 #endif
 
 
 // Fetch 16b from N streams, compute SIMD delta
 int bytedelta_forward(const uint8_t *input, uint8_t *output, int32_t length, uint8_t meta,
                       blosc2_cparams *cparams, uint8_t id) {
   BLOSC_UNUSED_PARAM(id);
@@ -89,43 +93,139 @@
     blosc2_schunk* schunk = (blosc2_schunk*)(cparams->schunk);
     typesize = schunk->typesize;
   }
 
   const int stream_len = length / typesize;
   for (int ich = 0; ich < typesize; ++ich) {
     int ip = 0;
+    uint8_t _v2 = 0;
     // SIMD delta within each channel, store
 #if defined(CPU_HAS_SIMD)
     bytes16 v2 = {0};
     for (; ip < stream_len - 15; ip += 16) {
       bytes16 v = simd_load(input);
       input += 16;
       bytes16 delta = simd_sub(v, simd_concat(v, v2));
       simd_store(output, delta);
       output += 16;
       v2 = v;
     }
+    if (stream_len > 15) {
+      _v2 = simd_get_last(v2);
+    }
 #endif // #if defined(CPU_HAS_SIMD)
     // scalar leftover
-    uint8_t _v2 = 0;
     for (; ip < stream_len ; ip++) {
       uint8_t v = *input;
       input++;
       *output = v - _v2;
       output++;
       _v2 = v;
     }
   }
 
   return BLOSC2_ERROR_SUCCESS;
 }
 
 // Fetch 16b from N streams, sum SIMD undelta
 int bytedelta_backward(const uint8_t *input, uint8_t *output, int32_t length, uint8_t meta,
-                      blosc2_dparams *dparams, uint8_t id) {
+                       blosc2_dparams *dparams, uint8_t id) {
+  BLOSC_UNUSED_PARAM(id);
+
+  int typesize = meta;
+  if (typesize == 0) {
+    if (dparams->schunk == NULL) {
+      BLOSC_TRACE_ERROR("When meta is 0, you need to be on a schunk!");
+      BLOSC_ERROR(BLOSC2_ERROR_FAILURE);
+    }
+    blosc2_schunk* schunk = (blosc2_schunk*)(dparams->schunk);
+    typesize = schunk->typesize;
+  }
+
+  const int stream_len = length / typesize;
+  for (int ich = 0; ich < typesize; ++ich) {
+    int ip = 0;
+    uint8_t _v2 = 0;
+    // SIMD fetch 16 bytes from each channel, prefix-sum un-delta
+#if defined(CPU_HAS_SIMD)
+    bytes16 v2 = {0};
+    for (; ip < stream_len - 15; ip += 16) {
+      bytes16 v = simd_load(input);
+      input += 16;
+      // un-delta via prefix sum
+      v2 = simd_add(simd_prefix_sum(v), simd_duplane15(v2));
+      simd_store(output, v2);
+      output += 16;
+    }
+    if (stream_len > 15) {
+      _v2 = simd_get_last(v2);
+    }
+#endif // #if defined(CPU_HAS_SIMD)
+    // scalar leftover
+    for (; ip < stream_len; ip++) {
+      uint8_t v = *input + _v2;
+      input++;
+      *output = v;
+      output++;
+      _v2 = v;
+    }
+  }
+
+  return BLOSC2_ERROR_SUCCESS;
+}
+
+// This is the original (and buggy) version of bytedelta.  It is kept here for backwards compatibility.
+// See #524 for details.
+// Fetch 16b from N streams, compute SIMD delta
+int bytedelta_forward_buggy(const uint8_t *input, uint8_t *output, int32_t length,
+                            uint8_t meta, blosc2_cparams *cparams, uint8_t id) {
+  BLOSC_UNUSED_PARAM(id);
+
+  int typesize = meta;
+  if (typesize == 0) {
+    if (cparams->schunk == NULL) {
+      BLOSC_TRACE_ERROR("When meta is 0, you need to be on a schunk!");
+      BLOSC_ERROR(BLOSC2_ERROR_FAILURE);
+    }
+    blosc2_schunk* schunk = (blosc2_schunk*)(cparams->schunk);
+    typesize = schunk->typesize;
+  }
+
+  const int stream_len = length / typesize;
+  for (int ich = 0; ich < typesize; ++ich) {
+    int ip = 0;
+    // SIMD delta within each channel, store
+#if defined(CPU_HAS_SIMD)
+    bytes16 v2 = {0};
+    for (; ip < stream_len - 15; ip += 16) {
+      bytes16 v = simd_load(input);
+      input += 16;
+      bytes16 delta = simd_sub(v, simd_concat(v, v2));
+      simd_store(output, delta);
+      output += 16;
+      v2 = v;
+    }
+#endif // #if defined(CPU_HAS_SIMD)
+    // scalar leftover
+    uint8_t _v2 = 0;
+    for (; ip < stream_len ; ip++) {
+      uint8_t v = *input;
+      input++;
+      *output = v - _v2;
+      output++;
+      _v2 = v;
+    }
+  }
+
+  return BLOSC2_ERROR_SUCCESS;
+}
+
+// Fetch 16b from N streams, sum SIMD undelta
+int bytedelta_backward_buggy(const uint8_t *input, uint8_t *output, int32_t length,
+                             uint8_t meta, blosc2_dparams *dparams, uint8_t id) {
   BLOSC_UNUSED_PARAM(id);
 
   int typesize = meta;
   if (typesize == 0) {
     if (dparams->schunk == NULL) {
       BLOSC_TRACE_ERROR("When meta is 0, you need to be on a schunk!");
       BLOSC_ERROR(BLOSC2_ERROR_FAILURE);
```

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.h` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.h`

 * *Files 13% similar despite different names*

```diff
@@ -15,10 +15,16 @@
 
 #include <stdint.h>
 
 int bytedelta_forward(const uint8_t* input, uint8_t* output, int32_t length, uint8_t meta,
                       blosc2_cparams* cparams, uint8_t id);
 
 int bytedelta_backward(const uint8_t* input, uint8_t* output, int32_t length, uint8_t meta,
-                      blosc2_dparams* dparams, uint8_t id);
+                       blosc2_dparams* dparams, uint8_t id);
 
-#endif /* BLOSC_PLUGINS_FILTERS_BYTEDELTA_BYTEDELTA_H*/
+int bytedelta_forward_buggy(const uint8_t* input, uint8_t* output, int32_t length, uint8_t meta,
+                            blosc2_cparams* cparams, uint8_t id);
+
+int bytedelta_backward_buggy(const uint8_t* input, uint8_t* output, int32_t length, uint8_t meta,
+                             blosc2_dparams* dparams, uint8_t id);
+
+#endif /* BLOSC_PLUGINS_FILTERS_BYTEDELTA_BYTEDELTA_H */
```

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/bytedelta/test_bytedelta.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndcell/test_ndcell.c`

 * *Files 4% similar despite different names*

```diff
@@ -6,80 +6,75 @@
     License: BSD 3-Clause (see LICENSE.txt)
 
     See LICENSE.txt for details about copyright and rights to use.
 
     Test program demonstrating use of the Blosc filter from C code.
     To compile this program:
 
-    $ gcc -O test_bytedelta.c -o test_bytedelta -lblosc2
+    $ gcc -O test_ndcell.c -o test_ndcell -lblosc2
 
     To run:
 
-    $ ./test_bytedelta
+    $ ./test_ndcell
     Successful roundtrip!
     Compression: 41472 -> 4937 (8.4x)
     rand: 36535 obtained
 
     Successful roundtrip!
     Compression: 1792 -> 1005 (1.8x)
-    mixed_values: 787 obtained
+    same_cells: 787 obtained
 
     Successful roundtrip!
     Compression: 16128 -> 1599 (10.1x)
-    arange_like: 14529 obtained
+    some_matches: 14529 obtained
 
 **********************************************************************/
 
+#include "ndcell.h"
 #include "blosc2/filters-registry.h"
 #include "b2nd.h"
 
 #include <inttypes.h>
 #include <stdlib.h>
 #include <stdio.h>
 #include <stdint.h>
 
-static int test_bytedelta(blosc2_schunk *schunk) {
+static int test_ndcell(blosc2_schunk *schunk) {
 
   int64_t nchunks = schunk->nchunks;
   int32_t chunksize = (int32_t) (schunk->chunksize);
+  //   int isize = (int) array->extchunknitems * typesize;
   uint8_t *data_in = malloc(chunksize);
   int decompressed;
   int64_t csize;
   int64_t dsize;
   int64_t csize_f = 0;
   uint8_t *data_out = malloc(chunksize + BLOSC2_MAX_OVERHEAD);
   uint8_t *data_dest = malloc(chunksize);
 
   /* Create a context for compression */
   blosc2_cparams cparams = BLOSC2_CPARAMS_DEFAULTS;
+  cparams.splitmode = BLOSC_ALWAYS_SPLIT;
   cparams.typesize = schunk->typesize;
   cparams.compcode = BLOSC_LZ4;
-  cparams.filters[BLOSC2_MAX_FILTERS - 2] = BLOSC_SHUFFLE;
-  cparams.filters[BLOSC2_MAX_FILTERS - 1] = BLOSC_FILTER_BYTEDELTA;
-  cparams.filters_meta[BLOSC2_MAX_FILTERS - 1] = 0;  // 0 means typesize when using schunks
+  cparams.filters[4] = BLOSC_FILTER_NDCELL;
+  cparams.filters_meta[4] = 4;
+  cparams.filters[BLOSC2_MAX_FILTERS - 1] = BLOSC_SHUFFLE;
   cparams.clevel = 9;
   cparams.nthreads = 1;
   cparams.blocksize = schunk->blocksize;
   cparams.schunk = schunk;
   blosc2_context *cctx;
   cctx = blosc2_create_cctx(cparams);
-  if (cctx == NULL) {
-    printf("Cannot create compression context!\n");
-    return -1;
-  }
 
   blosc2_dparams dparams = BLOSC2_DPARAMS_DEFAULTS;
   dparams.nthreads = 1;
   dparams.schunk = schunk;
   blosc2_context *dctx;
   dctx = blosc2_create_dctx(dparams);
-  if (cctx == NULL) {
-    printf("Cannot create decompression context!\n");
-    return -1;
-  }
 
   for (int ci = 0; ci < nchunks; ci++) {
 
     decompressed = blosc2_schunk_decompress_chunk(schunk, ci, data_in, chunksize);
     if (decompressed < 0) {
       printf("Error decompressing chunk \n");
       return -1;
@@ -122,15 +117,15 @@
   printf("Successful roundtrip!\n");
   printf("Compression: %d -> %" PRId64 " (%.1fx)\n", chunksize, csize_f, (1. * chunksize) / (double) csize_f);
   return (int) (chunksize - csize_f);
 }
 
 
 int rand_() {
-  int8_t ndim = 3;
+  int ndim = 3;
   int typesize = 4;
   int64_t shape[] = {32, 18, 32};
   int32_t chunkshape[] = {17, 16, 24};
   int32_t blockshape[] = {8, 9, 8};
   int64_t nelem = 1;
   for (int i = 0; i < ndim; ++i) {
     nelem *= (int) (shape[i]);
@@ -150,36 +145,37 @@
                                         NULL, 0);
 
   b2nd_array_t *arr;
   BLOSC_ERROR(b2nd_from_cbuffer(ctx, &arr, data, size));
   blosc2_schunk *schunk = arr->sc;
 
   /* Run the test. */
-  int result = test_bytedelta(schunk);
+  int result = test_ndcell(schunk);
   BLOSC_ERROR(b2nd_free_ctx(ctx));
   BLOSC_ERROR(b2nd_free(arr));
   free(data);
+
   return result;
 }
 
-int mixed_values() {
-  int8_t ndim = 2;
-  int typesize = 4;
+int same_cells() {
+  int ndim = 2;
+  int typesize = 8;
   int64_t shape[] = {128, 111};
   int32_t chunkshape[] = {32, 11};
   int32_t blockshape[] = {16, 7};
   int64_t nelem = 1;
   for (int i = 0; i < ndim; ++i) {
     nelem *= (int) (shape[i]);
   }
   int64_t size = typesize * nelem;
-  int32_t *data = calloc(nelem, typesize);
-  for (int i = 0; i < (nelem / 4); i++) {
-    data[i * 4] = 11111111;
-    data[i * 4 + 1] = 99999999;
+  double *data = malloc(size);
+  for (int64_t i = 0; i < (nelem / 4); i++) {
+    data[i * 4] = (double) 11111111;
+    data[i * 4 + 1] = (double) 99999999;
   }
 
   blosc2_cparams cparams = BLOSC2_CPARAMS_DEFAULTS;
   cparams.typesize = typesize;
   blosc2_storage b2_storage = {.cparams=&cparams};
   b2_storage.contiguous = true;
 
@@ -187,75 +183,74 @@
                                         NULL, 0);
 
   b2nd_array_t *arr;
   BLOSC_ERROR(b2nd_from_cbuffer(ctx, &arr, data, size));
   blosc2_schunk *schunk = arr->sc;
 
   /* Run the test. */
-  int result = test_bytedelta(schunk);
+  int result = test_ndcell(schunk);
   BLOSC_ERROR(b2nd_free_ctx(ctx));
   BLOSC_ERROR(b2nd_free(arr));
   free(data);
 
   return result;
 }
 
-int arange_like() {
-  int8_t ndim = 2;
+int some_matches() {
+  int ndim = 2;
   int typesize = 8;
   int64_t shape[] = {128, 111};
   int32_t chunkshape[] = {48, 32};
   int32_t blockshape[] = {14, 18};
   int64_t nelem = 1;
   for (int i = 0; i < ndim; ++i) {
     nelem *= (int) (shape[i]);
   }
   int64_t size = typesize * nelem;
   double *data = malloc(size);
-  for (int64_t i = 0; i < nelem; i++) {
+  for (int64_t i = 0; i < (nelem / 2); i++) {
     data[i] = (double) i;
   }
+  for (int64_t i = (nelem / 2); i < nelem; i++) {
+    data[i] = (double) 1;
+  }
 
   blosc2_cparams cparams = BLOSC2_CPARAMS_DEFAULTS;
   cparams.typesize = typesize;
   blosc2_storage b2_storage = {.cparams=&cparams};
   b2_storage.contiguous = true;
 
   b2nd_context_t *ctx = b2nd_create_ctx(&b2_storage, ndim, shape, chunkshape, blockshape, NULL, 0,
                                         NULL, 0);
 
   b2nd_array_t *arr;
   BLOSC_ERROR(b2nd_from_cbuffer(ctx, &arr, data, size));
   blosc2_schunk *schunk = arr->sc;
 
   /* Run the test. */
-  int result = test_bytedelta(schunk);
+  int result = test_ndcell(schunk);
   BLOSC_ERROR(b2nd_free_ctx(ctx));
   BLOSC_ERROR(b2nd_free(arr));
   free(data);
 
   return result;
 }
 
 
 int main(void) {
   int result;
   blosc2_init();
-
   result = rand_();
-  printf("rand: saved %d bytes \n \n", result);
+  printf("rand: %d obtained \n \n", result);
   if (result < 0)
     return result;
-
-  result = mixed_values();
-  printf("mixed_values: saved %d bytes \n \n", result);
+  result = same_cells();
+  printf("same_cells: %d obtained \n \n", result);
   if (result < 0)
     return result;
-
-  result = arange_like();
-  printf("arange_like: saved %d bytes \n \n", result);
+  result = some_matches();
+  printf("some_matches: %d obtained \n \n", result);
   if (result < 0)
     return result;
-
   blosc2_destroy();
   return BLOSC2_ERROR_SUCCESS;
 }
```

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/filters-registry.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/filters-registry.c`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
-  Copyright (c) 2021  The Blosc Development Team <blosc@blosc.org> 
+  Copyright (c) 2021  The Blosc Development Team <blosc@blosc.org>
   https://blosc.org
   License: BSD 3-Clause (see LICENSE.txt)
 */
 
 #include "blosc2/filters-registry.h"
 #include "ndmean/ndmean.h"
 #include "ndcell/ndcell.h"
@@ -25,15 +25,25 @@
   ndmean.id = BLOSC_FILTER_NDMEAN;
   ndmean.name = "ndmean";
   ndmean.version = 1;
   ndmean.forward = &ndmean_forward;
   ndmean.backward = &ndmean_backward;
   register_filter_private(&ndmean);
 
+  // Buggy version. See #524
+  blosc2_filter bytedelta_buggy;
+  bytedelta_buggy.id = BLOSC_FILTER_BYTEDELTA_BUGGY;
+  bytedelta_buggy.name = "bytedelta_buggy";
+  bytedelta_buggy.version = 1;
+  bytedelta_buggy.forward = &bytedelta_forward_buggy;
+  bytedelta_buggy.backward = &bytedelta_backward_buggy;
+  register_filter_private(&bytedelta_buggy);
+
+  // Fixed version. See #524
   blosc2_filter bytedelta;
   bytedelta.id = BLOSC_FILTER_BYTEDELTA;
   bytedelta.name = "bytedelta";
+  bytedelta.version = 1;
   bytedelta.forward = &bytedelta_forward;
   bytedelta.backward = &bytedelta_backward;
   register_filter_private(&bytedelta);
-
 }
```

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndcell/CMakeLists.txt` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndcell/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndcell/README.md` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndcell/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.h` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndcell/test_ndcell.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_repart.c`

 * *Files 12% similar despite different names*

```diff
@@ -5,62 +5,83 @@
     https://blosc.org
     License: BSD 3-Clause (see LICENSE.txt)
 
     See LICENSE.txt for details about copyright and rights to use.
 
     Test program demonstrating use of the Blosc filter from C code.
     To compile this program:
-
-    $ gcc -O test_ndcell.c -o test_ndcell -lblosc2
+    $ gcc -O test_ndmean_repart.c -o test_ndmean_repart -lblosc2
 
     To run:
 
-    $ ./test_ndcell
+    $ ./test_ndmean_repart
+    Blosc version info: 2.0.0a6.dev ($Date:: 2018-05-18 #$)
+    Using 1 thread
+    Using ZSTD compressor
     Successful roundtrip!
-    Compression: 41472 -> 4937 (8.4x)
-    rand: 36535 obtained
+    Compression: 41472 -> 1015 (40.9x)
+    rand: 40457 obtained
 
     Successful roundtrip!
-    Compression: 1792 -> 1005 (1.8x)
-    same_cells: 787 obtained
+    Compression: 1792 -> 323 (5.5x)
+    same_cells: 1469 obtained
 
     Successful roundtrip!
-    Compression: 16128 -> 1599 (10.1x)
-    some_matches: 14529 obtained
+    Compression: 16128 -> 767 (21.0x)
+    some_matches: 15361 obtained
 
 **********************************************************************/
 
-#include "ndcell.h"
+#include "ndmean.h"
 #include "blosc2/filters-registry.h"
 #include "b2nd.h"
 
 #include <inttypes.h>
-#include <stdlib.h>
+#include <math.h>
 #include <stdio.h>
-#include <stdint.h>
 
-static int test_ndcell(blosc2_schunk *schunk) {
+#define EPSILON (float) (1e-5)
+
+static bool is_close(double d1, double d2) {
+
+  double aux = 1;
+  if (fabs(d1) < fabs(d2)) {
+    if (fabs(d1) > 0) {
+      aux = fabs(d2);
+    }
+  } else {
+    if (fabs(d2) > 0) {
+      aux = fabs(d1);
+    }
+  }
+
+  return fabs(d1 - d2) < aux * EPSILON;
+}
+
+
+static int test_ndmean(blosc2_schunk *schunk) {
 
+  int32_t typesize = schunk->typesize;
   int64_t nchunks = schunk->nchunks;
   int32_t chunksize = (int32_t) (schunk->chunksize);
   //   int isize = (int) array->extchunknitems * typesize;
   uint8_t *data_in = malloc(chunksize);
   int decompressed;
   int64_t csize;
   int64_t dsize;
   int64_t csize_f = 0;
   uint8_t *data_out = malloc(chunksize + BLOSC2_MAX_OVERHEAD);
   uint8_t *data_dest = malloc(chunksize);
 
   /* Create a context for compression */
   blosc2_cparams cparams = BLOSC2_CPARAMS_DEFAULTS;
   cparams.splitmode = BLOSC_ALWAYS_SPLIT;
-  cparams.typesize = schunk->typesize;
-  cparams.compcode = BLOSC_LZ4;
-  cparams.filters[4] = BLOSC_FILTER_NDCELL;
+  cparams.typesize = typesize;
+  cparams.compcode = BLOSC_BLOSCLZ;
+  cparams.filters[4] = BLOSC_FILTER_NDMEAN;
   cparams.filters_meta[4] = 4;
   cparams.filters[BLOSC2_MAX_FILTERS - 1] = BLOSC_SHUFFLE;
   cparams.clevel = 9;
   cparams.nthreads = 1;
   cparams.blocksize = schunk->blocksize;
   cparams.schunk = schunk;
   blosc2_context *cctx;
@@ -94,20 +115,35 @@
     /* Decompress  */
     dsize = blosc2_decompress_ctx(dctx, data_out, chunksize + BLOSC2_MAX_OVERHEAD, data_dest, chunksize);
     if (dsize <= 0) {
       printf("Decompression error.  Error code: %" PRId64 "\n", dsize);
       return (int) dsize;
     }
 
-    for (int i = 0; i < chunksize; i++) {
-      if (data_in[i] != data_dest[i]) {
-        printf("i: %d, data %u, dest %u", i, data_in[i], data_dest[i]);
-        printf("\n Decompressed data differs from original!\n");
-        return -1;
-      }
+    switch (typesize) {
+      case 4:
+        for (int i = 0; i < chunksize / typesize; i++) {
+          if (!is_close(((float *) data_in)[i], ((float *) data_dest)[i])) {
+            printf("i: %d, data %.9f, dest %.9f", i, ((float *) data_in)[i], ((float *) data_dest)[i]);
+            printf("\n Decompressed data differs from original!\n");
+            return -1;
+          }
+        }
+        break;
+      case 8:
+        for (int i = 0; i < chunksize / typesize; i++) {
+          if (!is_close(((double *) data_in)[i], ((double *) data_dest)[i])) {
+            printf("i: %d, data %.9f, dest %.9f", i, ((double *) data_in)[i], ((double *) data_dest)[i]);
+            printf("\n Decompressed data differs from original!\n");
+            return -1;
+          }
+        }
+        break;
+      default :
+        break;
     }
   }
   csize_f = csize_f / nchunks;
 
   free(data_in);
   free(data_out);
   free(data_dest);
@@ -116,141 +152,99 @@
 
   printf("Successful roundtrip!\n");
   printf("Compression: %d -> %" PRId64 " (%.1fx)\n", chunksize, csize_f, (1. * chunksize) / (double) csize_f);
   return (int) (chunksize - csize_f);
 }
 
 
-int rand_() {
-  int ndim = 3;
-  int typesize = 4;
-  int64_t shape[] = {32, 18, 32};
-  int32_t chunkshape[] = {17, 16, 24};
-  int32_t blockshape[] = {8, 9, 8};
-  int64_t nelem = 1;
-  for (int i = 0; i < ndim; ++i) {
-    nelem *= (int) (shape[i]);
-  }
-  int64_t size = typesize * nelem;
-  float *data = malloc(size);
-  for (int64_t i = 0; i < nelem; i++) {
-    data[i] = (float) (rand() % 220);
-  }
-
-  blosc2_cparams cparams = BLOSC2_CPARAMS_DEFAULTS;
-  cparams.typesize = typesize;
-  blosc2_storage b2_storage = {.cparams=&cparams};
-  b2_storage.contiguous = true;
-
-  b2nd_context_t *ctx = b2nd_create_ctx(&b2_storage, ndim, shape, chunkshape, blockshape, NULL, 0,
-                                        NULL, 0);
-
-  b2nd_array_t *arr;
-  BLOSC_ERROR(b2nd_from_cbuffer(ctx, &arr, data, size));
-  blosc2_schunk *schunk = arr->sc;
-
-  /* Run the test. */
-  int result = test_ndcell(schunk);
-  BLOSC_ERROR(b2nd_free_ctx(ctx));
-  BLOSC_ERROR(b2nd_free(arr));
-  free(data);
-
-  return result;
-}
-
 int same_cells() {
-  int ndim = 2;
+  int ndim = 3;
   int typesize = 8;
-  int64_t shape[] = {128, 111};
-  int32_t chunkshape[] = {32, 11};
-  int32_t blockshape[] = {16, 7};
-  int64_t nelem = 1;
+  int64_t shape[] = {128, 64, 32};
+  int32_t chunkshape[] = {32, 32, 16};
+  int32_t blockshape[] = {16, 8, 8};
+  int64_t isize = 1;
   for (int i = 0; i < ndim; ++i) {
-    nelem *= (int) (shape[i]);
+    isize *= (int) (shape[i]);
   }
-  int64_t size = typesize * nelem;
-  double *data = malloc(size);
-  for (int64_t i = 0; i < (nelem / 4); i++) {
-    data[i * 4] = (double) 11111111;
-    data[i * 4 + 1] = (double) 99999999;
+  int64_t nbytes = typesize * isize;
+  double *data = malloc(nbytes);
+  for (int64_t i = 0; i < isize; i += 4) {
+    data[i] = 123412240;
+    data[i + 1] = 123412221;
+    data[i + 2] = 123412232;
+    data[i + 3] = 123412211;
   }
 
   blosc2_cparams cparams = BLOSC2_CPARAMS_DEFAULTS;
   cparams.typesize = typesize;
   blosc2_storage b2_storage = {.cparams=&cparams};
   b2_storage.contiguous = true;
 
   b2nd_context_t *ctx = b2nd_create_ctx(&b2_storage, ndim, shape, chunkshape, blockshape, NULL, 0,
                                         NULL, 0);
 
   b2nd_array_t *arr;
-  BLOSC_ERROR(b2nd_from_cbuffer(ctx, &arr, data, size));
+  BLOSC_ERROR(b2nd_from_cbuffer(ctx, &arr, data, nbytes));
   blosc2_schunk *schunk = arr->sc;
 
   /* Run the test. */
-  int result = test_ndcell(schunk);
+  int result = test_ndmean(schunk);
   BLOSC_ERROR(b2nd_free_ctx(ctx));
   BLOSC_ERROR(b2nd_free(arr));
-  free(data);
-
   return result;
 }
 
 int some_matches() {
   int ndim = 2;
   int typesize = 8;
-  int64_t shape[] = {128, 111};
+  int64_t shape[] = {128, 128};
   int32_t chunkshape[] = {48, 32};
-  int32_t blockshape[] = {14, 18};
-  int64_t nelem = 1;
+  int32_t blockshape[] = {16, 16};
+  int64_t isize = 1;
   for (int i = 0; i < ndim; ++i) {
-    nelem *= (int) (shape[i]);
+    isize *= (int) (shape[i]);
   }
-  int64_t size = typesize * nelem;
-  double *data = malloc(size);
-  for (int64_t i = 0; i < (nelem / 2); i++) {
-    data[i] = (double) i;
+  int64_t nbytes = typesize * isize;
+  double *data = malloc(nbytes);
+  for (int64_t i = 0; i < (isize / 2); i++) {
+    data[i] = (double) (i / 200) + 133213124;
   }
-  for (int64_t i = (nelem / 2); i < nelem; i++) {
-    data[i] = (double) 1;
+  for (int64_t i = (isize / 2); i < isize; i++) {
+    data[i] = (double) (i / 100) + 133213124;
   }
 
   blosc2_cparams cparams = BLOSC2_CPARAMS_DEFAULTS;
   cparams.typesize = typesize;
   blosc2_storage b2_storage = {.cparams=&cparams};
   b2_storage.contiguous = true;
 
   b2nd_context_t *ctx = b2nd_create_ctx(&b2_storage, ndim, shape, chunkshape, blockshape, NULL, 0,
                                         NULL, 0);
 
   b2nd_array_t *arr;
-  BLOSC_ERROR(b2nd_from_cbuffer(ctx, &arr, data, size));
+  BLOSC_ERROR(b2nd_from_cbuffer(ctx, &arr, data, nbytes));
   blosc2_schunk *schunk = arr->sc;
 
   /* Run the test. */
-  int result = test_ndcell(schunk);
+  int result = test_ndmean(schunk);
   BLOSC_ERROR(b2nd_free_ctx(ctx));
   BLOSC_ERROR(b2nd_free(arr));
-  free(data);
-
   return result;
 }
 
 
 int main(void) {
+
   int result;
   blosc2_init();
-  result = rand_();
-  printf("rand: %d obtained \n \n", result);
-  if (result < 0)
-    return result;
   result = same_cells();
   printf("same_cells: %d obtained \n \n", result);
-  if (result < 0)
-    return result;
+  if (result <= 0)
+    return -1;
   result = some_matches();
   printf("some_matches: %d obtained \n \n", result);
-  if (result < 0)
-    return result;
+  if (result <= 0)
+    return -1;
   blosc2_destroy();
   return BLOSC2_ERROR_SUCCESS;
 }
```

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndmean/CMakeLists.txt` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndmean/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndmean/README.md` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndmean/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.h` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_mean.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_mean.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/plugin_utils.c` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/plugin_utils.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/test_data/README.md` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/test_data/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/test_data/example_day_month_temp.b2nd` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/test_data/example_day_month_temp.b2nd`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/plugins/test_data/example_item_prices.b2nd` & `blosc2-2.2.5/blosc2/c-blosc2/plugins/test_data/example_item_prices.b2nd`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/CMakeLists.txt` & `blosc2-2.2.5/blosc2/c-blosc2/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/Makefile` & `blosc2-2.2.5/blosc2/c-blosc2/tests/Makefile`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/CMakeLists.txt` & `blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/cutest.h` & `blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/cutest.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_append.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_append.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_copy.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_copy.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_delete.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_delete.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_full.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_full.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice_buffer.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice_buffer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_insert.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_insert.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_metalayers.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_metalayers.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_open_offset.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_open_offset.c`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
   // fileframe (file) + offset -> schunk (on-disk contiguous, super-chunk)
   blosc_set_timestamp(&last);
   b2nd_array_t* arr_read_offset;
   BLOSC_ERROR(b2nd_open_offset("file:///frame_simple.b2frame", &arr_read_offset, offset));
   blosc_set_timestamp(&current);
   ttotal = blosc_elapsed_secs(last, current);
   printf("Time for fileframe (%s) + offset %ld -> open_offset : %.3g s, %.1f GB/s\n",
-         arr_read_offset->sc->storage->urlpath, offset, ttotal, (double)arr_read_offset->sc->nbytes / (ttotal * GB));
+         arr_read_offset->sc->storage->urlpath, (long)offset, ttotal, (double)arr_read_offset->sc->nbytes / (ttotal * GB));
 
   uint8_t* cframe_read_start, *cframe_read_offset;
   bool cframe_needs_free2, cframe_needs_free3;
   int64_t frame_len2 = b2nd_to_cframe(arr_read_start, &cframe_read_start, &frame_len,
                                       &cframe_needs_free2);
   if (frame_len2 != frame_len) {
     return (int)frame_len2;
```

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_persistency.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_persistency.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_resize.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_resize.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_roundtrip.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_roundtrip.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_save.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_save.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_serialize.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_serialize.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_set_slice_buffer.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_set_slice_buffer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze_index.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze_index.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_uninit.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_uninit.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_b2nd_zeros.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_b2nd_zeros.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/b2nd/test_common.h` & `blosc2-2.2.5/blosc2/c-blosc2/tests/b2nd/test_common.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/cutest.h` & `blosc2-2.2.5/blosc2/c-blosc2/tests/cutest.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/CMakeLists.txt` & `blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/README.md` & `blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/corpus/README.md` & `blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/corpus/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-blosclz.b2frame` & `blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-blosclz.b2frame`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4.b2frame` & `blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4.b2frame`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4hc.b2frame` & `blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4hc.b2frame`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zlib.b2frame` & `blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zlib.b2frame`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zstd.b2frame` & `blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zstd.b2frame`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/fuzz_compress_chunk.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/fuzz_compress_chunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/fuzz_compress_frame.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/fuzz_compress_frame.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_chunk.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_chunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_frame.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_frame.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/generate_inputs_corpus.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/generate_inputs_corpus.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/fuzz/standalone.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/fuzz/standalone.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/gcc-segfault-issue.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/gcc-segfault-issue.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/print_versions.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/print_versions.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_api.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_api.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_bitshuffle_leftovers.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_bitshuffle_leftovers.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_blosc1_compat.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_blosc1_compat.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_change_nthreads_append.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_change_nthreads_append.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_common.h` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_common.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_compress_roundtrip.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_compress_roundtrip.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_compress_roundtrip.csv` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_compress_roundtrip.csv`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_compressor.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_compressor.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_contexts.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_contexts.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_copy.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_copy.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_delete_chunk.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_delete_chunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_delta.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_delta.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_delta_schunk.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_delta_schunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_dict_schunk.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_dict_schunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_empty_buffer.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_empty_buffer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_fill_special.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_fill_special.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_frame.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_frame.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_frame_get_offsets.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_frame_get_offsets.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_frame_offset.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_frame_offset.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_get_slice_buffer.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_get_slice_buffer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_getitem.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_getitem.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_getitem.csv` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_getitem.csv`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_getitem_delta.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_getitem_delta.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_insert_chunk.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_insert_chunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_lazychunk.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_lazychunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_lazychunk_memcpyed.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_lazychunk_memcpyed.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_maskout.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_maskout.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_maxout.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_maxout.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_noinit.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_noinit.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_nolock.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_nolock.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_nthreads.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_nthreads.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_postfilter.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_postfilter.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_prefilter.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_prefilter.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_reorder_offsets.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_reorder_offsets.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_schunk.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_schunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_schunk_frame.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_schunk_frame.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_schunk_header.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_schunk_header.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_set_slice_buffer.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_set_slice_buffer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_sframe.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_sframe.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_sframe_lazychunk.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_sframe_lazychunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.csv` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.csv`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.csv` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.csv`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.csv` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.csv`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.csv` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.csv`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.csv` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.csv`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_small_chunks.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_small_chunks.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_udio.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_udio.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_update_chunk.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_update_chunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_urcodecs.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_urcodecs.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_urfilters.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_urfilters.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/c-blosc2/tests/test_zero_runlen.c` & `blosc2-2.2.5/blosc2/c-blosc2/tests/test_zero_runlen.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/core.py` & `blosc2-2.2.5/blosc2/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -680,17 +680,17 @@
 
     Examples
     --------
     >>> import os
     >>> import numpy as np
     >>> th = np.arange(1e3, dtype=np.float32)
     >>> cframe = blosc2.pack_tensor(th)
-    >>> if not os.getenv("BTUNE_BALANCE"):
+    >>> if not os.getenv("BTUNE_TRADEOFF"):
     ...     assert len(cframe) < th.size * th.itemsize
-    ... 
+    ...
     >>> th2 = blosc2.unpack_tensor(cframe)
     >>> a = np.asarray(th)
     >>> a2 = np.asarray(th2)
     >>> np.array_equal(a, a2)
     True
 
     See also
```

### Comparing `blosc2-2.2.4/blosc2/info.py` & `blosc2-2.2.5/blosc2/info.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/ndarray.py` & `blosc2-2.2.5/blosc2/ndarray.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2/schunk.py` & `blosc2-2.2.5/blosc2/schunk.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/blosc2.egg-info/PKG-INFO` & `blosc2-2.2.5/blosc2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blosc2
-Version: 2.2.4
+Version: 2.2.5
 Summary: Python wrapper for the C-Blosc2 library
 Author-email: Blosc Development Team <blosc@blosc.org>
 Maintainer-email: Blosc Development Team <blosc@blosc.org>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/Blosc/python-blosc2
 Project-URL: documentation, https://www.blosc.org/python-blosc2/python-blosc2.html
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `blosc2-2.2.4/blosc2.egg-info/SOURCES.txt` & `blosc2-2.2.5/blosc2.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -791,14 +791,15 @@
 blosc2/c-blosc2/tests/test_copy.c
 blosc2/c-blosc2/tests/test_delete_chunk.c
 blosc2/c-blosc2/tests/test_delta.c
 blosc2/c-blosc2/tests/test_delta_schunk.c
 blosc2/c-blosc2/tests/test_dict_schunk.c
 blosc2/c-blosc2/tests/test_empty_buffer.c
 blosc2/c-blosc2/tests/test_fill_special.c
+blosc2/c-blosc2/tests/test_filters.c
 blosc2/c-blosc2/tests/test_frame.c
 blosc2/c-blosc2/tests/test_frame_get_offsets.c
 blosc2/c-blosc2/tests/test_frame_offset.c
 blosc2/c-blosc2/tests/test_get_slice_buffer.c
 blosc2/c-blosc2/tests/test_getitem.c
 blosc2/c-blosc2/tests/test_getitem.csv
 blosc2/c-blosc2/tests/test_getitem_delta.c
```

### Comparing `blosc2-2.2.4/doc/_static/blosc-logo_128.png` & `blosc2-2.2.5/doc/_static/blosc-logo_128.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/_static/blosc-logo_256.png` & `blosc2-2.2.5/doc/_static/blosc-logo_256.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/_static/css/custom.css` & `blosc2-2.2.5/doc/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/conf.py` & `blosc2-2.2.5/doc/conf.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/getting_started/installation.rst` & `blosc2-2.2.5/doc/getting_started/installation.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/getting_started/overview.rst` & `blosc2-2.2.5/doc/getting_started/overview.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/getting_started/tutorials/00.schunk-basics.ipynb` & `blosc2-2.2.5/doc/getting_started/tutorials/00.schunk-basics.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996527777777777%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Basics: compressing data with the SChunk class\\n')], "*

 * *            'delete: [0]}}}'}*

```diff
@@ -1,14 +1,14 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Basics: compressing data with Super-Chunks\n",
+                "# Basics: compressing data with the SChunk class\n",
                 "\n",
                 "Python-Blosc2 is a thin wrapper for the C-Blosc2 format and compression library.  It allows to easily and quickly create, append, insert, update and delete data and metadata in a super-chunk container (SChunk class)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
```

### Comparing `blosc2-2.2.4/doc/getting_started/tutorials/01.schunk-slicing_and_beyond.ipynb` & `blosc2-2.2.5/doc/getting_started/tutorials/01.schunk-slicing_and_beyond.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996843434343434%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, '## Getting data from a SChunk\\n')], delete: [2]}}}"}*

```diff
@@ -31,15 +31,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "It is important to set the `typesize` correctly as these methods will work with items and not with bytes.\n",
                 "\n",
-                "## Getting data in a SChunk\n",
+                "## Getting data from a SChunk\n",
                 "\n",
                 "Let's begin by retrieving the data from the whole SChunk. We could use the `decompress_chunk` method:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
```

### Comparing `blosc2-2.2.4/doc/getting_started/tutorials/02.ndarray-basics.ipynb` & `blosc2-2.2.5/doc/getting_started/tutorials/02.ndarray-basics.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993872549019608%*

 * *Differences: {"'cells'": "{12: {'source': ['This time we even set the chunks and blocks shapes. You can now "*

 * *            "open it with modes `w`, `a` or `r`.']}}"}*

```diff
@@ -250,19 +250,15 @@
                 "print(array.info)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "This time we even set the chunks and blocks shapes.\n",
-                "\n",
-                "## Updating and inserting\n",
-                "\n",
-                "First, let's update the first chunk:"
+                "This time we even set the chunks and blocks shapes. You can now open it with modes `w`, `a` or `r`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {
                 "ExecuteTime": {
```

### Comparing `blosc2-2.2.4/doc/getting_started/tutorials/10.ucodecs-ufilters.ipynb` & `blosc2-2.2.5/doc/getting_started/tutorials/10.ucodecs-ufilters.ipynb`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/getting_started/tutorials/11.prefilters.ipynb` & `blosc2-2.2.5/doc/getting_started/tutorials/11.prefilters.ipynb`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/getting_started/tutorials/12.postfilters.ipynb` & `blosc2-2.2.5/doc/getting_started/tutorials/12.postfilters.ipynb`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/getting_started/tutorials/images/blosc2-pipeline.png` & `blosc2-2.2.5/doc/getting_started/tutorials/images/blosc2-pipeline.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/getting_started/tutorials/images/blosc2-pipeline.svg` & `blosc2-2.2.5/doc/getting_started/tutorials/images/blosc2-pipeline.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/backward.png` & `blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/backward.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/backward.svg` & `blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/backward.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/decoder.png` & `blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/decoder.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/decoder.svg` & `blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/decoder.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/decoder2.png` & `blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/decoder2.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/decoder2.svg` & `blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/decoder2.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/encoder.png` & `blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/encoder.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/encoder.svg` & `blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/encoder.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/encoder2.png` & `blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/encoder2.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/encoder2.svg` & `blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/encoder2.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/forward.png` & `blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/forward.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/getting_started/tutorials/images/ucodecs-filters/forward.svg` & `blosc2-2.2.5/doc/getting_started/tutorials/images/ucodecs-filters/forward.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/python-blosc2.rst` & `blosc2-2.2.5/doc/python-blosc2.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     ---
 
     Getting Started
     ^^^^^^^^^^^^^^^
 
     New to Python-Blosc2? Check out the getting started guides. They contain an
-    introduction to Python-Blosc2 main concepts and an installation tutorial.
+    introduction to Python-Blosc2 main concepts and different tutorials.
 
     +++
 
     .. link-button:: getting_started/index
             :type: ref
             :text: To the getting started guides
             :classes: btn-info
@@ -74,8 +74,8 @@
 ..  toctree::
     :maxdepth: 1
     :hidden:
 
     Getting Started <getting_started/index>
     API Reference <reference/index>
     Development <development/index>
-    Release Notes <release_notes/index>
+    Release Notes <release_notes/index>
```

### Comparing `blosc2-2.2.4/doc/reference/autofiles/schunk/attributes/meta.rst` & `blosc2-2.2.5/doc/reference/autofiles/schunk/attributes/meta.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/reference/autofiles/schunk/attributes/vlmeta.rst` & `blosc2-2.2.5/doc/reference/autofiles/schunk/attributes/vlmeta.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/reference/ndarray_api.rst` & `blosc2-2.2.5/doc/reference/ndarray_api.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/reference/schunk_api.rst` & `blosc2-2.2.5/doc/reference/schunk_api.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/doc/reference/top_level.rst` & `blosc2-2.2.5/doc/reference/top_level.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/compress2_decompress2.py` & `blosc2-2.2.5/examples/compress2_decompress2.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/compress_decompress.py` & `blosc2-2.2.5/examples/compress_decompress.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/filler.py` & `blosc2-2.2.5/examples/filler.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/ndarray/asarray_.py` & `blosc2-2.2.5/examples/ndarray/asarray_.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/ndarray/buffer.py` & `blosc2-2.2.5/examples/ndarray/buffer.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/ndarray/bytedelta_filter.py` & `blosc2-2.2.5/examples/ndarray/bytedelta_filter.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/ndarray/copy_.py` & `blosc2-2.2.5/examples/ndarray/copy_.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/ndarray/empty_.py` & `blosc2-2.2.5/examples/ndarray/empty_.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/ndarray/formats.py` & `blosc2-2.2.5/examples/ndarray/formats.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/ndarray/getitem.py` & `blosc2-2.2.5/examples/ndarray/getitem.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/ndarray/iterchunks_info.py` & `blosc2-2.2.5/examples/ndarray/iterchunks_info.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/ndarray/meta.py` & `blosc2-2.2.5/examples/ndarray/meta.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/ndarray/ndarray_copy.py` & `blosc2-2.2.5/examples/ndarray/ndarray_copy.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/ndarray/ndmean.py` & `blosc2-2.2.5/examples/ndarray/ndmean.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/ndarray/persistency.py` & `blosc2-2.2.5/examples/ndarray/persistency.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/ndarray/resize_.py` & `blosc2-2.2.5/examples/ndarray/resize_.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/ndarray/work_with_numpy.py` & `blosc2-2.2.5/examples/ndarray/work_with_numpy.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/ndarray/zfp_codec.py` & `blosc2-2.2.5/examples/ndarray/zfp_codec.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/pack_array.py` & `blosc2-2.2.5/examples/pack_array.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/pack_tensor.py` & `blosc2-2.2.5/examples/pack_tensor.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/postfilter1.py` & `blosc2-2.2.5/examples/postfilter1.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/postfilter2.py` & `blosc2-2.2.5/examples/postfilter2.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/postfilter3.py` & `blosc2-2.2.5/examples/postfilter3.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/prefilter.py` & `blosc2-2.2.5/examples/prefilter.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/save_tensor.py` & `blosc2-2.2.5/examples/save_tensor.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/schunk.py` & `blosc2-2.2.5/examples/schunk.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/schunk_roundtrip.py` & `blosc2-2.2.5/examples/schunk_roundtrip.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/ucodecs.py` & `blosc2-2.2.5/examples/ucodecs.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/ufilters.py` & `blosc2-2.2.5/examples/ufilters.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/examples/vlmeta.py` & `blosc2-2.2.5/examples/vlmeta.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/images/Complete-Write-Read-B2ND.png` & `blosc2-2.2.5/images/Complete-Write-Read-B2ND.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/images/M1-i386-vs-arm64-pack.png` & `blosc2-2.2.5/images/M1-i386-vs-arm64-pack.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/images/M1-i386-vs-arm64-unpack.png` & `blosc2-2.2.5/images/M1-i386-vs-arm64-unpack.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/images/Read-Partial-Slices-B2ND.png` & `blosc2-2.2.5/images/Read-Partial-Slices-B2ND.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/images/b2nd-2level-parts.png` & `blosc2-2.2.5/images/b2nd-2level-parts.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/images/linspace-compress.png` & `blosc2-2.2.5/images/linspace-compress.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/images/linspace-decompress.png` & `blosc2-2.2.5/images/linspace-decompress.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/images/pack-array-cratios.png` & `blosc2-2.2.5/images/pack-array-cratios.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/pyproject.toml` & `blosc2-2.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/setup.py` & `blosc2-2.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/ndarray/test_auto_parts.py` & `blosc2-2.2.5/tests/ndarray/test_auto_parts.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/ndarray/test_buffer.py` & `blosc2-2.2.5/tests/ndarray/test_buffer.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/ndarray/test_copy.py` & `blosc2-2.2.5/tests/ndarray/test_copy.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/ndarray/test_empty.py` & `blosc2-2.2.5/tests/ndarray/test_empty.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/ndarray/test_full.py` & `blosc2-2.2.5/tests/ndarray/test_full.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/ndarray/test_getitem.py` & `blosc2-2.2.5/tests/ndarray/test_getitem.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/ndarray/test_iterchunks_info.py` & `blosc2-2.2.5/tests/ndarray/test_iterchunks_info.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/ndarray/test_lossy.py` & `blosc2-2.2.5/tests/ndarray/test_lossy.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/ndarray/test_metalayers.py` & `blosc2-2.2.5/tests/ndarray/test_metalayers.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/ndarray/test_mode.py` & `blosc2-2.2.5/tests/ndarray/test_mode.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/ndarray/test_numpy.py` & `blosc2-2.2.5/tests/ndarray/test_numpy.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/ndarray/test_persistency.py` & `blosc2-2.2.5/tests/ndarray/test_persistency.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/ndarray/test_resize.py` & `blosc2-2.2.5/tests/ndarray/test_resize.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/ndarray/test_setitem.py` & `blosc2-2.2.5/tests/ndarray/test_setitem.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/ndarray/test_slice.py` & `blosc2-2.2.5/tests/ndarray/test_slice.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/ndarray/test_squeeze.py` & `blosc2-2.2.5/tests/ndarray/test_squeeze.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/ndarray/test_struct_dtype.py` & `blosc2-2.2.5/tests/ndarray/test_struct_dtype.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/ndarray/test_zeros.py` & `blosc2-2.2.5/tests/ndarray/test_zeros.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/test_bytes_array.py` & `blosc2-2.2.5/tests/test_bytes_array.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/test_comp_info.py` & `blosc2-2.2.5/tests/test_comp_info.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/test_compress2.py` & `blosc2-2.2.5/tests/test_compress2.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/test_compression_parameters.py` & `blosc2-2.2.5/tests/test_compression_parameters.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/test_compressors.py` & `blosc2-2.2.5/tests/test_compressors.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/test_decompress.py` & `blosc2-2.2.5/tests/test_decompress.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/test_iterchunks.py` & `blosc2-2.2.5/tests/test_iterchunks.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/test_open.py` & `blosc2-2.2.5/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/test_postfilters.py` & `blosc2-2.2.5/tests/test_postfilters.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/test_prefilters.py` & `blosc2-2.2.5/tests/test_prefilters.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/test_python_blosc.py` & `blosc2-2.2.5/tests/test_python_blosc.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/test_schunk.py` & `blosc2-2.2.5/tests/test_schunk.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     blosc2.remove_urlpath(urlpath)
 
     data = np.arange(200 * 1000 * nchunks, dtype="int32")
     schunk = blosc2.SChunk(chunksize=200 * 1000 * 4, data=data, **storage)
 
     cframe = schunk.to_cframe()
     schunk2 = blosc2.schunk_from_cframe(cframe, copy)
-    if not os.getenv("BTUNE_BALANCE"):
+    if not os.getenv("BTUNE_TRADEOFF"):
         for key in cparams:
             if key == "nthreads":
                 continue
             assert schunk2.cparams[key] == cparams[key]
 
     data2 = np.empty(data.shape, dtype=data.dtype)
     schunk2.get_slice(out=data2)
```

### Comparing `blosc2-2.2.4/tests/test_schunk_constructor.py` & `blosc2-2.2.5/tests/test_schunk_constructor.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/test_schunk_delete.py` & `blosc2-2.2.5/tests/test_schunk_delete.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/test_schunk_get_slice.py` & `blosc2-2.2.5/tests/test_schunk_get_slice.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/test_schunk_insert.py` & `blosc2-2.2.5/tests/test_schunk_insert.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/test_schunk_set_slice.py` & `blosc2-2.2.5/tests/test_schunk_set_slice.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/test_schunk_update.py` & `blosc2-2.2.5/tests/test_schunk_update.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/test_tensor.py` & `blosc2-2.2.5/tests/test_tensor.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         (1e6, "f8"),
         (1e6, "i1"),
     ],
 )
 def test_pack_array(size, dtype):
     nparray = np.arange(size, dtype=dtype)
     parray = blosc2.pack_array(nparray)
-    if not os.getenv("BTUNE_BALANCE"):
+    if not os.getenv("BTUNE_TRADEOFF"):
         assert len(parray) < nparray.size * nparray.itemsize
 
     a2 = blosc2.unpack_array(parray)
     assert np.array_equal(nparray, a2)
 
 
 @pytest.mark.parametrize(
@@ -44,26 +44,26 @@
         (1e6, np.int8),
         pytest.param(3e8, "int64", marks=pytest.mark.heavy),  # > 2 GB
     ],
 )
 def test_pack_array2(size, dtype):
     nparray = np.arange(size, dtype=dtype)
     parray = blosc2.pack_array2(nparray)
-    if not os.getenv("BTUNE_BALANCE"):
+    if not os.getenv("BTUNE_TRADEOFF"):
         assert len(parray) < nparray.size * nparray.itemsize
 
     a2 = blosc2.unpack_array2(parray)
     assert np.array_equal(nparray, a2)
 
 
 @pytest.mark.parametrize("size, dtype", [(100_000, "i4,i4"), (10_000, "i4,f8"), (3000, "i4,f4,S8")])
 def test_pack_array2_struct(size, dtype):
     nparray = np.fromiter(iter(range(size)), dtype="i4,f4,S8")
     parray = blosc2.pack_array2(nparray)
-    if not os.getenv("BTUNE_BALANCE"):
+    if not os.getenv("BTUNE_TRADEOFF"):
         assert len(parray) < nparray.size * nparray.itemsize
 
     a2 = blosc2.unpack_array2(parray)
     assert np.array_equal(nparray, a2)
 
 
 @pytest.mark.parametrize(
@@ -76,15 +76,15 @@
 )
 def test_pack_tensor_torch(size, dtype):
     torch = pytest.importorskip("torch")
     dtype = getattr(torch, dtype)
     tensor = torch.arange(size, dtype=dtype)
     cframe = blosc2.pack_tensor(tensor)
     atensor = np.asarray(tensor)
-    if not os.getenv("BTUNE_BALANCE"):
+    if not os.getenv("BTUNE_TRADEOFF"):
         assert len(cframe) < atensor.size * atensor.dtype.itemsize
 
     tensor2 = blosc2.unpack_tensor(cframe)
     assert np.array_equal(atensor, np.asarray(tensor2))
 
 
 @pytest.mark.parametrize(
@@ -97,15 +97,15 @@
 )
 def test_pack_tensor_tensorflow(size, dtype):
     tensorflow = pytest.importorskip("tensorflow")
     array = np.arange(size, dtype=dtype)
     tensor = tensorflow.constant(array)
     cframe = blosc2.pack_tensor(tensor)
     atensor = np.asarray(tensor)
-    if not os.getenv("BTUNE_BALANCE"):
+    if not os.getenv("BTUNE_TRADEOFF"):
         assert len(cframe) < atensor.size * atensor.dtype.itemsize
 
     tensor2 = blosc2.unpack_tensor(cframe)
     assert np.array_equal(atensor, np.asarray(tensor2))
 
 
 @pytest.mark.parametrize(
@@ -117,15 +117,15 @@
         (1e6, np.int8),
         pytest.param(3e8, "int64", marks=pytest.mark.heavy),  # > 2 GB
     ],
 )
 def test_pack_tensor_array(size, dtype):
     nparray = np.arange(size, dtype=dtype)
     parray = blosc2.pack_tensor(nparray)
-    if not os.getenv("BTUNE_BALANCE"):
+    if not os.getenv("BTUNE_TRADEOFF"):
         assert len(parray) < nparray.size * nparray.itemsize
 
     a2 = blosc2.unpack_tensor(parray)
     assert np.array_equal(nparray, a2)
 
 
 ##### save / load  #####
@@ -137,15 +137,15 @@
         (1e6, "int64", "test.bl2"),
         (1e6, "float32", "test.bl2"),
     ],
 )
 def test_save_array(size, dtype, urlpath):
     nparray = np.arange(size, dtype=dtype)
     serial_size = blosc2.save_array(nparray, urlpath, mode="w")
-    if not os.getenv("BTUNE_BALANCE"):
+    if not os.getenv("BTUNE_TRADEOFF"):
         assert serial_size < nparray.size * nparray.itemsize
 
     a2 = blosc2.load_array(urlpath)
     blosc2.remove_urlpath(urlpath)
     assert np.array_equal(nparray, a2)
 
 
@@ -155,15 +155,15 @@
         (1e6, "int64", "test.bl2"),
         (1e6, "float32", "test.bl2"),
     ],
 )
 def test_save_tensor_array(size, dtype, urlpath):
     nparray = np.arange(size, dtype=dtype)
     serial_size = blosc2.save_tensor(nparray, urlpath, mode="w")
-    if not os.getenv("BTUNE_BALANCE"):
+    if not os.getenv("BTUNE_TRADEOFF"):
         assert serial_size < nparray.size * nparray.itemsize
 
     a2 = blosc2.load_tensor(urlpath)
     blosc2.remove_urlpath(urlpath)
     assert np.array_equal(nparray, a2)
 
 
@@ -175,15 +175,15 @@
     ],
 )
 def test_save_tensor_tensorflow(size, dtype, urlpath):
     tensorflow = pytest.importorskip("tensorflow")
     nparray = np.arange(size, dtype=dtype)
     tensor = tensorflow.constant(nparray)
     serial_size = blosc2.save_tensor(tensor, urlpath, mode="w")
-    if not os.getenv("BTUNE_BALANCE"):
+    if not os.getenv("BTUNE_TRADEOFF"):
         assert serial_size < nparray.size * nparray.itemsize
 
     tensor2 = blosc2.load_tensor(urlpath)
     blosc2.remove_urlpath(urlpath)
     assert np.array_equal(nparray, np.asarray(tensor2))
 
 
@@ -195,15 +195,15 @@
     ],
 )
 def test_save_tensor_torch(size, dtype, urlpath):
     torch = pytest.importorskip("torch")
     nparray = np.arange(size, dtype=dtype)
     tensor = torch.tensor(nparray)
     serial_size = blosc2.save_tensor(tensor, urlpath, mode="w")
-    if not os.getenv("BTUNE_BALANCE"):
+    if not os.getenv("BTUNE_TRADEOFF"):
         assert serial_size < nparray.size * nparray.itemsize
 
     tensor2 = blosc2.load_tensor(urlpath)
     blosc2.remove_urlpath(urlpath)
     assert np.array_equal(nparray, np.asarray(tensor2))
 
 
@@ -213,14 +213,14 @@
         (1e6, True, "test.bl2"),
         (1e6, False, "test.bl2"),
     ],
 )
 def test_save_tensor_sparse(size, sparse, urlpath):
     nparray = np.arange(size, dtype=np.int32)
     serial_size = blosc2.save_tensor(nparray, urlpath, mode="w", contiguous=not sparse)
-    if not os.getenv("BTUNE_BALANCE"):
+    if not os.getenv("BTUNE_TRADEOFF"):
         assert serial_size < nparray.size * nparray.itemsize
 
     a2 = blosc2.load_tensor(urlpath)
     assert os.path.isdir(urlpath) == sparse
     blosc2.remove_urlpath(urlpath)
     assert np.array_equal(nparray, a2)
```

### Comparing `blosc2-2.2.4/tests/test_ucodecs.py` & `blosc2-2.2.5/tests/test_ucodecs.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/test_ufilters.py` & `blosc2-2.2.5/tests/test_ufilters.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.4/tests/test_vlmeta.py` & `blosc2-2.2.5/tests/test_vlmeta.py`

 * *Files identical despite different names*

