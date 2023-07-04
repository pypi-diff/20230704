# Comparing `tmp/ephysiopy-1.9.21.tar.gz` & `tmp/ephysiopy-1.9.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ephysiopy-1.9.21.tar", last modified: Fri Jun 16 13:04:35 2023, max compression
+gzip compressed data, was "ephysiopy-1.9.22.tar", last modified: Tue Jul  4 12:58:23 2023, max compression
```

## Comparing `ephysiopy-1.9.21.tar` & `ephysiopy-1.9.22.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:04:35.307211 ephysiopy-1.9.21/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-06-16 13:04:35.307211 ephysiopy-1.9.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:04:35.303211 ephysiopy-1.9.21/ephysiopy/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:04:35.303211 ephysiopy-1.9.21/ephysiopy/axona/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/axona/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/axona/axonaIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/axona/file_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/axona/tetrode_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/axona/tintcolours.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:04:35.303211 ephysiopy-1.9.21/ephysiopy/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34668 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/common/binning.py
--rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/common/ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/common/fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/common/gridcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/common/mle_von_mises_vals.py
--rw-r--r--   0 runner    (1001) docker     (123)    49500 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/common/phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/common/rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (123)    28784 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/common/spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/common/statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:04:35.307211 ephysiopy-1.9.21/ephysiopy/format_converters/
--rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/format_converters/OE_Axona.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/format_converters/OE_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/format_converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:04:35.307211 ephysiopy-1.9.21/ephysiopy/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24047 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/io/recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:04:35.307211 ephysiopy-1.9.21/ephysiopy/openephys2py/
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/openephys2py/KiloSort.py
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/openephys2py/OESettings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/openephys2py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:04:35.307211 ephysiopy-1.9.21/ephysiopy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-16 13:04:25.000000 ephysiopy-1.9.21/ephysiopy/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-16 13:04:26.000000 ephysiopy-1.9.21/ephysiopy/tests/test_axona_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-16 13:04:26.000000 ephysiopy-1.9.21/ephysiopy/tests/test_axona_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-06-16 13:04:26.000000 ephysiopy-1.9.21/ephysiopy/tests/test_binning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-16 13:04:26.000000 ephysiopy-1.9.21/ephysiopy/tests/test_dacq2py.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-06-16 13:04:26.000000 ephysiopy-1.9.21/ephysiopy/tests/test_ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-06-16 13:04:26.000000 ephysiopy-1.9.21/ephysiopy/tests/test_fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-16 13:04:26.000000 ephysiopy-1.9.21/ephysiopy/tests/test_gridcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-16 13:04:26.000000 ephysiopy-1.9.21/ephysiopy/tests/test_openephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-16 13:04:26.000000 ephysiopy-1.9.21/ephysiopy/tests/test_phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-16 13:04:26.000000 ephysiopy-1.9.21/ephysiopy/tests/test_rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-16 13:04:26.000000 ephysiopy-1.9.21/ephysiopy/tests/test_spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-16 13:04:26.000000 ephysiopy-1.9.21/ephysiopy/tests/test_statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-16 13:04:26.000000 ephysiopy-1.9.21/ephysiopy/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:04:35.307211 ephysiopy-1.9.21/ephysiopy/visualise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 13:04:26.000000 ephysiopy-1.9.21/ephysiopy/visualise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32324 2023-06-16 13:04:26.000000 ephysiopy-1.9.21/ephysiopy/visualise/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:04:35.303211 ephysiopy-1.9.21/ephysiopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-06-16 13:04:35.000000 ephysiopy-1.9.21/ephysiopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-16 13:04:35.000000 ephysiopy-1.9.21/ephysiopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:04:35.000000 ephysiopy-1.9.21/ephysiopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 13:04:35.000000 ephysiopy-1.9.21/ephysiopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 13:04:35.000000 ephysiopy-1.9.21/ephysiopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-16 13:04:35.307211 ephysiopy-1.9.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-16 13:04:26.000000 ephysiopy-1.9.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:23.482486 ephysiopy-1.9.22/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-04 12:58:23.482486 ephysiopy-1.9.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:23.478486 ephysiopy-1.9.22/ephysiopy/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:23.478486 ephysiopy-1.9.22/ephysiopy/axona/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/axona/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/axona/axonaIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/axona/file_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/axona/tetrode_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/axona/tintcolours.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:23.478486 ephysiopy-1.9.22/ephysiopy/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34668 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/common/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/common/ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/common/fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/common/gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/common/mle_von_mises_vals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49500 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/common/phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/common/rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28784 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/common/spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/common/statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:23.478486 ephysiopy-1.9.22/ephysiopy/format_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/format_converters/OE_Axona.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/format_converters/OE_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/format_converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:23.478486 ephysiopy-1.9.22/ephysiopy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24089 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/io/recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:23.482486 ephysiopy-1.9.22/ephysiopy/openephys2py/
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/openephys2py/KiloSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/openephys2py/OESettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/openephys2py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:23.482486 ephysiopy-1.9.22/ephysiopy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_axona_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_axona_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_dacq2py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_openephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:23.482486 ephysiopy-1.9.22/ephysiopy/visualise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/visualise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32324 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/visualise/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:23.478486 ephysiopy-1.9.22/ephysiopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-04 12:58:23.000000 ephysiopy-1.9.22/ephysiopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-04 12:58:23.000000 ephysiopy-1.9.22/ephysiopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 12:58:23.000000 ephysiopy-1.9.22/ephysiopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-04 12:58:23.000000 ephysiopy-1.9.22/ephysiopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 12:58:23.000000 ephysiopy-1.9.22/ephysiopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-04 12:58:23.482486 ephysiopy-1.9.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/setup.py
```

### Comparing `ephysiopy-1.9.21/LICENSE` & `ephysiopy-1.9.22/LICENSE`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/PKG-INFO` & `ephysiopy-1.9.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 1.9.21
+Version: 1.9.22
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-1.9.21/README.md` & `ephysiopy-1.9.22/README.md`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/axona/axonaIO.py` & `ephysiopy-1.9.22/ephysiopy/axona/axonaIO.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/axona/file_headers.py` & `ephysiopy-1.9.22/ephysiopy/axona/file_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/axona/tetrode_dict.py` & `ephysiopy-1.9.22/ephysiopy/axona/tetrode_dict.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/axona/tintcolours.py` & `ephysiopy-1.9.22/ephysiopy/axona/tintcolours.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/common/binning.py` & `ephysiopy-1.9.22/ephysiopy/common/binning.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/common/ephys_generic.py` & `ephysiopy-1.9.22/ephysiopy/common/ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/common/fieldcalcs.py` & `ephysiopy-1.9.22/ephysiopy/common/fieldcalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/common/gridcell.py` & `ephysiopy-1.9.22/ephysiopy/common/gridcell.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/common/mle_von_mises_vals.py` & `ephysiopy-1.9.22/ephysiopy/common/mle_von_mises_vals.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/common/phasecoding.py` & `ephysiopy-1.9.22/ephysiopy/common/phasecoding.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/common/rhythmicity.py` & `ephysiopy-1.9.22/ephysiopy/common/rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/common/spikecalcs.py` & `ephysiopy-1.9.22/ephysiopy/common/spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/common/statscalcs.py` & `ephysiopy-1.9.22/ephysiopy/common/statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/common/utils.py` & `ephysiopy-1.9.22/ephysiopy/common/utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/format_converters/OE_Axona.py` & `ephysiopy-1.9.22/ephysiopy/format_converters/OE_Axona.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/format_converters/OE_numpy.py` & `ephysiopy-1.9.22/ephysiopy/format_converters/OE_numpy.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/io/recording.py` & `ephysiopy-1.9.22/ephysiopy/io/recording.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,15 +459,15 @@
                     tokens = line.split(":")
                     start_time = int(tokens[-1])
                     sample_rate = int(tokens[0].split("@")
                                       [-1].strip().split()[0])
                     recording_start_time = start_time / sample_rate
         if self.path2PosData is not None:
             pos_data_type = getattr(self, "pos_data_type", "PosTracker")
-            if pos_data_type == "PosTracker":
+            if pos_data_type == "PosTracker" or pos_data_type == "Pos Tracker":
                 print("Loading PosTracker data...")
                 pos_data = np.load(os.path.join(
                     self.path2PosData, "data_array.npy"))
             if pos_data_type == "TrackingPlugin":
                 print("Loading Tracking Plugin data...")
                 pos_data = loadTrackingPluginData(
                     os.path.join(self.path2PosData, "data_array.npy")
@@ -576,15 +576,15 @@
         for d, c, f in os.walk(pname_root):
             for ff in f:
                 if "." not in c:  # ignore hidden directories
                     if "data_array.npy" in ff:
                         if PurePath(d).match(str(PosTracker_match)):
                             if self.path2PosData is None:
                                 self.path2PosData = os.path.join(d)
-                                setattr(self, "pos_data_type", "PosTracker")
+                                setattr(self, "pos_data_type", "Pos Tracker")
                                 print(f"Pos data at: {self.path2PosData}")
                             self.path2PosOEBin = Path(d).parents[1]
                         if PurePath(d).match("*pos_data*"):
                             if self.path2PosData is None:
                                 self.path2PosData = os.path.join(d)
                                 print(f"Pos data at: {self.path2PosData}")
                         if PurePath(d).match(str(TrackingPlugin_match)):
@@ -593,19 +593,19 @@
                                 setattr(self,
                                         "pos_data_type",
                                         "TrackingPlugin")
                                 print(f"Pos data at: {self.path2PosData}")
                     if "continuous.dat" in ff:
                         if PurePath(d).match(str(APdata_match)):
                             self.path2APdata = os.path.join(d)
-                            print(f"Continuous data at: {self.path2APdata}")
+                            print(f"Continuous AP data at: {self.path2APdata}")
                             self.path2APOEBin = Path(d).parents[1]
                         if PurePath(d).match(str(LFPdata_match)):
                             self.path2LFPdata = os.path.join(d)
-                            print(f"Continuous data at: {self.path2LFPdata}")
+                            print(f"Continuous LFP data at: {self.path2LFPdata}")
                         if PurePath(d).match(str(Rawdata_match)):
                             self.path2APdata = os.path.join(d)
                             self.path2LFPdata = os.path.join(d)
                         if PurePath(d).match(str(TrackMe_match)):
                             self.path2PosData = os.path.join(d)
                             setattr(self, "pos_data_type", "TrackMe")
                             print(f"TrackMe posdata at: {self.path2PosData}")
```

### Comparing `ephysiopy-1.9.21/ephysiopy/openephys2py/KiloSort.py` & `ephysiopy-1.9.22/ephysiopy/openephys2py/KiloSort.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/openephys2py/OESettings.py` & `ephysiopy-1.9.22/ephysiopy/openephys2py/OESettings.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,14 +199,15 @@
     Exposure: int = field(default=20)
     LeftBorder: int = field(default=0)
     RightBorder: int = field(default=800)
     TopBorder: int = field(default=0)
     BottomBorder: int = field(default=600)
     AutoExposure: bool = field(default=False)
     OverlayPath: bool = field(default=False)
+    sample_rate: int = field(default=30)
 
 
 @dataclass
 class TrackMe(OEPlugin):
     """
     Documents the TrackMe plugin
     """
@@ -284,16 +285,16 @@
     Loads up the structure.oebin file for openephys flat binary
     format recordings
     """
 
     def __init__(self, pname: str):
         self.filename = []
         self.data = []
-        import os
         import json
+        import os
 
         for d, _, f in os.walk(pname):
             for ff in f:
                 if "structure.oebin" in ff:
                     self.filename.append(os.path.join(d, ff))
                     with open(os.path.join(d, ff), "r") as f:
                         self.data.append(json.load(f))
@@ -322,14 +323,15 @@
         self.tree = None
         """
         It's not uncommon to have > 1 of the same type of processor, i.e.
         2 x bandpass filter to look at LFP and APs. This deals with that...
         """
         self.possible_processors = OrderedDict([
             ("Pos Tracker", PosTracker()),
+            ("PosTracker", PosTracker()),
             ("Rhythm FPGA", RhythmFPGA()),
             ("Neuropix-PXI", NeuropixPXI()),
             ("Acquisition Board", AcquisitionBoard()),
             ("Spike Sorter", SpikeSorter()),
             ("TrackMe", TrackMe()),
             ("Record Node", RecordNode())
         ])
@@ -355,18 +357,23 @@
         """
         if self.tree is None:
             self.load()
         # quick hack to deal with flat binary format that has no settings.xml
         if self.tree is not None:
             for elem in self.tree.iter("PROCESSOR"):
                 i_proc = elem.get("name")
+                if "/" in i_proc:
+                    i_proc = i_proc.split("/")[-1]
                 if i_proc == "Record Node":  # special as could be > 1
                     recNode = RecordNode()
                     recurseNode(elem, addValues2Class, recNode)
-                    self.record_nodes[i_proc + " " + recNode.nodeId] = recNode
+                    if recNode.nodeId is not None:
+                        self.record_nodes[i_proc + " " + recNode.nodeId] = recNode
+                    else:
+                        self.record_nodes[i_proc] = recNode
                 elif i_proc in self.possible_processors.keys():
                     self.processors[i_proc] = self.possible_processors[i_proc]
                     recurseNode(elem, addValues2Class, self.processors[i_proc])
                 else:
                     self.processors[i_proc] = OEPlugin()
                     recurseNode(elem, addValues2Class, self.processors[i_proc])
```

### Comparing `ephysiopy-1.9.21/ephysiopy/tests/conftest.py` & `ephysiopy-1.9.22/ephysiopy/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/tests/test_axona_headers.py` & `ephysiopy-1.9.22/ephysiopy/tests/test_axona_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/tests/test_axona_io.py` & `ephysiopy-1.9.22/ephysiopy/tests/test_axona_io.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/tests/test_binning.py` & `ephysiopy-1.9.22/ephysiopy/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/tests/test_dacq2py.py` & `ephysiopy-1.9.22/ephysiopy/tests/test_dacq2py.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/tests/test_ephys_generic.py` & `ephysiopy-1.9.22/ephysiopy/tests/test_ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/tests/test_fieldcalcs.py` & `ephysiopy-1.9.22/ephysiopy/tests/test_fieldcalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/tests/test_gridcell.py` & `ephysiopy-1.9.22/ephysiopy/tests/test_gridcell.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/tests/test_phasecoding.py` & `ephysiopy-1.9.22/ephysiopy/tests/test_phasecoding.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/tests/test_rhythmicity.py` & `ephysiopy-1.9.22/ephysiopy/tests/test_rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/tests/test_spikecalcs.py` & `ephysiopy-1.9.22/ephysiopy/tests/test_spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/tests/test_statscalcs.py` & `ephysiopy-1.9.22/ephysiopy/tests/test_statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/tests/test_utils.py` & `ephysiopy-1.9.22/ephysiopy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy/visualise/plotting.py` & `ephysiopy-1.9.22/ephysiopy/visualise/plotting.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/ephysiopy.egg-info/PKG-INFO` & `ephysiopy-1.9.22/ephysiopy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 1.9.21
+Version: 1.9.22
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-1.9.21/ephysiopy.egg-info/SOURCES.txt` & `ephysiopy-1.9.22/ephysiopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.21/setup.py` & `ephysiopy-1.9.22/setup.py`

 * *Files identical despite different names*

