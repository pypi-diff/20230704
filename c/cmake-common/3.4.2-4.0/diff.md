# Comparing `tmp/cmake_common-3.4.2.tar.gz` & `tmp/cmake_common-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmake_common-3.4.2.tar", last modified: Thu Mar  2 23:11:21 2023, max compression
+gzip compressed data, was "cmake_common-4.0.tar", last modified: Tue Jul  4 00:05:28 2023, max compression
```

## Comparing `cmake_common-3.4.2.tar` & `cmake_common-4.0.tar`

### file list

```diff
@@ -1,117 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.595240 cmake_common-3.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.587240 cmake_common-3.4.2/.ci/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.ci/run_foo.ps1
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.ci/verify_arch.ps1
--rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.ci/verify_arch.sh
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.ci/verify_symbols.ps1
--rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.ci/verify_symbols.sh
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.583240 cmake_common-3.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.583240 cmake_common-3.4.2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.587240 cmake_common-3.4.2/.github/actions/build-boost/
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/actions/build-boost/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.587240 cmake_common-3.4.2/.github/actions/build-example/
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/actions/build-example/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.587240 cmake_common-3.4.2/.github/actions/check-arch/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/actions/check-arch/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.587240 cmake_common-3.4.2/.github/actions/check-boost-bootstrapped/
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/actions/check-boost-bootstrapped/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.587240 cmake_common-3.4.2/.github/actions/check-boost-download/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/actions/check-boost-download/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.587240 cmake_common-3.4.2/.github/actions/check-boost-libraries/
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/actions/check-boost-libraries/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.587240 cmake_common-3.4.2/.github/actions/check-runtime-library/
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/actions/check-runtime-library/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.587240 cmake_common-3.4.2/.github/actions/check-symbols/
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/actions/check-symbols/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.587240 cmake_common-3.4.2/.github/actions/common-variables/
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/actions/common-variables/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.587240 cmake_common-3.4.2/.github/actions/download-boost/
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/actions/download-boost/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.587240 cmake_common-3.4.2/.github/actions/run-example/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/actions/run-example/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.587240 cmake_common-3.4.2/.github/actions/run-example-boost/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/actions/run-example-boost/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.587240 cmake_common-3.4.2/.github/actions/software-environment/
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/actions/software-environment/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.587240 cmake_common-3.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/workflows/basic.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/workflows/boost_clang_windows.yml
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/workflows/boost_download.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/workflows/boost_toolsets.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/workflows/ci_appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/workflows/ci_github.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/workflows/ci_travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/workflows/cygwin_static_libstdc++.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/workflows/example_toolsets.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.github/workflows/msvc_versions.yml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-02 23:11:08.000000 cmake_common-3.4.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-02 23:11:08.000000 cmake_common-3.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-03-02 23:11:21.595240 cmake_common-3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-03-02 23:11:08.000000 cmake_common-3.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.591240 cmake_common-3.4.2/cmake_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-03-02 23:11:21.000000 cmake_common-3.4.2/cmake_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-03-02 23:11:21.000000 cmake_common-3.4.2/cmake_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 23:11:21.000000 cmake_common-3.4.2/cmake_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-02 23:11:21.000000 cmake_common-3.4.2/cmake_common.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-02 23:11:21.000000 cmake_common-3.4.2/cmake_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-02 23:11:21.000000 cmake_common-3.4.2/cmake_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-03-02 23:11:08.000000 cmake_common-3.4.2/common.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.591240 cmake_common-3.4.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-03-02 23:11:08.000000 cmake_common-3.4.2/docs/boost.md
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-03-02 23:11:08.000000 cmake_common-3.4.2/docs/ci.md
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-03-02 23:11:08.000000 cmake_common-3.4.2/docs/cmake.md
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-03-02 23:11:08.000000 cmake_common-3.4.2/docs/ctest-driver.md
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-02 23:11:08.000000 cmake_common-3.4.2/docs/project-clang-format.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.583240 cmake_common-3.4.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.591240 cmake_common-3.4.2/examples/boost/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-02 23:11:08.000000 cmake_common-3.4.2/examples/boost/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-02 23:11:08.000000 cmake_common-3.4.2/examples/boost/foo.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.591240 cmake_common-3.4.2/examples/dynamic/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-02 23:11:08.000000 cmake_common-3.4.2/examples/dynamic/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-02 23:11:08.000000 cmake_common-3.4.2/examples/dynamic/baz.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-02 23:11:08.000000 cmake_common-3.4.2/examples/dynamic/baz.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-02 23:11:08.000000 cmake_common-3.4.2/examples/dynamic/foo.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.591240 cmake_common-3.4.2/examples/simple/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-02 23:11:08.000000 cmake_common-3.4.2/examples/simple/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-02 23:11:08.000000 cmake_common-3.4.2/examples/simple/foo.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.591240 cmake_common-3.4.2/examples/static/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-03-02 23:11:08.000000 cmake_common-3.4.2/examples/static/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-02 23:11:08.000000 cmake_common-3.4.2/examples/static/bar.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-02 23:11:08.000000 cmake_common-3.4.2/examples/static/bar.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-02 23:11:08.000000 cmake_common-3.4.2/examples/static/foo.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.591240 cmake_common-3.4.2/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.591240 cmake_common-3.4.2/project/boost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/boost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/boost/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/boost/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/boost/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/boost/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/boost/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.595240 cmake_common-3.4.2/project/ci/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/ci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.595240 cmake_common-3.4.2/project/ci/appveyor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/ci/appveyor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/ci/appveyor/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/ci/boost.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/ci/cmake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/ci/dirs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.595240 cmake_common-3.4.2/project/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/cmake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/cmake/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/linkage.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/mingw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/os.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)    21866 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/toolset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-02 23:11:08.000000 cmake_common-3.4.2/project/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-03-02 23:11:08.000000 cmake_common-3.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 23:11:21.595240 cmake_common-3.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 23:11:21.595240 cmake_common-3.4.2/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5254 2023-03-02 23:11:08.000000 cmake_common-3.4.2/tools/ctest-driver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5360 2023-03-02 23:11:08.000000 cmake_common-3.4.2/tools/project-clang-format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.700981 cmake_common-4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.676978 cmake_common-4.0/.ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-04 00:05:03.000000 cmake_common-4.0/.ci/run_foo.ps1
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-04 00:05:03.000000 cmake_common-4.0/.ci/verify_arch.ps1
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-07-04 00:05:03.000000 cmake_common-4.0/.ci/verify_arch.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-04 00:05:03.000000 cmake_common-4.0/.ci/verify_symbols.ps1
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-07-04 00:05:03.000000 cmake_common-4.0/.ci/verify_symbols.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-04 00:05:03.000000 cmake_common-4.0/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-04 00:05:03.000000 cmake_common-4.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.668978 cmake_common-4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.668978 cmake_common-4.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.676978 cmake_common-4.0/.github/actions/build-boost/
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-04 00:05:03.000000 cmake_common-4.0/.github/actions/build-boost/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.676978 cmake_common-4.0/.github/actions/build-example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-04 00:05:03.000000 cmake_common-4.0/.github/actions/build-example/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.676978 cmake_common-4.0/.github/actions/check-arch/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-04 00:05:03.000000 cmake_common-4.0/.github/actions/check-arch/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.676978 cmake_common-4.0/.github/actions/check-boost-bootstrapped/
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-04 00:05:03.000000 cmake_common-4.0/.github/actions/check-boost-bootstrapped/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.676978 cmake_common-4.0/.github/actions/check-boost-download/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-04 00:05:03.000000 cmake_common-4.0/.github/actions/check-boost-download/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.680979 cmake_common-4.0/.github/actions/check-boost-libraries/
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-04 00:05:03.000000 cmake_common-4.0/.github/actions/check-boost-libraries/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.680979 cmake_common-4.0/.github/actions/check-runtime-library/
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-04 00:05:03.000000 cmake_common-4.0/.github/actions/check-runtime-library/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.680979 cmake_common-4.0/.github/actions/check-symbols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-04 00:05:03.000000 cmake_common-4.0/.github/actions/check-symbols/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.680979 cmake_common-4.0/.github/actions/common-variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-04 00:05:03.000000 cmake_common-4.0/.github/actions/common-variables/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.680979 cmake_common-4.0/.github/actions/download-boost/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-04 00:05:03.000000 cmake_common-4.0/.github/actions/download-boost/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.680979 cmake_common-4.0/.github/actions/run-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-04 00:05:03.000000 cmake_common-4.0/.github/actions/run-example/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.680979 cmake_common-4.0/.github/actions/run-example-boost/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-04 00:05:03.000000 cmake_common-4.0/.github/actions/run-example-boost/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.680979 cmake_common-4.0/.github/actions/software-environment/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-04 00:05:03.000000 cmake_common-4.0/.github/actions/software-environment/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.684979 cmake_common-4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-04 00:05:03.000000 cmake_common-4.0/.github/workflows/basic.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-07-04 00:05:03.000000 cmake_common-4.0/.github/workflows/boost_clang_windows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-04 00:05:03.000000 cmake_common-4.0/.github/workflows/boost_download.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-04 00:05:03.000000 cmake_common-4.0/.github/workflows/boost_toolsets.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-04 00:05:03.000000 cmake_common-4.0/.github/workflows/cygwin_static_libstdc++.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-04 00:05:03.000000 cmake_common-4.0/.github/workflows/example_toolsets.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-04 00:05:03.000000 cmake_common-4.0/.github/workflows/msvc_versions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-04 00:05:03.000000 cmake_common-4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-04 00:05:03.000000 cmake_common-4.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-04 00:05:03.000000 cmake_common-4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-07-04 00:05:28.700981 cmake_common-4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-04 00:05:03.000000 cmake_common-4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.688979 cmake_common-4.0/cmake_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-07-04 00:05:28.000000 cmake_common-4.0/cmake_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-04 00:05:28.000000 cmake_common-4.0/cmake_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 00:05:28.000000 cmake_common-4.0/cmake_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 00:05:28.000000 cmake_common-4.0/cmake_common.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-04 00:05:28.000000 cmake_common-4.0/cmake_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 00:05:28.000000 cmake_common-4.0/cmake_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-07-04 00:05:03.000000 cmake_common-4.0/common.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.688979 cmake_common-4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-04 00:05:03.000000 cmake_common-4.0/docs/boost.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-07-04 00:05:03.000000 cmake_common-4.0/docs/cmake.md
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-04 00:05:03.000000 cmake_common-4.0/docs/ctest-driver.md
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-04 00:05:03.000000 cmake_common-4.0/docs/project-clang-format.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.668978 cmake_common-4.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.688979 cmake_common-4.0/examples/boost/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-04 00:05:03.000000 cmake_common-4.0/examples/boost/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-04 00:05:03.000000 cmake_common-4.0/examples/boost/foo.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.692980 cmake_common-4.0/examples/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-04 00:05:03.000000 cmake_common-4.0/examples/dynamic/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-04 00:05:03.000000 cmake_common-4.0/examples/dynamic/baz.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-04 00:05:03.000000 cmake_common-4.0/examples/dynamic/baz.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-04 00:05:03.000000 cmake_common-4.0/examples/dynamic/foo.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.692980 cmake_common-4.0/examples/simple/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-04 00:05:03.000000 cmake_common-4.0/examples/simple/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-04 00:05:03.000000 cmake_common-4.0/examples/simple/foo.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.692980 cmake_common-4.0/examples/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-04 00:05:03.000000 cmake_common-4.0/examples/static/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-04 00:05:03.000000 cmake_common-4.0/examples/static/bar.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-04 00:05:03.000000 cmake_common-4.0/examples/static/bar.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-04 00:05:03.000000 cmake_common-4.0/examples/static/foo.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.696980 cmake_common-4.0/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:03.000000 cmake_common-4.0/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.700981 cmake_common-4.0/project/boost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:03.000000 cmake_common-4.0/project/boost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-04 00:05:03.000000 cmake_common-4.0/project/boost/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-07-04 00:05:03.000000 cmake_common-4.0/project/boost/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-04 00:05:03.000000 cmake_common-4.0/project/boost/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-07-04 00:05:03.000000 cmake_common-4.0/project/boost/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-04 00:05:03.000000 cmake_common-4.0/project/boost/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-07-04 00:05:03.000000 cmake_common-4.0/project/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-04 00:05:03.000000 cmake_common-4.0/project/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-04 00:05:03.000000 cmake_common-4.0/project/linkage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-04 00:05:03.000000 cmake_common-4.0/project/mingw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-04 00:05:03.000000 cmake_common-4.0/project/os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-04 00:05:03.000000 cmake_common-4.0/project/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21852 2023-07-04 00:05:03.000000 cmake_common-4.0/project/toolset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-04 00:05:03.000000 cmake_common-4.0/project/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-04 00:05:03.000000 cmake_common-4.0/project/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-04 00:05:03.000000 cmake_common-4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 00:05:28.700981 cmake_common-4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:05:28.700981 cmake_common-4.0/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5254 2023-07-04 00:05:03.000000 cmake_common-4.0/tools/ctest-driver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5360 2023-07-04 00:05:03.000000 cmake_common-4.0/tools/project-clang-format.py
```

### Comparing `cmake_common-3.4.2/.ci/verify_arch.ps1` & `cmake_common-4.0/.ci/verify_arch.ps1`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/.ci/verify_arch.sh` & `cmake_common-4.0/.ci/verify_arch.sh`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/.ci/verify_symbols.sh` & `cmake_common-4.0/.ci/verify_symbols.sh`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/.github/actions/build-boost/action.yml` & `cmake_common-4.0/.github/actions/build-boost/action.yml`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/.github/actions/build-example/action.yml` & `cmake_common-4.0/.github/actions/build-example/action.yml`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,17 @@
     description: Target platform
     required: false
     default: x64
   configuration:
     description: Configuration to build
     required: false
     default: Debug
+  cmake-args:
+    description: Additional CMake arguments
+    required: false
 outputs:
   install-dir:
     description: Installation directory
     value: '${{ steps.install-dir.outputs.path }}'
 runs:
   using: composite
   steps:
@@ -59,11 +62,11 @@
             '${{ inputs.toolset }}'
         )
 
         if ($boost_dir) {
             $args += '--boost',$boost_dir
         }
 
-        $args += '--',$src_dir
+        $args += '--',$src_dir,'TMP'
         $env:VERBOSE = 1
-        & $python -m project.cmake.build $args
+        & $python -m project.build $args ${{ inputs.cmake-args }}
       shell: pwsh
```

### Comparing `cmake_common-3.4.2/.github/actions/check-arch/action.yml` & `cmake_common-4.0/.github/actions/check-arch/action.yml`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/.github/actions/check-boost-bootstrapped/action.yml` & `cmake_common-4.0/.github/actions/check-boost-bootstrapped/action.yml`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/.github/actions/check-boost-download/action.yml` & `cmake_common-4.0/.github/actions/check-boost-download/action.yml`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/.github/actions/check-boost-libraries/action.yml` & `cmake_common-4.0/.github/actions/check-boost-libraries/action.yml`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/.github/actions/check-symbols/action.yml` & `cmake_common-4.0/.github/actions/check-symbols/action.yml`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/.github/actions/common-variables/action.yml` & `cmake_common-4.0/.github/actions/common-variables/action.yml`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/.github/actions/download-boost/action.yml` & `cmake_common-4.0/.github/actions/download-boost/action.yml`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/.github/actions/run-example/action.yml` & `cmake_common-4.0/.github/actions/run-example/action.yml`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/.github/actions/run-example-boost/action.yml` & `cmake_common-4.0/.github/actions/run-example-boost/action.yml`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/.github/actions/software-environment/action.yml` & `cmake_common-4.0/.github/actions/software-environment/action.yml`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/.github/workflows/basic.yml` & `cmake_common-4.0/.github/workflows/basic.yml`

 * *Files 3% similar despite different names*

```diff
@@ -44,20 +44,20 @@
       - name: Cache Boost
         uses: actions/cache@v3
         with:
           path: boost_*.tar.gz
           key: 'boost_${{ matrix.boost-version }}'
       - name: Build Boost
         run: |
-          python -m project.boost.download --cache . '${{ matrix.boost-version }}' boost
-          python -m project.boost.build -- boost --with-filesystem
+          python -m project.boost.download --cache . '${{ matrix.boost-version }}' boost/
+          python -m project.boost.build -- boost/ --with-filesystem
       - name: Build example project
         run: |
           $src_dir = Join-Path examples boost
-          python -m project.cmake.build --boost boost --install install -- $src_dir
+          python -m project.build --boost boost/ --install install/ -- $src_dir build/
       - name: Run example project
         run: ./.ci/run_foo.ps1 (Join-Path (Get-Location).Path install bin foo)
 
   # Check that the most basic use-case works w/ different Python versions.
   python-versions:
     strategy:
       matrix:
@@ -86,23 +86,23 @@
           key: 'boost_${{ matrix.boost-version }}'
       - name: 'Install package & dependencies'
         run: pip install -q -e .
       - name: Check that scripts are runnable
         run: |
           boost-download --version
           boost-build --version
-          cmake-build --version
+          project-build --version
       - name: Build Boost
         run: |
-          boost-download --cache . '${{ matrix.boost-version }}' boost
-          boost-build -- boost --with-filesystem
+          boost-download --cache . '${{ matrix.boost-version }}' boost/
+          boost-build -- boost/ --with-filesystem
       - name: Build example project
         run: |
           $src_dir = Join-Path examples boost
-          cmake-build --boost boost --install install -- $src_dir
+          project-build --boost boost/ --install install/ -- $src_dir build/
       - name: Run example project
         run: ./.ci/run_foo.ps1 (Join-Path (Get-Location).Path install bin foo)
 
   # Build a Python package and upload to PyPI.
   publish:
     # TODO: figure out how to add a dependency on the *toolsets workflows.
     needs: [lint, os, python-versions]
```

### Comparing `cmake_common-3.4.2/.github/workflows/boost_clang_windows.yml` & `cmake_common-4.0/.github/workflows/boost_clang_windows.yml`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/.github/workflows/boost_download.yml` & `cmake_common-4.0/.github/workflows/boost_download.yml`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/.github/workflows/boost_toolsets.yml` & `cmake_common-4.0/.github/workflows/boost_toolsets.yml`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,16 @@
         uses: ./.github/actions/build-example
         with:
           src-dir: examples/boost
           boost-dir: '${{ env.BOOST_DIR }}'
           toolset: '${{ matrix.toolset }}'
           platform: '${{ matrix.platform }}'
           configuration: '${{ matrix.configuration }}'
+          # Older Boosts don't like the newer standards (auto_ptr, etc.)
+          cmake-args: -D CC_CXX_STANDARD=14
 
       - name: Verify runtime library linkage
         uses: ./.github/actions/check-runtime-library
         with:
           path: '${{ steps.build_example.outputs.install-dir }}'
 
       - name: Verify architecture
```

### Comparing `cmake_common-3.4.2/.github/workflows/cygwin_static_libstdc++.yml` & `cmake_common-4.0/.github/workflows/cygwin_static_libstdc++.yml`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/.github/workflows/example_toolsets.yml` & `cmake_common-4.0/.github/workflows/example_toolsets.yml`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/.github/workflows/msvc_versions.yml` & `cmake_common-4.0/.github/workflows/msvc_versions.yml`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/LICENSE.txt` & `cmake_common-4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/README.md` & `cmake_common-4.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,42 @@
+Metadata-Version: 2.1
+Name: cmake_common
+Version: 4.0
+Summary: Utilities to help develop C++/CMake projects
+Author-email: Egor Tensin <Egor.Tensin@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/egor-tensin/cmake-common
+Project-URL: Bug Tracker, https://github.com/egor-tensin/cmake-common/issues
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: C++
+Classifier: Topic :: Software Development :: Build Tools
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 cmake-common
 ============
 
 [![Basic usage](https://github.com/egor-tensin/cmake-common/actions/workflows/basic.yml/badge.svg)](https://github.com/egor-tensin/cmake-common/actions/workflows/basic.yml)
 [![Boost (toolsets)](https://github.com/egor-tensin/cmake-common/actions/workflows/boost_toolsets.yml/badge.svg)](https://github.com/egor-tensin/cmake-common/actions/workflows/boost_toolsets.yml)
 [![Examples (toolsets)](https://github.com/egor-tensin/cmake-common/actions/workflows/example_toolsets.yml/badge.svg)](https://github.com/egor-tensin/cmake-common/actions/workflows/example_toolsets.yml)
 
 Utilities to help develop C++/CMake projects.
 
+Description
+-----------
+
+This main goal of this project is to make it easier to build (potentially,
+cross-compile) Boost and CMake projects using different toolsets.
+It does so providing a set of command-line utilities that allow users to
+download/build Boost & use it in a CMake project in a consistent way &mdash; no
+matter the compiler or the target platform.
+
 Installation
 ------------
 
 * Via PyPI:
 
       pip install cmake-common
 
@@ -21,17 +47,15 @@
   All the scripts provided by the PyPI package are thin wrappers around the
   `project` package modules:
 
   | Script         | Module
   | -------------- | ------
   | boost-download | `python3 -m project.boost.download`
   | boost-build    | `python3 -m project.boost.build`
-  | cmake-build    | `python3 -m project.cmake.build`
-  | ci-boost       | `python3 -m project.ci.boost`
-  | ci-cmake       | `python3 -m project.ci.cmake`
+  | project-build  | `python3 -m project.build`
 
 Toolsets
 --------
 
 Supported platform/build system/compiler combinations include, but are not
 limited to:
 
@@ -50,15 +74,15 @@
 1. Both GNU make and MinGW mingw32-make.
 2. clang-cl is supported by Boost 1.69.0 or higher only.
 
 All of those are verified continuously by the [Boost (toolsets)] and [Examples
 (toolsets)] workflows.
 
 For a complete list of possible `--toolset` parameter values, pass the
-`--help-toolsets` flag to either `boost-build` or `cmake-build`.
+`--help-toolsets` flag to either `boost-build` or `project-build`.
 
 [Boost (toolsets)]: https://github.com/egor-tensin/cmake-common/actions/workflows/boost_toolsets.yml
 [Examples (toolsets)]: https://github.com/egor-tensin/cmake-common/actions/workflows/example_toolsets.yml
 
 Usage
 -----
 
@@ -74,15 +98,15 @@
 
 Pass the `--help` flag to view detailed usage information.
 
 ### CMake project
 
 Build (and optionally, install) a CMake project.
 
-    $ cmake-build --configuration Release --install path/to/somewhere --boost path/to/boost -- examples/simple
+    $ project-build --configuration Release --install path/to/somewhere --boost path/to/boost -- examples/simple build/
     ...
 
     $ ./path/to/somewhere/bin/foo
     foo
 
 Pass the `--help` flag to view detailed usage information.
 
@@ -93,39 +117,18 @@
     include(path/to/common.cmake)
 
 in CMakeLists.txt.
 
 This file aids in quick-and-dirty development by
 
 * linking everything (including the runtime) statically by default,
-* setting some useful compilation options (enables warnings, defines useful
+* setting some useful compilation options (enables warnings, defines common
 Windows-specific macros, strips debug symbols in release builds, etc.).
 
-Everything is optional (use the `CC_*` CMake options to opt out).
-
-### CI
-
-Utility scripts `ci-boost` and `ci-cmake` allow building Boost and CMake
-projects on multiple CI systems.
-They work by calling the generic scripts from above, auto-filling some
-parameters from environment variables.
-
-|                   | Travis                               | AppVeyor                                   | GitHub Actions
-| ----------------- | ------------------------------------ | ------------------------------------------ | --------------
-| `--toolset`       | `$TOOLSET`                           | `%TOOLSET%`                                | `$TOOLSET`
-| `--platform`      | `$PLATFORM`                          | `%PLATFORM%`                               | `$PLATFORM`
-| `--configuration` | `$CONFIGURATION`                     | `%CONFIGURATION%`                          | `$CONFIGURATION`
-| Boost version     | `$BOOST_VERSION`                     | `%BOOST_VERSION%`                          | `$BOOST_VERSION`
-| Boost path        | `$TRAVIS_BUILD_DIR/../build/boost`   | `%APPVEYOR_BUILD_FOLDER%\..\build\boost`   | `$GITHUB_WORKSPACE/../build/boost`
-| Build path        | `$TRAVIS_BUILD_DIR/../build/cmake`   | `%APPVEYOR_BUILD_FOLDER%\..\build\cmake`   | `$GITHUB_WORKSPACE/../build/cmake`
-| Install path      | `$TRAVIS_BUILD_DIR/../build/install` | `%APPVEYOR_BUILD_FOLDER%\..\build\install` | `$GITHUB_WORKSPACE/../build/install`
-
-
-For an example of how to integrate `ci-boost` and `ci-cmake` into a CI
-workflow, see [docs/ci.md](docs/ci.md).
+Everything is enabled by default (use the `CC_*` CMake options to opt out).
 
 Tools
 -----
 
 * [project-clang-format.py] &mdash; `clang-format` all C/C++ files in the
 project.
 * [ctest-driver.py] &mdash; wrap an executable for testing with CTest;
```

### Comparing `cmake_common-3.4.2/cmake_common.egg-info/SOURCES.txt` & `cmake_common-4.0/cmake_common.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -24,28 +24,24 @@
 .github/actions/run-example/action.yml
 .github/actions/run-example-boost/action.yml
 .github/actions/software-environment/action.yml
 .github/workflows/basic.yml
 .github/workflows/boost_clang_windows.yml
 .github/workflows/boost_download.yml
 .github/workflows/boost_toolsets.yml
-.github/workflows/ci_appveyor.yml
-.github/workflows/ci_github.yml
-.github/workflows/ci_travis.yml
 .github/workflows/cygwin_static_libstdc++.yml
 .github/workflows/example_toolsets.yml
 .github/workflows/msvc_versions.yml
 cmake_common.egg-info/PKG-INFO
 cmake_common.egg-info/SOURCES.txt
 cmake_common.egg-info/dependency_links.txt
 cmake_common.egg-info/entry_points.txt
 cmake_common.egg-info/requires.txt
 cmake_common.egg-info/top_level.txt
 docs/boost.md
-docs/ci.md
 docs/cmake.md
 docs/ctest-driver.md
 docs/project-clang-format.md
 examples/boost/CMakeLists.txt
 examples/boost/foo.cpp
 examples/dynamic/CMakeLists.txt
 examples/dynamic/baz.cpp
@@ -54,31 +50,24 @@
 examples/simple/CMakeLists.txt
 examples/simple/foo.cpp
 examples/static/CMakeLists.txt
 examples/static/bar.cpp
 examples/static/bar.hpp
 examples/static/foo.cpp
 project/__init__.py
+project/build.py
 project/configuration.py
 project/linkage.py
 project/mingw.py
 project/os.py
 project/platform.py
 project/toolset.py
 project/utils.py
 project/version.py
 project/boost/__init__.py
 project/boost/archive.py
 project/boost/build.py
 project/boost/directory.py
 project/boost/download.py
 project/boost/version.py
-project/ci/__init__.py
-project/ci/boost.py
-project/ci/cmake.py
-project/ci/dirs.py
-project/ci/appveyor/__init__.py
-project/ci/appveyor/generator.py
-project/cmake/__init__.py
-project/cmake/build.py
 tools/ctest-driver.py
 tools/project-clang-format.py
```

### Comparing `cmake_common-3.4.2/common.cmake` & `cmake_common-4.0/common.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # It's a CMake code snippet I use in all of my CMake projects.
 # It makes targets link the runtime statically by default, strips debug symbols
 # in release builds and sets a couple of useful compilation options.
 
 # Add this to the top-level CMakeLists.txt (unless a higher version has already
 # been specified):
 #
-#     cmake_minimum_required(VERSION 3.1)
+#     cmake_minimum_required(VERSION 3.8)
 
 # Without this policy set, this line:
 #
 #     if(toolset STREQUAL "MSVC")
 #
 # evaluates to false even when using Visual Studio (since MSVC is a predefined
 # variable; it's completely bonkers).
@@ -50,21 +50,21 @@
 set(default_value ON)
 get_directory_property(parent_dir PARENT_DIRECTORY)
 if(parent_dir)
     set(default_value OFF)
 endif()
 
 if(NOT DEFINED CC_CXX_STANDARD)
-    set(CC_CXX_STANDARD "14" CACHE STRING "C++ standard version")
+    set(CC_CXX_STANDARD "17" CACHE STRING "C++ standard version")
 endif()
-if(NOT DEFINED CC_BEST_PRACTICES)
-    option(CC_BEST_PRACTICES "Set common compiler options" "${default_value}")
+if(NOT DEFINED CC_COMMON_OPTIONS)
+    option(CC_COMMON_OPTIONS "Set common compiler options" "${default_value}")
 endif()
-if(NOT DEFINED CC_WINDOWS_DEF)
-    option(CC_WINDOWS_DEF "Define useful Windows macros" "${default_value}")
+if(NOT DEFINED CC_WINDOWS_DEFINES)
+    option(CC_WINDOWS_DEFINES "Use common Windows macros" "${default_value}")
 endif()
 if(NOT DEFINED CC_STATIC_RUNTIME)
     set(static_runtime_default_value "${default_value}")
     if(DEFINED Boost_USE_STATIC_LIBS AND NOT Boost_USE_STATIC_LIBS)
         # Linking to dynamic Boost libs and the static runtime is a no-no:
         set(static_runtime_default_value OFF)
     endif()
@@ -76,16 +76,16 @@
 
 option(Boost_USE_STATIC_LIBS "Use the static Boost libraries" "${default_value}")
 option(Boost_USE_STATIC_RUNTIME "Use Boost libraries linked to the runtime statically" "${CC_STATIC_RUNTIME}")
 
 if(NOT parent_dir)
     message(STATUS "common.cmake: Toolset:                 ${toolset}")
     message(STATUS "common.cmake: C++ standard:            ${CC_CXX_STANDARD}")
-    message(STATUS "common.cmake: Common compiler options: ${CC_BEST_PRACTICES}")
-    message(STATUS "common.cmake: Useful Windows macros:   ${CC_WINDOWS_DEF}")
+    message(STATUS "common.cmake: Common compiler options: ${CC_COMMON_OPTIONS}")
+    message(STATUS "common.cmake: Common Windows defines:  ${CC_WINDOWS_DEFINES}")
     message(STATUS "common.cmake: Static Boost libraries:  ${Boost_USE_STATIC_LIBS}")
     message(STATUS "common.cmake: Static runtime:          ${CC_STATIC_RUNTIME}")
     message(STATUS "common.cmake: Strip symbols:           ${CC_STRIP_SYMBOLS}")
 endif()
 
 # C++ standard
 # ------------
@@ -93,50 +93,50 @@
 set(CMAKE_CXX_STANDARD "${CC_CXX_STANDARD}")
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 set(CMAKE_CXX_EXTENSIONS OFF)
 
 # Common compiler options
 # -----------------------
 
-function(_cc_best_practices_msvc target)
+function(_cc_common_options_msvc target)
     set(compile_options /MP /W4)
     target_compile_options("${target}" PRIVATE ${compile_options})
 endfunction()
 
-function(_cc_best_practices_gcc target)
+function(_cc_common_options_gcc target)
     set(compile_options -Wall -Wextra)
     target_compile_options("${target}" PRIVATE ${compile_options})
 endfunction()
 
-function(_cc_best_practices target)
+function(_cc_common_options target)
     get_target_property(target_type "${target}" TYPE)
     get_target_property(aliased "${target}" ALIASED_TARGET)
     if(NOT target_type STREQUAL "INTERFACE_LIBRARY" AND NOT aliased)
-        message(STATUS "common.cmake: ${target}: Settings common compiler options")
+        message(STATUS "common.cmake: ${target}: Setting common compiler options")
         if(is_msvc)
-            _cc_best_practices_msvc("${target}")
-        elseif(is_gcc)
-            _cc_best_practices_gcc("${target}")
+            _cc_common_options_msvc("${target}")
+        elseif(is_gcc OR is_clang)
+            _cc_common_options_gcc("${target}")
         endif()
     endif()
 endfunction()
 
 # Useful Windows macros
 # ---------------------
 
-function(_cc_common_windows_definitions target)
+function(_cc_common_windows_defines target)
     set(compile_definitions WIN32_LEAN_AND_MEAN NOMINMAX)
     get_target_property(target_type "${target}" TYPE)
     if(target_type STREQUAL "INTERFACE_LIBRARY")
-        message(STATUS "common.cmake: ${target}: Defining useful Windows macros")
+        message(STATUS "common.cmake: ${target}: Using common Windows defines")
         target_compile_definitions("${target}" INTERFACE ${compile_definitions})
     else()
         get_target_property(aliased "${target}" ALIASED_TARGET)
         if(NOT aliased)
-            message(STATUS "common.cmake: ${target}: Defining useful Windows macros")
+            message(STATUS "common.cmake: ${target}: Using common Windows defines")
             target_compile_definitions("${target}" PRIVATE ${compile_definitions})
         endif()
     endif()
 endfunction()
 
 # Static runtime
 # --------------
@@ -297,19 +297,19 @@
 # Main macros
 # -----------
 
 function(_cc_apply_settings target)
     if(TARGET "${target}")
         get_target_property(target_imported "${target}" IMPORTED)
         if(NOT target_imported)
-            if(CC_BEST_PRACTICES)
-                _cc_best_practices("${target}")
+            if(CC_COMMON_OPTIONS)
+                _cc_common_options("${target}")
             endif()
-            if(CC_WINDOWS_DEF)
-                _cc_common_windows_definitions("${target}")
+            if(CC_WINDOWS_DEFINES)
+                _cc_common_windows_defines("${target}")
             endif()
             if(CC_STRIP_SYMBOLS)
                 _cc_strip_symbols("${target}")
             endif()
             if(CC_STATIC_RUNTIME)
                 _cc_static_runtime("${target}")
             endif()
```

### Comparing `cmake_common-3.4.2/docs/boost.md` & `cmake_common-4.0/docs/boost.md`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/docs/ctest-driver.md` & `cmake_common-4.0/docs/ctest-driver.md`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/project/boost/archive.py` & `cmake_common-4.0/project/boost/archive.py`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/project/boost/build.py` & `cmake_common-4.0/project/boost/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # Copyright (c) 2019 Egor Tensin <Egor.Tensin@gmail.com>
 # This file is part of the "cmake-common" project.
 # For details, see https://github.com/egor-tensin/cmake-common.
 # Distributed under the MIT License.
 
 R'''Build Boost.
 
-This script builds the Boost libraries.  Its main utility is setting the
-correct --stagedir parameter value to avoid name clashes.
+The main utility of this script is setting the correct --stagedir parameter
+value to avoid name clashes.
+
+It also facilitates building with different toolsets/for different platforms
+with the help from the --toolset and --platform parameters.
 
 Usage example:
 
     $ boost-build -- boost_1_71_0/ --with-filesystem --with-program_options
     ...
 
 Consult the output of `boost-build --help` for more details.
```

### Comparing `cmake_common-3.4.2/project/boost/directory.py` & `cmake_common-4.0/project/boost/directory.py`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/project/boost/download.py` & `cmake_common-4.0/project/boost/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # This file is part of the "cmake-common" project.
 # For details, see https://github.com/egor-tensin/cmake-common.
 # Distributed under the MIT License.
 
 R'''Download & bootstrap Boost.
 
 This script downloads and unpacks a Boost distribution archive.  Its main
-utility is that it's supposed to be cross-platform.
+utility is that it's cross-platform & supports different Boost versions out of
+the box.
 
 Usage examples:
 
     $ boost-download 1.71.0
     ...
 
     $ boost-download --unpack ~/workspace/third-party/ 1.65.0
```

### Comparing `cmake_common-3.4.2/project/boost/version.py` & `cmake_common-4.0/project/boost/version.py`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/project/cmake/build.py` & `cmake_common-4.0/project/build.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Copyright (c) 2019 Egor Tensin <Egor.Tensin@gmail.com>
 # This file is part of the "cmake-common" project.
 # For details, see https://github.com/egor-tensin/cmake-common.
 # Distributed under the MIT License.
 
 R'''Build a CMake project.
 
-This script is used basically to invoke the CMake executable in a
-cross-platform way (provided the platform has Python 3, of course).  The
-motivation was to merge my Travis and AppVeyor build scripts (largely similar,
-but written in bash and PowerShell, respectively).
+This script works nicely with boost-build from this package - it will use the
+correct --stagedir directory automatically.
 
-A simple usage example:
+Also, it facilitates building with different toolsets/for different platforms
+with the help from the --toolset and --platform parameters.
 
-    $ cmake-build --configuration Release --install path/to/somewhere -- examples/simple
+Usage example:
+
+    $ project-build --configuration Release --install path/to/somewhere -- examples/simple build/
     ...
 
     $ ./path/to/somewhere/bin/foo
     foo
 '''
 
 import argparse
@@ -132,21 +133,22 @@
         return result
 
     def run(self, toolset):
         run_cmake(self._cmake_args(toolset))
 
 
 class BuildParameters:
-    def __init__(self, src_dir, build_dir=None, install_dir=None,
+    BUILD_DIR_TMP_PLACEHOLDER = 'TMP'
+
+    def __init__(self, src_dir, build_dir, install_dir=None,
                  platform=None, configuration=None, boost_dir=None,
                  toolset_version=None, cmake_args=None):
 
         src_dir = normalize_path(src_dir)
-        if build_dir is not None:
-            build_dir = normalize_path(build_dir)
+        build_dir = self.normalize_build_dir(build_dir)
         if install_dir is not None:
             install_dir = normalize_path(install_dir)
         platform = platform or DEFAULT_PLATFORM
         configuration = configuration or DEFAULT_CONFIGURATION
         if boost_dir is not None:
             boost_dir = normalize_path(boost_dir)
         toolset_version = toolset_version or DEFAULT_TOOLSET_VERSION
@@ -163,17 +165,23 @@
 
     @staticmethod
     def from_args(args):
         args = vars(args)
         args.pop('help_toolsets', None)
         return BuildParameters(**args)
 
+    @staticmethod
+    def normalize_build_dir(build_dir):
+        if build_dir == BuildParameters.BUILD_DIR_TMP_PLACEHOLDER:
+            return build_dir
+        return normalize_path(build_dir)
+
     @contextmanager
     def create_build_dir(self):
-        if self.build_dir is not None:
+        if self.build_dir != BuildParameters.BUILD_DIR_TMP_PLACEHOLDER:
             logging.info('Build directory: %s', self.build_dir)
             mkdir_parent(self.build_dir)
             yield self.build_dir
             return
 
         with tempfile.TemporaryDirectory(dir=os.path.dirname(self.src_dir)) as build_dir:
             logging.info('Build directory: %s', build_dir)
@@ -210,17 +218,14 @@
 
     parser = argparse.ArgumentParser(
         description=__doc__,
         formatter_class=argparse.RawDescriptionHelpFormatter)
 
     project.version.add_to_arg_parser(parser)
 
-    parser.add_argument('--build', metavar='DIR', dest='build_dir',
-                        type=normalize_path,
-                        help='build directory (temporary directory unless specified)')
     parser.add_argument('--install', metavar='DIR', dest='install_dir',
                         type=normalize_path,
                         help='install directory')
 
     platform_options = '/'.join(map(str, Platform.all()))
     configuration_options = '/'.join(map(str, Configuration.all()))
 
@@ -237,19 +242,19 @@
 
     parser.add_argument('--toolset', metavar='TOOLSET', dest='toolset_version',
                         type=ToolsetVersion.parse, default=DEFAULT_TOOLSET_VERSION,
                         help=f'toolset to use ({ToolsetVersion.usage()})')
     parser.add_argument('--help-toolsets', action='store_true',
                         help='show detailed info about supported toolsets')
 
-    parser.add_argument('src_dir', metavar='DIR',
-                        type=normalize_path,
+    parser.add_argument('src_dir', type=normalize_path,
                         help='source directory')
-    parser.add_argument('cmake_args', metavar='CMAKE_ARG',
-                        nargs='*', default=[],
+    parser.add_argument('build_dir', type=BuildParameters.normalize_build_dir,
+                        help=f"build directory ('{BuildParameters.BUILD_DIR_TMP_PLACEHOLDER}' to use a temporary directory)")
+    parser.add_argument('cmake_args', nargs='*', default=[],
                         help='additional CMake arguments, to be passed verbatim')
 
     return parser.parse_args(argv)
 
 
 def main(argv=None):
     args = _parse_args(argv)
```

### Comparing `cmake_common-3.4.2/project/configuration.py` & `cmake_common-4.0/project/configuration.py`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/project/linkage.py` & `cmake_common-4.0/project/linkage.py`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/project/mingw.py` & `cmake_common-4.0/project/mingw.py`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/project/os.py` & `cmake_common-4.0/project/os.py`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/project/platform.py` & `cmake_common-4.0/project/platform.py`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/project/toolset.py` & `cmake_common-4.0/project/toolset.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,17 +304,16 @@
             prefix = f'{hint}'
             if s.startswith(prefix):
                 return ToolsetVersion(hint, hint.parse_version(s[len(prefix):]))
         raise argparse.ArgumentTypeError(f'invalid toolset: {s}')
 
 
 class Toolset(abc.ABC):
-    @staticmethod
     @contextmanager
-    def b2_args():
+    def b2_args(self):
         # Write the config file, etc.
         yield []
 
     @staticmethod
     def bootstrap_bat_args():
         return []
```

### Comparing `cmake_common-3.4.2/project/utils.py` & `cmake_common-4.0/project/utils.py`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/pyproject.toml` & `cmake_common-4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -26,17 +26,15 @@
 [project.urls]
 "Homepage" = "https://github.com/egor-tensin/cmake-common"
 "Bug Tracker" = "https://github.com/egor-tensin/cmake-common/issues"
 
 [project.scripts]
 boost-build = "project.boost.build:_main"
 boost-download = "project.boost.download:_main"
-ci-boost = "project.ci.boost:main"
-ci-cmake = "project.ci.cmake:main"
-cmake-build = "project.cmake.build:main"
+project-build = "project.build:main"
 
 [tool.setuptools]
 script-files = [
     "tools/ctest-driver.py",
     "tools/project-clang-format.py",
 ]
```

### Comparing `cmake_common-3.4.2/tools/ctest-driver.py` & `cmake_common-4.0/tools/ctest-driver.py`

 * *Files identical despite different names*

### Comparing `cmake_common-3.4.2/tools/project-clang-format.py` & `cmake_common-4.0/tools/project-clang-format.py`

 * *Files identical despite different names*

