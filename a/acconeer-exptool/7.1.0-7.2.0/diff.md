# Comparing `tmp/acconeer-exptool-7.1.0.tar.gz` & `tmp/acconeer-exptool-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acconeer-exptool-7.1.0.tar", last modified: Wed Jun 21 08:08:36 2023, max compression
+gzip compressed data, was "acconeer-exptool-7.2.0.tar", last modified: Tue Jul  4 08:42:24 2023, max compression
```

## Comparing `acconeer-exptool-7.1.0.tar` & `acconeer-exptool-7.2.0.tar`

### file list

```diff
@@ -1,621 +1,624 @@
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.701143 acconeer-exptool-7.1.0/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/.gitattributes
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.633143 acconeer-exptool-7.1.0/.github/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.641143 acconeer-exptool-7.1.0/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      877 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      368 2023-03-03 12:25:40.000000 acconeer-exptool-7.1.0/.gitignore
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      158 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/.readthedocs.yaml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14786 2023-06-21 08:08:21.000000 acconeer-exptool-7.1.0/CHANGELOG.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13663 2023-04-03 10:32:44.000000 acconeer-exptool-7.1.0/Jenkinsfile
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1881 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/LICENSE.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      217 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/MANIFEST.in
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8990 2023-06-21 08:08:36.701143 acconeer-exptool-7.1.0/PKG-INFO
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7948 2023-04-04 08:04:50.000000 acconeer-exptool-7.1.0/README.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       86 2023-06-21 08:08:21.000000 acconeer-exptool-7.1.0/UNRELEASED_CHANGELOG.md
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.641143 acconeer-exptool-7.1.0/docker/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1865 2023-03-03 13:14:28.000000 acconeer-exptool-7.1.0/docker/Dockerfile
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       82 2023-03-03 12:25:40.000000 acconeer-exptool-7.1.0/docker/requirements-dev.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1604 2023-03-27 08:58:09.000000 acconeer-exptool-7.1.0/dodo.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.633143 acconeer-exptool-7.1.0/examples/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.641143 acconeer-exptool-7.1.0/examples/a111/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3247 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/basic.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1819 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/basic_continuous.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2657 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/load_record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1273 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/load_record_h5.m
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.641143 acconeer-exptool-7.1.0/examples/a111/plotting/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1999 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/plotting/plot_with_matplotlib.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2551 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/plotting/plot_with_pyqtgraph.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.641143 acconeer-exptool-7.1.0/examples/a111/record_data/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1156 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/record_data/barebones.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2541 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/record_data/long_duration_split_files.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1958 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/record_data/with_cli.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.641143 acconeer-exptool-7.1.0/examples/a111/services/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2251 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/services/envelope.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3013 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/services/iq.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2277 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/services/power_bins.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2861 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/services/sparse.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.641143 acconeer-exptool-7.1.0/examples/a111/utils/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      802 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/utils/ping.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      805 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/utils/test_throughput.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/examples/a121/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1222 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/basic.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/examples/a121/bilateration/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8174 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/bilateration/bilaterator.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/examples/a121/distance/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4522 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/distance/detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5053 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/distance/processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      776 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/extended_config.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1518 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a121/load_record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1405 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a121/load_record_h5.m
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/examples/a121/phase_tracking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5808 2023-04-11 13:56:57.000000 acconeer-exptool-7.1.0/examples/a121/phase_tracking/phase_tracking.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4538 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/plot.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/examples/a121/presence/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11241 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/presence/detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11026 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/presence/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/examples/a121/record_data/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      975 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/examples/a121/record_data/barebones.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1017 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/examples/a121/record_data/with_cli.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1140 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/reuse_calibration.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/examples/a121/smart_presence/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10430 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/smart_presence/processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9497 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/smart_presence/ref_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4253 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/stress.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      946 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/subsweeps.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/examples/a121/surface_velocity/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8515 2023-04-17 09:00:31.000000 acconeer-exptool-7.1.0/examples/a121/surface_velocity/example_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8864 2023-04-17 09:00:31.000000 acconeer-exptool-7.1.0/examples/a121/surface_velocity/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/examples/a121/touchless_button/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3927 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/touchless_button/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/examples/a121/vibration/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4410 2023-04-28 14:58:15.000000 acconeer-exptool-7.1.0/examples/a121/vibration/vibration.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/gui/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1254 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/gui/main.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6585 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/noxfile.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/portable/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       27 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/portable/.gitignore
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1571 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/portable/make.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/portable/package/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      108 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/portable/package/cmd_with_path.bat
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      346 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/portable/package/run_app.bat
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.649143 acconeer-exptool-7.1.0/portable/package/tools/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      989 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/portable/package/tools/update.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      168 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/portable/package/update.bat
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2361 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/pyproject.toml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2433 2023-06-21 08:08:36.705143 acconeer-exptool-7.1.0/setup.cfg
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.637143 acconeer-exptool-7.1.0/src/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.633143 acconeer-exptool-7.1.0/src/acconeer/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.649143 acconeer-exptool-7.1.0/src/acconeer/exptool/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      295 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3212 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_bs_thread.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.649143 acconeer-exptool-7.1.0/src/acconeer/exptool/_pyusb/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      100 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_pyusb/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5890 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_pyusb/pyusbcomm.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.649143 acconeer-exptool-7.1.0/src/acconeer/exptool/_structs/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_structs/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15542 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_structs/configbase.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15673 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_structs/qtpidgets.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.649143 acconeer-exptool-7.1.0/src/acconeer/exptool/_tests/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_tests/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4259 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_tests/test_rig.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       22 2023-06-21 08:08:36.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_version.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.649143 acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1071 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/LICENSE
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      190 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2847 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6837 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/usb_cdc.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2021 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/winusb.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3466 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/winusbclasses.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      231 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/winusberror.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10029 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/winusbpy.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12307 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/winusbutils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.649143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      438 2023-04-03 10:32:44.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.653143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      119 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7940 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5916 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5513 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/client_factory.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      517 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/common.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.653143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/json/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/json/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18330 2023-03-03 12:25:40.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/json/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14209 2023-03-03 12:25:40.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/links.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.653143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/mock/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/mock/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7621 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/mock/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1496 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/multiwrap.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.653143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24884 2023-05-12 09:53:24.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/client.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.653143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/data/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/data/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8068 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6351 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/protocol.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9853 2023-04-03 10:32:44.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/regmap.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7176 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_conf_to_rss_sdk.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    28007 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      587 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_modes.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3710 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.653143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      242 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.653143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/_base/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2708 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/_base/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      860 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/_base/module_info.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1695 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/_standalone_main.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.653143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/breathing/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/breathing/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      538 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/breathing/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7469 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/breathing/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4554 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/breathing/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.653143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      618 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6054 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5308 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.657143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press_sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press_sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press_sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11319 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press_sparse/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4931 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.657143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/distance_detector/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/distance_detector/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/distance_detector/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      948 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/distance_detector/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21416 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/distance_detector/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2204 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/distance_detector/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6126 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/distance_detector/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.657143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/envelope/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/envelope/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/envelope/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      862 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/envelope/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3943 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/envelope/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/envelope/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5280 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/envelope/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.657143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/iq/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/iq/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/iq/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      565 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/iq/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1985 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/iq/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3928 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/iq/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.657143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      939 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27784 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9166 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      104 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    16847 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.661143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/parking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/parking/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/parking/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      890 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/parking/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9162 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/parking/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8503 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/parking/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.661143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/phase_tracking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      110 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/phase_tracking/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/phase_tracking/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      576 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2599 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4172 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/phase_tracking/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.661143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/power_bins/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       99 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/power_bins/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/power_bins/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      612 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/power_bins/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/power_bins/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1400 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/power_bins/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.661143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15250 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13885 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.661143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      917 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14079 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10519 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.661143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sleep_breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sleep_breathing/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sleep_breathing/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      615 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10381 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4623 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.665143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5079 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.665143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_fft/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_fft/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_fft/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1341 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4454 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_fft/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.665143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      557 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5185 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5472 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.665143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/speed_sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/speed_sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/speed_sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      824 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12380 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      186 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/speed_sparse/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7812 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/speed_sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.665143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/tank_level_short/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/tank_level_short/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/tank_level_short/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10409 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3125 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/tank_level_short/ui.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2560 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.669143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/wave_to_exit/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/wave_to_exit/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/wave_to_exit/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      545 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4662 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6099 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9009 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/recording.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.669143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1207 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1790 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_cli.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.669143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      989 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.669143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      690 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.669143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4195 2023-03-29 12:24:17.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    22075 2023-06-20 07:07:07.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10223 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/session_config.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11207 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1035 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.669143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      607 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8821 2023-04-17 09:35:06.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/client_info.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4798 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/metadata.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8216 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2192 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/result.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1351 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2906 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/server_info.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/server_log_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2189 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1675 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      144 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/dtypes.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.669143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/mediators/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      150 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/mediators/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      931 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/mediators/link.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1265 2023-05-15 11:16:12.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/mediators/recorder.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.669143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      401 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.669143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      439 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7119 2023-05-15 11:16:12.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5053 2023-05-15 11:16:12.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1324 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15568 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.673143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      403 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1023 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6512 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      985 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1037 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.673143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      521 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      687 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1150 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       96 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/parse_error.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4314 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1123 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      752 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2836 2023-02-27 12:43:10.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1045 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      791 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       97 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/server_error.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1998 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/links.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      643 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11369 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3996 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.673143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      276 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8225 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3012 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12719 2023-05-15 11:16:12.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1526 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/session_schema.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      928 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.673143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/im_record/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       95 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/im_record/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3543 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18924 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.673143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core_ext/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      118 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core_ext/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4868 2023-05-29 14:09:50.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core_ext/_replaying_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      318 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_h5_utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7945 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_perf_calc.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2516 2023-02-27 12:43:10.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_rate_calc.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.673143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      720 2023-06-12 13:00:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4086 2023-04-17 09:23:23.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_base.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.673143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      367 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7933 2023-06-02 14:43:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/_a121.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      434 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/_detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      617 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3783 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.673143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/processor/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      446 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/processor/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8320 2023-06-02 14:43:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1276 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6615 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10729 2023-06-12 13:00:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.673143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/bilateration/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/bilateration/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      395 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/bilateration/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24992 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/bilateration/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    17474 2023-03-29 12:24:17.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/bilateration/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.677143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      303 2023-06-12 13:00:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/breathing/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      759 2023-06-12 13:00:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/breathing/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    20031 2023-06-12 13:00:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/breathing/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8542 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/breathing/_ref_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    31517 2023-06-12 13:00:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/breathing/_ref_app_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6541 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/breathing/_serializer.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.677143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      507 2023-03-29 12:24:17.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      855 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5471 2023-03-29 12:24:17.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/_aggregator.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      307 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    59448 2023-06-20 13:22:54.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/_detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    26179 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    30450 2023-06-20 13:22:54.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/_processors.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15812 2023-03-29 12:24:17.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.677143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/phase_tracking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/phase_tracking/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/phase_tracking/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7575 2023-03-03 13:14:28.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7141 2023-06-20 13:22:54.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.677143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      235 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2175 2023-03-13 14:50:09.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14812 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/_detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    29697 2023-06-21 08:00:20.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18288 2023-06-20 13:22:54.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/_processors.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4717 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.677143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/smart_presence/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      182 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/smart_presence/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2223 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/smart_presence/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6607 2023-03-23 08:31:28.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/smart_presence/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7165 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21790 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6835 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/smart_presence/_serializer.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.677143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/sparse_iq/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      220 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/sparse_iq/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/sparse_iq/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8167 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3116 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7245 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.677143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/speed/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      213 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/speed/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      347 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/speed/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14231 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/speed/_detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21150 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/speed/_detector_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4909 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/speed/_processors.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.681143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/surface_velocity/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      130 2023-03-24 13:36:14.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/surface_velocity/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11611 2023-05-16 12:47:42.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21732 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14090 2023-06-20 13:22:54.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.681143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      219 2023-03-22 21:29:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1658 2023-03-29 12:24:17.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    29464 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7290 2023-06-20 13:22:54.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6265 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4229 2023-03-22 21:29:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/_serializer.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.681143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      306 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      486 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1100 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1738 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7687 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14754 2023-06-01 09:22:41.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2896 2023-03-29 12:24:17.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.681143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/vibration/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/vibration/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/vibration/__main__,py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8514 2023-04-28 14:58:15.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/vibration/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7628 2023-06-20 13:22:54.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/vibration/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/py.typed
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.681143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      333 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4475 2023-03-31 10:16:50.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/launcher.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.681143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      909 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      994 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/_argument_parser.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1718 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/_enums.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      102 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/_exceptions.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      983 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/_version_checker.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2698 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.681143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app_model/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      239 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app_model/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27095 2023-06-21 08:08:21.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app_model/app_model.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app_model/app_model_listener.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      981 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app_model/file_detective.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      428 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app_model/plugin_protocols.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2074 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app_model/port_updater.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.685143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      478 2023-06-02 14:43:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2737 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_application_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4985 2023-06-02 14:43:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_backend.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1610 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_backend_logger.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2040 2023-06-02 14:43:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_backend_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1559 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4770 2023-06-02 14:43:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_model.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2786 2023-06-02 14:43:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_tasks.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1685 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/plugin_loader.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.685143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/pluginbase/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      241 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/pluginbase/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      973 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      431 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/pluginbase/plugin_preset_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1024 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1836 2023-06-02 14:43:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/py.typed
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      470 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/qt_subclasses.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      804 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/storage.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.685143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      445 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2141 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/app_model_viewer.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2641 2023-04-11 13:56:57.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/device_comboboxes.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.685143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/flash_tab/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       94 2023-04-21 06:43:18.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/flash_tab/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14023 2023-04-21 06:43:18.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4635 2023-04-19 09:25:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/flash_tab/threads.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15274 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1802 2023-04-21 06:43:18.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/help_tab.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2142 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/icons.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3910 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/main_window.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1968 2023-04-11 13:56:57.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/misc.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.685143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      798 2023-06-14 14:27:03.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7130 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1290 2023-03-13 14:50:09.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1026 2023-04-19 09:25:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6271 2023-06-14 14:27:03.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/json_save_load_buttons.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6159 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1432 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3612 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.689143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      769 2023-03-03 13:14:28.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      499 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/common.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3814 2023-04-19 09:25:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2082 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27081 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2004 2023-04-28 14:58:15.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.689143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      227 2023-06-14 14:27:03.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1757 2023-06-14 14:27:03.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/dialog.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6112 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/preview.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4004 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/set_config_presenter.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13043 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6682 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7963 2023-04-19 09:25:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1887 2023-04-19 09:25:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      294 2023-04-19 09:25:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/types.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3848 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9480 2023-04-11 13:26:50.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/status_bar.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.689143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       98 2023-04-11 13:56:57.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10441 2023-04-11 13:56:57.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5853 2023-04-11 13:56:57.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/hints.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12509 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4551 2023-04-11 13:56:57.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2636 2023-04-21 06:43:18.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1382 2023-04-21 06:43:18.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.689143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    84005 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4735 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/data_processing.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.689143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/elements/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/elements/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8476 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/elements/helper.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2346 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/elements/modules.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10745 2023-05-12 09:53:24.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/elements/qt_subclasses.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.689143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    90184 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/a111_gui.png
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    57036 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/a121_gui.png
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4162 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/icon-black.svg
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    35706 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/icon.png
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3208 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/loader.gif
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.637143 acconeer-exptool-7.1.0/src/acconeer/exptool/data/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.689143 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1245 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/LICENSE.txt
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.693143 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/aarch64/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   513305 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.693143 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/amd64/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   209008 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   314552 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.693143 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/armv6/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   484176 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.693143 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/armv7/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   399731 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.697143 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/i386/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   160256 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   271672 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.697143 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/x86_64/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   504389 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.697143 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      338 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      115 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5843 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_bin_fetcher.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3629 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_dev_license.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4284 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_dev_license_tui.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      416 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_device_flasher_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12868 2023-04-04 08:04:50.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_flasher.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      828 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_products.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.697143 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_stm32uart/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      150 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_stm32uart/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      274 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_stm32uart/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6665 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.697143 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_xc120/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      258 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_xc120/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9147 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9417 2023-04-21 13:00:24.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      224 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_xc120/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11051 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/libft4222.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3338 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/mpl_process.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3185 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/pg_process.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.697143 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/__main__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.701143 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      244 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1431 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/platform_install.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      980 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/prompts.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      690 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/setup_group.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/setup_step.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      520 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.701143 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/cli/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      106 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/cli/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      684 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/cli/argument_parser.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.701143 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/platforms/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/platforms/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/platforms/how_to.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1867 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/platforms/linux.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/py.typed
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21469 2023-03-22 21:29:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.701143 acconeer-exptool-7.1.0/src/acconeer_exptool.egg-info/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8990 2023-06-21 08:08:36.000000 acconeer-exptool-7.1.0/src/acconeer_exptool.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    26248 2023-06-21 08:08:36.000000 acconeer-exptool-7.1.0/src/acconeer_exptool.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-06-21 08:08:36.000000 acconeer-exptool-7.1.0/src/acconeer_exptool.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-06-21 08:08:36.000000 acconeer-exptool-7.1.0/src/acconeer_exptool.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      475 2023-06-21 08:08:36.000000 acconeer-exptool-7.1.0/src/acconeer_exptool.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        9 2023-06-21 08:08:36.000000 acconeer-exptool-7.1.0/src/acconeer_exptool.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.701143 acconeer-exptool-7.1.0/tools/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3930 2023-06-21 08:08:21.000000 acconeer-exptool-7.1.0/tools/check_changelog.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12005 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/tools/check_copyright.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/tools/check_line_length.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1495 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/tools/check_permissions.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4237 2023-04-03 10:32:44.000000 acconeer-exptool-7.1.0/tools/check_sdk_mentions.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1801 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/tools/check_whitespace.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2064 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/tools/update_regmap.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.701143 acconeer-exptool-7.1.0/utils/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14756 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/utils/convert_to_csv.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/.gitattributes
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.335974 acconeer-exptool-7.2.0/.github/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.339974 acconeer-exptool-7.2.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      877 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      368 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/.gitignore
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      158 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/.readthedocs.yaml
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15293 2023-07-04 08:38:59.000000 acconeer-exptool-7.2.0/CHANGELOG.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13663 2023-07-04 08:36:53.000000 acconeer-exptool-7.2.0/Jenkinsfile
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1881 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/LICENSE.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      217 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8990 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/PKG-INFO
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7948 2023-07-04 08:36:53.000000 acconeer-exptool-7.2.0/README.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       86 2023-07-04 08:38:59.000000 acconeer-exptool-7.2.0/UNRELEASED_CHANGELOG.md
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.339974 acconeer-exptool-7.2.0/docker/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1865 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/docker/Dockerfile
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       82 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/docker/requirements-dev.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1604 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/dodo.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.335974 acconeer-exptool-7.2.0/examples/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.339974 acconeer-exptool-7.2.0/examples/a111/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3247 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/basic.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1819 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/basic_continuous.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2657 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/load_record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1273 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/load_record_h5.m
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.339974 acconeer-exptool-7.2.0/examples/a111/plotting/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1999 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/plotting/plot_with_matplotlib.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2551 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/plotting/plot_with_pyqtgraph.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.339974 acconeer-exptool-7.2.0/examples/a111/record_data/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1156 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/record_data/barebones.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2541 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/record_data/long_duration_split_files.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1958 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/record_data/with_cli.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.339974 acconeer-exptool-7.2.0/examples/a111/services/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2251 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/services/envelope.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3013 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/services/iq.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2277 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/services/power_bins.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2861 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/services/sparse.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.339974 acconeer-exptool-7.2.0/examples/a111/utils/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      802 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/utils/ping.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      805 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/utils/test_throughput.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/examples/a121/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1222 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/basic.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/examples/a121/bilateration/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8174 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/bilateration/bilaterator.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/examples/a121/distance/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4522 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/distance/detector.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5053 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/distance/processor.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      776 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/extended_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1518 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a121/load_record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1405 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a121/load_record_h5.m
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/examples/a121/phase_tracking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5808 2023-04-11 14:12:33.000000 acconeer-exptool-7.2.0/examples/a121/phase_tracking/phase_tracking.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4538 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/plot.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/examples/a121/presence/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11241 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/presence/detector.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11026 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/presence/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/examples/a121/record_data/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      975 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/examples/a121/record_data/barebones.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1017 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/examples/a121/record_data/with_cli.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1140 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/reuse_calibration.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/examples/a121/smart_presence/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10430 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/smart_presence/processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    17513 2023-07-03 11:33:15.000000 acconeer-exptool-7.2.0/examples/a121/smart_presence/ref_app.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/examples/a121/speed/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9030 2023-07-03 12:00:03.000000 acconeer-exptool-7.2.0/examples/a121/speed/detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9179 2023-07-03 12:00:03.000000 acconeer-exptool-7.2.0/examples/a121/speed/processor.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4253 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/stress.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      946 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/subsweeps.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/examples/a121/surface_velocity/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8515 2023-04-17 09:00:03.000000 acconeer-exptool-7.2.0/examples/a121/surface_velocity/example_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8864 2023-04-17 09:00:03.000000 acconeer-exptool-7.2.0/examples/a121/surface_velocity/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/examples/a121/touchless_button/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3927 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/touchless_button/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/examples/a121/vibration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4410 2023-04-28 09:00:03.000000 acconeer-exptool-7.2.0/examples/a121/vibration/vibration.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/gui/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1254 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/gui/main.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6585 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/noxfile.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/portable/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       27 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/portable/.gitignore
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1571 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/portable/make.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/portable/package/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      108 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/portable/package/cmd_with_path.bat
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      346 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/portable/package/run_app.bat
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/portable/package/tools/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      989 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/portable/package/tools/update.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      168 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/portable/package/update.bat
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2361 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/pyproject.toml
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2433 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/setup.cfg
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.339974 acconeer-exptool-7.2.0/src/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.335974 acconeer-exptool-7.2.0/src/acconeer/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/src/acconeer/exptool/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      295 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3212 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_bs_thread.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/src/acconeer/exptool/_pyusb/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      100 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_pyusb/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5890 2023-01-24 10:54:24.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_pyusb/pyusbcomm.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/src/acconeer/exptool/_structs/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_structs/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15542 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_structs/configbase.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15673 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_structs/qtpidgets.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/src/acconeer/exptool/_tests/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_tests/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4259 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_tests/test_rig.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       22 2023-07-04 08:42:24.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_version.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1071 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/LICENSE
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      190 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2847 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6837 2023-01-27 07:25:26.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/usb_cdc.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2021 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/winusb.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3466 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/winusbclasses.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      231 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/winusberror.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10029 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/winusbpy.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12307 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/winusbutils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      438 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      119 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7940 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5916 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5513 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/client_factory.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      517 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/common.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/json/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/json/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18330 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/json/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14209 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/links.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/mock/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/mock/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7621 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/mock/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1496 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/multiwrap.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24884 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/client.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/data/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/data/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8068 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6351 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/protocol.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9853 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/regmap.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7176 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_conf_to_rss_sdk.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    28007 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      587 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_modes.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3710 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      242 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/_base/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2708 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/_base/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      860 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/_base/module_info.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1695 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/_standalone_main.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/breathing/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/breathing/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      538 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/breathing/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7469 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/breathing/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4554 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/breathing/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      618 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6054 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5308 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press_sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press_sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press_sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11319 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press_sparse/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4931 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/distance_detector/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/distance_detector/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/distance_detector/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      948 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/distance_detector/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21416 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/distance_detector/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2204 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/distance_detector/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6126 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/distance_detector/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/envelope/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/envelope/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/envelope/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      862 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/envelope/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3943 2022-12-29 10:02:50.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/envelope/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/envelope/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5280 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/envelope/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/iq/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/iq/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/iq/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      565 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/iq/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1985 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/iq/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3928 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/iq/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.351974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      939 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27784 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9166 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      104 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    16847 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.351974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/parking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/parking/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/parking/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      890 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/parking/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9162 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/parking/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8503 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/parking/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.351974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/phase_tracking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      110 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/phase_tracking/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/phase_tracking/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      576 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2599 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4172 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/phase_tracking/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.351974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/power_bins/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       99 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/power_bins/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/power_bins/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      612 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/power_bins/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/power_bins/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1400 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/power_bins/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.351974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-23 12:52:12.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-23 12:52:12.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2023-02-23 12:52:12.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15250 2023-02-23 12:52:12.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13885 2023-02-23 12:52:12.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.351974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      917 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14079 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10519 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.351974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sleep_breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sleep_breathing/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sleep_breathing/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      615 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10381 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4623 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.351974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5079 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.351974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_fft/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_fft/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_fft/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1341 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4454 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_fft/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.351974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      557 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5185 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5472 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.351974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/speed_sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/speed_sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/speed_sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      824 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12380 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      186 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/speed_sparse/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7812 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/speed_sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.355974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/tank_level_short/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/tank_level_short/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/tank_level_short/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10409 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3125 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/tank_level_short/ui.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2560 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.355974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/wave_to_exit/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/wave_to_exit/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/wave_to_exit/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      545 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4662 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6099 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9009 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/recording.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.355974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1207 2023-07-04 08:36:53.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1790 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_cli.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.355974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      989 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.355974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      690 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.355974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2023-02-08 08:37:09.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4195 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    22075 2023-06-20 09:52:28.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10223 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/session_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11481 2023-07-04 08:07:41.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1035 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.355974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      607 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8821 2023-04-17 12:37:45.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/client_info.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4798 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/metadata.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8216 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2192 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/result.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1351 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2906 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/server_info.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/server_log_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2189 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1675 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/utils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      144 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/dtypes.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.355974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/mediators/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      150 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/mediators/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      931 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/mediators/link.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1265 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/mediators/recorder.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.355974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      401 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.355974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      439 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6983 2023-07-03 12:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5053 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1324 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15557 2023-07-03 12:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.359974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      403 2023-02-13 09:23:58.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1023 2023-02-13 09:23:58.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6512 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      985 2023-02-13 09:23:58.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1037 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.359974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      521 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      687 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1150 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       96 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/parse_error.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4314 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1123 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      752 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2836 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1045 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      791 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       97 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/server_error.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1998 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/links.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      643 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11180 2023-07-03 12:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3996 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.359974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      276 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8225 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3012 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12719 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1526 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/session_schema.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      928 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.359974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/im_record/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       95 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/im_record/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3543 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18924 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.359974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core_ext/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      118 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core_ext/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4868 2023-05-31 21:00:04.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core_ext/_replaying_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      318 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_h5_utils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7945 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_perf_calc.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2516 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_rate_calc.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.359974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      720 2023-06-15 10:34:10.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4086 2023-04-17 12:37:45.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_base.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.359974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      367 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8056 2023-07-04 08:07:41.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/_a121.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      434 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      617 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3783 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.359974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/processor/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      446 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/processor/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8320 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1276 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6615 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10729 2023-06-15 10:34:10.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.359974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/bilateration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2023-02-06 10:47:51.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/bilateration/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      395 2023-03-28 07:00:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/bilateration/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24992 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/bilateration/_plugin.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    17474 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/bilateration/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.359974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      303 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      759 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    20031 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8542 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/_ref_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    31517 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/_ref_app_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6541 2023-07-03 12:37:27.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/_serializer.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.359974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      507 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      855 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/__main__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5471 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/_aggregator.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      307 2023-03-28 07:00:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    59450 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    26179 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    30450 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/_processors.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15812 2023-07-03 12:37:27.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/_serializers.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.363974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/phase_tracking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/phase_tracking/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/phase_tracking/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7575 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7141 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.363974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      235 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2856 2023-06-30 11:48:25.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15804 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    30047 2023-06-30 11:48:25.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18288 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/_processors.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4717 2023-07-03 12:37:27.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/_serializers.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.363974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/smart_presence/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      182 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/smart_presence/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8375 2023-06-30 09:00:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/smart_presence/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6607 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/smart_presence/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18184 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    32608 2023-06-30 09:00:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10926 2023-07-03 12:37:27.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/smart_presence/_serializer.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.363974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/sparse_iq/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      220 2023-02-06 16:11:20.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/sparse_iq/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/sparse_iq/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8167 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3116 2023-02-06 16:11:20.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7245 2023-07-03 12:37:27.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.363974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/speed/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      213 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/speed/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      347 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/speed/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14635 2023-06-30 13:44:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/speed/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21150 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/speed/_detector_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4909 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/speed/_processors.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.363974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/surface_velocity/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      130 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/surface_velocity/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11611 2023-05-23 09:13:41.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21732 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14090 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.363974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/tank_level/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      219 2023-06-27 15:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/tank_level/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1658 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/tank_level/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    29464 2023-06-27 15:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/tank_level/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7290 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/tank_level/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6265 2023-06-27 15:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4229 2023-07-03 12:37:27.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/tank_level/_serializer.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.363974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      306 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      486 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1100 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1738 2023-01-27 07:25:26.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7687 2023-03-31 08:15:54.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14754 2023-06-01 09:17:58.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2896 2023-07-03 12:37:27.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/_serializers.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.363974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/vibration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/vibration/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/vibration/__main__,py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8514 2023-04-28 09:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/vibration/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7628 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/vibration/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/py.typed
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.363974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      333 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/__main__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4475 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/launcher.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.367974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      909 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      994 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/_argument_parser.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1718 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/_enums.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      102 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/_exceptions.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      983 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/_version_checker.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2698 2022-12-29 10:02:50.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.367974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app_model/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      239 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app_model/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27095 2023-06-21 08:08:07.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app_model/app_model.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app_model/app_model_listener.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      981 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app_model/file_detective.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      428 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app_model/plugin_protocols.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2074 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app_model/port_updater.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.367974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      478 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2737 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_application_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4985 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_backend.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1610 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_backend_logger.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2040 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_backend_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1559 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4770 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_model.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2786 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_tasks.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1685 2023-07-03 10:00:04.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/plugin_loader.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.367974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/pluginbase/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      241 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/pluginbase/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      973 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      431 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/pluginbase/plugin_preset_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1024 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1836 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/py.typed
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      470 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/qt_subclasses.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      804 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/storage.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.367974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      445 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2141 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/app_model_viewer.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2641 2023-04-11 13:26:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/device_comboboxes.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.367974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/flash_tab/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       94 2023-04-21 07:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/flash_tab/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14023 2023-04-21 07:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4635 2023-04-19 08:17:48.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/flash_tab/threads.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15274 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1802 2023-04-21 07:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/help_tab.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2142 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/icons.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3910 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/main_window.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1968 2023-04-11 13:26:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/misc.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.367974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      798 2023-06-13 21:00:27.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7130 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1290 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1026 2023-04-19 07:00:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6271 2023-06-13 21:00:27.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/json_save_load_buttons.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6159 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1432 2023-03-27 09:23:59.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3612 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      769 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      499 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/common.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3814 2023-04-19 07:00:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2082 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27081 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2004 2023-04-28 09:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      227 2023-06-13 21:00:27.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1757 2023-06-13 21:00:27.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/dialog.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6112 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/preview.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4004 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/set_config_presenter.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13043 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6682 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7963 2023-04-19 07:00:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1887 2023-04-19 07:00:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      294 2023-04-19 07:00:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/types.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3848 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/utils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9480 2023-04-11 13:26:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/status_bar.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       98 2023-04-11 13:26:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10441 2023-04-11 13:26:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4912 2023-06-30 11:48:25.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/hints.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12509 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4551 2023-04-11 13:26:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2636 2023-04-21 07:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1382 2023-04-26 12:00:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    84005 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4735 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/data_processing.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/elements/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/elements/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8476 2022-12-29 10:02:50.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/elements/helper.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2346 2023-02-23 12:52:12.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/elements/modules.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10745 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/elements/qt_subclasses.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    90184 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/a111_gui.png
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    57036 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/a121_gui.png
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4162 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/icon-black.svg
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    35706 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/icon.png
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3208 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/loader.gif
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.339974 acconeer-exptool-7.2.0/src/acconeer/exptool/data/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1245 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/LICENSE.txt
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/aarch64/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   513305 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/amd64/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   209008 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   314552 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/armv6/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   484176 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/armv7/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   399731 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/i386/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   160256 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   271672 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/x86_64/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   504389 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      338 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      115 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5843 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_bin_fetcher.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3629 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_dev_license.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4284 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_dev_license_tui.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      416 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_device_flasher_base.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12868 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_flasher.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      828 2023-01-27 07:25:26.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_products.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_stm32uart/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      150 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_stm32uart/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      274 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_stm32uart/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6665 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_xc120/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      258 2023-01-27 07:25:26.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_xc120/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9147 2023-01-27 07:25:26.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9417 2023-04-21 06:44:46.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      224 2023-01-27 07:25:26.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_xc120/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11051 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/libft4222.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3338 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/mpl_process.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3185 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/pg_process.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2022-12-22 13:05:40.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/__main__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      244 2022-12-22 13:05:40.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1431 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/platform_install.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      980 2022-12-22 13:05:40.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/prompts.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      690 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/setup_group.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2022-12-22 13:05:40.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/setup_step.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      520 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/cli/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      106 2022-12-22 13:05:40.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/cli/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      684 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/cli/argument_parser.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/platforms/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/platforms/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/platforms/how_to.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1867 2022-12-22 13:05:40.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/platforms/linux.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/py.typed
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21469 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/src/acconeer_exptool.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8990 2023-07-04 08:42:24.000000 acconeer-exptool-7.2.0/src/acconeer_exptool.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    26313 2023-07-04 08:42:24.000000 acconeer-exptool-7.2.0/src/acconeer_exptool.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-07-04 08:42:24.000000 acconeer-exptool-7.2.0/src/acconeer_exptool.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-07-04 08:42:23.000000 acconeer-exptool-7.2.0/src/acconeer_exptool.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      475 2023-07-04 08:42:24.000000 acconeer-exptool-7.2.0/src/acconeer_exptool.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        9 2023-07-04 08:42:24.000000 acconeer-exptool-7.2.0/src/acconeer_exptool.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/tools/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3930 2023-06-22 13:14:00.000000 acconeer-exptool-7.2.0/tools/check_changelog.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12005 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/tools/check_copyright.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/tools/check_line_length.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1495 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/tools/check_permissions.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4237 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/tools/check_sdk_mentions.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1801 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/tools/check_whitespace.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2064 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/tools/update_regmap.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/utils/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14763 2023-06-30 11:48:25.000000 acconeer-exptool-7.2.0/utils/convert_to_csv.py
```

### Comparing `acconeer-exptool-7.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `acconeer-exptool-7.2.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/CHANGELOG.md` & `acconeer-exptool-7.2.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,25 @@
 # Changelog
 
+## v7.2.0
+
+### Added
+- A121: Smart presence: Add wake up mode
+- A121: Client now raises an error if no sensors can be detected
+        on the server.
+- Documentation for the speed detector
+- Examples for the speed detector
+- Better handling of unexpected communication errors (lost connection, etc.)
+  in the A121 Client.
+
+### Fixed
+ - A111: convert_to_csv.py can now output metadata for the envelope service
+ - A121: Detach recorded if start_session fails
+ - A121: Validate start point in subsweep config
+
 ## v7.1.0
 
 ### Added
 - New algorithm: Speed detector
 - Config load- & save for the majority of configs in the A121 App.
 - Export some configurations to C via the config save buttons.
   + Sparse IQ
```

### Comparing `acconeer-exptool-7.1.0/Jenkinsfile` & `acconeer-exptool-7.2.0/Jenkinsfile`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     (BuildScope.HOURLY)  : ["3.9"],
     (BuildScope.NIGHTLY) : ["3.7", "3.8", "3.9", "3.10", "3.11"],
 ]
 
 @Field
 def integrationTestA121RssVersionsForBuildScope = [
     (BuildScope.SANITY)  : [branch: "master"],
-    (BuildScope.HOURLY)  : [tag: "a121-v1.0.0"],
-    (BuildScope.NIGHTLY) : [branch: "master", tag: "a121-v1.0.0"],
+    (BuildScope.HOURLY)  : [tag: "a121-v1.1.0"],
+    (BuildScope.NIGHTLY) : [branch: "master", tag: "a121-v1.1.0"],
 ]
 
 @Field
 def integrationTestA111RssVersionsForBuildScope = [
     (BuildScope.SANITY)  : [branch: "master"],
     (BuildScope.HOURLY)  : [],
     (BuildScope.NIGHTLY) : [branch: "master", tag: "a111-v2.14.2"],
@@ -172,15 +172,15 @@
                         printNodeInfo()
                         checkoutAndCleanup()
 
                         findBuildAndCopyArtifacts(
                             [
                                 projectName: 'sw-main',
                                 artifactNames: ["out/internal_stash_binaries_sanitizer_a121.tgz"],
-                            ] << rssVersion // e.g. [branch: 'master'] or [tag: 'a121-v1.0.0']
+                            ] << rssVersion // e.g. [branch: 'master'] or [tag: 'a121-vX.Y.Z']
                         )
                         sh 'mkdir stash'
                         sh 'tar -xzf out/internal_stash_binaries_sanitizer_a121.tgz -C stash'
                     }
                     stage("Run integration tests (py=${integrationTestPythonVersions}, rss=${rssVersionName})") {
                         buildDocker(path: 'docker').inside(dockerArgs(env)) {
                             integrationTestPythonVersions.each { v -> sh "python${v} -V" }
```

### Comparing `acconeer-exptool-7.1.0/LICENSE.md` & `acconeer-exptool-7.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/PKG-INFO` & `acconeer-exptool-7.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acconeer-exptool
-Version: 7.1.0
+Version: 7.2.0
 Summary: Acconeer Exploration Tool
 Home-page: https://github.com/acconeer/acconeer-python-exploration
 Author: Acconeer AB
 Author-email: tools@acconeer.com
 License: BSD 3-Clause Clear License
 Project-URL: Tracker, https://github.com/acconeer/acconeer-python-exploration/issues
 Project-URL: Documentation, https://acconeer-python-exploration.readthedocs.io
@@ -36,15 +36,15 @@
 _**Explore the Next Sense**_ with Acconeer Exploration Tool! Use one of our [evaluation kits](https://www.acconeer.com/products) together with our Python examples and start exploring the world of Acconeer's radar sensor technology. The Python scripts and the Application in this repository will help you to easily stream the radar sensor's data to your local machine to start radar sensor evaluation and/or algorithm development for your application.
 
 To run the Python exploration scripts, you will need an [evaluation kit](https://www.acconeer.com/products) running the included Exploration or Module server, both of which are supplied with the [Acconeer SDK and Module SW](https://developer.acconeer.com/) image.
 
 This release is developed for [Acconeer SDK and Module SW](https://developer.acconeer.com/)
 **A111-v2.14.2**
 and
-**A121-v1.0.0**.
+**A121-v1.1.0**.
 Running this version is strongly recommended, as we continuously fix bugs and add features.
 
 <p align="center">
   <img alt="The application in action" src="https://raw.githubusercontent.com/acconeer/acconeer-python-exploration/8f633e02abac99ffec6fefec4339d13bc5c18388/docs/_static/gui.png" width=85%>
 </p>
 
 ## Quickstart for Windows
```

### Comparing `acconeer-exptool-7.1.0/README.md` & `acconeer-exptool-7.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 _**Explore the Next Sense**_ with Acconeer Exploration Tool! Use one of our [evaluation kits](https://www.acconeer.com/products) together with our Python examples and start exploring the world of Acconeer's radar sensor technology. The Python scripts and the Application in this repository will help you to easily stream the radar sensor's data to your local machine to start radar sensor evaluation and/or algorithm development for your application.
 
 To run the Python exploration scripts, you will need an [evaluation kit](https://www.acconeer.com/products) running the included Exploration or Module server, both of which are supplied with the [Acconeer SDK and Module SW](https://developer.acconeer.com/) image.
 
 This release is developed for [Acconeer SDK and Module SW](https://developer.acconeer.com/)
 **A111-v2.14.2**
 and
-**A121-v1.0.0**.
+**A121-v1.1.0**.
 Running this version is strongly recommended, as we continuously fix bugs and add features.
 
 <p align="center">
   <img alt="The application in action" src="https://raw.githubusercontent.com/acconeer/acconeer-python-exploration/8f633e02abac99ffec6fefec4339d13bc5c18388/docs/_static/gui.png" width=85%>
 </p>
 
 ## Quickstart for Windows
```

### Comparing `acconeer-exptool-7.1.0/docker/Dockerfile` & `acconeer-exptool-7.2.0/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/dodo.py` & `acconeer-exptool-7.2.0/dodo.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a111/basic.py` & `acconeer-exptool-7.2.0/examples/a111/basic.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a111/basic_continuous.py` & `acconeer-exptool-7.2.0/examples/a111/basic_continuous.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a111/load_record.py` & `acconeer-exptool-7.2.0/examples/a111/load_record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a111/load_record_h5.m` & `acconeer-exptool-7.2.0/examples/a111/load_record_h5.m`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a111/plotting/plot_with_matplotlib.py` & `acconeer-exptool-7.2.0/examples/a111/plotting/plot_with_matplotlib.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a111/plotting/plot_with_pyqtgraph.py` & `acconeer-exptool-7.2.0/examples/a111/plotting/plot_with_pyqtgraph.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a111/record_data/barebones.py` & `acconeer-exptool-7.2.0/examples/a111/record_data/barebones.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a111/record_data/long_duration_split_files.py` & `acconeer-exptool-7.2.0/examples/a111/record_data/long_duration_split_files.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a111/record_data/with_cli.py` & `acconeer-exptool-7.2.0/examples/a111/record_data/with_cli.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a111/services/envelope.py` & `acconeer-exptool-7.2.0/examples/a111/services/envelope.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a111/services/iq.py` & `acconeer-exptool-7.2.0/examples/a111/services/iq.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a111/services/power_bins.py` & `acconeer-exptool-7.2.0/examples/a111/services/power_bins.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a111/services/sparse.py` & `acconeer-exptool-7.2.0/examples/a111/services/sparse.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a111/utils/ping.py` & `acconeer-exptool-7.2.0/examples/a111/utils/ping.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a111/utils/test_throughput.py` & `acconeer-exptool-7.2.0/examples/a111/utils/test_throughput.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a121/basic.py` & `acconeer-exptool-7.2.0/examples/a121/basic.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a121/bilateration/bilaterator.py` & `acconeer-exptool-7.2.0/examples/a121/bilateration/bilaterator.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a121/distance/detector.py` & `acconeer-exptool-7.2.0/examples/a121/distance/detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a121/distance/processor.py` & `acconeer-exptool-7.2.0/examples/a121/distance/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a121/extended_config.py` & `acconeer-exptool-7.2.0/examples/a121/extended_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a121/load_record.py` & `acconeer-exptool-7.2.0/examples/a121/load_record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a121/load_record_h5.m` & `acconeer-exptool-7.2.0/examples/a121/load_record_h5.m`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a121/phase_tracking/phase_tracking.py` & `acconeer-exptool-7.2.0/examples/a121/phase_tracking/phase_tracking.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a121/plot.py` & `acconeer-exptool-7.2.0/examples/a121/plot.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a121/presence/detector.py` & `acconeer-exptool-7.2.0/examples/a121/presence/detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a121/presence/processor.py` & `acconeer-exptool-7.2.0/examples/a121/presence/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a121/record_data/barebones.py` & `acconeer-exptool-7.2.0/examples/a121/record_data/barebones.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a121/record_data/with_cli.py` & `acconeer-exptool-7.2.0/examples/a121/record_data/with_cli.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a121/reuse_calibration.py` & `acconeer-exptool-7.2.0/examples/a121/reuse_calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a121/smart_presence/processor.py` & `acconeer-exptool-7.2.0/examples/a121/smart_presence/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a121/smart_presence/ref_app.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,262 +1,276 @@
-# Copyright (c) Acconeer AB, 2023
+# Copyright (c) Acconeer AB, 2022
 # All rights reserved
 
-from __future__ import annotations
-
 import numpy as np
-import numpy.typing as npt
 
 from PySide6 import QtCore
 
 import pyqtgraph as pg
 
 import acconeer.exptool as et
-from acconeer.exptool import a121
-from acconeer.exptool.a121.algo.smart_presence import RefApp, RefAppConfig
-
-
-def main():
-    args = a121.ExampleArgumentParser().parse_args()
-    et.utils.config_logging(args)
-
-    client = a121.Client.open(**a121.get_client_args(args))
-
-    ref_app_config = RefAppConfig(
-        start_m=1.0,
-        end_m=3.0,
-        num_zones=3,
-    )
-
-    ref_app = RefApp(client=client, sensor_id=1, ref_app_config=ref_app_config)
-    ref_app.start()
-
-    pg_updater = PGUpdater(
-        ref_app_config,
-        ref_app.detector._get_sensor_config(ref_app_config),
-        ref_app.detector.estimated_frame_rate,
-        ref_app.ref_app_processor.zone_limits,
-    )
-    pg_process = et.PGProcess(pg_updater)
-    pg_process.start()
-
-    interrupt_handler = et.utils.ExampleInterruptHandler()
-    print("Press Ctrl-C to end session")
-
-    while not interrupt_handler.got_signal:
-        ref_app_result = ref_app.get_next()
-        if ref_app_result.presence_detected:
-            print(f"Presence in zone {ref_app_result.max_presence_zone}")
-        else:
-            print("No presence")
-        try:
-            pg_process.put_data(ref_app_result)
-        except et.PGProccessDiedException:
-            break
-
-    ref_app.stop()
-
-    print("Disconnecting...")
-    client.close()
 
 
 class PGUpdater:
-    def __init__(
-        self,
-        ref_app_config: RefAppConfig,
-        sensor_config: a121.SensorConfig,
-        estimated_frame_rate: float,
-        zone_limits: npt.NDArray[np.float_],
-    ):
-        self.ref_app_config = ref_app_config
-
-        self.history_length_s = 5
-        self.estimated_frame_rate = estimated_frame_rate
-        self.history_length_n = int(round(self.history_length_s * estimated_frame_rate))
-        self.intra_history = np.zeros(self.history_length_n)
-        self.inter_history = np.zeros(self.history_length_n)
-
-        self.num_sectors = min(ref_app_config.num_zones, sensor_config.num_points)
-        self.sector_size = max(1, -(-sensor_config.num_points // self.num_sectors))
-
-        self.sector_offset = (self.num_sectors * self.sector_size - sensor_config.num_points) // 2
-        self.zone_limits = zone_limits
+    def __init__(self, sensor_config, processing_config, session_info):
+        self.sensor_config = sensor_config
+        self.processing_config = processing_config
+
+        self.history_length_s = processing_config.history_length_s
+        self.depths = et.a111.get_range_depths(sensor_config, session_info)
+
+        max_num_of_sectors = max(6, self.depths.size // 3)
+        self.sector_size = max(1, -(-self.depths.size // max_num_of_sectors))
+        self.num_sectors = -(-self.depths.size // self.sector_size)
+        self.sector_offset = (self.num_sectors * self.sector_size - self.depths.size) // 2
 
         self.setup_is_done = False
 
     def setup(self, win):
-        win.setWindowTitle("Acconeer smart presence example")
+        win.setWindowTitle("Acconeer presence detection example")
 
-        self.intra_limit_lines = []
-        self.inter_limit_lines = []
+        self.limit_lines = []
+        dashed_pen = pg.mkPen("k", width=2.5, style=QtCore.Qt.DashLine)
 
-        # Intra presence history plot
+        # Data plot
 
-        self.intra_hist_plot = win.addPlot(
+        self.data_plot = win.addPlot(
             row=0,
             col=0,
-            title="Intra presence history (fast motions)",
+            title="Frame (blue), fast (orange), and slow (green)",
         )
-        self.intra_hist_plot.setMenuEnabled(False)
-        self.intra_hist_plot.setMouseEnabled(x=False, y=False)
-        self.intra_hist_plot.hideButtons()
-        self.intra_hist_plot.showGrid(x=True, y=True)
-        self.intra_hist_plot.setLabel("bottom", "Time (s)")
-        self.intra_hist_plot.setLabel("left", "Score")
-        self.intra_hist_plot.setXRange(-self.history_length_s, 0)
-        self.intra_history_smooth_max = et.utils.SmoothMax(self.estimated_frame_rate)
-        self.intra_hist_plot.setYRange(0, 10)
-        if not self.ref_app_config.intra_enable:
-            intra_color = et.utils.color_cycler(1)
-            intra_color = f"{intra_color}50"
-            intra_dashed_pen = pg.mkPen(intra_color, width=2.5, style=QtCore.Qt.DashLine)
-            intra_pen = pg.mkPen(intra_color, width=2)
-        else:
-            intra_dashed_pen = et.utils.pg_pen_cycler(1, width=2.5, style="--")
-            intra_pen = et.utils.pg_pen_cycler(1)
+        self.data_plot.setMenuEnabled(False)
+        self.data_plot.setMouseEnabled(x=False, y=False)
+        self.data_plot.hideButtons()
+        self.data_plot.showGrid(x=True, y=True)
+        self.data_plot.setLabel("bottom", "Depth (m)")
+        self.data_plot.setLabel("left", "Amplitude")
+        self.data_plot.setYRange(0, 2**16)
+        self.frame_scatter = pg.ScatterPlotItem(
+            size=10,
+            brush=et.utils.pg_brush_cycler(0),
+        )
+        self.fast_scatter = pg.ScatterPlotItem(
+            size=10,
+            brush=et.utils.pg_brush_cycler(1),
+        )
+        self.slow_scatter = pg.ScatterPlotItem(
+            size=10,
+            brush=et.utils.pg_brush_cycler(2),
+        )
+        self.data_plot.addItem(self.frame_scatter)
+        self.data_plot.addItem(self.fast_scatter)
+        self.data_plot.addItem(self.slow_scatter)
+        self.frame_smooth_limits = et.utils.SmoothLimits(self.sensor_config.update_rate)
 
-        self.intra_hist_curve = self.intra_hist_plot.plot(pen=intra_pen)
-        limit_line = pg.InfiniteLine(angle=0, pen=intra_dashed_pen)
-        self.intra_hist_plot.addItem(limit_line)
-        self.intra_limit_lines.append(limit_line)
+        # Noise estimation plot
 
-        for line in self.intra_limit_lines:
-            line.setPos(self.ref_app_config.intra_detection_threshold)
+        self.noise_plot = win.addPlot(
+            row=1,
+            col=0,
+            title="Noise",
+        )
+        self.noise_plot.setMenuEnabled(False)
+        self.noise_plot.setMouseEnabled(x=False, y=False)
+        self.noise_plot.hideButtons()
+        self.noise_plot.showGrid(x=True, y=True)
+        self.noise_plot.setLabel("bottom", "Depth (m)")
+        self.noise_plot.setLabel("left", "Amplitude")
+        self.noise_curve = self.noise_plot.plot(pen=et.utils.pg_pen_cycler())
+        self.noise_smooth_max = et.utils.SmoothMax(self.sensor_config.update_rate)
 
-        # Inter presence history plot
+        # Depthwise presence plot
 
-        self.inter_hist_plot = win.addPlot(
-            row=0,
-            col=1,
-            title="Inter presence history (slow motions)",
+        self.move_plot = win.addPlot(
+            row=2,
+            col=0,
+            title="Depthwise presence",
         )
-        self.inter_hist_plot.setMenuEnabled(False)
-        self.inter_hist_plot.setMouseEnabled(x=False, y=False)
-        self.inter_hist_plot.hideButtons()
-        self.inter_hist_plot.showGrid(x=True, y=True)
-        self.inter_hist_plot.setLabel("bottom", "Time (s)")
-        self.inter_hist_plot.setLabel("left", "Score")
-        self.inter_hist_plot.setXRange(-self.history_length_s, 0)
-        self.inter_history_smooth_max = et.utils.SmoothMax(self.estimated_frame_rate)
-        self.inter_hist_plot.setYRange(0, 10)
-        if not self.ref_app_config.inter_enable:
-            inter_color = et.utils.color_cycler(0)
-            inter_color = f"{inter_color}50"
-            inter_dashed_pen = pg.mkPen(inter_color, width=2.5, style=QtCore.Qt.DashLine)
-            inter_pen = pg.mkPen(inter_color, width=2)
-        else:
-            inter_pen = et.utils.pg_pen_cycler(0)
-            inter_dashed_pen = et.utils.pg_pen_cycler(0, width=2.5, style="--")
+        self.move_plot.setMenuEnabled(False)
+        self.move_plot.setMouseEnabled(x=False, y=False)
+        self.move_plot.hideButtons()
+        self.move_plot.showGrid(x=True, y=True)
+        self.move_plot.setLabel("bottom", "Depth (m)")
+        self.move_plot.setLabel("left", "Norm. ampl.")
+        zero_curve = self.move_plot.plot(self.depths, np.zeros_like(self.depths))
+        self.inter_curve = self.move_plot.plot()
+        self.total_curve = self.move_plot.plot()
+        self.move_smooth_max = et.utils.SmoothMax(
+            self.sensor_config.update_rate,
+            tau_decay=1.0,
+            tau_grow=0.25,
+        )
+
+        self.move_depth_line = pg.InfiniteLine(pen=pg.mkPen("k", width=1.5))
+        self.move_depth_line.hide()
+        self.move_plot.addItem(self.move_depth_line)
+        limit_line = pg.InfiniteLine(angle=0, pen=dashed_pen)
+        self.move_plot.addItem(limit_line)
+        self.limit_lines.append(limit_line)
+
+        fbi = pg.FillBetweenItem(
+            zero_curve,
+            self.inter_curve,
+            brush=et.utils.pg_brush_cycler(0),
+        )
+        self.move_plot.addItem(fbi)
 
-        self.inter_hist_curve = self.inter_hist_plot.plot(pen=inter_pen)
-        limit_line = pg.InfiniteLine(angle=0, pen=inter_dashed_pen)
-        self.inter_hist_plot.addItem(limit_line)
-        self.inter_limit_lines.append(limit_line)
+        fbi = pg.FillBetweenItem(
+            self.inter_curve,
+            self.total_curve,
+            brush=et.utils.pg_brush_cycler(1),
+        )
+        self.move_plot.addItem(fbi)
 
-        for line in self.inter_limit_lines:
-            line.setPos(self.ref_app_config.inter_detection_threshold)
+        # Presence history plot
 
-        # Sector plot
+        self.move_hist_plot = pg.PlotItem(title="Presence history")
+        self.move_hist_plot.setMenuEnabled(False)
+        self.move_hist_plot.setMouseEnabled(x=False, y=False)
+        self.move_hist_plot.hideButtons()
+        self.move_hist_plot.showGrid(x=True, y=True)
+        self.move_hist_plot.setLabel("bottom", "Time (s)")
+        self.move_hist_plot.setLabel("left", "Score")
+        self.move_hist_plot.setXRange(-self.history_length_s, 0)
+        self.history_smooth_max = et.utils.SmoothMax(self.sensor_config.update_rate)
+        self.move_hist_plot.setYRange(0, 10)
+
+        self.move_hist_curve = self.move_hist_plot.plot(pen=et.utils.pg_pen_cycler())
+        limit_line = pg.InfiniteLine(angle=0, pen=dashed_pen)
+        self.move_hist_plot.addItem(limit_line)
+        self.limit_lines.append(limit_line)
 
-        self.sector_plot = pg.PlotItem(
-            title="Detection zone<br>Detection type: fast (orange), slow (blue), both (green)"
+        self.present_html_format = (
+            '<div style="text-align: center">'
+            '<span style="color: #FFFFFF;font-size:15pt;">'
+            "{}</span></div>"
         )
+        not_present_html = (
+            '<div style="text-align: center">'
+            '<span style="color: #FFFFFF;font-size:15pt;">'
+            "{}</span></div>".format("No presence detected")
+        )
+        self.present_text_item = pg.TextItem(
+            fill=pg.mkColor(0xFF, 0x7F, 0x0E, 200),
+            anchor=(0.5, 0),
+        )
+        self.not_present_text_item = pg.TextItem(
+            html=not_present_html,
+            fill=pg.mkColor(0x1F, 0x77, 0xB4, 180),
+            anchor=(0.5, 0),
+        )
+
+        self.move_hist_plot.addItem(self.present_text_item)
+        self.move_hist_plot.addItem(self.not_present_text_item)
+        self.present_text_item.hide()
+        self.not_present_text_item.hide()
+
+        # Sector plot
+
+        self.sector_plot = pg.PlotItem()
         self.sector_plot.setAspectLocked()
         self.sector_plot.hideAxis("left")
         self.sector_plot.hideAxis("bottom")
         self.sectors = []
-        self.limit_text = []
-
-        self.range_html = (
-            '<div style="text-align: center">'
-            '<span style="color: #000000;font-size:12pt;">'
-            "{}</span></div>"
-        )
 
         pen = pg.mkPen("k", width=1)
         span_deg = 25
         for r in np.flip(np.arange(self.num_sectors) + 1):
             sector = pg.QtWidgets.QGraphicsEllipseItem(-r, -r, r * 2, r * 2)
             sector.setStartAngle(-16 * span_deg)
             sector.setSpanAngle(16 * span_deg * 2)
             sector.setPen(pen)
             self.sector_plot.addItem(sector)
             self.sectors.append(sector)
 
-            limit = pg.TextItem(html=self.range_html, anchor=(0.5, 0.5), angle=25)
-            x = r * np.cos(np.radians(span_deg))
-            y = r * np.sin(np.radians(span_deg))
-            limit.setPos(x, y + 0.25)
-            self.sector_plot.addItem(limit)
-            self.limit_text.append(limit)
-
         self.sectors.reverse()
 
-        start_limit_text = pg.TextItem(html=self.range_html, anchor=(0.5, 0.5), angle=25)
-        range_html = self.range_html.format(f"{self.ref_app_config.start_m}")
-        start_limit_text.setHtml(range_html)
-        start_limit_text.setPos(0, 0.25)
-        self.sector_plot.addItem(start_limit_text)
-
-        unit_text = pg.TextItem(html=self.range_html, anchor=(0.5, 0.5))
-        unit_html = self.range_html.format("[m]")
-        unit_text.setHtml(unit_html)
-        unit_text.setPos(
-            self.num_sectors + 0.5, (self.num_sectors + 1) * np.sin(np.radians(span_deg))
-        )
-        self.sector_plot.addItem(unit_text)
-
-        for (text_item, limit) in zip(self.limit_text, np.flip(self.zone_limits)):
-            range_html = self.range_html.format(np.around(limit, 1))
-            text_item.setHtml(range_html)
-
-        sublayout = win.addLayout(row=1, col=0, colspan=2)
+        sublayout = win.addLayout(row=3, col=0)
         sublayout.layout.setColumnStretchFactor(0, 2)
-        sublayout.addItem(self.sector_plot, row=0, col=0)
+        sublayout.addItem(self.move_hist_plot, col=0)
+        sublayout.addItem(self.sector_plot, col=1)
 
         self.setup_is_done = True
+        self.update_processing_config()
 
-    def update(self, data):
-        # Intra presence
-
-        move_hist_xs = np.linspace(-self.history_length_s, 0, self.history_length_n)
-
-        self.intra_history = np.roll(self.intra_history, -1)
-        self.intra_history[-1] = data.intra_presence_score
-
-        m_hist = max(
-            float(np.max(self.intra_history)), self.ref_app_config.intra_detection_threshold * 1.05
-        )
-        m_hist = self.intra_history_smooth_max.update(m_hist)
+    def update_processing_config(self, processing_config=None):
+        if processing_config is None:
+            processing_config = self.processing_config
+        else:
+            self.processing_config = processing_config
 
-        self.intra_hist_plot.setYRange(0, m_hist)
-        self.intra_hist_curve.setData(move_hist_xs, self.intra_history)
+        if not self.setup_is_done:
+            return
 
-        # Inter presence
+        self.data_plot.setVisible(self.processing_config.show_data)
+        self.noise_plot.setVisible(self.processing_config.show_noise)
+        self.move_plot.setVisible(self.processing_config.show_depthwise_output)
+        self.sector_plot.setVisible(self.processing_config.show_sectors)
 
-        self.inter_history = np.roll(self.inter_history, -1)
-        self.inter_history[-1] = data.inter_presence_score
+        for line in self.limit_lines:
+            line.setPos(processing_config.detection_threshold)
 
-        m_hist = max(
-            float(np.max(self.inter_history)), self.ref_app_config.inter_detection_threshold * 1.05
+    def update(self, data):
+        self.frame_scatter.setData(
+            np.tile(self.depths, self.sensor_config.sweeps_per_frame),
+            data["frame"].flatten(),
         )
-        m_hist = self.inter_history_smooth_max.update(m_hist)
 
-        self.inter_hist_plot.setYRange(0, m_hist)
-        self.inter_hist_curve.setData(move_hist_xs, self.inter_history)
+        self.fast_scatter.setData(self.depths, data["fast"])
+        self.slow_scatter.setData(self.depths, data["slow"])
+        self.data_plot.setYRange(*self.frame_smooth_limits.update(data["frame"]))
+
+        noise = data["noise"]
+        self.noise_curve.setData(self.depths, noise)
+        self.noise_plot.setYRange(0, self.noise_smooth_max.update(noise))
+
+        movement_x = data["presence_distance"]
+
+        move_ys = data["depthwise_presence"]
+        self.inter_curve.setData(self.depths, data["inter"])
+        self.total_curve.setData(self.depths, move_ys)
+        m = self.move_smooth_max.update(np.max(move_ys))
+        m = max(m, 2 * self.processing_config.detection_threshold)
+        self.move_plot.setYRange(0, m)
+        self.move_depth_line.setPos(movement_x)
+        self.move_depth_line.setVisible(bool(data["presence_detected"]))
+
+        move_hist_ys = data["presence_history"]
+        move_hist_xs = np.linspace(-self.history_length_s, 0, len(move_hist_ys))
+
+        m_hist = max(np.max(move_hist_ys), self.processing_config.detection_threshold * 1.05)
+        m_hist = self.history_smooth_max.update(m_hist)
+
+        if self.processing_config.history_plot_ceiling is not None:
+            self.move_hist_plot.setYRange(0, self.processing_config.history_plot_ceiling)
+            self.move_hist_curve.setData(
+                move_hist_xs,
+                np.minimum(move_hist_ys, self.processing_config.history_plot_ceiling),
+            )
+            self.set_present_text_y_pos(self.processing_config.history_plot_ceiling)
+        else:
+            self.move_hist_plot.setYRange(0, m_hist)
+            self.move_hist_curve.setData(move_hist_xs, move_hist_ys)
+            self.set_present_text_y_pos(m_hist)
+
+        if data["presence_detected"]:
+            present_text = "Presence detected at {:.0f} cm".format(movement_x * 100)
+            present_html = self.present_html_format.format(present_text)
+            self.present_text_item.setHtml(present_html)
 
-        # Sector
+            self.present_text_item.show()
+            self.not_present_text_item.hide()
+        else:
+            self.present_text_item.hide()
+            self.not_present_text_item.show()
 
-        brush = et.utils.pg_brush_cycler(7)
+        brush = et.utils.pg_brush_cycler(0)
         for sector in self.sectors:
             sector.setBrush(brush)
 
-        if data.presence_detected:
-            assert data.max_presence_zone is not None
-            if data.max_presence_zone == data.max_intra_zone:
-                self.sectors[data.max_presence_zone].setBrush(et.utils.pg_brush_cycler(1))
-            else:
-                self.sectors[data.max_presence_zone].setBrush(et.utils.pg_brush_cycler(0))
-
-
-if __name__ == "__main__":
-    main()
+        if data["presence_detected"]:
+            index = (data["presence_distance_index"] + self.sector_offset) // self.sector_size
+            self.sectors[index].setBrush(et.utils.pg_brush_cycler(1))
+
+    def set_present_text_y_pos(self, y):
+        self.present_text_item.setPos(-self.history_length_s / 2, 0.95 * y)
+        self.not_present_text_item.setPos(-self.history_length_s / 2, 0.95 * y)
```

### Comparing `acconeer-exptool-7.1.0/examples/a121/stress.py` & `acconeer-exptool-7.2.0/examples/a121/stress.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a121/subsweeps.py` & `acconeer-exptool-7.2.0/examples/a121/subsweeps.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a121/surface_velocity/example_app.py` & `acconeer-exptool-7.2.0/examples/a121/surface_velocity/example_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a121/surface_velocity/processor.py` & `acconeer-exptool-7.2.0/examples/a121/surface_velocity/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a121/touchless_button/processor.py` & `acconeer-exptool-7.2.0/examples/a121/touchless_button/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/examples/a121/vibration/vibration.py` & `acconeer-exptool-7.2.0/examples/a121/vibration/vibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/gui/main.py` & `acconeer-exptool-7.2.0/gui/main.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/noxfile.py` & `acconeer-exptool-7.2.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/portable/make.py` & `acconeer-exptool-7.2.0/portable/make.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/portable/package/tools/update.py` & `acconeer-exptool-7.2.0/portable/package/tools/update.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/pyproject.toml` & `acconeer-exptool-7.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/setup.cfg` & `acconeer-exptool-7.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/_bs_thread.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/_bs_thread.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/_pyusb/pyusbcomm.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/_pyusb/pyusbcomm.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/_structs/configbase.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/_structs/configbase.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/_structs/qtpidgets.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/_structs/qtpidgets.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/_tests/test_rig.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/_tests/test_rig.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/LICENSE` & `acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/LICENSE`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/__main__.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/usb_cdc.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/usb_cdc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/winusb.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/winusb.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/winusbclasses.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/winusbclasses.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/winusbpy.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/winusbpy.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/winusbutils.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/winusbutils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/base.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/client.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/client_factory.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/client_factory.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/common.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/common.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/json/client.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/json/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/links.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/links.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/mock/client.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/mock/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/multiwrap.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/multiwrap.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/client.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/protocol.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/protocol.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/regmap.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/regmap.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_conf_to_rss_sdk.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_conf_to_rss_sdk.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_configs.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_modes.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_modes.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_utils.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/_base/calibration.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/_base/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/_base/module_info.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/_base/module_info.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/_standalone_main.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/_standalone_main.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/breathing/_meta.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/breathing/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/breathing/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/breathing/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/breathing/ui.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/breathing/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press/_meta.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press/ui.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/distance_detector/_meta.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/distance_detector/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/distance_detector/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/distance_detector/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/distance_detector/calibration.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/distance_detector/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/distance_detector/ui.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/distance_detector/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/envelope/_meta.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/envelope/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/envelope/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/envelope/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/envelope/calibration.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/envelope/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/envelope/ui.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/envelope/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/iq/_meta.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/iq/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/iq/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/iq/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/iq/ui.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/iq/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/parking/_meta.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/parking/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/parking/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/parking/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/parking/ui.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/parking/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/phase_tracking/ui.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/phase_tracking/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/power_bins/_meta.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/power_bins/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/power_bins/ui.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/power_bins/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse/_meta.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse/ui.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_fft/ui.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_fft/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/speed_sparse/ui.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/speed_sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/tank_level_short/ui.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/tank_level_short/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/utils.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/recording.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/recording.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/__init__.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
-SDK_VERSION = "1.0.0"
+SDK_VERSION = "1.1.0"
 
 from ._cli import ExampleArgumentParser, get_client_args
 from ._core import (
     _H5PY_STR_DTYPE,
     PRF,
     Client,
     ClientError,
```

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_cli.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_cli.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/__init__.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/__init__.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/session_config.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/session_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,14 +173,23 @@
                         "step_length",
                         f"Measuring range is too long for PRF (max {self.prf.mmd:.2f}m), "
                         + "try decreasing the step length.",
                     ),
                 ]
             )
 
+        if self.start_point < -275:
+            validation_results.append(
+                ValidationError(
+                    self,
+                    "start_point",
+                    "Start point must be larger than or equal to -275",
+                )
+            )
+
         return validation_results
 
     def validate(self) -> None:
         """Performs self-validation
 
         :raises ValidationError: If anything is invalid.
         """
```

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/__init__.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/client_info.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/client_info.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/metadata.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/metadata.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/record.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/result.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/result.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/server_info.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/server_info.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/utils.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/mediators/link.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/mediators/link.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/mediators/recorder.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/mediators/recorder.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/client.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,22 @@
 class ClientCreationError(Exception):
     pass
 
 
 class ClientABCWithGoodError(abc.ABC):
     def __new__(cls, *args: Any, **kwargs: Any) -> ClientABCWithGoodError:
         try:
-            return super().__new__(cls)  # , *args, **kwargs)
-        except TypeError as te:  # te here is the "Can't instantiate ..."-error
-            raise ClientCreationError("Client cannot be instantiated, use Client.open()") from te
+            return super().__new__(cls)
+        except TypeError:  # te here is the "Can't instantiate ..."-error
+            if cls == Client:
+                raise ClientCreationError(
+                    "Client cannot be instantiated, use Client.open()"
+                ) from None
+            else:
+                raise
 
 
 class Client(ClientABCWithGoodError):
 
     __registry: List[Type[Client]] = []
 
     @classmethod
@@ -53,32 +58,27 @@
     ) -> Client:
         """
         Open a new client
         """
         if len([e for e in [ip_address, serial_port, usb_device, mock] if e is not None]) > 1:
             raise ValueError("Only one connection can be selected")
 
-        client = None
         for subclass in cls.__registry:
             try:
-                client = subclass.open(
+                return subclass.open(
                     ip_address,
                     tcp_port,
                     serial_port,
                     usb_device,
                     mock,
                     override_baudrate,
                     _override_protocol,
                 )
             except ClientCreationError:
-                pass
-
-        if client is not None:
-            client._open()
-            return client
+                continue
 
         # This should not happen since the current implementation
         # only has two clients which are mutual exclusive.
         # * The mock client (mock is not None)
         # * The exploration client (mock is None)
         raise ClientCreationError("No client could be created")
 
@@ -87,19 +87,14 @@
         """Registers a subclass"""
         if not issubclass(subclass, cls):
             raise TypeError(f"{subclass.__name__!r} needs to be a subclass of {cls.__name__}.")
         cls.__registry.append(subclass)
         return subclass
 
     @abc.abstractmethod
-    def _open(self) -> None:
-        """Connects to client, called from open"""
-        ...
-
-    @abc.abstractmethod
     def setup_session(
         self,
         config: Union[SensorConfig, SessionConfig],
         calibrations: Optional[dict[int, SensorCalibration]] = None,
     ) -> Union[Metadata, list[dict[int, Metadata]]]:
         """Sets up the session specified by ``config``.
```

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
+import contextlib
 import json
 import logging
 import time
 from typing import Any, Iterator, Optional, Tuple, Type, Union
 
 import attrs
 from serial.serialutil import SerialException
 
 from acconeer.exptool.a121._core.entities import (
     ClientInfo,
     Metadata,
     Result,
     SensorCalibration,
     SensorConfig,
-    SensorInfo,
     ServerInfo,
     ServerLogMessage,
     SessionConfig,
 )
 from acconeer.exptool.a121._core.utils import (
     create_extended_structure,
     iterate_extended_structure,
@@ -35,15 +35,14 @@
 from .communication_protocol import CommunicationProtocol
 from .exploration_protocol import (
     ExplorationProtocol,
     ServerError,
     get_exploration_protocol,
     messages,
 )
-from .exploration_protocol.messages.system_info_response import SystemInfoDict
 from .links import AdaptedSerialLink, BufferedLink, NullLinkError
 from .message import Message, MessageT
 from .utils import autodetermine_client_link, get_calibrations_provided, link_factory
 
 
 log = logging.getLogger(__name__)
 
@@ -52,16 +51,15 @@
 class ExplorationClient(CommonClient):
     _link: BufferedLink
     _default_link_timeout: float
     _link_timeout: float
     _protocol: Type[CommunicationProtocol]
     _protocol_overridden: bool
     _tick_unwrapper: TickUnwrapper
-    _sensor_infos: dict[int, SensorInfo]
-    _system_info: Optional[SystemInfoDict]
+    _server_info: Optional[ServerInfo]
     _result_queue: list[list[dict[int, Result]]]
     _message_stream: Iterator[Message]
     _log_queue: list[ServerLogMessage]
 
     @classmethod
     def open(
         cls,
@@ -69,14 +67,16 @@
         tcp_port: Optional[int] = None,
         serial_port: Optional[str] = None,
         usb_device: Optional[Union[str, bool]] = None,
         mock: Optional[bool] = None,
         override_baudrate: Optional[int] = None,
         _override_protocol: Optional[Type[CommunicationProtocol]] = None,
     ) -> Client:
+        if mock is not None:
+            raise ClientCreationError
 
         client_info = ClientInfo._from_open(
             ip_address=ip_address,
             tcp_port=tcp_port,
             override_baudrate=override_baudrate,
             serial_port=serial_port,
             usb_device=usb_device,
@@ -85,155 +85,130 @@
         return cls(client_info=client_info, _override_protocol=_override_protocol)
 
     def __init__(
         self,
         client_info: ClientInfo = ClientInfo(mock=None),
         _override_protocol: Optional[Type[CommunicationProtocol]] = None,
     ) -> None:
-        if client_info.mock is not None:
-            raise ClientCreationError()
-
         super().__init__(client_info)
         self._tick_unwrapper = TickUnwrapper()
         self._message_stream = iter([])
-        self._sensor_infos = {}
-        self._system_info = None
+        self._server_info = None
         self._log_queue = []
+        self._closed = False
+        self._crashing = False
 
         self._protocol: Type[CommunicationProtocol] = ExplorationProtocol
         self._protocol_overridden = False
 
         if _override_protocol is not None:
             self._protocol = _override_protocol
             self._protocol_overridden = True
 
         self._link = link_factory(self.client_info)
+        try:
+            self._connect_link()
+        except NullLinkError:
+            self._client_info = autodetermine_client_link(self.client_info)
+            self._link = link_factory(self.client_info)
+            self._connect_link()
 
-    def _assert_connected(self) -> None:
-        if not self.connected:
-            raise ClientError("Client is not connected.")
-
-    def _assert_session_setup(self) -> None:
-        self._assert_connected()
-        if not self.session_is_setup:
-            raise ClientError("Session is not set up.")
-
-    def _assert_session_started(self) -> None:
-        self._assert_session_setup()
-        if not self.session_is_started:
-            raise ClientError("Session is not started.")
-
-    def _get_message_stream(self) -> Iterator[Message]:
-        """returns an iterator of parsed messages"""
-        while True:
-            header: dict[str, Any] = json.loads(self._link.recv_until(self._protocol.end_sequence))
-            try:
-                payload_size = header["payload_size"]
-            except KeyError:
-                payload = bytes()
-            else:
-                payload = self._link.recv(payload_size)
-
-            resp = self._protocol.parse_message(header, payload)
-            yield resp
-
-    def _assert_deadline_not_reached(self, deadline: Optional[float]) -> None:
-        if deadline is not None and time.monotonic() > deadline:
-            raise ClientError("Client timed out.")
-
-    def _apply_messages_until_message_type_encountered(
-        self, message_type: Type[MessageT], timeout_s: Optional[float] = None
-    ) -> MessageT:
-        """Retrieves and applies messages until a message of type ``message_type`` is encountered.
-
-        :param message_type: a subclass of ``Message``
-        :param timeout_s: Limit the time spent in this function
-        :raises ClientError:
-            if timeout_s is set and that amount of time has elapsed
-            without predicate evaluating to True
-        """
-        deadline = None if (timeout_s is None) else time.monotonic() + timeout_s
-
-        if message_type in [messages.ErroneousMessage, messages.EmptyResultMessage]:
-            raise ClientError("Cannot wait for error messages")
-
-        for message in self._message_stream:
-            if type(message) == messages.LogMessage:
-                self._log_queue.append(message.message)
-            elif type(message) == messages.EmptyResultMessage:
-                raise RuntimeError("Received an empty Result from Server.")
-            elif type(message) == messages.ErroneousMessage:
-                last_error = ""
-                for log in self._log_queue:
-                    if log.level == "ERROR" and "exploration_server" not in log.module:
-                        last_error = f" ({log.log})"
-                raise ServerError(f"{message}{last_error}")
-
-            if type(message) == message_type:
-                return message
-
-            self._assert_deadline_not_reached(deadline)
-        raise ClientError("No message received")
+        self._connect_client()
 
     def _connect_link(self) -> None:
         self._default_link_timeout = self._link.timeout
         self._link_timeout = self._default_link_timeout
 
         try:
             self._link.connect()
         except SerialException as exc:
             if "Permission denied" in str(exc):
                 text = "\n".join(
                     [
-                        str(exc),
-                        "",
                         "You are probably missing permissions to access the serial port.",
                         "",
                         "Run the setup script to fix it:",
                         "$ python -m acconeer.exptool.setup",
                         "",
                         "Reboot for the changes to take effect.",
                     ]
                 )
                 raise ClientError(text) from exc
             else:
                 raise
 
+    def _connect_client(self) -> None:
         self._message_stream = self._get_message_stream()
+        self._server_info = self._retrieve_server_info()
 
-        self._link.send(self._protocol.get_system_info_command())
-        system_info_response = self._apply_messages_until_message_type_encountered(
-            messages.SystemInfoResponse
-        )
-        self._system_info = system_info_response.system_info
-
-        self._link.send(self._protocol.get_sensor_info_command())
-        sensor_info_response = self._apply_messages_until_message_type_encountered(
-            messages.SensorInfoResponse
-        )
-        self._sensor_infos = sensor_info_response.sensor_infos
-
-        sensor = self._system_info.get("sensor") if self._system_info else None
-        if sensor != "a121":
+        if self._server_info.connected_sensors == []:
             self._link.disconnect()
-            raise ClientError(f"Wrong sensor version, expected a121 but got {sensor}")
+            raise ClientError("Exploration server is running but no sensors are detected.")
 
         if not self._protocol_overridden:
             self._update_protocol_based_on_servers_rss_version()
 
         self._update_baudrate()
 
-    def _update_protocol_based_on_servers_rss_version(self) -> None:
+    def _get_message_stream(self) -> Iterator[Message]:
+        """returns an iterator of parsed messages"""
+        while True:
+            with self._close_before_reraise():
+                header: dict[str, Any] = json.loads(
+                    self._link.recv_until(self._protocol.end_sequence)
+                )
+
+            try:
+                payload_size = header["payload_size"]
+            except KeyError:
+                payload = bytes()
+            else:
+                with self._close_before_reraise():
+                    payload = self._link.recv(payload_size)
+
+            resp = self._protocol.parse_message(header, payload)
+            yield resp
+
+    @contextlib.contextmanager
+    def _close_before_reraise(self) -> Iterator[None]:
         try:
-            new_protocol = get_exploration_protocol(self.server_info.parsed_rss_version)
+            yield
         except Exception:
+            self._crashing = True
             self.close()
             raise
-        else:
-            self._protocol = new_protocol
+
+    def _retrieve_server_info(self) -> ServerInfo:
+        system_info_response = self._send_command_and_wait_for_response(
+            self._protocol.get_system_info_command(),
+            messages.SystemInfoResponse,
+        )
+
+        sensor = system_info_response.system_info.get("sensor")
+        if sensor != "a121":
+            self.close()
+            raise ClientError(f"Wrong sensor version, expected a121 but got {sensor}")
+
+        sensor_info_response = self._send_command_and_wait_for_response(
+            self._protocol.get_sensor_info_command(),
+            messages.SensorInfoResponse,
+        )
+
+        return ServerInfo(
+            rss_version=system_info_response.system_info["rss_version"],
+            sensor_count=system_info_response.system_info["sensor_count"],
+            ticks_per_second=system_info_response.system_info["ticks_per_second"],
+            hardware_name=system_info_response.system_info.get("hw", None),
+            sensor_infos=sensor_info_response.sensor_infos,
+            max_baudrate=system_info_response.system_info.get("max_baudrate"),
+        )
+
+    def _update_protocol_based_on_servers_rss_version(self) -> None:
+        with self._close_before_reraise():
+            self._protocol = get_exploration_protocol(self.server_info.parsed_rss_version)
 
     def _update_baudrate(self) -> None:
         # Only Change baudrate for AdaptedSerialLink
         if not isinstance(self._link, AdaptedSerialLink):
             return
 
         if self.client_info.serial is None:
@@ -253,29 +228,19 @@
                 raise ClientError(f"Cannot set a baudrate lower than {DEFAULT_BAUDRATE}")
             baudrate_to_use = overridden_baudrate
 
         # Do not change baudrate if DEFAULT_BAUDRATE
         if baudrate_to_use == DEFAULT_BAUDRATE:
             return
 
-        self._link.send(self._protocol.set_baudrate_command(baudrate_to_use))
-
-        self._apply_messages_until_message_type_encountered(messages.SetBaudrateResponse)
-        self._baudrate_ack_received = False
-
+        _ = self._send_command_and_wait_for_response(
+            self._protocol.set_baudrate_command(baudrate_to_use), messages.SetBaudrateResponse
+        )
         self._link.baudrate = baudrate_to_use
 
-    def _open(self) -> None:
-        try:
-            self._connect_link()
-        except NullLinkError:
-            self._client_info = autodetermine_client_link(self.client_info)
-            self._link = link_factory(self.client_info)
-            self._connect_link()
-
     def setup_session(
         self,
         config: Union[SensorConfig, SessionConfig],
         calibrations: Optional[dict[int, SensorCalibration]] = None,
     ) -> Union[Metadata, list[dict[int, Metadata]]]:
         if self.session_is_started:
             raise ClientError("Session is currently running, can't setup.")
@@ -283,19 +248,19 @@
         if isinstance(config, SensorConfig):
             config = SessionConfig(config)
 
         config.validate()
 
         self._calibrations_provided = get_calibrations_provided(config, calibrations)
 
-        self._link.send(self._protocol.setup_command(config, calibrations))
-
+        message = self._send_command_and_wait_for_response(
+            self._protocol.setup_command(config, calibrations),
+            messages.SetupResponse,
+        )
         self._session_config = config
-
-        message = self._apply_messages_until_message_type_encountered(messages.SetupResponse)
         self._metadata = [
             {
                 sensor_id: metadata
                 for metadata, sensor_id in zip(metadata_group, config_group.keys())
             }
             for metadata_group, config_group in zip(
                 message.grouped_metadatas, self._session_config.groups
@@ -316,105 +281,144 @@
         self._link.timeout = self._link_timeout
 
         if self.session_config.extended:
             return self._metadata
         else:
             return unextend(self._metadata)
 
+    def _send_command_and_wait_for_response(
+        self, command: bytes, response_type: Type[MessageT], timeout_s: Optional[float] = None
+    ) -> MessageT:
+        with self._close_before_reraise():
+            self._link.send(command)
+
+        return self._wait_for_response(response_type, timeout_s)
+
+    def _wait_for_response(
+        self, message_type: Type[MessageT], timeout_s: Optional[float] = None
+    ) -> MessageT:
+        """Retrieves and applies messages until a message of type ``message_type`` is encountered.
+
+        :param message_type: a subclass of ``Message``
+        :param timeout_s: Limit the time spent in this function
+        :raises ClientError:
+            if timeout_s is set and that amount of time has elapsed
+            without predicate evaluating to True
+        """
+        deadline = None if (timeout_s is None) else time.monotonic() + timeout_s
+
+        if message_type in [messages.ErroneousMessage, messages.EmptyResultMessage]:
+            raise ClientError("Cannot wait for error messages")
+
+        for message in self._message_stream:
+            if type(message) == messages.LogMessage:
+                self._log_queue.append(message.message)
+            elif type(message) == messages.EmptyResultMessage:
+                raise RuntimeError("Received an empty Result from Server.")
+            elif type(message) == messages.ErroneousMessage:
+                last_error = ""
+                for log in self._log_queue:
+                    if log.level == "ERROR" and "exploration_server" not in log.module:
+                        last_error = f" ({log.log})"
+                raise ServerError(f"{message}{last_error}")
+
+            if type(message) == message_type:
+                return message
+
+            if deadline is not None and time.monotonic() > deadline:
+                raise ClientError("Client timed out.")
+
+        raise ClientError("No message received")
+
     def start_session(self) -> None:
         self._assert_session_setup()
 
         if self.session_is_started:
             raise ClientError("Session is already started.")
 
         self._recorder_start_session()
         self._session_is_started = True
 
         self._link.timeout = self._link_timeout
-        self._link.send(self._protocol.start_streaming_command())
-        self._apply_messages_until_message_type_encountered(messages.StartStreamingResponse)
+        _ = self._send_command_and_wait_for_response(
+            self._protocol.start_streaming_command(),
+            messages.StartStreamingResponse,
+        )
 
     def get_next(self) -> Union[Result, list[dict[int, Result]]]:
         self._assert_session_started()
 
-        result_message = self._apply_messages_until_message_type_encountered(
-            messages.ResultMessage
-        )
+        result_message = self._wait_for_response(messages.ResultMessage)
 
         if self._metadata is None:
             raise RuntimeError(f"{self} has no metadata")
 
-        if self._system_info is None:
+        if self._server_info is None:
             raise RuntimeError(f"{self} has no system info")
 
         if self._session_config is None:
             raise RuntimeError(f"{self} has no session config")
 
         extended_results = result_message.get_extended_results(
-            tps=self._system_info["ticks_per_second"],
+            tps=self._server_info.ticks_per_second,
             metadata=self._metadata,
             config_groups=self._session_config.groups,
         )
 
         extended_results = self._tick_unwrapper.unwrap_ticks(extended_results)
 
         self._recorder_sample(extended_results)
         return self._return_results(extended_results)
 
     def stop_session(self) -> None:
         self._assert_session_started()
 
-        self._link.send(self._protocol.stop_streaming_command())
-
-        try:
-            self._apply_messages_until_message_type_encountered(
-                messages.StopStreamingResponse, timeout_s=self._link.timeout + 1
-            )
-            self._session_is_started = False
-        except Exception:
-            raise
-        finally:
-            self._link.timeout = self._default_link_timeout
+        _ = self._send_command_and_wait_for_response(
+            self._protocol.stop_streaming_command(),
+            messages.StopStreamingResponse,
+            timeout_s=self._link.timeout + 1,
+        )
 
+        self._link.timeout = self._default_link_timeout
+        self._session_is_started = False
         self._recorder_stop_session()
-
         self._log_queue.clear()
 
     def close(self) -> None:
-        # TODO: Make sure this cleans up corner-cases (like lost connection)
-        #       to not hog resources.
-
-        if self.session_is_started:
-            self.stop_session()
+        if self._closed:
+            return
 
-        self._tick_unwrapper = TickUnwrapper()
-        self._system_info = None
-        self._sensor_infos = {}
-        self._message_stream = iter([])
-        self._metadata = None
-        self._log_queue.clear()
-        self._link.disconnect()
+        try:
+            if self.session_is_started:
+                if self._crashing:
+                    self._session_is_started = False
+                    self._recorder_stop_session()
+                else:
+                    self.stop_session()
+        except Exception:
+            raise
+        finally:
+            self._tick_unwrapper = TickUnwrapper()
+            self._server_info = None
+            self._message_stream = iter([])
+            self._metadata = None
+            self._log_queue.clear()
+            self._link.disconnect()
+            self._closed = True
 
     @property
     def connected(self) -> bool:
-        return self._sensor_infos != {} and self._system_info is not None
+        return self._server_info is not None
 
     @property
     def server_info(self) -> ServerInfo:
         self._assert_connected()
 
-        assert self._system_info is not None  # Should never happend if client is connected
-        return ServerInfo(
-            rss_version=self._system_info["rss_version"],
-            sensor_count=self._system_info["sensor_count"],
-            ticks_per_second=self._system_info["ticks_per_second"],
-            hardware_name=self._system_info.get("hw", None),
-            sensor_infos=self._sensor_infos,
-            max_baudrate=self._system_info.get("max_baudrate"),
-        )
+        assert self._server_info is not None  # Should never happend if client is connected
+        return self._server_info
 
 
 class TickUnwrapper:
     """Wraps unwrap_ticks to be applied over extended results"""
 
     def __init__(self) -> None:
         self.next_minimum_tick: Optional[int] = None
```

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/links.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/links.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/message.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,31 +87,29 @@
         tcp_port: Optional[int] = None,
         serial_port: Optional[str] = None,
         usb_device: Optional[Union[str, bool]] = None,
         mock: Optional[bool] = None,
         override_baudrate: Optional[int] = None,
         _override_protocol: Optional[Type[CommunicationProtocol]] = None,
     ) -> Client:
+        if mock is None:
+            raise ClientCreationError
 
         client_info = ClientInfo._from_open(
             mock=mock,
         )
 
         return cls(client_info=client_info)
 
     def __init__(self, client_info: ClientInfo = ClientInfo(mock=MockInfo())) -> None:
-
-        if client_info.mock is None:
-            raise ClientCreationError()
-
+        super().__init__(client_info)
         self._start_time = time.perf_counter()
-        self._connected = False
+        self._connected = True
         self._mock_update_rate = self.MAX_MOCK_UPDATE_RATE_HZ
         self._mock_next_data_time = 0.0
-        super().__init__(client_info)
 
     @classmethod
     def _sensor_config_to_metadata(
         cls, sensor_config: SensorConfig, update_rate: Optional[float]
     ) -> Metadata:
         subsweep_data_length = []
         subsweep_data_offset = []
@@ -214,20 +212,14 @@
         for group in config.groups:
             result_dict = {}
             for sensor_id, sensor_config in group.items():
                 result_dict[sensor_id] = self._sensor_config_to_result(sensor_id, sensor_config)
             result_list.append(result_dict)
         return result_list
 
-    def _open(self) -> None:
-        if not self._connected:
-            self._connected = True
-        else:
-            raise ClientError("Client is already connected")
-
     def setup_session(
         self,
         config: Union[SensorConfig, SessionConfig],
         calibrations: Optional[dict[int, SensorCalibration]] = None,
     ) -> Union[Metadata, list[dict[int, Metadata]]]:
         if self.session_is_started:
             raise ClientError("Session is currently running, can't setup.")
```

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/session_schema.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/session_schema.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/utils.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core_ext/_replaying_client.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core_ext/_replaying_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_perf_calc.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_perf_calc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_rate_calc.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_rate_calc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/__init__.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_base.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/_a121.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/_a121.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,17 @@
         else:
             self._recorder = None
 
         self.callback(PluginStateMessage(state=PluginState.LOADED_STARTING))
         try:
             self._start_session(self._recorder)
         except Exception as exc:
+            recorder = self.client.detach_recorder()
+            if recorder is not None:
+                recorder.close()
             self.callback(PluginStateMessage(state=PluginState.LOADED_IDLE))
             raise HandledException("Could not start") from exc
 
         self._started = True
 
         self.broadcast()
```

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_utils.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/bilateration/_plugin.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/bilateration/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/bilateration/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/bilateration/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/breathing/_configs.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/breathing/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/breathing/_ref_app.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/_ref_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/breathing/_ref_app_plugin.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/_ref_app_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/breathing/_serializer.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/_serializer.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/__main__.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/_aggregator.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/_aggregator.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/_detector.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
                 continue
 
             if isinstance(v, a121.SessionConfig):
                 _create_h5_string_dataset(group, k, v.to_json())
             elif isinstance(v, a121.SensorCalibration):
                 sensor_calibration_group = group.create_group("sensor_calibration")
                 v.to_h5(sensor_calibration_group)
-            elif isinstance(v, (np.ndarray, float, int, np.int64)):
+            elif isinstance(v, (np.ndarray, float, int, np.integer)):
                 group.create_dataset(k, data=v, track_times=False)
             else:
                 raise RuntimeError(
                     f"Unexpected {type(self).__name__} field '{k}' of type '{type(v)}'"
                 )
 
         if self.recorded_thresholds_mean_sweep is not None:
```

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/_processors.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/_processors.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/_serializers.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/_serializers.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/_configs.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/_configs.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,7 +69,30 @@
         inter_frame_slow_cutoff=0.2,
         inter_frame_fast_cutoff=6,
         inter_frame_deviation_time_const=0.5,
         inter_output_time_const=2,
         inter_phase_boost=False,
         inter_frame_presence_timeout=3,
     )
+
+
+def get_low_power_config() -> DetectorConfig:
+    return DetectorConfig(
+        start_m=0.725,
+        end_m=1.505,
+        frame_rate=1,
+        sweeps_per_frame=16,
+        hwaas=8,
+        inter_frame_idle_state=a121.IdleState.DEEP_SLEEP,
+        intra_enable=True,
+        intra_detection_threshold=1.5,
+        intra_frame_time_const=0.15,
+        intra_output_time_const=0.3,
+        inter_enable=True,
+        inter_detection_threshold=1,
+        inter_frame_slow_cutoff=0.2,
+        inter_frame_fast_cutoff=5,
+        inter_frame_deviation_time_const=0.5,
+        inter_output_time_const=2,
+        inter_phase_boost=False,
+        inter_frame_presence_timeout=3,
+    )
```

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/_detector.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,35 @@
                 or is_multiple_of(SPARSE_IQ_PPC, step_length)
             ):
                 raise ValueError(f"step_length must be a divisor or multiple of {SPARSE_IQ_PPC}")
 
     def _collect_validation_results(self) -> list[a121.ValidationResult]:
         validation_results: list[a121.ValidationResult] = []
 
+        for res in Detector._get_sensor_config(self)._collect_validation_results():
+            res.source = self
+
+            if res.aspect == "num_points":
+                validation_results.append(
+                    a121.ValidationError(
+                        self,
+                        "start_m",
+                        "Range is too long. Increasing the range start reduces buffer usage.",
+                    )
+                )
+                validation_results.append(
+                    a121.ValidationError(
+                        self,
+                        "end_m",
+                        "Range is too long. Decreasing the range end reduces buffer usage.",
+                    )
+                )
+            else:
+                validation_results.append(res)
+
         if self.sweeps_per_frame <= Processor.NOISE_ESTIMATION_DIFF_ORDER:
             validation_results.append(
                 a121.ValidationError(
                     self,
                     "sweeps_per_frame",
                     f"Must be greater than {Processor.NOISE_ESTIMATION_DIFF_ORDER}",
                 )
@@ -365,26 +386,35 @@
             processor_extra_result=processor_result.extra_result,
             service_result=result,
         )
 
     def update_config(self, config: DetectorConfig) -> None:
         raise NotImplementedError
 
-    def stop(self) -> Any:
+    def stop_detector(self) -> Any:
         if not self.started:
             raise RuntimeError("Already stopped")
 
         self.client.stop_session()
+        self.started = False
+
+        return None
+
+    def stop_recorder(self) -> Any:
         recorder = self.client.detach_recorder()
         if recorder is None:
             recorder_result = None
         else:
             recorder_result = recorder.close()
 
-        self.started = False
+        return recorder_result
+
+    def stop(self) -> Any:
+        self.stop_detector()
+        recorder_result = self.stop_recorder()
 
         return recorder_result
 
 
 def _record_algo_data(
     algo_group: h5py.Group,
     sensor_id: int,
```

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,20 @@
     icons,
     is_task,
     pidgets,
 )
 from acconeer.exptool.app.new.ui.plugin_components.pidgets.hooks import disable_if, parameter_is
 from acconeer.exptool.app.new.ui.plugin_components.save_dialog import PresentationType
 
-from ._configs import get_long_range_config, get_medium_range_config, get_short_range_config
+from ._configs import (
+    get_long_range_config,
+    get_low_power_config,
+    get_medium_range_config,
+    get_short_range_config,
+)
 from ._detector import (
     Detector,
     DetectorConfig,
     DetectorContext,
     DetectorMetadata,
     DetectorResult,
     _load_algo_data,
@@ -63,21 +68,23 @@
     context: Optional[DetectorContext] = attrs.field(default=None)
 
 
 class PluginPresetId(Enum):
     SHORT_RANGE = auto()
     MEDIUM_RANGE = auto()
     LONG_RANGE = auto()
+    LOW_POWER = auto()
 
 
 class BackendPlugin(DetectorBackendPluginBase[SharedState]):
     PLUGIN_PRESETS: Mapping[int, Callable[[], DetectorConfig]] = {
         PluginPresetId.SHORT_RANGE.value: lambda: get_short_range_config(),
         PluginPresetId.MEDIUM_RANGE.value: lambda: get_medium_range_config(),
         PluginPresetId.LONG_RANGE.value: lambda: get_long_range_config(),
+        PluginPresetId.LOW_POWER.value: lambda: get_low_power_config(),
     }
 
     def __init__(
         self, callback: Callable[[Message], None], generation: PluginGeneration, key: str
     ) -> None:
         super().__init__(callback=callback, generation=generation, key=key)
 
@@ -746,10 +753,15 @@
             preset_id=PluginPresetId.MEDIUM_RANGE,
         ),
         PluginPresetBase(
             name="Long range",
             description="Long range",
             preset_id=PluginPresetId.LONG_RANGE,
         ),
+        PluginPresetBase(
+            name="Low power, Wake up",
+            description="Low power presence detection, which can be used as a trigger",
+            preset_id=PluginPresetId.LOW_POWER,
+        ),
     ],
     default_preset_id=PluginPresetId.MEDIUM_RANGE,
 )
```

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/_processors.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/_processors.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/_serializers.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/_serializers.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/smart_presence/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/smart_presence/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,397 +7,326 @@
 from enum import Enum, auto
 from typing import Callable, Mapping, Optional
 
 import attrs
 import h5py
 import numpy as np
 
-from PySide6 import QtCore
 from PySide6.QtWidgets import QPushButton, QVBoxLayout, QWidget
 
 import pyqtgraph as pg
 
 import acconeer.exptool as et
 from acconeer.exptool import a121
 from acconeer.exptool.a121._h5_utils import _create_h5_string_dataset
-from acconeer.exptool.a121.algo._base import AlgoBase
 from acconeer.exptool.a121.algo._plugins import (
     DetectorBackendPluginBase,
     DetectorPlotPluginBase,
     DetectorViewPluginBase,
 )
-from acconeer.exptool.a121.algo.presence._detector import Detector
-from acconeer.exptool.a121.algo.presence._detector_plugin import ViewPlugin as PresenceViewPlugin
 from acconeer.exptool.app.new import (
     AppModel,
     AttrsConfigEditor,
     BackendLogger,
     GeneralMessage,
     GroupBox,
     Message,
     MiscErrorView,
-    PidgetGroupFactoryMapping,
+    PidgetFactoryMapping,
     PluginFamily,
     PluginGeneration,
     PluginPresetBase,
     PluginSpecBase,
     PluginState,
     icons,
     is_task,
     pidgets,
 )
+from acconeer.exptool.app.new.ui.plugin_components.range_help_view import RangeHelpView
 
-from ._configs import get_long_range_config, get_medium_range_config, get_short_range_config
-from ._ref_app import RefApp, RefAppConfig, RefAppResult, _load_algo_data
-
-
-@attrs.mutable(kw_only=True)
-class PlotConfig(AlgoBase):
-    show_all_detected_zones: bool = attrs.field(default=False)
+from ._example_app import ExampleApp, ExampleAppConfig, ExampleAppResult, _load_algo_data
 
 
 @attrs.mutable(kw_only=True)
 class SharedState:
     sensor_id: int = attrs.field(default=1)
-    config: RefAppConfig = attrs.field(factory=RefAppConfig)
-    plot_config: PlotConfig = attrs.field(factory=PlotConfig)
+    config: ExampleAppConfig = attrs.field(factory=ExampleAppConfig)
 
 
 class PluginPresetId(Enum):
-    SHORT_RANGE = auto()
-    MEDIUM_RANGE = auto()
-    LONG_RANGE = auto()
+    DEFAULT = auto()
 
 
 class BackendPlugin(DetectorBackendPluginBase[SharedState]):
 
-    PLUGIN_PRESETS: Mapping[int, Callable[[], RefAppConfig]] = {
-        PluginPresetId.SHORT_RANGE.value: lambda: get_short_range_config(),
-        PluginPresetId.MEDIUM_RANGE.value: lambda: get_medium_range_config(),
-        PluginPresetId.LONG_RANGE.value: lambda: get_long_range_config(),
+    PLUGIN_PRESETS: Mapping[int, Callable[[], ExampleAppConfig]] = {
+        PluginPresetId.DEFAULT.value: lambda: ExampleAppConfig()
     }
 
     def __init__(
         self, callback: Callable[[Message], None], generation: PluginGeneration, key: str
     ) -> None:
         super().__init__(callback=callback, generation=generation, key=key)
 
         self._recorder: Optional[a121.H5Recorder] = None
-        self._ref_app_instance: Optional[RefApp] = None
+        self._exempel_app_instance: Optional[ExampleApp] = None
         self._log = BackendLogger.getLogger(__name__)
 
         self.restore_defaults()
 
     def _load_from_cache(self, file: h5py.File) -> None:
-        self.shared_state.config = RefAppConfig.from_json(file["config"][()])
-        self.shared_state.plot_config = PlotConfig.from_json(file["plot_config"][()])
-
-        show_all_detected_zones = self.shared_state.plot_config.show_all_detected_zones
-        self.shared_state.config.show_all_detected_zones = show_all_detected_zones
+        self.shared_state.config = ExampleAppConfig.from_json(file["config"][()])
 
     @is_task
     def restore_defaults(self) -> None:
         self.shared_state = SharedState()
         self.broadcast()
 
     @is_task
     def update_sensor_id(self, *, sensor_id: int) -> None:
         self.shared_state.sensor_id = sensor_id
         self.broadcast()
 
-    @is_task
-    def update_plot_config(self, *, config: PlotConfig) -> None:
-        self.shared_state.plot_config = config
-        self.broadcast()
-
     def _sync_sensor_ids(self) -> None:
         if self.client is not None:
             sensor_ids = self.client.server_info.connected_sensors
 
             if len(sensor_ids) > 0 and self.shared_state.sensor_id not in sensor_ids:
                 self.shared_state.sensor_id = sensor_ids[0]
 
     @is_task
-    def update_config(self, *, config: RefAppConfig) -> None:
+    def update_config(self, *, config: ExampleAppConfig) -> None:
         self.shared_state.config = config
         self.broadcast()
 
     def save_to_cache(self, file: h5py.File) -> None:
         _create_h5_string_dataset(file, "config", self.shared_state.config.to_json())
-        _create_h5_string_dataset(file, "plot_config", self.shared_state.plot_config.to_json())
 
     @is_task
     def set_preset(self, preset_id: int) -> None:
         preset_config = self.PLUGIN_PRESETS[preset_id]
         self.shared_state.config = preset_config()
-        self.shared_state.plot_config = PlotConfig()
         self.broadcast()
 
     def load_from_record_setup(self, *, record: a121.H5Record) -> None:
         algo_group = record.get_algo_group(self.key)
         _, config = _load_algo_data(algo_group)
         self.shared_state.config = config
         self.shared_state.sensor_id = record.sensor_id
 
     def _start_session(self, recorder: Optional[a121.H5Recorder]) -> None:
         assert self.client
-        self._ref_app_instance = RefApp(
+        self._example_app_instance = ExampleApp(
             client=self.client,
             sensor_id=self.shared_state.sensor_id,
-            ref_app_config=self.shared_state.config,
+            example_app_config=self.shared_state.config,
         )
-        self._ref_app_instance.start(recorder)
+        self._example_app_instance.start(recorder)
         self.callback(
             GeneralMessage(
                 name="setup",
                 kwargs=dict(
-                    ref_app_config=self.shared_state.config,
-                    sensor_config=Detector._get_sensor_config(
-                        self._ref_app_instance.detector.config
-                    ),
-                    plot_config=self.shared_state.plot_config,
-                    estimated_frame_rate=self._ref_app_instance.detector.estimated_frame_rate,
+                    example_app_config=self.shared_state.config,
                 ),
                 recipient="plot_plugin",
             )
         )
 
     def end_session(self) -> None:
-        if self._ref_app_instance is None:
+        if self._example_app_instance is None:
             raise RuntimeError
         if self._recorder is not None:
             self._recorder.close()
-        self._ref_app_instance.stop()
+        self._example_app_instance.stop()
 
     def get_next(self) -> None:
         assert self.client
-        if self._ref_app_instance is None:
+        if self._example_app_instance is None:
             raise RuntimeError
-        result = self._ref_app_instance.get_next()
+        result = self._example_app_instance.get_next()
 
         self.callback(GeneralMessage(name="plot", data=result, recipient="plot_plugin"))
 
 
 class PlotPlugin(DetectorPlotPluginBase):
+
+    _VELOCITY_Y_SCALE_MARGIN_M = 0.25
+
     def __init__(self, *, plot_layout: pg.GraphicsLayout, app_model: AppModel) -> None:
         super().__init__(plot_layout=plot_layout, app_model=app_model)
 
     def setup_from_message(self, message: GeneralMessage) -> None:
         assert message.kwargs is not None
         self.setup(**message.kwargs)
 
     def update_from_message(self, message: GeneralMessage) -> None:
-        assert isinstance(message.data, RefAppResult)
+        assert isinstance(message.data, ExampleAppResult)
         self.update(message.data)
 
     def setup(
         self,
-        ref_app_config: RefAppConfig,
-        sensor_config: a121.SensorConfig,
-        plot_config: PlotConfig,
-        estimated_frame_rate: float,
+        example_app_config: ExampleAppConfig,
     ) -> None:
-        self.ref_app_config = ref_app_config
-        self.distances = np.linspace(
-            ref_app_config.start_m, ref_app_config.end_m, sensor_config.num_points
-        )
-
-        self.show_all_detected_zones = plot_config.show_all_detected_zones
-
-        self.history_length_s = 5
-        self.history_length_n = int(round(self.history_length_s * estimated_frame_rate))
-        self.intra_history = np.zeros(self.history_length_n)
-        self.inter_history = np.zeros(self.history_length_n)
-
-        self.num_sectors = min(ref_app_config.num_zones, self.distances.size)
-        self.sector_size = max(1, -(-self.distances.size // self.num_sectors))
-
-        self.sector_offset = (self.num_sectors * self.sector_size - self.distances.size) // 2
-        win = self.plot_layout
-
-        self.intra_limit_lines = []
-        self.inter_limit_lines = []
-
-        # Intra presence history plot
-
-        self.intra_hist_plot = win.addPlot(
-            row=0,
-            col=0,
-            title="Intra presence history (fast motions)",
-        )
-        self.intra_hist_plot.setMenuEnabled(False)
-        self.intra_hist_plot.setMouseEnabled(x=False, y=False)
-        self.intra_hist_plot.hideButtons()
-        self.intra_hist_plot.showGrid(x=True, y=True)
-        self.intra_hist_plot.setLabel("bottom", "Time (s)")
-        self.intra_hist_plot.setLabel("left", "Score")
-        self.intra_hist_plot.setXRange(-self.history_length_s, 0)
-        self.intra_history_smooth_max = et.utils.SmoothMax(estimated_frame_rate)
-        self.intra_hist_plot.setYRange(0, 10)
-        if not self.ref_app_config.intra_enable:
-            intra_color = et.utils.color_cycler(1)
-            intra_color = f"{intra_color}50"
-            intra_dashed_pen = pg.mkPen(intra_color, width=2.5, style=QtCore.Qt.DashLine)
-            intra_pen = pg.mkPen(intra_color, width=2)
-        else:
-            intra_dashed_pen = et.utils.pg_pen_cycler(1, width=2.5, style="--")
-            intra_pen = et.utils.pg_pen_cycler(1)
 
-        self.intra_hist_curve = self.intra_hist_plot.plot(pen=intra_pen)
-        limit_line = pg.InfiniteLine(angle=0, pen=intra_dashed_pen)
-        self.intra_hist_plot.addItem(limit_line)
-        self.intra_limit_lines.append(limit_line)
-
-        for line in self.intra_limit_lines:
-            line.setPos(self.ref_app_config.intra_detection_threshold)
-
-        # Inter presence history plot
-
-        self.inter_hist_plot = win.addPlot(
-            row=0,
-            col=1,
-            title="Inter presence history (slow motions)",
-        )
-        self.inter_hist_plot.setMenuEnabled(False)
-        self.inter_hist_plot.setMouseEnabled(x=False, y=False)
-        self.inter_hist_plot.hideButtons()
-        self.inter_hist_plot.showGrid(x=True, y=True)
-        self.inter_hist_plot.setLabel("bottom", "Time (s)")
-        self.inter_hist_plot.setLabel("left", "Score")
-        self.inter_hist_plot.setXRange(-self.history_length_s, 0)
-        self.inter_history_smooth_max = et.utils.SmoothMax(estimated_frame_rate)
-        self.inter_hist_plot.setYRange(0, 10)
-        if not self.ref_app_config.inter_enable:
-            inter_color = et.utils.color_cycler(0)
-            inter_color = f"{inter_color}50"
-            inter_dashed_pen = pg.mkPen(inter_color, width=2.5, style=QtCore.Qt.DashLine)
-            inter_pen = pg.mkPen(inter_color, width=2)
+        self.slow_zone = example_app_config.slow_zone
+        self.history_length_s = 10
+        if example_app_config.frame_rate is None:
+            estimated_frame_rate = (
+                example_app_config.sweep_rate / example_app_config.sweeps_per_frame
+            )
         else:
-            inter_pen = et.utils.pg_pen_cycler(0)
-            inter_dashed_pen = et.utils.pg_pen_cycler(0, width=2.5, style="--")
+            estimated_frame_rate = example_app_config.frame_rate
+
+        self.history_length_n = int(np.around(self.history_length_s * estimated_frame_rate))
 
-        self.inter_hist_curve = self.inter_hist_plot.plot(pen=inter_pen)
-        limit_line = pg.InfiniteLine(angle=0, pen=inter_dashed_pen)
-        self.inter_hist_plot.addItem(limit_line)
-        self.inter_limit_lines.append(limit_line)
+        c0_dashed_pen = et.utils.pg_pen_cycler(0, width=2.5, style="--")
 
-        for line in self.inter_limit_lines:
-            line.setPos(self.ref_app_config.inter_detection_threshold)
+        # Velocity plot
 
-        # Sector plot
+        self.velocity_history_plot = self._create_plot(self.plot_layout, row=0, col=0)
+        self.velocity_history_plot.setTitle("Estimated velocity")
+        self.velocity_history_plot.setLabel(axis="left", text="Velocity", units="m/s")
+        self.velocity_history_plot.setLabel(axis="bottom", text="Time", units="s")
+        self.velocity_history_plot.addLegend(labelTextSize="10pt")
+        self.velocity_smooth_limits = et.utils.SmoothLimits()
 
-        self.sector_plot = pg.PlotItem(
-            title="Detection zone<br>Detection type: fast (orange), slow (blue), both (green)"
+        self.velocity_curve = self.velocity_history_plot.plot(
+            pen=et.utils.pg_pen_cycler(0), name="Estimated velocity"
         )
-        self.sector_plot.setAspectLocked()
-        self.sector_plot.hideAxis("left")
-        self.sector_plot.hideAxis("bottom")
-        self.sectors = []
-        self.limit_text = []
 
-        self.range_html = (
+        self.psd_html = (
             '<div style="text-align: center">'
-            '<span style="color: #000000;font-size:12pt;">'
+            '<span style="color: #FFFFFF;font-size:13pt;">'
             "{}</span></div>"
         )
 
-        pen = pg.mkPen("k", width=1)
-        span_deg = 25
-        for r in np.flip(np.arange(self.num_sectors) + 1):
-            sector = pg.QtWidgets.QGraphicsEllipseItem(-r, -r, r * 2, r * 2)
-            sector.setStartAngle(-16 * span_deg)
-            sector.setSpanAngle(16 * span_deg * 2)
-            sector.setPen(pen)
-            self.sector_plot.addItem(sector)
-            self.sectors.append(sector)
-
-            limit = pg.TextItem(html=self.range_html, anchor=(0.5, 0.5), angle=25)
-            x = r * np.cos(np.radians(span_deg))
-            y = r * np.sin(np.radians(span_deg))
-            limit.setPos(x, y + 0.25)
-            self.sector_plot.addItem(limit)
-            self.limit_text.append(limit)
-
-        self.sectors.reverse()
-
-        start_limit_text = pg.TextItem(html=self.range_html, anchor=(0.5, 0.5), angle=25)
-        range_html = self.range_html.format(f"{ref_app_config.start_m}")
-        start_limit_text.setHtml(range_html)
-        start_limit_text.setPos(0, 0.25)
-        self.sector_plot.addItem(start_limit_text)
-
-        unit_text = pg.TextItem(html=self.range_html, anchor=(0.5, 0.5))
-        unit_html = self.range_html.format("[m]")
-        unit_text.setHtml(unit_html)
-        unit_text.setPos(
-            self.num_sectors + 0.5, (self.num_sectors + 1) * np.sin(np.radians(span_deg))
-        )
-        self.sector_plot.addItem(unit_text)
-
-        sublayout = win.addLayout(row=1, col=0, colspan=2)
-        sublayout.layout.setColumnStretchFactor(0, 2)
-        sublayout.addItem(self.sector_plot, row=0, col=0)
-
-    def update(self, data: RefAppResult) -> None:
-
-        # Intra presence
-
-        move_hist_xs = np.linspace(-self.history_length_s, 0, self.history_length_n)
-
-        self.intra_history = np.roll(self.intra_history, -1)
-        self.intra_history[-1] = data.intra_presence_score
-
-        m_hist = max(
-            float(np.max(self.intra_history)), self.ref_app_config.intra_detection_threshold * 1.05
-        )
-        m_hist = self.intra_history_smooth_max.update(m_hist)
-
-        self.intra_hist_plot.setYRange(0, m_hist)
-        self.intra_hist_curve.setData(move_hist_xs, self.intra_history)
-
-        # Inter presence
-
-        self.inter_history = np.roll(self.inter_history, -1)
-        self.inter_history[-1] = data.inter_presence_score
-
-        m_hist = max(
-            float(np.max(self.inter_history)), self.ref_app_config.inter_detection_threshold * 1.05
-        )
-        m_hist = self.inter_history_smooth_max.update(m_hist)
-
-        self.inter_hist_plot.setYRange(0, m_hist)
-        self.inter_hist_curve.setData(move_hist_xs, self.inter_history)
-
-        # Sector
-
-        brush = et.utils.pg_brush_cycler(7)
-        for sector in self.sectors:
-            sector.setBrush(brush)
-
-        if data.presence_detected:
-            if self.show_all_detected_zones:
-                for zone, (inter_value, intra_value) in enumerate(
-                    zip(data.inter_zone_detections, data.intra_zone_detections)
-                ):
-                    if inter_value + intra_value == 2:
-                        self.sectors[zone].setBrush(et.utils.pg_brush_cycler(2))
-                    elif inter_value == 1:
-                        self.sectors[zone].setBrush(et.utils.pg_brush_cycler(0))
-                    elif intra_value == 1:
-                        self.sectors[zone].setBrush(et.utils.pg_brush_cycler(1))
-            else:
-                assert data.max_presence_zone is not None
-                if data.max_presence_zone == data.max_intra_zone:
-                    self.sectors[data.max_presence_zone].setBrush(et.utils.pg_brush_cycler(1))
-                else:
-                    self.sectors[data.max_presence_zone].setBrush(et.utils.pg_brush_cycler(0))
-
-        for (text_item, limit) in zip(self.limit_text, np.flip(data.zone_limits)):
-            range_html = self.range_html.format(np.around(limit, 1))
-            text_item.setHtml(range_html)
+        self.distance_text_item = pg.TextItem(
+            html=self.psd_html,
+            fill=pg.mkColor(0x1F, 0x77, 0xB4, 180),
+            anchor=(0.5, 0),
+        )
+
+        self.velocity_history_plot.addItem(self.distance_text_item)
+
+        self.velocity_history = np.zeros(self.history_length_n)
+
+        self.lower_std_history = np.zeros(self.history_length_n)
+        self.upper_std_history = np.zeros(self.history_length_n)
+
+        self.lower_std_curve = self.velocity_history_plot.plot()
+        self.upper_std_curve = self.velocity_history_plot.plot()
+
+        fbi = pg.FillBetweenItem(
+            self.lower_std_curve,
+            self.upper_std_curve,
+            brush=pg.mkBrush(f"{et.utils.color_cycler(0)}50"),
+        )
+
+        self.velocity_history_plot.addItem(fbi)
+
+        # PSD plot
+
+        self.psd_plot = self._create_plot(self.plot_layout, row=1, col=0)
+        self.psd_plot.setTitle("PSD<br>(colored area represents the slow zone)")
+        self.psd_plot.setLabel(axis="left", text="Power")
+        self.psd_plot.setLabel(axis="bottom", text="Velocity", units="m/s")
+        self.psd_plot.addLegend(labelTextSize="10pt")
+
+        self.psd_smooth_max = et.utils.SmoothMax(tau_grow=0.5, tau_decay=2.0)
+        self.psd_curve = self.psd_plot.plot(pen=et.utils.pg_pen_cycler(0), name="PSD")
+        self.psd_threshold = self.psd_plot.plot(pen=c0_dashed_pen, name="Threshold")
+
+        psd_slow_zone_color = et.utils.color_cycler(0)
+        psd_slow_zone_color = f"{psd_slow_zone_color}50"
+        psd_slow_zone_brush = pg.mkBrush(psd_slow_zone_color)
+
+        self.psd_slow_zone = pg.LinearRegionItem(brush=psd_slow_zone_brush, movable=False)
+        self.psd_plot.addItem(self.psd_slow_zone)
+
+        brush = et.utils.pg_brush_cycler(0)
+        self.psd_peak_plot_item = pg.PlotDataItem(
+            pen=None, symbol="o", symbolSize=8, symbolBrush=brush, symbolPen="k"
+        )
+        self.psd_plot.addItem(self.psd_peak_plot_item)
+
+        self.psd_plot.setLogMode(x=False, y=True)
+
+    def update(self, example_app_result: ExampleAppResult) -> None:
+        processor_extra_result = example_app_result.processor_extra_result
+
+        lim = self.velocity_smooth_limits.update(example_app_result.velocity)
+
+        self.velocity_history_plot.setYRange(
+            lim[0] - self._VELOCITY_Y_SCALE_MARGIN_M, lim[1] + self._VELOCITY_Y_SCALE_MARGIN_M
+        )
+        self.velocity_history_plot.setXRange(-self.history_length_s, 0)
+
+        xs = np.linspace(-self.history_length_s, 0, self.history_length_n)
+
+        self.velocity_history = np.roll(self.velocity_history, -1)
+        self.velocity_history[-1] = example_app_result.velocity
+        self.velocity_curve.setData(xs, self.velocity_history)
+
+        velocity_html = self.psd_html.format(
+            f"Distance {np.around(example_app_result.distance_m, 2)} m"
+        )
+        self.distance_text_item.setHtml(velocity_html)
+        self.distance_text_item.setPos(
+            -self.history_length_s / 2, lim[1] + self._VELOCITY_Y_SCALE_MARGIN_M
+        )
+
+        self.lower_std_history = np.roll(self.lower_std_history, -1)
+        self.lower_std_history[-1] = (
+            example_app_result.velocity + 0.5 * processor_extra_result.peak_width
+        )
+        self.lower_std_curve.setData(xs, self.lower_std_history)
+
+        self.upper_std_history = np.roll(self.upper_std_history, -1)
+        self.upper_std_history[-1] = (
+            example_app_result.velocity - 0.5 * processor_extra_result.peak_width
+        )
+        self.upper_std_curve.setData(xs, self.upper_std_history)
+
+        lim = self.psd_smooth_max.update(processor_extra_result.psd_threshold)
+        self.psd_plot.setYRange(np.log10(0.2), np.log10(lim))
+        self.psd_plot.setXRange(
+            processor_extra_result.max_bin_vertical_vs[0],
+            processor_extra_result.max_bin_vertical_vs[-1],
+        )
+        self.psd_curve.setData(
+            processor_extra_result.vertical_velocities, processor_extra_result.psd
+        )
+        self.psd_threshold.setData(
+            processor_extra_result.vertical_velocities, processor_extra_result.psd_threshold
+        )
+        if processor_extra_result.peak_idx is not None:
+            self.psd_peak_plot_item.setData(
+                [processor_extra_result.vertical_velocities[processor_extra_result.peak_idx]],
+                [processor_extra_result.psd[processor_extra_result.peak_idx]],
+            )
+        else:
+            self.psd_peak_plot_item.clear()
+
+        middle_idx = int(np.around(processor_extra_result.vertical_velocities.shape[0] / 2))
+        self.psd_slow_zone.setRegion(
+            [
+                processor_extra_result.vertical_velocities[middle_idx - self.slow_zone],
+                processor_extra_result.vertical_velocities[middle_idx + self.slow_zone],
+            ]
+        )
+
+    @staticmethod
+    def _create_plot(parent: pg.GraphicsLayout, row: int, col: int) -> pg.PlotItem:
+        velocity_history_plot = parent.addPlot(row=row, col=col)
+        velocity_history_plot.setMenuEnabled(False)
+        velocity_history_plot.setMouseEnabled(x=False, y=False)
+        velocity_history_plot.hideButtons()
+        velocity_history_plot.showGrid(x=True, y=True, alpha=0.5)
+
+        return velocity_history_plot
 
 
 class ViewPlugin(DetectorViewPluginBase):
     def __init__(self, app_model: AppModel, view_widget: QWidget) -> None:
         super().__init__(app_model=app_model, view_widget=view_widget)
         self._log = logging.getLogger(__name__)
 
@@ -429,65 +358,163 @@
         self.sensor_id_pidget = pidgets.SensorIdPidgetFactory(items=[]).create(
             parent=sensor_selection_group
         )
         self.sensor_id_pidget.sig_update.connect(self._on_sensor_id_update)
         sensor_selection_group.layout().addWidget(self.sensor_id_pidget)
         scrolly_layout.addWidget(sensor_selection_group)
 
+        self.range_helper = RangeHelpView()
+        scrolly_layout.addWidget(self.range_helper)
+
         self.config_editor = AttrsConfigEditor(
-            title="Ref App parameters",
+            title="Example app parameters",
             factory_mapping=self._get_pidget_mapping(),
-            config_type=RefAppConfig,
+            config_type=ExampleAppConfig,
             parent=self.scrolly_widget,
         )
         self.config_editor.sig_update.connect(self._on_config_update)
         scrolly_layout.addWidget(self.config_editor)
 
-        self.plot_config_editor = AttrsConfigEditor(
-            title="Plot parameters",
-            factory_mapping={
-                "show_all_detected_zones": pidgets.CheckboxPidgetFactory(
-                    name_label_text="Show all detected zones",
-                )
-            },
-            config_type=PlotConfig,
-            save_load_buttons=False,
-            parent=self.scrolly_widget,
-        )
-        self.plot_config_editor.sig_update.connect(self._on_plot_config_update)
-        scrolly_layout.addWidget(self.plot_config_editor)
-
         self.sticky_widget.setLayout(sticky_layout)
         self.scrolly_widget.setLayout(scrolly_layout)
 
     @classmethod
-    def _get_pidget_mapping(cls) -> PidgetGroupFactoryMapping:
-        presence_pidget_mapping = dict(PresenceViewPlugin._get_pidget_mapping())
-        presence_pidget_mapping.update(
-            {
-                pidgets.FlatPidgetGroup(): {
-                    "num_zones": pidgets.IntPidgetFactory(
-                        name_label_text="Number of zones",
-                        limits=(1, None),
-                    ),
-                }
-            }
-        )
-        return presence_pidget_mapping
+    def _get_pidget_mapping(cls) -> PidgetFactoryMapping:
+        return {
+            "surface_distance": pidgets.FloatPidgetFactory(
+                name_label_text="Surface distance",
+                suffix=" m",
+                decimals=2,
+                limits=(0.1, 3),
+            ),
+            "sensor_angle": pidgets.FloatPidgetFactory(
+                name_label_text="Sensor angle",
+                suffix=" degrees",
+                decimals=1,
+                limits=(0, 89),
+            ),
+            "num_points": pidgets.IntPidgetFactory(
+                name_label_text="Number of distance points",
+                limits=(1, None),
+            ),
+            "sweep_rate": pidgets.FloatPidgetFactory(
+                name_label_text="Sweep rate",
+                suffix=" Hz",
+                decimals=1,
+                limits=(100, None),
+            ),
+            "sweeps_per_frame": pidgets.IntPidgetFactory(
+                name_label_text="Sweeps per frame",
+                limits=(64, 2048),
+            ),
+            "hwaas": pidgets.IntPidgetFactory(
+                name_label_text="HWAAS",
+                limits=(1, 511),
+            ),
+            "profile": pidgets.OptionalEnumPidgetFactory(
+                name_label_text="Profile",
+                checkbox_label_text="Override",
+                enum_type=a121.Profile,
+                label_mapping={
+                    a121.Profile.PROFILE_1: "1 (shortest)",
+                    a121.Profile.PROFILE_2: "2",
+                    a121.Profile.PROFILE_3: "3",
+                    a121.Profile.PROFILE_4: "4",
+                    a121.Profile.PROFILE_5: "5 (longest)",
+                },
+            ),
+            "step_length": pidgets.IntPidgetFactory(
+                name_label_text="Step length:",
+                limits=(1, None),
+            ),
+            "frame_rate": pidgets.OptionalFloatPidgetFactory(
+                name_label_text="Frame rate",
+                checkbox_label_text="Limit",
+                suffix=" Hz",
+                decimals=1,
+                limits=(1, None),
+                init_set_value=10,
+            ),
+            "continuous_sweep_mode": pidgets.CheckboxPidgetFactory(
+                name_label_text="Continuos sweep mode",
+            ),
+            "double_buffering": pidgets.CheckboxPidgetFactory(
+                name_label_text="Double buffering",
+            ),
+            "inter_frame_idle_state": pidgets.EnumPidgetFactory(
+                enum_type=a121.IdleState,
+                name_label_text="Inter frame idle state",
+                label_mapping={
+                    a121.IdleState.DEEP_SLEEP: "Deep sleep",
+                    a121.IdleState.SLEEP: "Sleep",
+                    a121.IdleState.READY: "Ready",
+                },
+            ),
+            "inter_sweep_idle_state": pidgets.EnumPidgetFactory(
+                enum_type=a121.IdleState,
+                name_label_text="Inter sweep idle state",
+                label_mapping={
+                    a121.IdleState.DEEP_SLEEP: "Deep sleep",
+                    a121.IdleState.SLEEP: "Sleep",
+                    a121.IdleState.READY: "Ready",
+                },
+            ),
+            "time_series_length": pidgets.IntPidgetFactory(
+                name_label_text="Time series length",
+                limits=(64, None),
+            ),
+            "psd_lp_coeff": pidgets.FloatSliderPidgetFactory(
+                name_label_text="PSD time filtering coeff.",
+                limits=(0, 1),
+                decimals=3,
+            ),
+            "slow_zone": pidgets.IntPidgetFactory(
+                name_label_text="Slow zone half length",
+                limits=(0, 20),
+            ),
+            "velocity_lp_coeff": pidgets.FloatSliderPidgetFactory(
+                name_label_text="Velocity time filtering coeff.\nper time series",
+                limits=(0, 1),
+                decimals=3,
+            ),
+            "cfar_win": pidgets.IntPidgetFactory(
+                name_label_text="CFAR window length",
+                limits=(0, 20),
+            ),
+            "cfar_guard": pidgets.IntPidgetFactory(
+                name_label_text="CFAR guard length",
+                limits=(0, 20),
+            ),
+            "cfar_sensitivity": pidgets.FloatSliderPidgetFactory(
+                name_label_text="Threshold sensitivity",
+                decimals=2,
+                limits=(0.01, 1),
+            ),
+            "max_peak_interval_s": pidgets.FloatPidgetFactory(
+                name_label_text="Max peak interval",
+                decimals=1,
+                limits=(0, 20),
+                suffix=" s",
+            ),
+        }
 
     def on_backend_state_update(self, backend_plugin_state: Optional[SharedState]) -> None:
         if backend_plugin_state is not None and backend_plugin_state.config is not None:
             results = backend_plugin_state.config._collect_validation_results()
 
             not_handled = self.config_editor.handle_validation_results(results)
 
             not_handled = self.misc_error_view.handle_validation_results(not_handled)
 
             assert not_handled == []
 
+            self.range_helper.update(
+                ExampleApp._get_sensor_config(backend_plugin_state.config).subsweep
+            )
+
     def on_app_model_update(self, app_model: AppModel) -> None:
         state = app_model.backend_plugin_state
 
         if state is None:
             self.start_button.setEnabled(False)
             self.stop_button.setEnabled(False)
 
@@ -497,30 +524,25 @@
 
             return
 
         assert isinstance(state, SharedState)
 
         self.config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
         self.config_editor.set_data(state.config)
-        self.plot_config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
-        self.plot_config_editor.set_data(state.plot_config)
         self.sensor_id_pidget.set_selected_sensor(state.sensor_id, app_model.connected_sensors)
         self.sensor_id_pidget.setEnabled(app_model.plugin_state.is_steady)
 
         self.start_button.setEnabled(
             app_model.is_ready_for_session() and self.config_editor.is_ready
         )
         self.stop_button.setEnabled(app_model.plugin_state == PluginState.LOADED_BUSY)
 
-    def _on_config_update(self, config: RefAppConfig) -> None:
+    def _on_config_update(self, config: ExampleAppConfig) -> None:
         BackendPlugin.update_config.rpc(self.app_model.put_task, config=config)
 
-    def _on_plot_config_update(self, config: PlotConfig) -> None:
-        BackendPlugin.update_plot_config.rpc(self.app_model.put_task, config=config)
-
     def _send_defaults_request(self) -> None:
         BackendPlugin.restore_defaults.rpc(self.app_model.put_task)
 
     def _on_sensor_id_update(self, sensor_id: int) -> None:
         BackendPlugin.update_sensor_id.rpc(self.app_model.put_task, sensor_id=sensor_id)
 
 
@@ -535,32 +557,18 @@
 
     def create_plot_plugin(
         self, app_model: AppModel, plot_layout: pg.GraphicsLayout
     ) -> PlotPlugin:
         return PlotPlugin(app_model=app_model, plot_layout=plot_layout)
 
 
-SMART_PRESENCE_PLUGIN = PluginSpec(
+SURFACE_VELOCITY_PLUGIN = PluginSpec(
     generation=PluginGeneration.A121,
-    key="smart_presence",
-    title="Smart presence",
-    description="Split presence detection range into zones.",
-    family=PluginFamily.REF_APP,
+    key="surface_velocity",
+    title="Surface velocity",
+    description="Estimate surface speed and direction of streaming water.",
+    family=PluginFamily.EXAMPLE_APP,
     presets=[
-        PluginPresetBase(
-            name="Short range",
-            description="Short range",
-            preset_id=PluginPresetId.SHORT_RANGE,
-        ),
-        PluginPresetBase(
-            name="Medium range",
-            description="Medium range",
-            preset_id=PluginPresetId.MEDIUM_RANGE,
-        ),
-        PluginPresetBase(
-            name="Long range",
-            description="Long range",
-            preset_id=PluginPresetId.LONG_RANGE,
-        ),
+        PluginPresetBase(name="Default", preset_id=PluginPresetId.DEFAULT),
     ],
-    default_preset_id=PluginPresetId.MEDIUM_RANGE,
+    default_preset_id=PluginPresetId.DEFAULT,
 )
```

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/speed/_detector.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/speed/_detector.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,14 +116,24 @@
 
         min_sweep_rate = self._get_min_sweep_rate(self.max_speed)
         frame_rate = self.frame_rate
         sweep_rate = self.sweep_rate
         sweeps_per_frame = self.num_bins * NUM_SEGMENTS
 
         max_frame_rate = None
+        profile_3_direct_leakage_end = int(
+            2 * ENVELOPE_FWHM_M[a121.Profile.PROFILE_3] / PERCEIVED_WAVELENGTH
+        )
+
+        if self.start_point < profile_3_direct_leakage_end:
+            validation_results.append(
+                a121.ValidationWarning(
+                    self, "start_point", "Range includes direct leakage, risk for missed detection"
+                )
+            )
 
         if self.num_points == 1 and self.step_length is not None:
             validation_results.append(
                 a121.ValidationWarning(
                     self,
                     "step_length",
                     "Step length is not used when sampling a single point.",
@@ -200,35 +210,40 @@
     """Profile used for measurement"""
 
 
 @attrs.frozen(kw_only=True)
 class DetectorExtraResult:
 
     psd: npt.NDArray[np.float_]
+    """Full Power Spectral Density from the DFT"""
+
     velocities: npt.NDArray[np.float_]
+    """The frequency bins interpreted as speeds"""
+
     actual_thresholds: npt.NDArray[np.float_]
-    display_speed: np.float_ = attrs.field(default=0.0)
+    """The thresholds that was used in this frame"""
 
 
 @attrs.frozen(kw_only=True)
 class DetectorResult:
 
     speed_per_depth: npt.NDArray[np.float_]
+    """The measured speed for each depth"""
+
     extra_result: DetectorExtraResult
+    """Detailed results, used for plotting"""
 
     @property
     def max_speed(self) -> np.float_:
         return max(np.min(self.speed_per_depth), np.max(self.speed_per_depth), key=np.abs)
 
 
 class Detector(Controller[DetectorConfig, DetectorResult]):
     MIN_DIST_M = {
-        a121.Profile.PROFILE_1: 2 * ENVELOPE_FWHM_M[a121.Profile.PROFILE_1],
-        a121.Profile.PROFILE_2: 2 * ENVELOPE_FWHM_M[a121.Profile.PROFILE_2],
-        a121.Profile.PROFILE_3: 2 * ENVELOPE_FWHM_M[a121.Profile.PROFILE_3],
+        a121.Profile.PROFILE_3: None,
         a121.Profile.PROFILE_4: 2 * ENVELOPE_FWHM_M[a121.Profile.PROFILE_4],
         a121.Profile.PROFILE_5: 2 * ENVELOPE_FWHM_M[a121.Profile.PROFILE_5],
     }
 
     DEFAULT_STEP_LENGTH = {
         a121.Profile.PROFILE_1: 12,
         a121.Profile.PROFILE_2: 24,
```

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/speed/_detector_plugin.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/speed/_detector_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/speed/_processors.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/speed/_processors.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/tank_level/_plugin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,337 +1,501 @@
 # Copyright (c) Acconeer AB, 2023
 # All rights reserved
 
 from __future__ import annotations
 
 import logging
 from enum import Enum, auto
-from typing import Callable, Mapping, Optional
+from typing import Any, Callable, Mapping, Optional
 
 import attrs
 import h5py
 import numpy as np
 
-from PySide6.QtWidgets import QPushButton, QVBoxLayout, QWidget
+from PySide6.QtWidgets import QLabel, QPushButton, QVBoxLayout, QWidget
 
 import pyqtgraph as pg
 
 import acconeer.exptool as et
 from acconeer.exptool import a121
 from acconeer.exptool.a121._h5_utils import _create_h5_string_dataset
 from acconeer.exptool.a121.algo._plugins import (
     DetectorBackendPluginBase,
     DetectorPlotPluginBase,
     DetectorViewPluginBase,
 )
+from acconeer.exptool.a121.algo.distance._detector import DetailedStatus, Detector
+from acconeer.exptool.a121.algo.distance._detector_plugin import ViewPlugin as DistanceViewPlugin
+from acconeer.exptool.a121.algo.tank_level._configs import (
+    get_large_config,
+    get_medium_config,
+    get_small_config,
+)
+from acconeer.exptool.a121.algo.tank_level._processor import ProcessorLevelStatus
+from acconeer.exptool.a121.algo.tank_level._ref_app import (
+    RefApp,
+    RefAppConfig,
+    RefAppContext,
+    RefAppResult,
+    _load_algo_data,
+)
 from acconeer.exptool.app.new import (
     AppModel,
-    AttrsConfigEditor,
     BackendLogger,
     GeneralMessage,
     GroupBox,
+    HandledException,
     Message,
-    MiscErrorView,
-    PidgetFactoryMapping,
     PluginFamily,
     PluginGeneration,
     PluginPresetBase,
     PluginSpecBase,
     PluginState,
+    PluginStateMessage,
     icons,
     is_task,
+)
+from acconeer.exptool.app.new.ui.plugin_components import (
+    AttrsConfigEditor,
+    PidgetFactoryMapping,
+    PresentationType,
     pidgets,
 )
-from acconeer.exptool.app.new.ui.plugin_components.range_help_view import RangeHelpView
 
-from ._example_app import ExampleApp, ExampleAppConfig, ExampleAppResult, _load_algo_data
+
+NO_DETECTION_TIMEOUT = 50
+TIME_HISTORY_S = 30
 
 
 @attrs.mutable(kw_only=True)
 class SharedState:
     sensor_id: int = attrs.field(default=1)
-    config: ExampleAppConfig = attrs.field(factory=ExampleAppConfig)
+    config: RefAppConfig = attrs.field(factory=RefAppConfig)
+    context: RefAppContext = attrs.field(factory=RefAppContext)
 
 
 class PluginPresetId(Enum):
-    DEFAULT = auto()
+    SMALL = auto()
+    MEDIUM = auto()
+    LARGE = auto()
+
+
+@attrs.mutable(kw_only=True)
+class TankLevelPreset:
+    config: RefAppConfig = attrs.field()
 
 
 class BackendPlugin(DetectorBackendPluginBase[SharedState]):
 
-    PLUGIN_PRESETS: Mapping[int, Callable[[], ExampleAppConfig]] = {
-        PluginPresetId.DEFAULT.value: lambda: ExampleAppConfig()
+    PLUGIN_PRESETS: Mapping[int, TankLevelPreset] = {
+        PluginPresetId.SMALL.value: TankLevelPreset(
+            config=get_small_config(),
+        ),
+        PluginPresetId.MEDIUM.value: TankLevelPreset(
+            config=get_medium_config(),
+        ),
+        PluginPresetId.LARGE.value: TankLevelPreset(
+            config=get_large_config(),
+        ),
     }
 
     def __init__(
         self, callback: Callable[[Message], None], generation: PluginGeneration, key: str
     ) -> None:
         super().__init__(callback=callback, generation=generation, key=key)
 
-        self._recorder: Optional[a121.H5Recorder] = None
-        self._exempel_app_instance: Optional[ExampleApp] = None
+        self._recorder = None
+        self._ref_app_instance: Optional[RefApp] = None
         self._log = BackendLogger.getLogger(__name__)
 
         self.restore_defaults()
 
     def _load_from_cache(self, file: h5py.File) -> None:
-        self.shared_state.config = ExampleAppConfig.from_json(file["config"][()])
+        self.shared_state.config = RefAppConfig.from_json(file["config"][()])
+        self.shared_state.context = RefAppContext.from_h5(file["context"])
 
     @is_task
     def restore_defaults(self) -> None:
-        self.shared_state = SharedState()
-        self.broadcast()
-
-    @is_task
-    def update_sensor_id(self, *, sensor_id: int) -> None:
-        self.shared_state.sensor_id = sensor_id
+        self.shared_state = SharedState(config=get_small_config())
         self.broadcast()
 
     def _sync_sensor_ids(self) -> None:
         if self.client is not None:
             sensor_ids = self.client.server_info.connected_sensors
 
             if len(sensor_ids) > 0 and self.shared_state.sensor_id not in sensor_ids:
                 self.shared_state.sensor_id = sensor_ids[0]
 
     @is_task
-    def update_config(self, *, config: ExampleAppConfig) -> None:
+    def update_config(self, *, config: RefAppConfig) -> None:
         self.shared_state.config = config
         self.broadcast()
 
-    def save_to_cache(self, file: h5py.File) -> None:
-        _create_h5_string_dataset(file, "config", self.shared_state.config.to_json())
+    @is_task
+    def update_sensor_id(self, *, sensor_id: int) -> None:
+        self.shared_state.sensor_id = sensor_id
+        self.broadcast()
 
     @is_task
     def set_preset(self, preset_id: int) -> None:
         preset_config = self.PLUGIN_PRESETS[preset_id]
-        self.shared_state.config = preset_config()
+        self.shared_state.config = preset_config.config
         self.broadcast()
 
+    def save_to_cache(self, file: h5py.File) -> None:
+        _create_h5_string_dataset(file, "config", self.shared_state.config.to_json())
+        context_group = file.create_group("context")
+        self.shared_state.context.to_h5(context_group)
+
     def load_from_record_setup(self, *, record: a121.H5Record) -> None:
         algo_group = record.get_algo_group(self.key)
-        _, config = _load_algo_data(algo_group)
+        sensor_id, config, context = _load_algo_data(algo_group)
         self.shared_state.config = config
-        self.shared_state.sensor_id = record.sensor_id
+        self.shared_state.context = context
+        self.shared_state.sensor_id = sensor_id
 
     def _start_session(self, recorder: Optional[a121.H5Recorder]) -> None:
         assert self.client
-        self._example_app_instance = ExampleApp(
+
+        self._ref_app_instance = RefApp(
             client=self.client,
             sensor_id=self.shared_state.sensor_id,
-            example_app_config=self.shared_state.config,
+            config=self.shared_state.config,
+            context=self.shared_state.context,
         )
-        self._example_app_instance.start(recorder)
+
+        self._ref_app_instance.start(recorder)
+
         self.callback(
             GeneralMessage(
                 name="setup",
-                kwargs=dict(
-                    example_app_config=self.shared_state.config,
-                ),
+                kwargs={
+                    "config": self.shared_state.config,
+                    "num_curves": len(self._ref_app_instance._detector.processor_specs),
+                },
                 recipient="plot_plugin",
             )
         )
 
     def end_session(self) -> None:
-        if self._example_app_instance is None:
+        if self._ref_app_instance is None:
             raise RuntimeError
+
         if self._recorder is not None:
             self._recorder.close()
-        self._example_app_instance.stop()
+
+        self._ref_app_instance.stop()
 
     def get_next(self) -> None:
-        assert self.client
-        if self._example_app_instance is None:
+        assert self.client is not None
+        if self._ref_app_instance is None:
             raise RuntimeError
-        result = self._example_app_instance.get_next()
+        result = self._ref_app_instance.get_next()
 
         self.callback(GeneralMessage(name="plot", data=result, recipient="plot_plugin"))
 
+    @is_task
+    def calibrate_detector(self) -> None:
+        if self._started:
+            raise RuntimeError
+
+        if self.client is None:
+            raise RuntimeError
+
+        if not self.client.connected:
+            raise RuntimeError
+
+        self.callback(PluginStateMessage(state=PluginState.LOADED_BUSY))
+
+        try:
+            self._ref_app_instance = RefApp(
+                client=self.client,
+                sensor_id=self.shared_state.sensor_id,
+                config=self.shared_state.config,
+                context=None,
+            )
+            self._ref_app_instance.calibrate()
+        except Exception as exc:
+            raise HandledException("Failed to calibrate detector") from exc
+        finally:
+            self.callback(PluginStateMessage(state=PluginState.LOADED_IDLE))
+
+        self.shared_state.context = self._ref_app_instance._detector.context
+        self.broadcast()
+
 
 class PlotPlugin(DetectorPlotPluginBase):
 
-    _VELOCITY_Y_SCALE_MARGIN_M = 0.25
+    STATUS_MSG_MAP = {
+        ProcessorLevelStatus.IN_RANGE: "In range",
+        ProcessorLevelStatus.NO_DETECTION: "Not available",
+        ProcessorLevelStatus.OVERFLOW: "Warning: Overflow",
+        ProcessorLevelStatus.OUT_OF_RANGE: "Out of range",
+    }
 
     def __init__(self, *, plot_layout: pg.GraphicsLayout, app_model: AppModel) -> None:
         super().__init__(plot_layout=plot_layout, app_model=app_model)
 
+        self.counter = 0
+        self.bar_loc = 0
+
     def setup_from_message(self, message: GeneralMessage) -> None:
         assert message.kwargs is not None
         self.setup(**message.kwargs)
 
     def update_from_message(self, message: GeneralMessage) -> None:
-        assert isinstance(message.data, ExampleAppResult)
+        assert isinstance(message.data, RefAppResult)
         self.update(message.data)
 
     def setup(
         self,
-        example_app_config: ExampleAppConfig,
+        config: RefAppConfig,
+        num_curves: int,
     ) -> None:
 
-        self.slow_zone = example_app_config.slow_zone
-        self.history_length_s = 10
-        if example_app_config.frame_rate is None:
-            estimated_frame_rate = (
-                example_app_config.sweep_rate / example_app_config.sweeps_per_frame
-            )
-        else:
-            estimated_frame_rate = example_app_config.frame_rate
-
-        self.history_length_n = int(np.around(self.history_length_s * estimated_frame_rate))
-
-        c0_dashed_pen = et.utils.pg_pen_cycler(0, width=2.5, style="--")
+        self.num_curves = num_curves
+        self.start_m = config.start_m
+        self.end_m = config.end_m
+
+        win = self.plot_layout
+
+        # Sweep plot
+        self.sweep_plot = win.addPlot(row=1, col=0, colspan=3)
+        self.sweep_plot.setMenuEnabled(False)
+        self.sweep_plot.showGrid(x=True, y=True)
+        self.sweep_plot.addLegend()
+        self.sweep_plot.setLabel("left", "Amplitude")
+        self.sweep_plot.setLabel("bottom", "Distance (m)")
+        self.sweep_plot.addItem(pg.PlotDataItem())
+
+        self.vertical_line_start = pg.InfiniteLine(
+            pen=et.utils.pg_pen_cycler(2),
+            label="Tank start",
+            labelOpts={
+                "position": 0.5,
+                "color": (0, 100, 0),
+                "fill": (200, 200, 200, 50),
+                "movable": True,
+            },
+        )
+        self.sweep_plot.addItem(self.vertical_line_start)
+        self.vertical_line_end = pg.InfiniteLine(
+            pen=et.utils.pg_pen_cycler(2),
+            label="Tank end",
+            labelOpts={
+                "position": 0.5,
+                "color": (0, 100, 0),
+                "fill": (200, 200, 200, 50),
+                "movable": True,
+            },
+        )
+        self.sweep_plot.addItem(self.vertical_line_end)
 
-        # Velocity plot
+        pen = et.utils.pg_pen_cycler(0)
+        brush = et.utils.pg_brush_cycler(0)
+        symbol_kw = dict(symbol="o", symbolSize=1, symbolBrush=brush, symbolPen="k")
+        feat_kw = dict(pen=pen, **symbol_kw)
+        self.sweep_curves = [self.sweep_plot.plot(**feat_kw) for _ in range(self.num_curves)]
+
+        pen = et.utils.pg_pen_cycler(1)
+        brush = et.utils.pg_brush_cycler(1)
+        symbol_kw = dict(symbol="o", symbolSize=1, symbolBrush=brush, symbolPen="k")
+        feat_kw = dict(pen=pen, **symbol_kw)
+        self.threshold_curves = [self.sweep_plot.plot(**feat_kw) for _ in range(self.num_curves)]
+
+        sweep_plot_legend = pg.LegendItem(offset=(0.0, 0.5))
+        sweep_plot_legend.setParentItem(self.sweep_plot)
+        sweep_plot_legend.addItem(self.sweep_curves[0], "Sweep")
+        sweep_plot_legend.addItem(self.threshold_curves[0], "Threshold")
+
+        # Level history plot
+        self.level_history_plot = win.addPlot(row=0, col=1, colspan=2)
+        self.level_history_plot.setMenuEnabled(False)
+        self.level_history_plot.showGrid(x=True, y=True)
+        self.level_history_plot.addLegend()
+        self.level_history_plot.setLabel("left", "Estimated level (cm)")
+        self.level_history_plot.setLabel("bottom", "Time (s)")
+        self.level_history_plot.addItem(pg.PlotDataItem())
 
-        self.velocity_history_plot = self._create_plot(self.plot_layout, row=0, col=0)
-        self.velocity_history_plot.setTitle("Estimated velocity")
-        self.velocity_history_plot.setLabel(axis="left", text="Velocity", units="m/s")
-        self.velocity_history_plot.setLabel(axis="bottom", text="Time", units="s")
-        self.velocity_history_plot.addLegend(labelTextSize="10pt")
-        self.velocity_smooth_limits = et.utils.SmoothLimits()
+        pen = et.utils.pg_pen_cycler(0)
+        brush = et.utils.pg_brush_cycler(0)
+        symbol_kw = dict(symbol="o", symbolSize=5, symbolBrush=brush, symbolPen="k")
+        feat_kw = dict(pen=pen, **symbol_kw)
+        self.level_history_curve = self.level_history_plot.plot(**feat_kw)
+
+        self.sweep_smooth_max = et.utils.SmoothMax()
+        self.distance_hist_smooth_lim = et.utils.SmoothLimits()
+
+        # Rect plot
+        self.num_rects = 15
+        self.rect_plot = pg.PlotItem()
+        self.rect_plot.setAspectLocked()
+        self.rect_plot.hideAxis("left")
+        self.rect_plot.hideAxis("bottom")
+        self.rects = []
+
+        pen = pg.mkPen(None)
+        rect_width = self.num_rects / 2.0
+        for r in np.arange(self.num_rects) + 1:
+            rect = pg.QtWidgets.QGraphicsRectItem(0, r, rect_width, 1)
+            rect.setPen(pen)
+            self.rect_plot.addItem(rect)
+            self.rects.append(rect)
 
-        self.velocity_curve = self.velocity_history_plot.plot(
-            pen=et.utils.pg_pen_cycler(0), name="Estimated velocity"
-        )
+        self.plot_layout.addItem(self.rect_plot, row=0, col=0)
 
-        self.psd_html = (
+        # text items
+        self.level_html_format = (
             '<div style="text-align: center">'
-            '<span style="color: #FFFFFF;font-size:13pt;">'
+            '<span style="color: #FFFFFF;font-size:12pt;">'
             "{}</span></div>"
         )
 
-        self.distance_text_item = pg.TextItem(
-            html=self.psd_html,
+        self.level_text_item = pg.TextItem(
             fill=pg.mkColor(0x1F, 0x77, 0xB4, 180),
             anchor=(0.5, 0),
         )
 
-        self.velocity_history_plot.addItem(self.distance_text_item)
-
-        self.velocity_history = np.zeros(self.history_length_n)
-
-        self.lower_std_history = np.zeros(self.history_length_n)
-        self.upper_std_history = np.zeros(self.history_length_n)
+        self.rect_plot.addItem(self.level_text_item)
+        self.level_text_item.hide()
 
-        self.lower_std_curve = self.velocity_history_plot.plot()
-        self.upper_std_curve = self.velocity_history_plot.plot()
-
-        fbi = pg.FillBetweenItem(
-            self.lower_std_curve,
-            self.upper_std_curve,
-            brush=pg.mkBrush(f"{et.utils.color_cycler(0)}50"),
-        )
-
-        self.velocity_history_plot.addItem(fbi)
-
-        # PSD plot
-
-        self.psd_plot = self._create_plot(self.plot_layout, row=1, col=0)
-        self.psd_plot.setTitle("PSD<br>(colored area represents the slow zone)")
-        self.psd_plot.setLabel(axis="left", text="Power")
-        self.psd_plot.setLabel(axis="bottom", text="Velocity", units="m/s")
-        self.psd_plot.addLegend(labelTextSize="10pt")
-
-        self.psd_smooth_max = et.utils.SmoothMax(tau_grow=0.5, tau_decay=2.0)
-        self.psd_curve = self.psd_plot.plot(pen=et.utils.pg_pen_cycler(0), name="PSD")
-        self.psd_threshold = self.psd_plot.plot(pen=c0_dashed_pen, name="Threshold")
-
-        psd_slow_zone_color = et.utils.color_cycler(0)
-        psd_slow_zone_color = f"{psd_slow_zone_color}50"
-        psd_slow_zone_brush = pg.mkBrush(psd_slow_zone_color)
-
-        self.psd_slow_zone = pg.LinearRegionItem(brush=psd_slow_zone_brush, movable=False)
-        self.psd_plot.addItem(self.psd_slow_zone)
-
-        brush = et.utils.pg_brush_cycler(0)
-        self.psd_peak_plot_item = pg.PlotDataItem(
-            pen=None, symbol="o", symbolSize=8, symbolBrush=brush, symbolPen="k"
-        )
-        self.psd_plot.addItem(self.psd_peak_plot_item)
-
-        self.psd_plot.setLogMode(x=False, y=True)
-
-    def update(self, example_app_result: ExampleAppResult) -> None:
-        processor_extra_result = example_app_result.processor_extra_result
-
-        lim = self.velocity_smooth_limits.update(example_app_result.velocity)
-
-        self.velocity_history_plot.setYRange(
-            lim[0] - self._VELOCITY_Y_SCALE_MARGIN_M, lim[1] + self._VELOCITY_Y_SCALE_MARGIN_M
-        )
-        self.velocity_history_plot.setXRange(-self.history_length_s, 0)
-
-        xs = np.linspace(-self.history_length_s, 0, self.history_length_n)
+    def update(
+        self,
+        result: RefAppResult,
+    ) -> None:
+        # Get the first element as the plugin only supports single sensor operation.
+        (detector_result,) = list(result.extra_result.detector_result.values())
+        assert detector_result.distances is not None
+
+        time_and_level_dict = (
+            result.extra_result.processor_extra_result.level_and_time_for_plotting
+        )
+
+        # update sweep plot
+        max_val_in_plot = 0
+        for idx, processor_result in enumerate(detector_result.processor_results):
+            assert processor_result.extra_result.used_threshold is not None
+            assert processor_result.extra_result.distances_m is not None
+            assert processor_result.extra_result.abs_sweep is not None
 
-        self.velocity_history = np.roll(self.velocity_history, -1)
-        self.velocity_history[-1] = example_app_result.velocity
-        self.velocity_curve.setData(xs, self.velocity_history)
+            self.sweep_curves[idx].setData(
+                processor_result.extra_result.distances_m, processor_result.extra_result.abs_sweep
+            )
 
-        velocity_html = self.psd_html.format(
-            f"Distance {np.around(example_app_result.distance_m, 2)} m"
-        )
-        self.distance_text_item.setHtml(velocity_html)
-        self.distance_text_item.setPos(
-            -self.history_length_s / 2, lim[1] + self._VELOCITY_Y_SCALE_MARGIN_M
-        )
+            self.threshold_curves[idx].setData(
+                processor_result.extra_result.distances_m,
+                processor_result.extra_result.used_threshold,
+            )
 
-        self.lower_std_history = np.roll(self.lower_std_history, -1)
-        self.lower_std_history[-1] = (
-            example_app_result.velocity + 0.5 * processor_extra_result.peak_width
-        )
-        self.lower_std_curve.setData(xs, self.lower_std_history)
+            max_val_in_subsweep = max(
+                max(processor_result.extra_result.used_threshold),
+                max(processor_result.extra_result.abs_sweep),
+            )
 
-        self.upper_std_history = np.roll(self.upper_std_history, -1)
-        self.upper_std_history[-1] = (
-            example_app_result.velocity - 0.5 * processor_extra_result.peak_width
-        )
-        self.upper_std_curve.setData(xs, self.upper_std_history)
+            max_val_in_plot = max(max_val_in_plot, max_val_in_subsweep)
 
-        lim = self.psd_smooth_max.update(processor_extra_result.psd_threshold)
-        self.psd_plot.setYRange(np.log10(0.2), np.log10(lim))
-        self.psd_plot.setXRange(
-            processor_extra_result.max_bin_vertical_vs[0],
-            processor_extra_result.max_bin_vertical_vs[-1],
-        )
-        self.psd_curve.setData(
-            processor_extra_result.vertical_velocities, processor_extra_result.psd
-        )
-        self.psd_threshold.setData(
-            processor_extra_result.vertical_velocities, processor_extra_result.psd_threshold
-        )
-        if processor_extra_result.peak_idx is not None:
-            self.psd_peak_plot_item.setData(
-                [processor_extra_result.vertical_velocities[processor_extra_result.peak_idx]],
-                [processor_extra_result.psd[processor_extra_result.peak_idx]],
+        self.sweep_plot.setYRange(0, self.sweep_smooth_max.update(max_val_in_plot))
+        self.vertical_line_start.setValue(self.start_m)
+        self.vertical_line_end.setValue(self.end_m)
+        self.vertical_line_start.show()
+        self.vertical_line_end.show()
+
+        # update level history plot
+        if any(~np.isnan(time_and_level_dict["level"])):
+            self.level_history_curve.setData(
+                time_and_level_dict["time"], time_and_level_dict["level"] * 100
             )
-        else:
-            self.psd_peak_plot_item.clear()
-
-        middle_idx = int(np.around(processor_extra_result.vertical_velocities.shape[0] / 2))
-        self.psd_slow_zone.setRegion(
-            [
-                processor_extra_result.vertical_velocities[middle_idx - self.slow_zone],
-                processor_extra_result.vertical_velocities[middle_idx + self.slow_zone],
-            ]
-        )
-
-    @staticmethod
-    def _create_plot(parent: pg.GraphicsLayout, row: int, col: int) -> pg.PlotItem:
-        velocity_history_plot = parent.addPlot(row=row, col=col)
-        velocity_history_plot.setMenuEnabled(False)
-        velocity_history_plot.setMouseEnabled(x=False, y=False)
-        velocity_history_plot.hideButtons()
-        velocity_history_plot.showGrid(x=True, y=True, alpha=0.5)
+            self.level_history_plot.setXRange(-TIME_HISTORY_S + 1, 0)
+            self.level_history_plot.setYRange(0, (self.end_m - self.start_m + 0.01) * 100)
 
-        return velocity_history_plot
+        # update level plot
+        if (
+            result.level is not None
+            and result.peak_detected is not None
+            and result.peak_status is not None
+        ):
+            current_level = result.level
+            peak_detected = result.peak_detected
+            peak_status = result.peak_status
+
+            # Show the percentage level plot if the plot width is greater than 600 pixels,
+            # otherwise display the level as text.
+            if self.plot_layout.width() >= 600:
+                level_text = self.STATUS_MSG_MAP[peak_status]
+                if peak_status == ProcessorLevelStatus.OVERFLOW:
+                    for rect in self.rects:
+                        rect.setBrush(et.utils.pg_brush_cycler(0))
+                elif peak_detected and (peak_status == ProcessorLevelStatus.IN_RANGE):
+                    self.bar_loc = round(
+                        current_level / (self.end_m - self.start_m) * self.num_rects
+                    )
+                    for rect in self.rects[: self.bar_loc]:
+                        rect.setBrush(et.utils.pg_brush_cycler(0))
+
+                    for rect in self.rects[self.bar_loc :]:
+                        rect.setBrush(et.utils.pg_brush_cycler(1))
+
+                    level_text = "Level: {:.1f} cm, {:.0f} %".format(
+                        current_level * 100,
+                        current_level / (self.end_m - self.start_m) * 100,
+                    )
+                    self.counter = 0
+                elif peak_detected and (peak_status == ProcessorLevelStatus.OUT_OF_RANGE):
+                    for rect in self.rects:
+                        rect.setBrush(et.utils.pg_brush_cycler(1))
+                elif ~peak_detected and (self.counter <= NO_DETECTION_TIMEOUT):
+                    for rect in self.rects[: self.bar_loc]:
+                        rect.setBrush(et.utils.pg_brush_cycler(0))
+
+                    for rect in self.rects[self.bar_loc :]:
+                        rect.setBrush(et.utils.pg_brush_cycler(1))
+
+                    self.counter += 1
+                else:
+                    for rect in self.rects:
+                        rect.setBrush(et.utils.pg_brush_cycler(1))
+                        self.bar_loc = 0
+                for rect in self.rects:
+                    rect.setVisible(True)
+
+                level_html = self.level_html_format.format(level_text)
+                self.level_text_item.setHtml(level_html)
+                self.level_text_item.setPos(self.num_rects / 4.0, self.num_rects + 4.0)
+                self.level_text_item.show()
+            else:
+                level_text = self.STATUS_MSG_MAP[peak_status]
+                if peak_detected and (peak_status == ProcessorLevelStatus.IN_RANGE):
+                    level_text = "Level: {:.1f} cm, {:.0f} %".format(
+                        current_level * 100,
+                        current_level / (self.end_m - self.start_m) * 100,
+                    )
+                    self.counter = 0
+                level_html = self.level_html_format.format(level_text)
+                self.level_text_item.setHtml(level_html)
+                self.level_text_item.setPos(self.num_rects / 4.0, self.num_rects + 4.0)
+                self.level_text_item.show()
+                for rect in self.rects:
+                    rect.setVisible(False)
 
 
 class ViewPlugin(DetectorViewPluginBase):
+
+    TEXT_MSG_MAP = {
+        DetailedStatus.OK: "Ready to start.",
+        DetailedStatus.CONTEXT_MISSING: "Run detector calibration.",
+        DetailedStatus.CALIBRATION_MISSING: "Run detector calibration.",
+        DetailedStatus.CONFIG_MISMATCH: (
+            "Current configuration does not match the configuration "
+            + "used during detector calibration. Run detector calibration."
+        ),
+    }
+
     def __init__(self, app_model: AppModel, view_widget: QWidget) -> None:
         super().__init__(app_model=app_model, view_widget=view_widget)
+        self.app_model = app_model
         self._log = logging.getLogger(__name__)
 
         sticky_layout = QVBoxLayout()
         sticky_layout.setContentsMargins(0, 0, 0, 0)
         scrolly_layout = QVBoxLayout()
         scrolly_layout.setContentsMargins(0, 0, 0, 0)
 
@@ -341,234 +505,263 @@
         self.start_button.clicked.connect(self._send_start_request)
 
         self.stop_button = QPushButton(icons.STOP(), "Stop")
         self.stop_button.setShortcut("space")
         self.stop_button.setToolTip("Stops the session.\n\nShortcut: Space")
         self.stop_button.clicked.connect(self._send_stop_request)
 
+        self.calibrate_detector_button = QPushButton(icons.CALIBRATE(), "Calibrate detector")
+        self.calibrate_detector_button.clicked.connect(self._on_calibrate_detector)
+
+        self.defaults_button = QPushButton(icons.RESTORE(), "Reset settings and calibrations")
+        self.defaults_button.clicked.connect(self._send_defaults_request)
+
+        self.message_box = QLabel(self.sticky_widget)
+        self.message_box.setWordWrap(True)
+
         button_group = GroupBox.grid("Controls", parent=self.sticky_widget)
         button_group.layout().addWidget(self.start_button, 0, 0)
         button_group.layout().addWidget(self.stop_button, 0, 1)
+        button_group.layout().addWidget(self.calibrate_detector_button, 1, 0, 1, -1)
+        button_group.layout().addWidget(self.defaults_button, 3, 0, 1, -1)
+        button_group.layout().addWidget(self.message_box, 4, 0, 1, -1)
 
         sticky_layout.addWidget(button_group)
 
-        self.misc_error_view = MiscErrorView(self.scrolly_widget)
-        scrolly_layout.addWidget(self.misc_error_view)
-
         sensor_selection_group = GroupBox.vertical("Sensor selection", parent=self.scrolly_widget)
         self.sensor_id_pidget = pidgets.SensorIdPidgetFactory(items=[]).create(
             parent=sensor_selection_group
         )
         self.sensor_id_pidget.sig_update.connect(self._on_sensor_id_update)
         sensor_selection_group.layout().addWidget(self.sensor_id_pidget)
         scrolly_layout.addWidget(sensor_selection_group)
 
-        self.range_helper = RangeHelpView()
-        scrolly_layout.addWidget(self.range_helper)
+        self.tank_level_config_editor = AttrsConfigEditor(
+            title="Tank level indicator parameters",
+            factory_mapping=self._get_processor_pidget_mapping(),
+            config_type=RefAppConfig,
+            extra_presenter=_set_config_presenter,
+            parent=self.scrolly_widget,
+        )
+        self.tank_level_config_editor.sig_update.connect(self._on_config_update)
+        scrolly_layout.addWidget(self.tank_level_config_editor)
 
         self.config_editor = AttrsConfigEditor(
-            title="Example app parameters",
-            factory_mapping=self._get_pidget_mapping(),
-            config_type=ExampleAppConfig,
+            title="Detector parameters",
+            factory_mapping=self._get_detector_pidget_mapping(),
+            config_type=RefAppConfig,
+            save_load_buttons=False,
             parent=self.scrolly_widget,
         )
         self.config_editor.sig_update.connect(self._on_config_update)
         scrolly_layout.addWidget(self.config_editor)
 
         self.sticky_widget.setLayout(sticky_layout)
         self.scrolly_widget.setLayout(scrolly_layout)
 
     @classmethod
-    def _get_pidget_mapping(cls) -> PidgetFactoryMapping:
+    def _get_processor_pidget_mapping(cls) -> PidgetFactoryMapping:
         return {
-            "surface_distance": pidgets.FloatPidgetFactory(
-                name_label_text="Surface distance",
-                suffix=" m",
-                decimals=2,
-                limits=(0.1, 3),
-            ),
-            "sensor_angle": pidgets.FloatPidgetFactory(
-                name_label_text="Sensor angle",
-                suffix=" degrees",
-                decimals=1,
-                limits=(0, 89),
-            ),
-            "num_points": pidgets.IntPidgetFactory(
-                name_label_text="Number of distance points",
-                limits=(1, None),
-            ),
-            "sweep_rate": pidgets.FloatPidgetFactory(
-                name_label_text="Sweep rate",
-                suffix=" Hz",
-                decimals=1,
-                limits=(100, None),
-            ),
-            "sweeps_per_frame": pidgets.IntPidgetFactory(
-                name_label_text="Sweeps per frame",
-                limits=(64, 2048),
-            ),
-            "hwaas": pidgets.IntPidgetFactory(
-                name_label_text="HWAAS",
-                limits=(1, 511),
-            ),
-            "profile": pidgets.OptionalEnumPidgetFactory(
-                name_label_text="Profile",
-                checkbox_label_text="Override",
-                enum_type=a121.Profile,
-                label_mapping={
-                    a121.Profile.PROFILE_1: "1 (shortest)",
-                    a121.Profile.PROFILE_2: "2",
-                    a121.Profile.PROFILE_3: "3",
-                    a121.Profile.PROFILE_4: "4",
-                    a121.Profile.PROFILE_5: "5 (longest)",
-                },
-            ),
-            "step_length": pidgets.IntPidgetFactory(
-                name_label_text="Step length:",
-                limits=(1, None),
-            ),
-            "frame_rate": pidgets.OptionalFloatPidgetFactory(
-                name_label_text="Frame rate",
-                checkbox_label_text="Limit",
-                suffix=" Hz",
-                decimals=1,
-                limits=(1, None),
-                init_set_value=10,
-            ),
-            "continuous_sweep_mode": pidgets.CheckboxPidgetFactory(
-                name_label_text="Continuos sweep mode",
-            ),
-            "double_buffering": pidgets.CheckboxPidgetFactory(
-                name_label_text="Double buffering",
-            ),
-            "inter_frame_idle_state": pidgets.EnumPidgetFactory(
-                enum_type=a121.IdleState,
-                name_label_text="Inter frame idle state",
-                label_mapping={
-                    a121.IdleState.DEEP_SLEEP: "Deep sleep",
-                    a121.IdleState.SLEEP: "Sleep",
-                    a121.IdleState.READY: "Ready",
-                },
-            ),
-            "inter_sweep_idle_state": pidgets.EnumPidgetFactory(
-                enum_type=a121.IdleState,
-                name_label_text="Inter sweep idle state",
-                label_mapping={
-                    a121.IdleState.DEEP_SLEEP: "Deep sleep",
-                    a121.IdleState.SLEEP: "Sleep",
-                    a121.IdleState.READY: "Ready",
-                },
-            ),
-            "time_series_length": pidgets.IntPidgetFactory(
-                name_label_text="Time series length",
-                limits=(64, None),
+            "median_filter_length": pidgets.IntPidgetFactory(
+                name_label_text="Median filter length",
+                limits=(1, 10),
+            ),
+            "num_medians_to_average": pidgets.IntPidgetFactory(
+                name_label_text="Num measurements averaged",
+                limits=(1, 10),
             ),
-            "psd_lp_coeff": pidgets.FloatSliderPidgetFactory(
-                name_label_text="PSD time filtering coeff.",
-                limits=(0, 1),
+            "start_m": pidgets.FloatPidgetFactory(
+                name_label_text="Tank start",
+                suffix=" m",
                 decimals=3,
+                limits=(0.03, 20),
             ),
-            "slow_zone": pidgets.IntPidgetFactory(
-                name_label_text="Slow zone half length",
-                limits=(0, 20),
-            ),
-            "velocity_lp_coeff": pidgets.FloatSliderPidgetFactory(
-                name_label_text="Velocity time filtering coeff.\nper time series",
-                limits=(0, 1),
+            "end_m": pidgets.FloatPidgetFactory(
+                name_label_text="Tank end",
+                suffix=" m",
                 decimals=3,
+                limits=(0.05, 20),
             ),
-            "cfar_win": pidgets.IntPidgetFactory(
-                name_label_text="CFAR window length",
-                limits=(0, 20),
-            ),
-            "cfar_guard": pidgets.IntPidgetFactory(
-                name_label_text="CFAR guard length",
-                limits=(0, 20),
-            ),
-            "cfar_sensitivity": pidgets.FloatSliderPidgetFactory(
-                name_label_text="Threshold sensitivity",
-                decimals=2,
-                limits=(0.01, 1),
-            ),
-            "max_peak_interval_s": pidgets.FloatPidgetFactory(
-                name_label_text="Max peak interval",
-                decimals=1,
-                limits=(0, 20),
-                suffix=" s",
+        }
+
+    @classmethod
+    def _get_detector_pidget_mapping(cls) -> PidgetFactoryMapping:
+        COMMON_PIDGETS = {
+            "max_profile",
+            "reflector_shape",
+            "peaksorting_method",
+            "threshold_method",
+            "fixed_threshold_value",
+            "num_frames_in_recorded_threshold",
+            "threshold_sensitivity",
+            "signal_quality",
+        }
+
+        return {
+            "max_step_length": pidgets.OptionalIntPidgetFactory(
+                name_label_text="Max step length",
+                checkbox_label_text="Set",
+                limits=(1, None),
+                init_set_value=1,
             ),
+            **{
+                aspect: factory
+                for aspect, factory in DistanceViewPlugin.get_pidget_mapping().items()
+                if aspect in COMMON_PIDGETS
+            },
         }
 
     def on_backend_state_update(self, backend_plugin_state: Optional[SharedState]) -> None:
         if backend_plugin_state is not None and backend_plugin_state.config is not None:
-            results = backend_plugin_state.config._collect_validation_results()
+            self.config_editor.set_data(backend_plugin_state.config)
+            self.tank_level_config_editor.set_data(backend_plugin_state.config)
 
-            not_handled = self.config_editor.handle_validation_results(results)
+            results = backend_plugin_state.config._collect_validation_results()
 
-            not_handled = self.misc_error_view.handle_validation_results(not_handled)
+            not_handled = self.tank_level_config_editor.handle_validation_results(results)
+            not_handled = self.config_editor.handle_validation_results(not_handled)
 
             assert not_handled == []
-
-            self.range_helper.update(
-                ExampleApp._get_sensor_config(backend_plugin_state.config).subsweep
-            )
+        else:
+            self.config_editor.set_data(None)
+            self.tank_level_config_editor.set_data(None)
 
     def on_app_model_update(self, app_model: AppModel) -> None:
         state = app_model.backend_plugin_state
 
         if state is None:
             self.start_button.setEnabled(False)
+            self.calibrate_detector_button.setEnabled(False)
             self.stop_button.setEnabled(False)
+            self.defaults_button.setEnabled(False)
 
-            self.config_editor.set_data(None)
             self.config_editor.setEnabled(False)
+            self.tank_level_config_editor.setEnabled(False)
             self.sensor_id_pidget.set_selected_sensor(None, [])
+            self.message_box.setText("")
 
             return
 
         assert isinstance(state, SharedState)
 
+        self.defaults_button.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
+
+        self.tank_level_config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
         self.config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
-        self.config_editor.set_data(state.config)
+
         self.sensor_id_pidget.set_selected_sensor(state.sensor_id, app_model.connected_sensors)
         self.sensor_id_pidget.setEnabled(app_model.plugin_state.is_steady)
 
+        detector_status = Detector.get_detector_status(
+            state.config.to_detector_config(), state.context, [state.sensor_id]
+        )
+
+        self.message_box.setText(self.TEXT_MSG_MAP[detector_status.detector_state])
+
+        app_model_ready = app_model.is_ready_for_session()
+        try:
+            state.config.validate()
+        except a121.ValidationError:
+            config_valid = False
+        else:
+            config_valid = True
+
+        self.calibrate_detector_button.setEnabled(
+            app_model_ready
+            and config_valid
+            and self.config_editor.is_ready
+            and self.tank_level_config_editor.is_ready
+        )
         self.start_button.setEnabled(
-            app_model.is_ready_for_session() and self.config_editor.is_ready
+            detector_status.ready_to_start
+            and app_model_ready
+            and config_valid
+            and self.config_editor.is_ready
+            and self.tank_level_config_editor.is_ready
         )
         self.stop_button.setEnabled(app_model.plugin_state == PluginState.LOADED_BUSY)
 
-    def _on_config_update(self, config: ExampleAppConfig) -> None:
+    def _on_sensor_id_update(self, sensor_id: int) -> None:
+        BackendPlugin.update_sensor_id.rpc(self.app_model.put_task, sensor_id=sensor_id)
+
+    def _on_config_update(self, config: RefAppConfig) -> None:
         BackendPlugin.update_config.rpc(self.app_model.put_task, config=config)
 
+    # TODO: move to detector base (?)
+    def _send_start_request(self) -> None:
+        BackendPlugin.start_session.rpc(
+            self.app_model.put_task, with_recorder=self.app_model.recording_enabled
+        )
+
+    # TODO: move to detector base (?)
+    def _send_stop_request(self) -> None:
+        BackendPlugin.stop_session.rpc(self.app_model.put_task)
+
+    def _on_calibrate_detector(self) -> None:
+        BackendPlugin.calibrate_detector.rpc(self.app_model.put_task)
+
     def _send_defaults_request(self) -> None:
         BackendPlugin.restore_defaults.rpc(self.app_model.put_task)
 
-    def _on_sensor_id_update(self, sensor_id: int) -> None:
-        BackendPlugin.update_sensor_id.rpc(self.app_model.put_task, sensor_id=sensor_id)
+
+def _set_config_presenter(instance: Any, presentation_type: PresentationType) -> Optional[str]:
+    if isinstance(instance, RefAppConfig) and presentation_type is PresentationType.C_SET_CONFIG:
+        config: RefAppConfig = instance
+        distance_config = config.to_detector_config()
+
+        return f"""
+static void set_config(acc_ref_app_tank_level_config_t *config, tank_level_preset_config_t preset)
+{{
+    // This snippet is generated to be compatible with RSS A121 v1.0.0
+    // If there is a version missmatch the snippet might need some modification
+
+    (void)preset;
+
+    config->tank_range_start_m     = {config.start_m:.3f}f;
+    config->tank_range_end_m       = {config.end_m:.3f}f;
+    config->median_filter_length   = {config.median_filter_length}U;
+    config->num_medians_to_average = {config.num_medians_to_average}U;
+
+    acc_detector_distance_config_start_set(config->distance_config, {distance_config.start_m:.3f}f);
+    acc_detector_distance_config_end_set(config->distance_config, {distance_config.end_m:.3f}f);
+    acc_detector_distance_config_max_step_length_set(config->distance_config, {distance_config.max_step_length or 0}U);
+    acc_detector_distance_config_max_profile_set(config->distance_config, ACC_CONFIG_{distance_config.max_profile.name});
+    acc_detector_distance_config_num_frames_recorded_threshold_set(config->distance_config, {distance_config.num_frames_in_recorded_threshold}U);
+    acc_detector_distance_config_peak_sorting_set(config->distance_config, ACC_DETECTOR_DISTANCE_PEAK_SORTING_{distance_config.peaksorting_method.name});
+    acc_detector_distance_config_reflector_shape_set(config->distance_config, ACC_DETECTOR_DISTANCE_REFLECTOR_SHAPE_{distance_config.reflector_shape.name});
+    acc_detector_distance_config_threshold_sensitivity_set(config->distance_config, {distance_config.threshold_sensitivity:.3f}f);
+    acc_detector_distance_config_signal_quality_set(config->distance_config, {distance_config.signal_quality:.3f}f);
+    acc_detector_distance_config_close_range_leakage_cancellation_set(config->distance_config, {str(distance_config.close_range_leakage_cancellation).lower()});
+}}
+"""
+
+    return None
 
 
 class PluginSpec(PluginSpecBase):
     def create_backend_plugin(
         self, callback: Callable[[Message], None], key: str
     ) -> BackendPlugin:
-        return BackendPlugin(callback=callback, generation=self.generation, key=key)
+        return BackendPlugin(callback, generation=self.generation, key=key)
 
     def create_view_plugin(self, app_model: AppModel, view_widget: QWidget) -> ViewPlugin:
         return ViewPlugin(app_model=app_model, view_widget=view_widget)
 
     def create_plot_plugin(
         self, app_model: AppModel, plot_layout: pg.GraphicsLayout
     ) -> PlotPlugin:
         return PlotPlugin(app_model=app_model, plot_layout=plot_layout)
 
 
-SURFACE_VELOCITY_PLUGIN = PluginSpec(
+TANK_LEVEL_PLUGIN = PluginSpec(
     generation=PluginGeneration.A121,
-    key="surface_velocity",
-    title="Surface velocity",
-    description="Estimate surface speed and direction of streaming water.",
-    family=PluginFamily.EXAMPLE_APP,
+    key="tank_level",
+    title="Tank level",
+    description="Measure liquid levels in tanks",
+    family=PluginFamily.REF_APP,
     presets=[
-        PluginPresetBase(name="Default", preset_id=PluginPresetId.DEFAULT),
+        PluginPresetBase(name="Small", preset_id=PluginPresetId.SMALL),
+        PluginPresetBase(name="Medium", preset_id=PluginPresetId.MEDIUM),
+        PluginPresetBase(name="Large", preset_id=PluginPresetId.LARGE),
     ],
-    default_preset_id=PluginPresetId.DEFAULT,
+    default_preset_id=PluginPresetId.SMALL,
 )
```

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/_configs.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/tank_level/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/_plugin.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,125 +1,137 @@
 # Copyright (c) Acconeer AB, 2023
 # All rights reserved
 
 from __future__ import annotations
 
 import logging
 from enum import Enum, auto
-from typing import Any, Callable, Mapping, Optional
+from typing import Callable, List, Mapping, Optional, Tuple
 
 import attrs
 import h5py
 import numpy as np
+import numpy.typing as npt
 
-from PySide6.QtWidgets import QLabel, QPushButton, QVBoxLayout, QWidget
+from PySide6 import QtCore
+from PySide6.QtWidgets import QPushButton, QVBoxLayout, QWidget
 
 import pyqtgraph as pg
 
 import acconeer.exptool as et
 from acconeer.exptool import a121
 from acconeer.exptool.a121._h5_utils import _create_h5_string_dataset
+from acconeer.exptool.a121.algo._base import AlgoBase
 from acconeer.exptool.a121.algo._plugins import (
     DetectorBackendPluginBase,
     DetectorPlotPluginBase,
     DetectorViewPluginBase,
 )
-from acconeer.exptool.a121.algo.distance._detector import DetailedStatus, Detector
-from acconeer.exptool.a121.algo.distance._detector_plugin import ViewPlugin as DistanceViewPlugin
-from acconeer.exptool.a121.algo.tank_level._configs import (
-    get_large_config,
-    get_medium_config,
-    get_small_config,
-)
-from acconeer.exptool.a121.algo.tank_level._processor import ProcessorLevelStatus
-from acconeer.exptool.a121.algo.tank_level._ref_app import (
-    RefApp,
-    RefAppConfig,
-    RefAppContext,
-    RefAppResult,
-    _load_algo_data,
-)
+from acconeer.exptool.a121.algo.presence._detector import Detector
+from acconeer.exptool.a121.algo.presence._detector_plugin import ViewPlugin as PresenceViewPlugin
 from acconeer.exptool.app.new import (
     AppModel,
+    AttrsConfigEditor,
     BackendLogger,
     GeneralMessage,
     GroupBox,
-    HandledException,
     Message,
+    MiscErrorView,
+    PidgetGroupFactoryMapping,
     PluginFamily,
     PluginGeneration,
     PluginPresetBase,
     PluginSpecBase,
     PluginState,
-    PluginStateMessage,
     icons,
     is_task,
-)
-from acconeer.exptool.app.new.ui.plugin_components import (
-    AttrsConfigEditor,
-    PidgetFactoryMapping,
-    PresentationType,
     pidgets,
 )
 
+from ._configs import (
+    get_ceiling_config,
+    get_long_range_config,
+    get_low_power_config,
+    get_medium_range_config,
+    get_short_range_config,
+)
+from ._ref_app import (
+    PresenceWakeUpConfig,
+    PresenceZoneConfig,
+    RefApp,
+    RefAppConfig,
+    RefAppContext,
+    RefAppResult,
+    _load_algo_data,
+    _Mode,
+)
+
 
-NO_DETECTION_TIMEOUT = 50
-TIME_HISTORY_S = 30
+@attrs.mutable(kw_only=True)
+class PlotConfig(AlgoBase):
+    show_all_detected_zones: bool = attrs.field(default=False)
 
 
 @attrs.mutable(kw_only=True)
 class SharedState:
     sensor_id: int = attrs.field(default=1)
     config: RefAppConfig = attrs.field(factory=RefAppConfig)
-    context: RefAppContext = attrs.field(factory=RefAppContext)
+    plot_config: PlotConfig = attrs.field(factory=PlotConfig)
+    ref_app_context: Optional[RefAppContext] = attrs.field(default=None)
 
 
 class PluginPresetId(Enum):
-    SMALL = auto()
-    MEDIUM = auto()
-    LARGE = auto()
-
-
-@attrs.mutable(kw_only=True)
-class TankLevelPreset:
-    config: RefAppConfig = attrs.field()
+    SHORT_RANGE = auto()
+    MEDIUM_RANGE = auto()
+    LONG_RANGE = auto()
+    CEILING = auto()
+    LOW_POWER = auto()
 
 
 class BackendPlugin(DetectorBackendPluginBase[SharedState]):
 
-    PLUGIN_PRESETS: Mapping[int, TankLevelPreset] = {
-        PluginPresetId.SMALL.value: TankLevelPreset(
-            config=get_small_config(),
-        ),
-        PluginPresetId.MEDIUM.value: TankLevelPreset(
-            config=get_medium_config(),
-        ),
-        PluginPresetId.LARGE.value: TankLevelPreset(
-            config=get_large_config(),
-        ),
+    PLUGIN_PRESETS: Mapping[int, Callable[[], RefAppConfig]] = {
+        PluginPresetId.SHORT_RANGE.value: lambda: get_short_range_config(),
+        PluginPresetId.MEDIUM_RANGE.value: lambda: get_medium_range_config(),
+        PluginPresetId.LONG_RANGE.value: lambda: get_long_range_config(),
+        PluginPresetId.CEILING.value: lambda: get_ceiling_config(),
+        PluginPresetId.LOW_POWER.value: lambda: get_low_power_config(),
     }
 
     def __init__(
         self, callback: Callable[[Message], None], generation: PluginGeneration, key: str
     ) -> None:
         super().__init__(callback=callback, generation=generation, key=key)
 
-        self._recorder = None
+        self._recorder: Optional[a121.H5Recorder] = None
         self._ref_app_instance: Optional[RefApp] = None
         self._log = BackendLogger.getLogger(__name__)
 
         self.restore_defaults()
 
     def _load_from_cache(self, file: h5py.File) -> None:
         self.shared_state.config = RefAppConfig.from_json(file["config"][()])
-        self.shared_state.context = RefAppContext.from_h5(file["context"])
+        self.shared_state.plot_config = PlotConfig.from_json(file["plot_config"][()])
+
+        show_all_detected_zones = self.shared_state.plot_config.show_all_detected_zones
+        self.shared_state.config.show_all_detected_zones = show_all_detected_zones
 
     @is_task
     def restore_defaults(self) -> None:
-        self.shared_state = SharedState(config=get_small_config())
+        self.shared_state = SharedState()
+        self.broadcast()
+
+    @is_task
+    def update_sensor_id(self, *, sensor_id: int) -> None:
+        self.shared_state.sensor_id = sensor_id
+        self.broadcast()
+
+    @is_task
+    def update_plot_config(self, *, config: PlotConfig) -> None:
+        self.shared_state.plot_config = config
         self.broadcast()
 
     def _sync_sensor_ids(self) -> None:
         if self.client is not None:
             sensor_ids = self.client.server_info.connected_sensors
 
             if len(sensor_ids) > 0 and self.shared_state.sensor_id not in sensor_ids:
@@ -127,375 +139,475 @@
 
     @is_task
     def update_config(self, *, config: RefAppConfig) -> None:
         self.shared_state.config = config
         self.broadcast()
 
     @is_task
-    def update_sensor_id(self, *, sensor_id: int) -> None:
-        self.shared_state.sensor_id = sensor_id
+    def update_nominal_config(self, *, config: PresenceZoneConfig) -> None:
+        self.shared_state.config.nominal_config = config
         self.broadcast()
 
     @is_task
-    def set_preset(self, preset_id: int) -> None:
-        preset_config = self.PLUGIN_PRESETS[preset_id]
-        self.shared_state.config = preset_config.config
+    def update_wake_up_config(self, *, config: PresenceWakeUpConfig) -> None:
+        self.shared_state.config.wake_up_config = config
         self.broadcast()
 
     def save_to_cache(self, file: h5py.File) -> None:
         _create_h5_string_dataset(file, "config", self.shared_state.config.to_json())
-        context_group = file.create_group("context")
-        self.shared_state.context.to_h5(context_group)
+        _create_h5_string_dataset(file, "plot_config", self.shared_state.plot_config.to_json())
+
+    @is_task
+    def set_preset(self, preset_id: int) -> None:
+        preset_config = self.PLUGIN_PRESETS[preset_id]
+        self.shared_state.config = preset_config()
+        self.shared_state.plot_config = PlotConfig()
+        self.broadcast()
 
     def load_from_record_setup(self, *, record: a121.H5Record) -> None:
         algo_group = record.get_algo_group(self.key)
-        sensor_id, config, context = _load_algo_data(algo_group)
+        _, config, ref_app_context = _load_algo_data(algo_group)
         self.shared_state.config = config
-        self.shared_state.context = context
-        self.shared_state.sensor_id = sensor_id
+        self.shared_state.ref_app_context = ref_app_context
+        self.shared_state.sensor_id = record.session(0).sensor_id
 
     def _start_session(self, recorder: Optional[a121.H5Recorder]) -> None:
         assert self.client
-
         self._ref_app_instance = RefApp(
             client=self.client,
             sensor_id=self.shared_state.sensor_id,
-            config=self.shared_state.config,
-            context=self.shared_state.context,
+            ref_app_config=self.shared_state.config,
+            ref_app_context=self.shared_state.ref_app_context,
         )
 
         self._ref_app_instance.start(recorder)
 
+        nominal_sensor_config = Detector._get_sensor_config(
+            self._ref_app_instance.nominal_detector_config
+        )
+        distances = np.linspace(
+            self.shared_state.config.nominal_config.start_m,
+            self.shared_state.config.nominal_config.end_m,
+            nominal_sensor_config.num_points,
+        )
+        nominal_zone_limits = self._ref_app_instance.ref_app_processor.create_zones(
+            distances, self.shared_state.config.nominal_config.num_zones
+        )
+
+        # self._ref_app_instance.ref_app_processor.zone_limits will always be for
+        # wake_up_config if wake_up_mode is enabled
         self.callback(
             GeneralMessage(
                 name="setup",
-                kwargs={
-                    "config": self.shared_state.config,
-                    "num_curves": len(self._ref_app_instance._detector.processor_specs),
-                },
+                kwargs=dict(
+                    ref_app_config=self.shared_state.config,
+                    plot_config=self.shared_state.plot_config,
+                    estimated_frame_rate=self._ref_app_instance.detector.estimated_frame_rate,
+                    nominal_zone_limits=nominal_zone_limits,
+                    wake_up_zone_limits=self._ref_app_instance.ref_app_processor.zone_limits,
+                ),
                 recipient="plot_plugin",
             )
         )
 
     def end_session(self) -> None:
         if self._ref_app_instance is None:
             raise RuntimeError
-
         if self._recorder is not None:
             self._recorder.close()
-
         self._ref_app_instance.stop()
 
     def get_next(self) -> None:
-        assert self.client is not None
+        assert self.client
         if self._ref_app_instance is None:
             raise RuntimeError
         result = self._ref_app_instance.get_next()
 
         self.callback(GeneralMessage(name="plot", data=result, recipient="plot_plugin"))
 
-    @is_task
-    def calibrate_detector(self) -> None:
-        if self._started:
-            raise RuntimeError
-
-        if self.client is None:
-            raise RuntimeError
-
-        if not self.client.connected:
-            raise RuntimeError
-
-        self.callback(PluginStateMessage(state=PluginState.LOADED_BUSY))
-
-        try:
-            self._ref_app_instance = RefApp(
-                client=self.client,
-                sensor_id=self.shared_state.sensor_id,
-                config=self.shared_state.config,
-                context=None,
-            )
-            self._ref_app_instance.calibrate()
-        except Exception as exc:
-            raise HandledException("Failed to calibrate detector") from exc
-        finally:
-            self.callback(PluginStateMessage(state=PluginState.LOADED_IDLE))
-
-        self.shared_state.context = self._ref_app_instance._detector.context
-        self.broadcast()
-
 
 class PlotPlugin(DetectorPlotPluginBase):
-
-    STATUS_MSG_MAP = {
-        ProcessorLevelStatus.IN_RANGE: "In range",
-        ProcessorLevelStatus.NO_DETECTION: "Not available",
-        ProcessorLevelStatus.OVERFLOW: "Warning: Overflow",
-        ProcessorLevelStatus.OUT_OF_RANGE: "Out of range",
-    }
-
     def __init__(self, *, plot_layout: pg.GraphicsLayout, app_model: AppModel) -> None:
         super().__init__(plot_layout=plot_layout, app_model=app_model)
 
-        self.counter = 0
-        self.bar_loc = 0
-
     def setup_from_message(self, message: GeneralMessage) -> None:
         assert message.kwargs is not None
         self.setup(**message.kwargs)
 
     def update_from_message(self, message: GeneralMessage) -> None:
         assert isinstance(message.data, RefAppResult)
         self.update(message.data)
 
     def setup(
         self,
-        config: RefAppConfig,
-        num_curves: int,
+        ref_app_config: RefAppConfig,
+        plot_config: PlotConfig,
+        estimated_frame_rate: float,
+        nominal_zone_limits: npt.NDArray[np.float_],
+        wake_up_zone_limits: npt.NDArray[np.float_],
     ) -> None:
-
-        self.num_curves = num_curves
-        self.start_m = config.start_m
-        self.end_m = config.end_m
+        self.ref_app_config = ref_app_config
+        self.nominal_config = ref_app_config.nominal_config
+        self.wake_up_config = ref_app_config.wake_up_config
+
+        self.show_all_detected_zones = plot_config.show_all_detected_zones
+
+        self.history_length_s = 5
+        self.time_fifo: List[float] = []
+        self.intra_fifo: List[float] = []
+        self.inter_fifo: List[float] = []
 
         win = self.plot_layout
 
-        # Sweep plot
-        self.sweep_plot = win.addPlot(row=1, col=0, colspan=3)
-        self.sweep_plot.setMenuEnabled(False)
-        self.sweep_plot.showGrid(x=True, y=True)
-        self.sweep_plot.addLegend()
-        self.sweep_plot.setLabel("left", "Amplitude")
-        self.sweep_plot.setLabel("bottom", "Distance (m)")
-        self.sweep_plot.addItem(pg.PlotDataItem())
-
-        self.vertical_line_start = pg.InfiniteLine(
-            pen=et.utils.pg_pen_cycler(2),
-            label="Tank start",
-            labelOpts={
-                "position": 0.5,
-                "color": (0, 100, 0),
-                "fill": (200, 200, 200, 50),
-                "movable": True,
-            },
-        )
-        self.sweep_plot.addItem(self.vertical_line_start)
-        self.vertical_line_end = pg.InfiniteLine(
-            pen=et.utils.pg_pen_cycler(2),
-            label="Tank end",
-            labelOpts={
-                "position": 0.5,
-                "color": (0, 100, 0),
-                "fill": (200, 200, 200, 50),
-                "movable": True,
-            },
+        self.intra_limit_lines = []
+        self.inter_limit_lines = []
+
+        # Intra presence history plot
+
+        self.intra_hist_plot = win.addPlot(
+            row=0,
+            col=0,
+            title="Intra presence history (fast motions)",
+        )
+        self.intra_hist_plot.setMenuEnabled(False)
+        self.intra_hist_plot.setMouseEnabled(x=False, y=False)
+        self.intra_hist_plot.hideButtons()
+        self.intra_hist_plot.showGrid(x=True, y=True)
+        self.intra_hist_plot.setLabel("bottom", "Time (s)")
+        self.intra_hist_plot.setLabel("left", "Score")
+        self.intra_hist_plot.setXRange(-self.history_length_s, 0)
+        self.intra_history_smooth_max = et.utils.SmoothMax(estimated_frame_rate)
+        self.intra_hist_plot.setYRange(0, 10)
+        if not self.nominal_config.intra_enable:
+            intra_color = et.utils.color_cycler(1)
+            intra_color = f"{intra_color}50"
+            self.nominal_intra_dashed_pen = pg.mkPen(
+                intra_color, width=2.5, style=QtCore.Qt.DashLine
+            )
+            self.nominal_intra_pen = pg.mkPen(intra_color, width=2)
+        else:
+            self.nominal_intra_dashed_pen = et.utils.pg_pen_cycler(1, width=2.5, style="--")
+            self.nominal_intra_pen = et.utils.pg_pen_cycler(1)
+
+        self.intra_hist_curve = self.intra_hist_plot.plot(pen=self.nominal_intra_pen)
+        limit_line = pg.InfiniteLine(angle=0, pen=self.nominal_intra_dashed_pen)
+        self.intra_hist_plot.addItem(limit_line)
+        self.intra_limit_lines.append(limit_line)
+
+        for line in self.intra_limit_lines:
+            line.setPos(self.nominal_config.intra_detection_threshold)
+
+        # Inter presence history plot
+
+        self.inter_hist_plot = win.addPlot(
+            row=0,
+            col=1,
+            title="Inter presence history (slow motions)",
+        )
+        self.inter_hist_plot.setMenuEnabled(False)
+        self.inter_hist_plot.setMouseEnabled(x=False, y=False)
+        self.inter_hist_plot.hideButtons()
+        self.inter_hist_plot.showGrid(x=True, y=True)
+        self.inter_hist_plot.setLabel("bottom", "Time (s)")
+        self.inter_hist_plot.setLabel("left", "Score")
+        self.inter_hist_plot.setXRange(-self.history_length_s, 0)
+        self.inter_history_smooth_max = et.utils.SmoothMax(estimated_frame_rate)
+        self.inter_hist_plot.setYRange(0, 10)
+        if not self.nominal_config.inter_enable:
+            inter_color = et.utils.color_cycler(0)
+            inter_color = f"{inter_color}50"
+            self.nominal_inter_dashed_pen = pg.mkPen(
+                inter_color, width=2.5, style=QtCore.Qt.DashLine
+            )
+            self.nominal_inter_pen = pg.mkPen(inter_color, width=2)
+        else:
+            self.nominal_inter_pen = et.utils.pg_pen_cycler(0)
+            self.nominal_inter_dashed_pen = et.utils.pg_pen_cycler(0, width=2.5, style="--")
+
+        self.inter_hist_curve = self.inter_hist_plot.plot(pen=self.nominal_inter_pen)
+        limit_line = pg.InfiniteLine(angle=0, pen=self.nominal_inter_dashed_pen)
+        self.inter_hist_plot.addItem(limit_line)
+        self.inter_limit_lines.append(limit_line)
+
+        for line in self.inter_limit_lines:
+            line.setPos(self.nominal_config.inter_detection_threshold)
+
+        # Sector plot
+
+        if ref_app_config.wake_up_mode:
+            title = (
+                "Nominal config<br>"
+                "Detection type: fast (orange), slow (blue), both (green)<br>"
+                "Green background indicates active"
+            )
+        else:
+            title = "Nominal config<br>" "Detection type: fast (orange), slow (blue), both (green)"
+
+        self.nominal_sector_plot, self.nominal_sectors = self.create_sector_plot(
+            title,
+            self.ref_app_config.nominal_config.num_zones,
+            self.nominal_config.start_m,
+            nominal_zone_limits,
         )
-        self.sweep_plot.addItem(self.vertical_line_end)
 
-        pen = et.utils.pg_pen_cycler(0)
-        brush = et.utils.pg_brush_cycler(0)
-        symbol_kw = dict(symbol="o", symbolSize=1, symbolBrush=brush, symbolPen="k")
-        feat_kw = dict(pen=pen, **symbol_kw)
-        self.sweep_curves = [self.sweep_plot.plot(**feat_kw) for _ in range(self.num_curves)]
-
-        pen = et.utils.pg_pen_cycler(1)
-        brush = et.utils.pg_brush_cycler(1)
-        symbol_kw = dict(symbol="o", symbolSize=1, symbolBrush=brush, symbolPen="k")
-        feat_kw = dict(pen=pen, **symbol_kw)
-        self.threshold_curves = [self.sweep_plot.plot(**feat_kw) for _ in range(self.num_curves)]
-
-        sweep_plot_legend = pg.LegendItem(offset=(0.0, 0.5))
-        sweep_plot_legend.setParentItem(self.sweep_plot)
-        sweep_plot_legend.addItem(self.sweep_curves[0], "Sweep")
-        sweep_plot_legend.addItem(self.threshold_curves[0], "Threshold")
-
-        # Level history plot
-        self.level_history_plot = win.addPlot(row=0, col=1, colspan=2)
-        self.level_history_plot.setMenuEnabled(False)
-        self.level_history_plot.showGrid(x=True, y=True)
-        self.level_history_plot.addLegend()
-        self.level_history_plot.setLabel("left", "Estimated level (cm)")
-        self.level_history_plot.setLabel("bottom", "Time (s)")
-        self.level_history_plot.addItem(pg.PlotDataItem())
-
-        pen = et.utils.pg_pen_cycler(0)
-        brush = et.utils.pg_brush_cycler(0)
-        symbol_kw = dict(symbol="o", symbolSize=5, symbolBrush=brush, symbolPen="k")
-        feat_kw = dict(pen=pen, **symbol_kw)
-        self.level_history_curve = self.level_history_plot.plot(**feat_kw)
-
-        self.sweep_smooth_max = et.utils.SmoothMax()
-        self.distance_hist_smooth_lim = et.utils.SmoothLimits()
-
-        # Rect plot
-        self.num_rects = 15
-        self.rect_plot = pg.PlotItem()
-        self.rect_plot.setAspectLocked()
-        self.rect_plot.hideAxis("left")
-        self.rect_plot.hideAxis("bottom")
-        self.rects = []
-
-        pen = pg.mkPen(None)
-        rect_width = self.num_rects / 2.0
-        for r in np.arange(self.num_rects) + 1:
-            rect = pg.QtWidgets.QGraphicsRectItem(0, r, rect_width, 1)
-            rect.setPen(pen)
-            self.rect_plot.addItem(rect)
-            self.rects.append(rect)
+        if not ref_app_config.wake_up_mode:
+            sublayout = win.addLayout(row=1, col=0, colspan=2)
+            sublayout.layout.setColumnStretchFactor(0, 2)
+            sublayout.addItem(self.nominal_sector_plot, row=0, col=0)
+        else:
+            assert self.wake_up_config is not None
+            sublayout = win.addLayout(row=1, col=0, colspan=2)
+            sublayout.addItem(self.nominal_sector_plot, row=0, col=1)
+
+            title = (
+                "Wake up config<br>"
+                "Detection type: fast (orange), slow (blue), both (green),<br>"
+                "lingering (light grey)<br>"
+                "Green background indicates active"
+            )
+            self.wake_up_sector_plot, self.wake_up_sectors = self.create_sector_plot(
+                title,
+                self.wake_up_config.num_zones,
+                self.wake_up_config.start_m,
+                wake_up_zone_limits,
+            )
 
-        self.plot_layout.addItem(self.rect_plot, row=0, col=0)
+            sublayout.addItem(self.wake_up_sector_plot, row=0, col=0)
 
-        # text items
-        self.level_html_format = (
+            if self.wake_up_config.intra_enable:
+                self.wake_up_intra_dashed_pen = et.utils.pg_pen_cycler(1, width=2.5, style="--")
+                self.wake_up_intra_pen = et.utils.pg_pen_cycler(1)
+            else:
+                intra_color = et.utils.color_cycler(1)
+                intra_color = f"{intra_color}50"
+                self.wake_up_intra_dashed_pen = pg.mkPen(
+                    intra_color, width=2.5, style=QtCore.Qt.DashLine
+                )
+                self.wake_up_intra_pen = pg.mkPen(intra_color, width=2)
+
+            if self.wake_up_config.inter_enable:
+                self.wake_up_inter_pen = et.utils.pg_pen_cycler(0)
+                self.wake_up_inter_dashed_pen = et.utils.pg_pen_cycler(0, width=2.5, style="--")
+            else:
+                inter_color = et.utils.color_cycler(0)
+                inter_color = f"{inter_color}50"
+                self.wake_up_inter_dashed_pen = pg.mkPen(
+                    inter_color, width=2.5, style=QtCore.Qt.DashLine
+                )
+                self.wake_up_inter_pen = pg.mkPen(inter_color, width=2)
+
+    @staticmethod
+    def create_sector_plot(
+        title: str, num_sectors: int, start_m: float, zone_limits: npt.NDArray[np.float_]
+    ) -> Tuple[pg.PlotItem, List[pg.QtWidgets.QGraphicsEllipseItem]]:
+        sector_plot = pg.PlotItem(title=title)
+
+        sector_plot.setAspectLocked()
+        sector_plot.hideAxis("left")
+        sector_plot.hideAxis("bottom")
+
+        sectors = []
+        limit_text = []
+
+        range_html = (
             '<div style="text-align: center">'
-            '<span style="color: #FFFFFF;font-size:12pt;">'
+            '<span style="color: #000000;font-size:12pt;">'
             "{}</span></div>"
         )
 
-        self.level_text_item = pg.TextItem(
-            fill=pg.mkColor(0x1F, 0x77, 0xB4, 180),
-            anchor=(0.5, 0),
-        )
+        if start_m == zone_limits[0]:
+            x_offset = 0.7
+        else:
+            x_offset = 0
 
-        self.rect_plot.addItem(self.level_text_item)
-        self.level_text_item.hide()
+        pen = pg.mkPen("k", width=1)
+        span_deg = 25
+        for r in np.flip(np.arange(1, num_sectors + 2)):
+            sector = pg.QtWidgets.QGraphicsEllipseItem(-r, -r, r * 2, r * 2)
+            sector.setStartAngle(-16 * span_deg)
+            sector.setSpanAngle(16 * span_deg * 2)
+            sector.setPen(pen)
+            sector_plot.addItem(sector)
+            sectors.append(sector)
+
+            if r != 1:
+                limit = pg.TextItem(html=range_html, anchor=(0.5, 0.5), angle=25)
+                x = r * np.cos(np.radians(span_deg))
+                y = r * np.sin(np.radians(span_deg))
+                limit.setPos(x - x_offset, y + 0.25)
+                sector_plot.addItem(limit)
+                limit_text.append(limit)
+
+        sectors.reverse()
+
+        if not start_m == zone_limits[0]:
+            start_limit_text = pg.TextItem(html=range_html, anchor=(0.5, 0.5), angle=25)
+            start_range_html = range_html.format(f"{start_m}")
+            start_limit_text.setHtml(start_range_html)
+            x = 1 * np.cos(np.radians(span_deg))
+            y = 1 * np.sin(np.radians(span_deg))
+
+            start_limit_text.setPos(x, y + 0.25)
+            sector_plot.addItem(start_limit_text)
+
+        unit_text = pg.TextItem(html=range_html, anchor=(0.5, 0.5))
+        unit_html = range_html.format("[m]")
+        unit_text.setHtml(unit_html)
+        x = (num_sectors + 2) * np.cos(np.radians(span_deg))
+        y = (num_sectors + 2) * np.sin(np.radians(span_deg))
+        unit_text.setPos(x - x_offset, y + 0.25)
+        sector_plot.addItem(unit_text)
+
+        for (text_item, limit) in zip(limit_text, np.flip(zone_limits)):
+            zone_range_html = range_html.format(np.around(limit, 1))
+            text_item.setHtml(zone_range_html)
+
+        return sector_plot, sectors
+
+    def update(self, data: RefAppResult) -> None:
+        if data.used_config == _Mode.NOMINAL_CONFIG:
+            inter_threshold = self.nominal_config.inter_detection_threshold
+            intra_threshold = self.nominal_config.intra_detection_threshold
+            intra_pen = self.nominal_intra_pen
+            intra_dashed_pen = self.nominal_intra_dashed_pen
+            inter_pen = self.nominal_inter_pen
+            inter_dashed_pen = self.nominal_inter_dashed_pen
+        else:
+            assert self.wake_up_config is not None
+            inter_threshold = self.wake_up_config.inter_detection_threshold
+            intra_threshold = self.wake_up_config.intra_detection_threshold
+            intra_pen = self.wake_up_intra_pen
+            intra_dashed_pen = self.wake_up_intra_dashed_pen
+            inter_pen = self.wake_up_inter_pen
+            inter_dashed_pen = self.wake_up_inter_dashed_pen
+
+        self.time_fifo.append(data.service_result.tick_time)
+
+        if data.switch_delay:
+            self.intra_fifo.append(float("nan"))
+            self.inter_fifo.append(float("nan"))
+        else:
+            self.intra_fifo.append(data.intra_presence_score)
+            self.inter_fifo.append(data.inter_presence_score)
 
-    def update(
-        self,
-        result: RefAppResult,
-    ) -> None:
-        # Get the first element as the plugin only supports single sensor operation.
-        (detector_result,) = list(result.extra_result.detector_result.values())
-        assert detector_result.distances is not None
-
-        time_and_level_dict = (
-            result.extra_result.processor_extra_result.level_and_time_for_plotting
-        )
-
-        # update sweep plot
-        max_val_in_plot = 0
-        for idx, processor_result in enumerate(detector_result.processor_results):
-            assert processor_result.extra_result.used_threshold is not None
-            assert processor_result.extra_result.distances_m is not None
-            assert processor_result.extra_result.abs_sweep is not None
+        while self.time_fifo[-1] - self.time_fifo[0] > self.history_length_s:
+            self.time_fifo.pop(0)
+            self.intra_fifo.pop(0)
+            self.inter_fifo.pop(0)
 
-            self.sweep_curves[idx].setData(
-                processor_result.extra_result.distances_m, processor_result.extra_result.abs_sweep
-            )
+        times = [t - self.time_fifo[-1] for t in self.time_fifo]
 
-            self.threshold_curves[idx].setData(
-                processor_result.extra_result.distances_m,
-                processor_result.extra_result.used_threshold,
-            )
+        # Intra presence
 
-            max_val_in_subsweep = max(
-                max(processor_result.extra_result.used_threshold),
-                max(processor_result.extra_result.abs_sweep),
-            )
+        if np.isnan(self.intra_fifo).all():
+            m_hist = intra_threshold
+        else:
+            m_hist = np.maximum(float(np.nanmax(self.intra_fifo)), intra_threshold * 1.05)
 
-            max_val_in_plot = max(max_val_in_plot, max_val_in_subsweep)
+        m_hist = self.intra_history_smooth_max.update(m_hist)
 
-        self.sweep_plot.setYRange(0, self.sweep_smooth_max.update(max_val_in_plot))
-        self.vertical_line_start.setValue(self.start_m)
-        self.vertical_line_end.setValue(self.end_m)
-        self.vertical_line_start.show()
-        self.vertical_line_end.show()
-
-        # update level history plot
-        if any(~np.isnan(time_and_level_dict["level"])):
-            self.level_history_curve.setData(
-                time_and_level_dict["time"], time_and_level_dict["level"] * 100
-            )
-            self.level_history_plot.setXRange(-TIME_HISTORY_S + 1, 0)
-            self.level_history_plot.setYRange(0, (self.end_m - self.start_m + 0.01) * 100)
+        self.intra_hist_plot.setYRange(0, m_hist)
+        self.intra_hist_curve.setData(times, self.intra_fifo, connect="finite")
+        self.intra_hist_curve.setPen(intra_pen)
 
-        # update level plot
-        if (
-            result.level is not None
-            and result.peak_detected is not None
-            and result.peak_status is not None
-        ):
-            current_level = result.level
-            peak_detected = result.peak_detected
-            peak_status = result.peak_status
-
-            # Show the percentage level plot if the plot width is greater than 600 pixels,
-            # otherwise display the level as text.
-            if self.plot_layout.width() >= 600:
-                level_text = self.STATUS_MSG_MAP[peak_status]
-                if peak_status == ProcessorLevelStatus.OVERFLOW:
-                    for rect in self.rects:
-                        rect.setBrush(et.utils.pg_brush_cycler(0))
-                elif peak_detected and (peak_status == ProcessorLevelStatus.IN_RANGE):
-                    self.bar_loc = round(
-                        current_level / (self.end_m - self.start_m) * self.num_rects
-                    )
-                    for rect in self.rects[: self.bar_loc]:
-                        rect.setBrush(et.utils.pg_brush_cycler(0))
+        for line in self.intra_limit_lines:
+            line.setPos(intra_threshold)
+            line.setPen(intra_dashed_pen)
 
-                    for rect in self.rects[self.bar_loc :]:
-                        rect.setBrush(et.utils.pg_brush_cycler(1))
+        # Inter presence
 
-                    level_text = "Level: {:.1f} cm, {:.0f} %".format(
-                        current_level * 100,
-                        current_level / (self.end_m - self.start_m) * 100,
-                    )
-                    self.counter = 0
-                elif peak_detected and (peak_status == ProcessorLevelStatus.OUT_OF_RANGE):
-                    for rect in self.rects:
-                        rect.setBrush(et.utils.pg_brush_cycler(1))
-                elif ~peak_detected and (self.counter <= NO_DETECTION_TIMEOUT):
-                    for rect in self.rects[: self.bar_loc]:
-                        rect.setBrush(et.utils.pg_brush_cycler(0))
-
-                    for rect in self.rects[self.bar_loc :]:
-                        rect.setBrush(et.utils.pg_brush_cycler(1))
-
-                    self.counter += 1
-                else:
-                    for rect in self.rects:
-                        rect.setBrush(et.utils.pg_brush_cycler(1))
-                        self.bar_loc = 0
-                for rect in self.rects:
-                    rect.setVisible(True)
-
-                level_html = self.level_html_format.format(level_text)
-                self.level_text_item.setHtml(level_html)
-                self.level_text_item.setPos(self.num_rects / 4.0, self.num_rects + 4.0)
-                self.level_text_item.show()
-            else:
-                level_text = self.STATUS_MSG_MAP[peak_status]
-                if peak_detected and (peak_status == ProcessorLevelStatus.IN_RANGE):
-                    level_text = "Level: {:.1f} cm, {:.0f} %".format(
-                        current_level * 100,
-                        current_level / (self.end_m - self.start_m) * 100,
-                    )
-                    self.counter = 0
-                level_html = self.level_html_format.format(level_text)
-                self.level_text_item.setHtml(level_html)
-                self.level_text_item.setPos(self.num_rects / 4.0, self.num_rects + 4.0)
-                self.level_text_item.show()
-                for rect in self.rects:
-                    rect.setVisible(False)
+        if np.isnan(self.inter_fifo).all():
+            m_hist = inter_threshold
+        else:
+            m_hist = np.maximum(float(np.nanmax(self.inter_fifo)), inter_threshold * 1.05)
 
+        m_hist = self.inter_history_smooth_max.update(m_hist)
 
-class ViewPlugin(DetectorViewPluginBase):
+        self.inter_hist_plot.setYRange(0, m_hist)
+        self.inter_hist_curve.setData(times, self.inter_fifo, connect="finite")
+        self.inter_hist_curve.setPen(inter_pen)
 
-    TEXT_MSG_MAP = {
-        DetailedStatus.OK: "Ready to start.",
-        DetailedStatus.CONTEXT_MISSING: "Run detector calibration.",
-        DetailedStatus.CALIBRATION_MISSING: "Run detector calibration.",
-        DetailedStatus.CONFIG_MISMATCH: (
-            "Current configuration does not match the configuration "
-            + "used during detector calibration. Run detector calibration."
-        ),
-    }
+        for line in self.inter_limit_lines:
+            line.setPos(inter_threshold)
+            line.setPen(inter_dashed_pen)
+
+        # Sector
+
+        brush = et.utils.pg_brush_cycler(7)
+        for sector in self.nominal_sectors:
+            sector.setBrush(brush)
 
+        if not self.ref_app_config.wake_up_mode:
+            sectors = self.nominal_sectors[1:]
+            show_all_zones = self.show_all_detected_zones
+            color_nominal = "white"
+        else:
+            if data.used_config == _Mode.WAKE_UP_CONFIG:
+                sectors = self.wake_up_sectors[1:]
+                show_all_zones = True
+                color_wake_up = "#DFF1D6"
+                color_nominal = "white"
+            else:
+                sectors = self.nominal_sectors[1:]
+                show_all_zones = self.show_all_detected_zones
+                color_wake_up = "white"
+                color_nominal = "#DFF1D6"
+
+            vb = self.nominal_sector_plot.getViewBox()
+            vb.setBackgroundColor(color_nominal)
+            vb = self.wake_up_sector_plot.getViewBox()
+            vb.setBackgroundColor(color_wake_up)
+
+            for sector in self.wake_up_sectors:
+                sector.setBrush(brush)
+
+        if data.presence_detected:
+            self.color_zones(data, show_all_zones, sectors)
+            self.switch_data = data
+        elif data.switch_delay:
+            self.color_zones(self.switch_data, True, self.wake_up_sectors[1:])
+
+        self.nominal_sectors[0].setPen(pg.mkPen(color_nominal, width=1))
+        self.nominal_sectors[0].setBrush(pg.mkBrush(color_nominal))
+
+        if self.ref_app_config.wake_up_mode:
+            self.wake_up_sectors[0].setPen(pg.mkPen(color_wake_up, width=1))
+            self.wake_up_sectors[0].setBrush(pg.mkBrush(color_wake_up))
+
+    @staticmethod
+    def color_zones(
+        data: RefAppResult,
+        show_all_detected_zones: bool,
+        sectors: List[pg.QtWidgets.QGraphicsEllipseItem],
+    ) -> None:
+        if show_all_detected_zones:
+            for zone, (inter_value, intra_value) in enumerate(
+                zip(data.inter_zone_detections, data.intra_zone_detections)
+            ):
+                if inter_value + intra_value == 2:
+                    sectors[zone].setBrush(et.utils.pg_brush_cycler(2))
+                elif inter_value == 1:
+                    sectors[zone].setBrush(et.utils.pg_brush_cycler(0))
+                elif intra_value == 1:
+                    sectors[zone].setBrush(et.utils.pg_brush_cycler(1))
+                elif data.used_config == _Mode.WAKE_UP_CONFIG:
+                    assert data.wake_up_detections is not None
+                    if data.wake_up_detections[zone] > 0:
+                        sectors[zone].setBrush(pg.mkBrush("#b5afa0"))
+        else:
+            assert data.max_presence_zone is not None
+            if data.max_presence_zone == data.max_intra_zone:
+                sectors[data.max_presence_zone].setBrush(et.utils.pg_brush_cycler(1))
+            else:
+                sectors[data.max_presence_zone].setBrush(et.utils.pg_brush_cycler(0))
+
+
+class ViewPlugin(DetectorViewPluginBase):
     def __init__(self, app_model: AppModel, view_widget: QWidget) -> None:
         super().__init__(app_model=app_model, view_widget=view_widget)
-        self.app_model = app_model
         self._log = logging.getLogger(__name__)
 
         sticky_layout = QVBoxLayout()
         sticky_layout.setContentsMargins(0, 0, 0, 0)
         scrolly_layout = QVBoxLayout()
         scrolly_layout.setContentsMargins(0, 0, 0, 0)
 
@@ -505,263 +617,218 @@
         self.start_button.clicked.connect(self._send_start_request)
 
         self.stop_button = QPushButton(icons.STOP(), "Stop")
         self.stop_button.setShortcut("space")
         self.stop_button.setToolTip("Stops the session.\n\nShortcut: Space")
         self.stop_button.clicked.connect(self._send_stop_request)
 
-        self.calibrate_detector_button = QPushButton(icons.CALIBRATE(), "Calibrate detector")
-        self.calibrate_detector_button.clicked.connect(self._on_calibrate_detector)
-
-        self.defaults_button = QPushButton(icons.RESTORE(), "Reset settings and calibrations")
-        self.defaults_button.clicked.connect(self._send_defaults_request)
-
-        self.message_box = QLabel(self.sticky_widget)
-        self.message_box.setWordWrap(True)
-
         button_group = GroupBox.grid("Controls", parent=self.sticky_widget)
         button_group.layout().addWidget(self.start_button, 0, 0)
         button_group.layout().addWidget(self.stop_button, 0, 1)
-        button_group.layout().addWidget(self.calibrate_detector_button, 1, 0, 1, -1)
-        button_group.layout().addWidget(self.defaults_button, 3, 0, 1, -1)
-        button_group.layout().addWidget(self.message_box, 4, 0, 1, -1)
 
         sticky_layout.addWidget(button_group)
 
+        self.misc_error_view = MiscErrorView(self.scrolly_widget)
+        scrolly_layout.addWidget(self.misc_error_view)
+
         sensor_selection_group = GroupBox.vertical("Sensor selection", parent=self.scrolly_widget)
         self.sensor_id_pidget = pidgets.SensorIdPidgetFactory(items=[]).create(
             parent=sensor_selection_group
         )
         self.sensor_id_pidget.sig_update.connect(self._on_sensor_id_update)
         sensor_selection_group.layout().addWidget(self.sensor_id_pidget)
         scrolly_layout.addWidget(sensor_selection_group)
 
-        self.tank_level_config_editor = AttrsConfigEditor(
-            title="Tank level indicator parameters",
-            factory_mapping=self._get_processor_pidget_mapping(),
+        self.config_editor = AttrsConfigEditor(
+            title="Ref App parameters",
+            factory_mapping={
+                "wake_up_mode": pidgets.CheckboxPidgetFactory(
+                    name_label_text="Switch config on wake up"
+                )
+            },
             config_type=RefAppConfig,
-            extra_presenter=_set_config_presenter,
             parent=self.scrolly_widget,
         )
-        self.tank_level_config_editor.sig_update.connect(self._on_config_update)
-        scrolly_layout.addWidget(self.tank_level_config_editor)
+        self.config_editor.sig_update.connect(self._on_config_update)
+        scrolly_layout.addWidget(self.config_editor)
 
-        self.config_editor = AttrsConfigEditor(
-            title="Detector parameters",
-            factory_mapping=self._get_detector_pidget_mapping(),
-            config_type=RefAppConfig,
+        self.wake_up_config_editor = AttrsConfigEditor(
+            title="Wake up config parameters",
+            factory_mapping=self._get_presence_wake_up_pidget_mapping(),
+            config_type=PresenceWakeUpConfig,
+            parent=self.scrolly_widget,
+        )
+        self.wake_up_config_editor.sig_update.connect(self._on_wake_up_config_update)
+        scrolly_layout.addWidget(self.wake_up_config_editor)
+
+        self.nominal_config_editor = AttrsConfigEditor(
+            title="Nominal config parameters",
+            factory_mapping=self._get_presence_zone_pidget_mapping(),
+            config_type=PresenceZoneConfig,
+            parent=self.scrolly_widget,
+        )
+        self.nominal_config_editor.sig_update.connect(self._on_nominal_config_update)
+        scrolly_layout.addWidget(self.nominal_config_editor)
+
+        self.plot_config_editor = AttrsConfigEditor(
+            title="Plot parameters",
+            factory_mapping={
+                "show_all_detected_zones": pidgets.CheckboxPidgetFactory(
+                    name_label_text="Show all detected zones",
+                )
+            },
+            config_type=PlotConfig,
             save_load_buttons=False,
             parent=self.scrolly_widget,
         )
-        self.config_editor.sig_update.connect(self._on_config_update)
-        scrolly_layout.addWidget(self.config_editor)
+        self.plot_config_editor.sig_update.connect(self._on_plot_config_update)
+        scrolly_layout.addWidget(self.plot_config_editor)
 
         self.sticky_widget.setLayout(sticky_layout)
         self.scrolly_widget.setLayout(scrolly_layout)
 
     @classmethod
-    def _get_processor_pidget_mapping(cls) -> PidgetFactoryMapping:
-        return {
-            "median_filter_length": pidgets.IntPidgetFactory(
-                name_label_text="Median filter length",
-                limits=(1, 10),
-            ),
-            "num_medians_to_average": pidgets.IntPidgetFactory(
-                name_label_text="Num measurements averaged",
-                limits=(1, 10),
-            ),
-            "start_m": pidgets.FloatPidgetFactory(
-                name_label_text="Tank start",
-                suffix=" m",
-                decimals=3,
-                limits=(0.03, 20),
-            ),
-            "end_m": pidgets.FloatPidgetFactory(
-                name_label_text="Tank end",
-                suffix=" m",
-                decimals=3,
-                limits=(0.05, 20),
-            ),
-        }
+    def _get_presence_zone_pidget_mapping(cls) -> PidgetGroupFactoryMapping:
+        presence_pidget_mapping = dict(PresenceViewPlugin._get_pidget_mapping())
+        presence_pidget_mapping.update(
+            {
+                pidgets.FlatPidgetGroup(): {
+                    "num_zones": pidgets.IntPidgetFactory(
+                        name_label_text="Number of zones", limits=(1, None)
+                    )
+                }
+            }
+        )
+        return presence_pidget_mapping
 
     @classmethod
-    def _get_detector_pidget_mapping(cls) -> PidgetFactoryMapping:
-        COMMON_PIDGETS = {
-            "max_profile",
-            "reflector_shape",
-            "peaksorting_method",
-            "threshold_method",
-            "fixed_threshold_value",
-            "num_frames_in_recorded_threshold",
-            "threshold_sensitivity",
-            "signal_quality",
-        }
-
-        return {
-            "max_step_length": pidgets.OptionalIntPidgetFactory(
-                name_label_text="Max step length",
-                checkbox_label_text="Set",
-                limits=(1, None),
-                init_set_value=1,
-            ),
-            **{
-                aspect: factory
-                for aspect, factory in DistanceViewPlugin.get_pidget_mapping().items()
-                if aspect in COMMON_PIDGETS
-            },
-        }
+    def _get_presence_wake_up_pidget_mapping(cls) -> PidgetGroupFactoryMapping:
+        presence_pidget_mapping = dict(cls._get_presence_zone_pidget_mapping())
+        presence_pidget_mapping.update(
+            {
+                pidgets.FlatPidgetGroup(): {
+                    "num_zones_for_wake_up": pidgets.IntPidgetFactory(
+                        name_label_text="Number zones for wake up", limits=(1, None)
+                    )
+                }
+            }
+        )
+        return presence_pidget_mapping
 
     def on_backend_state_update(self, backend_plugin_state: Optional[SharedState]) -> None:
         if backend_plugin_state is not None and backend_plugin_state.config is not None:
-            self.config_editor.set_data(backend_plugin_state.config)
-            self.tank_level_config_editor.set_data(backend_plugin_state.config)
-
             results = backend_plugin_state.config._collect_validation_results()
 
-            not_handled = self.tank_level_config_editor.handle_validation_results(results)
-            not_handled = self.config_editor.handle_validation_results(not_handled)
+            not_handled = self.config_editor.handle_validation_results(results)
+
+            not_handled = self.wake_up_config_editor.handle_validation_results(not_handled)
+
+            not_handled = self.misc_error_view.handle_validation_results(not_handled)
+
+            self.wake_up_config_editor.setHidden(not backend_plugin_state.config.wake_up_mode)
 
             assert not_handled == []
-        else:
-            self.config_editor.set_data(None)
-            self.tank_level_config_editor.set_data(None)
 
     def on_app_model_update(self, app_model: AppModel) -> None:
         state = app_model.backend_plugin_state
 
         if state is None:
             self.start_button.setEnabled(False)
-            self.calibrate_detector_button.setEnabled(False)
             self.stop_button.setEnabled(False)
-            self.defaults_button.setEnabled(False)
 
+            self.config_editor.set_data(None)
             self.config_editor.setEnabled(False)
-            self.tank_level_config_editor.setEnabled(False)
+            self.nominal_config_editor.set_data(None)
+            self.nominal_config_editor.setEnabled(False)
+            self.wake_up_config_editor.set_data(None)
+            self.wake_up_config_editor.setEnabled(False)
             self.sensor_id_pidget.set_selected_sensor(None, [])
-            self.message_box.setText("")
 
             return
 
         assert isinstance(state, SharedState)
 
-        self.defaults_button.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
-
-        self.tank_level_config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
         self.config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
-
+        self.config_editor.set_data(state.config)
+        self.nominal_config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
+        self.nominal_config_editor.set_data(state.config.nominal_config)
+        self.wake_up_config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
+        self.wake_up_config_editor.set_data(state.config.wake_up_config)
+        self.plot_config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
+        self.plot_config_editor.set_data(state.plot_config)
         self.sensor_id_pidget.set_selected_sensor(state.sensor_id, app_model.connected_sensors)
         self.sensor_id_pidget.setEnabled(app_model.plugin_state.is_steady)
 
-        detector_status = Detector.get_detector_status(
-            state.config.to_detector_config(), state.context, [state.sensor_id]
-        )
-
-        self.message_box.setText(self.TEXT_MSG_MAP[detector_status.detector_state])
-
-        app_model_ready = app_model.is_ready_for_session()
-        try:
-            state.config.validate()
-        except a121.ValidationError:
-            config_valid = False
-        else:
-            config_valid = True
-
-        self.calibrate_detector_button.setEnabled(
-            app_model_ready
-            and config_valid
-            and self.config_editor.is_ready
-            and self.tank_level_config_editor.is_ready
-        )
         self.start_button.setEnabled(
-            detector_status.ready_to_start
-            and app_model_ready
-            and config_valid
-            and self.config_editor.is_ready
-            and self.tank_level_config_editor.is_ready
+            app_model.is_ready_for_session() and self.config_editor.is_ready
         )
         self.stop_button.setEnabled(app_model.plugin_state == PluginState.LOADED_BUSY)
 
-    def _on_sensor_id_update(self, sensor_id: int) -> None:
-        BackendPlugin.update_sensor_id.rpc(self.app_model.put_task, sensor_id=sensor_id)
-
     def _on_config_update(self, config: RefAppConfig) -> None:
         BackendPlugin.update_config.rpc(self.app_model.put_task, config=config)
 
-    # TODO: move to detector base (?)
-    def _send_start_request(self) -> None:
-        BackendPlugin.start_session.rpc(
-            self.app_model.put_task, with_recorder=self.app_model.recording_enabled
-        )
+    def _on_nominal_config_update(self, config: PresenceZoneConfig) -> None:
+        BackendPlugin.update_nominal_config.rpc(self.app_model.put_task, config=config)
 
-    # TODO: move to detector base (?)
-    def _send_stop_request(self) -> None:
-        BackendPlugin.stop_session.rpc(self.app_model.put_task)
+    def _on_wake_up_config_update(self, config: PresenceWakeUpConfig) -> None:
+        BackendPlugin.update_wake_up_config.rpc(self.app_model.put_task, config=config)
 
-    def _on_calibrate_detector(self) -> None:
-        BackendPlugin.calibrate_detector.rpc(self.app_model.put_task)
+    def _on_plot_config_update(self, config: PlotConfig) -> None:
+        BackendPlugin.update_plot_config.rpc(self.app_model.put_task, config=config)
 
     def _send_defaults_request(self) -> None:
         BackendPlugin.restore_defaults.rpc(self.app_model.put_task)
 
-
-def _set_config_presenter(instance: Any, presentation_type: PresentationType) -> Optional[str]:
-    if isinstance(instance, RefAppConfig) and presentation_type is PresentationType.C_SET_CONFIG:
-        config: RefAppConfig = instance
-        distance_config = config.to_detector_config()
-
-        return f"""
-static void set_config(acc_ref_app_tank_level_config_t *config, tank_level_preset_config_t preset)
-{{
-    // This snippet is generated to be compatible with RSS A121 v1.0.0
-    // If there is a version missmatch the snippet might need some modification
-
-    (void)preset;
-
-    config->tank_range_start_m     = {config.start_m:.3f}f;
-    config->tank_range_end_m       = {config.end_m:.3f}f;
-    config->median_filter_length   = {config.median_filter_length}U;
-    config->num_medians_to_average = {config.num_medians_to_average}U;
-
-    acc_detector_distance_config_start_set(config->distance_config, {distance_config.start_m:.3f}f);
-    acc_detector_distance_config_end_set(config->distance_config, {distance_config.end_m:.3f}f);
-    acc_detector_distance_config_max_step_length_set(config->distance_config, {distance_config.max_step_length or 0}U);
-    acc_detector_distance_config_max_profile_set(config->distance_config, ACC_CONFIG_{distance_config.max_profile.name});
-    acc_detector_distance_config_num_frames_recorded_threshold_set(config->distance_config, {distance_config.num_frames_in_recorded_threshold}U);
-    acc_detector_distance_config_peak_sorting_set(config->distance_config, ACC_DETECTOR_DISTANCE_PEAK_SORTING_{distance_config.peaksorting_method.name});
-    acc_detector_distance_config_reflector_shape_set(config->distance_config, ACC_DETECTOR_DISTANCE_REFLECTOR_SHAPE_{distance_config.reflector_shape.name});
-    acc_detector_distance_config_threshold_sensitivity_set(config->distance_config, {distance_config.threshold_sensitivity:.3f}f);
-    acc_detector_distance_config_signal_quality_set(config->distance_config, {distance_config.signal_quality:.3f}f);
-    acc_detector_distance_config_close_range_leakage_cancellation_set(config->distance_config, {str(distance_config.close_range_leakage_cancellation).lower()});
-}}
-"""
-
-    return None
+    def _on_sensor_id_update(self, sensor_id: int) -> None:
+        BackendPlugin.update_sensor_id.rpc(self.app_model.put_task, sensor_id=sensor_id)
 
 
 class PluginSpec(PluginSpecBase):
     def create_backend_plugin(
         self, callback: Callable[[Message], None], key: str
     ) -> BackendPlugin:
-        return BackendPlugin(callback, generation=self.generation, key=key)
+        return BackendPlugin(callback=callback, generation=self.generation, key=key)
 
     def create_view_plugin(self, app_model: AppModel, view_widget: QWidget) -> ViewPlugin:
         return ViewPlugin(app_model=app_model, view_widget=view_widget)
 
     def create_plot_plugin(
         self, app_model: AppModel, plot_layout: pg.GraphicsLayout
     ) -> PlotPlugin:
         return PlotPlugin(app_model=app_model, plot_layout=plot_layout)
 
 
-TANK_LEVEL_PLUGIN = PluginSpec(
+SMART_PRESENCE_PLUGIN = PluginSpec(
     generation=PluginGeneration.A121,
-    key="tank_level",
-    title="Tank level",
-    description="Measure liquid levels in tanks",
+    key="smart_presence",
+    title="Smart presence",
+    description="Split presence detection range into zones.",
     family=PluginFamily.REF_APP,
     presets=[
-        PluginPresetBase(name="Small", preset_id=PluginPresetId.SMALL),
-        PluginPresetBase(name="Medium", preset_id=PluginPresetId.MEDIUM),
-        PluginPresetBase(name="Large", preset_id=PluginPresetId.LARGE),
+        PluginPresetBase(
+            name="Short range",
+            description="Short range",
+            preset_id=PluginPresetId.SHORT_RANGE,
+        ),
+        PluginPresetBase(
+            name="Medium range",
+            description="Medium range",
+            preset_id=PluginPresetId.MEDIUM_RANGE,
+        ),
+        PluginPresetBase(
+            name="Long range",
+            description="Long range",
+            preset_id=PluginPresetId.LONG_RANGE,
+        ),
+        PluginPresetBase(
+            name="Ceiling",
+            description="Ceiling",
+            preset_id=PluginPresetId.CEILING,
+        ),
+        PluginPresetBase(
+            name="Low power, Wake up",
+            description="Low power, Wake up",
+            preset_id=PluginPresetId.LOW_POWER,
+        ),
     ],
-    default_preset_id=PluginPresetId.SMALL,
+    default_preset_id=PluginPresetId.MEDIUM_RANGE,
 )
```

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/tank_level/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/_serializer.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/tank_level/_serializer.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/_configs.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/_serializers.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/_serializers.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/vibration/_plugin.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/vibration/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/vibration/_processor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/vibration/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/launcher.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/launcher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/__init__.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/_argument_parser.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/_argument_parser.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/_enums.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/_enums.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/_version_checker.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/_version_checker.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app_model/app_model.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app_model/app_model.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app_model/app_model_listener.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app_model/app_model_listener.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app_model/file_detective.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app_model/file_detective.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app_model/port_updater.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app_model/port_updater.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_application_client.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_application_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_backend.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_backend.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_backend_logger.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_backend_logger.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_backend_plugin.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_backend_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_message.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_model.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_model.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_tasks.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_tasks.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/plugin_loader.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/storage.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/storage.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/app_model_viewer.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/app_model_viewer.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/device_comboboxes.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/device_comboboxes.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/flash_tab/threads.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/flash_tab/threads.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/help_tab.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/help_tab.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/icons.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/icons.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/main_window.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/main_window.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/misc.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/misc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/json_save_load_buttons.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/json_save_load_buttons.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/dialog.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/dialog.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/preview.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/preview.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/set_config_presenter.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/set_config_presenter.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/utils.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/status_bar.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/status_bar.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/hints.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/hints.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright (c) Acconeer AB, 2023
 # All rights reserved
 
 from __future__ import annotations
 
 import abc
-import platform
 import webbrowser
 from typing import List, Optional
 
 import qtawesome as qta
 
 from PySide6.QtWidgets import QHBoxLayout, QLabel, QPushButton, QWidget
 
@@ -77,39 +76,14 @@
         self.button.setHidden(True)
 
     def _on_click(self) -> None:
         if self._how_to_fix_url is not None:
             webbrowser.open_new_tab(self._how_to_fix_url)
 
 
-class ConnectionHint(HintObject):
-    def __init__(self) -> None:
-        super().__init__(
-            "Stability warning",
-            "You may experience stability issues due to windows serial port driver",
-            r"https://docs.acconeer.com/en/latest/evk_setup/xc120_xe121.html",
-        )
-
-    @staticmethod
-    def _should_show(app_model: AppModel) -> bool:
-        if platform.system().lower() != "windows":
-            return False
-
-        if (
-            app_model.serial_connection_device is not None
-            and app_model.connection_interface == ConnectionInterface.SERIAL
-        ):
-            if app_model.serial_connection_device.name is not None:
-                if app_model.serial_connection_device.unflashed:
-                    return False
-                return "xc120" in app_model.serial_connection_device.name.lower()
-
-        return False
-
-
 class UnflashedDeviceHint(HintObject):
     def __init__(self) -> None:
         super().__init__(
             "Unflashed device",
             "The device needs to be flashed with exploration server firmware",
             r"https://docs.acconeer.com/en/latest/evk_setup/xc120_xe121.html",
         )
@@ -171,8 +145,7 @@
         self.layout().addWidget(hint_widget)
 
         # Prioritized hint order:
         # The first will have priority over the second
         # The second will have priority over the third...
         hint_widget.add_hint(InaccessibleDeviceHint())
         hint_widget.add_hint(UnflashedDeviceHint())
-        hint_widget.add_hint(ConnectionHint())
```

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/utils.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/app.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/data_processing.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/data_processing.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/elements/helper.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/elements/helper.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/elements/modules.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/elements/modules.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/elements/qt_subclasses.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/elements/qt_subclasses.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/a111_gui.png` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/a111_gui.png`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/a121_gui.png` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/a121_gui.png`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/icon-black.svg` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/icon-black.svg`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/icon.png` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/icon.png`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/loader.gif` & `acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/loader.gif`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/LICENSE.txt` & `acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44` & `acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll` & `acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll` & `acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44` & `acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44` & `acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll` & `acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll` & `acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44` & `acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_bin_fetcher.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_bin_fetcher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_dev_license.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_dev_license.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_dev_license_tui.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_dev_license_tui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_flasher.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_flasher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_products.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_products.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/libft4222.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/libft4222.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/mpl_process.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/mpl_process.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/pg_process.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/pg_process.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/setup/__main__.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/setup/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/platform_install.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/platform_install.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/prompts.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/prompts.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/setup_group.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/setup_group.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/setup_step.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/setup_step.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/utils.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/setup/cli/argument_parser.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/setup/cli/argument_parser.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/setup/platforms/linux.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/setup/platforms/linux.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer/exptool/utils.py` & `acconeer-exptool-7.2.0/src/acconeer/exptool/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/src/acconeer_exptool.egg-info/PKG-INFO` & `acconeer-exptool-7.2.0/src/acconeer_exptool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acconeer-exptool
-Version: 7.1.0
+Version: 7.2.0
 Summary: Acconeer Exploration Tool
 Home-page: https://github.com/acconeer/acconeer-python-exploration
 Author: Acconeer AB
 Author-email: tools@acconeer.com
 License: BSD 3-Clause Clear License
 Project-URL: Tracker, https://github.com/acconeer/acconeer-python-exploration/issues
 Project-URL: Documentation, https://acconeer-python-exploration.readthedocs.io
@@ -36,15 +36,15 @@
 _**Explore the Next Sense**_ with Acconeer Exploration Tool! Use one of our [evaluation kits](https://www.acconeer.com/products) together with our Python examples and start exploring the world of Acconeer's radar sensor technology. The Python scripts and the Application in this repository will help you to easily stream the radar sensor's data to your local machine to start radar sensor evaluation and/or algorithm development for your application.
 
 To run the Python exploration scripts, you will need an [evaluation kit](https://www.acconeer.com/products) running the included Exploration or Module server, both of which are supplied with the [Acconeer SDK and Module SW](https://developer.acconeer.com/) image.
 
 This release is developed for [Acconeer SDK and Module SW](https://developer.acconeer.com/)
 **A111-v2.14.2**
 and
-**A121-v1.0.0**.
+**A121-v1.1.0**.
 Running this version is strongly recommended, as we continuously fix bugs and add features.
 
 <p align="center">
   <img alt="The application in action" src="https://raw.githubusercontent.com/acconeer/acconeer-python-exploration/8f633e02abac99ffec6fefec4339d13bc5c18388/docs/_static/gui.png" width=85%>
 </p>
 
 ## Quickstart for Windows
```

### Comparing `acconeer-exptool-7.1.0/src/acconeer_exptool.egg-info/SOURCES.txt` & `acconeer-exptool-7.2.0/src/acconeer_exptool.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 examples/a121/phase_tracking/phase_tracking.py
 examples/a121/presence/detector.py
 examples/a121/presence/processor.py
 examples/a121/record_data/barebones.py
 examples/a121/record_data/with_cli.py
 examples/a121/smart_presence/processor.py
 examples/a121/smart_presence/ref_app.py
+examples/a121/speed/detector.py
+examples/a121/speed/processor.py
 examples/a121/surface_velocity/example_app.py
 examples/a121/surface_velocity/processor.py
 examples/a121/touchless_button/processor.py
 examples/a121/vibration/vibration.py
 gui/main.py
 portable/.gitignore
 portable/make.py
```

### Comparing `acconeer-exptool-7.1.0/tools/check_changelog.py` & `acconeer-exptool-7.2.0/tools/check_changelog.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/tools/check_copyright.py` & `acconeer-exptool-7.2.0/tools/check_copyright.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/tools/check_line_length.py` & `acconeer-exptool-7.2.0/tools/check_line_length.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/tools/check_permissions.py` & `acconeer-exptool-7.2.0/tools/check_permissions.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/tools/check_sdk_mentions.py` & `acconeer-exptool-7.2.0/tools/check_sdk_mentions.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/tools/check_whitespace.py` & `acconeer-exptool-7.2.0/tools/check_whitespace.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/tools/update_regmap.py` & `acconeer-exptool-7.2.0/tools/update_regmap.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.1.0/utils/convert_to_csv.py` & `acconeer-exptool-7.2.0/utils/convert_to_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Acconeer AB, 2022
+# Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
 import abc
 import argparse
 import csv
@@ -132,15 +132,15 @@
 
     def get_metadata_rows(self, sensor: int) -> list[np.ndarray]:
         depths = et.a111.get_range_depths(self._record.sensor_config, self._record.session_info)
         num_points = len(depths)
         rounded_depths = np.round(depths, decimals=6)
 
         if self._record.mode != et.a111.Mode.SPARSE:
-            return rounded_depths
+            return [rounded_depths]
         else:
             spf = self._record.sensor_config.sweeps_per_frame
             sweep_numbers = np.repeat(range(spf), repeats=num_points).astype(int)
             depths_header = np.tile(rounded_depths, spf)
             return [sweep_numbers, depths_header]
 
     def convert(self, sensor: int) -> np.ndarray:
```

