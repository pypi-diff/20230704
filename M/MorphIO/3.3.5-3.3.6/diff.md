# Comparing `tmp/MorphIO-3.3.5.tar.gz` & `tmp/MorphIO-3.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MorphIO-3.3.5.tar", last modified: Wed Jun  7 10:42:54 2023, max compression
+gzip compressed data, was "dist/MorphIO-3.3.6.tar", last modified: Tue Jul  4 12:30:49 2023, max compression
```

## Comparing `MorphIO-3.3.5.tar` & `MorphIO-3.3.6.tar`

### file list

```diff
@@ -1,348 +1,348 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-07 10:42:35.000000 MorphIO-3.3.5/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-07 10:42:35.000000 MorphIO-3.3.5/.github/workflows/check-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-07 10:42:35.000000 MorphIO-3.3.5/.github/workflows/clang_format_check.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-07 10:42:35.000000 MorphIO-3.3.5/.github/workflows/coverage_test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-07 10:42:35.000000 MorphIO-3.3.5/.github/workflows/docstring_check.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-06-07 10:42:35.000000 MorphIO-3.3.5/.github/workflows/publish-sdist-wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-07 10:42:35.000000 MorphIO-3.3.5/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-07 10:42:35.000000 MorphIO-3.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-07 10:42:35.000000 MorphIO-3.3.5/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-07 10:42:35.000000 MorphIO-3.3.5/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-07 10:42:35.000000 MorphIO-3.3.5/3rdparty/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/cmake/gsl-lite-config-version.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/cmake/gsl-lite-config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/gsl-lite.natvis
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl/gsl
--rw-r--r--   0 runner    (1001) docker     (123)    15134 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl/gsl-lite-vc6.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl/gsl-lite.h
--rw-r--r--   0 runner    (1001) docker     (123)   188581 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl/gsl-lite.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl-lite/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl-lite/gsl-lite.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl.h
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/HighFive/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/HighFive/CMake/
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/CMake/HighFiveConfig.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/CMake/HighFiveTargetDeps.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/CMake/HighFiveTargetExport.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/HighFive/CMake/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/CMake/config/CompilerFlagsHelpers.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/CMake/config/ReleaseDebugAutoFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/CMake/config/TestHelpers.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)   114982 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/Doxyfile
--rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/DoxygenLayout.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/doxygen-awesome-css/
--rw-r--r--   0 runner    (1001) docker     (123)    63015 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/doxygen-awesome-css/doxygen-awesome.css
--rwxr-xr-x   0 runner    (1001) docker     (123)     1042 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/doxygen-awesome-css/update_doxygen_awesome.sh
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example1_hdf5.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example1_highfive.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example3.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example6.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example_boost.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example_boost_ublas.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example_easy_h5py.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example_easy_highfive.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example_eigen.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example_props.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/examples.js
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/godbolt.org.ico
--rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/doc/poster/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/HighFive/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Attribute.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5DataSet.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5DataSpace.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11803 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5DataType.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Easy.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Exception.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5File.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5FileDriver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Group.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Object.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16748 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5PropertyList.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Reference.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Selection.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Utility.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Version.hpp.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Attribute_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30878 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Converter_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5DataSet_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17089 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5DataType_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Dataspace_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Exception_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5FileDriver_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5File_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Friends.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Iterables_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Node_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15668 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Node_traits_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Object_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Path_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Path_traits_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17579 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5PropertyList_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5ReadWrite_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Reference_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Selection_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12595 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Slice_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Slice_traits_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5_definitions.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_Eigen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_opencv.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_public.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_scalar.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_vector.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-07 10:42:39.000000 MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_xtensor.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-07 10:42:40.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-07 10:42:40.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-07 10:42:40.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/cmake/GhcHelper.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-07 10:42:40.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/cmake/config.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/include/ghc/
--rw-r--r--   0 runner    (1001) docker     (123)   192164 2023-06-07 10:42:40.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/include/ghc/filesystem.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-07 10:42:40.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/include/ghc/fs_fwd.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-07 10:42:40.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/include/ghc/fs_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-07 10:42:40.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/include/ghc/fs_std.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-07 10:42:40.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/include/ghc/fs_std_fwd.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-07 10:42:40.000000 MorphIO-3.3.5/3rdparty/ghc_filesystem/include/ghc/fs_std_impl.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/lexertl14/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/char_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/debug.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/dot.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/enums.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    34590 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/generate_cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30752 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/generator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/internals.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/iterator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/licence_1_0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16457 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/lookup.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/match_results.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/memory_file.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/narrow.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/observer_ptr.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/
--rw-r--r--   0 runner    (1001) docker     (123)    37446 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/parser.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/
--rw-r--r--   0 runner    (1001) docker     (123)    32275 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/blocks.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    39423 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold4.inc
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_token.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    29156 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    51193 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_state.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    28271 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/scripts.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23049 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/table.inc
--rw-r--r--   0 runner    (1001) docker     (123)    46160 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/unicode.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/end_node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/iteration_node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/leaf_node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/selection_node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/sequence_node.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/partition/charset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/partition/equivset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    34712 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/rules.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/runtime_error.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/serialise.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/sm_to_csm.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/sm_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/state_machine.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/stream_shared_iterator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/string_token.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15071 2023-06-07 10:42:41.000000 MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/utf_iterators.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-07 10:42:35.000000 MorphIO-3.3.5/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-07 10:42:35.000000 MorphIO-3.3.5/CHANGELOG.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/CMake/
--rw-r--r--   0 runner    (1001) docker     (123)    11773 2023-06-07 10:42:35.000000 MorphIO-3.3.5/CMake/CodeCoverage.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-07 10:42:35.000000 MorphIO-3.3.5/CMake/CompilerFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-07 10:42:35.000000 MorphIO-3.3.5/CMake/MorphIOConfig.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-07 10:42:35.000000 MorphIO-3.3.5/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-07 10:42:35.000000 MorphIO-3.3.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-07 10:42:35.000000 MorphIO-3.3.5/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-07 10:42:35.000000 MorphIO-3.3.5/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-07 10:42:35.000000 MorphIO-3.3.5/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/MorphIO.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-07 10:42:53.000000 MorphIO-3.3.5/MorphIO.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-06-07 10:42:54.000000 MorphIO-3.3.5/MorphIO.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 10:42:53.000000 MorphIO-3.3.5/MorphIO.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 10:42:53.000000 MorphIO-3.3.5/MorphIO.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-07 10:42:53.000000 MorphIO-3.3.5/MorphIO.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 10:42:53.000000 MorphIO-3.3.5/MorphIO.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-07 10:42:54.000000 MorphIO-3.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-06-07 10:42:35.000000 MorphIO-3.3.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/binds/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/binds/python/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/bind_enums.h
--rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/bind_immutable.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/bind_immutable.h
--rw-r--r--   0 runner    (1001) docker     (123)    20865 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/bind_misc.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/bind_misc.h
--rw-r--r--   0 runner    (1001) docker     (123)    30892 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/bind_mutable.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/bind_mutable.h
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/bind_vasculature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/bind_vasculature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/bindings_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/bindings_utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/binds/python/generated/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/generated/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)    73608 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/generated/docstrings.h
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-07 10:42:35.000000 MorphIO-3.3.5/binds/python/morphio.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/binds/python/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/binds/python/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23979 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    65705 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28337 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    49082 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    24008 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    42266 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (123)    31971 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    79251 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   126295 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    90338 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    14556 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    27013 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/binds/python/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-06-07 10:42:41.000000 MorphIO-3.3.5/binds/python/pybind11/tools/pybind11Tools.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/include/morphio/
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/collection.h
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/dendritic_spine.h
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/endoplasmic_reticulum.h
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/enums.h
--rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/errorMessages.h
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/exceptions.h
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/glial_cell.h
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mito_section.h
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mitochondria.h
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/morphology.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/include/morphio/mut/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mut/dendritic_spine.h
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mut/endoplasmic_reticulum.h
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mut/glial_cell.h
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mut/mito_section.h
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mut/mitochondria.h
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mut/modifiers.h
--rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mut/morphology.h
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mut/section.h
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mut/soma.h
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/mut/writers.h
--rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/properties.h
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/section.h
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/section_base.h
--rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/section_iterators.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/soma.h
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/tools.h
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/types.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/include/morphio/vasc/
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/vasc/iterators.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/vasc/properties.h
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/vasc/section.h
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/vasc/vasculature.h
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/vector_types.h
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-07 10:42:35.000000 MorphIO-3.3.5/include/morphio/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/morphio/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-07 10:42:35.000000 MorphIO-3.3.5/morphio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/morphio/mut/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-07 10:42:35.000000 MorphIO-3.3.5/morphio/mut/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/morphio/vasculature/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-07 10:42:35.000000 MorphIO-3.3.5/morphio/vasculature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-07 10:42:35.000000 MorphIO-3.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 10:42:54.000000 MorphIO-3.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-07 10:42:35.000000 MorphIO-3.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14940 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/collection.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/dendritic_spine.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/endoplasmic_reticulum.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/enums.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/errorMessages.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/glial_cell.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mito_section.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mitochondria.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/morphology.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/src/mut/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mut/dendritic_spine.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mut/endoplasmic_reticulum.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mut/glial_cell.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mut/mito_section.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mut/mitochondria.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mut/modifiers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14634 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mut/morphology.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mut/section.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mut/soma.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17226 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/mut/writers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/point_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/point_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/properties.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/src/readers/
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/readers/NeurolucidaLexer.inc
--rw-r--r--   0 runner    (1001) docker     (123)    14782 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/readers/morphologyASC.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/readers/morphologyASC.h
--rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/readers/morphologyHDF5.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/readers/morphologyHDF5.h
--rw-r--r--   0 runner    (1001) docker     (123)    15036 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/readers/morphologySWC.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/readers/morphologySWC.h
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/readers/vasculatureHDF5.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/readers/vasculatureHDF5.h
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/section.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/shared_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/shared_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/soma.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:54.000000 MorphIO-3.3.5/src/vasc/
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/vasc/properties.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/vasc/section.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/vasc/vasculature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-07 10:42:35.000000 MorphIO-3.3.5/src/version.cpp.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-04 12:30:25.000000 MorphIO-3.3.6/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-04 12:30:25.000000 MorphIO-3.3.6/.github/workflows/check-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-04 12:30:25.000000 MorphIO-3.3.6/.github/workflows/clang_format_check.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-04 12:30:25.000000 MorphIO-3.3.6/.github/workflows/coverage_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-04 12:30:25.000000 MorphIO-3.3.6/.github/workflows/docstring_check.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-07-04 12:30:25.000000 MorphIO-3.3.6/.github/workflows/publish-sdist-wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-04 12:30:25.000000 MorphIO-3.3.6/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-04 12:30:25.000000 MorphIO-3.3.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-04 12:30:25.000000 MorphIO-3.3.6/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-04 12:30:25.000000 MorphIO-3.3.6/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 12:30:25.000000 MorphIO-3.3.6/3rdparty/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/GSL_LITE/
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-04 12:30:32.000000 MorphIO-3.3.6/3rdparty/GSL_LITE/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/GSL_LITE/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-04 12:30:32.000000 MorphIO-3.3.6/3rdparty/GSL_LITE/cmake/gsl-lite-config-version.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-04 12:30:32.000000 MorphIO-3.3.6/3rdparty/GSL_LITE/cmake/gsl-lite-config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-04 12:30:32.000000 MorphIO-3.3.6/3rdparty/GSL_LITE/gsl-lite.natvis
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/GSL_LITE/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/GSL_LITE/include/gsl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-04 12:30:32.000000 MorphIO-3.3.6/3rdparty/GSL_LITE/include/gsl/gsl
+-rw-r--r--   0 runner    (1001) docker     (123)    15134 2023-07-04 12:30:32.000000 MorphIO-3.3.6/3rdparty/GSL_LITE/include/gsl/gsl-lite-vc6.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-04 12:30:32.000000 MorphIO-3.3.6/3rdparty/GSL_LITE/include/gsl/gsl-lite.h
+-rw-r--r--   0 runner    (1001) docker     (123)   188581 2023-07-04 12:30:32.000000 MorphIO-3.3.6/3rdparty/GSL_LITE/include/gsl/gsl-lite.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/GSL_LITE/include/gsl-lite/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-04 12:30:32.000000 MorphIO-3.3.6/3rdparty/GSL_LITE/include/gsl-lite/gsl-lite.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-04 12:30:32.000000 MorphIO-3.3.6/3rdparty/GSL_LITE/include/gsl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-04 12:30:32.000000 MorphIO-3.3.6/3rdparty/GSL_LITE/include/gsl.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/HighFive/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/HighFive/CMake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/CMake/HighFiveConfig.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/CMake/HighFiveTargetDeps.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/CMake/HighFiveTargetExport.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/HighFive/CMake/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/CMake/config/CompilerFlagsHelpers.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/CMake/config/ReleaseDebugAutoFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/CMake/config/TestHelpers.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/HighFive/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/doc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   114912 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/doc/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/doc/DoxygenLayout.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/HighFive/doc/doxygen-awesome-css/
+-rw-r--r--   0 runner    (1001) docker     (123)    63015 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/doc/doxygen-awesome-css/doxygen-awesome.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1042 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/doc/doxygen-awesome-css/update_doxygen_awesome.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/doc/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/HighFive/doc/poster/
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/doc/poster/example1_hdf5.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/doc/poster/example1_highfive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/doc/poster/example3.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/doc/poster/example6.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/doc/poster/example_boost.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/doc/poster/example_boost_ublas.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/doc/poster/example_easy_h5py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/doc/poster/example_easy_highfive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/doc/poster/example_eigen.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/doc/poster/example_props.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/doc/poster/examples.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/doc/poster/godbolt.org.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/doc/poster/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/HighFive/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5Attribute.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5DataSet.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5DataSpace.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11803 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5DataType.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5Easy.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5Exception.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5File.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5FileDriver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5Group.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5Object.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16748 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5PropertyList.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5Reference.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5Selection.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5Utility.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5Version.hpp.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Attribute_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30878 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Converter_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5DataSet_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5DataType_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Dataspace_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Exception_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5FileDriver_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5File_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Friends.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Iterables_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Node_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15668 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Node_traits_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Object_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Path_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Path_traits_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17579 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5PropertyList_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5ReadWrite_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Reference_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Selection_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Slice_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Slice_traits_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5_definitions.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/h5easy_bits/
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_Eigen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_opencv.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_public.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_scalar.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_vector.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-04 12:30:33.000000 MorphIO-3.3.6/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_xtensor.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/ghc_filesystem/
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-04 12:30:35.000000 MorphIO-3.3.6/3rdparty/ghc_filesystem/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-04 12:30:35.000000 MorphIO-3.3.6/3rdparty/ghc_filesystem/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/ghc_filesystem/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-04 12:30:35.000000 MorphIO-3.3.6/3rdparty/ghc_filesystem/cmake/GhcHelper.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-04 12:30:35.000000 MorphIO-3.3.6/3rdparty/ghc_filesystem/cmake/config.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/ghc_filesystem/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/ghc_filesystem/include/ghc/
+-rw-r--r--   0 runner    (1001) docker     (123)   192164 2023-07-04 12:30:35.000000 MorphIO-3.3.6/3rdparty/ghc_filesystem/include/ghc/filesystem.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-04 12:30:35.000000 MorphIO-3.3.6/3rdparty/ghc_filesystem/include/ghc/fs_fwd.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-04 12:30:35.000000 MorphIO-3.3.6/3rdparty/ghc_filesystem/include/ghc/fs_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-04 12:30:35.000000 MorphIO-3.3.6/3rdparty/ghc_filesystem/include/ghc/fs_std.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-04 12:30:35.000000 MorphIO-3.3.6/3rdparty/ghc_filesystem/include/ghc/fs_std_fwd.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-04 12:30:35.000000 MorphIO-3.3.6/3rdparty/ghc_filesystem/include/ghc/fs_std_impl.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/lexertl14/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/char_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/debug.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/dot.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/enums.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    34590 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/generate_cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30752 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/generator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/internals.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/licence_1_0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16457 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/lookup.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/match_results.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/memory_file.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/narrow.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/observer_ptr.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)    37446 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/parser.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tokeniser/
+-rw-r--r--   0 runner    (1001) docker     (123)    32275 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tokeniser/blocks.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    39423 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold4.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_token.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    29156 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    51193 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_state.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28271 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tokeniser/scripts.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23049 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tokeniser/table.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    46160 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tokeniser/unicode.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tree/end_node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tree/iteration_node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tree/leaf_node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tree/node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tree/selection_node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tree/sequence_node.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/partition/charset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/partition/equivset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    34712 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/rules.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/runtime_error.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/serialise.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/sm_to_csm.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/sm_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/state_machine.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/stream_shared_iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/string_token.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15071 2023-07-04 12:30:36.000000 MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/utf_iterators.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-04 12:30:25.000000 MorphIO-3.3.6/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-04 12:30:25.000000 MorphIO-3.3.6/CHANGELOG.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/CMake/
+-rw-r--r--   0 runner    (1001) docker     (123)    31017 2023-07-04 12:30:25.000000 MorphIO-3.3.6/CMake/CodeCoverage.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-04 12:30:25.000000 MorphIO-3.3.6/CMake/CompilerFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-04 12:30:25.000000 MorphIO-3.3.6/CMake/MorphIOConfig.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-04 12:30:25.000000 MorphIO-3.3.6/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-04 12:30:25.000000 MorphIO-3.3.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-04 12:30:25.000000 MorphIO-3.3.6/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-04 12:30:25.000000 MorphIO-3.3.6/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-04 12:30:25.000000 MorphIO-3.3.6/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/MorphIO.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-04 12:30:48.000000 MorphIO-3.3.6/MorphIO.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-04 12:30:49.000000 MorphIO-3.3.6/MorphIO.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 12:30:48.000000 MorphIO-3.3.6/MorphIO.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 12:30:48.000000 MorphIO-3.3.6/MorphIO.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-04 12:30:48.000000 MorphIO-3.3.6/MorphIO.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 12:30:48.000000 MorphIO-3.3.6/MorphIO.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-04 12:30:49.000000 MorphIO-3.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-04 12:30:25.000000 MorphIO-3.3.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/binds/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/binds/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-04 12:30:25.000000 MorphIO-3.3.6/binds/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-07-04 12:30:25.000000 MorphIO-3.3.6/binds/python/bind_enums.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-04 12:30:25.000000 MorphIO-3.3.6/binds/python/bind_enums.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19507 2023-07-04 12:30:25.000000 MorphIO-3.3.6/binds/python/bind_immutable.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-04 12:30:25.000000 MorphIO-3.3.6/binds/python/bind_immutable.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14769 2023-07-04 12:30:25.000000 MorphIO-3.3.6/binds/python/bind_misc.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-04 12:30:25.000000 MorphIO-3.3.6/binds/python/bind_misc.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25809 2023-07-04 12:30:25.000000 MorphIO-3.3.6/binds/python/bind_mutable.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-04 12:30:25.000000 MorphIO-3.3.6/binds/python/bind_mutable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-07-04 12:30:25.000000 MorphIO-3.3.6/binds/python/bind_vasculature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-04 12:30:25.000000 MorphIO-3.3.6/binds/python/bind_vasculature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-04 12:30:25.000000 MorphIO-3.3.6/binds/python/bindings_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-04 12:30:25.000000 MorphIO-3.3.6/binds/python/bindings_utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/binds/python/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 12:30:25.000000 MorphIO-3.3.6/binds/python/generated/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)    85826 2023-07-04 12:30:25.000000 MorphIO-3.3.6/binds/python/generated/docstrings.h
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-04 12:30:25.000000 MorphIO-3.3.6/binds/python/morphio.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/binds/python/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/binds/python/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23979 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    65705 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28337 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    49082 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24008 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    42266 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31971 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    79251 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   126295 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    90338 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14556 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27013 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/binds/python/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-07-04 12:30:37.000000 MorphIO-3.3.6/binds/python/pybind11/tools/pybind11Tools.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/include/morphio/
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/collection.h
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/dendritic_spine.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/endoplasmic_reticulum.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/enums.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/errorMessages.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/glial_cell.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/mito_section.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/mitochondria.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/morphology.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/include/morphio/mut/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/mut/dendritic_spine.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/mut/endoplasmic_reticulum.h
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/mut/glial_cell.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/mut/mito_section.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/mut/mitochondria.h
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/mut/modifiers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/mut/morphology.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/mut/section.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/mut/soma.h
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/mut/writers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/properties.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/section.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/section_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/section_iterators.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/soma.h
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/tools.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/types.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/include/morphio/vasc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/vasc/iterators.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/vasc/properties.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/vasc/section.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/vasc/vasculature.h
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/vector_types.h
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 12:30:25.000000 MorphIO-3.3.6/include/morphio/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/morphio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-04 12:30:25.000000 MorphIO-3.3.6/morphio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/morphio/mut/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-04 12:30:25.000000 MorphIO-3.3.6/morphio/mut/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/morphio/vasculature/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-04 12:30:25.000000 MorphIO-3.3.6/morphio/vasculature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-04 12:30:25.000000 MorphIO-3.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 12:30:49.000000 MorphIO-3.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-04 12:30:25.000000 MorphIO-3.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14940 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/collection.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/dendritic_spine.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/endoplasmic_reticulum.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/enums.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17273 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/errorMessages.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/glial_cell.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/mito_section.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/mitochondria.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/morphology.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/src/mut/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/mut/dendritic_spine.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/mut/endoplasmic_reticulum.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/mut/glial_cell.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/mut/mito_section.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/mut/mitochondria.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/mut/modifiers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/mut/morphology.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/mut/section.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/mut/soma.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18554 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/mut/writers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/point_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/point_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/properties.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/src/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/readers/NeurolucidaLexer.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    14782 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/readers/morphologyASC.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/readers/morphologyASC.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/readers/morphologyHDF5.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/readers/morphologyHDF5.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/readers/morphologySWC.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/readers/morphologySWC.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/readers/vasculatureHDF5.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/readers/vasculatureHDF5.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/section.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/shared_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/shared_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/soma.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:30:49.000000 MorphIO-3.3.6/src/vasc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/vasc/properties.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/vasc/section.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/vasc/vasculature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-04 12:30:25.000000 MorphIO-3.3.6/src/version.cpp.in
```

### Comparing `MorphIO-3.3.5/.clang-format` & `MorphIO-3.3.6/.clang-format`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/.github/workflows/check-sdist.yml` & `MorphIO-3.3.6/.github/workflows/check-sdist.yml`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/.github/workflows/clang_format_check.yaml` & `MorphIO-3.3.6/.github/workflows/clang_format_check.yaml`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/.github/workflows/coverage_test.yaml` & `MorphIO-3.3.6/.github/workflows/coverage_test.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -24,8 +24,8 @@
         run: sudo apt-get update && sudo apt-get install build-essential libhdf5-dev lcov
       - name: Build and run unittests
         run: ci/coverage_test.sh
       - name: Upload Coverage to Coveralls
         uses: coverallsapp/github-action@master
         with:
           github-token: ${{ secrets.GITHUB_TOKEN }}
-          path-to-lcov: build/build-coverage/coverage.info.cleaned
+          path-to-lcov: build/build-coverage/coverage.info
```

### Comparing `MorphIO-3.3.5/.github/workflows/docstring_check.yaml` & `MorphIO-3.3.6/.github/workflows/docstring_check.yaml`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/.github/workflows/publish-sdist-wheels.yml` & `MorphIO-3.3.6/.github/workflows/publish-sdist-wheels.yml`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/.github/workflows/run-tests.yml` & `MorphIO-3.3.6/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/.gitmodules` & `MorphIO-3.3.6/.gitmodules`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/.readthedocs.yaml` & `MorphIO-3.3.6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/CMakeLists.txt` & `MorphIO-3.3.6/3rdparty/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/GSL_LITE/CMakeLists.txt` & `MorphIO-3.3.6/3rdparty/GSL_LITE/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/GSL_LITE/cmake/gsl-lite-config-version.cmake.in` & `MorphIO-3.3.6/3rdparty/GSL_LITE/cmake/gsl-lite-config-version.cmake.in`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/GSL_LITE/gsl-lite.natvis` & `MorphIO-3.3.6/3rdparty/GSL_LITE/gsl-lite.natvis`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl/gsl` & `MorphIO-3.3.6/3rdparty/GSL_LITE/include/gsl/gsl`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl/gsl-lite-vc6.hpp` & `MorphIO-3.3.6/3rdparty/GSL_LITE/include/gsl/gsl-lite-vc6.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl/gsl-lite.h` & `MorphIO-3.3.6/3rdparty/GSL_LITE/include/gsl/gsl-lite.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl/gsl-lite.hpp` & `MorphIO-3.3.6/3rdparty/GSL_LITE/include/gsl/gsl-lite.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl-lite/gsl-lite.hpp` & `MorphIO-3.3.6/3rdparty/GSL_LITE/include/gsl-lite/gsl-lite.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl.h` & `MorphIO-3.3.6/3rdparty/GSL_LITE/include/gsl.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/GSL_LITE/include/gsl.hpp` & `MorphIO-3.3.6/3rdparty/GSL_LITE/include/gsl.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/CMake/HighFiveConfig.cmake.in` & `MorphIO-3.3.6/3rdparty/HighFive/CMake/HighFiveConfig.cmake.in`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,14 @@
   endforeach()
 endfunction()
 
 if(TARGET HighFive)
     return()
 endif()
 
-@PACKAGE_INIT@
-
 # Get HighFive targets
 include("${CMAKE_CURRENT_LIST_DIR}/HighFiveTargets.cmake")
 
 # Recreate combined HighFive
 add_library(HighFive INTERFACE IMPORTED)
 set_property(TARGET HighFive APPEND PROPERTY INTERFACE_COMPILE_DEFINITIONS MPI_NO_CPPBIND)  # No c++ bindings
 
@@ -59,16 +57,12 @@
 set(HIGHFIVE_PARALLEL_HDF5 @HIGHFIVE_PARALLEL_HDF5@ CACHE BOOL "Enable Parallel HDF5 support")
 option(HIGHFIVE_VERBOSE "Enable verbose logging" @HIGHFIVE_VERBOSE@)
 
 if(HIGHFIVE_USE_XTENSOR AND NOT CMAKE_VERSION VERSION_LESS 3.8)
   set_property(TARGET HighFive APPEND PROPERTY INTERFACE_COMPILE_FEATURES cxx_std_14)
 endif()
 
-if(NOT HighFive_FIND_QUIETLY)
-  message(STATUS "HIGHFIVE @PROJECT_VERSION@: (Re)Detecting Highfive dependencies (HIGHFIVE_USE_INSTALL_DEPS=NO)")
-endif()
+message(STATUS "HIGHFIVE @PROJECT_VERSION@: (Re)Detecting Highfive dependencies (HIGHFIVE_USE_INSTALL_DEPS=NO)")
 include("${CMAKE_CURRENT_LIST_DIR}/HighFiveTargetDeps.cmake")
 foreach(dependency HighFive_libheaders libdeps)
     copy_interface_properties(HighFive ${dependency})
 endforeach()
-
-check_required_components(HighFive)
```

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/CMake/HighFiveTargetDeps.cmake` & `MorphIO-3.3.6/3rdparty/HighFive/CMake/HighFiveTargetDeps.cmake`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/CMake/HighFiveTargetExport.cmake` & `MorphIO-3.3.6/3rdparty/HighFive/CMake/HighFiveTargetExport.cmake`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/CMake/config/CompilerFlagsHelpers.cmake` & `MorphIO-3.3.6/3rdparty/HighFive/CMake/config/CompilerFlagsHelpers.cmake`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,17 @@
 		set(CMAKE_${COMPILER_LANGUAGE}_WARNING_ALL "-qformat=all -qinfo=lan:trx:ret:zea:cmp:ret")
 
 	## GCC, CLANG, rest of the world
 	elseif(CMAKE_${COMPILER_LANGUAGE}_COMPILER_ID MATCHES "Clang"
         OR CMAKE_${COMPILER_LANGUAGE}_COMPILER_ID MATCHES "GNU"
         OR CMAKE_${COMPILER_LANGUAGE}_COMPILER_ID MATCHES "Intel")
 		set(CMAKE_${COMPILER_LANGUAGE}_WARNING_ALL " -Wall -Wextra")
-		string(CONCAT CMAKE_${COMPILER_LANGUAGE}_WARNING_DEBUG " -Werror -Wshadow -Wnon-virtual-dtor -Wunused -Woverloaded-virtual -Wformat=2 -Wconversion -Wsign-conversion -Wno-error=deprecated-declarations"
+		string(CONCAT CMAKE_${COMPILER_LANGUAGE}_WARNING_DEBUG
+			" -Werror -Wshadow -Wnon-virtual-dtor -Wunused -Woverloaded-virtual"
+			" -Wformat=2 -Wconversion -Wsign-conversion -Wno-error=deprecated-declarations"
 		)
 		if(NOT CMAKE_${COMPILER_LANGUAGE}_COMPILER_IS_ICC)
 			string(CONCAT CMAKE_${COMPILER_LANGUAGE}_WARNING_DEBUG
 				${CMAKE_${COMPILER_LANGUAGE}_WARNING_DEBUG}
 				" -Wpedantic -Wcast-align -Wdouble-promotion"
 			)
 		endif()
```

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/CMake/config/ReleaseDebugAutoFlags.cmake` & `MorphIO-3.3.6/3rdparty/HighFive/CMake/config/ReleaseDebugAutoFlags.cmake`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/CMake/config/TestHelpers.cmake` & `MorphIO-3.3.6/3rdparty/HighFive/CMake/config/TestHelpers.cmake`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/CMakeLists.txt` & `MorphIO-3.3.6/3rdparty/HighFive/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
 
 # Preparing local building (tests, examples)
 # ------------------------------------------
 
 # Disable test if Boost was expressly disabled, or if HighFive is a sub-project
 if (NOT CMAKE_CURRENT_SOURCE_DIR STREQUAL CMAKE_SOURCE_DIR)
-  if(HIGHFIVE_UNIT_TESTS AND NOT HighFive_FIND_QUIETLY)
+  if(HIGHFIVE_UNIT_TESTS)
     message(WARNING "Unit tests have been DISABLED.")
   endif()
   set(HIGHFIVE_UNIT_TESTS FALSE)
 endif()
 
 if(HIGHFIVE_UNIT_TESTS)
   if(EXISTS ${CMAKE_CURRENT_LIST_DIR}/deps/catch2/CMakeLists.txt)
```

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/doc/Doxyfile` & `MorphIO-3.3.6/3rdparty/HighFive/doc/Doxyfile`

 * *Files 0% similar despite different names*

```diff
@@ -861,15 +861,14 @@
 # The INPUT tag is used to specify the files and/or directories that contain
 # documented source files. You may enter file names like myfile.cpp or
 # directories like /usr/src/myproject. Separate the files or directories with
 # spaces. See also FILE_PATTERNS and EXTENSION_MAPPING
 # Note: If this tag is empty the current directory is searched.
 
 INPUT                  = @CMAKE_CURRENT_SOURCE_DIR@/../include \
-                         @CMAKE_CURRENT_SOURCE_DIR@/installation.md \
                          @CMAKE_CURRENT_SOURCE_DIR@/../CHANGELOG.md \
                          @CMAKE_CURRENT_SOURCE_DIR@/../README.md
 
 # This tag can be used to specify the character encoding of the source files
 # that doxygen parses. Internally doxygen uses the UTF-8 encoding. Doxygen uses
 # libiconv (or the iconv built into libc) for the transcoding. See the libiconv
 # documentation (see:
```

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/doc/DoxygenLayout.xml` & `MorphIO-3.3.6/3rdparty/HighFive/doc/DoxygenLayout.xml`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/doc/doxygen-awesome-css/doxygen-awesome.css` & `MorphIO-3.3.6/3rdparty/HighFive/doc/doxygen-awesome-css/doxygen-awesome.css`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/doc/doxygen-awesome-css/update_doxygen_awesome.sh` & `MorphIO-3.3.6/3rdparty/HighFive/doc/doxygen-awesome-css/update_doxygen_awesome.sh`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example1_hdf5.cpp` & `MorphIO-3.3.6/3rdparty/HighFive/doc/poster/example1_hdf5.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example3.cpp` & `MorphIO-3.3.6/3rdparty/HighFive/doc/poster/example3.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example6.cpp` & `MorphIO-3.3.6/3rdparty/HighFive/doc/poster/example6.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example_boost.cpp` & `MorphIO-3.3.6/3rdparty/HighFive/doc/poster/example_boost.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example_boost_ublas.cpp` & `MorphIO-3.3.6/3rdparty/HighFive/doc/poster/example_boost_ublas.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example_easy_h5py.py` & `MorphIO-3.3.6/3rdparty/HighFive/doc/poster/example_easy_h5py.py`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example_easy_highfive.cpp` & `MorphIO-3.3.6/3rdparty/HighFive/doc/poster/example_easy_highfive.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example_eigen.cpp` & `MorphIO-3.3.6/3rdparty/HighFive/doc/poster/example_eigen.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/doc/poster/example_props.cpp` & `MorphIO-3.3.6/3rdparty/HighFive/doc/poster/example_props.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/doc/poster/examples.js` & `MorphIO-3.3.6/3rdparty/HighFive/doc/poster/examples.js`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/doc/poster/godbolt.org.ico` & `MorphIO-3.3.6/3rdparty/HighFive/doc/poster/godbolt.org.ico`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/doc/poster/index.html` & `MorphIO-3.3.6/3rdparty/HighFive/doc/poster/index.html`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Attribute.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5Attribute.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -83,49 +83,31 @@
     /// the attribute are different
     ///
     /// The array type can be a N-pointer or a N-vector ( e.g int** integer two
     /// dimensional array )
     template <typename T>
     void read(T& array) const;
 
-    /// \brief Read the attribute into a buffer.
-    ///
-    /// Note, this is the shallowest wrapper around `H5Aread`.
-    template <typename T>
-    void read(T* array, const DataType& mem_datatype) const;
-
     /// \brief Read the attribute into a buffer
-    ///
-    /// This overload deduces the memory datatype from `T`.
     template <typename T>
-    void read(T* array) const;
+    void read(T* array, const DataType& dtype = {}) const;
 
     ///
     /// Write the integrality N-dimension buffer to this attribute
     /// An exception is raised if the numbers of dimension of the buffer and of
     /// the attribute are different
     ///
     /// The array type can be a N-pointer or a N-vector ( e.g int** integer two
     /// dimensional array )
     template <typename T>
     void write(const T& buffer);
 
-    /// \brief Write to this attribute from `buffer`.
-    ///
-    /// Note that this is the shallowest wrapper around `H5Awrite`. It's useful
-    /// if you need full control. If possible prefer `Attribute::write`.
-    template <typename T>
-    void write_raw(const T* buffer, const DataType& mem_dtype);
-
-    /// \brief Write to this attribute from `buffer`.
-    ///
-    /// This version attempts to automatically deduce the datatype
-    /// of the buffer. Note, that the file datatype is already set.
+    /// \brief Write a buffer to this attribute
     template <typename T>
-    void write_raw(const T* buffer);
+    void write_raw(const T* buffer, const DataType& dtype = {});
 
     /// \brief Get the list of properties for creation of this attribute
     AttributeCreateProps getCreatePropertyList() const {
         return details::get_plist<AttributeCreateProps>(*this, H5Aget_create_plist);
     }
 
     // No empty attributes
```

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5DataSet.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5DataSet.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5DataSpace.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5DataSpace.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5DataType.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5DataType.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Easy.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5Easy.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Exception.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5Exception.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5File.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5File.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5FileDriver.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5FileDriver.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Group.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5Group.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Object.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5Object.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5PropertyList.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5PropertyList.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Reference.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5Reference.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Selection.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5Selection.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Utility.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5Utility.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/H5Version.hpp.in` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/H5Version.hpp.in`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits_misc.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits_misc.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Attribute_misc.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Attribute_misc.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -96,32 +96,28 @@
         // This one is deprecated since 1.12.0
         (void) H5Dvlen_reclaim(t.getId(), mem_space.getId(), H5P_DEFAULT, r.get_pointer());
 #endif
     }
 }
 
 template <typename T>
-inline void Attribute::read(T* array, const DataType& mem_datatype) const {
+inline void Attribute::read(T* array, const DataType& dtype) const {
     static_assert(!std::is_const<T>::value,
                   "read() requires a non-const structure to read data into");
+    using element_type = typename details::inspector<T>::base_type;
+    // Auto-detect mem datatype if not provided
+    const DataType& mem_datatype = dtype.empty() ? create_and_check_datatype<element_type>()
+                                                 : dtype;
 
     if (H5Aread(getId(), mem_datatype.getId(), static_cast<void*>(array)) < 0) {
         HDF5ErrMapper::ToException<AttributeException>("Error during HDF5 Read: ");
     }
 }
 
 template <typename T>
-inline void Attribute::read(T* array) const {
-    using element_type = typename details::inspector<T>::base_type;
-    const DataType& mem_datatype = create_and_check_datatype<element_type>();
-
-    read(array, mem_datatype);
-}
-
-template <typename T>
 inline void Attribute::write(const T& buffer) {
     const DataSpace& mem_space = getMemSpace();
 
     if (mem_space.getElementCount() == 0) {
         return;
     }
 
@@ -137,22 +133,17 @@
         throw DataSpaceException(ss.str());
     }
     auto w = details::data_converter::serialize<T>(buffer);
     write_raw(w.get_pointer(), buffer_info.data_type);
 }
 
 template <typename T>
-inline void Attribute::write_raw(const T* buffer, const DataType& mem_datatype) {
+inline void Attribute::write_raw(const T* buffer, const DataType& dtype) {
+    using element_type = typename details::inspector<T>::base_type;
+    const auto& mem_datatype = dtype.empty() ? create_and_check_datatype<element_type>() : dtype;
+
     if (H5Awrite(getId(), mem_datatype.getId(), buffer) < 0) {
         HDF5ErrMapper::ToException<DataSetException>("Error during HDF5 Write: ");
     }
 }
 
-template <typename T>
-inline void Attribute::write_raw(const T* buffer) {
-    using element_type = typename details::inspector<T>::base_type;
-    const auto& mem_datatype = create_and_check_datatype<element_type>();
-
-    write_raw(buffer, mem_datatype);
-}
-
 }  // namespace HighFive
```

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Converter_misc.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Converter_misc.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5DataSet_misc.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5DataSet_misc.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5DataType_misc.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5DataType_misc.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -22,72 +22,14 @@
 #include <half.hpp>
 #endif
 
 #include "H5Converter_misc.hpp"
 
 namespace HighFive {
 
-namespace detail {
-
-inline hid_t h5t_copy(hid_t original) {
-    auto copy = H5Tcopy(original);
-    if (copy == H5I_INVALID_HID) {
-        HDF5ErrMapper::ToException<DataTypeException>("Error copying datatype.");
-    }
-
-    return copy;
-}
-
-inline hsize_t h5t_get_size(hid_t hid) {
-    hsize_t size = H5Tget_size(hid);
-    if (size == 0) {
-        HDF5ErrMapper::ToException<DataTypeException>("Error getting size of datatype.");
-    }
-
-    return size;
-}
-
-inline H5T_cset_t h5t_get_cset(hid_t hid) {
-    auto cset = H5Tget_cset(hid);
-    if (cset == H5T_CSET_ERROR) {
-        HDF5ErrMapper::ToException<DataTypeException>("Error getting cset of datatype.");
-    }
-
-    return cset;
-}
-
-inline H5T_str_t h5t_get_strpad(hid_t hid) {
-    auto strpad = H5Tget_strpad(hid);
-    if (strpad == H5T_STR_ERROR) {
-        HDF5ErrMapper::ToException<DataTypeException>("Error getting strpad of datatype.");
-    }
-
-    return strpad;
-}
-
-inline void h5t_set_size(hid_t hid, hsize_t size) {
-    if (H5Tset_size(hid, size) < 0) {
-        HDF5ErrMapper::ToException<DataTypeException>("Error setting size of datatype.");
-    }
-}
-
-inline void h5t_set_cset(hid_t hid, H5T_cset_t cset) {
-    if (H5Tset_cset(hid, cset) < 0) {
-        HDF5ErrMapper::ToException<DataTypeException>("Error setting cset of datatype.");
-    }
-}
-
-inline void h5t_set_strpad(hid_t hid, H5T_str_t strpad) {
-    if (H5Tset_strpad(hid, strpad) < 0) {
-        HDF5ErrMapper::ToException<DataTypeException>("Error setting strpad of datatype.");
-    }
-}
-}  // namespace detail
-
-
 namespace {  // unnamed
 inline DataTypeClass convert_type_class(const H5T_class_t& tclass);
 inline std::string type_class_string(DataTypeClass);
 inline hid_t create_string(std::size_t length);
 }  // namespace
 
 inline bool DataType::empty() const noexcept {
@@ -95,15 +37,15 @@
 }
 
 inline DataTypeClass DataType::getClass() const {
     return convert_type_class(H5Tget_class(_hid));
 }
 
 inline size_t DataType::getSize() const {
-    return detail::h5t_get_size(_hid);
+    return H5Tget_size(_hid);
 }
 
 inline bool DataType::operator==(const DataType& other) const {
     return (H5Tequal(_hid, other._hid) > 0);
 }
 
 inline bool DataType::operator!=(const DataType& other) const {
@@ -129,113 +71,113 @@
 inline std::string DataType::string() const {
     return type_class_string(getClass()) + std::to_string(getSize() * 8);
 }
 
 // char mapping
 template <>
 inline AtomicType<char>::AtomicType() {
-    _hid = detail::h5t_copy(H5T_NATIVE_CHAR);
+    _hid = H5Tcopy(H5T_NATIVE_CHAR);
 }
 
 template <>
 inline AtomicType<signed char>::AtomicType() {
-    _hid = detail::h5t_copy(H5T_NATIVE_SCHAR);
+    _hid = H5Tcopy(H5T_NATIVE_SCHAR);
 }
 
 template <>
 inline AtomicType<unsigned char>::AtomicType() {
-    _hid = detail::h5t_copy(H5T_NATIVE_UCHAR);
+    _hid = H5Tcopy(H5T_NATIVE_UCHAR);
 }
 
 // short mapping
 template <>
 inline AtomicType<short>::AtomicType() {
-    _hid = detail::h5t_copy(H5T_NATIVE_SHORT);
+    _hid = H5Tcopy(H5T_NATIVE_SHORT);
 }
 
 template <>
 inline AtomicType<unsigned short>::AtomicType() {
-    _hid = detail::h5t_copy(H5T_NATIVE_USHORT);
+    _hid = H5Tcopy(H5T_NATIVE_USHORT);
 }
 
 // integer mapping
 template <>
 inline AtomicType<int>::AtomicType() {
-    _hid = detail::h5t_copy(H5T_NATIVE_INT);
+    _hid = H5Tcopy(H5T_NATIVE_INT);
 }
 
 template <>
 inline AtomicType<unsigned>::AtomicType() {
-    _hid = detail::h5t_copy(H5T_NATIVE_UINT);
+    _hid = H5Tcopy(H5T_NATIVE_UINT);
 }
 
 // long mapping
 template <>
 inline AtomicType<long>::AtomicType() {
-    _hid = detail::h5t_copy(H5T_NATIVE_LONG);
+    _hid = H5Tcopy(H5T_NATIVE_LONG);
 }
 
 template <>
 inline AtomicType<unsigned long>::AtomicType() {
-    _hid = detail::h5t_copy(H5T_NATIVE_ULONG);
+    _hid = H5Tcopy(H5T_NATIVE_ULONG);
 }
 
 // long long mapping
 template <>
 inline AtomicType<long long>::AtomicType() {
-    _hid = detail::h5t_copy(H5T_NATIVE_LLONG);
+    _hid = H5Tcopy(H5T_NATIVE_LLONG);
 }
 
 template <>
 inline AtomicType<unsigned long long>::AtomicType() {
-    _hid = detail::h5t_copy(H5T_NATIVE_ULLONG);
+    _hid = H5Tcopy(H5T_NATIVE_ULLONG);
 }
 
 // half-float, float, double and long double mapping
 #ifdef H5_USE_HALF_FLOAT
 using float16_t = half_float::half;
 
 template <>
 inline AtomicType<float16_t>::AtomicType() {
-    _hid = detail::h5t_copy(H5T_NATIVE_FLOAT);
+    _hid = H5Tcopy(H5T_NATIVE_FLOAT);
     // Sign position, exponent position, exponent size, mantissa position, mantissa size
     H5Tset_fields(_hid, 15, 10, 5, 0, 10);
     // Total datatype size (in bytes)
-    detail::h5t_set_size(_hid, 2);
+    H5Tset_size(_hid, 2);
     // Floating point exponent bias
     H5Tset_ebias(_hid, 15);
 }
 #endif
 
 template <>
 inline AtomicType<float>::AtomicType() {
-    _hid = detail::h5t_copy(H5T_NATIVE_FLOAT);
+    _hid = H5Tcopy(H5T_NATIVE_FLOAT);
 }
 
 template <>
 inline AtomicType<double>::AtomicType() {
-    _hid = detail::h5t_copy(H5T_NATIVE_DOUBLE);
+    _hid = H5Tcopy(H5T_NATIVE_DOUBLE);
 }
 
 template <>
 inline AtomicType<long double>::AtomicType() {
-    _hid = detail::h5t_copy(H5T_NATIVE_LDOUBLE);
+    _hid = H5Tcopy(H5T_NATIVE_LDOUBLE);
 }
 
 // std string
 template <>
 inline AtomicType<std::string>::AtomicType() {
     _hid = create_string(H5T_VARIABLE);
 }
 
 #if HIGHFIVE_CXX_STD >= 17
 // std byte
 template <>
 inline AtomicType<std::byte>::AtomicType() {
-    _hid = detail::h5t_copy(H5T_NATIVE_B8);
+    _hid = H5Tcopy(H5T_NATIVE_B8);
 }
 #endif
 
 // Fixed-Length strings
 // require class specialization templated for the char length
 template <size_t StrLen>
 class AtomicType<char[StrLen]>: public DataType {
@@ -325,15 +267,15 @@
     return std::string(datavec[i].data());
 }
 
 // Internal
 // Reference mapping
 template <>
 inline AtomicType<Reference>::AtomicType() {
-    _hid = detail::h5t_copy(H5T_STD_REF_OBJ);
+    _hid = H5Tcopy(H5T_STD_REF_OBJ);
 }
 
 inline size_t find_first_atomic_member_size(hid_t hid) {
     // Recursive exit condition
     if (H5Tget_class(hid) == H5T_COMPOUND) {
         auto number_of_members = H5Tget_nmembers(hid);
         if (number_of_members == -1) {
@@ -348,15 +290,15 @@
         auto member_type = H5Tget_member_type(hid, 0);
         auto size = find_first_atomic_member_size(member_type);
         H5Tclose(member_type);
         return size;
     } else if (H5Tget_class(hid) == H5T_STRING) {
         return 1;
     }
-    return detail::h5t_get_size(hid);
+    return H5Tget_size(hid);
 }
 
 // Calculate the padding required to align an element of a struct
 // For padding see explanation here: https://en.cppreference.com/w/cpp/language/object#Alignment
 // It is to compute padding following last element inserted inside a struct
 // 1) We want to push back an element padded to the structure
 // 'current_size' is the size of the structure before adding the new element.
@@ -379,15 +321,15 @@
 
 inline void CompoundType::create(size_t size) {
     if (size == 0) {
         size_t current_size = 0, max_atomic_size = 0;
 
         // Do a first pass to find the total size of the compound datatype
         for (auto& member: members) {
-            size_t member_size = detail::h5t_get_size(member.base_type.getId());
+            size_t member_size = H5Tget_size(member.base_type.getId());
 
             if (member_size == 0) {
                 throw DataTypeException("Cannot get size of DataType with hid: " +
                                         std::to_string(member.base_type.getId()));
             }
 
             size_t first_atomic_size = find_first_atomic_member_size(member.base_type.getId());
@@ -447,17 +389,20 @@
 inline void EnumType<T>::commit(const Object& object, const std::string& name) const {
     H5Tcommit2(object.getId(), name.c_str(), getId(), H5P_DEFAULT, H5P_DEFAULT, H5P_DEFAULT);
 }
 
 namespace {
 
 inline hid_t create_string(size_t length) {
-    hid_t _hid = detail::h5t_copy(H5T_C_S1);
-    detail::h5t_set_size(_hid, length);
-    detail::h5t_set_cset(_hid, H5T_CSET_UTF8);
+    hid_t _hid = H5Tcopy(H5T_C_S1);
+    if (H5Tset_size(_hid, length) < 0) {
+        HDF5ErrMapper::ToException<DataTypeException>("Unable to define datatype size to variable");
+    }
+    // define encoding to UTF-8 by default
+    H5Tset_cset(_hid, H5T_CSET_UTF8);
     return _hid;
 }
 
 
 inline DataTypeClass convert_type_class(const H5T_class_t& tclass) {
     switch (tclass) {
     case H5T_TIME:
```

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Dataspace_misc.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Dataspace_misc.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Exception_misc.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Exception_misc.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5FileDriver_misc.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5FileDriver_misc.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5File_misc.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5File_misc.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Iterables_misc.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Iterables_misc.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Node_traits.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Node_traits.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Node_traits_misc.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Node_traits_misc.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Object_misc.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Object_misc.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Path_traits.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Path_traits.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Path_traits_misc.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Path_traits_misc.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     }
     _file_obj.reset(new File(file_id));
 }
 
 template <typename Derivate>
 inline std::string PathTraits<Derivate>::getPath() const {
     return details::get_name([this](char* buffer, size_t length) {
-        return H5Iget_name(static_cast<const Derivate&>(*this).getId(), buffer, length);
+        return H5Iget_name(static_cast<const Derivate*>(this)->getId(), buffer, length);
     });
 }
 
 template <typename Derivate>
 inline File& PathTraits<Derivate>::getFile() const noexcept {
     return *_file_obj;
 }
```

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5PropertyList_misc.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5PropertyList_misc.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5ReadWrite_misc.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5ReadWrite_misc.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Reference_misc.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Reference_misc.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Selection_misc.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Selection_misc.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Slice_traits.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Slice_traits.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -255,23 +255,14 @@
     /// by taking the union of regular hyperslabs. An irregular hyperslab, in general, does not fit
     /// nicely into a multi-dimensional array, but only a subset of such an array.
     ///
     /// Therefore, the only memspaces supported for general hyperslabs are one-dimensional arrays.
     Selection select(const HyperSlab& hyperslab) const;
 
     ///
-    /// \brief Select an \p hyperslab in the current Slice/Dataset.
-    ///
-    /// If the selection can be read into a simple, multi-dimensional dataspace,
-    /// then this overload enable specifying the shape of the memory dataspace
-    /// with `memspace`. Note, that simple implies no offsets, strides or
-    /// number of blocks, just the size of the block in each dimension.
-    Selection select(const HyperSlab& hyperslab, const DataSpace& memspace) const;
-
-    ///
     /// \brief Select a region in the current Slice/Dataset of \p count points at
     /// \p offset separated by \p stride. If strides are not provided they will
     /// default to 1 in all dimensions.
     ///
     /// vector offset and count have to be from the same dimension
     ///
     Selection select(const std::vector<size_t>& offset,
@@ -313,63 +304,40 @@
     /// responsibility to ensure that the right amount of space has been
     /// allocated.
     /// \param array: A buffer containing enough space for the data
     /// \param dtype: The type of the data, in case it cannot be automatically guessed
     /// \param xfer_props: Data Transfer properties
     template <typename T>
     void read(T* array,
-              const DataType& dtype,
+              const DataType& dtype = DataType(),
               const DataTransferProps& xfer_props = DataTransferProps()) const;
 
     ///
-    /// Read the entire dataset into a raw buffer
-    ///
-    /// Same as `read(T*, const DataType&, const DataTransferProps&)`. However,
-    /// this overload deduces the HDF5 datatype of the element of `array` from
-    /// `T`. Note, that the file datatype is already fixed.
-    ///
-    /// \param array: A buffer containing enough space for the data
-    /// \param xfer_props: Data Transfer properties
-    template <typename T>
-    void read(T* array, const DataTransferProps& xfer_props = DataTransferProps()) const;
-
-    ///
     /// Write the integrality N-dimension buffer to this dataset
     /// An exception is raised is if the numbers of dimension of the buffer and
     /// of the dataset are different
     ///
     /// The array type can be a N-pointer or a N-vector ( e.g int** integer two
     /// dimensional array )
     template <typename T>
     void write(const T& buffer, const DataTransferProps& xfer_props = DataTransferProps());
 
     ///
-    /// Write from a raw pointer into this dataset.
+    /// Write from a raw buffer into this dataset
     ///
     /// No dimensionality checks will be performed, it is the user's
     /// responsibility to ensure that the buffer holds the right amount of
     /// elements. For n-dimensional matrices the buffer layout follows H5
     /// default conventions.
-    ///
-    /// Note, this is the shallowest wrapper around `H5Dwrite` and should
-    /// be used if full control is needed. Generally prefer `write`.
-    ///
     /// \param buffer: A buffer containing the data to be written
-    /// \param dtype: The datatype of `buffer`, i.e. the memory data type.
+    /// \param dtype: The type of the data, in case it cannot be automatically guessed
     /// \param xfer_props: The HDF5 data transfer properties, e.g. collective MPI-IO.
     template <typename T>
     void write_raw(const T* buffer,
-                   const DataType& mem_datatype,
+                   const DataType& dtype = DataType(),
                    const DataTransferProps& xfer_props = DataTransferProps());
 
-    ///
-    /// Write from a raw pointer into this dataset.
-    ///
-    /// Same as `write_raw(const T*, const DataTransferProps&)`. However, this
-    /// overload attempts to guess the data type of `buffer`, i.e. the memory
-    /// datatype. Note that the file datatype is already fixed.
-    ///
-    template <typename T>
-    void write_raw(const T* buffer, const DataTransferProps& xfer_props = DataTransferProps());
+  protected:
+    inline Selection select_impl(const HyperSlab& hyperslab, const DataSpace& memspace) const;
 };
 
 }  // namespace HighFive
```

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Slice_traits_misc.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Slice_traits_misc.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -60,16 +60,16 @@
 inline ElementSet::ElementSet(const std::vector<std::vector<std::size_t>>& element_ids) {
     for (const auto& vec: element_ids) {
         std::copy(vec.begin(), vec.end(), std::back_inserter(_ids));
     }
 }
 
 template <typename Derivate>
-inline Selection SliceTraits<Derivate>::select(const HyperSlab& hyperslab,
-                                               const DataSpace& memspace) const {
+inline Selection SliceTraits<Derivate>::select_impl(const HyperSlab& hyperslab,
+                                                    const DataSpace& memspace) const {
     // Note: The current limitation are that memspace must describe a
     //       packed memspace.
     //
     //       The reason for this is that we're unable to unpack general
     //       hyperslabs when the memory is not contiguous, e.g.
     //       `std::vector<std::vector<double>>`.
     const auto& slice = static_cast<const Derivate&>(*this);
@@ -94,15 +94,15 @@
 template <typename Derivate>
 inline Selection SliceTraits<Derivate>::select(const std::vector<size_t>& offset,
                                                const std::vector<size_t>& count,
                                                const std::vector<size_t>& stride,
                                                const std::vector<size_t>& block) const {
     auto slab = HyperSlab(RegularHyperSlab(offset, count, stride, block));
     auto memspace = DataSpace(count);
-    return select(slab, memspace);
+    return select_impl(slab, memspace);
 }
 
 template <typename Derivate>
 inline Selection SliceTraits<Derivate>::select(const std::vector<size_t>& columns) const {
     const auto& slice = static_cast<const Derivate&>(*this);
     const DataSpace& space = slice.getSpace();
     std::vector<size_t> dims = space.getDimensions();
@@ -117,15 +117,15 @@
         offsets.back() = column;
         slab |= RegularHyperSlab(offsets, counts);
     }
 
     std::vector<size_t> memdims = dims;
     memdims.back() = columns.size();
 
-    return select(slab, DataSpace(memdims));
+    return select_impl(slab, DataSpace(memdims));
 }
 
 template <typename Derivate>
 inline Selection SliceTraits<Derivate>::select(const ElementSet& elements) const {
     const auto& slice = static_cast<const Derivate&>(*this);
     const hsize_t* data = nullptr;
     const DataSpace space = slice.getSpace().clone();
@@ -210,40 +210,35 @@
     }
 }
 
 
 template <typename Derivate>
 template <typename T>
 inline void SliceTraits<Derivate>::read(T* array,
-                                        const DataType& mem_datatype,
+                                        const DataType& dtype,
                                         const DataTransferProps& xfer_props) const {
     static_assert(!std::is_const<T>::value,
                   "read() requires a non-const structure to read data into");
-
     const auto& slice = static_cast<const Derivate&>(*this);
+    using element_type = typename details::inspector<T>::base_type;
+
+    // Auto-detect mem datatype if not provided
+    const DataType& mem_datatype = dtype.empty() ? create_and_check_datatype<element_type>()
+                                                 : dtype;
 
     if (H5Dread(details::get_dataset(slice).getId(),
                 mem_datatype.getId(),
                 details::get_memspace_id(slice),
                 slice.getSpace().getId(),
                 xfer_props.getId(),
                 static_cast<void*>(array)) < 0) {
         HDF5ErrMapper::ToException<DataSetException>("Error during HDF5 Read.");
     }
 }
 
-template <typename Derivate>
-template <typename T>
-inline void SliceTraits<Derivate>::read(T* array, const DataTransferProps& xfer_props) const {
-    using element_type = typename details::inspector<T>::base_type;
-    const DataType& mem_datatype = create_and_check_datatype<element_type>();
-
-    read(array, mem_datatype, xfer_props);
-}
-
 
 template <typename Derivate>
 template <typename T>
 inline void SliceTraits<Derivate>::write(const T& buffer, const DataTransferProps& xfer_props) {
     const auto& slice = static_cast<const Derivate&>(*this);
     const DataSpace& mem_space = slice.getMemSpace();
 
@@ -267,32 +262,25 @@
     write_raw(w.get_pointer(), buffer_info.data_type, xfer_props);
 }
 
 
 template <typename Derivate>
 template <typename T>
 inline void SliceTraits<Derivate>::write_raw(const T* buffer,
-                                             const DataType& mem_datatype,
+                                             const DataType& dtype,
                                              const DataTransferProps& xfer_props) {
+    using element_type = typename details::inspector<T>::base_type;
     const auto& slice = static_cast<const Derivate&>(*this);
+    const auto& mem_datatype = dtype.empty() ? create_and_check_datatype<element_type>() : dtype;
 
     if (H5Dwrite(details::get_dataset(slice).getId(),
                  mem_datatype.getId(),
                  details::get_memspace_id(slice),
                  slice.getSpace().getId(),
                  xfer_props.getId(),
                  static_cast<const void*>(buffer)) < 0) {
         HDF5ErrMapper::ToException<DataSetException>("Error during HDF5 Write: ");
     }
 }
 
-template <typename Derivate>
-template <typename T>
-inline void SliceTraits<Derivate>::write_raw(const T* buffer, const DataTransferProps& xfer_props) {
-    using element_type = typename details::inspector<T>::base_type;
-    const auto& mem_datatype = create_and_check_datatype<element_type>();
-
-    write_raw(buffer, mem_datatype, xfer_props);
-}
-
 
 }  // namespace HighFive
```

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5Utils.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5Utils.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/bits/H5_definitions.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/bits/H5_definitions.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_Eigen.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_Eigen.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_misc.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_misc.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_opencv.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_opencv.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_public.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_public.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_scalar.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_scalar.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_vector.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_vector.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_xtensor.hpp` & `MorphIO-3.3.6/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_xtensor.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/ghc_filesystem/CMakeLists.txt` & `MorphIO-3.3.6/3rdparty/ghc_filesystem/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/ghc_filesystem/LICENSE` & `MorphIO-3.3.6/3rdparty/ghc_filesystem/LICENSE`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/ghc_filesystem/cmake/GhcHelper.cmake` & `MorphIO-3.3.6/3rdparty/ghc_filesystem/cmake/GhcHelper.cmake`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/ghc_filesystem/include/ghc/filesystem.hpp` & `MorphIO-3.3.6/3rdparty/ghc_filesystem/include/ghc/filesystem.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/ghc_filesystem/include/ghc/fs_fwd.hpp` & `MorphIO-3.3.6/3rdparty/ghc_filesystem/include/ghc/fs_fwd.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/ghc_filesystem/include/ghc/fs_impl.hpp` & `MorphIO-3.3.6/3rdparty/ghc_filesystem/include/ghc/fs_impl.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/ghc_filesystem/include/ghc/fs_std.hpp` & `MorphIO-3.3.6/3rdparty/ghc_filesystem/include/ghc/fs_std.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/ghc_filesystem/include/ghc/fs_std_fwd.hpp` & `MorphIO-3.3.6/3rdparty/ghc_filesystem/include/ghc/fs_std_fwd.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/ghc_filesystem/include/ghc/fs_std_impl.hpp` & `MorphIO-3.3.6/3rdparty/ghc_filesystem/include/ghc/fs_std_impl.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/CMakeLists.txt` & `MorphIO-3.3.6/3rdparty/lexertl14/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/char_traits.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/char_traits.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/debug.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/debug.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/dot.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/dot.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/enums.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/enums.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/generate_cpp.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/generate_cpp.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/generator.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/generator.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/internals.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/internals.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/iterator.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/iterator.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/licence_1_0.txt` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/licence_1_0.txt`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/lookup.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/lookup.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/match_results.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/match_results.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/memory_file.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/memory_file.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/narrow.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/narrow.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/parser.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/parser.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/blocks.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tokeniser/blocks.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold2.inc` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold2.inc`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold4.inc` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold4.inc`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_token.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_token.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_helper.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_helper.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_state.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_state.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/scripts.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tokeniser/scripts.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/table.inc` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tokeniser/table.inc`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tokeniser/unicode.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tokeniser/unicode.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/end_node.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tree/end_node.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/iteration_node.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tree/iteration_node.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/leaf_node.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tree/leaf_node.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/node.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tree/node.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/selection_node.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tree/selection_node.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/parser/tree/sequence_node.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/parser/tree/sequence_node.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/partition/charset.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/partition/charset.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/partition/equivset.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/partition/equivset.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/rules.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/rules.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/runtime_error.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/runtime_error.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/serialise.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/serialise.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/sm_to_csm.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/sm_to_csm.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/sm_traits.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/sm_traits.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/state_machine.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/state_machine.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/stream_shared_iterator.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/stream_shared_iterator.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/string_token.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/string_token.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/3rdparty/lexertl14/include/lexertl/utf_iterators.hpp` & `MorphIO-3.3.6/3rdparty/lexertl14/include/lexertl/utf_iterators.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/CHANGELOG.md` & `MorphIO-3.3.6/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+v3.3.6
+======
+Improvements:
+* don't allow negative IDs in SWC, except for the special parent == -1, for the first sample (#466)
+* Bump HighFive to v2.7.1 (#449)
+* Increase allowed section type to 19 (#462)
+* Have warnings for incompatible soma-types (#458):
+    * SWC files should have soma that are either a point, or a set of stacked cylinders.
+    * H5 & ASC consider the soma to be a contour
+    * allow assignment of soma type for mutable soma
+    * add errors for soma access / write if wrong size
+     - ERROR_SOMA_INVALID_SINGLE_POINT
+     - ERROR_SOMA_INVALID_THREE_POINT_CYLINDER
+     - ERROR_SOMA_INVALID_CONTOUR
+* increased test coverage and cleanup
+
 v3.3.5
 ======
 New Features:
 * Abstraction for morphology collection. (#444)
 
 Improvements:
 * Don't ignore choice of `MORPHIO_ENABLE_COVERAGE`. (#452)
```

### Comparing `MorphIO-3.3.5/CMake/CompilerFlags.cmake` & `MorphIO-3.3.6/CMake/CompilerFlags.cmake`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/CMakeLists.txt` & `MorphIO-3.3.6/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
   message("Floating Point Type: double")
 else()
   message("Floating Point Type: float")
 endif()
 
 set(CMAKE_MODULE_PATH ${PROJECT_SOURCE_DIR}/CMake)
 include(CompilerFlags)
+
 set(CMAKE_CXX_FLAGS "${FLAGS}")
 
 set(CMAKE_CXX_STANDARD 14)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 
 if (EXTERNAL_HIGHFIVE)
   find_package(HighFive REQUIRED)
```

### Comparing `MorphIO-3.3.5/CONTRIBUTING.md` & `MorphIO-3.3.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/COPYING` & `MorphIO-3.3.6/COPYING`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/COPYING.LESSER` & `MorphIO-3.3.6/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/MANIFEST.in` & `MorphIO-3.3.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/MorphIO.egg-info/PKG-INFO` & `MorphIO-3.3.6/MorphIO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MorphIO
-Version: 3.3.5
+Version: 3.3.6
 Summary: A neuron morphology IO library
 Home-page: https://github.com/BlueBrain/MorphIO/
 Author: Blue Brain Project, EPFL
 License: LGPLv3
 Description: .. image:: doc/source/logo/BBP-MorphIO.jpg
```

### Comparing `MorphIO-3.3.5/MorphIO.egg-info/SOURCES.txt` & `MorphIO-3.3.6/MorphIO.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 3rdparty/HighFive/CMake/config/CompilerFlagsHelpers.cmake
 3rdparty/HighFive/CMake/config/ReleaseDebugAutoFlags.cmake
 3rdparty/HighFive/CMake/config/TestHelpers.cmake
 3rdparty/HighFive/doc/CMakeLists.txt
 3rdparty/HighFive/doc/Doxyfile
 3rdparty/HighFive/doc/DoxygenLayout.xml
 3rdparty/HighFive/doc/environment.yaml
-3rdparty/HighFive/doc/installation.md
 3rdparty/HighFive/doc/doxygen-awesome-css/doxygen-awesome.css
 3rdparty/HighFive/doc/doxygen-awesome-css/update_doxygen_awesome.sh
 3rdparty/HighFive/doc/poster/example1_hdf5.cpp
 3rdparty/HighFive/doc/poster/example1_highfive.cpp
 3rdparty/HighFive/doc/poster/example3.cpp
 3rdparty/HighFive/doc/poster/example6.cpp
 3rdparty/HighFive/doc/poster/example_boost.cpp
@@ -163,14 +162,15 @@
 MorphIO.egg-info/PKG-INFO
 MorphIO.egg-info/SOURCES.txt
 MorphIO.egg-info/dependency_links.txt
 MorphIO.egg-info/not-zip-safe
 MorphIO.egg-info/requires.txt
 MorphIO.egg-info/top_level.txt
 binds/python/CMakeLists.txt
+binds/python/bind_enums.cpp
 binds/python/bind_enums.h
 binds/python/bind_immutable.cpp
 binds/python/bind_immutable.h
 binds/python/bind_misc.cpp
 binds/python/bind_misc.h
 binds/python/bind_mutable.cpp
 binds/python/bind_mutable.h
```

### Comparing `MorphIO-3.3.5/PKG-INFO` & `MorphIO-3.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MorphIO
-Version: 3.3.5
+Version: 3.3.6
 Summary: A neuron morphology IO library
 Home-page: https://github.com/BlueBrain/MorphIO/
 Author: Blue Brain Project, EPFL
 License: LGPLv3
 Description: .. image:: doc/source/logo/BBP-MorphIO.jpg
```

### Comparing `MorphIO-3.3.5/README.rst` & `MorphIO-3.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/bind_misc.cpp` & `MorphIO-3.3.6/binds/python/bind_immutable.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,409 +1,422 @@
-#include "bind_misc.h"
+#include "bind_immutable.h"
 
+#include <pybind11/iostream.h>  // py::add_ostream_redirect
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 
-#include <morphio/collection.h>
+#include <morphio/dendritic_spine.h>
+#include <morphio/endoplasmic_reticulum.h>
 #include <morphio/enums.h>
-#include <morphio/errorMessages.h>
+#include <morphio/glial_cell.h>
+#include <morphio/mut/dendritic_spine.h>
+#include <morphio/mut/endoplasmic_reticulum.h>
+#include <morphio/mut/glial_cell.h>
+#include <morphio/mut/mitochondria.h>
+#include <morphio/mut/morphology.h>
+#include <morphio/soma.h>
 #include <morphio/types.h>
-#include <morphio/version.h>
 
-#include "../../include/morphio/enums.h"
+#include <memory>  // std::make_unique
+
 #include "bind_enums.h"
+#include "bindings_utils.h"
+#include "generated/docstrings.h"
+
 
 namespace py = pybind11;
+using namespace py::literals;
+
+void bind_morphology(py::module& m);
+void bind_glialcell(py::module& m);
+void bind_mitochondria(py::module& m);
+void bind_mitosection(py::module& m);
+void bind_section(py::module& m);
+void bind_soma(py::module& m);
+void bind_endoplasmic_reticulum(py::module& m);
+void bind_dendritic_spine(py::module& m);
+
+void bind_immutable(py::module& m) {
+    // http://pybind11.readthedocs.io/en/stable/advanced/pycpp/utilities.html?highlight=iostream#capturing-standard-output-from-ostream
+    py::add_ostream_redirect(m, "ostream_redirect");
+    bind_morphology(m);
+    bind_glialcell(m);
+    bind_mitochondria(m);
+    bind_mitosection(m);
+    bind_section(m);
+    bind_soma(m);
+    bind_endoplasmic_reticulum(m);
+    bind_dendritic_spine(m);
+}
 
-void bind_misc(py::module& m) {
-    using namespace py::literals;
+void bind_morphology(py::module& m) {
+#define D(x) DOC(morphio, Morphology, x)
+    py::class_<morphio::Morphology>(m, "Morphology", DOC(morphio, Morphology))
+        .def(py::init<const std::string&, unsigned int>(),
+             "filename"_a,
+             "options"_a = morphio::enums::Option::NO_MODIFIER)
+        .def(py::init<const std::string&, const std::string&, unsigned int>(),
+             "filename"_a,
+             "extension"_a,
+             "options"_a = morphio::enums::Option::NO_MODIFIER)
+        .def(py::init<morphio::mut::Morphology&>())
+        .def(py::init([](py::object arg, unsigned int options) {
+                 return std::make_unique<morphio::Morphology>(py::str(arg), options);
+             }),
+             "filename"_a,
+             "options"_a = morphio::enums::Option::NO_MODIFIER,
+             "Additional Ctor that accepts as filename any python object that implements __repr__ "
+             "or __str__")
+        .def("as_mutable",
+             [](const morphio::Morphology* morph) { return morphio::mut::Morphology(*morph); })
+
+        // Cell sub-parts accessors
+        .def_property_readonly("soma", &morphio::Morphology::soma, D(soma))
+        .def_property_readonly("mitochondria", &morphio::Morphology::mitochondria, D(mitochondria))
+        .def_property_readonly("annotations", &morphio::Morphology::annotations, D(annotations))
+        .def_property_readonly("markers", &morphio::Morphology::markers, D(markers))
+        .def_property_readonly("endoplasmic_reticulum",
+                               &morphio::Morphology::endoplasmicReticulum,
+                               D(endoplasmicReticulum))
+        .def_property_readonly("root_sections", &morphio::Morphology::rootSections, D(rootSections))
+        .def_property_readonly("sections", &morphio::Morphology::sections, D(section))
+        .def("section", &morphio::Morphology::section, D(section), "section_id"_a)
 
-    m.def("set_maximum_warnings",
-          &morphio::set_maximum_warnings,
-          "Set the maximum number of warnings to be printed on screen\n"
-          "0 will print no warning\n"
-          "-1 will print them all");
-    m.def("set_raise_warnings", &morphio::set_raise_warnings, "Whether to raise warning as errors");
-    m.def("set_ignored_warning",
-          static_cast<void (*)(morphio::Warning, bool)>(&morphio::set_ignored_warning),
-          "Ignore/Unignore a specific warning message",
-          "warning"_a,
-          "ignore"_a = true);
-    m.def("set_ignored_warning",
-          static_cast<void (*)(const std::vector<morphio::Warning>&, bool)>(
-              &morphio::set_ignored_warning),
-          "Ignore/Unignore a list of warnings",
-          "warning"_a,
-          "ignore"_a = true);
-
-    py::enum_<morphio::enums::AnnotationType>(m, "AnnotationType", py::arithmetic())
-        .value("single_child",
-               morphio::enums::AnnotationType::SINGLE_CHILD,
-               "Indicates that a section has only one child");
-
-    py::enum_<IterType>(m, "IterType", py::arithmetic())
-        .value("depth_first", IterType::DEPTH_FIRST)
-        .value("breadth_first", IterType::BREADTH_FIRST)
-        .value("upstream", IterType::UPSTREAM)
-        .export_values();
-
-    py::enum_<morphio::enums::LogLevel>(m, "LogLevel")
-        .value("error", morphio::enums::LogLevel::ERROR)
-        .value("warning", morphio::enums::LogLevel::WARNING)
-        .value("info", morphio::enums::LogLevel::INFO)
-        .value("debug", morphio::enums::LogLevel::DEBUG);
-
-    py::enum_<morphio::enums::SectionType>(m, "SectionType", py::arithmetic())
-        .value("undefined", morphio::enums::SectionType::SECTION_UNDEFINED)
-        .value("soma", morphio::enums::SectionType::SECTION_SOMA)
-        .value("axon", morphio::enums::SectionType::SECTION_AXON)
-        .value("basal_dendrite", morphio::enums::SectionType::SECTION_DENDRITE)
-        .value("apical_dendrite", morphio::enums::SectionType::SECTION_APICAL_DENDRITE)
-        .value("custom5", morphio::enums::SectionType::SECTION_CUSTOM_5)
-        .value("custom6", morphio::enums::SectionType::SECTION_CUSTOM_6)
-        .value("custom7", morphio::enums::SectionType::SECTION_CUSTOM_7)
-        .value("custom8", morphio::enums::SectionType::SECTION_CUSTOM_8)
-        .value("custom9", morphio::enums::SectionType::SECTION_CUSTOM_9)
-        .value("custom10", morphio::enums::SectionType::SECTION_CUSTOM_10)
-        .value("glia_perivascular_process",
-               morphio::enums::SectionType::SECTION_GLIA_PERIVASCULAR_PROCESS)
-        .value("glia_process", morphio::enums::SectionType::SECTION_GLIA_PROCESS)
-        .value("spine_head", morphio::enums::SectionType::SECTION_SPINE_HEAD)
-        .value("spine_neck", morphio::enums::SectionType::SECTION_SPINE_NECK)
-        .value("all", morphio::enums::SectionType::SECTION_ALL)
-        .export_values();
-
-    py::enum_<morphio::enums::VascularSectionType>(m, "VasculatureSectionType", py::arithmetic())
-        .value("undefined", morphio::enums::VascularSectionType::SECTION_NOT_DEFINED)
-        .value("vein", morphio::enums::VascularSectionType::SECTION_VEIN)
-        .value("artery", morphio::enums::VascularSectionType::SECTION_ARTERY)
-        .value("venule", morphio::enums::VascularSectionType::SECTION_VENULE)
-        .value("arteriole", morphio::enums::VascularSectionType::SECTION_ARTERIOLE)
-        .value("venous_capillary", morphio::enums::VascularSectionType::SECTION_VENOUS_CAPILLARY)
-        .value("arterial_capillary",
-               morphio::enums::VascularSectionType::SECTION_ARTERIAL_CAPILLARY)
-        .value("transitional", morphio::enums::VascularSectionType::SECTION_TRANSITIONAL)
-        .export_values();
-
-    py::enum_<morphio::enums::Option>(m, "Option", py::arithmetic())
-        .value("no_modifier", morphio::enums::Option::NO_MODIFIER)
-        .value("two_points_sections", morphio::enums::Option::TWO_POINTS_SECTIONS)
-        .value("soma_sphere", morphio::enums::Option::SOMA_SPHERE)
-        .value("no_duplicates", morphio::enums::Option::NO_DUPLICATES)
-        .value("nrn_order", morphio::enums::Option::NRN_ORDER)
-        .export_values();
-
-
-    py::enum_<morphio::enums::CellFamily>(m, "CellFamily", py::arithmetic())
-        .value("NEURON", morphio::enums::CellFamily::NEURON)
-        .value("GLIA", morphio::enums::CellFamily::GLIA)
-        .value("SPINE", morphio::enums::CellFamily::SPINE)
-        .export_values();
-
-
-    py::enum_<morphio::enums::Warning>(m, "Warning")
-        .value("undefined", morphio::enums::Warning::UNDEFINED)
-        .value("mitochondria_write_not_supported",
-               morphio::enums::Warning::MITOCHONDRIA_WRITE_NOT_SUPPORTED)
-        .value("write_no_soma", morphio::enums::Warning::WRITE_NO_SOMA)
-        .value("write_empty_morphology", morphio::enums::Warning::WRITE_EMPTY_MORPHOLOGY)
-        .value("soma_non_conform", morphio::enums::SOMA_NON_CONFORM)
-        .value("no_soma_found", morphio::enums::Warning::NO_SOMA_FOUND)
-        .value("disconnected_neurite", morphio::enums::DISCONNECTED_NEURITE)
-        .value("wrong_duplicate", morphio::enums::WRONG_DUPLICATE)
-        .value("appending_empty_section", morphio::enums::APPENDING_EMPTY_SECTION)
-        .value("wrong_root_point", morphio::enums::Warning::WRONG_ROOT_POINT)
-        .value("only_child", morphio::enums::Warning::ONLY_CHILD)
-        .value("zero_diameter", morphio::enums::Warning::ZERO_DIAMETER);
-
-    py::enum_<morphio::enums::SomaType>(m, "SomaType", py::arithmetic())
-        .value("SOMA_UNDEFINED", morphio::enums::SomaType::SOMA_UNDEFINED)
-        .value("SOMA_SINGLE_POINT", morphio::enums::SomaType::SOMA_SINGLE_POINT)
-        .value("SOMA_NEUROMORPHO_THREE_POINT_CYLINDERS",
-               morphio::enums::SomaType::SOMA_NEUROMORPHO_THREE_POINT_CYLINDERS)
-        .value("SOMA_CYLINDERS", morphio::enums::SomaType::SOMA_CYLINDERS)
-        .value("SOMA_SIMPLE_CONTOUR", morphio::enums::SomaType::SOMA_SIMPLE_CONTOUR);
-
-    m.attr("version") = morphio::getVersionString();
-
-    auto base = py::register_exception<morphio::MorphioError&>(m, "MorphioError");
-    // base.ptr() signifies "inherits from"
-    auto raw = py::register_exception<morphio::RawDataError&>(m, "RawDataError", base.ptr());
-    py::register_exception<morphio::UnknownFileType&>(m, "UnknownFileType", base.ptr());
-    py::register_exception<morphio::SomaError&>(m, "SomaError", base.ptr());
-    py::register_exception<morphio::IDSequenceError&>(m, "IDSequenceError", raw.ptr());
-    py::register_exception<morphio::MultipleTrees&>(m, "MultipleTrees", raw.ptr());
-    py::register_exception<morphio::MissingParentError&>(m, "MissingParentError", raw.ptr());
-    py::register_exception<morphio::SectionBuilderError&>(m, "SectionBuilderError", raw.ptr());
-    py::register_exception<morphio::WriterError&>(m, "WriterError", base.ptr());
-
-
-    py::class_<morphio::Points>(m, "Points", py::buffer_protocol())
-        .def_buffer([](morphio::Points& points) -> py::buffer_info {
-            return py::buffer_info(points.data(),              /* Pointer to buffer */
-                                   sizeof(morphio::floatType), /* Size of one scalar */
-                                   py::format_descriptor<morphio::floatType>::format(), /* Python
-                                                                              struct-style format
-                                                                              descriptor */
-                                   2, /* Number of dimensions */
-                                   {static_cast<ssize_t>(points.size()),
-                                    static_cast<ssize_t>(3)},       /* Buffer dimensions */
-                                   {sizeof(morphio::floatType) * 3, /* Strides (in bytes) for each
-                                                                       index */
-                                    sizeof(morphio::floatType)});
-        });
-
-    py::class_<morphio::Property::Properties>(
-        m, "Properties", "The higher level container structure is Property::Properties")
-        .def_readwrite("point_level",
-                       &morphio::Property::Properties::_pointLevel,
-                       "Returns the structure that stores information at the point level")
-        .def_readwrite("section_level",
-                       &morphio::Property::Properties::_sectionLevel,
-                       "Returns the structure that stores information at the section level")
-        .def_readwrite("cell_level",
-                       &morphio::Property::Properties::_cellLevel,
-                       "Returns the structure that stores information at the cell level");
-
-
-    py::class_<morphio::Property::PointLevel>(m,
-                                              "PointLevel",
-                                              "Container class for information available at the "
-                                              "point level (point coordinate, diameter, perimeter)")
-        .def(py::init<>())
-        .def(py::init<std::vector<morphio::Property::Point::Type>,
-                      std::vector<morphio::Property::Diameter::Type>>(),
-             "points"_a,
-             "diameters"_a)
-        .def(py::init<std::vector<morphio::Property::Point::Type>,
-                      std::vector<morphio::Property::Diameter::Type>,
-                      std::vector<morphio::Property::Perimeter::Type>>(),
-             "points"_a,
-             "diameters"_a,
-             "perimeters"_a)
-        .def_readwrite("points",
-                       &morphio::Property::PointLevel::_points,
-                       "Returns the list of point coordinates")
-        .def_readwrite("perimeters",
-                       &morphio::Property::PointLevel::_perimeters,
-                       "Returns the list of perimeters")
-        .def_readwrite("diameters",
-                       &morphio::Property::PointLevel::_diameters,
-                       "Returns the list of diameters");
-
-    py::class_<morphio::Property::SectionLevel>(m,
-                                                "SectionLevel",
-                                                "Container class for information available at the "
-                                                "section level (section type, parent section)")
-        .def_readwrite("sections",
-                       &morphio::Property::SectionLevel::_sections,
-                       "Returns a list of [offset, parent section ID]")
-        .def_readwrite("section_types",
-                       &morphio::Property::SectionLevel::_sectionTypes,
-                       "Returns the list of section types")
-        .def_readwrite("children",
-                       &morphio::Property::SectionLevel::_children,
-                       "Returns a dictionary where key is a section ID "
-                       "and value is the list of children section IDs");
-
-    py::class_<morphio::Property::CellLevel>(m,
-                                             "CellLevel",
-                                             "Container class for information available at the "
-                                             "cell level (cell type, file version, soma type)")
-        .def_readwrite("cell_family",
-                       &morphio::Property::CellLevel::_cellFamily,
-                       "Returns the cell family (neuron or glia)")
-        .def_readwrite("soma_type",
-                       &morphio::Property::CellLevel::_somaType,
-                       "Returns the soma type")
-        .def_readwrite("version", &morphio::Property::CellLevel::_version, "Returns the version");
-
-    py::class_<morphio::Property::Annotation>(
-        m,
-        "Annotation",
-        "Container class for information about anomalies detected while parsing the file (no soma, "
-        "section with a single child...)")
-        .def_readwrite("type", &morphio::Property::Annotation::_type, "Returns the type")
-        .def_readwrite("section_id",
-                       &morphio::Property::Annotation::_sectionId,
-                       "Returns the sectionId")
-        .def_readwrite("line_number",
-                       &morphio::Property::Annotation::_lineNumber,
-                       "Returns the lineNumber")
-        .def_readwrite("details", &morphio::Property::Annotation::_details, "Returns the details")
+        // Property accessors
         .def_property_readonly(
             "points",
-            [](morphio::Property::Annotation* a) { return a->_points._points; },
-            "Returns the list of coordinates of annotated points")
+            [](morphio::Morphology* morpho) {
+                const auto& data = morpho->points();
+                return py::array(static_cast<py::ssize_t>(data.size()), data.data());
+            },
+            D(points))
+        .def_property_readonly(
+            "n_points",
+            [](const morphio::Morphology& obj) { return obj.points().size(); },
+            "Returns the number of points from all sections (soma points are not included)")
         .def_property_readonly(
             "diameters",
-            [](morphio::Property::Annotation* a) { return a->_points._diameters; },
-            "Returns the list of diameters of annotated points")
+            [](const morphio::Morphology& morpho) {
+                const auto& data = morpho.diameters();
+                return py::array(static_cast<py::ssize_t>(data.size()), data.data());
+            },
+            D(diameters))
         .def_property_readonly(
             "perimeters",
-            [](morphio::Property::Annotation* a) { return a->_points._perimeters; },
-            "Returns the list of perimeters of annotated points");
+            [](const morphio::Morphology& obj) {
+                const auto& data = obj.perimeters();
+                return py::array(static_cast<py::ssize_t>(data.size()), data.data());
+            },
+            D(perimeters))
+        .def_property_readonly(
+            "section_offsets",
+            [](const morphio::Morphology& morpho) { return as_pyarray(morpho.sectionOffsets()); },
+            D(sectionOffsets))
+        .def_property_readonly(
+            "section_types",
+            [](const morphio::Morphology& morph) {
+                const auto& data = morph.sectionTypes();
+                return py::array(static_cast<py::ssize_t>(data.size()), data.data());
+            },
+            D(sectionTypes))
+        .def_property_readonly("connectivity", &morphio::Morphology::connectivity, D(connectivity))
+        .def_property_readonly("soma_type", &morphio::Morphology::somaType, D(somaType))
+        .def_property_readonly("cell_family", &morphio::Morphology::cellFamily, D(cellFamily))
+        .def_property_readonly("version", &morphio::Morphology::version, D(version))
+
+        // Iterators
+        .def(
+            "iter",
+            [](morphio::Morphology* morpho, IterType type) {
+                switch (type) {
+                case IterType::DEPTH_FIRST:
+                    return py::make_iterator(morpho->depth_begin(), morpho->depth_end());
+                case IterType::BREADTH_FIRST:
+                    return py::make_iterator(morpho->breadth_begin(), morpho->breadth_end());
+                case IterType::UPSTREAM:
+                default:
+                    throw morphio::MorphioError(
+                        "Only iteration types depth_first and breadth_first are supported");
+                }
+            },
+            py::keep_alive<0, 1>() /* Essential: keep object alive while iterator exists */,
+            "Section iterator that runs successively on every neurite\n"
+            "\n"
+            "iter_type controls the order of iteration on sections of a given neurite. 2 values "
+            "can be passed:\n"
+            "\n"
+            "- ``morphio.IterType.depth_first`` (default)\n"
+            "- ``morphio.IterType.breadth_first``\n",
+            "iter_type"_a = IterType::DEPTH_FIRST);
+#undef D
+}
+
+void bind_glialcell(py::module& m) {
+    py::class_<morphio::GlialCell, morphio::Morphology>(m, "GlialCell", DOC(morphio, GlialCell))
+        .def(py::init<const std::string&>())
+        .def(py::init(
+                 [](py::object arg) { return std::make_unique<morphio::GlialCell>(py::str(arg)); }),
+             "filename"_a,
+             "Additional Ctor that accepts as filename any python object that implements __repr__ "
+             "or __str__");
+}
 
-    py::class_<morphio::Property::Marker>(m,
-                                          "Marker",
-                                          "Container class for NeuroLucida extra Markers ")
-        .def_property_readonly(
-            "label",
-            [](morphio::Property::Marker* marker) { return marker->_label; },
-            "Returns the label")
+void bind_mitochondria(py::module& m) {
+    py::class_<morphio::Mitochondria>(m, "Mitochondria", DOC(morphio, Mitochondria))
+        .def("section",
+             &morphio::Mitochondria::section,
+             DOC(morphio, Mitochondria, section),
+             "section_id"_a)
+        .def_property_readonly("sections",
+                               &morphio::Mitochondria::sections,
+                               DOC(morphio, Mitochondria, sections))
+        .def_property_readonly("root_sections",
+                               &morphio::Mitochondria::rootSections,
+                               DOC(morphio, Mitochondria, rootSections));
+}
+
+void bind_mitosection(py::module& m) {
+    using morphio::MitoSection;
+    py::class_<MitoSection>(m, "MitoSection", "Class representing a Mitochondrial Section")
+        // Topology-related member functions
+        .def_property_readonly("parent", &MitoSection::parent, DOC(morphio, SectionBase, parent))
+        .def_property_readonly("is_root", &MitoSection::isRoot, DOC(morphio, SectionBase, isRoot))
+        .def_property_readonly("children",
+                               &MitoSection::children,
+                               DOC(morphio, SectionBase, children))
+
+        // Property-related accesors
+        .def_property_readonly("id", &MitoSection::id, DOC(morphio, SectionBase, id))
         .def_property_readonly(
-            "points",
-            [](morphio::Property::Marker* marker) { return marker->_pointLevel._points; },
-            "Returns the list of coordinates of the marker points")
+            "neurite_section_ids",
+            [](MitoSection* section) { return span_to_ndarray(section->neuriteSectionIds()); },
+            DOC(morphio, MitoSection, neuriteSectionIds))
         .def_property_readonly(
             "diameters",
-            [](morphio::Property::Marker* marker) { return marker->_pointLevel._diameters; },
-            "Returns the list of diameters of the marker points")
+            [](MitoSection* section) { return span_to_ndarray(section->diameters()); },
+            DOC(morphio, MitoSection, diameters))
         .def_property_readonly(
-            "section_id",
-            [](morphio::Property::Marker* marker) { return marker->_sectionId; },
-            "Returns the id of section that contains the marker");
-
-    py::class_<morphio::Property::MitochondriaPointLevel>(
-        m,
-        "MitochondriaPointLevel",
-        "Container class for the information available at the mitochondrial point level (enclosing "
-        "neuronal section, relative distance to start of neuronal section, diameter)")
-        .def(py::init<>())
-        .def(py::init<std::vector<uint32_t>,
-                      std::vector<morphio::floatType>,
-                      std::vector<morphio::Property::Diameter::Type>>(),
-             "neuronal_section_ids"_a,
-             "distances_to_section_start"_a,
-             "diameters"_a);
-
-    py::class_<morphio::Property::DendriticSpine::PostSynapticDensity>(
-        m, "PostSynapticDensity", "DendriticSpine post-synaptic density")
-        .def(py::init<>())
-        .def(py::init<morphio::Property::DendriticSpine::SectionId_t,
-                      morphio::Property::DendriticSpine::SegmentId_t,
-                      morphio::Property::DendriticSpine::Offset_t>(),
-             "section_id"_a,
-             "segment_id"_a,
-             "offset"_a)
-        .def_readonly("section_id",
-                      &morphio::Property::DendriticSpine::PostSynapticDensity::sectionId,
-                      "Returns `sectionId` of post-synaptic density")
-        .def_readonly("segment_id",
-                      &morphio::Property::DendriticSpine::PostSynapticDensity::segmentId,
-                      "Returns `segmentId` of post-synaptic density")
-        .def_readonly("offset",
-                      &morphio::Property::DendriticSpine::PostSynapticDensity::offset,
-                      "Returns `offset` of post-synaptic density");
-
-    py::class_<morphio::Collection>(m, "Collection", "A collection of morphologies")
-        .def(py::init<std::string>(), "collection_path"_a)
-        .def(py::init([](py::object arg) { return morphio::Collection(py::str(arg)); }),
-             "collection_path"_a,
-             "Create a collection from a Path-like object.")
-        .def(py::init([](py::object arg, std::vector<std::string> extensions) {
-                 return morphio::Collection(py::str(arg), std::move(extensions));
-             }),
-             "collection_path"_a,
-             "extensions"_a,
-             "Create a collection from a Path-like object.")
+            "relative_path_lengths",
+            [](MitoSection* section) { return span_to_ndarray(section->relativePathLengths()); },
+            DOC(morphio, MitoSection, relativePathLengths))
+        .def("has_same_shape",
+             &MitoSection::hasSameShape,
+             DOC(morphio, MitoSection, relativePathLengths))
+
+        // Iterators
         .def(
-            "load",
-            [](morphio::Collection* collection,
-               const std::string& morph_name,
-               unsigned int options,
-               bool is_mutable) -> py::object {
-                if (is_mutable) {
-                    return py::cast(
-                        collection->load<morphio::mut::Morphology>(morph_name, options));
-                } else {
-                    return py::cast(collection->load<morphio::Morphology>(morph_name, options));
+            "iter",
+            [](MitoSection* section, IterType type) {
+                switch (type) {
+                case IterType::DEPTH_FIRST:
+                    return py::make_iterator(section->depth_begin(), section->depth_end());
+                case IterType::BREADTH_FIRST:
+                    return py::make_iterator(section->breadth_begin(), section->breadth_end());
+                case IterType::UPSTREAM:
+                    return py::make_iterator(section->upstream_begin(), section->upstream_end());
+                default:
+                    throw morphio::MorphioError(
+                        "Only iteration types depth_first, breadth_first and "
+                        "upstream are supported");
                 }
             },
-            "morph_name"_a,
-            "options"_a = morphio::enums::Option::NO_MODIFIER,
-            "mutable"_a = false,
-            "Load the morphology named 'morph_name' form the collection.")
+            py::keep_alive<0, 1>() /* Essential: keep object alive while iterator exists */,
+            "Depth first iterator starting at a given section id\n"
+            "\n"
+            "If id == -1, the iteration will be successively performed starting\n"
+            "at each root section",
+            "iter_type"_a = IterType::DEPTH_FIRST);
+}
+
+void bind_section(py::module& m) {
+#define D(x) DOC(morphio, Section, x)
+#define DB(x) DOC(morphio, SectionBase, x)
+    using morphio::Section;
+    py::class_<Section>(m, "Section", "Class representing a Section")
+        .def("__str__",
+             [](const Section& section) {
+                 std::stringstream ss;
+                 ss << section;
+                 return ss.str();
+             })
+        .def_property_readonly("parent", &Section::parent, DB(parent))
+        .def_property_readonly("is_root", &Section::isRoot, DB(isRoot))
+        .def_property_readonly("children", &Section::children, DB(children))
+        .def_property_readonly("id", &Section::id, DB(id))
+        .def_property_readonly("type", &Section::type, D(type))
+        .def_property_readonly(
+            "points",
+            [](Section* section) { return span_array_to_ndarray(section->points()); },
+            D(points))
+        .def_property_readonly(
+            "n_points",
+            [](const Section& section) { return section.points().size(); },
+            "Returns the number of points in section")
+        .def_property_readonly(
+            "diameters",
+            [](Section* section) { return span_to_ndarray(section->diameters()); },
+            D(diameters))
+        .def_property_readonly(
+            "perimeters",
+            [](Section* section) { return span_to_ndarray(section->perimeters()); },
+            D(perimeters))
+        .def("is_heterogeneous",
+             &Section::isHeterogeneous,
+             D(isHeterogeneous),
+             py::arg("downstream") = true)
+        .def("has_same_shape", &Section::hasSameShape, D(hasSameShape))
         .def(
-            "load_unordered",
-            [](morphio::Collection* collection,
-               std::vector<std::string> morphology_names,
-               unsigned int options,
-               bool is_mutable) -> py::object {
-                if (is_mutable) {
-                    return py::cast(
-                        collection->load_unordered<morphio::mut::Morphology>(morphology_names,
-                                                                             options));
-                } else {
-                    return py::cast(
-                        collection->load_unordered<morphio::Morphology>(morphology_names, options));
+            "iter",
+            [](Section* section, IterType type) {
+                switch (type) {
+                case IterType::DEPTH_FIRST:
+                    return py::make_iterator(section->depth_begin(), section->depth_end());
+                case IterType::BREADTH_FIRST:
+                    return py::make_iterator(section->breadth_begin(), section->breadth_end());
+                case IterType::UPSTREAM:
+                    return py::make_iterator(section->upstream_begin(), section->upstream_end());
+                default:
+                    throw morphio::MorphioError(
+                        "Only iteration types depth_first, breadth_first and "
+                        "upstream are supported");
                 }
             },
-            "morphology_names"_a,
-            "options"_a = morphio::enums::Option::NO_MODIFIER,
-            "mutable"_a = false,
-            R"(Create an iterable of loop index and morphology.
-
-When reading from containers, the order in which morphologies are read can
-have a large impact on the overall time to load those morphologies.
-
-This iterator provides means of reordering loops to optimize the access
-pattern. Loops such as the following
-
-    for k, morph_name in enumerate(morphology_names):
-        morph = collection.load(morphology_names[k])
-        f(k, morph)
-
-can be replaced with
-
-    for k, morph in collection.load_unordered(morphology_names):
-      assert collection.load(morphology_names[k]) == morph
-      f(k, morph)
-
-The order in which the morphologies are returned in unspecified, but the
-loop index `k` can be used to retrieve the correct state corresponding to
-iteration `k` of the original loop.
-
-The iterable returned by `Collection.load_unordered` should only be used while
-`collection` is valid, e.g. within its context or before calling
-`Collection.close`.
-
-Note: This API is 'experimental', meaning it might change in the future.
-)")
-
-        .def("argsort",
-             &morphio::Collection::argsort,
-             "morphology_names"_a,
-             R"(Argsort `morphology_names` by optimal access order.
-
-Note: This API is 'experimental', meaning it might change in the future.
-)")
-        .def("__enter__", [](morphio::Collection* collection) { return collection; })
-        .def("__exit__",
-             [](morphio::Collection* collection,
-                const py::object&,
-                const py::object&,
-                const py::object&) { collection->close(); })
-        .def("close", &morphio::Collection::close);
+            py::keep_alive<0, 1>() /* Essential: keep object alive while iterator exists */,
+            "Section iterator\n"
+            "\n"
+            "iter_type controls the iteration order. 3 values can be passed:\n"
+            "\n"
+            "- ``morphio.IterType.depth_first`` (default)\n"
+            "- ``morphio.IterType.breadth_first``\n"
+            "- ``morphio.IterType.upstream``\n",
+            "iter_type"_a = IterType::DEPTH_FIRST);
+#undef D
+}
 
-    py::class_<morphio::LoadUnordered<morphio::Morphology>>(
-        m, "LoadImmutableUnordered", "An iterable of immutable morphologies.")
-        .def(
-            "__iter__",
-            [](const morphio::LoadUnordered<morphio::Morphology>& iterable) {
-                return py::make_iterator(iterable.begin(), iterable.end());
-            },
-            // Bind the lifetime of the `morphio::LoadUnordered` (1) to the
-            // lifetime of the returned iterator (0).
-            py::keep_alive<0, 1>());
+void bind_soma(py::module& m) {
+    py::class_<morphio::Soma>(m, "Soma", DOC(morphio, Soma))
+        .def(py::init<const morphio::Soma&>())
+        .def_property_readonly(
+            "points",
+            [](morphio::Soma* soma) { return span_array_to_ndarray(soma->points()); },
+            DOC(morphio, Soma, points))
+        .def_property_readonly(
+            "diameters",
+            [](morphio::Soma* soma) { return span_to_ndarray(soma->diameters()); },
+            DOC(morphio, Soma, diameters))
+
+        .def_property_readonly(
+            "center",
+            [](morphio::Soma* soma) { return py::array(3, soma->center().data()); },
+            DOC(morphio, Soma, center))
+        .def_property_readonly("max_distance",
+                               &morphio::Soma::maxDistance,
+                               DOC(morphio, Soma, maxDistance))
+        .def_property_readonly("type", &morphio::Soma::type, DOC(morphio, Soma, type))
+        .def_property_readonly("surface", &morphio::Soma::surface, DOC(morphio, Soma, surface));
+}
+
+void bind_endoplasmic_reticulum(py::module& m) {
+    py::class_<morphio::EndoplasmicReticulum>(m,
+                                              "EndoplasmicReticulum",
+                                              DOC(morphio, EndoplasmicReticulum))
+        .def_property_readonly("section_indices",
+                               &morphio::EndoplasmicReticulum::sectionIndices,
+                               DOC(morphio, EndoplasmicReticulum, sectionIndices))
+        .def_property_readonly("volumes",
+                               &morphio::EndoplasmicReticulum::volumes,
+                               DOC(morphio, EndoplasmicReticulum, volumes))
+        .def_property_readonly("surface_areas",
+                               &morphio::EndoplasmicReticulum::surfaceAreas,
+                               DOC(morphio, EndoplasmicReticulum, surfaceAreas))
+        .def_property_readonly("filament_counts",
+                               &morphio::EndoplasmicReticulum::filamentCounts,
+                               DOC(morphio, EndoplasmicReticulum, filamentCounts));
+}
 
-    py::class_<morphio::LoadUnordered<morphio::mut::Morphology>>(
-        m, "LoadMutableUnordered", "An iterable of mutable morphologies.")
+void bind_dendritic_spine(py::module& m) {
+    py::class_<morphio::DendriticSpine, morphio::Morphology>(m,
+                                                             "DendriticSpine",
+                                                             DOC(morphio, DendriticSpine))
+        .def(py::init([](py::object arg) {
+                 return std::make_unique<morphio::DendriticSpine>(py::str(arg));
+             }),
+             "filename"_a)
+        .def_property_readonly("root_sections",
+                               &morphio::DendriticSpine::rootSections,
+                               DOC(morphio, Morphology, rootSections))
+        .def_property_readonly("sections",
+                               &morphio::DendriticSpine::sections,
+                               DOC(morphio, Morphology, sections))
+        .def("section",
+             &morphio::DendriticSpine::section,
+             DOC(morphio, Morphology, section),
+             "section_id"_a)
+        .def_property_readonly(
+            "points",
+            [](morphio::DendriticSpine* morpho) {
+                const auto& data = morpho->points();
+                return py::array(static_cast<py::ssize_t>(data.size()), data.data());
+            },
+            DOC(morphio, Morphology, points))
+        .def_property_readonly(
+            "diameters",
+            [](const morphio::DendriticSpine& morpho) {
+                const auto& data = morpho.diameters();
+                return py::array(static_cast<py::ssize_t>(data.size()), data.data());
+            },
+            DOC(morphio, Morphology, diameters))
+        .def_property_readonly(
+            "section_offsets",
+            [](const morphio::DendriticSpine& morpho) {
+                return as_pyarray(morpho.sectionOffsets());
+            },
+            DOC(morphio, Morphology, sectionOffsets))
+        .def_property_readonly(
+            "section_types",
+            [](const morphio::DendriticSpine& morph) {
+                const auto& data = morph.sectionTypes();
+                return py::array(static_cast<py::ssize_t>(data.size()), data.data());
+            },
+            DOC(morphio, Morphology, sectionTypes))
+        .def_property_readonly("connectivity",
+                               &morphio::DendriticSpine::connectivity,
+                               DOC(morphio, Morphology, connectivity))
+        .def_property_readonly("cell_family",
+                               &morphio::DendriticSpine::cellFamily,
+                               DOC(morphio, Morphology, cellFamily))
+        .def_property_readonly("post_synaptic_density",
+                               &morphio::DendriticSpine::postSynapticDensity,
+                               DOC(morphio, DendriticSpine, postSynapticDensity))
+        .def_property_readonly("version",
+                               &morphio::DendriticSpine::version,
+                               DOC(morphio, Morphology, version))
+
+        // Iterators
+        .def(
+            "iter",
+            [](morphio::DendriticSpine* morpho, IterType type) {
+                switch (type) {
+                case IterType::DEPTH_FIRST:
+                    return py::make_iterator(morpho->depth_begin(), morpho->depth_end());
+                case IterType::BREADTH_FIRST:
+                    return py::make_iterator(morpho->breadth_begin(), morpho->breadth_end());
+                case IterType::UPSTREAM:
+                default:
+                    throw morphio::MorphioError(
+                        "Only iteration types depth_first and breadth_first are supported");
+                }
+            },
+            py::keep_alive<0, 1>() /* Essential: keep object alive while iterator exists */,
+            "Section iterator that runs successively on every neurite\n"
+            "\n"
+            "iter_type controls the order of iteration on sections of a given neurite. 2 values "
+            "can be passed:\n"
+            "\n"
+            "- ``morphio.IterType.depth_first`` (default)\n"
+            "- ``morphio.IterType.breadth_first``\n",
+            "iter_type"_a = IterType::DEPTH_FIRST)
         .def(
-            "__iter__",
-            [](const morphio::LoadUnordered<morphio::mut::Morphology>& iterable) {
-                return py::make_iterator(iterable.begin(), iterable.end());
-            },
-            // Bind the lifetime of the `morphio::LoadUnordered` (1) to the
-            // lifetime of the returned iterator (0).
-            py::keep_alive<0, 1>());
+            "write",
+            [](morphio::mut::DendriticSpine* morph, py::object arg) { morph->write(py::str(arg)); },
+            "filename"_a);
 }
```

### Comparing `MorphIO-3.3.5/binds/python/bind_mutable.cpp` & `MorphIO-3.3.6/binds/python/bind_mutable.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -12,421 +12,338 @@
 #include <morphio/mut/morphology.h>
 
 #include <array>
 #include <memory>  // std::make_unique
 
 #include "bind_enums.h"
 #include "bindings_utils.h"
+#include "generated/docstrings.h"
 
 namespace py = pybind11;
+using namespace py::literals;
 
-mutable_binding_classes bind_mutable_classes(py::module& m) {
-    using namespace py::literals;
-
-    return mutable_binding_classes{
-        py::class_<morphio::mut::Morphology>(m,
-                                             "Morphology",
-                                             "Class representing a mutable Morphology"),
-        py::class_<morphio::mut::GlialCell, morphio::mut::Morphology>(
-            m, "GlialCell", "Class representing a mutable Glial Cell"),
-        py::class_<morphio::mut::Mitochondria>(m,
-                                               "Mitochondria",
-                                               "Class representing a mutable Mitochondria"),
-        py::class_<morphio::mut::MitoSection, std::shared_ptr<morphio::mut::MitoSection>>(
-            m, "MitoSection", "Class representing a mutable Mitochondrial Section"),
-        py::class_<morphio::mut::Section, std::shared_ptr<morphio::mut::Section>>(
-            m, "Section", "Class representing a mutable Section"),
-        py::class_<morphio::mut::Soma, std::shared_ptr<morphio::mut::Soma>>(
-            m, "Soma", "Class representing a mutable Soma"),
-        py::class_<morphio::mut::EndoplasmicReticulum>(
-            m, "EndoplasmicReticulum", "Class representing a mutable Endoplasmic Reticulum"),
-        py::class_<morphio::mut::DendriticSpine, morphio::mut::Morphology>(
-            m, "DendriticSpine", "Class representing a mutable Dendritic Spine")};
+void bind_mut_morphology(py::module& m);
+void bind_mut_glialcell(py::module& m);
+void bind_mut_mitochondria(py::module& m);
+void bind_mut_mitosection(py::module& m);
+void bind_mut_section(py::module& m);
+void bind_mut_soma(py::module& m);
+void bind_mut_endoplasmic_reticulum(py::module& m);
+void bind_mut_dendritic_spine(py::module& m);
+
+void bind_mutable(py::module& m) {
+    bind_mut_morphology(m);
+    bind_mut_glialcell(m);
+    bind_mut_mitochondria(m);
+    bind_mut_mitosection(m);
+    bind_mut_section(m);
+    bind_mut_soma(m);
+    bind_mut_endoplasmic_reticulum(m);
+    bind_mut_dendritic_spine(m);
 }
 
-void bind_mutable_methods(mutable_binding_classes& mutable_classes) {
-    using namespace py::literals;
+void bind_mut_morphology(py::module& m) {
+#define D(x) DOC(morphio, mut, Morphology, x)
+    using morphio::mut::Morphology;
 
-    mutable_classes.Morphology_mut_class.def(py::init<>())
+    py::class_<Morphology>(m, "Morphology", "Class representing a mutable Morphology")
+        .def(py::init<>())
         .def(py::init<const std::string&, unsigned int>(),
              "filename"_a,
              "options"_a = morphio::enums::Option::NO_MODIFIER)
         .def(py::init<const morphio::Morphology&, unsigned int>(),
              "morphology"_a,
              "options"_a = morphio::enums::Option::NO_MODIFIER)
-        .def(py::init<const morphio::mut::Morphology&, unsigned int>(),
+        .def(py::init<const Morphology&, unsigned int>(),
              "morphology"_a,
              "options"_a = morphio::enums::Option::NO_MODIFIER)
         .def(py::init([](py::object arg, unsigned int options) {
-                 return std::make_unique<morphio::mut::Morphology>(py::str(arg), options);
+                 return std::make_unique<Morphology>(py::str(arg), options);
              }),
              "filename"_a,
              "options"_a = morphio::enums::Option::NO_MODIFIER,
              "Additional Ctor that accepts as filename any python "
              "object that implements __repr__ or __str__")
 
         // Cell sub-part accessors
-        .def_property_readonly("sections",
-                               &morphio::mut::Morphology::sections,
-                               "Returns a list containing IDs of all sections. "
-                               "The first section of the vector is the soma section")
+        .def_property_readonly("sections", &Morphology::sections, D(sections))
         .def_property_readonly("root_sections",
-                               &morphio::mut::Morphology::rootSections,
-                               "Returns a list of all root sections IDs "
-                               "(sections whose parent ID are -1)",
+                               &Morphology::rootSections,
+                               D(rootSections),
                                py::return_value_policy::reference)
-        .def_property_readonly(
-            "soma",
-            static_cast<std::shared_ptr<morphio::mut::Soma>& (morphio::mut::Morphology::*) ()>(
-                &morphio::mut::Morphology::soma),
-            "Returns a reference to the soma object\n\n"
-            "Note: multiple morphologies can share the same Soma "
-            "instance")
-        .def_property_readonly(
-            "mitochondria",
-            static_cast<morphio::mut::Mitochondria& (morphio::mut::Morphology::*) ()>(
-                &morphio::mut::Morphology::mitochondria),
-            "Returns a reference to the mitochondria container class")
-        .def_property_readonly(
-            "endoplasmic_reticulum",
-            static_cast<morphio::mut::EndoplasmicReticulum& (morphio::mut::Morphology::*) ()>(
-                &morphio::mut::Morphology::endoplasmicReticulum),
-            "Returns a reference to the endoplasmic reticulum container class")
-        .def_property_readonly("annotations",
-                               &morphio::mut::Morphology::annotations,
-                               "Returns a list of annotations")
-        .def_property_readonly("markers",
-                               &morphio::mut::Morphology::markers,
-                               "Returns the list of NeuroLucida markers")
-        .def("section",
-             &morphio::mut::Morphology::section,
-             "Returns the section with the given id\n\n"
-             "Note: multiple morphologies can share the same Section "
-             "instances",
-             "section_id"_a)
-        .def("build_read_only",
-             &morphio::mut::Morphology::buildReadOnly,
-             "Returns the data structure used to create read-only "
-             "morphologies")
+        .def_property_readonly("soma",
+                               static_cast<std::shared_ptr<morphio::mut::Soma>& (Morphology::*) ()>(
+                                   &Morphology::soma),
+                               D(soma))
+        .def_property_readonly("mitochondria",
+                               static_cast<morphio::mut::Mitochondria& (Morphology::*) ()>(
+                                   &Morphology::mitochondria),
+                               D(mitochondria))
+        .def_property_readonly("endoplasmic_reticulum",
+                               static_cast<morphio::mut::EndoplasmicReticulum& (Morphology::*) ()>(
+                                   &Morphology::endoplasmicReticulum),
+                               D(endoplasmicReticulum))
+        .def_property_readonly("annotations", &Morphology::annotations, D(annotations))
+        .def_property_readonly("markers", &Morphology::markers, D(markers))
+        .def("section", &Morphology::section, D(section), "section_id"_a)
+        .def("build_read_only", &Morphology::buildReadOnly, D(buildReadOnly))
         .def("append_root_section",
-             static_cast<std::shared_ptr<morphio::mut::Section> (morphio::mut::Morphology::*)(
-                 const morphio::Property::PointLevel&, morphio::SectionType)>(
-                 &morphio::mut::Morphology::appendRootSection),
-             "Append a root Section\n",
+             static_cast<std::shared_ptr<morphio::mut::Section> (
+                 Morphology::*)(const morphio::Property::PointLevel&, morphio::SectionType)>(
+                 &Morphology::appendRootSection),
+             D(appendRootSection),
              "point_level_properties"_a,
              "section_type"_a)
         .def("append_root_section",
-             static_cast<std::shared_ptr<morphio::mut::Section> (morphio::mut::Morphology::*)(
-                 const morphio::Section&, bool)>(&morphio::mut::Morphology::appendRootSection),
-             "Append the existing immutable Section as a root section\n"
-             "If recursive == true, all descendent will be appended as "
-             "well",
+             static_cast<std::shared_ptr<morphio::mut::Section> (
+                 Morphology::*)(const morphio::Section&, bool)>(&Morphology::appendRootSection),
+             D(appendRootSection),
              "immutable_section"_a,
              "recursive"_a = false)
 
         .def("delete_section",
-             &morphio::mut::Morphology::deleteSection,
-             "Delete the given section\n"
-             "\n"
-             "Will silently fail if the section is not part of the tree\n"
-             "\n"
-             "If recursive == true, all descendent sections will be "
-             "deleted as well\n"
-             "Else, children will be re-attached to their grand-parent",
+             &Morphology::deleteSection,
+             D(deleteSection),
              "section"_a,
              "recursive"_a = true)
-
-        .def("as_immutable",
-             [](const morphio::mut::Morphology* morph) { return morphio::Morphology(*morph); })
-
-        .def_property_readonly("connectivity",
-                               &morphio::mut::Morphology::connectivity,
-                               "Return the graph connectivity of the morphology "
-                               "where each section is seen as a node\nNote: -1 is the soma node")
-
-        .def_property_readonly("cell_family",
-                               &morphio::mut::Morphology::cellFamily,
-                               "Returns the cell family (neuron or glia)")
-
-        .def_property_readonly("soma_type",
-                               &morphio::mut::Morphology::somaType,
-                               "Returns the soma type")
-
-        .def_property_readonly("version", &morphio::mut::Morphology::version, "Returns the version")
-
+        .def("as_immutable", [](const Morphology* morph) { return morphio::Morphology(*morph); })
+        .def_property_readonly("connectivity", &Morphology::connectivity, D(connectivity))
+        .def_property_readonly("cell_family", &Morphology::cellFamily, D(cellFamily))
+        .def_property_readonly("soma_type", &Morphology::somaType, D(somaType))
+        .def_property_readonly("version", &Morphology::version, D(version))
         .def("remove_unifurcations",
-             static_cast<void (morphio::mut::Morphology::*)()>(
-                 &morphio::mut::Morphology::removeUnifurcations),
-             "Fixes the morphology single child sections and issues warnings"
-             "if the section starts and ends are inconsistent")
-
+             static_cast<void (Morphology::*)()>(&Morphology::removeUnifurcations),
+             D(removeUnifurcations))
         .def(
             "write",
-            [](morphio::mut::Morphology* morph, py::object arg) { morph->write(py::str(arg)); },
-            "Write file to H5, SWC, ASC format depending on filename "
-            "extension",
+            [](Morphology* morph, py::object arg) { morph->write(py::str(arg)); },
+            D(write),
             "filename"_a)
 
         // Iterators
         .def(
             "iter",
-            [](morphio::mut::Morphology* morph, IterType type) {
+            [](Morphology* morph, IterType type) {
                 switch (type) {
                 case IterType::DEPTH_FIRST:
                     return py::make_iterator(morph->depth_begin(), morph->depth_end());
                 case IterType::BREADTH_FIRST:
                     return py::make_iterator(morph->breadth_begin(), morph->breadth_end());
                 case IterType::UPSTREAM:
                 default:
                     throw morphio::MorphioError(
                         "Only iteration types depth_first and "
                         "breadth_first are supported");
                 }
             },
-            py::keep_alive<0, 1>() /* Essential: keep object alive
-                                      while iterator exists */
-            ,
-            "Section iterator that runs successively on every "
-            "neurite\n"
+            py::keep_alive<0, 1>(), /* Essential: keep object alive while iterator exists */
+            "Section iterator that runs successively on every neurite\n"
             "\n"
             "iter_type controls the order of iteration on sections of "
             "a given neurite. 2 values can be passed:\n"
             "\n"
             "- ``morphio.IterType.depth_first`` (default)\n"
             "- ``morphio.IterType.breadth_first``\n",
             "iter_type"_a = IterType::DEPTH_FIRST)
         .def("append_root_section",
              static_cast<std::shared_ptr<morphio::mut::Section> (
-                 morphio::mut::Morphology::*)(const std::shared_ptr<morphio::mut::Section>&, bool)>(
-                 &morphio::mut::Morphology::appendRootSection),
-             "Append the existing mutable Section as a root section\n"
-             "If recursive == true, all descendent will be appended as well",
+                 Morphology::*)(const std::shared_ptr<morphio::mut::Section>&, bool)>(
+                 &Morphology::appendRootSection),
+             D(appendRootSection),
              "mutable_section"_a,
              "recursive"_a = false);
+#undef D
+}
 
-    mutable_classes.GlialCell_mut_class.def(py::init<>())
+void bind_mut_glialcell(py::module& m) {
+    py::class_<morphio::mut::GlialCell, morphio::mut::Morphology>(m,
+                                                                  "GlialCell",
+                                                                  DOC(morphio, mut, GlialCell))
+        .def(py::init<>())
         .def(py::init([](py::object arg) {
                  return std::make_unique<morphio::mut::GlialCell>(py::str(arg));
              }),
              "filename"_a,
              "Additional Ctor that accepts as filename any python "
              "object that implements __repr__ or __str__");
+}
 
-
-    mutable_classes.Mitochondria_mut_class.def(py::init<>())
+void bind_mut_mitochondria(py::module& m) {
+#define D(x) DOC(morphio, mut, Mitochondria, x)
+    using morphio::mut::Mitochondria;
+    using morphio::mut::MitoSection;
+    py::class_<Mitochondria>(m, "Mitochondria", DOC(morphio, mut, Mitochondria))
+        .def(py::init<>())
         .def_property_readonly("root_sections",
-                               &morphio::mut::Mitochondria::rootSections,
-                               "Returns a list of all root sections IDs "
-                               "(sections whose parent ID are -1)",
+                               &Mitochondria::rootSections,
+                               D(rootSections),
                                py::return_value_policy::reference)
-        .def_property_readonly("sections",
-                               &morphio::mut::Mitochondria::sections,
-                               "Return a dict where key is the mitochondrial section ID"
-                               " and value is the mithochondrial section")
-        .def("is_root",
-             &morphio::mut::Mitochondria::isRoot,
-             "Return True if section is a root section",
-             "section_id"_a)
-        .def("parent",
-             &morphio::mut::Mitochondria::parent,
-             "Returns the parent mithochondrial section ID",
-             "section_id"_a)
-        .def("children", &morphio::mut::Mitochondria::children, "section_id"_a)
-        .def("section",
-             &morphio::mut::Mitochondria::section,
-             "Get a reference to the given mithochondrial section\n\n"
-             "Note: multiple mitochondria can shared the same references",
-             "section_id"_a)
+        .def_property_readonly("sections", &Mitochondria::sections, D(sections))
+        .def("is_root", &Mitochondria::isRoot, D(isRoot), "section_id"_a)
+        .def("parent", &Mitochondria::parent, D(parent), "section_id"_a)
+        .def("children", &Mitochondria::children, D(children), "section_id"_a)
+        .def("section", &Mitochondria::section, D(section), "section_id"_a)
         .def("append_root_section",
-             static_cast<std::shared_ptr<morphio::mut::MitoSection> (morphio::mut::Mitochondria::*)(
+             static_cast<std::shared_ptr<MitoSection> (Mitochondria::*)(
                  const morphio::Property::MitochondriaPointLevel&)>(
-                 &morphio::mut::Mitochondria::appendRootSection),
-             "Append a new root MitoSection",
+                 &Mitochondria::appendRootSection),
+             D(appendRootSection),
              "point_level_properties"_a)
         .def("append_root_section",
-             static_cast<std::shared_ptr<morphio::mut::MitoSection> (
-                 morphio::mut::Mitochondria::*)(const morphio::MitoSection&, bool recursive)>(
-                 &morphio::mut::Mitochondria::appendRootSection),
-             "Append a new root MitoSection (if recursive == true, all "
-             "descendent will be appended "
-             "as well)",
+             static_cast<std::shared_ptr<MitoSection> (Mitochondria::*)(const morphio::MitoSection&,
+                                                                        bool recursive)>(
+                 &Mitochondria::appendRootSection),
+             D(appendRootSection_2),
              "immutable_section"_a,
              "recursive"_a = true)
         .def("append_root_section",
-             static_cast<std::shared_ptr<morphio::mut::MitoSection> (morphio::mut::Mitochondria::*)(
-                 const std::shared_ptr<morphio::mut::MitoSection>&, bool recursive)>(
-                 &morphio::mut::Mitochondria::appendRootSection),
-             "Append a new root MitoSection (if recursive == true, all "
-             "descendent will be appended "
-             "as well)",
+             static_cast<std::shared_ptr<MitoSection> (
+                 Mitochondria::*)(const std::shared_ptr<MitoSection>&, bool recursive)>(
+                 &Mitochondria::appendRootSection),
+             D(appendRootSection_2),
              "section"_a,
              "recursive"_a = true)
-
         .def(
             "depth_begin",
-            [](morphio::mut::Mitochondria* morph,
-               std::shared_ptr<morphio::mut::MitoSection> section) {
+            [](Mitochondria* morph, std::shared_ptr<MitoSection> section) {
                 return py::make_iterator(morph->depth_begin(section), morph->depth_end());
             },
             py::keep_alive<0, 1>() /* Essential: keep object alive while iterator exists */,
-            "Depth first iterator starting at a given section id\n"
-            "\n"
-            "If id == -1, the iteration will be successively performed "
-            "starting\n"
-            "at each root section",
+            D(depth_begin),
             "section_id"_a = -1)
         .def(
             "breadth_begin",
-            [](morphio::mut::Mitochondria* morph,
-               std::shared_ptr<morphio::mut::MitoSection> section) {
+            [](Mitochondria* morph, std::shared_ptr<MitoSection> section) {
                 return py::make_iterator(morph->breadth_begin(section), morph->breadth_end());
             },
             py::keep_alive<0, 1>() /* Essential: keep object alive while iterator exists */,
-            "Breadth first iterator starting at a given section id\n"
-            "\n"
-            "If id == -1, the iteration will be successively performed "
-            "starting\n"
-            "at each root section",
+            D(breadth_begin),
             "section_id"_a = -1)
         .def(
             "upstream_begin",
-            [](morphio::mut::Mitochondria* morph,
-               std::shared_ptr<morphio::mut::MitoSection> section) {
+            [](Mitochondria* morph, std::shared_ptr<MitoSection> section) {
                 return py::make_iterator(morph->upstream_begin(section), morph->upstream_end());
             },
             py::keep_alive<0, 1>() /* Essential: keep object alive while iterator exists */,
-            "Upstream iterator starting at a given section id\n\n"
-            "If id == -1, the iteration will be successively performed starting\n"
-            "at each root section",
+            D(upstream_begin),
             "section_id"_a = -1);
+#undef D
+}
 
-    using mitosection_floats_f = std::vector<morphio::floatType>& (morphio::mut::MitoSection::*) ();
-    using mitosection_ints_f = std::vector<uint32_t>& (morphio::mut::MitoSection::*) ();
-
-    mutable_classes.MitoSection_mut_class
-        .def_property_readonly("id", &morphio::mut::MitoSection::id, "Return the section ID")
+void bind_mut_mitosection(py::module& m) {
+    using morphio::mut::MitoSection;
+    using mitosection_floats_f = std::vector<morphio::floatType>& (MitoSection::*) ();
+    using mitosection_ints_f = std::vector<uint32_t>& (MitoSection::*) ();
+
+    py::class_<MitoSection, std::shared_ptr<MitoSection>>(m,
+                                                          "MitoSection",
+                                                          DOC(morphio, mut, MitoSection))
+        .def_property_readonly("id", &MitoSection::id, "Return the section ID")
         .def_property(
             "diameters",
-            static_cast<mitosection_floats_f>(&morphio::mut::MitoSection::diameters),
-            [](morphio::mut::MitoSection* section,
-               const std::vector<morphio::floatType>& _diameters) {
+            static_cast<mitosection_floats_f>(&MitoSection::diameters),
+            [](MitoSection* section, const std::vector<morphio::floatType>& _diameters) {
                 section->diameters() = _diameters;
             },
             "Returns the diameters of all points of this section")
         .def_property(
             "relative_path_lengths",
-            static_cast<mitosection_floats_f>(&morphio::mut::MitoSection::pathLengths),
-            [](morphio::mut::MitoSection* section,
-               const std::vector<morphio::floatType>& _pathLengths) {
+            static_cast<mitosection_floats_f>(&MitoSection::pathLengths),
+            [](MitoSection* section, const std::vector<morphio::floatType>& _pathLengths) {
                 section->pathLengths() = _pathLengths;
             },
             "Returns the relative distance (between 0 and 1)\n"
             "between the start of the neuronal section and each point\n"
             "of this mitochondrial section")
         .def_property(
             "neurite_section_ids",
-            static_cast<mitosection_ints_f>(&morphio::mut::MitoSection::neuriteSectionIds),
-            [](morphio::mut::MitoSection* section,
-               const std::vector<uint32_t>& _neuriteSectionIds) {
+            static_cast<mitosection_ints_f>(&MitoSection::neuriteSectionIds),
+            [](MitoSection* section, const std::vector<uint32_t>& _neuriteSectionIds) {
                 section->neuriteSectionIds() = _neuriteSectionIds;
             },
             "Returns the neurite section Ids of all points of this section")
-
-        .def("has_same_shape", &morphio::mut::MitoSection::hasSameShape)
-
+        .def("has_same_shape",
+             &MitoSection::hasSameShape,
+             DOC(morphio, mut, MitoSection, hasSameShape))
         .def("append_section",
-             static_cast<std::shared_ptr<morphio::mut::MitoSection> (morphio::mut::MitoSection::*)(
-                 const morphio::Property::MitochondriaPointLevel&)>(
-                 &morphio::mut::MitoSection::appendSection),
-             "Append a new MitoSection to this mito section",
+             static_cast<std::shared_ptr<MitoSection> (MitoSection::*)(
+                 const morphio::Property::MitochondriaPointLevel&)>(&MitoSection::appendSection),
+             DOC(morphio, mut, MitoSection, appendSection),
              "point_level_properties"_a)
-
         .def("append_section",
-             static_cast<std::shared_ptr<morphio::mut::MitoSection> (morphio::mut::MitoSection::*)(
-                 const std::shared_ptr<morphio::mut::MitoSection>&, bool)>(
-                 &morphio::mut::MitoSection::appendSection),
-             "Append a copy of the section to this section\n"
-             "If recursive == true, all descendent will be appended as well",
+             static_cast<std::shared_ptr<MitoSection> (MitoSection::*)(
+                 const std::shared_ptr<MitoSection>&, bool)>(&MitoSection::appendSection),
+             DOC(morphio, mut, MitoSection, appendSection_2),
              "section"_a,
              "recursive"_a = false)
-
         .def("append_section",
-             static_cast<std::shared_ptr<morphio::mut::MitoSection> (morphio::mut::MitoSection::*)(
-                 const morphio::MitoSection&, bool)>(&morphio::mut::MitoSection::appendSection),
-             "Append the existing immutable MitoSection to this section\n"
-             "If recursive == true, all descendent will be appended as well",
+             static_cast<std::shared_ptr<MitoSection> (
+                 MitoSection::*)(const morphio::MitoSection&, bool)>(&MitoSection::appendSection),
+             DOC(morphio, mut, MitoSection, appendSection_2),
              "immutable_section"_a,
              "recursive"_a = false);
+}
 
-
-    mutable_classes.Section_mut_class
+void bind_mut_section(py::module& m) {
+#define D(x) DOC(morphio, mut, Section, x)
+    py::class_<morphio::mut::Section, std::shared_ptr<morphio::mut::Section>>(
+        m, "Section", "Class representing a mutable Section")
         .def("__str__",
              [](const morphio::mut::Section& section) {
                  std::stringstream ss;
                  ss << section;
                  return ss.str();
              })
-
-        .def_property_readonly("id", &morphio::mut::Section::id, "Return the section ID")
+        .def_property_readonly("id", &morphio::mut::Section::id, D(id))
         .def_property(
             "type",
             static_cast<const morphio::SectionType& (morphio::mut::Section::*) () const>(
                 &morphio::mut::Section::type),
             [](morphio::mut::Section* section, morphio::SectionType _type) {
                 section->type() = _type;
             },
-            "Returns the morphological type of this section "
-            "(dendrite, axon, ...)")
+            D(type))
         .def_property(
             "points",
             [](morphio::mut::Section* section) {
                 return py::array(static_cast<py::ssize_t>(section->points().size()),
                                  section->points().data());
             },
             [](morphio::mut::Section* section, py::array_t<morphio::floatType> _points) {
                 section->points() = array_to_points(_points);
             },
-            "Returns the coordinates (x,y,z) of all points of this section")
+            D(points))
         .def_property(
             "diameters",
             [](morphio::mut::Section* section) {
                 return py::array(static_cast<py::ssize_t>(section->diameters().size()),
                                  section->diameters().data());
             },
             [](morphio::mut::Section* section, py::array_t<morphio::floatType> _diameters) {
                 section->diameters() = _diameters.cast<std::vector<morphio::floatType>>();
             },
-            "Returns the diameters of all points of this section")
+            D(diameters))
         .def_property(
             "perimeters",
             [](morphio::mut::Section* section) {
                 return py::array(static_cast<py::ssize_t>(section->perimeters().size()),
                                  section->perimeters().data());
             },
             [](morphio::mut::Section* section, py::array_t<morphio::floatType> _perimeters) {
                 section->perimeters() = _perimeters.cast<std::vector<morphio::floatType>>();
             },
-            "Returns the perimeters of all points of this section")
-        .def_property_readonly("is_root",
-                               &morphio::mut::Section::isRoot,
-                               "Return True if section is a root section")
-        .def_property_readonly("parent",
-                               &morphio::mut::Section::parent,
-                               "Get the parent ID\n\n"
-                               "Note: Root sections return -1")
-        .def_property_readonly("children",
-                               &morphio::mut::Section::children,
-                               "Returns a list of children IDs")
+            D(perimeters))
+        .def_property_readonly("is_root", &morphio::mut::Section::isRoot, D(isRoot))
+        .def_property_readonly("parent", &morphio::mut::Section::parent, D(parent))
+        .def_property_readonly("children", &morphio::mut::Section::children, D(children))
         .def("is_heterogeneous",
              &morphio::mut::Section::isHeterogeneous,
-             "Returns true if the tree downtream (downstream = true) or upstream (downstream = "
-             "false)\n"
-             "has the same type as the current section.",
+             D(isHeterogeneous),
              py::arg("downstream") = true)
-        .def("has_same_shape", &morphio::mut::Section::hasSameShape)
+        .def("has_same_shape", &morphio::mut::Section::hasSameShape, D(hasSameShape))
 
         // Iterators
         .def(
             "iter",
             [](morphio::mut::Section* section, IterType type) {
                 switch (type) {
                 case IterType::DEPTH_FIRST:
@@ -448,77 +365,83 @@
             "\n"
             "- ``morphio.IterType.depth_first`` (default)\n"
             "- ``morphio.IterType.breadth_first``\n"
             "- ``morphio.IterType.upstream``\n",
             "iter_type"_a = IterType::DEPTH_FIRST)
 
         // Editing
+
+        .def("append_section",
+             static_cast<std::shared_ptr<morphio::mut::Section> (morphio::mut::Section::*)(
+                 const morphio::Property::PointLevel&, morphio::SectionType)>(
+                 &morphio::mut::Section::appendSection),
+             D(appendSection),
+             "point_level_properties"_a,
+             "section_type"_a = morphio::SectionType::SECTION_UNDEFINED)
         .def("append_section",
              static_cast<std::shared_ptr<morphio::mut::Section> (morphio::mut::Section::*)(
                  const morphio::Section&, bool)>(&morphio::mut::Section::appendSection),
-             "Append the existing immutable Section to this section"
-             "If recursive == true, all descendent will be appended as well",
+             D(appendSection_2),
              "immutable_section"_a,
              "recursive"_a = false)
-
         .def("append_section",
              static_cast<std::shared_ptr<morphio::mut::Section> (
                  morphio::mut::Section::*)(std::shared_ptr<morphio::mut::Section>, bool)>(
                  &morphio::mut::Section::appendSection),
-             "Append the existing mutable Section to this section\n"
-             "If recursive == true, all descendent will be appended as well",
+             D(appendSection_2),
              "mutable_section"_a,
-             "recursive"_a = false)
-
-        .def("append_section",
-             static_cast<std::shared_ptr<morphio::mut::Section> (morphio::mut::Section::*)(
-                 const morphio::Property::PointLevel&, morphio::SectionType)>(
-                 &morphio::mut::Section::appendSection),
-             "Append a new Section to this section\n"
-             " If section_type is omitted or set to 'undefined'"
-             " the type of the parent section will be used",
-             "point_level_properties"_a,
-             "section_type"_a = morphio::SectionType::SECTION_UNDEFINED);
+             "recursive"_a = false);
+#undef D
+}
 
-    mutable_classes.Soma_mut_class.def(py::init<const morphio::Property::PointLevel&>())
+void bind_mut_soma(py::module& m) {
+#define D(x) DOC(morphio, mut, Soma, x)
+    py::class_<morphio::mut::Soma, std::shared_ptr<morphio::mut::Soma>>(m,
+                                                                        "Soma",
+                                                                        DOC(morphio, mut, Soma))
+        .def(py::init<const morphio::Property::PointLevel&>())
         .def_property(
             "points",
             [](morphio::mut::Soma* soma) {
                 return py::array(static_cast<py::ssize_t>(soma->points().size()),
                                  soma->points().data());
             },
             [](morphio::mut::Soma* soma, py::array_t<morphio::floatType> _points) {
                 soma->points() = array_to_points(_points);
             },
-            "Returns the coordinates (x,y,z) of all soma point")
+            D(points))
         .def_property(
             "diameters",
             [](morphio::mut::Soma* soma) {
                 return py::array(static_cast<py::ssize_t>(soma->diameters().size()),
                                  soma->diameters().data());
             },
             [](morphio::mut::Soma* soma, py::array_t<morphio::floatType> _diameters) {
                 soma->diameters() = _diameters.cast<std::vector<morphio::floatType>>();
             },
-            "Returns the diameters of all soma points")
-        .def_property_readonly("type", &morphio::mut::Soma::type, "Returns the soma type")
-        .def_property_readonly("surface",
-                               &morphio::mut::Soma::surface,
-                               "Returns the soma surface\n\n"
-                               "Note: the soma surface computation depends on the soma type")
-        .def_property_readonly("max_distance",
-                               &morphio::mut::Soma::maxDistance,
-                               "Return the maximum distance between the center of gravity "
-                               "and any of the soma points")
+            D(diameters))
+        .def_property(
+            "type",
+            [](morphio::mut::Soma* soma) { return soma->type(); },
+            [](morphio::mut::Soma* soma, morphio::SomaType type) { soma->type() = type; },
+            D(type))
+        .def_property_readonly("surface", &morphio::mut::Soma::surface, D(surface))
+        .def_property_readonly("max_distance", &morphio::mut::Soma::maxDistance, D(maxDistance))
         .def_property_readonly(
             "center",
             [](morphio::mut::Soma* soma) { return py::array(3, soma->center().data()); },
-            "Returns the center of gravity of the soma points");
+            D(center));
+#undef D
+}
 
-    mutable_classes.EndoplasmicReticulum_mut_class.def(py::init<>())
+void bind_mut_endoplasmic_reticulum(py::module& m) {
+    py::class_<morphio::mut::EndoplasmicReticulum>(m,
+                                                   "EndoplasmicReticulum",
+                                                   DOC(morphio, mut, EndoplasmicReticulum))
+        .def(py::init<>())
         .def(py::init<const std::vector<uint32_t>&,
                       const std::vector<morphio::floatType>&,
                       const std::vector<morphio::floatType>&,
                       const std::vector<uint32_t>&>())
         .def(py::init<const morphio::EndoplasmicReticulum&>())
         .def(py::init<const morphio::mut::EndoplasmicReticulum&>())
 
@@ -527,93 +450,91 @@
             [](morphio::mut::EndoplasmicReticulum* reticulum) {
                 return py::array(static_cast<py::ssize_t>(reticulum->sectionIndices().size()),
                                  reticulum->sectionIndices().data());
             },
             [](morphio::mut::EndoplasmicReticulum* reticulum, py::array_t<uint32_t> indices) {
                 reticulum->sectionIndices() = indices.cast<std::vector<uint32_t>>();
             },
-            "Returns the list of neuronal section indices")
+            DOC(morphio, mut, EndoplasmicReticulum, sectionIndices))
         .def_property(
             "volumes",
             [](morphio::mut::EndoplasmicReticulum* reticulum) {
                 return py::array(static_cast<py::ssize_t>(reticulum->volumes().size()),
                                  reticulum->volumes().data());
             },
             [](morphio::mut::EndoplasmicReticulum* reticulum,
                py::array_t<morphio::floatType> volumes) {
                 reticulum->volumes() = volumes.cast<std::vector<morphio::floatType>>();
             },
-            "Returns the volumes for each neuronal section")
-
+            DOC(morphio, mut, EndoplasmicReticulum, volumes))
         .def_property(
             "surface_areas",
             [](morphio::mut::EndoplasmicReticulum* reticulum) {
                 return py::array(static_cast<py::ssize_t>(reticulum->surfaceAreas().size()),
                                  reticulum->surfaceAreas().data());
             },
             [](morphio::mut::EndoplasmicReticulum* reticulum,
                py::array_t<morphio::floatType> areas) {
                 reticulum->surfaceAreas() = areas.cast<std::vector<morphio::floatType>>();
             },
-            "Returns the surface areas for each neuronal section")
-
+            DOC(morphio, mut, EndoplasmicReticulum, surfaceAreas))
         .def_property(
             "filament_counts",
             [](morphio::mut::EndoplasmicReticulum* reticulum) {
                 return py::array(static_cast<py::ssize_t>(reticulum->filamentCounts().size()),
                                  reticulum->filamentCounts().data());
             },
             [](morphio::mut::EndoplasmicReticulum* reticulum, py::array_t<uint32_t> counts) {
                 reticulum->filamentCounts() = counts.cast<std::vector<uint32_t>>();
             },
-            "Returns the number of filaments for each neuronal section");
+            DOC(morphio, mut, EndoplasmicReticulum, filamentCounts));
+}
 
-    mutable_classes.DendriticSpine_mut_class.def(py::init<>())
+void bind_mut_dendritic_spine(py::module& m) {
+    py::class_<morphio::mut::DendriticSpine, morphio::mut::Morphology>(
+        m, "DendriticSpine", DOC(morphio, mut, DendriticSpine))
+        .def(py::init<>())
         .def(py::init([](py::object arg) {
                  return std::make_unique<morphio::mut::DendriticSpine>(py::str(arg));
              }),
              "filename"_a,
              "Additional Ctor that accepts as filename any python "
              "object that implements __repr__ or __str__")
         .def_property_readonly("sections",
                                &morphio::mut::DendriticSpine::sections,
-                               "Returns a list containing IDs of all sections.")
+                               DOC(morphio, mut, Morphology, sections))
         .def_property_readonly("root_sections",
                                &morphio::mut::DendriticSpine::rootSections,
-                               "Returns a list of all root sections IDs "
-                               "(sections whose parent ID are -1)",
+                               DOC(morphio, mut, Morphology, rootSections),
                                py::return_value_policy::reference)
         .def("append_root_section",
              static_cast<std::shared_ptr<morphio::mut::Section> (morphio::mut::DendriticSpine::*)(
                  const morphio::Property::PointLevel&, morphio::SectionType)>(
                  &morphio::mut::Morphology::appendRootSection),
-             "Append a root Section\n",
+             DOC(morphio, mut, Morphology, appendRootSection),
              "point_level_properties"_a,
              "section_type"_a)
         .def("append_root_section",
              static_cast<std::shared_ptr<morphio::mut::Section> (morphio::mut::DendriticSpine::*)(
                  const morphio::Section&, bool)>(&morphio::mut::Morphology::appendRootSection),
-             "Append the existing immutable Section as a root section\n"
-             "If recursive == true, all descendent will be appended as "
-             "well",
+             DOC(morphio, mut, Morphology, appendRootSection_2),
              "immutable_section"_a,
              "recursive"_a = false)
 
         .def_property(
             "post_synaptic_density",
-
             [](const morphio::mut::DendriticSpine& dendritic_spine) {
                 return dendritic_spine.postSynapticDensity();
             },
             [](morphio::mut::DendriticSpine* dendritic_spine,
                const std::vector<morphio::Property::DendriticSpine::PostSynapticDensity>& psds) {
                 dendritic_spine->postSynapticDensity() = psds;
             },
-            "Returns the post synaptic density values")
+            DOC(morphio, mut, DendriticSpine, postSynapticDensity))
         .def_property_readonly("cell_family",
                                &morphio::mut::DendriticSpine::cellFamily,
-                               "Returns the cell family")
+                               DOC(morphio, enums, CellFamily))
         .def(
             "write",
             [](morphio::mut::DendriticSpine* morph, py::object arg) { morph->write(py::str(arg)); },
             "filename"_a);
 }
```

### Comparing `MorphIO-3.3.5/binds/python/bind_vasculature.cpp` & `MorphIO-3.3.6/binds/python/bind_vasculature.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/bindings_utils.cpp` & `MorphIO-3.3.6/binds/python/bindings_utils.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/CMakeLists.txt` & `MorphIO-3.3.6/binds/python/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/LICENSE` & `MorphIO-3.3.6/binds/python/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/attr.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/buffer_info.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/cast.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/chrono.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/complex.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/class.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/common.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/descr.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/init.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/internals.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/type_caster_base.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/detail/typeid.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/eigen.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/embed.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/eval.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/functional.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/gil.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/iostream.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/numpy.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/operators.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/options.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/pybind11.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/pytypes.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/stl/filesystem.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/stl.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/include/pybind11/stl_bind.h` & `MorphIO-3.3.6/binds/python/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/tools/FindCatch.cmake` & `MorphIO-3.3.6/binds/python/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/tools/FindEigen3.cmake` & `MorphIO-3.3.6/binds/python/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/tools/FindPythonLibsNew.cmake` & `MorphIO-3.3.6/binds/python/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/tools/pybind11Common.cmake` & `MorphIO-3.3.6/binds/python/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/tools/pybind11NewTools.cmake` & `MorphIO-3.3.6/binds/python/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/binds/python/pybind11/tools/pybind11Tools.cmake` & `MorphIO-3.3.6/binds/python/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/include/morphio/collection.h` & `MorphIO-3.3.6/include/morphio/collection.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/include/morphio/dendritic_spine.h` & `MorphIO-3.3.6/include/morphio/dendritic_spine.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/include/morphio/endoplasmic_reticulum.h` & `MorphIO-3.3.6/include/morphio/endoplasmic_reticulum.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/include/morphio/errorMessages.h` & `MorphIO-3.3.6/include/morphio/errorMessages.h`

 * *Files 1% similar despite different names*

```diff
@@ -62,22 +62,23 @@
 };
 
 // TODO: this shouldn't be global static
 static std::set<Warning> _ignoredWarnings;
 
 /** A sample of section for error reporting, includes its position (line) within the file. **/
 struct Sample {
+    enum : unsigned int { UNKNOWN_ID = 0xFFFFFFFE };
     Sample() = default;
 
     floatType diameter = -1.;
     bool valid = false;
     Point point{};
     SectionType type = SECTION_UNDEFINED;
-    int parentId = -1;
-    unsigned int id = 0;
+    unsigned int parentId = UNKNOWN_ID;
+    unsigned int id = UNKNOWN_ID;
     unsigned int lineNumber = 0;
 };
 
 /** Class that can generate error messages and holds a collection of predefined errors
     messages **/
 class ErrorMessages
 {
@@ -205,14 +206,23 @@
                                              size_t length2) const;
 
     /** Cant write perimeter data to SWC,ASC error message */
     std::string ERROR_PERIMETER_DATA_NOT_WRITABLE();
     /** Single section child SWC error message */
     std::string ERROR_ONLY_CHILD_SWC_WRITER(unsigned int parentId) const;
 
+    /** Single point soma must have one point */
+    std::string ERROR_SOMA_INVALID_SINGLE_POINT() const;
+
+    /** Multiple points for single point soma */
+    std::string ERROR_SOMA_INVALID_THREE_POINT_CYLINDER() const;
+
+    /** Contour soma must have at least 3 points. */
+    std::string ERROR_SOMA_INVALID_CONTOUR() const;
+
 
     ////////////////////////////////////////////////////////////////////////////////
     //              WARNINGS
     ////////////////////////////////////////////////////////////////////////////////
 
     /** Writing of mitochondria is not supported warning message */
     std::string WARNING_MITOCHONDRIA_WRITE_NOT_SUPPORTED() const;
@@ -240,14 +250,20 @@
     std::string WARNING_NEUROMORPHO_SOMA_NON_CONFORM(const Sample& root,
                                                      const Sample& child1,
                                                      const Sample& child2);
 
     /** Wrong root point warning message */
     std::string WARNING_WRONG_ROOT_POINT(const std::vector<Sample>& children) const;
 
+    /**  Soma must be a contour for ASC and H5 */
+    std::string WARNING_SOMA_NON_CONTOUR() const;
+
+    /* Soma must be stacked cylinders or a point */
+    std::string WARNING_SOMA_NON_CYLINDER_OR_POINT() const;
+
   private:
     std::string _uri;
 };
 
 }  // namespace readers
 
 }  // namespace morphio
```

### Comparing `MorphIO-3.3.5/include/morphio/exceptions.h` & `MorphIO-3.3.6/include/morphio/exceptions.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/include/morphio/mito_section.h` & `MorphIO-3.3.6/include/morphio/mito_section.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/include/morphio/mitochondria.h` & `MorphIO-3.3.6/include/morphio/mitochondria.h`

 * *Files 13% similar despite different names*

```diff
@@ -14,16 +14,25 @@
  * mitochondrial level. As the Morphology class, it implements a section accessor
  * and a root section accessor returning views on the Properties object for the
  * queried mitochondrial section.
  **/
 class Mitochondria
 {
   public:
+    /// Return the Section with the given id.
     MitoSection section(uint32_t id) const;
+
+    /// Return a vector of all root sections
     std::vector<MitoSection> rootSections() const;
+
+    /** Return a vector containing all section objects
+     *
+     * Notes:
+     * Soma is not included
+     **/
     std::vector<MitoSection> sections() const;
 
   private:
     explicit Mitochondria(const std::shared_ptr<Property::Properties>& properties)
         : properties_(properties) {}
     std::shared_ptr<Property::Properties> properties_;
```

### Comparing `MorphIO-3.3.5/include/morphio/morphology.h` & `MorphIO-3.3.6/include/morphio/morphology.h`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,19 @@
 
     /**
      * Return a vector of all root sections
      * (sections whose parent ID are -1)
      **/
     std::vector<Section> rootSections() const;
 
-    /** Return a vector containing all section objects */
+    /** Return a vector containing all section objects
+     *
+     * Notes:
+     * Soma is not included
+     **/
     std::vector<Section> sections() const;
 
     /**
      * Return the Section with the given id.
      *
      * @throw RawDataError if the id is out of range
      */
```

### Comparing `MorphIO-3.3.5/include/morphio/mut/endoplasmic_reticulum.h` & `MorphIO-3.3.6/include/morphio/mut/endoplasmic_reticulum.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/include/morphio/mut/mito_section.h` & `MorphIO-3.3.6/include/morphio/mut/mito_section.h`

 * *Files 12% similar despite different names*

```diff
@@ -15,33 +15,45 @@
   public:
     MitoSection(Mitochondria* mitochondria,
                 unsigned int id,
                 const Property::MitochondriaPointLevel& pointProperties);
     MitoSection(Mitochondria* mitochondria, unsigned int id, const morphio::MitoSection& section);
     MitoSection(Mitochondria* mitochondria, unsigned int id, const MitoSection& section);
 
+    /// Append a MitoSection
     std::shared_ptr<MitoSection> appendSection(const Property::MitochondriaPointLevel& points);
 
+    /**
+       Append a MitoSection
+
+       If recursive == true, all descendent mito sections will be appended as well
+    **/
     std::shared_ptr<MitoSection> appendSection(const std::shared_ptr<MitoSection>& original_section,
                                                bool recursive);
 
+    /**
+       Append a MitoSection
+
+       If recursive == true, all descendent mito sections will be appended as well
+    **/
     std::shared_ptr<MitoSection> appendSection(const morphio::MitoSection& section, bool recursive);
 
+    /// Get the Section parent
     std::shared_ptr<MitoSection> parent() const;
+
+    /// Return true if section is a root section
     bool isRoot() const;
+
+    /// Get the Section children
     const std::vector<std::shared_ptr<MitoSection>>& children() const;
 
-    /**
-     * Return true if the both sections have the same neuriteSectionIds, diameters and pathLengths
-     */
+    /// Return true if the both sections have the same neuriteSectionIds, diameters and pathLengths
     bool hasSameShape(const MitoSection& other) const noexcept;
 
-    /**
-     * Return the section id
-     **/
+    /// Return the section id
     inline uint32_t id() const noexcept;
 
     /** @{
      * Return the diameters of all points of this section
      **/
     inline const std::vector<morphio::floatType>& diameters() const noexcept;
     inline std::vector<morphio::floatType>& diameters() noexcept;
```

### Comparing `MorphIO-3.3.5/include/morphio/mut/mitochondria.h` & `MorphIO-3.3.6/include/morphio/mut/mitochondria.h`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,25 @@
 class Mitochondria
 {
     using MitoSectionP = std::shared_ptr<MitoSection>;
 
   public:
     Mitochondria() = default;
 
+    /// Get the Section children
     const std::vector<MitoSectionP>& children(const MitoSectionP&) const;
+
+    /**
+       Get the shared pointer for the given section
+
+       Note: multiple morphologies can share the same Section instances.
+    **/
     const MitoSectionP& section(uint32_t id) const;
+
+    /// Returns the dictionary id -> Section for this tree
     const std::map<uint32_t, MitoSectionP>& sections() const noexcept;
 
     /**
        Depth first iterator starting at a given section id
 
        If id == -1, the iteration will start at each root section, successively
     **/
```

### Comparing `MorphIO-3.3.5/include/morphio/mut/modifiers.h` & `MorphIO-3.3.6/include/morphio/mut/modifiers.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/include/morphio/mut/morphology.h` & `MorphIO-3.3.6/include/morphio/mut/morphology.h`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     }
     ///
     /// Return the endoplasmic reticulum container class
     const EndoplasmicReticulum& endoplasmicReticulum() const noexcept {
         return _endoplasmicReticulum;
     }
 
-    /// Return the annotation object
+    /// Return the annotation objects
     const std::vector<Property::Annotation>& annotations() const noexcept {
         return _cellProperties->_annotations;
     }
 
     /// Return the markers from the ASC file
     const std::vector<Property::Marker>& markers() const noexcept {
         return _cellProperties->_markers;
```

### Comparing `MorphIO-3.3.5/include/morphio/mut/section.h` & `MorphIO-3.3.6/include/morphio/mut/section.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/include/morphio/mut/soma.h` & `MorphIO-3.3.6/include/morphio/mut/soma.h`

 * *Files 13% similar despite different names*

```diff
@@ -28,17 +28,23 @@
         return point_properties_._diameters;
     }
     const std::vector<morphio::floatType>& diameters() const noexcept {
         return point_properties_._diameters;
     }
 
     /// Return the soma type
-    SomaType type() const noexcept {
+    const SomaType& type() const noexcept {
         return soma_type_;
     }
+
+    /// Return the soma type
+    SomaType& type() noexcept {
+        return soma_type_;
+    }
+
     /**
      * Return the center of gravity of the soma points
      **/
     Point center() const;
 
     /**
        Return the soma surface
```

### Comparing `MorphIO-3.3.5/include/morphio/properties.h` & `MorphIO-3.3.6/include/morphio/properties.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/include/morphio/section.h` & `MorphIO-3.3.6/include/morphio/section.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/include/morphio/section_base.h` & `MorphIO-3.3.6/include/morphio/section_base.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/include/morphio/section_iterators.hpp` & `MorphIO-3.3.6/include/morphio/section_iterators.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/include/morphio/soma.h` & `MorphIO-3.3.6/include/morphio/soma.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/include/morphio/tools.h` & `MorphIO-3.3.6/include/morphio/tools.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/include/morphio/types.h` & `MorphIO-3.3.6/include/morphio/types.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/include/morphio/vasc/iterators.hpp` & `MorphIO-3.3.6/include/morphio/vasc/iterators.hpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/include/morphio/vasc/properties.h` & `MorphIO-3.3.6/include/morphio/vasc/properties.h`

 * *Files 6% similar despite different names*

```diff
@@ -58,14 +58,17 @@
 struct VascSectionLevel {
     std::vector<VascSection::Type> _sections;
     std::vector<SectionType::Type> _sectionTypes;
     std::map<uint32_t, std::vector<uint32_t>> _predecessors;
     std::map<uint32_t, std::vector<uint32_t>> _successors;
     bool operator==(const VascSectionLevel& other) const;
     bool operator!=(const VascSectionLevel& other) const;
+
+    // Like operator!= but with logLevel argument
+    bool diff(const VascSectionLevel& other, LogLevel logLevel) const;
 };
 
 /** Class that holds all other levels(point, edge, etc.) information */
 struct Properties {
     VascPointLevel _pointLevel;
     VascEdgeLevel _edgeLevel;
     VascSectionLevel _sectionLevel;
@@ -73,28 +76,22 @@
 
     template <typename T>
     std::vector<typename T::Type>& get_mut() noexcept;
 
     template <typename T>
     const std::vector<typename T::Type>& get() const noexcept;
 
-    inline const std::map<uint32_t, std::vector<uint32_t>>& predecessors() const noexcept;
-    inline const std::map<uint32_t, std::vector<uint32_t>>& successors() const noexcept;
-
-    bool operator==(const Properties& other) const;
-    bool operator!=(const Properties& other) const;
+    const std::map<uint32_t, std::vector<uint32_t>>& predecessors() const noexcept {
+        return _sectionLevel._predecessors;
+    }
+    const std::map<uint32_t, std::vector<uint32_t>>& successors() const noexcept {
+        return _sectionLevel._successors;
+    }
 };
 
-inline const std::map<uint32_t, std::vector<uint32_t>>& Properties::predecessors() const noexcept {
-    return _sectionLevel._predecessors;
-}
-inline const std::map<uint32_t, std::vector<uint32_t>>& Properties::successors() const noexcept {
-    return _sectionLevel._successors;
-}
-
 std::ostream& operator<<(std::ostream& os, const Properties& properties);
 std::ostream& operator<<(std::ostream& os, const VascPointLevel& pointLevel);
 
 #define INSTANTIATE_TEMPLATE_GET(T, M)                                       \
     template <>                                                              \
     inline std::vector<T::Type>& Properties::get_mut<T>() noexcept {         \
         return M;                                                            \
```

### Comparing `MorphIO-3.3.5/include/morphio/vasc/section.h` & `MorphIO-3.3.6/include/morphio/vasc/section.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/include/morphio/vasc/vasculature.h` & `MorphIO-3.3.6/include/morphio/vasc/vasculature.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/include/morphio/vector_types.h` & `MorphIO-3.3.6/include/morphio/vector_types.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/morphio/__init__.py` & `MorphIO-3.3.6/morphio/__init__.py`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/setup.py` & `MorphIO-3.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/CMakeLists.txt` & `MorphIO-3.3.6/src/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -75,20 +75,16 @@
   PROPERTIES
   CXX_STANDARD 14
   CXX_STANDARD_REQUIRED YES
   CXX_EXTENSIONS NO
   )
 
 if (MORPHIO_ENABLE_COVERAGE)
-  target_compile_options(morphio_obj
-    PUBLIC -g -O0 --coverage -fprofile-arcs -ftest-coverage
-    )
-  target_link_libraries(morphio_obj
-    PUBLIC gcov
-    )
+  include(CodeCoverage)
+  append_coverage_compiler_flags_to_target(morphio_obj)
 endif()
 
 
 if (NOT WIN32)
   target_compile_options(morphio_obj
     PRIVATE
     -Wall
@@ -111,21 +107,14 @@
      $<INSTALL_INTERFACE:include>
      $<TARGET_PROPERTY:gsl-lite,INTERFACE_INCLUDE_DIRECTORIES>
      $<TARGET_PROPERTY:HighFive,INTERFACE_INCLUDE_DIRECTORIES>
     PRIVATE
      $<TARGET_PROPERTY:lexertl,INTERFACE_INCLUDE_DIRECTORIES>
      )
   target_link_libraries(${TARGET} PUBLIC gsl-lite PRIVATE HighFive lexertl)
-
-  if (MORPHIO_ENABLE_COVERAGE)
-     target_link_libraries(${TARGET}
-     PUBLIC gcov
-     )
-  endif()
-
 endforeach(TARGET)
 
 install(
   # DIRECTORY ${CMAKE_CURRENT_BINARY_DIR}
   TARGETS morphio_shared
   EXPORT MorphIOTargets
   LIBRARY DESTINATION lib
```

### Comparing `MorphIO-3.3.5/src/collection.cpp` & `MorphIO-3.3.6/src/collection.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/dendritic_spine.cpp` & `MorphIO-3.3.6/src/dendritic_spine.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/endoplasmic_reticulum.cpp` & `MorphIO-3.3.6/src/endoplasmic_reticulum.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/enums.cpp` & `MorphIO-3.3.6/src/enums.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/errorMessages.cpp` & `MorphIO-3.3.6/src/errorMessages.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,48 @@
-//#include <cmath>
 #include <iostream>  // std::cerr
 #include <sstream>   // std::ostringstream
 #include <string>
 #include <vector>
 
 #include <morphio/errorMessages.h>
 
 namespace morphio {
 static int MORPHIO_MAX_N_WARNINGS = 100;
 static bool MORPHIO_RAISE_WARNINGS = false;
 
 /**
-   Controls the maximum number of warning to be printed on screen
-   0 will print no warning
-   -1 will print them all
-**/
+ * Controls the maximum number of warning to be printed on screen.
+ * 0 will print no warning
+ * -1 will print them all
+ */
 void set_maximum_warnings(int n_warnings) {
     MORPHIO_MAX_N_WARNINGS = n_warnings;
 }
 
-/**
-   Whether to raise warning as errors
-**/
+/*
+ *   Whether to raise warning as errors
+ */
 void set_raise_warnings(bool is_raise) {
     MORPHIO_RAISE_WARNINGS = is_raise;
 }
 
+/**
+ *   Ignore/Unignore a specific warning message
+ */
 void set_ignored_warning(Warning warning, bool ignore) {
     if (ignore) {
         readers::_ignoredWarnings.insert(warning);
     } else {
         readers::_ignoredWarnings.erase(warning);
     }
 }
 
+/**
+ *   Ignore/Unignore a specific warning message
+ */
 void set_ignored_warning(const std::vector<Warning>& warnings, bool ignore) {
     for (auto warning : warnings) {
         set_ignored_warning(warning, ignore);
     }
 }
 
 void printError(Warning warning, const std::string& msg) {
@@ -72,14 +77,16 @@
 
 std::string ErrorMessages::errorMsg(long unsigned int lineNumber,
                                     ErrorLevel errorLevel,
                                     std::string msg) const {
     return "\n" + (_uri.empty() ? "" : errorLink(lineNumber, errorLevel) + "\n") + msg;
 }
 
+// LCOV_EXCL_START {  all the error messages are excluded from coverage
+
 ////////////////////////////////////////////////////////////////////////////////
 //              ERRORS
 ////////////////////////////////////////////////////////////////////////////////
 
 std::string ErrorMessages::ERROR_OPENING_FILE() const {
     return "Error opening morphology file:\n" + errorMsg(0, ErrorLevel::ERROR);
 }
@@ -249,14 +256,26 @@
     return ("Section " + std::to_string(parentId) +
             " has a single child section. "
             "Single child section are not allowed when writing to SWC format. "
             "Please sanitize the morphology first.\n"
             "Tip: you can use 'removeUnifurcations() (C++) / remove_unifurcations() (python)'");
 }
 
+std::string ErrorMessages::ERROR_SOMA_INVALID_SINGLE_POINT() const {
+    return "Single point soma must have one point";
+}
+
+std::string ErrorMessages::ERROR_SOMA_INVALID_THREE_POINT_CYLINDER() const {
+    return "Multiple points for single point soma";
+}
+
+std::string ErrorMessages::ERROR_SOMA_INVALID_CONTOUR() const {
+    return "Contour soma must have at least 3 points.";
+}
+
 
 ////////////////////////////////////////////////////////////////////////////////
 //              WARNINGS
 ////////////////////////////////////////////////////////////////////////////////
 std::string ErrorMessages::WARNING_WRITE_NO_SOMA() const {
     return errorMsg(0, ErrorLevel::WARNING, "Warning: writing file without a soma");
 }
@@ -387,10 +406,26 @@
            "point:";
     for (const auto& child : children) {
         oss << errorMsg(child.lineNumber, ErrorLevel::WARNING, "");
     }
     return oss.str();
 }
 
+std::string ErrorMessages::WARNING_SOMA_NON_CONTOUR() const {
+    return errorMsg(0,
+                    ErrorLevel::WARNING,
+                    "Soma must be a contour for ASC and H5: see "
+                    "https://github.com/BlueBrain/MorphIO/issues/457");
+}
+
+std::string ErrorMessages::WARNING_SOMA_NON_CYLINDER_OR_POINT() const {
+    return errorMsg(0,
+                    ErrorLevel::WARNING,
+                    "Soma must be stacked cylinders or a point: see "
+                    "https://github.com/BlueBrain/MorphIO/issues/457");
+}
+
+// LCOV_EXCL_STOP }
+
 }  // namespace readers
 
 }  // namespace morphio
```

### Comparing `MorphIO-3.3.5/src/mito_section.cpp` & `MorphIO-3.3.6/src/mito_section.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/mitochondria.cpp` & `MorphIO-3.3.6/src/mitochondria.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/morphology.cpp` & `MorphIO-3.3.6/src/morphology.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/mut/dendritic_spine.cpp` & `MorphIO-3.3.6/src/mut/dendritic_spine.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/mut/endoplasmic_reticulum.cpp` & `MorphIO-3.3.6/src/mut/endoplasmic_reticulum.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/mut/mito_section.cpp` & `MorphIO-3.3.6/src/mut/mito_section.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/mut/mitochondria.cpp` & `MorphIO-3.3.6/src/mut/mitochondria.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/mut/modifiers.cpp` & `MorphIO-3.3.6/src/mut/modifiers.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/mut/morphology.cpp` & `MorphIO-3.3.6/src/mut/morphology.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -388,18 +388,20 @@
 void Morphology::write(const std::string& filename) const {
     for (const auto& root : rootSections()) {
         if (root->points().size() < 2) {
             throw morphio::SectionBuilderError("Root sections must have at least 2 points");
         }
     }
 
-    std::string extension;
+    const size_t pos = filename.find_last_of('.');
+    if(pos == std::string::npos) {
+        throw UnknownFileType("Missing file extension.");
+    }
 
-    const size_t pos = filename.find_last_of(".");
-    assert(pos != std::string::npos);
+    std::string extension;
     for (char c : filename.substr(pos)) {
         extension += static_cast<char>(std::tolower(static_cast<unsigned char>(c)));
     }
 
     if (extension == ".h5") {
         writer::h5(*this, filename);
     } else if (extension == ".asc") {
```

### Comparing `MorphIO-3.3.5/src/mut/section.cpp` & `MorphIO-3.3.6/src/mut/section.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/mut/soma.cpp` & `MorphIO-3.3.6/src/mut/soma.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/mut/writers.cpp` & `MorphIO-3.3.6/src/mut/writers.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -100,14 +100,24 @@
 void swc(const Morphology& morphology, const std::string& filename) {
     const auto& soma = morphology.soma();
     const auto& soma_points = soma->points();
     if (soma_points.empty() && morphology.rootSections().empty()) {
         printError(Warning::WRITE_EMPTY_MORPHOLOGY,
                    readers::ErrorMessages().WARNING_WRITE_EMPTY_MORPHOLOGY());
         return;
+    } else if (!(soma->type() == SomaType::SOMA_NEUROMORPHO_THREE_POINT_CYLINDERS ||
+                 soma->type() == SomaType::SOMA_CYLINDERS ||
+                 soma->type() == SomaType::SOMA_SINGLE_POINT)) {
+        printError(Warning::SOMA_NON_CYLINDER_OR_POINT,
+                   readers::ErrorMessages().WARNING_SOMA_NON_CYLINDER_OR_POINT());
+    } else if (soma->type() == SomaType::SOMA_SINGLE_POINT && soma_points.size() != 1) {
+        throw WriterError(readers::ErrorMessages().ERROR_SOMA_INVALID_SINGLE_POINT());
+    } else if (soma->type() == SomaType::SOMA_NEUROMORPHO_THREE_POINT_CYLINDERS &&
+               soma_points.size() != 3) {
+        throw WriterError(readers::ErrorMessages().ERROR_SOMA_INVALID_THREE_POINT_CYLINDER());
     }
 
     checkSomaHasSameNumberPointsDiameters(*soma);
 
     if (hasPerimeterData(morphology)) {
         throw WriterError(readers::ErrorMessages().ERROR_PERIMETER_DATA_NOT_WRITABLE());
     }
@@ -206,18 +216,26 @@
         }
         myfile << indent << ")\n";
     }
 }
 
 void asc(const Morphology& morphology, const std::string& filename) {
     const auto& soma = morphology.soma();
+    const auto& somaPoints = soma->points();
+
     if (soma->points().empty() && morphology.rootSections().empty()) {
         printError(Warning::WRITE_EMPTY_MORPHOLOGY,
                    readers::ErrorMessages().WARNING_WRITE_EMPTY_MORPHOLOGY());
         return;
+    } else if (soma->type() != SomaType::SOMA_SIMPLE_CONTOUR) {
+        printError(Warning::SOMA_NON_CONTOUR, readers::ErrorMessages().WARNING_SOMA_NON_CONTOUR());
+    } else if (somaPoints.empty()) {
+        printError(Warning::WRITE_NO_SOMA, readers::ErrorMessages().WARNING_WRITE_NO_SOMA());
+    } else if (somaPoints.size() < 3) {
+        throw WriterError(readers::ErrorMessages().ERROR_SOMA_INVALID_CONTOUR());
     }
 
     checkSomaHasSameNumberPointsDiameters(*soma);
 
     if (hasPerimeterData(morphology)) {
         throw WriterError(readers::ErrorMessages().ERROR_PERIMETER_DATA_NOT_WRITABLE());
     }
@@ -234,16 +252,14 @@
     header[SECTION_DENDRITE] = "( (Color Red)\n  (Dendrite)\n";
     header[SECTION_APICAL_DENDRITE] = "( (Color Red)\n  (Apical)\n";
 
     if (!soma->points().empty()) {
         myfile << "(\"CellBody\"\n  (Color Red)\n  (CellBody)\n";
         _write_asc_points(myfile, soma->points(), soma->diameters(), 2);
         myfile << ")\n\n";
-    } else {
-        printError(Warning::WRITE_NO_SOMA, readers::ErrorMessages().WARNING_WRITE_NO_SOMA());
     }
 
     for (const std::shared_ptr<Section>& section : morphology.rootSections()) {
         // allowed types are only the ones available in the header
         if (header.count(section->type()) == 0) {
             throw WriterError(
                 readers::ErrorMessages().ERROR_UNSUPPORTED_SECTION_TYPE(section->type()));
@@ -363,23 +379,26 @@
     write_dataset(g_postsynaptic_density, "offset", offsets);
 }
 
 
 void h5(const Morphology& morpho, const std::string& filename) {
     const auto& soma = morpho.soma();
     const auto& somaPoints = soma->points();
-    const auto numberOfSomaPoints = somaPoints.size();
 
-    if (numberOfSomaPoints < 1) {
+    if (somaPoints.empty()) {
         if (morpho.rootSections().empty()) {
             printError(Warning::WRITE_EMPTY_MORPHOLOGY,
                        readers::ErrorMessages().WARNING_WRITE_EMPTY_MORPHOLOGY());
             return;
         }
         printError(Warning::WRITE_NO_SOMA, readers::ErrorMessages().WARNING_WRITE_NO_SOMA());
+    } else if (soma->type() != SomaType::SOMA_SIMPLE_CONTOUR) {
+        printError(Warning::SOMA_NON_CONTOUR, readers::ErrorMessages().WARNING_SOMA_NON_CONTOUR());
+    } else if (somaPoints.size() < 3) {
+        throw WriterError(readers::ErrorMessages().ERROR_SOMA_INVALID_CONTOUR());
     }
 
     checkSomaHasSameNumberPointsDiameters(*soma);
 
     HighFive::File h5_file(filename,
                            HighFive::File::ReadWrite | HighFive::File::Create |
                                HighFive::File::Truncate);
@@ -391,15 +410,15 @@
     std::vector<std::vector<int32_t>> raw_structure;
     std::vector<morphio::floatType> raw_perimeters;
 
     const auto& somaDiameters = soma->diameters();
 
     bool hasPerimeterData_ = hasPerimeterData(morpho);
 
-    for (unsigned int i = 0; i < numberOfSomaPoints; ++i) {
+    for (unsigned int i = 0; i < somaPoints.size(); ++i) {
         raw_points.push_back(
             {somaPoints[i][0], somaPoints[i][1], somaPoints[i][2], somaDiameters[i]});
 
         // If the morphology has some perimeter data, we need to fill some
         // perimeter dummy value in the soma range of the data structure to keep
         // the length matching
         if (hasPerimeterData_) {
```

### Comparing `MorphIO-3.3.5/src/point_utils.cpp` & `MorphIO-3.3.6/src/point_utils.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/point_utils.h` & `MorphIO-3.3.6/src/point_utils.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/properties.cpp` & `MorphIO-3.3.6/src/properties.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -3,88 +3,18 @@
 #include <morphio/errorMessages.h>
 #include <morphio/properties.h>
 #include <morphio/vector_types.h>
 
 #include "point_utils.h"
 #include "shared_utils.hpp"
 
-
 namespace morphio {
 namespace Property {
 
-PointLevel::PointLevel(std::vector<Point::Type> points,
-                       std::vector<Diameter::Type> diameters,
-                       std::vector<Perimeter::Type> perimeters)
-    : _points(std::move(points))
-    , _diameters(std::move(diameters))
-    , _perimeters(std::move(perimeters)) {
-    if (_points.size() != _diameters.size()) {
-        throw SectionBuilderError(
-            "Point vector have size: " + std::to_string(_points.size()) +
-            " while Diameter vector has size: " + std::to_string(_diameters.size()));
-    }
-
-    if (!_perimeters.empty() && _points.size() != _perimeters.size()) {
-        throw SectionBuilderError(
-            "Point vector have size: " + std::to_string(_points.size()) +
-            " while Perimeter vector has size: " + std::to_string(_perimeters.size()));
-    }
-}
-
-PointLevel::PointLevel(const PointLevel& data)
-    : PointLevel(data._points, data._diameters, data._perimeters) {}
-
-PointLevel::PointLevel(const PointLevel& data, SectionRange range) {
-    _points = copySpan<Property::Point>(data._points, range);
-    _diameters = copySpan<Property::Diameter>(data._diameters, range);
-    _perimeters = copySpan<Property::Perimeter>(data._perimeters, range);
-}
-
-PointLevel& PointLevel::operator=(const PointLevel& other) {
-    if (&other == this) {
-        return *this;
-    }
-
-    this->_points = other._points;
-    this->_diameters = other._diameters;
-    this->_perimeters = other._perimeters;
-    return *this;
-}
-
-template <typename T>
-bool compare(const std::vector<T>& vec1,
-             const std::vector<T>& vec2,
-             const std::string& name,
-             LogLevel logLevel) {
-    if (vec1 == vec2) {
-        return true;
-    }
-
-    if (vec1.size() != vec2.size()) {
-        if (logLevel > LogLevel::ERROR) {
-            printError(Warning::UNDEFINED,
-                       "Error comparing " + name + ", size differs: " +
-                           std::to_string(vec1.size()) + " vs " + std::to_string(vec2.size()));
-        }
-        return false;
-    }
-
-    if (logLevel > LogLevel::ERROR) {
-        printError(Warning::UNDEFINED, "Error comparing " + name + ", elements differ:");
-        for (unsigned int i = 0; i < vec1.size(); ++i) {
-            if (vec1[i] != vec2[i]) {
-                printError(Warning::UNDEFINED,
-                           valueToString(vec1[i]) + " <--> " + valueToString(vec2[i]));
-            }
-        }
-    }
-
-    return false;
-}
-
+namespace details {
 static bool compare_section_structure(const std::vector<Section::Type>& vec1,
                                       const std::vector<Section::Type>& vec2,
                                       const std::string& name,
                                       LogLevel logLevel) {
     if (vec1.size() != vec2.size()) {
         if (logLevel > LogLevel::ERROR) {
             printError(Warning::UNDEFINED,
@@ -107,122 +37,83 @@
             return false;
         }
     }
 
     return true;
 }
 
-template <typename T>
-bool compare(const morphio::range<T>& vec1,
-             const morphio::range<T>& vec2,
-             const std::string& name,
-             LogLevel logLevel) {
-    if (vec1.size() != vec2.size()) {
-        if (logLevel > LogLevel::ERROR) {
-            printError(Warning::UNDEFINED,
-                       "Error comparing " + name + ", size differs: " +
-                           std::to_string(vec1.size()) + " vs " + std::to_string(vec2.size()));
-        }
-        return false;
-    }
+}  // namespace details
 
-    for (unsigned int i = 0; i < vec1.size(); ++i) {
-        if (std::fabs(vec1[i] - vec2[i]) > morphio::epsilon) {
-            printError(Warning::UNDEFINED, "Error comparing " + name + ", elements differ:");
-            printError(Warning::UNDEFINED,
-                       valueToString(vec1[i]) + " <--> " + valueToString(vec2[i]));
-            printError(Warning::UNDEFINED, valueToString(subtract(vec2[i], vec1[i])));
-            return false;
-        }
-    }
-    return true;
-}
-
-template <>
-bool compare(const morphio::range<const morphio::Point>& vec1,
-             const morphio::range<const morphio::Point>& vec2,
-             const std::string& name,
-             LogLevel logLevel) {
-    if (vec1.size() != vec2.size()) {
-        if (logLevel > LogLevel::ERROR) {
-            printError(Warning::UNDEFINED,
-                       "Error comparing " + name + ", size differs: " +
-                           std::to_string(vec1.size()) + " vs " + std::to_string(vec2.size()));
-        }
-        return false;
+PointLevel::PointLevel(std::vector<Point::Type> points,
+                       std::vector<Diameter::Type> diameters,
+                       std::vector<Perimeter::Type> perimeters)
+    : _points(std::move(points))
+    , _diameters(std::move(diameters))
+    , _perimeters(std::move(perimeters)) {
+    if (_points.size() != _diameters.size()) {
+        throw SectionBuilderError(
+            "Point vector have size: " + std::to_string(_points.size()) +
+            " while Diameter vector has size: " + std::to_string(_diameters.size()));
     }
 
-    for (unsigned int i = 0; i < vec1.size(); ++i) {
-        if (std::fabs(euclidean_distance(vec1[i], vec2[i])) > morphio::epsilon) {
-            if (logLevel > LogLevel::ERROR) {
-                printError(Warning::UNDEFINED, "Error comparing " + name + ", elements differ:");
-                printError(Warning::UNDEFINED,
-                           valueToString(vec1[i]) + " <--> " + valueToString(vec2[i]));
-                printError(Warning::UNDEFINED, valueToString(subtract(vec2[i], vec1[i])));
-            }
-            return false;
-        }
+    if (!_perimeters.empty() && _points.size() != _perimeters.size()) {
+        throw SectionBuilderError(
+            "Point vector have size: " + std::to_string(_points.size()) +
+            " while Perimeter vector has size: " + std::to_string(_perimeters.size()));
     }
-    return true;
 }
 
-template <typename T, typename U>
-bool compare(const std::map<T, U>& vec1,
-             const std::map<T, U>& vec2,
-             const std::string& name,
-             LogLevel logLevel) {
-    if (vec1 == vec2) {
-        return true;
-    }
-    if (logLevel > LogLevel::ERROR) {
-        if (vec1.size() != vec2.size()) {
-            printError(Warning::UNDEFINED,
-                       "Error comparing " + name + ", size differs: " +
-                           std::to_string(vec1.size()) + " vs " + std::to_string(vec2.size()));
-        }
-    }
+PointLevel::PointLevel(const PointLevel& data)
+    : PointLevel(data._points, data._diameters, data._perimeters) {}
 
-    return false;
+PointLevel::PointLevel(const PointLevel& data, SectionRange range) {
+    _points = copySpan<Property::Point>(data._points, range);
+    _diameters = copySpan<Property::Diameter>(data._diameters, range);
+    _perimeters = copySpan<Property::Perimeter>(data._perimeters, range);
 }
 
-template <typename T>
-bool compare(const T& el1, const T& el2, const std::string& name, LogLevel logLevel) {
-    if (el1 == el2) {
-        return true;
+PointLevel& PointLevel::operator=(const PointLevel& other) {
+    if (&other == this) {
+        return *this;
     }
 
-    if (logLevel > LogLevel::ERROR) {
-        printError(Warning::UNDEFINED, name + " differs");
-    }
-    return false;
+    _points = other._points;
+    _diameters = other._diameters;
+    _perimeters = other._perimeters;
+
+    return *this;
 }
 
 bool SectionLevel::diff(const SectionLevel& other, LogLevel logLevel) const {
     return !(this == &other ||
-             (compare_section_structure(this->_sections, other._sections, "_sections", logLevel) &&
-              compare(this->_sectionTypes, other._sectionTypes, "_sectionTypes", logLevel) &&
-              compare(this->_children, other._children, "_children", logLevel)));
+             (details::compare_section_structure(
+                  this->_sections, other._sections, "_sections", logLevel) &&
+              morphio::property::compare(
+                  this->_sectionTypes, other._sectionTypes, "_sectionTypes", logLevel) &&
+              morphio::property::compare(this->_children, other._children, "_children", logLevel)));
 }
 
 bool SectionLevel::operator==(const SectionLevel& other) const {
     return !diff(other, LogLevel::ERROR);
 }
 
 bool SectionLevel::operator!=(const SectionLevel& other) const {
     return diff(other, LogLevel::ERROR);
 }
 
 bool CellLevel::diff(const CellLevel& other, LogLevel logLevel) const {
-    if (logLevel && this->_cellFamily != other._cellFamily) {
+    if (this == &other) {
+        return false;
+    }
+
+    if (logLevel > 0 && this->_cellFamily != other._cellFamily) {
         std::cout << "this->_cellFamily: " << this->_cellFamily << '\n'
                   << "other._cellFamily: " << other._cellFamily << '\n';
     }
-    return !(this == &other || (this->_cellFamily == other._cellFamily
-                                // this->_somaType == other._somaType
-                                ));
+    return !(this->_cellFamily == other._cellFamily && this->_somaType == other._somaType);
 }
 
 bool CellLevel::operator==(const CellLevel& other) const {
     return !diff(other, LogLevel::ERROR);
 }
 
 bool CellLevel::operator!=(const CellLevel& other) const {
@@ -259,52 +150,55 @@
             " while diameter vector has size: " + std::to_string(_diameters.size()));
     }
 }
 
 bool MitochondriaSectionLevel::diff(const MitochondriaSectionLevel& other,
                                     LogLevel logLevel) const {
     return !(this == &other ||
-             (compare_section_structure(this->_sections, other._sections, "_sections", logLevel) &&
-              compare(this->_children, other._children, "_children", logLevel)));
+             (details::compare_section_structure(
+                  this->_sections, other._sections, "_sections", logLevel) &&
+              morphio::property::compare(this->_children, other._children, "_children", logLevel)));
 }
 
 bool MitochondriaSectionLevel::operator==(const MitochondriaSectionLevel& other) const {
     return !diff(other, LogLevel::ERROR);
 }
 
 bool MitochondriaSectionLevel::operator!=(const MitochondriaSectionLevel& other) const {
     return diff(other, LogLevel::ERROR);
 }
 
 bool MitochondriaPointLevel::diff(const MitochondriaPointLevel& other, LogLevel logLevel) const {
     return !(this == &other ||
-             (compare(this->_sectionIds, other._sectionIds, "mito section ids", logLevel) &&
-              compare(this->_relativePathLengths,
-                      other._relativePathLengths,
-                      "mito relative pathlength",
-                      logLevel) &&
-              compare(this->_diameters, other._diameters, "mito section diameters", logLevel)));
+             (morphio::property::compare(
+                  this->_sectionIds, other._sectionIds, "mito section ids", logLevel) &&
+              morphio::property::compare(this->_relativePathLengths,
+                                         other._relativePathLengths,
+                                         "mito relative pathlength",
+                                         logLevel) &&
+              morphio::property::compare(
+                  this->_diameters, other._diameters, "mito section diameters", logLevel)));
 }
 
 bool MitochondriaPointLevel::operator==(const MitochondriaPointLevel& other) const {
     return !diff(other, LogLevel::ERROR);
 }
 
 bool MitochondriaPointLevel::operator!=(const MitochondriaPointLevel& other) const {
     return diff(other, LogLevel::ERROR);
 }
 
-std::ostream& operator<<(std::ostream& os, const PointLevel& prop) {
+std::ostream& operator<<(std::ostream& os, const PointLevel& pointLevel) {
     os << "Point level properties:\n"
        << "Point Diameter"
-       << (prop._perimeters.size() == prop._points.size() ? " Perimeter\n" : "\n");
-    for (unsigned int i = 0; i < prop._points.size(); ++i) {
-        os << dumpPoint(prop._points[i]) << ' ' << prop._diameters[i];
-        if (prop._perimeters.size() == prop._points.size()) {
-            os << ' ' << prop._perimeters[i];
+       << (pointLevel._perimeters.size() == pointLevel._points.size() ? " Perimeter\n" : "\n");
+    for (unsigned int i = 0; i < pointLevel._points.size(); ++i) {
+        os << dumpPoint(pointLevel._points[i]) << ' ' << pointLevel._diameters[i];
+        if (pointLevel._perimeters.size() == pointLevel._points.size()) {
+            os << ' ' << pointLevel._perimeters[i];
         }
         os << '\n';
     }
     return os;
 }
 
 std::ostream& operator<<(std::ostream& os, const Properties& properties) {
```

### Comparing `MorphIO-3.3.5/src/readers/NeurolucidaLexer.inc` & `MorphIO-3.3.6/src/readers/NeurolucidaLexer.inc`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/readers/morphologyASC.cpp` & `MorphIO-3.3.6/src/readers/morphologyASC.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/readers/morphologyHDF5.cpp` & `MorphIO-3.3.6/src/readers/morphologyHDF5.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/readers/morphologyHDF5.h` & `MorphIO-3.3.6/src/readers/morphologyHDF5.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/readers/morphologySWC.cpp` & `MorphIO-3.3.6/src/readers/morphologySWC.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,79 @@
 #include "morphologySWC.h"
 
+#include <algorithm>
 #include <cstdint>        // uint32_t
 #include <memory>         // std::shared_ptr
 #include <sstream>        // std::stringstream
 #include <string>         // std::string
 #include <unordered_map>  // std::unordered_map
 #include <vector>         // std::vector
 
 #include <morphio/errorMessages.h>
 #include <morphio/mut/morphology.h>
 #include <morphio/mut/section.h>
 #include <morphio/mut/soma.h>
 #include <morphio/properties.h>
 
 namespace {
+// It's not clear if -1 is the only way of identifying the root section.
+const int SWC_UNDEFINED_PARENT = -1;
+const unsigned int SWC_ROOT = 0xFFFFFFFD;
+
 bool _ignoreLine(const std::string& line) {
     std::size_t pos = line.find_first_not_of("\n\r\t ");
     return pos == std::string::npos || line[pos] == '#';
 }
 
 morphio::readers::Sample readSample(const char* line, unsigned int lineNumber_) {
 #ifdef MORPHIO_USE_DOUBLE
-    const char* const format = "%u%d%lg%lg%lg%lg%d";
+    const char* const format = "%d%d%lg%lg%lg%lg%d";
 #else
-    const char* const format = "%u%d%f%f%f%f%d";
+    const char* const format = "%d%d%f%f%f%f%d";
 #endif
 
     morphio::floatType radius = -1.;
     int int_type = -1;
     morphio::readers::Sample sample;
+    int parentId = -1;
+    int id = -1;
     sample.valid = sscanf(line,
                           format,
-                          &sample.id,
+                          &id,
                           &int_type,
                           &sample.point[0],
                           &sample.point[1],
                           &sample.point[2],
                           &radius,
-                          &sample.parentId) == 7;
+                          &parentId) == 7;
+
+    if (id < 0) {
+        throw morphio::RawDataError("Negative IDs are not supported");
+    }
+    sample.id = static_cast<unsigned int>(id);
+
+    if (parentId < -1) {
+        throw morphio::RawDataError("Negative ParentIDs are not supported");
+    } else if (parentId == SWC_UNDEFINED_PARENT) {
+        sample.parentId = SWC_ROOT;
+    } else {
+        sample.parentId = static_cast<unsigned int>(parentId);
+    }
 
     sample.type = static_cast<morphio::SectionType>(int_type);
     sample.diameter = radius * 2;  // The point array stores diameters.
     sample.lineNumber = lineNumber_;
     return sample;
 }
 
 }  // unnamed namespace
 
 namespace morphio {
 namespace readers {
 namespace swc {
-// It's not clear if -1 is the only way of identifying a root section.
-const int SWC_UNDEFINED_PARENT = -1;
-
 /**
    Parsing SWC according to this specification:
    http://www.neuronland.org/NLMorphologyConverter/MorphologyFormats/SWC/Spec.html
 **/
 class SWCBuilder
 {
   public:
@@ -89,67 +106,67 @@
                 throw RawDataError(err.ERROR_REPEATED_ID(samples[sample.id], sample));
             }
 
             samples[sample.id] = sample;
             children[sample.parentId].push_back(sample.id);
 
             if (sample.type == SECTION_SOMA) {
-                lastSomaPoint = static_cast<int>(sample.id);
+                lastSomaPoint = sample.id;
             }
         }
     }
 
     /**
        Are considered potential somata all sample
-       with parentId == -1 and sample.type == SECTION_SOMA
+       with parentId == SWC_ROOT and sample.type == SECTION_SOMA
      **/
     std::vector<Sample> _potentialSomata() {
         std::vector<Sample> somata;
-        for (auto id : children[-1]) {
+        for (auto id : children[SWC_ROOT]) {
             if (samples[id].type == SECTION_SOMA) {
                 somata.push_back(samples[id]);
             }
         }
         return somata;
     }
 
     void raiseIfBrokenSoma(const Sample& sample) {
         if (sample.type != SECTION_SOMA) {
             return;
         }
 
-        if (sample.parentId != -1 && !children[static_cast<int>(sample.id)].empty()) {
+        if (sample.parentId != SWC_ROOT && !children[sample.id].empty()) {
             std::vector<Sample> soma_bifurcations;
-            for (auto id : children[static_cast<int>(sample.id)]) {
+            for (unsigned int id : children[sample.id]) {
                 if (samples[id].type == SECTION_SOMA) {
                     soma_bifurcations.push_back(samples[id]);
                 } else {
                     neurite_wrong_root.push_back(samples[id]);
                 }
             }
 
             if (soma_bifurcations.size() > 1) {
                 throw morphio::SomaError(err.ERROR_SOMA_BIFURCATION(sample, soma_bifurcations));
             }
         }
 
-        if (sample.parentId != -1 &&
-            samples[static_cast<unsigned int>(sample.parentId)].type != SECTION_SOMA) {
+        if (sample.parentId != SWC_ROOT && samples.count(sample.parentId) > 0 &&
+            samples[sample.parentId].type != SECTION_SOMA) {
             throw morphio::SomaError(err.ERROR_SOMA_WITH_NEURITE_PARENT(sample));
         }
     }
 
     void raiseIfSelfParent(const Sample& sample) {
-        if (sample.parentId == static_cast<int>(sample.id)) {
+        if (sample.parentId == sample.id) {
             throw morphio::RawDataError(err.ERROR_SELF_PARENT(sample));
         }
     }
 
     void warnIfDisconnectedNeurite(const Sample& sample) {
-        if (sample.parentId == SWC_UNDEFINED_PARENT && sample.type != SECTION_SOMA) {
+        if (sample.parentId == SWC_ROOT && sample.type != SECTION_SOMA) {
             printError(Warning::DISCONNECTED_NEURITE, err.WARNING_DISCONNECTED_NEURITE(sample));
         }
     }
 
     void checkSoma() {
         auto somata = _potentialSomata();
 
@@ -164,67 +181,64 @@
                 const auto& sample = sample_pair.second;
                 warnIfDisconnectedNeurite(sample);
             }
         }
     }
 
     void raiseIfNoParent(const Sample& sample) {
-        if (sample.parentId > -1 &&
-            samples.count(static_cast<unsigned int>(sample.parentId)) == 0) {
+        if (sample.parentId != SWC_ROOT && samples.count(sample.parentId) == 0) {
             throw morphio::MissingParentError(err.ERROR_MISSING_PARENT(sample));
         }
     }
 
     void warnIfZeroDiameter(const Sample& sample) {
         if (sample.diameter < morphio::epsilon) {
             printError(Warning::ZERO_DIAMETER, err.WARNING_ZERO_DIAMETER(sample));
         }
     }
 
-    /**
-       A neurite which is not attached to the soma
-    **/
-    bool isOrphanNeurite(const Sample& sample) {
-        return (sample.parentId == SWC_UNDEFINED_PARENT && sample.type != SECTION_SOMA);
-    }
-
     bool isRootPoint(const Sample& sample) {
-        return isOrphanNeurite(sample) ||
+        bool isOrphanNeurite = sample.parentId == SWC_ROOT && sample.type != SECTION_SOMA;
+        return isOrphanNeurite ||
                (sample.type != SECTION_SOMA &&
-                samples[static_cast<unsigned int>(sample.parentId)].type ==
-                    SECTION_SOMA);  // Exclude soma bifurcations
+                samples[sample.parentId].type == SECTION_SOMA);  // Exclude soma bifurcations
     }
 
     bool isSectionStart(const Sample& sample) {
         return (isRootPoint(sample) ||
-                (sample.parentId > -1 &&
-                 isSectionEnd(samples[static_cast<unsigned int>(sample.parentId)])));  // Standard
-                                                                                       // section
+                (sample.parentId != SWC_ROOT &&
+                 isSectionEnd(samples[sample.parentId])));  // Standard section
     }
 
     bool isSectionEnd(const Sample& sample) {
-        int id = static_cast<int>(sample.id);
-        return id == lastSomaPoint ||        // End of soma
-               children[id].empty() ||       // Reached leaf
-               (children[id].size() >= 2 &&  // Reached neurite
-                                             // bifurcation
+        return sample.id == lastSomaPoint ||        // End of soma
+               children[sample.id].empty() ||       // Reached leaf
+               (children[sample.id].size() >= 2 &&  // Reached neurite bifurcation
                 sample.type != SECTION_SOMA);
     }
 
     template <typename T>
     void appendSample(const std::shared_ptr<T>& somaOrSection, const Sample& sample) {
         somaOrSection->points().push_back(sample.point);
         somaOrSection->diameters().push_back(sample.diameter);
     }
 
-    void _pushChildren(std::vector<unsigned int>& vec, int32_t id) {
-        for (unsigned int childId : children[id]) {
-            vec.push_back(childId);
-            _pushChildren(vec, static_cast<int>(childId));
-        }
+    std::vector<unsigned int> constructDepthFirstSamples() {
+        std::vector<unsigned int> ret;
+        ret.reserve(samples.size());
+        const auto pushChildren = [&](const auto& f, unsigned int id) -> void {
+            for (unsigned int childId : children[id]) {
+                ret.push_back(childId);
+                f(f, childId);
+            }
+        };
+
+        pushChildren(pushChildren, SWC_ROOT);
+
+        return ret;
     }
 
     void raiseIfNonConform(const Sample& sample) {
         raiseIfSelfParent(sample);
         raiseIfBrokenSoma(sample);
         raiseIfNoParent(sample);
         warnIfZeroDiameter(sample);
@@ -272,19 +286,19 @@
         }
         case 2: {
             return SOMA_CYLINDERS;
         }
         // NeuroMorpho format is characterized by a 3 points soma
         // with a bifurcation at soma root
         case 3: {
-            uint32_t somaRootId = children[-1][0];
-            auto& somaChildren = children[static_cast<int>(somaRootId)];
+            uint32_t somaRootId = children[SWC_ROOT][0];
+            const auto& somaChildren = children[somaRootId];
 
             std::vector<Sample> children_soma_points;
-            for (auto child : somaChildren) {
+            for (unsigned int child : somaChildren) {
                 if (this->samples[child].type == SECTION_SOMA) {
                     children_soma_points.push_back(this->samples[child]);
                 }
             }
 
             if (children_soma_points.size() == 2) {
                 //  NeuroMorpho is the main provider of morphologies, but they
@@ -317,16 +331,15 @@
         checkSoma();
 
         // The process might occasionally creates empty section before
         // filling them so the warning is ignored
         bool originalIsIgnored = err.isIgnored(morphio::Warning::APPENDING_EMPTY_SECTION);
         set_ignored_warning(morphio::Warning::APPENDING_EMPTY_SECTION, true);
 
-        std::vector<unsigned int> depthFirstSamples;
-        _pushChildren(depthFirstSamples, -1);
+        std::vector<unsigned int> depthFirstSamples = constructDepthFirstSamples();
         for (const auto id : depthFirstSamples) {
             const Sample& sample = samples[id];
 
             // Bifurcation right at the start
             if (isRootPoint(sample) && isSectionEnd(sample)) {
                 continue;
             }
@@ -396,17 +409,17 @@
     // Dictionary: SWC Id of the last point of a section to morphio::mut::Section ID
     std::unordered_map<uint32_t, uint32_t> swcIdToSectionId;
 
     // Neurite that do not have parent ID = 1, allowed for soma contour, not
     // 3-pts soma
     std::vector<Sample> neurite_wrong_root;
 
-    int lastSomaPoint = -1;
-    std::unordered_map<int32_t, std::vector<uint32_t>> children;
-    std::unordered_map<uint32_t, Sample> samples;
+    unsigned int lastSomaPoint = 0;
+    std::unordered_map<unsigned int, std::vector<unsigned int>> children;
+    std::unordered_map<unsigned int, Sample> samples;
     mut::Morphology morph;
     ErrorMessages err;
 };
 
 Property::Properties load(const std::string& path,
                           const std::string& contents,
                           unsigned int options) {
```

### Comparing `MorphIO-3.3.5/src/readers/vasculatureHDF5.cpp` & `MorphIO-3.3.6/src/readers/vasculatureHDF5.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/readers/vasculatureHDF5.h` & `MorphIO-3.3.6/src/readers/vasculatureHDF5.h`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/section.cpp` & `MorphIO-3.3.6/src/section.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/soma.cpp` & `MorphIO-3.3.6/src/soma.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #include <morphio/section.h>
 #include <morphio/soma.h>
 #include <morphio/vector_types.h>
+#include <stdexcept>
 
 #include "point_utils.h"
 #include "shared_utils.hpp"
 
 namespace morphio {
 Soma::Soma(const std::shared_ptr<Property::Properties>& properties)
     : properties_(properties) {}
@@ -21,15 +22,15 @@
     }
 
     case SOMA_SINGLE_POINT:
     case SOMA_CYLINDERS:
     case SOMA_SIMPLE_CONTOUR:
     case SOMA_UNDEFINED:
     default:
-        throw;
+        throw std::runtime_error("Volume is not supported");
     }
 }
 
 floatType Soma::surface() const {
     return _somaSurface(type(), diameters(), points());
 }
```

### Comparing `MorphIO-3.3.5/src/vasc/section.cpp` & `MorphIO-3.3.6/src/vasc/section.cpp`

 * *Files identical despite different names*

### Comparing `MorphIO-3.3.5/src/vasc/vasculature.cpp` & `MorphIO-3.3.6/src/vasc/vasculature.cpp`

 * *Files identical despite different names*

