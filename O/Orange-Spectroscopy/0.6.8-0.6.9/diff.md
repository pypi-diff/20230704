# Comparing `tmp/Orange-Spectroscopy-0.6.8.tar.gz` & `tmp/Orange-Spectroscopy-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Orange-Spectroscopy-0.6.8.tar", last modified: Thu Dec  8 15:15:45 2022, max compression
+gzip compressed data, was "Orange-Spectroscopy-0.6.9.tar", last modified: Wed Feb 22 16:44:10 2023, max compression
```

## Comparing `Orange-Spectroscopy-0.6.8.tar` & `Orange-Spectroscopy-0.6.9.tar`

### file list

```diff
@@ -1,360 +1,359 @@
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.295954 Orange-Spectroscopy-0.6.8/
--rw-rw-r--   0 marko     (1000) marko     (1000)      304 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/.coveragerc
--rw-rw-r--   0 marko     (1000) marko     (1000)      282 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/.gitignore
--rw-rw-r--   0 marko     (1000) marko     (1000)     3504 2020-06-09 12:02:20.000000 Orange-Spectroscopy-0.6.8/CONTRIBUTING.md
--rw-rw-r--   0 marko     (1000) marko     (1000)      612 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/LICENSE
--rw-rw-r--   0 marko     (1000) marko     (1000)      705 2022-09-02 11:01:23.000000 Orange-Spectroscopy-0.6.8/MANIFEST.in
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.211954 Orange-Spectroscopy-0.6.8/Orange_Spectroscopy.egg-info/
--rw-rw-r--   0 marko     (1000) marko     (1000)     1204 2022-12-08 15:15:45.000000 Orange-Spectroscopy-0.6.8/Orange_Spectroscopy.egg-info/PKG-INFO
--rw-rw-r--   0 marko     (1000) marko     (1000)    15242 2022-12-08 15:15:45.000000 Orange-Spectroscopy-0.6.8/Orange_Spectroscopy.egg-info/SOURCES.txt
--rw-rw-r--   0 marko     (1000) marko     (1000)        1 2022-12-08 15:15:45.000000 Orange-Spectroscopy-0.6.8/Orange_Spectroscopy.egg-info/dependency_links.txt
--rw-rw-r--   0 marko     (1000) marko     (1000)      299 2022-12-08 15:15:45.000000 Orange-Spectroscopy-0.6.8/Orange_Spectroscopy.egg-info/entry_points.txt
--rw-rw-r--   0 marko     (1000) marko     (1000)       14 2022-12-08 15:15:45.000000 Orange-Spectroscopy-0.6.8/Orange_Spectroscopy.egg-info/namespace_packages.txt
--rw-rw-r--   0 marko     (1000) marko     (1000)        1 2019-10-18 12:44:58.000000 Orange-Spectroscopy-0.6.8/Orange_Spectroscopy.egg-info/not-zip-safe
--rw-rw-r--   0 marko     (1000) marko     (1000)      331 2022-12-08 15:15:45.000000 Orange-Spectroscopy-0.6.8/Orange_Spectroscopy.egg-info/requires.txt
--rw-rw-r--   0 marko     (1000) marko     (1000)       14 2022-12-08 15:15:45.000000 Orange-Spectroscopy-0.6.8/Orange_Spectroscopy.egg-info/top_level.txt
--rw-rw-r--   0 marko     (1000) marko     (1000)     1204 2022-12-08 15:15:45.291954 Orange-Spectroscopy-0.6.8/PKG-INFO
--rw-rw-r--   0 marko     (1000) marko     (1000)     1734 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/README.md
--rw-rw-r--   0 marko     (1000) marko     (1000)      577 2021-07-07 12:48:35.000000 Orange-Spectroscopy-0.6.8/README.pypi
--rw-rw-r--   0 marko     (1000) marko     (1000)     1640 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/RELEASING.md
--rw-rw-r--   0 marko     (1000) marko     (1000)      179 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/codecov.yml
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.211954 Orange-Spectroscopy-0.6.8/conda/
--rw-rw-r--   0 marko     (1000) marko     (1000)     1223 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/conda/meta.yaml
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.215954 Orange-Spectroscopy-0.6.8/doc/
--rw-rw-r--   0 marko     (1000) marko     (1000)     7464 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.8/doc/Makefile
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.207954 Orange-Spectroscopy-0.6.8/doc/build/
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.215954 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/
--rw-rw-r--   0 marko     (1000) marko     (1000)      230 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/.buildinfo
--rw-rw-r--   0 marko     (1000) marko     (1000)     4052 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/OrangeSpectroscopyAdd-on.hhc
--rw-rw-r--   0 marko     (1000) marko     (1000)       11 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/OrangeSpectroscopyAdd-on.hhk
--rw-rw-r--   0 marko     (1000) marko     (1000)     1191 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/OrangeSpectroscopyAdd-on.hhp
--rw-rw-r--   0 marko     (1000) marko     (1000)      165 2021-08-20 11:35:41.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/OrangeSpectroscopyAdd-on.stp
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.219954 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/
--rw-rw-r--   0 marko     (1000) marko     (1000)     5422 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Average-Spectra-stamped.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    62941 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/HyperSpectra-stamped.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    60888 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Integrate-Spectra-Example.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    31757 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Integrate-Spectra-stamped.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    70077 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Interpolate-Example2.png
--rw-rw-r--   0 marko     (1000) marko     (1000)     7843 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Interpolate-stamped.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    68448 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Multifile-Example.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    18921 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Multifile-stamped.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    97594 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/PLS-Example.png
--rw-rw-r--   0 marko     (1000) marko     (1000)     9120 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/PLS-stamped.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    47004 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Peak-Fit-stamped.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    86533 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Preprocess-Spectra-Example.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    33892 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Preprocess-Spectra-stamped.png
--rw-rw-r--   0 marko     (1000) marko     (1000)     5064 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Reshape-Map-stamped.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    85445 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Spectra-Example1.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    54120 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Spectra-stamped.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    24261 2020-06-09 12:02:20.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Tilefile-Example.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    19885 2020-06-09 12:02:20.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Tilefile-stamped.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    14866 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/snr_average_x.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    16023 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/snr_print.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    15770 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/snr_std_y.png
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.223954 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/
--rw-rw-r--   0 marko     (1000) marko     (1000)    11185 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/alabaster.css
--rw-rw-r--   0 marko     (1000) marko     (1000)    14667 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/basic.css
--rw-rw-r--   0 marko     (1000) marko     (1000)       42 2021-08-20 11:35:40.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/custom.css
--rw-rw-r--   0 marko     (1000) marko     (1000)     9630 2021-12-17 11:18:57.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/doctools.js
--rw-rw-r--   0 marko     (1000) marko     (1000)      354 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/documentation_options.js
--rw-rw-r--   0 marko     (1000) marko     (1000)      286 2021-12-17 11:18:57.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/file.png
--rw-rw-r--   0 marko     (1000) marko     (1000)   287630 2021-12-17 11:18:57.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/jquery-3.5.1.js
--rw-rw-r--   0 marko     (1000) marko     (1000)    89476 2021-12-17 11:18:57.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/jquery.js
--rw-rw-r--   0 marko     (1000) marko     (1000)      325 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/language_data.js
--rw-rw-r--   0 marko     (1000) marko     (1000)       90 2021-12-17 11:18:57.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/minus.png
--rw-rw-r--   0 marko     (1000) marko     (1000)       90 2021-12-17 11:18:57.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/plus.png
--rw-rw-r--   0 marko     (1000) marko     (1000)     4846 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/pygments.css
--rw-rw-r--   0 marko     (1000) marko     (1000)    16793 2021-12-17 11:18:57.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/searchtools.js
--rw-rw-r--   0 marko     (1000) marko     (1000)      427 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/style.css
--rw-rw-r--   0 marko     (1000) marko     (1000)    68420 2021-12-17 11:18:57.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/underscore-1.13.1.js
--rw-rw-r--   0 marko     (1000) marko     (1000)    19530 2021-12-17 11:18:57.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/underscore.js
--rw-rw-r--   0 marko     (1000) marko     (1000)     1419 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/genindex.html
--rw-rw-r--   0 marko     (1000) marko     (1000)     4626 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/index.html
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.223954 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/
--rw-rw-r--   0 marko     (1000) marko     (1000)     2670 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/SpikeRemoval.html
--rw-rw-r--   0 marko     (1000) marko     (1000)     5030 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/als.html
--rw-rw-r--   0 marko     (1000) marko     (1000)     3922 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/atmcorr.html
--rw-rw-r--   0 marko     (1000) marko     (1000)     2452 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/average.html
--rw-rw-r--   0 marko     (1000) marko     (1000)     3938 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/hyperspectra.html
--rw-rw-r--   0 marko     (1000) marko     (1000)     3945 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/integrate-spectra.html
--rw-rw-r--   0 marko     (1000) marko     (1000)     2089 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/interferogram-to-spectrum.html
--rw-rw-r--   0 marko     (1000) marko     (1000)     5470 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/interpolate.html
--rw-rw-r--   0 marko     (1000) marko     (1000)     3567 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/multifile.html
--rw-rw-r--   0 marko     (1000) marko     (1000)     9159 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/peakfit.html
--rw-rw-r--   0 marko     (1000) marko     (1000)     3706 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/pls.html
--rw-rw-r--   0 marko     (1000) marko     (1000)     7121 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/preprocess-spectra.html
--rw-rw-r--   0 marko     (1000) marko     (1000)     2370 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/reshape-map.html
--rw-rw-r--   0 marko     (1000) marko     (1000)     3479 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/snr.html
--rw-rw-r--   0 marko     (1000) marko     (1000)     5036 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/spectra.html
--rw-rw-r--   0 marko     (1000) marko     (1000)     4625 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/tilefile.html
--rw-rw-r--   0 marko     (1000) marko     (1000)     9749 2020-07-16 12:50:48.000000 Orange-Spectroscopy-0.6.8/doc/conf.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     1272 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/doc/index.rst
--rw-rw-r--   0 marko     (1000) marko     (1000)     7009 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.8/doc/make.bat
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.223954 Orange-Spectroscopy-0.6.8/doc/static/
--rw-rw-r--   0 marko     (1000) marko     (1000)      427 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.8/doc/static/style.css
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.223954 Orange-Spectroscopy-0.6.8/doc/widgets/
--rw-rw-r--   0 marko     (1000) marko     (1000)      550 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/doc/widgets/average.md
--rw-rw-r--   0 marko     (1000) marko     (1000)     1829 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/doc/widgets/hyperspectra.md
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.231954 Orange-Spectroscopy-0.6.8/doc/widgets/images/
--rw-rw-r--   0 marko     (1000) marko     (1000)     5422 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/doc/widgets/images/Average-Spectra-stamped.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    62941 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.8/doc/widgets/images/HyperSpectra-stamped.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    60888 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.8/doc/widgets/images/Integrate-Spectra-Example.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    31757 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.8/doc/widgets/images/Integrate-Spectra-stamped.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    14226 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.8/doc/widgets/images/Interferogram-to-Spectrum-stamped.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    75648 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.8/doc/widgets/images/Interpolate-Example1.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    70077 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.8/doc/widgets/images/Interpolate-Example2.png
--rw-rw-r--   0 marko     (1000) marko     (1000)     7843 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.8/doc/widgets/images/Interpolate-stamped.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    68448 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.8/doc/widgets/images/Multifile-Example.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    18921 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.8/doc/widgets/images/Multifile-stamped.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    86533 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/doc/widgets/images/Preprocess-Spectra-Example.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    33892 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/doc/widgets/images/Preprocess-Spectra-stamped.png
--rw-rw-r--   0 marko     (1000) marko     (1000)     5064 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/doc/widgets/images/Reshape-Map-stamped.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    85445 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/doc/widgets/images/Spectra-Example1.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    54120 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/doc/widgets/images/Spectra-stamped.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    24261 2020-06-09 12:02:20.000000 Orange-Spectroscopy-0.6.8/doc/widgets/images/Tilefile-Example.png
--rw-rw-r--   0 marko     (1000) marko     (1000)    19885 2020-06-09 12:02:20.000000 Orange-Spectroscopy-0.6.8/doc/widgets/images/Tilefile-stamped.png
--rw-rw-r--   0 marko     (1000) marko     (1000)     1676 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/doc/widgets/integrate-spectra.md
--rw-rw-r--   0 marko     (1000) marko     (1000)      277 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/doc/widgets/interferogram-to-spectrum.md
--rw-rw-r--   0 marko     (1000) marko     (1000)     2938 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/doc/widgets/interpolate.md
--rw-rw-r--   0 marko     (1000) marko     (1000)     1455 2020-06-09 12:02:20.000000 Orange-Spectroscopy-0.6.8/doc/widgets/multifile.md
--rw-rw-r--   0 marko     (1000) marko     (1000)     4387 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/doc/widgets/preprocess-spectra.md
--rw-rw-r--   0 marko     (1000) marko     (1000)      439 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/doc/widgets/reshape-map.md
--rw-rw-r--   0 marko     (1000) marko     (1000)     2593 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/doc/widgets/spectra.md
--rw-rw-r--   0 marko     (1000) marko     (1000)     2443 2020-06-09 12:02:20.000000 Orange-Spectroscopy-0.6.8/doc/widgets/tilefile.md
--rw-rw-r--   0 marko     (1000) marko     (1000)     3314 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/doc/widgets.json
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.231954 Orange-Spectroscopy-0.6.8/orangecontrib/
--rw-rw-r--   0 marko     (1000) marko     (1000)      164 2020-08-27 10:15:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/__init__.py
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.231954 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/
--rw-rw-r--   0 marko     (1000) marko     (1000)      634 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/__init__.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     1699 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/data.py
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.239954 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/
--rw-rw-r--   0 marko     (1000) marko     (1000)    82060 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/Au168mA_nodisplacement.gsf
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.239954 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/Hermes_HDF5/
--rw-rw-r--   0 marko     (1000) marko     (1000)     7704 2020-07-09 11:24:19.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/Hermes_HDF5/small_OK.hdf5
--rw-rw-r--   0 marko     (1000) marko     (1000)    88727 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/IFG_single.dpt
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.239954 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/NeaReaderGSF_test/
--rwxrwxr-x   0 marko     (1000) marko     (1000)     4292 2020-01-09 13:54:30.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/NeaReaderGSF_test/NeaReaderGSF_test O2A raw.gsf
--rwxrwxr-x   0 marko     (1000) marko     (1000)     4292 2020-01-09 13:54:30.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/NeaReaderGSF_test/NeaReaderGSF_test O2P raw.gsf
--rwxrwxr-x   0 marko     (1000) marko     (1000)     7977 2020-01-09 13:54:30.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/NeaReaderGSF_test/NeaReaderGSF_test.html
--rw-rw-r--   0 marko     (1000) marko     (1000)        0 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/__init__.py
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.243954 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/
--rw-rw-r--   0 marko     (1000) marko     (1000)    17408 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/4_noimage_agg256.bsp
--rw-rw-r--   0 marko     (1000) marko     (1000)     3324 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/4_noimage_agg256.dat
--rw-rw-r--   0 marko     (1000) marko     (1000)      348 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/4_noimage_agg256.hdr
--rw-rw-r--   0 marko     (1000) marko     (1000)    80636 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/4_noimage_agg256.seq
--rw-rw-r--   0 marko     (1000) marko     (1000)     2172 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024.dat
--rw-rw-r--   0 marko     (1000) marko     (1000)     2172 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024.dms
--rw-rw-r--   0 marko     (1000) marko     (1000)      348 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024.hdr
--rw-rw-r--   0 marko     (1000) marko     (1000)     1596 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024_0000_0000.dmd
--rw-rw-r--   0 marko     (1000) marko     (1000)    20924 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024_0000_0000.drd
--rw-rw-r--   0 marko     (1000) marko     (1000)     1596 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024_0000_0001.dmd
--rw-rw-r--   0 marko     (1000) marko     (1000)    20924 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024_0000_0001.drd
--rw-rw-r--   0 marko     (1000) marko     (1000)    17920 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/5_mosaic_agg1024.dmt
--rw-rw-r--   0 marko     (1000) marko     (1000)    18432 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/background_agg256.bsp
--rw-rw-r--   0 marko     (1000) marko     (1000)     3324 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/background_agg256.dat
--rw-rw-r--   0 marko     (1000) marko     (1000)    80636 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/background_agg256.seq
--rw-rw-r--   0 marko     (1000) marko     (1000)  1034486 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/collagen.csv
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.243954 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/emsc/
--rw-rw-r--   0 marko     (1000) marko     (1000)    20282 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/emsc/MieStd1_rawSpec.csv
--rw-rw-r--   0 marko     (1000) marko     (1000)    17864 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/emsc/MieStd2_refSpec.csv
--rw-rw-r--   0 marko     (1000) marko     (1000)     2272 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/emsc/MieStd3_corr.csv
--rw-rw-r--   0 marko     (1000) marko     (1000)      763 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/emsc/MieStd4_param.csv
--rw-rw-r--   0 marko     (1000) marko     (1000)     2494 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/emsc/MieStd5_residuals.csv
--rw-rw-r--   0 marko     (1000) marko     (1000)       51 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/emsc/MieStd6_niter.csv
--rw-rw-r--   0 marko     (1000) marko     (1000)       61 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/emsc/MieStd7_RMSE.csv
--rw-rw-r--   0 marko     (1000) marko     (1000)     4565 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/exafs-test.tab
--rw-rw-r--   0 marko     (1000) marko     (1000)    49200 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/m_xyxy.spc
--rw-rw-r--   0 marko     (1000) marko     (1000)     1156 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/map_test.xyz
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.247954 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/matlab/
--rw-rw-r--   0 marko     (1000) marko     (1000)      400 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/matlab/metas_mixed.mat
--rw-rw-r--   0 marko     (1000) marko     (1000)      392 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/matlab/metas_numeric.mat
--rw-rw-r--   0 marko     (1000) marko     (1000)      328 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/matlab/metas_string.mat
--rw-rw-r--   0 marko     (1000) marko     (1000)      304 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/matlab/names.mat
--rw-rw-r--   0 marko     (1000) marko     (1000)      224 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/matlab/only_annotations.mat
--rw-rw-r--   0 marko     (1000) marko     (1000)      232 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/matlab/simple.mat
--rw-rw-r--   0 marko     (1000) marko     (1000)      312 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/matlab/wavenumbers.mat
--rw-rw-r--   0 marko     (1000) marko     (1000)     5654 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/max_iv.hdr
--rw-rw-r--   0 marko     (1000) marko     (1000)      510 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/max_iv_a000.xim
--rw-rw-r--   0 marko     (1000) marko     (1000)      510 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/max_iv_a001.xim
--rw-rw-r--   0 marko     (1000) marko     (1000)     1163 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/nea_test_v2.txt
--rw-rw-r--   0 marko     (1000) marko     (1000)  1184436 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/peach_juice.0
--rw-rw-r--   0 marko     (1000) marko     (1000)    36122 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/peach_juice.dpt
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.247954 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/photothermal/
--rw-rw-r--   0 marko     (1000) marko     (1000)   249008 2021-07-07 12:48:35.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/photothermal/Hyper_Sample.ptir
--rw-rw-r--   0 marko     (1000) marko     (1000)   139224 2021-07-07 12:48:35.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/photothermal/Nodax_Spectral_Array.ptir
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.247954 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/renishaw_test_files/
--rw-rw-r--   0 marko     (1000) marko     (1000)    74855 2020-08-27 10:04:31.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/renishaw_test_files/sp.wdf
--rw-rw-r--   0 marko     (1000) marko     (1000)      575 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/rock.txt
--rw-rw-r--   0 marko     (1000) marko     (1000)     8868 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/sample1.spa
--rwxrwxr-x   0 marko     (1000) marko     (1000)  1737576 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/small_Omnic.map
--rw-rw-r--   0 marko     (1000) marko     (1000)    11336 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/small_diamond_nxs.nxs
--rw-rw-r--   0 marko     (1000) marko     (1000)     8016 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/spectra20_small.nea
--rw-rw-r--   0 marko     (1000) marko     (1000)    11032 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/three_coordinates_data.csv
--rw-rw-r--   0 marko     (1000) marko     (1000)    80272 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/whitelight.gsf
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.251954 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/
--rw-rw-r--   0 marko     (1000) marko     (1000)      839 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/__init__.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     8064 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/agilent.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     3274 2022-12-08 14:53:12.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/ascii.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     1319 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/diamond.py
--rw-rw-r--   0 marko     (1000) marko     (1000)      762 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/envi.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     1721 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/gsf.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     3643 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/matlab.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     3802 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/maxiv.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     1388 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/meta.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    11337 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/neaspec.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     1147 2022-12-08 14:17:01.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/old.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     5224 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/omnic.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     7251 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/opus.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     7418 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/ptir.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     3365 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/soleil.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     3853 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/util.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     2204 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/wire.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    12418 2021-07-07 12:48:35.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/irfft.py
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.251954 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/models/
--rw-rw-r--   0 marko     (1000) marko     (1000)        0 2020-06-09 12:02:20.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/models/__init__.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     2107 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/models/pls.py
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.255954 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/preprocess/
--rw-rw-r--   0 marko     (1000) marko     (1000)    31209 2022-11-11 09:13:31.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/preprocess/__init__.py
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.255954 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/preprocess/als/
--rw-rw-r--   0 marko     (1000) marko     (1000)     4146 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/preprocess/als/__init__.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    10814 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/preprocess/als/baseline.py
--rwxrwxr-x   0 marko     (1000) marko     (1000)     7407 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/preprocess/atm_corr.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     7060 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/preprocess/emsc.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    11757 2022-11-11 09:13:31.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/preprocess/integrate.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    16476 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/preprocess/me_emsc.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     1301 2020-01-28 13:00:39.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/preprocess/npfunc.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     3506 2022-11-11 09:13:31.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/preprocess/transform.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     7596 2022-11-11 09:13:31.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/preprocess/utils.py
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.271954 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/
--rw-rw-r--   0 marko     (1000) marko     (1000)      481 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/__init__.py
--rw-rw-r--   0 marko     (1000) marko     (1000)      547 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/bigdata.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     2320 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/example_connect_settings.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     4560 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/spectral_preprocess.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     1575 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_als.py
--rwxrwxr-x   0 marko     (1000) marko     (1000)     1424 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_atm_corr.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     6746 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_conversion.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     2058 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_cut.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     1596 2021-07-07 12:48:35.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_despike.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     2339 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_editor_als.py
--rwxrwxr-x   0 marko     (1000) marko     (1000)     2244 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_editor_atm_corr.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     2639 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_editor_baseline.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     2121 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_editor_emsc.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     1315 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_editor_gaussian.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     3816 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_editor_me_emsc.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     2264 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_editor_normalize.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     1630 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_editor_spikeremoval.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     7762 2020-01-28 13:00:39.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_emsc.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     7145 2022-11-11 09:13:31.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_integrate.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     5785 2022-11-11 09:13:31.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_interpolate.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     5522 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_irfft.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    10199 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_me_emsc.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     1163 2020-01-28 13:00:39.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_npfunc.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    11846 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owalignstack.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     6019 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owaverage.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     4324 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owbin.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     5812 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owfft.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    27531 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owhyper.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     5554 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owintegrate.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     3289 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owinterpolate.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    14859 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owmultifile.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    19217 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owpeakfit.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     2735 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owpls.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    16169 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owpreprocess.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     3214 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owreshape.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     3028 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owsnr.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    25487 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owspectra.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     5765 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owspectralseries.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    20839 2022-11-11 09:13:31.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_preprocess.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    22263 2022-12-08 14:53:12.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_readers.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     4399 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_tile_reader.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     2122 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_utils.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     1337 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_widgets_utils.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     2324 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_xas.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     1120 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/time_interpolation.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     3398 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/time_irfft.py
--rw-rw-r--   0 marko     (1000) marko     (1000)      821 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/time_preprocess.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     1260 2020-01-28 13:00:39.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/util.py
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.271954 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tutorials/
--rw-rw-r--   0 marko     (1000) marko     (1000)        0 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tutorials/__init__.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    10590 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tutorials/tile-loader.ows
--rw-rw-r--   0 marko     (1000) marko     (1000)      438 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/util.py
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.275954 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/
--rw-rw-r--   0 marko     (1000) marko     (1000)     4298 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/__init__.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    21621 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/agilent.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     1984 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/binning.py
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.275954 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/pymca5/
--rw-rw-r--   0 marko     (1000) marko     (1000)     6737 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/pymca5/DataObject.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    12800 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/pymca5/OmnicMap.py
--rw-rw-r--   0 marko     (1000) marko     (1000)        0 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/pymca5/__init__.py
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.275954 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/skimage/
--rw-rw-r--   0 marko     (1000) marko     (1000)     1648 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/skimage/README.txt
--rw-rw-r--   0 marko     (1000) marko     (1000)        0 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/skimage/__init__.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    11583 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/skimage/register_translation.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     8405 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/skimage/shape.py
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.279954 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/spc/
--rw-rw-r--   0 marko     (1000) marko     (1000)      213 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/spc/README.txt
--rw-rw-r--   0 marko     (1000) marko     (1000)      232 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/spc/__init__.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     1691 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/spc/global_fun.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    25174 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/spc/spc.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     5891 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/spc/sub.py
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.287954 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/
--rw-rw-r--   0 marko     (1000) marko     (1000)     1071 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/__init__.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    17491 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/gui.py
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.291954 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/
--rw-rw-r--   0 marko     (1000) marko     (1000)     7458 2020-06-09 12:02:20.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/PLS.svg
--rw-rw-r--   0 marko     (1000) marko     (1000)     4452 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/average.svg
--rw-rw-r--   0 marko     (1000) marko     (1000)     2088 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/bin.svg
--rw-rw-r--   0 marko     (1000) marko     (1000)     4674 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/category.svg
--rw-rw-r--   0 marko     (1000) marko     (1000)      982 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/fft.svg
--rw-rw-r--   0 marko     (1000) marko     (1000)     1494 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/hyper.svg
--rw-rw-r--   0 marko     (1000) marko     (1000)     1150 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/integrate.svg
--rw-rw-r--   0 marko     (1000) marko     (1000)      759 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/interpolate.svg
--rw-rw-r--   0 marko     (1000) marko     (1000)     3335 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/multifile.svg
--rw-rw-r--   0 marko     (1000) marko     (1000)      631 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/mywidget.svg
--rw-rw-r--   0 marko     (1000) marko     (1000)    12119 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/peakfit.svg
--rw-rw-r--   0 marko     (1000) marko     (1000)     1561 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/preprocess.svg
--rw-rw-r--   0 marko     (1000) marko     (1000)     1353 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/reshape.svg
--rw-rw-r--   0 marko     (1000) marko     (1000)     6411 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/snr.svg
--rw-rw-r--   0 marko     (1000) marko     (1000)      922 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/spectra.svg
--rw-rw-r--   0 marko     (1000) marko     (1000)     2499 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/spectralseries.svg
--rw-rw-r--   0 marko     (1000) marko     (1000)      461 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/stackalign.svg
--rw-rw-r--   0 marko     (1000) marko     (1000)     9635 2020-06-09 12:02:20.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/tilefile.svg
--rw-rw-r--   0 marko     (1000) marko     (1000)     6170 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/line_geometry.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     4795 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owaverage.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     7247 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owbin.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    24501 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owfft.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    53356 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owhyper.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    11753 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owintegrate.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     5608 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owinterpolate.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    18361 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owmultifile.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    17229 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owpeakfit.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     2876 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owpls.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    35824 2022-11-29 15:00:18.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owpreprocess.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     5275 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owreshape.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     8182 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owsnr.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    64536 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owspectra.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    11140 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owspectralseries.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    10082 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owstackalign.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    22732 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owtilefile.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    20059 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/peak_editors.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     2335 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/peakfit_compute.py
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2022-12-08 15:15:45.291954 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/
--rw-rw-r--   0 marko     (1000) marko     (1000)      245 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/__init__.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     4770 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/als.py
--rwxrwxr-x   0 marko     (1000) marko     (1000)     6885 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/atm_corr.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     6404 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/baseline.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    10132 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/emsc.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     8911 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/integrate.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     6037 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/me_emsc.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    16141 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/misc.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     9878 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/normalize.py
--rw-rw-r--   0 marko     (1000) marko     (1000)      357 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/registry.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     2741 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/spikeremoval.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     3224 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/utils.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    14887 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/xas.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     4583 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/utils.py
--rw-rw-r--   0 marko     (1000) marko     (1000)    12456 2019-07-08 11:08:51.000000 Orange-Spectroscopy-0.6.8/pylintrc
--rw-rw-r--   0 marko     (1000) marko     (1000)      115 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.8/pyproject.toml
--rw-rw-r--   0 marko     (1000) marko     (1000)    50260 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.8/screenshot.png
--rw-rw-r--   0 marko     (1000) marko     (1000)       38 2022-12-08 15:15:45.295954 Orange-Spectroscopy-0.6.8/setup.cfg
--rw-rw-r--   0 marko     (1000) marko     (1000)     5179 2022-12-08 14:53:23.000000 Orange-Spectroscopy-0.6.8/setup.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.587075 Orange-Spectroscopy-0.6.9/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      304 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/.coveragerc
+-rw-rw-r--   0 marko     (1000) marko     (1000)      282 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/.gitignore
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3504 2020-06-09 12:02:20.000000 Orange-Spectroscopy-0.6.9/CONTRIBUTING.md
+-rw-rw-r--   0 marko     (1000) marko     (1000)      612 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/LICENSE
+-rw-rw-r--   0 marko     (1000) marko     (1000)      705 2022-09-02 11:01:23.000000 Orange-Spectroscopy-0.6.9/MANIFEST.in
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.419075 Orange-Spectroscopy-0.6.9/Orange_Spectroscopy.egg-info/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1204 2023-02-22 16:44:10.000000 Orange-Spectroscopy-0.6.9/Orange_Spectroscopy.egg-info/PKG-INFO
+-rw-rw-r--   0 marko     (1000) marko     (1000)    15205 2023-02-22 16:44:10.000000 Orange-Spectroscopy-0.6.9/Orange_Spectroscopy.egg-info/SOURCES.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)        1 2023-02-22 16:44:10.000000 Orange-Spectroscopy-0.6.9/Orange_Spectroscopy.egg-info/dependency_links.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)      299 2023-02-22 16:44:10.000000 Orange-Spectroscopy-0.6.9/Orange_Spectroscopy.egg-info/entry_points.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)       14 2023-02-22 16:44:10.000000 Orange-Spectroscopy-0.6.9/Orange_Spectroscopy.egg-info/namespace_packages.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)        1 2019-10-18 12:44:58.000000 Orange-Spectroscopy-0.6.9/Orange_Spectroscopy.egg-info/not-zip-safe
+-rw-rw-r--   0 marko     (1000) marko     (1000)      331 2023-02-22 16:44:10.000000 Orange-Spectroscopy-0.6.9/Orange_Spectroscopy.egg-info/requires.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)       14 2023-02-22 16:44:10.000000 Orange-Spectroscopy-0.6.9/Orange_Spectroscopy.egg-info/top_level.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1204 2023-02-22 16:44:10.587075 Orange-Spectroscopy-0.6.9/PKG-INFO
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1734 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/README.md
+-rw-rw-r--   0 marko     (1000) marko     (1000)      577 2021-07-07 12:48:35.000000 Orange-Spectroscopy-0.6.9/README.pypi
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1640 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/RELEASING.md
+-rw-rw-r--   0 marko     (1000) marko     (1000)      179 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/codecov.yml
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.419075 Orange-Spectroscopy-0.6.9/conda/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1230 2023-02-22 15:59:06.000000 Orange-Spectroscopy-0.6.9/conda/meta.yaml
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.419075 Orange-Spectroscopy-0.6.9/doc/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     7464 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.9/doc/Makefile
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.411075 Orange-Spectroscopy-0.6.9/doc/build/
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.423075 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      230 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/.buildinfo
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4052 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/OrangeSpectroscopyAdd-on.hhc
+-rw-rw-r--   0 marko     (1000) marko     (1000)       11 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/OrangeSpectroscopyAdd-on.hhk
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1191 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/OrangeSpectroscopyAdd-on.hhp
+-rw-rw-r--   0 marko     (1000) marko     (1000)      165 2021-08-20 11:35:41.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/OrangeSpectroscopyAdd-on.stp
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.439075 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5422 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Average-Spectra-stamped.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    62941 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/HyperSpectra-stamped.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    60888 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Integrate-Spectra-Example.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    31757 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Integrate-Spectra-stamped.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    70077 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Interpolate-Example2.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)     7843 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Interpolate-stamped.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    68448 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Multifile-Example.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    18921 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Multifile-stamped.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    97594 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/PLS-Example.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)     9120 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/PLS-stamped.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    47004 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Peak-Fit-stamped.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    86533 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Preprocess-Spectra-Example.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    33892 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Preprocess-Spectra-stamped.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5064 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Reshape-Map-stamped.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    85445 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Spectra-Example1.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    54120 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Spectra-stamped.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    24261 2020-06-09 12:02:20.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Tilefile-Example.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    19885 2020-06-09 12:02:20.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Tilefile-stamped.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    14866 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/snr_average_x.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    16023 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/snr_print.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    15770 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/snr_std_y.png
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.447075 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/
+-rw-rw-r--   0 marko     (1000) marko     (1000)    11185 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/alabaster.css
+-rw-rw-r--   0 marko     (1000) marko     (1000)    14667 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/basic.css
+-rw-rw-r--   0 marko     (1000) marko     (1000)       42 2021-08-20 11:35:40.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/custom.css
+-rw-rw-r--   0 marko     (1000) marko     (1000)     9630 2021-12-17 11:18:57.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/doctools.js
+-rw-rw-r--   0 marko     (1000) marko     (1000)      354 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/documentation_options.js
+-rw-rw-r--   0 marko     (1000) marko     (1000)      286 2021-12-17 11:18:57.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/file.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)   287630 2021-12-17 11:18:57.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/jquery-3.5.1.js
+-rw-rw-r--   0 marko     (1000) marko     (1000)    89476 2021-12-17 11:18:57.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/jquery.js
+-rw-rw-r--   0 marko     (1000) marko     (1000)      325 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/language_data.js
+-rw-rw-r--   0 marko     (1000) marko     (1000)       90 2021-12-17 11:18:57.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/minus.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)       90 2021-12-17 11:18:57.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/plus.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4846 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/pygments.css
+-rw-rw-r--   0 marko     (1000) marko     (1000)    16793 2021-12-17 11:18:57.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/searchtools.js
+-rw-rw-r--   0 marko     (1000) marko     (1000)      427 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/style.css
+-rw-rw-r--   0 marko     (1000) marko     (1000)    68420 2021-12-17 11:18:57.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/underscore-1.13.1.js
+-rw-rw-r--   0 marko     (1000) marko     (1000)    19530 2021-12-17 11:18:57.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/underscore.js
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1419 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/genindex.html
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4626 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/index.html
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.455075 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2670 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/SpikeRemoval.html
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5030 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/als.html
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3922 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/atmcorr.html
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2452 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/average.html
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3938 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/hyperspectra.html
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3945 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/integrate-spectra.html
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2089 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/interferogram-to-spectrum.html
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5470 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/interpolate.html
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3567 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/multifile.html
+-rw-rw-r--   0 marko     (1000) marko     (1000)     9159 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/peakfit.html
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3706 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/pls.html
+-rw-rw-r--   0 marko     (1000) marko     (1000)     7121 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/preprocess-spectra.html
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2370 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/reshape-map.html
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3479 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/snr.html
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5036 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/spectra.html
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4625 2022-12-08 15:15:36.000000 Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/tilefile.html
+-rw-rw-r--   0 marko     (1000) marko     (1000)     9749 2020-07-16 12:50:48.000000 Orange-Spectroscopy-0.6.9/doc/conf.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1272 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/doc/index.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)     7009 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.9/doc/make.bat
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.455075 Orange-Spectroscopy-0.6.9/doc/static/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      427 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.9/doc/static/style.css
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.459075 Orange-Spectroscopy-0.6.9/doc/widgets/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      550 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/doc/widgets/average.md
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1829 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/doc/widgets/hyperspectra.md
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.475075 Orange-Spectroscopy-0.6.9/doc/widgets/images/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5422 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/doc/widgets/images/Average-Spectra-stamped.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    62941 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.9/doc/widgets/images/HyperSpectra-stamped.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    60888 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.9/doc/widgets/images/Integrate-Spectra-Example.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    31757 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.9/doc/widgets/images/Integrate-Spectra-stamped.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    14226 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.9/doc/widgets/images/Interferogram-to-Spectrum-stamped.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    75648 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.9/doc/widgets/images/Interpolate-Example1.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    70077 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.9/doc/widgets/images/Interpolate-Example2.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)     7843 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.9/doc/widgets/images/Interpolate-stamped.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    68448 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.9/doc/widgets/images/Multifile-Example.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    18921 2019-05-30 11:25:48.000000 Orange-Spectroscopy-0.6.9/doc/widgets/images/Multifile-stamped.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    86533 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/doc/widgets/images/Preprocess-Spectra-Example.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    33892 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/doc/widgets/images/Preprocess-Spectra-stamped.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5064 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/doc/widgets/images/Reshape-Map-stamped.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    85445 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/doc/widgets/images/Spectra-Example1.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    54120 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/doc/widgets/images/Spectra-stamped.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    24261 2020-06-09 12:02:20.000000 Orange-Spectroscopy-0.6.9/doc/widgets/images/Tilefile-Example.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    19885 2020-06-09 12:02:20.000000 Orange-Spectroscopy-0.6.9/doc/widgets/images/Tilefile-stamped.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1676 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/doc/widgets/integrate-spectra.md
+-rw-rw-r--   0 marko     (1000) marko     (1000)      277 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/doc/widgets/interferogram-to-spectrum.md
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2938 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/doc/widgets/interpolate.md
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1455 2020-06-09 12:02:20.000000 Orange-Spectroscopy-0.6.9/doc/widgets/multifile.md
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4387 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/doc/widgets/preprocess-spectra.md
+-rw-rw-r--   0 marko     (1000) marko     (1000)      439 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/doc/widgets/reshape-map.md
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2593 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/doc/widgets/spectra.md
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2443 2020-06-09 12:02:20.000000 Orange-Spectroscopy-0.6.9/doc/widgets/tilefile.md
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3314 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/doc/widgets.json
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.475075 Orange-Spectroscopy-0.6.9/orangecontrib/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      164 2020-08-27 10:15:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/__init__.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.475075 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      634 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1699 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/data.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.507075 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/
+-rw-rw-r--   0 marko     (1000) marko     (1000)    82060 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/Au168mA_nodisplacement.gsf
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.507075 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/Hermes_HDF5/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     7704 2020-07-09 11:24:19.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/Hermes_HDF5/small_OK.hdf5
+-rw-rw-r--   0 marko     (1000) marko     (1000)    88727 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/IFG_single.dpt
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.511075 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/NeaReaderGSF_test/
+-rwxrwxr-x   0 marko     (1000) marko     (1000)     4292 2020-01-09 13:54:30.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/NeaReaderGSF_test/NeaReaderGSF_test O2A raw.gsf
+-rwxrwxr-x   0 marko     (1000) marko     (1000)     4292 2020-01-09 13:54:30.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/NeaReaderGSF_test/NeaReaderGSF_test O2P raw.gsf
+-rwxrwxr-x   0 marko     (1000) marko     (1000)     7977 2020-01-09 13:54:30.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/NeaReaderGSF_test/NeaReaderGSF_test.html
+-rw-rw-r--   0 marko     (1000) marko     (1000)        0 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/__init__.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.519075 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/
+-rw-rw-r--   0 marko     (1000) marko     (1000)    17408 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/4_noimage_agg256.bsp
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3324 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/4_noimage_agg256.dat
+-rw-rw-r--   0 marko     (1000) marko     (1000)      348 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/4_noimage_agg256.hdr
+-rw-rw-r--   0 marko     (1000) marko     (1000)    80636 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/4_noimage_agg256.seq
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2172 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024.dat
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2172 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024.dms
+-rw-rw-r--   0 marko     (1000) marko     (1000)      348 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024.hdr
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1596 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024_0000_0000.dmd
+-rw-rw-r--   0 marko     (1000) marko     (1000)    20924 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024_0000_0000.drd
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1596 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024_0000_0001.dmd
+-rw-rw-r--   0 marko     (1000) marko     (1000)    20924 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024_0000_0001.drd
+-rw-rw-r--   0 marko     (1000) marko     (1000)    17920 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/5_mosaic_agg1024.dmt
+-rw-rw-r--   0 marko     (1000) marko     (1000)    18432 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/background_agg256.bsp
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3324 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/background_agg256.dat
+-rw-rw-r--   0 marko     (1000) marko     (1000)    80636 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/background_agg256.seq
+-rw-rw-r--   0 marko     (1000) marko     (1000)  1034486 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/collagen.csv
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.523075 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/emsc/
+-rw-rw-r--   0 marko     (1000) marko     (1000)    20282 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/emsc/MieStd1_rawSpec.csv
+-rw-rw-r--   0 marko     (1000) marko     (1000)    17864 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/emsc/MieStd2_refSpec.csv
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2272 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/emsc/MieStd3_corr.csv
+-rw-rw-r--   0 marko     (1000) marko     (1000)      763 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/emsc/MieStd4_param.csv
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2494 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/emsc/MieStd5_residuals.csv
+-rw-rw-r--   0 marko     (1000) marko     (1000)       51 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/emsc/MieStd6_niter.csv
+-rw-rw-r--   0 marko     (1000) marko     (1000)       61 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/emsc/MieStd7_RMSE.csv
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4565 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/exafs-test.tab
+-rw-rw-r--   0 marko     (1000) marko     (1000)    49200 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/m_xyxy.spc
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1156 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/map_test.xyz
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.523075 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/matlab/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      400 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/matlab/metas_mixed.mat
+-rw-rw-r--   0 marko     (1000) marko     (1000)      392 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/matlab/metas_numeric.mat
+-rw-rw-r--   0 marko     (1000) marko     (1000)      328 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/matlab/metas_string.mat
+-rw-rw-r--   0 marko     (1000) marko     (1000)      304 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/matlab/names.mat
+-rw-rw-r--   0 marko     (1000) marko     (1000)      224 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/matlab/only_annotations.mat
+-rw-rw-r--   0 marko     (1000) marko     (1000)      232 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/matlab/simple.mat
+-rw-rw-r--   0 marko     (1000) marko     (1000)      312 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/matlab/wavenumbers.mat
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5654 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/max_iv.hdr
+-rw-rw-r--   0 marko     (1000) marko     (1000)      510 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/max_iv_a000.xim
+-rw-rw-r--   0 marko     (1000) marko     (1000)      510 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/max_iv_a001.xim
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1163 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/nea_test_v2.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)  1184436 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/peach_juice.0
+-rw-rw-r--   0 marko     (1000) marko     (1000)    36122 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/peach_juice.dpt
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.527075 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/photothermal/
+-rw-rw-r--   0 marko     (1000) marko     (1000)   249008 2021-07-07 12:48:35.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/photothermal/Hyper_Sample.ptir
+-rw-rw-r--   0 marko     (1000) marko     (1000)   139224 2021-07-07 12:48:35.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/photothermal/Nodax_Spectral_Array.ptir
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.527075 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/renishaw_test_files/
+-rw-rw-r--   0 marko     (1000) marko     (1000)    74855 2020-08-27 10:04:31.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/renishaw_test_files/sp.wdf
+-rw-rw-r--   0 marko     (1000) marko     (1000)      575 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/rock.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)     8868 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/sample1.spa
+-rwxrwxr-x   0 marko     (1000) marko     (1000)  1737576 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/small_Omnic.map
+-rw-rw-r--   0 marko     (1000) marko     (1000)    11336 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/small_diamond_nxs.nxs
+-rw-rw-r--   0 marko     (1000) marko     (1000)     8016 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/spectra20_small.nea
+-rw-rw-r--   0 marko     (1000) marko     (1000)    11032 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/three_coordinates_data.csv
+-rw-rw-r--   0 marko     (1000) marko     (1000)    80272 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/whitelight.gsf
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.535075 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      839 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     8064 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/agilent.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3274 2022-12-08 14:53:12.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/ascii.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1319 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/diamond.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      762 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/envi.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1721 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/gsf.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3643 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/matlab.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3802 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/maxiv.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1388 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/meta.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    11337 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/neaspec.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5224 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/omnic.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     7469 2023-02-09 15:03:07.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/opus.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     7418 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/ptir.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3365 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/soleil.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3853 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/util.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2204 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/wire.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    12418 2021-07-07 12:48:35.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/irfft.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.535075 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/models/
+-rw-rw-r--   0 marko     (1000) marko     (1000)        0 2020-06-09 12:02:20.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/models/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2107 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/models/pls.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.539075 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/preprocess/
+-rw-rw-r--   0 marko     (1000) marko     (1000)    31209 2022-11-11 09:13:31.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/preprocess/__init__.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.539075 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/preprocess/als/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4146 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/preprocess/als/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    10814 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/preprocess/als/baseline.py
+-rwxrwxr-x   0 marko     (1000) marko     (1000)     7407 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/preprocess/atm_corr.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     7060 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/preprocess/emsc.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    11757 2022-11-11 09:13:31.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/preprocess/integrate.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    16476 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/preprocess/me_emsc.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1301 2020-01-28 13:00:39.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/preprocess/npfunc.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3506 2022-11-11 09:13:31.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/preprocess/transform.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     7596 2022-11-11 09:13:31.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/preprocess/utils.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.563075 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      481 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      547 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/bigdata.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2320 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/example_connect_settings.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4560 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/spectral_preprocess.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1575 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_als.py
+-rwxrwxr-x   0 marko     (1000) marko     (1000)     1424 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_atm_corr.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     6746 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_conversion.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2058 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_cut.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1596 2021-07-07 12:48:35.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_despike.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2339 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_editor_als.py
+-rwxrwxr-x   0 marko     (1000) marko     (1000)     2244 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_editor_atm_corr.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2639 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_editor_baseline.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2121 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_editor_emsc.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1315 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_editor_gaussian.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3816 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_editor_me_emsc.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2264 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_editor_normalize.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1630 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_editor_spikeremoval.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     7762 2020-01-28 13:00:39.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_emsc.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     7145 2022-11-11 09:13:31.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_integrate.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5785 2022-11-11 09:13:31.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_interpolate.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5522 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_irfft.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    10199 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_me_emsc.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1163 2020-01-28 13:00:39.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_npfunc.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    11846 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owalignstack.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     6019 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owaverage.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4324 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owbin.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5812 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owfft.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    27531 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owhyper.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5554 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owintegrate.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3289 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owinterpolate.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    17439 2023-02-22 15:38:18.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owmultifile.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    19217 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owpeakfit.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2735 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owpls.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    16169 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owpreprocess.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3214 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owreshape.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3028 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owsnr.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    25487 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owspectra.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5765 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owspectralseries.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    20839 2022-11-11 09:13:31.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_preprocess.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    22263 2022-12-08 14:53:12.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_readers.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4399 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_tile_reader.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2122 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_utils.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1337 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_widgets_utils.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2324 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_xas.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1120 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/time_interpolation.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3398 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/time_irfft.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      821 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/time_preprocess.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1260 2020-01-28 13:00:39.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/util.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.563075 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tutorials/
+-rw-rw-r--   0 marko     (1000) marko     (1000)        0 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tutorials/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    10590 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tutorials/tile-loader.ows
+-rw-rw-r--   0 marko     (1000) marko     (1000)      438 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/util.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.563075 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4298 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    21621 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/agilent.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1984 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/binning.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.563075 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/pymca5/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     6737 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/pymca5/DataObject.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    12800 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/pymca5/OmnicMap.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)        0 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/pymca5/__init__.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.567075 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/skimage/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1648 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/skimage/README.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)        0 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/skimage/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    11583 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/skimage/register_translation.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     8405 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/skimage/shape.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.567075 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/spc/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      213 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/spc/README.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)      232 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/spc/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1691 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/spc/global_fun.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    25174 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/spc/spc.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5891 2020-01-09 12:05:41.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/spc/sub.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.579075 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1071 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    17491 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/gui.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.583075 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     7458 2020-06-09 12:02:20.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/PLS.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4452 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/average.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2088 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/bin.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4674 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/category.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)      982 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/fft.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1494 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/hyper.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1150 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/integrate.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)      759 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/interpolate.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3335 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/multifile.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)      631 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/mywidget.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)    12119 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/peakfit.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1561 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/preprocess.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1353 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/reshape.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     6411 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/snr.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)      922 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/spectra.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2499 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/spectralseries.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)      461 2019-09-06 09:04:49.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/stackalign.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     9635 2020-06-09 12:02:20.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/tilefile.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     6170 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/line_geometry.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4795 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owaverage.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     7247 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owbin.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    24501 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owfft.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    53356 2023-01-20 10:48:41.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owhyper.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    11753 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owintegrate.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5608 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owinterpolate.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    20026 2023-02-22 15:38:18.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owmultifile.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    17229 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owpeakfit.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2876 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owpls.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    35908 2023-02-09 15:03:07.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owpreprocess.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5275 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owreshape.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     8182 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owsnr.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    64360 2023-02-09 15:03:07.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owspectra.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    11140 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owspectralseries.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    10082 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owstackalign.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    22732 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owtilefile.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    20059 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/peak_editors.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2335 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/peakfit_compute.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-02-22 16:44:10.587075 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      245 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4770 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/als.py
+-rwxrwxr-x   0 marko     (1000) marko     (1000)     6885 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/atm_corr.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     6404 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/baseline.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    10132 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/emsc.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     8911 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/integrate.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     6037 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/me_emsc.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    16141 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/misc.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     9878 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/normalize.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      357 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/registry.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2741 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/spikeremoval.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3224 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/utils.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    14887 2022-12-08 14:18:23.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/xas.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4583 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/utils.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    12456 2019-07-08 11:08:51.000000 Orange-Spectroscopy-0.6.9/pylintrc
+-rw-rw-r--   0 marko     (1000) marko     (1000)      115 2022-11-09 13:20:00.000000 Orange-Spectroscopy-0.6.9/pyproject.toml
+-rw-rw-r--   0 marko     (1000) marko     (1000)    50260 2019-05-30 11:25:49.000000 Orange-Spectroscopy-0.6.9/screenshot.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)       38 2023-02-22 16:44:10.587075 Orange-Spectroscopy-0.6.9/setup.cfg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5179 2023-02-22 15:39:59.000000 Orange-Spectroscopy-0.6.9/setup.py
```

### Comparing `Orange-Spectroscopy-0.6.8/CONTRIBUTING.md` & `Orange-Spectroscopy-0.6.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/LICENSE` & `Orange-Spectroscopy-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/MANIFEST.in` & `Orange-Spectroscopy-0.6.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/Orange_Spectroscopy.egg-info/PKG-INFO` & `Orange-Spectroscopy-0.6.9/Orange_Spectroscopy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Orange-Spectroscopy
-Version: 0.6.8
+Version: 0.6.9
 Summary: Extends Orange to handle spectral and hyperspectral analysis.
 Home-page: https://github.com/Quasars/orange-spectroscopy
 Author: Canadian Light Source, Biolab UL, Soleil, Elettra
 Author-email: marko.toplak@gmail.com
 License: GPLv3+
 Description: Spectral Orange
         ===============
```

### Comparing `Orange-Spectroscopy-0.6.8/Orange_Spectroscopy.egg-info/SOURCES.txt` & `Orange-Spectroscopy-0.6.9/Orange_Spectroscopy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,14 @@
 orangecontrib/spectroscopy/io/diamond.py
 orangecontrib/spectroscopy/io/envi.py
 orangecontrib/spectroscopy/io/gsf.py
 orangecontrib/spectroscopy/io/matlab.py
 orangecontrib/spectroscopy/io/maxiv.py
 orangecontrib/spectroscopy/io/meta.py
 orangecontrib/spectroscopy/io/neaspec.py
-orangecontrib/spectroscopy/io/old.py
 orangecontrib/spectroscopy/io/omnic.py
 orangecontrib/spectroscopy/io/opus.py
 orangecontrib/spectroscopy/io/ptir.py
 orangecontrib/spectroscopy/io/soleil.py
 orangecontrib/spectroscopy/io/util.py
 orangecontrib/spectroscopy/io/wire.py
 orangecontrib/spectroscopy/models/__init__.py
```

### Comparing `Orange-Spectroscopy-0.6.8/PKG-INFO` & `Orange-Spectroscopy-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Orange-Spectroscopy
-Version: 0.6.8
+Version: 0.6.9
 Summary: Extends Orange to handle spectral and hyperspectral analysis.
 Home-page: https://github.com/Quasars/orange-spectroscopy
 Author: Canadian Light Source, Biolab UL, Soleil, Elettra
 Author-email: marko.toplak@gmail.com
 License: GPLv3+
 Description: Spectral Orange
         ===============
```

### Comparing `Orange-Spectroscopy-0.6.8/README.md` & `Orange-Spectroscopy-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/README.pypi` & `Orange-Spectroscopy-0.6.9/README.pypi`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/RELEASING.md` & `Orange-Spectroscopy-0.6.9/RELEASING.md`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/conda/meta.yaml` & `Orange-Spectroscopy-0.6.9/conda/meta.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   run:
     - python >=3.8
     - numpy >=1.18.0
     - orange3 >=3.31.0
     - orange-canvas-core >=0.1.24
     - orange-widget-base >=4.16.1
     - scipy >=1.4.0
-    - scikit-learn >0.23.0
+    - scikit-learn >0.23.0,<1.2.0
     - spectral >=0.18,!=0.23
     - serverfiles >=0.2
     - AnyQt >=0.0.6
     - pyqtgraph >=0.11.1,!=0.12.4
     - colorcet
     - h5py
     - extranormal3 >=0.0.3
```

### Comparing `Orange-Spectroscopy-0.6.8/doc/Makefile` & `Orange-Spectroscopy-0.6.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/OrangeSpectroscopyAdd-on.hhc` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/OrangeSpectroscopyAdd-on.hhc`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/OrangeSpectroscopyAdd-on.hhp` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/OrangeSpectroscopyAdd-on.hhp`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Average-Spectra-stamped.png` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Average-Spectra-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/HyperSpectra-stamped.png` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/HyperSpectra-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Integrate-Spectra-Example.png` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Integrate-Spectra-Example.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Integrate-Spectra-stamped.png` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Integrate-Spectra-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Interpolate-Example2.png` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Interpolate-Example2.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Interpolate-stamped.png` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Interpolate-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Multifile-Example.png` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Multifile-Example.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Multifile-stamped.png` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Multifile-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/PLS-Example.png` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/PLS-Example.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/PLS-stamped.png` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/PLS-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Peak-Fit-stamped.png` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Peak-Fit-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Preprocess-Spectra-Example.png` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Preprocess-Spectra-Example.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Preprocess-Spectra-stamped.png` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Preprocess-Spectra-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Reshape-Map-stamped.png` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Reshape-Map-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Spectra-Example1.png` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Spectra-Example1.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Spectra-stamped.png` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Spectra-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Tilefile-Example.png` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Tilefile-Example.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/Tilefile-stamped.png` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/Tilefile-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/snr_average_x.png` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/snr_average_x.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/snr_print.png` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/snr_print.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_images/snr_std_y.png` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_images/snr_std_y.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/alabaster.css` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/basic.css` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/basic.css`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/doctools.js` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/jquery-3.5.1.js` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/jquery.js` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/pygments.css` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/searchtools.js` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/underscore-1.13.1.js` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/_static/underscore.js` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/genindex.html` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/genindex.html`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/index.html` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/index.html`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/SpikeRemoval.html` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/SpikeRemoval.html`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/als.html` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/als.html`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/atmcorr.html` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/atmcorr.html`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/average.html` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/average.html`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/hyperspectra.html` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/hyperspectra.html`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/integrate-spectra.html` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/integrate-spectra.html`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/interferogram-to-spectrum.html` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/interferogram-to-spectrum.html`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/interpolate.html` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/interpolate.html`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/multifile.html` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/multifile.html`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/peakfit.html` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/peakfit.html`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/pls.html` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/pls.html`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/preprocess-spectra.html` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/preprocess-spectra.html`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/reshape-map.html` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/reshape-map.html`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/snr.html` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/snr.html`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/spectra.html` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/spectra.html`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/build/htmlhelp/widgets/tilefile.html` & `Orange-Spectroscopy-0.6.9/doc/build/htmlhelp/widgets/tilefile.html`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/conf.py` & `Orange-Spectroscopy-0.6.9/doc/conf.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/index.rst` & `Orange-Spectroscopy-0.6.9/doc/index.rst`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/make.bat` & `Orange-Spectroscopy-0.6.9/doc/make.bat`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/average.md` & `Orange-Spectroscopy-0.6.9/doc/widgets/average.md`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/hyperspectra.md` & `Orange-Spectroscopy-0.6.9/doc/widgets/hyperspectra.md`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/images/Average-Spectra-stamped.png` & `Orange-Spectroscopy-0.6.9/doc/widgets/images/Average-Spectra-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/images/HyperSpectra-stamped.png` & `Orange-Spectroscopy-0.6.9/doc/widgets/images/HyperSpectra-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/images/Integrate-Spectra-Example.png` & `Orange-Spectroscopy-0.6.9/doc/widgets/images/Integrate-Spectra-Example.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/images/Integrate-Spectra-stamped.png` & `Orange-Spectroscopy-0.6.9/doc/widgets/images/Integrate-Spectra-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/images/Interferogram-to-Spectrum-stamped.png` & `Orange-Spectroscopy-0.6.9/doc/widgets/images/Interferogram-to-Spectrum-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/images/Interpolate-Example1.png` & `Orange-Spectroscopy-0.6.9/doc/widgets/images/Interpolate-Example1.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/images/Interpolate-Example2.png` & `Orange-Spectroscopy-0.6.9/doc/widgets/images/Interpolate-Example2.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/images/Interpolate-stamped.png` & `Orange-Spectroscopy-0.6.9/doc/widgets/images/Interpolate-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/images/Multifile-Example.png` & `Orange-Spectroscopy-0.6.9/doc/widgets/images/Multifile-Example.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/images/Multifile-stamped.png` & `Orange-Spectroscopy-0.6.9/doc/widgets/images/Multifile-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/images/Preprocess-Spectra-Example.png` & `Orange-Spectroscopy-0.6.9/doc/widgets/images/Preprocess-Spectra-Example.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/images/Preprocess-Spectra-stamped.png` & `Orange-Spectroscopy-0.6.9/doc/widgets/images/Preprocess-Spectra-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/images/Reshape-Map-stamped.png` & `Orange-Spectroscopy-0.6.9/doc/widgets/images/Reshape-Map-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/images/Spectra-Example1.png` & `Orange-Spectroscopy-0.6.9/doc/widgets/images/Spectra-Example1.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/images/Spectra-stamped.png` & `Orange-Spectroscopy-0.6.9/doc/widgets/images/Spectra-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/images/Tilefile-Example.png` & `Orange-Spectroscopy-0.6.9/doc/widgets/images/Tilefile-Example.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/images/Tilefile-stamped.png` & `Orange-Spectroscopy-0.6.9/doc/widgets/images/Tilefile-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/integrate-spectra.md` & `Orange-Spectroscopy-0.6.9/doc/widgets/integrate-spectra.md`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/interpolate.md` & `Orange-Spectroscopy-0.6.9/doc/widgets/interpolate.md`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/multifile.md` & `Orange-Spectroscopy-0.6.9/doc/widgets/multifile.md`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/preprocess-spectra.md` & `Orange-Spectroscopy-0.6.9/doc/widgets/preprocess-spectra.md`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/spectra.md` & `Orange-Spectroscopy-0.6.9/doc/widgets/spectra.md`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets/tilefile.md` & `Orange-Spectroscopy-0.6.9/doc/widgets/tilefile.md`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/doc/widgets.json` & `Orange-Spectroscopy-0.6.9/doc/widgets.json`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/__init__.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/data.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/data.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/Au168mA_nodisplacement.gsf` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/Au168mA_nodisplacement.gsf`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/Hermes_HDF5/small_OK.hdf5` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/Hermes_HDF5/small_OK.hdf5`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/IFG_single.dpt` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/IFG_single.dpt`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/NeaReaderGSF_test/NeaReaderGSF_test O2A raw.gsf` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/NeaReaderGSF_test/NeaReaderGSF_test O2A raw.gsf`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/NeaReaderGSF_test/NeaReaderGSF_test O2P raw.gsf` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/NeaReaderGSF_test/NeaReaderGSF_test O2P raw.gsf`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/NeaReaderGSF_test/NeaReaderGSF_test.html` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/NeaReaderGSF_test/NeaReaderGSF_test.html`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/4_noimage_agg256.bsp` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/4_noimage_agg256.bsp`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/4_noimage_agg256.dat` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/4_noimage_agg256.dat`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/4_noimage_agg256.seq` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/4_noimage_agg256.seq`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024.dat` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024.dat`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024.dms` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024.dms`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024_0000_0000.dmd` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024_0000_0000.dmd`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024_0000_0000.drd` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024_0000_0000.drd`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024_0000_0001.dmd` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024_0000_0001.dmd`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024_0000_0001.drd` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/5_Mosaic_agg1024_0000_0001.drd`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/5_mosaic_agg1024.dmt` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/5_mosaic_agg1024.dmt`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/background_agg256.bsp` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/background_agg256.bsp`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/background_agg256.dat` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/background_agg256.dat`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/agilent/background_agg256.seq` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/agilent/background_agg256.seq`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/collagen.csv` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/collagen.csv`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/emsc/MieStd1_rawSpec.csv` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/emsc/MieStd1_rawSpec.csv`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/emsc/MieStd2_refSpec.csv` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/emsc/MieStd2_refSpec.csv`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/emsc/MieStd3_corr.csv` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/emsc/MieStd3_corr.csv`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/emsc/MieStd4_param.csv` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/emsc/MieStd4_param.csv`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/emsc/MieStd5_residuals.csv` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/emsc/MieStd5_residuals.csv`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/exafs-test.tab` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/exafs-test.tab`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/m_xyxy.spc` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/m_xyxy.spc`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/map_test.xyz` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/map_test.xyz`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/max_iv.hdr` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/max_iv.hdr`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/nea_test_v2.txt` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/nea_test_v2.txt`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/peach_juice.0` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/peach_juice.0`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/peach_juice.dpt` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/peach_juice.dpt`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/photothermal/Hyper_Sample.ptir` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/photothermal/Hyper_Sample.ptir`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/photothermal/Nodax_Spectral_Array.ptir` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/photothermal/Nodax_Spectral_Array.ptir`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/renishaw_test_files/sp.wdf` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/renishaw_test_files/sp.wdf`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/rock.txt` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/rock.txt`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/sample1.spa` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/sample1.spa`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/small_Omnic.map` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/small_Omnic.map`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/small_diamond_nxs.nxs` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/small_diamond_nxs.nxs`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/spectra20_small.nea` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/spectra20_small.nea`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/three_coordinates_data.csv` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/three_coordinates_data.csv`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/datasets/whitelight.gsf` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/datasets/whitelight.gsf`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/__init__.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/agilent.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/agilent.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/ascii.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/ascii.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/diamond.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/diamond.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/envi.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/envi.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/gsf.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/gsf.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/matlab.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/matlab.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/maxiv.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/maxiv.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/meta.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/meta.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/neaspec.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/neaspec.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/omnic.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/omnic.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/opus.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/opus.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import io
+import warnings
 
 import Orange
 import numpy as np
 from Orange.data import FileFormat, ContinuousVariable, StringVariable, TimeVariable
 
 
 class OPUSReader(FileFormat):
@@ -163,26 +164,31 @@
                 if meta_data is not None:
                     # NB dtype default will be np.array(fill_value).dtype in future
                     meta_data = np.column_stack((meta_data, params.astype(object)))
                 else:
                     meta_data = params
 
         visible_images = []
-        for img in opusFC.getVisImages(self.filename):
-            try:
-                visible_images.append({
-                    'name': img['Title'],
-                    'image_ref': io.BytesIO(img['image']),
-                    'pos_x': img['Pos. X'] * img['PixelSizeX'],
-                    'pos_y': img['Pos. Y'] * img['PixelSizeY'],
-                    'pixel_size_x': img['PixelSizeX'],
-                    'pixel_size_y': img['PixelSizeY'],
-                })
-            except KeyError:
-                pass
+        try:
+            opus_imgs = opusFC.getVisImages(self.filename)
+        except Exception as e:
+            warnings.warn(f"Visible images load failed: {e}")
+        else:
+            for img in opus_imgs:
+                try:
+                    visible_images.append({
+                        'name': img['Title'],
+                        'image_ref': io.BytesIO(img['image']),
+                        'pos_x': img['Pos. X'] * img['PixelSizeX'],
+                        'pos_y': img['Pos. Y'] * img['PixelSizeY'],
+                        'pixel_size_x': img['PixelSizeX'],
+                        'pixel_size_y': img['PixelSizeY'],
+                    })
+                except KeyError:
+                    pass
 
         domain = Orange.data.Domain(attrs, clses, metas)
 
         meta_data = np.atleast_2d(meta_data)
 
         table = Orange.data.Table.from_numpy(domain,
                                              y_data.astype(float, order='C'),
```

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/ptir.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/ptir.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/soleil.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/soleil.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/util.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/util.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/io/wire.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/io/wire.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/irfft.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/irfft.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/models/pls.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/models/pls.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/preprocess/__init__.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/preprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/preprocess/als/__init__.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/preprocess/als/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/preprocess/als/baseline.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/preprocess/als/baseline.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/preprocess/atm_corr.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/preprocess/atm_corr.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/preprocess/emsc.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/preprocess/emsc.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/preprocess/integrate.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/preprocess/integrate.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/preprocess/me_emsc.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/preprocess/me_emsc.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/preprocess/npfunc.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/preprocess/npfunc.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/preprocess/transform.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/preprocess/transform.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/preprocess/utils.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/preprocess/utils.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/bigdata.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/bigdata.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/example_connect_settings.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/example_connect_settings.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/spectral_preprocess.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/spectral_preprocess.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_als.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_als.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_atm_corr.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_atm_corr.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_conversion.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_cut.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_cut.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_despike.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_despike.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_editor_als.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_editor_als.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_editor_atm_corr.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_editor_atm_corr.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_editor_baseline.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_editor_baseline.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_editor_emsc.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_editor_emsc.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_editor_gaussian.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_editor_gaussian.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_editor_me_emsc.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_editor_me_emsc.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_editor_normalize.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_editor_normalize.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_editor_spikeremoval.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_editor_spikeremoval.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_emsc.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_emsc.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_integrate.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_integrate.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_interpolate.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_irfft.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_irfft.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_me_emsc.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_me_emsc.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_npfunc.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_npfunc.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owalignstack.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owalignstack.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owaverage.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owaverage.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owbin.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owbin.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owfft.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owfft.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owhyper.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owhyper.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owintegrate.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owintegrate.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owinterpolate.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owinterpolate.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owmultifile.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owmultifile.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 from Orange.data.io import TabReader
 from Orange.tests import named_file
 
 from orangecontrib.spectroscopy.data import getx
 from orangecontrib.spectroscopy.io import SPAReader
 from orangecontrib.spectroscopy.io.ascii import AsciiColReader
 from orangecontrib.spectroscopy.io.util import SpectralFileFormat
-from orangecontrib.spectroscopy.widgets.owmultifile import OWMultifile, numpy_union_keep_order
+from orangecontrib.spectroscopy.widgets.owmultifile import OWMultifile, numpy_union_keep_order, \
+    wns_to_unique_str, decimals_neeeded_for_unique_str
 
 
 class TestOWFilesAuxiliary(unittest.TestCase):
 
     def test_numpy_union(self):
         A = np.array([2, 1, 3])
         B = np.array([1, 3])
@@ -30,20 +31,50 @@
         B = np.array([])
         np.testing.assert_equal(numpy_union_keep_order(A, B), [2, 1, 3])
         B = np.array([5, 4, 6, 3])
         np.testing.assert_equal(numpy_union_keep_order(A, B), [2, 1, 3, 5, 4, 6])
         A = np.array([])
         np.testing.assert_equal(numpy_union_keep_order(A, B), [5, 4, 6, 3])
 
+    def test_decimals_neeeded_for_unique_str(self):
+        fn = decimals_neeeded_for_unique_str
+        self.assertEqual(fn([1, 2]), 1)
+        self.assertEqual(fn([1.5, 2.5]), 1)
+        self.assertEqual(fn([1.49, 2.51]), 0)
+        self.assertEqual(fn([10, 20]), 0)
+        self.assertEqual(fn([10.0, 10.1]), 2)
+        self.assertEqual(fn([10.0, 10.2]), 1)
+        self.assertEqual(fn([10.00000001, 10.00000002]), 9)
+        self.assertEqual(fn([10.00000001, 10.000000015, 10.00000002]), 9)
+        self.assertEqual(fn([10.00000001, 10.000000014, 10.00000002]), 9)
+        self.assertEqual(fn([10.00000001, 10.000000013, 10.00000002]), 9)
+        self.assertEqual(fn([10.00000001, 10.000000012, 10.00000002]), 9)
+        self.assertEqual(fn([10.00000001, 10.000000011, 10.00000002]), 10)
+
+    def test_wns_to_unique_str(self):
+        names = wns_to_unique_str([1, 2, 2 + 1e-10, 3])
+        self.assertEqual(names, ['1.000000', '2.000000000000', '2.000000000100', '3.000000'])
+        names = wns_to_unique_str([1, 2, 2 + 0.99e-10, 3])
+        self.assertEqual(names, ['1.000000', '2.000000000000', '2.000000000099', '3.000000'])
+        names = wns_to_unique_str([4, 1, 2, 2 + 0.99e-10, 3])
+        self.assertEqual(names, ['4.000000', '1.000000', '2.000000000000', '2.000000000099', '3.000000'])
+        names = wns_to_unique_str([2+2e-10, 1, 2, 2 + 1e-10, 3])
+        self.assertEqual(names, ['2.000000000200', '1.000000', '2.000000000000', '2.000000000100', '3.000000'])
+
 
 class TestOWMultifile(WidgetTest):
 
     def setUp(self):
         self.widget = self.create_widget(OWMultifile)  # type: OWMultifile
 
+    def tearDown(self):
+        super().tearDown()
+        # clear FileFormat cache so the optional new classes are thrown out
+        FileFormat._ext_to_attr_if_attr2.cache_clear()
+
     def test_load_unload(self):
         # just to load the widget (it has no inputs)
         pass
 
     def load_files(self, *files, reader=None):
         files = [FileFormat.locate(name, dataset_dirs) for name in files]
 
@@ -195,16 +226,35 @@
                                                    "SPAReader": CountSPAReader}):
             # clear LRU cache so that new classes get use
             FileFormat._ext_to_attr_if_attr2.cache_clear()
             self.load_files("titanic.tab", "sample1.spa")
             self.assertEqual(CountSPAReader.read_count, 0)
             self.assertEqual(CountSPAReader.read_spectra_count, 1)
             self.assertEqual(CountTabReader.read_count, 1)
-            # clear cache so the new classes are thrown out
+
+    def test_spectra_almost_same_wavenumbers(self):
+
+        class ReadImaginaryFile(SPAReader):
+            read_count = -1
+
+            def read_spectra(self):
+                type(self).read_count += 1
+                if type(self).read_count == 0:
+                    return np.array([1, 2]), np.array([[42, 41]]), None
+                return np.array([1, 2 + 1e-10]), np.array([[43, 44]]), None
+
+        with patch.object(FileFormat, "registry", {"SPAReader": ReadImaginaryFile}):
+            # clear LRU cache so that new classes get use
             FileFormat._ext_to_attr_if_attr2.cache_clear()
+            self.load_files("sample1.spa", "sample1.spa")
+            out = self.get_output("Data")
+            np.testing.assert_equal(out.X, [[42, 41, np.nan],
+                                            [43, np.nan, 44]])
+            self.assertEqual([a.name for a in out.domain.attributes],
+                             ['1.000000', '2.000000000000', '2.000000000100'])
 
     def test_report_on_empty(self):
         self.widget.send_report()
 
     def test_report_files(self):
         self.load_files("iris", "iris")
         self.widget.send_report()
```

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owpeakfit.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owpeakfit.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owpls.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owpls.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owpreprocess.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owpreprocess.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owreshape.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owreshape.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owsnr.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owsnr.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owspectra.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owspectra.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_owspectralseries.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_owspectralseries.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_preprocess.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_readers.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_readers.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_tile_reader.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_tile_reader.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_utils.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_widgets_utils.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_widgets_utils.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/test_xas.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/test_xas.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/time_interpolation.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/time_interpolation.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/time_irfft.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/time_irfft.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/time_preprocess.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/time_preprocess.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tests/util.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tests/util.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/tutorials/tile-loader.ows` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/tutorials/tile-loader.ows`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/__init__.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/agilent.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/agilent.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/binning.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/binning.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/pymca5/DataObject.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/pymca5/DataObject.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/pymca5/OmnicMap.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/pymca5/OmnicMap.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/skimage/README.txt` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/skimage/README.txt`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/skimage/register_translation.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/skimage/register_translation.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/skimage/shape.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/skimage/shape.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/spc/global_fun.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/spc/global_fun.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/spc/spc.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/spc/spc.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/utils/spc/sub.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/utils/spc/sub.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/__init__.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/gui.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/gui.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/PLS.svg` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/PLS.svg`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/average.svg` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/average.svg`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/bin.svg` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/bin.svg`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/category.svg` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/category.svg`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/fft.svg` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/fft.svg`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/hyper.svg` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/hyper.svg`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/integrate.svg` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/integrate.svg`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/interpolate.svg` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/interpolate.svg`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/multifile.svg` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/multifile.svg`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/mywidget.svg` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/mywidget.svg`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/peakfit.svg` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/peakfit.svg`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/preprocess.svg` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/preprocess.svg`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/reshape.svg` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/reshape.svg`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/snr.svg` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/snr.svg`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/spectra.svg` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/spectra.svg`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/spectralseries.svg` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/spectralseries.svg`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/icons/tilefile.svg` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/icons/tilefile.svg`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/line_geometry.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/line_geometry.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owaverage.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owaverage.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owbin.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owbin.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owfft.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owfft.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owhyper.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owhyper.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owintegrate.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owintegrate.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owinterpolate.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owinterpolate.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owmultifile.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owmultifile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import math
 import os
 from functools import reduce
 from itertools import chain, count, repeat
-from collections import Counter, namedtuple
+from collections import Counter, namedtuple, defaultdict
 from typing import List
 
 import numpy as np
 
 from AnyQt.QtCore import Qt
 from AnyQt.QtWidgets import QSizePolicy as Policy, QGridLayout, QLabel, \
     QFileDialog, QStyle, QListWidget
@@ -37,27 +38,71 @@
 
     # take the missing elements in the correct order
     to_add = B[sorted(orig_sind[indices])]
 
     return np.concatenate((A, to_add))
 
 
+def decimals_neeeded_for_unique_str(l):
+    min_diff = min(np.abs(np.diff(sorted(l))))
+    log_diff = math.log(min_diff, 10)
+    # We need to avoid possible degenerate cases like (1.5, 2.5):
+    # the log of the difference (1.0) is 0, but rounded to zero
+    # decimals we would get (2, 2) due to floating point rounding behavior.
+    # Therefore, slightly increase the number of needed decimals.
+    # The number was selected such that (1.5, 2.5) returned 1 decimal,
+    # and (1.49, 2.51) returned 0.
+    log_diff = log_diff - 0.008
+    decimals = max(0, math.ceil(-log_diff))
+    return decimals
+
+
+def wns_to_unique_str(l):
+    """ Convert a list on wns to a list of unique strings.
+
+    Use 6 decimal places by default. If that is not sufficient,
+    increase precision as needed for wns in conflict.
+    """
+
+    # 6 used to be the default: "%f" means "%0.6f"
+    default_decimals = 6
+    default_format = "%0." + str(default_decimals) + "f"
+
+    same = defaultdict(list)
+    for wn in l:
+        same[default_format % wn].append(wn)
+
+    decimals = {}
+    for n in same:
+        if len(same[n]) == 1:
+            decimals[n] = default_decimals
+        else:
+            # add one decimal place because without it the error could be too big
+            # for example, (1.49, 2.51) would round to 1 and 3, with an added decimal
+            # it will show (1.5, 2.5). Max error before was 0.5*last_decimal_place,
+            # which seems too big.
+            decimals[n] = decimals_neeeded_for_unique_str(same[n]) + 1
+
+    return [("%0." + str(decimals[default_format % wn]) + "f") % wn for wn in l]
+
+
 def concatenate_data(tables, filenames, label):
     if not tables:
         return None
 
     orig_tables = tables
 
     # prepare xs from the spectral specific tables for join into a common domain
     spectral_specific_domains = []
     xss = [t.special_spectral_data[0] for t in tables
            if hasattr(t, "special_spectral_data")]
     xs = reduce(numpy_union_keep_order, xss, np.array([]))
     if len(xs):
-        attrs = [ContinuousVariable("%f" % f) for f in xs]
+        names = wns_to_unique_str(xs)
+        attrs = [ContinuousVariable(n) for n in names]
         spectral_specific_domains = [Domain(attrs, None, None)]
 
     domain = _merge_domains(spectral_specific_domains + [table.domain for table in tables])
     name = get_unique_names(domain, "Filename")
     source_var = StringVariable(name)
     name = get_unique_names(domain, "Label")
     label_var = StringVariable(name)
```

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owpeakfit.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owpeakfit.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owpls.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owpls.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owpreprocess.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owpreprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from Orange.widgets.data.utils.preprocess import SequenceFlow, Controller, \
     StandardItemModel
 from Orange.widgets.data.owpreprocess import (
     PreprocessAction, Description, icon_path, DescriptionRole, ParametersRole, blocked
 )
 from Orange.widgets.utils.sql import check_sql_input
 from Orange.widgets.utils.overlay import OverlayWidget
-from Orange.widgets.utils.colorpalette import DefaultColorBrewerPalette
 from Orange.widgets.utils.concurrent import TaskState, ConcurrentWidgetMixin, ConcurrentMixin
 
 from AnyQt.QtCore import (
     Qt, QEvent, QSize, QMimeData, QTimer
 )
 from AnyQt.QtWidgets import (
     QWidget, QListView, QVBoxLayout, QSizePolicy, QStyle,
@@ -36,15 +35,17 @@
 from orangecontrib.spectroscopy.preprocess.utils import PreprocessException
 from orangecontrib.spectroscopy.widgets.owspectra import CurvePlot, NoSuchCurve
 from orangecontrib.spectroscopy.widgets.preprocessors.misc import SavitzkyGolayFilteringEditor
 from orangecontrib.spectroscopy.widgets.preprocessors.utils import REFERENCE_DATA_PARAM
 from orangecontrib.spectroscopy.widgets.preprocessors.registry import preprocess_editors
 
 
-PREVIEW_COLORS = [QColor(*a).name() for a in DefaultColorBrewerPalette[8]]
+BREWER_PALETTE8 = [(127, 201, 127), (190, 174, 212), (253, 192, 134), (255, 255, 153),
+                   (56, 108, 176), (240, 2, 127), (191, 91, 23), (102, 102, 102)]
+PREVIEW_COLORS = [QColor(*a).name() for a in BREWER_PALETTE8]
 
 
 class ViewController(Controller):
 
     def createWidgetFor(self, index):
         w = super().createWidgetFor(index)
         w.parent_widget = self.parent()
```

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owreshape.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owreshape.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owsnr.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owsnr.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owspectra.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owspectra.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 import Orange.data
 from Orange.data import DiscreteVariable
 from Orange.widgets.widget import OWWidget, Msg, OWComponent, Input
 from Orange.widgets import gui
 from Orange.widgets.settings import \
     Setting, ContextSetting, DomainContextHandler, SettingProvider
 from Orange.widgets.utils.itemmodels import DomainModel
-from Orange.widgets.utils.colorpalette import ColorPaletteGenerator
 from Orange.widgets.utils.plot import \
     SELECT, PANNING, ZOOMING
 from Orange.widgets.utils import saveplot
 from Orange.widgets.visualize.owscatterplotgraph import LegendItem
 from Orange.widgets.utils.concurrent import TaskState, ConcurrentMixin
 from Orange.widgets.visualize.utils.plotutils import HelpEventDelegate
 
@@ -1409,17 +1408,15 @@
         self.pen_normal.clear()
         self.pen_subset.clear()
         self.pen_selected.clear()
         color_var = self.feature_color
         self.legend.clear()
         palette, legend = False, False
         if color_var is not None:
-            colors = color_var.colors
-            discrete_palette = ColorPaletteGenerator(
-                number_of_colors=len(colors), rgb_colors=colors)
+            discrete_palette = color_var.palette
             palette = [(v, discrete_palette[color_var.to_val(v)]) for v in color_var.values]
             legend = True
         elif self.color_individual:
             palette = [(i, QColor(*c)) for i, c in enumerate(self._color_individual_cycle)]
         if palette:
             for v, color in palette:
                 color = QColor(color)  # copy color
```

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owspectralseries.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owspectralseries.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owstackalign.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owstackalign.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/owtilefile.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/owtilefile.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/peak_editors.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/peak_editors.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/peakfit_compute.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/peakfit_compute.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/als.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/als.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/atm_corr.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/atm_corr.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/baseline.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/baseline.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/emsc.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/emsc.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/integrate.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/integrate.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/me_emsc.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/me_emsc.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/misc.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/misc.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/normalize.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/normalize.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/spikeremoval.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/spikeremoval.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/utils.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/utils.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/preprocessors/xas.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/preprocessors/xas.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/orangecontrib/spectroscopy/widgets/utils.py` & `Orange-Spectroscopy-0.6.9/orangecontrib/spectroscopy/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/pylintrc` & `Orange-Spectroscopy-0.6.9/pylintrc`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/screenshot.png` & `Orange-Spectroscopy-0.6.9/screenshot.png`

 * *Files identical despite different names*

### Comparing `Orange-Spectroscopy-0.6.8/setup.py` & `Orange-Spectroscopy-0.6.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         name="Orange-Spectroscopy",
         python_requires='>3.8.0',
         description='Extends Orange to handle spectral and hyperspectral analysis.',
         long_description=LONG_DESCRIPTION,
         long_description_content_type='text/markdown',
         author='Canadian Light Source, Biolab UL, Soleil, Elettra',
         author_email='marko.toplak@gmail.com',
-        version="0.6.8",
+        version="0.6.9",
         packages=PACKAGES,
         package_data=PACKAGE_DATA,
         data_files=DATA_FILES,
         install_requires=[
             'setuptools>=36.3',  # same as for Orange 3.28
             'pip>=9.0',  # same as for Orange 3.28
             'numpy>=1.18.0',
```

