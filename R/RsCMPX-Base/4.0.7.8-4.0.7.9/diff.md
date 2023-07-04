# Comparing `tmp/RsCMPX_Base-4.0.7.8.tar.gz` & `tmp/RsCMPX_Base-4.0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\RsCMPX_Base-4.0.7.8.tar", last modified: Mon Dec 28 20:24:14 2020, max compression
+gzip compressed data, was "dist\RsCMPX_Base-4.0.7.9.tar", last modified: Sun May 16 18:22:21 2021, max compression
```

## Comparing `RsCMPX_Base-4.0.7.8.tar` & `RsCMPX_Base-4.0.7.9.tar`

### file list

```diff
@@ -1,790 +1,791 @@
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.720286 RsCMPX_Base-4.0.7.8/
--rw-rw-rw-   0        0        0     2304 2020-12-28 20:24:14.720286 RsCMPX_Base-4.0.7.8/PKG-INFO
--rw-rw-rw-   0        0        0     1563 2020-12-28 20:24:11.000000 RsCMPX_Base-4.0.7.8/README.md
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:12.989093 RsCMPX_Base-4.0.7.8/RsCMPX_Base/
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.010038 RsCMPX_Base-4.0.7.8/RsCMPX_Base/CustomFiles/
--rw-rw-rw-   0        0        0        0 2020-12-28 20:24:11.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/CustomFiles/__init__.py
--rw-rw-rw-   0        0        0     2132 2020-12-28 20:24:11.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/CustomFiles/events.py
--rw-rw-rw-   0        0        0     4646 2020-12-28 20:24:11.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/CustomFiles/reliability.py
--rw-rw-rw-   0        0        0    17351 2020-12-28 20:24:11.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/CustomFiles/utilities.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.099799 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/
--rw-rw-rw-   0        0        0     1962 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.115755 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/
--rw-rw-rw-   0        0        0     4543 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Buffer.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.120741 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Buffer_/
--rw-rw-rw-   0        0        0      891 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Buffer_/LineCount.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Buffer_/__init__.py
--rw-rw-rw-   0        0        0     1060 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.124730 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/
--rw-rw-rw-   0        0        0     2791 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.134704 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/
--rw-rw-rw-   0        0        0     2051 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Slot.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.141685 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Slot_/
--rw-rw-rw-   0        0        0     1488 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Slot_/RxFilter.py
--rw-rw-rw-   0        0        0     1488 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Slot_/TxFilter.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Slot_/__init__.py
--rw-rw-rw-   0        0        0      893 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/State.py
--rw-rw-rw-   0        0        0     1249 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.147669 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/
--rw-rw-rw-   0        0        0     1298 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.155648 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/
--rw-rw-rw-   0        0        0     1005 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.161631 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected_/
--rw-rw-rw-   0        0        0     2063 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected_/Slot.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.171606 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected_/Slot_/
--rw-rw-rw-   0        0        0     2929 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected_/Slot_/RxFilter.py
--rw-rw-rw-   0        0        0     2929 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected_/Slot_/TxFilter.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected_/Slot_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected_/__init__.py
--rw-rw-rw-   0        0        0     1017 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.176591 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected_/
--rw-rw-rw-   0        0        0     2063 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected_/Slot.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.184571 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected_/Slot_/
--rw-rw-rw-   0        0        0     2935 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected_/Slot_/RxFilter.py
--rw-rw-rw-   0        0        0     2935 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected_/Slot_/TxFilter.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected_/Slot_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/__init__.py
--rw-rw-rw-   0        0        0     1319 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.193547 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/
--rw-rw-rw-   0        0        0     1005 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.198534 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected_/
--rw-rw-rw-   0        0        0     2063 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected_/Slot.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.206511 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected_/Slot_/
--rw-rw-rw-   0        0        0     2938 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected_/Slot_/RxFilter.py
--rw-rw-rw-   0        0        0     2938 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected_/Slot_/TxFilter.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected_/Slot_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected_/__init__.py
--rw-rw-rw-   0        0        0     1017 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.210501 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected_/
--rw-rw-rw-   0        0        0     2063 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected_/Slot.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.217484 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected_/Slot_/
--rw-rw-rw-   0        0        0     2944 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected_/Slot_/RxFilter.py
--rw-rw-rw-   0        0        0     2944 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected_/Slot_/TxFilter.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected_/Slot_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/__init__.py
--rw-rw-rw-   0        0        0     2499 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Ipc.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.221471 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Ipc_/
--rw-rw-rw-   0        0        0     1505 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Ipc_/Result.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Ipc_/__init__.py
--rw-rw-rw-   0        0        0     2449 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/MultiCmw.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.233441 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/MultiCmw_/
--rw-rw-rw-   0        0        0     1109 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/MultiCmw_/Identify.py
--rw-rw-rw-   0        0        0      973 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/MultiCmw_/Snumber.py
--rw-rw-rw-   0        0        0     1709 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/MultiCmw_/State.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/MultiCmw_/__init__.py
--rw-rw-rw-   0        0        0     4782 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.251394 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/
--rw-rw-rw-   0        0        0     1680 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.263360 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit_/
--rw-rw-rw-   0        0        0     1011 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit_/RxDc.py
--rw-rw-rw-   0        0        0     1029 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit_/RxImage.py
--rw-rw-rw-   0        0        0     1011 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit_/TxDc.py
--rw-rw-rw-   0        0        0     1029 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit_/TxImage.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit_/__init__.py
--rw-rw-rw-   0        0        0     1572 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Lvalid.py
--rw-rw-rw-   0        0        0      769 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Reliabiliy.py
--rw-rw-rw-   0        0        0     1064 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/State.py
--rw-rw-rw-   0        0        0     1671 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Trace.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.275328 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Trace_/
--rw-rw-rw-   0        0        0     1008 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Trace_/RxDc.py
--rw-rw-rw-   0        0        0     1026 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Trace_/RxImage.py
--rw-rw-rw-   0        0        0     1008 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Trace_/TxDc.py
--rw-rw-rw-   0        0        0     1026 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Trace_/TxImage.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Trace_/__init__.py
--rw-rw-rw-   0        0        0     1680 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.289291 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit_/
--rw-rw-rw-   0        0        0     1011 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit_/RxDc.py
--rw-rw-rw-   0        0        0     1029 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit_/RxImage.py
--rw-rw-rw-   0        0        0     1011 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit_/TxDc.py
--rw-rw-rw-   0        0        0     1029 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit_/TxImage.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit_/__init__.py
--rw-rw-rw-   0        0        0     1689 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.302256 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues_/
--rw-rw-rw-   0        0        0     1014 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues_/RxDc.py
--rw-rw-rw-   0        0        0     1032 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues_/RxImage.py
--rw-rw-rw-   0        0        0     1014 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues_/TxDc.py
--rw-rw-rw-   0        0        0     1032 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues_/TxImage.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/__init__.py
--rw-rw-rw-   0        0        0     1008 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Calibration.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.306244 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Calibration_/
--rw-rw-rw-   0        0        0     3395 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Calibration_/Base.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.315222 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Calibration_/Base_/
--rw-rw-rw-   0        0        0     3028 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Calibration_/Base_/Ipc.py
--rw-rw-rw-   0        0        0     1486 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Calibration_/Base_/Ipcr.py
--rw-rw-rw-   0        0        0     2354 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Calibration_/Base_/Latest.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.320207 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Calibration_/Base_/Latest_/
--rw-rw-rw-   0        0        0     1462 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Calibration_/Base_/Latest_/Specific.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Calibration_/Base_/Latest_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Calibration_/Base_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Calibration_/__init__.py
--rw-rw-rw-   0        0        0      983 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.324197 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/
--rw-rw-rw-   0        0        0     1278 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/Base.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.333173 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/Base_/
--rw-rw-rw-   0        0        0     1061 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/Base_/Correction.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.338159 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/
--rw-rw-rw-   0        0        0     1459 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.342149 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer_/
--rw-rw-rw-   0        0        0     2055 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer_/Slot.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.348134 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer_/Slot_/
--rw-rw-rw-   0        0        0     1141 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer_/Slot_/RxFilter.py
--rw-rw-rw-   0        0        0     1141 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer_/Slot_/TxFilter.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer_/Slot_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/__init__.py
--rw-rw-rw-   0        0        0      774 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/Base_/Salignment.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/Base_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/__init__.py
--rw-rw-rw-   0        0        0     3088 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Cmwd.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.353120 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Cmwd_/
--rw-rw-rw-   0        0        0      815 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Cmwd_/State.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Cmwd_/__init__.py
--rw-rw-rw-   0        0        0     2500 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.373066 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/
--rw-rw-rw-   0        0        0     3599 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.397002 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/
--rw-rw-rw-   0        0        0     2229 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Adjustment.py
--rw-rw-rw-   0        0        0     1061 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.403984 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/
--rw-rw-rw-   0        0        0     1013 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.408970 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/
--rw-rw-rw-   0        0        0     2055 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.418945 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/
--rw-rw-rw-   0        0        0     1015 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/RxFilter.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.425925 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/RxFilter_/
--rw-rw-rw-   0        0        0     1858 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/RxFilter_/Select.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/RxFilter_/__init__.py
--rw-rw-rw-   0        0        0     1015 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/TxFilter.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.433905 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/TxFilter_/
--rw-rw-rw-   0        0        0     1858 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/TxFilter_/Select.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/TxFilter_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/__init__.py
--rw-rw-rw-   0        0        0     1971 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.439887 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/
--rw-rw-rw-   0        0        0     3616 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.466818 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/
--rw-rw-rw-   0        0        0     1337 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Add.py
--rw-rw-rw-   0        0        0     1195 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Catalog.py
--rw-rw-rw-   0        0        0     1142 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Count.py
--rw-rw-rw-   0        0        0     1355 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Create.py
--rw-rw-rw-   0        0        0     2045 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Details.py
--rw-rw-rw-   0        0        0     1175 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Erase.py
--rw-rw-rw-   0        0        0      927 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Exist.py
--rw-rw-rw-   0        0        0      939 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Length.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/__init__.py
--rw-rw-rw-   0        0        0     1033 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/IpSubnet.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.472800 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/IpSubnet_/
--rw-rw-rw-   0        0        0     3916 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/IpSubnet_/NwAdapter.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/IpSubnet_/__init__.py
--rw-rw-rw-   0        0        0     1475 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Ipcr.py
--rw-rw-rw-   0        0        0     1033 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Mmonitor.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.477786 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Mmonitor_/
--rw-rw-rw-   0        0        0     3838 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Mmonitor_/IpAddress.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Mmonitor_/__init__.py
--rw-rw-rw-   0        0        0     1522 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/MultiCmw.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.482773 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/MultiCmw_/
--rw-rw-rw-   0        0        0     1178 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/MultiCmw_/Identify.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/MultiCmw_/__init__.py
--rw-rw-rw-   0        0        0     2058 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Salignment.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/__init__.py
--rw-rw-rw-   0        0        0     1064 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Cmwd.py
--rw-rw-rw-   0        0        0     2859 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/FreqCorrection.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.489754 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/FreqCorrection_/
--rw-rw-rw-   0        0        0     2468 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/FreqCorrection_/Activate.py
--rw-rw-rw-   0        0        0     2112 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/FreqCorrection_/Usage.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/FreqCorrection_/__init__.py
--rw-rw-rw-   0        0        0     3448 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Mutex.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.499729 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Mutex_/
--rw-rw-rw-   0        0        0     1173 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Mutex_/Define.py
--rw-rw-rw-   0        0        0     1134 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Mutex_/Lock.py
--rw-rw-rw-   0        0        0     1857 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Mutex_/State.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Mutex_/__init__.py
--rw-rw-rw-   0        0        0     3315 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Semaphore.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.513690 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Semaphore_/
--rw-rw-rw-   0        0        0      850 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Semaphore_/Acquire.py
--rw-rw-rw-   0        0        0      840 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Semaphore_/Count.py
--rw-rw-rw-   0        0        0     1328 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Semaphore_/Define.py
--rw-rw-rw-   0        0        0      990 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Semaphore_/Release.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Semaphore_/__init__.py
--rw-rw-rw-   0        0        0     1077 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.519674 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/
--rw-rw-rw-   0        0        0     2057 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.530645 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/
--rw-rw-rw-   0        0        0     3868 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Activate.py
--rw-rw-rw-   0        0        0     1196 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.539621 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/
--rw-rw-rw-   0        0        0     1409 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Rx.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.543610 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Rx_/
--rw-rw-rw-   0        0        0      876 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Rx_/All.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Rx_/__init__.py
--rw-rw-rw-   0        0        0     1409 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Tx.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.548596 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Tx_/
--rw-rw-rw-   0        0        0      876 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Tx_/All.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Tx_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/__init__.py
--rw-rw-rw-   0        0        0     1504 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Usage.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/__init__.py
--rw-rw-rw-   0        0        0     3013 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Spoint.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.557572 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Spoint_/
--rw-rw-rw-   0        0        0     1319 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Spoint_/Define.py
--rw-rw-rw-   0        0        0     2049 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Spoint_/Join.py
--rw-rw-rw-   0        0        0     1440 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Spoint_/Rewait.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Spoint_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/__init__.py
--rw-rw-rw-   0        0        0     4902 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.605444 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/
--rw-rw-rw-   0        0        0     1222 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Base.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.611429 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Base_/
--rw-rw-rw-   0        0        0      783 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Base_/Mmi.py
--rw-rw-rw-   0        0        0     1005 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.617414 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment_/
--rw-rw-rw-   0        0        0     1178 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment_/Path.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.624394 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment_/Path_/
--rw-rw-rw-   0        0        0     1975 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment_/Path_/Iq.py
--rw-rw-rw-   0        0        0     2020 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment_/Path_/Level.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment_/Path_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Base_/__init__.py
--rw-rw-rw-   0        0        0      782 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/BgInfo.py
--rw-rw-rw-   0        0        0     1851 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Cmw.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.629381 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Cmw_/
--rw-rw-rw-   0        0        0     1173 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Cmw_/LedTest.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.638358 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Cmw_/LedTest_/
--rw-rw-rw-   0        0        0     1055 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Cmw_/LedTest_/Rx.py
--rw-rw-rw-   0        0        0     1055 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Cmw_/LedTest_/Tx.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Cmw_/LedTest_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Cmw_/__init__.py
--rw-rw-rw-   0        0        0     2575 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.650325 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/
--rw-rw-rw-   0        0        0     1263 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.657306 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/
--rw-rw-rw-   0        0        0     3562 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/Rlogging.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.661296 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/Rlogging_/
--rw-rw-rw-   0        0        0      959 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/Rlogging_/Protocol.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/Rlogging_/__init__.py
--rw-rw-rw-   0        0        0     2924 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/TaLogging.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.669275 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/TaLogging_/
--rw-rw-rw-   0        0        0     1689 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/TaLogging_/Mode.py
--rw-rw-rw-   0        0        0      910 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/TaLogging_/Protocol.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/TaLogging_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/__init__.py
--rw-rw-rw-   0        0        0     1110 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Debug.py
--rw-rw-rw-   0        0        0     1029 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Statistics.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.674260 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Statistics_/
--rw-rw-rw-   0        0        0      943 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Statistics_/Process.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Statistics_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/__init__.py
--rw-rw-rw-   0        0        0     1212 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Eeprom.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.681242 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Eeprom_/
--rw-rw-rw-   0        0        0     1507 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Eeprom_/Data.py
--rw-rw-rw-   0        0        0     1408 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Eeprom_/Header.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Eeprom_/__init__.py
--rw-rw-rw-   0        0        0      981 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Error.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.686229 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Error_/
--rw-rw-rw-   0        0        0     2365 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Error_/Queue.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.690218 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Error_/Queue_/
--rw-rw-rw-   0        0        0     1189 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Error_/Queue_/Push.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Error_/Queue_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Error_/__init__.py
--rw-rw-rw-   0        0        0     1469 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.703184 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/
--rw-rw-rw-   0        0        0     2160 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.722133 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/
--rw-rw-rw-   0        0        0     1023 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Connection.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.728116 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Connection_/
--rw-rw-rw-   0        0        0      977 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Connection_/Target.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.736096 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Connection_/Target_/
--rw-rw-rw-   0        0        0     1006 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Connection_/Target_/Ids.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Connection_/Target_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Connection_/__init__.py
--rw-rw-rw-   0        0        0     1591 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Data.py
--rw-rw-rw-   0        0        0     1280 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Properties.py
--rw-rw-rw-   0        0        0     1279 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/References.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/__init__.py
--rw-rw-rw-   0        0        0      989 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Li.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.744074 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Li_/
--rw-rw-rw-   0        0        0      934 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Li_/Usecases.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Li_/__init__.py
--rw-rw-rw-   0        0        0     1354 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/UseCase.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.750059 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/UseCase_/
--rw-rw-rw-   0        0        0     1456 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/UseCase_/Data.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/UseCase_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/__init__.py
--rw-rw-rw-   0        0        0     1285 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Help.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.755045 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Help_/
--rw-rw-rw-   0        0        0     1200 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Help_/Syntax.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Help_/__init__.py
--rw-rw-rw-   0        0        0     1867 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Instrument.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.759034 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Instrument_/
--rw-rw-rw-   0        0        0      907 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Instrument_/Consistency.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Instrument_/__init__.py
--rw-rw-rw-   0        0        0      961 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Log.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.763023 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Log_/
--rw-rw-rw-   0        0        0      942 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Log_/Dump.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Log_/__init__.py
--rw-rw-rw-   0        0        0     1851 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Pias.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.772997 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Pias_/
--rw-rw-rw-   0        0        0     1783 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Pias_/Connect.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.777983 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Pias_/Connect_/
--rw-rw-rw-   0        0        0      928 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Pias_/Connect_/Multiple.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Pias_/Connect_/__init__.py
--rw-rw-rw-   0        0        0     1518 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Pias_/Scan.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Pias_/__init__.py
--rw-rw-rw-   0        0        0     4332 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Product.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.784965 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Product_/
--rw-rw-rw-   0        0        0     1688 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Product_/MacAddress.py
--rw-rw-rw-   0        0        0      782 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Product_/Time.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Product_/__init__.py
--rw-rw-rw-   0        0        0      987 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Record.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.789951 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Record_/
--rw-rw-rw-   0        0        0      975 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Record_/Macro.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.794938 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Record_/Macro_/
--rw-rw-rw-   0        0        0     3246 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Record_/Macro_/File.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Record_/Macro_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Record_/__init__.py
--rw-rw-rw-   0        0        0     1410 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Routing.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.801920 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Routing_/
--rw-rw-rw-   0        0        0      989 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Routing_/Expert.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.807904 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Routing_/Expert_/
--rw-rw-rw-   0        0        0     1759 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Routing_/Expert_/Setup.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Routing_/Expert_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Routing_/__init__.py
--rw-rw-rw-   0        0        0      749 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/SingleCmw.py
--rw-rw-rw-   0        0        0     1697 2020-12-28 20:24:08.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Status.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/__init__.py
--rw-rw-rw-   0        0        0     1667 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Display.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.812891 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Display_/
--rw-rw-rw-   0        0        0     1817 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Display_/Window.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.819873 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Display_/Window_/
--rw-rw-rw-   0        0        0     1520 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Display_/Window_/Select.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Display_/Window_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Display_/__init__.py
--rw-rw-rw-   0        0        0      800 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/FirmwareUpdate.py
--rw-rw-rw-   0        0        0      989 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/FormatPy.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.826852 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/FormatPy_/
--rw-rw-rw-   0        0        0     5053 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/FormatPy_/Base.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/FormatPy_/__init__.py
--rw-rw-rw-   0        0        0      687 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Get.py
--rw-rw-rw-   0        0        0      917 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/GlobalClearStatus.py
--rw-rw-rw-   0        0        0      882 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/GlobalWait.py
--rw-rw-rw-   0        0        0      873 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/GoToLocal.py
--rw-rw-rw-   0        0        0     1849 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/HardCopy.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.836827 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/HardCopy_/
--rw-rw-rw-   0        0        0     1271 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/HardCopy_/Device.py
--rw-rw-rw-   0        0        0     1036 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/HardCopy_/Interior.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/HardCopy_/__init__.py
--rw-rw-rw-   0        0        0     1905 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Instrument.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.845802 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Instrument_/
--rw-rw-rw-   0        0        0     2807 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Instrument_/Display.py
--rw-rw-rw-   0        0        0     2533 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Instrument_/Select.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Instrument_/__init__.py
--rw-rw-rw-   0        0        0     2143 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MacroCreate.py
--rw-rw-rw-   0        0        0     9419 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.870735 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/
--rw-rw-rw-   0        0        0     1763 2020-12-28 20:24:11.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Attribute.py
--rw-rw-rw-   0        0        0     2606 2020-12-28 20:24:11.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Catalog.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.874725 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Catalog_/
--rw-rw-rw-   0        0        0     1581 2020-12-28 20:24:11.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Catalog_/Length.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Catalog_/__init__.py
--rw-rw-rw-   0        0        0     1777 2020-12-28 20:24:11.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/CurrentDirectory.py
--rw-rw-rw-   0        0        0     2036 2020-12-28 20:24:11.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Dcatalog.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.879712 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Dcatalog_/
--rw-rw-rw-   0        0        0     1539 2020-12-28 20:24:11.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Dcatalog_/Length.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Dcatalog_/__init__.py
--rw-rw-rw-   0        0        0     1413 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Load.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.890682 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Load_/
--rw-rw-rw-   0        0        0     1221 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Load_/Item.py
--rw-rw-rw-   0        0        0     1364 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Load_/Macro.py
--rw-rw-rw-   0        0        0     1397 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Load_/State.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Load_/__init__.py
--rw-rw-rw-   0        0        0     1421 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Store.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.901653 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Store_/
--rw-rw-rw-   0        0        0     1510 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Store_/Item.py
--rw-rw-rw-   0        0        0     1211 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Store_/Macro.py
--rw-rw-rw-   0        0        0     1504 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Store_/State.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Store_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/__init__.py
--rw-rw-rw-   0        0        0     1094 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Procedure.py
--rw-rw-rw-   0        0        0     1019 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/RecallState.py
--rw-rw-rw-   0        0        0      981 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/SaveState.py
--rw-rw-rw-   0        0        0     1268 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.908634 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/
--rw-rw-rw-   0        0        0     1526 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.920602 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/
--rw-rw-rw-   0        0        0     1268 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/IpSubnet.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.930576 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/IpSubnet_/
--rw-rw-rw-   0        0        0     2274 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/IpSubnet_/Snode.py
--rw-rw-rw-   0        0        0     1901 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/IpSubnet_/SubMonitor.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/IpSubnet_/__init__.py
--rw-rw-rw-   0        0        0     1039 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/Reference.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.938554 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/Reference_/
--rw-rw-rw-   0        0        0      865 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/Reference_/Frequency.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/Reference_/__init__.py
--rw-rw-rw-   0        0        0     1706 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/Temperature.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.947530 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/Temperature_/
--rw-rw-rw-   0        0        0     2058 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/Temperature_/Exceeded.py
--rw-rw-rw-   0        0        0      815 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/Temperature_/Operating.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/Temperature_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/__init__.py
--rw-rw-rw-   0        0        0      758 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/FirmwareUpdate.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/__init__.py
--rw-rw-rw-   0        0        0      977 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Source.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.955516 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Source_/
--rw-rw-rw-   0        0        0     1015 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Source_/Base.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.961493 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Source_/Base_/
--rw-rw-rw-   0        0        0     1013 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Source_/Base_/Adjustment.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.967477 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Source_/Base_/Adjustment_/
--rw-rw-rw-   0        0        0     1205 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Source_/Base_/Adjustment_/State.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Source_/Base_/Adjustment_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Source_/Base_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Source_/__init__.py
--rw-rw-rw-   0        0        0     3065 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.988420 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/
--rw-rw-rw-   0        0        0      997 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Condition.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.993407 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Condition_/
--rw-rw-rw-   0        0        0     1431 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Condition_/Bits.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.004378 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Condition_/Bits_/
--rw-rw-rw-   0        0        0     1278 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Condition_/Bits_/All.py
--rw-rw-rw-   0        0        0     1308 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Condition_/Bits_/Cataloge.py
--rw-rw-rw-   0        0        0     1250 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Condition_/Bits_/Count.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Condition_/Bits_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Condition_/__init__.py
--rw-rw-rw-   0        0        0      973 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Event.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.009365 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Event_/
--rw-rw-rw-   0        0        0     2106 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Event_/Bits.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.021333 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Event_/Bits_/
--rw-rw-rw-   0        0        0     1266 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Event_/Bits_/All.py
--rw-rw-rw-   0        0        0     1238 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Event_/Bits_/Count.py
--rw-rw-rw-   0        0        0     1241 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Event_/Bits_/Next.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Event_/Bits_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Event_/__init__.py
--rw-rw-rw-   0        0        0     1037 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Generator.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.026319 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Generator_/
--rw-rw-rw-   0        0        0     1439 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Generator_/Condition.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.037290 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Generator_/Condition_/
--rw-rw-rw-   0        0        0     1266 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Generator_/Condition_/Off.py
--rw-rw-rw-   0        0        0     1260 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Generator_/Condition_/On.py
--rw-rw-rw-   0        0        0     1290 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Generator_/Condition_/Pending.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Generator_/Condition_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Generator_/__init__.py
--rw-rw-rw-   0        0        0     1049 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Measurement.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.044271 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Measurement_/
--rw-rw-rw-   0        0        0     1895 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Measurement_/Condition.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.066213 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/
--rw-rw-rw-   0        0        0     1272 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/Off.py
--rw-rw-rw-   0        0        0     1278 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/Qued.py
--rw-rw-rw-   0        0        0     1272 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/Rdy.py
--rw-rw-rw-   0        0        0     1272 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/Run.py
--rw-rw-rw-   0        0        0     1308 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/SdReached.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Measurement_/__init__.py
--rw-rw-rw-   0        0        0     3805 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Operation.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.075188 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Operation_/
--rw-rw-rw-   0        0        0     2805 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Operation_/Bit.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.093141 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/
--rw-rw-rw-   0        0        0     1052 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/Condition.py
--rw-rw-rw-   0        0        0     1653 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/Enable.py
--rw-rw-rw-   0        0        0     1030 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/Event.py
--rw-rw-rw-   0        0        0     1687 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/Ntransition.py
--rw-rw-rw-   0        0        0     1687 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/Ptransition.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Operation_/__init__.py
--rw-rw-rw-   0        0        0     3895 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Questionable.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.098128 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Questionable_/
--rw-rw-rw-   0        0        0     2805 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Questionable_/Bit.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.113087 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/
--rw-rw-rw-   0        0        0     1061 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/Condition.py
--rw-rw-rw-   0        0        0     1660 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/Enable.py
--rw-rw-rw-   0        0        0     1039 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/Event.py
--rw-rw-rw-   0        0        0     1705 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/Ntransition.py
--rw-rw-rw-   0        0        0     1705 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/Ptransition.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Questionable_/__init__.py
--rw-rw-rw-   0        0        0     1282 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Queue.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/__init__.py
--rw-rw-rw-   0        0        0    11892 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.172927 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/
--rw-rw-rw-   0        0        0     3120 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.201855 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/
--rw-rw-rw-   0        0        0     7286 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Device.py
--rw-rw-rw-   0        0        0     4421 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Display.py
--rw-rw-rw-   0        0        0     1041 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/IpSubnet.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.209829 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/IpSubnet_/
--rw-rw-rw-   0        0        0     1031 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/IpSubnet_/SubMonitor.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.216810 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/IpSubnet_/SubMonitor_/
--rw-rw-rw-   0        0        0     1055 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/IpSubnet_/SubMonitor_/Refresh.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/IpSubnet_/SubMonitor_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/IpSubnet_/__init__.py
--rw-rw-rw-   0        0        0     1511 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Option.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.226783 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Option_/
--rw-rw-rw-   0        0        0     1662 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Option_/Description.py
--rw-rw-rw-   0        0        0     2547 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Option_/ListPy.py
--rw-rw-rw-   0        0        0     1741 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Option_/Version.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Option_/__init__.py
--rw-rw-rw-   0        0        0     1475 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Password.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.231770 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Password_/
--rw-rw-rw-   0        0        0     1561 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Password_/Cenable.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Password_/__init__.py
--rw-rw-rw-   0        0        0     1471 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Reference.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.244736 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Reference_/
--rw-rw-rw-   0        0        0      975 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Reference_/Dc.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.250721 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Reference_/Dc_/
--rw-rw-rw-   0        0        0     1207 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Reference_/Dc_/Offset.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Reference_/Dc_/__init__.py
--rw-rw-rw-   0        0        0     3738 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Reference_/Frequency.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.258698 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Reference_/Frequency_/
--rw-rw-rw-   0        0        0     1013 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Reference_/Frequency_/Advanced.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.266677 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Reference_/Frequency_/Advanced_/
--rw-rw-rw-   0        0        0     1995 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Reference_/Frequency_/Advanced_/Source.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Reference_/Frequency_/Advanced_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Reference_/Frequency_/__init__.py
--rw-rw-rw-   0        0        0     1168 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Reference_/Phase.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Reference_/__init__.py
--rw-rw-rw-   0        0        0     1845 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Ssync.py
--rw-rw-rw-   0        0        0     2248 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/StIcon.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/__init__.py
--rw-rw-rw-   0        0        0     1843 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Cmw.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.275653 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Cmw_/
--rw-rw-rw-   0        0        0     1166 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Cmw_/Device.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.284629 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Cmw_/Device_/
--rw-rw-rw-   0        0        0     1042 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Cmw_/Device_/Id.py
--rw-rw-rw-   0        0        0     1060 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Cmw_/Device_/Vi.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Cmw_/Device_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Cmw_/__init__.py
--rw-rw-rw-   0        0        0     2350 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.308565 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/
--rw-rw-rw-   0        0        0     2117 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Gpib.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.315546 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/
--rw-rw-rw-   0        0        0     1202 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/Self.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.326517 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/Self_/
--rw-rw-rw-   0        0        0     1796 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/Self_/Addr.py
--rw-rw-rw-   0        0        0     1798 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/Self_/Enable.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/Self_/__init__.py
--rw-rw-rw-   0        0        0     1134 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/Vresource.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/__init__.py
--rw-rw-rw-   0        0        0     1936 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Hislip.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.331503 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Hislip_/
--rw-rw-rw-   0        0        0     1192 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Hislip_/Vresource.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Hislip_/__init__.py
--rw-rw-rw-   0        0        0     6229 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Net.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.340479 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Net_/
--rw-rw-rw-   0        0        0     2367 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Net_/Dns.py
--rw-rw-rw-   0        0        0     1738 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Net_/Subnet.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Net_/__init__.py
--rw-rw-rw-   0        0        0     1902 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Rsib.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.346463 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Rsib_/
--rw-rw-rw-   0        0        0     1134 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Rsib_/Vresource.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Rsib_/__init__.py
--rw-rw-rw-   0        0        0     2370 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Socket.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.360426 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Socket_/
--rw-rw-rw-   0        0        0     2226 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Socket_/Mode.py
--rw-rw-rw-   0        0        0     1881 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Socket_/Port.py
--rw-rw-rw-   0        0        0     1200 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Socket_/Vresource.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Socket_/__init__.py
--rw-rw-rw-   0        0        0      803 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Usb.py
--rw-rw-rw-   0        0        0     2091 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Vxi.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.372394 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Vxi_/
--rw-rw-rw-   0        0        0     1824 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Vxi_/Gtr.py
--rw-rw-rw-   0        0        0     1153 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Vxi_/Vresource.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Vxi_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/__init__.py
--rw-rw-rw-   0        0        0     1053 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Connector.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.378379 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Connector_/
--rw-rw-rw-   0        0        0     1494 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Connector_/Translation.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Connector_/__init__.py
--rw-rw-rw-   0        0        0     4086 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Date.py
--rw-rw-rw-   0        0        0      793 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Device.py
--rw-rw-rw-   0        0        0     1219 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/DeviceFootprint.py
--rw-rw-rw-   0        0        0     1708 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Display.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.384362 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Display_/
--rw-rw-rw-   0        0        0     1340 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Display_/Monitor.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.391343 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Display_/Monitor_/
--rw-rw-rw-   0        0        0      983 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Display_/Monitor_/Off.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Display_/Monitor_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Display_/__init__.py
--rw-rw-rw-   0        0        0     3084 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Error.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.398326 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Error_/
--rw-rw-rw-   0        0        0     1411 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Error_/Code.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Error_/__init__.py
--rw-rw-rw-   0        0        0      989 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Generator.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.405306 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Generator_/
--rw-rw-rw-   0        0        0      955 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Generator_/All.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.411290 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Generator_/All_/
--rw-rw-rw-   0        0        0     1053 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Generator_/All_/Off.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Generator_/All_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Generator_/__init__.py
--rw-rw-rw-   0        0        0     1453 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Help.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.426250 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Help_/
--rw-rw-rw-   0        0        0      994 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Help_/Headers.py
--rw-rw-rw-   0        0        0     1124 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Help_/Status.py
--rw-rw-rw-   0        0        0     1118 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Help_/Syntax.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Help_/__init__.py
--rw-rw-rw-   0        0        0     1001 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Measurement.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.431237 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Measurement_/
--rw-rw-rw-   0        0        0      955 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Measurement_/All.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.438217 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Measurement_/All_/
--rw-rw-rw-   0        0        0     1065 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Measurement_/All_/Off.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Measurement_/All_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Measurement_/__init__.py
--rw-rw-rw-   0        0        0      983 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Password.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.442207 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Password_/
--rw-rw-rw-   0        0        0     1060 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Password_/New.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Password_/__init__.py
--rw-rw-rw-   0        0        0      987 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Record.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.449189 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Record_/
--rw-rw-rw-   0        0        0      975 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Record_/Macro.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.455173 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Record_/Macro_/
--rw-rw-rw-   0        0        0     1584 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Record_/Macro_/File.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Record_/Macro_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Record_/__init__.py
--rw-rw-rw-   0        0        0     1017 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Routing.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.460160 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Routing_/
--rw-rw-rw-   0        0        0     1086 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Routing_/Possible.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Routing_/__init__.py
--rw-rw-rw-   0        0        0      989 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Signaling.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.465146 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Signaling_/
--rw-rw-rw-   0        0        0      955 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Signaling_/All.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.472127 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Signaling_/All_/
--rw-rw-rw-   0        0        0     1053 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Signaling_/All_/Off.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Signaling_/All_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Signaling_/__init__.py
--rw-rw-rw-   0        0        0     1013 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/SingleCmw.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.480106 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/SingleCmw_/
--rw-rw-rw-   0        0        0      739 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/SingleCmw_/Device.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/SingleCmw_/__init__.py
--rw-rw-rw-   0        0        0     1009 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Startup.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.487088 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Startup_/
--rw-rw-rw-   0        0        0     1116 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Startup_/Prepare.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Startup_/__init__.py
--rw-rw-rw-   0        0        0     5125 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Time.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.499055 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Time_/
--rw-rw-rw-   0        0        0     2541 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Time_/DaylightSavingTime.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.506038 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Time_/DaylightSavingTime_/
--rw-rw-rw-   0        0        0     2490 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Time_/DaylightSavingTime_/Rule.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Time_/DaylightSavingTime_/__init__.py
--rw-rw-rw-   0        0        0     1595 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Time_/HrTimer.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.511023 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Time_/HrTimer_/
--rw-rw-rw-   0        0        0     2300 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Time_/HrTimer_/Absolute.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.516353 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Time_/HrTimer_/Absolute_/
--rw-rw-rw-   0        0        0     2990 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Time_/HrTimer_/Absolute_/Set.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Time_/HrTimer_/Absolute_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Time_/HrTimer_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Time_/__init__.py
--rw-rw-rw-   0        0        0     1406 2020-12-28 20:24:09.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Update.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/__init__.py
--rw-rw-rw-   0        0        0      988 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.522335 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/
--rw-rw-rw-   0        0        0      980 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.526325 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/
--rw-rw-rw-   0        0        0     1210 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.534304 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/
--rw-rw-rw-   0        0        0     1962 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/Display.py
--rw-rw-rw-   0        0        0     4194 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.567216 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/
--rw-rw-rw-   0        0        0     1041 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Dexecution.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.572202 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Dexecution_/
--rw-rw-rw-   0        0        0     1756 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Dexecution_/Duration.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Dexecution_/__init__.py
--rw-rw-rw-   0        0        0     1663 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Enable.py
--rw-rw-rw-   0        0        0     3053 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/FilterPy.py
--rw-rw-rw-   0        0        0     1897 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/FormatPy.py
--rw-rw-rw-   0        0        0     1690 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Functions.py
--rw-rw-rw-   0        0        0     1722 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Name.py
--rw-rw-rw-   0        0        0     1663 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Parser.py
--rw-rw-rw-   0        0        0     1636 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Rpc.py
--rw-rw-rw-   0        0        0     1661 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Size.py
--rw-rw-rw-   0        0        0     1927 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/StartMode.py
--rw-rw-rw-   0        0        0     1907 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/StopMode.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/__init__.py
--rw-rw-rw-   0        0        0      984 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger.py
--rw-rw-rw-   0        0        0      893 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/TriggerInvoke.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.576191 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/
--rw-rw-rw-   0        0        0     1685 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.590155 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/
--rw-rw-rw-   0        0        0     2029 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/Eout.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.596138 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/
--rw-rw-rw-   0        0        0     1005 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/Catalog.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.602122 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/Catalog_/
--rw-rw-rw-   0        0        0     1080 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/Catalog_/Source.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/Catalog_/__init__.py
--rw-rw-rw-   0        0        0     1625 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/Source.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/__init__.py
--rw-rw-rw-   0        0        0     4136 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/ExtA.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.607109 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/ExtA_/
--rw-rw-rw-   0        0        0      920 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/ExtA_/Catalog.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/ExtA_/__init__.py
--rw-rw-rw-   0        0        0     4136 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/ExtB.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.611099 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/ExtB_/
--rw-rw-rw-   0        0        0      920 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/ExtB_/Catalog.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/ExtB_/__init__.py
--rw-rw-rw-   0        0        0     1882 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/UserInitiated.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.617556 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/UserInitiated_/
--rw-rw-rw-   0        0        0     1616 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/UserInitiated_/Execute.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/UserInitiated_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/__init__.py
--rw-rw-rw-   0        0        0    11186 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Unit.py
--rw-rw-rw-   0        0        0      987 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Write.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.623540 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Write_/
--rw-rw-rw-   0        0        0      979 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Write_/Eeprom.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.628526 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Write_/Eeprom_/
--rw-rw-rw-   0        0        0      972 2020-12-28 20:24:10.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Write_/Eeprom_/Data.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Write_/Eeprom_/__init__.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Write_/__init__.py
--rw-rw-rw-   0        0        0        0 2019-11-18 07:28:01.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/__init__.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:14.715299 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/
--rw-rw-rw-   0        0        0      560 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/ArgLinkedEventArgs.py
--rw-rw-rw-   0        0        0     4106 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/ArgSingle.py
--rw-rw-rw-   0        0        0     1086 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/ArgSingleList.py
--rw-rw-rw-   0        0        0     1028 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/ArgSingleSuppressed.py
--rw-rw-rw-   0        0        0     9241 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/ArgStringComposer.py
--rw-rw-rw-   0        0        0     5762 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/ArgStruct.py
--rw-rw-rw-   0        0        0     3433 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/ArgStructList.py
--rw-rw-rw-   0        0        0     2502 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/ArgStructStringParser.py
--rw-rw-rw-   0        0        0     5309 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/CommandsGroup.py
--rw-rw-rw-   0        0        0    20352 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/Conversions.py
--rw-rw-rw-   0        0        0     3693 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/ConverterFromScpiString.py
--rw-rw-rw-   0        0        0     4489 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/ConverterToScpiString.py
--rw-rw-rw-   0        0        0    10071 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/Core.py
--rw-rw-rw-   0        0        0    35553 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/Instrument.py
--rw-rw-rw-   0        0        0     4021 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/InstrumentErrors.py
--rw-rw-rw-   0        0        0     2161 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/InstrumentOptions.py
--rw-rw-rw-   0        0        0     5258 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/InstrumentSettings.py
--rw-rw-rw-   0        0        0     3467 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/InternalLinker.py
--rw-rw-rw-   0        0        0     4435 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/IoTransferEventArgs.py
--rw-rw-rw-   0        0        0     3747 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/RepeatedCapability.py
--rw-rw-rw-   0        0        0     4847 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/StreamReader.py
--rw-rw-rw-   0        0        0     5074 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/StreamWriter.py
--rw-rw-rw-   0        0        0     1069 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/StructBase.py
--rw-rw-rw-   0        0        0     3002 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/Types.py
--rw-rw-rw-   0        0        0     4669 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/Utilities.py
--rw-rw-rw-   0        0        0     5025 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/VisaPluginSocketIo.py
--rw-rw-rw-   0        0        0    44245 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/VisaSession.py
--rw-rw-rw-   0        0        0     7168 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/VisaSessionSim.py
--rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/__init__.py
--rw-rw-rw-   0        0        0    16279 2020-12-28 20:24:11.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/RsCMPX_Base.py
--rw-rw-rw-   0        0        0      848 2020-12-28 20:24:11.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/__init__.py
--rw-rw-rw-   0        0        0    11436 2020-12-28 20:24:05.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/enums.py
--rw-rw-rw-   0        0        0     5833 2020-12-28 20:24:05.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base/repcap.py
-drwxrwxrwx   0        0        0        0 2020-12-28 20:24:13.001062 RsCMPX_Base-4.0.7.8/RsCMPX_Base.egg-info/
--rw-rw-rw-   0        0        0     2304 2020-12-28 20:24:12.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    36939 2020-12-28 20:24:12.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-12-28 20:24:12.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2020-12-28 20:24:12.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2020-12-28 20:24:12.000000 RsCMPX_Base-4.0.7.8/RsCMPX_Base.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-12-28 20:24:14.722280 RsCMPX_Base-4.0.7.8/setup.cfg
--rw-rw-rw-   0        0        0      882 2020-12-28 20:24:11.000000 RsCMPX_Base-4.0.7.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:21.280895 RsCMPX_Base-4.0.7.9/
+-rw-rw-rw-   0        0        0     2474 2021-05-16 18:22:21.280895 RsCMPX_Base-4.0.7.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1638 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/README.md
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.330262 RsCMPX_Base-4.0.7.9/RsCMPX_Base/
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.375143 RsCMPX_Base-4.0.7.9/RsCMPX_Base/CustomFiles/
+-rw-rw-rw-   0        0        0        0 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/CustomFiles/__init__.py
+-rw-rw-rw-   0        0        0     3304 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/CustomFiles/events.py
+-rw-rw-rw-   0        0        0     4517 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/CustomFiles/reliability.py
+-rw-rw-rw-   0        0        0    18659 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/CustomFiles/utilities.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.544697 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/
+-rw-rw-rw-   0        0        0     1962 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.581592 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/
+-rw-rw-rw-   0        0        0     4568 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Buffer.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.594558 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Buffer_/
+-rw-rw-rw-   0        0        0      891 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Buffer_/LineCount.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Buffer_/__init__.py
+-rw-rw-rw-   0        0        0     1060 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.604531 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/
+-rw-rw-rw-   0        0        0     2791 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.632456 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/
+-rw-rw-rw-   0        0        0     2051 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Slot.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.650409 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Slot_/
+-rw-rw-rw-   0        0        0     1488 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Slot_/RxFilter.py
+-rw-rw-rw-   0        0        0     1488 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Slot_/TxFilter.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Slot_/__init__.py
+-rw-rw-rw-   0        0        0      893 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/State.py
+-rw-rw-rw-   0        0        0     1249 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.670357 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/
+-rw-rw-rw-   0        0        0     1298 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.687310 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/
+-rw-rw-rw-   0        0        0     1005 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.699278 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected_/
+-rw-rw-rw-   0        0        0     2063 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected_/Slot.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.717229 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected_/Slot_/
+-rw-rw-rw-   0        0        0     2929 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected_/Slot_/RxFilter.py
+-rw-rw-rw-   0        0        0     2929 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected_/Slot_/TxFilter.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected_/Slot_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected_/__init__.py
+-rw-rw-rw-   0        0        0     1017 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.727203 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected_/
+-rw-rw-rw-   0        0        0     2063 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected_/Slot.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.744158 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected_/Slot_/
+-rw-rw-rw-   0        0        0     2935 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected_/Slot_/RxFilter.py
+-rw-rw-rw-   0        0        0     2935 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected_/Slot_/TxFilter.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected_/Slot_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/__init__.py
+-rw-rw-rw-   0        0        0     1319 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.761113 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/
+-rw-rw-rw-   0        0        0     1005 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.772085 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected_/
+-rw-rw-rw-   0        0        0     2063 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected_/Slot.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.788043 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected_/Slot_/
+-rw-rw-rw-   0        0        0     2938 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected_/Slot_/RxFilter.py
+-rw-rw-rw-   0        0        0     2938 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected_/Slot_/TxFilter.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected_/Slot_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected_/__init__.py
+-rw-rw-rw-   0        0        0     1017 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.799012 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected_/
+-rw-rw-rw-   0        0        0     2063 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected_/Slot.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.814969 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected_/Slot_/
+-rw-rw-rw-   0        0        0     2944 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected_/Slot_/RxFilter.py
+-rw-rw-rw-   0        0        0     2944 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected_/Slot_/TxFilter.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected_/Slot_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/__init__.py
+-rw-rw-rw-   0        0        0     2499 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Ipc.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.825940 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Ipc_/
+-rw-rw-rw-   0        0        0     1505 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Ipc_/Result.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Ipc_/__init__.py
+-rw-rw-rw-   0        0        0     2449 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/MultiCmw.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.846883 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/MultiCmw_/
+-rw-rw-rw-   0        0        0     1109 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/MultiCmw_/Identify.py
+-rw-rw-rw-   0        0        0      974 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/MultiCmw_/Snumber.py
+-rw-rw-rw-   0        0        0     1709 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/MultiCmw_/State.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/MultiCmw_/__init__.py
+-rw-rw-rw-   0        0        0     4790 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.886137 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/
+-rw-rw-rw-   0        0        0     1680 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.910072 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit_/
+-rw-rw-rw-   0        0        0     1011 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit_/RxDc.py
+-rw-rw-rw-   0        0        0     1029 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit_/RxImage.py
+-rw-rw-rw-   0        0        0     1011 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit_/TxDc.py
+-rw-rw-rw-   0        0        0     1029 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit_/TxImage.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit_/__init__.py
+-rw-rw-rw-   0        0        0     1572 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Lvalid.py
+-rw-rw-rw-   0        0        0      773 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Reliability.py
+-rw-rw-rw-   0        0        0     1064 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/State.py
+-rw-rw-rw-   0        0        0     1671 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Trace.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.932013 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Trace_/
+-rw-rw-rw-   0        0        0     1008 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Trace_/RxDc.py
+-rw-rw-rw-   0        0        0     1026 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Trace_/RxImage.py
+-rw-rw-rw-   0        0        0     1008 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Trace_/TxDc.py
+-rw-rw-rw-   0        0        0     1026 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Trace_/TxImage.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Trace_/__init__.py
+-rw-rw-rw-   0        0        0     1680 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.956948 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit_/
+-rw-rw-rw-   0        0        0     1011 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit_/RxDc.py
+-rw-rw-rw-   0        0        0     1029 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit_/RxImage.py
+-rw-rw-rw-   0        0        0     1011 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit_/TxDc.py
+-rw-rw-rw-   0        0        0     1029 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit_/TxImage.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit_/__init__.py
+-rw-rw-rw-   0        0        0     1689 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.980883 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues_/
+-rw-rw-rw-   0        0        0     1014 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues_/RxDc.py
+-rw-rw-rw-   0        0        0     1032 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues_/RxImage.py
+-rw-rw-rw-   0        0        0     1014 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues_/TxDc.py
+-rw-rw-rw-   0        0        0     1032 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues_/TxImage.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/__init__.py
+-rw-rw-rw-   0        0        0     1008 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Calibration.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.990904 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Calibration_/
+-rw-rw-rw-   0        0        0     3395 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Calibration_/Base.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.009853 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Calibration_/Base_/
+-rw-rw-rw-   0        0        0     3028 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Calibration_/Base_/Ipc.py
+-rw-rw-rw-   0        0        0     1486 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Calibration_/Base_/Ipcr.py
+-rw-rw-rw-   0        0        0     2354 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Calibration_/Base_/Latest.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.019828 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Calibration_/Base_/Latest_/
+-rw-rw-rw-   0        0        0     1462 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Calibration_/Base_/Latest_/Specific.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Calibration_/Base_/Latest_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Calibration_/Base_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Calibration_/__init__.py
+-rw-rw-rw-   0        0        0      983 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.029800 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/
+-rw-rw-rw-   0        0        0     1278 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/Base.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.045757 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/Base_/
+-rw-rw-rw-   0        0        0     1061 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/Base_/Correction.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.054734 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/
+-rw-rw-rw-   0        0        0     1459 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.062712 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer_/
+-rw-rw-rw-   0        0        0     2055 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer_/Slot.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.077672 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer_/Slot_/
+-rw-rw-rw-   0        0        0     1141 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer_/Slot_/RxFilter.py
+-rw-rw-rw-   0        0        0     1141 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer_/Slot_/TxFilter.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer_/Slot_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/__init__.py
+-rw-rw-rw-   0        0        0      775 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/Base_/Salignment.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/Base_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/__init__.py
+-rw-rw-rw-   0        0        0     3088 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Cmwd.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.086649 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Cmwd_/
+-rw-rw-rw-   0        0        0      815 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Cmwd_/State.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Cmwd_/__init__.py
+-rw-rw-rw-   0        0        0     2500 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.120558 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/
+-rw-rw-rw-   0        0        0     3575 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.163443 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/
+-rw-rw-rw-   0        0        0     2229 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Adjustment.py
+-rw-rw-rw-   0        0        0     1061 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.173417 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/
+-rw-rw-rw-   0        0        0     1013 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.180401 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/
+-rw-rw-rw-   0        0        0     2055 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.195358 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/
+-rw-rw-rw-   0        0        0     1015 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/RxFilter.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.205840 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/RxFilter_/
+-rw-rw-rw-   0        0        0     1858 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/RxFilter_/Select.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/RxFilter_/__init__.py
+-rw-rw-rw-   0        0        0     1015 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/TxFilter.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.213818 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/TxFilter_/
+-rw-rw-rw-   0        0        0     1858 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/TxFilter_/Select.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/TxFilter_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/__init__.py
+-rw-rw-rw-   0        0        0     1971 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.223790 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/
+-rw-rw-rw-   0        0        0     6133 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.250719 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/
+-rw-rw-rw-   0        0        0     1196 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Catalog.py
+-rw-rw-rw-   0        0        0     1143 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Count.py
+-rw-rw-rw-   0        0        0     2045 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Details.py
+-rw-rw-rw-   0        0        0      927 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Exist.py
+-rw-rw-rw-   0        0        0      939 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Length.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/__init__.py
+-rw-rw-rw-   0        0        0     1015 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/IpSet.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.261690 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/IpSet_/
+-rw-rw-rw-   0        0        0     3910 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/IpSet_/NwAdapter.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/IpSet_/__init__.py
+-rw-rw-rw-   0        0        0     1475 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Ipcr.py
+-rw-rw-rw-   0        0        0     1033 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Mmonitor.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.270667 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Mmonitor_/
+-rw-rw-rw-   0        0        0     3838 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Mmonitor_/IpAddress.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Mmonitor_/__init__.py
+-rw-rw-rw-   0        0        0     1522 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/MultiCmw.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.279641 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/MultiCmw_/
+-rw-rw-rw-   0        0        0     1178 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/MultiCmw_/Identify.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/MultiCmw_/__init__.py
+-rw-rw-rw-   0        0        0     2058 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Salignment.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/__init__.py
+-rw-rw-rw-   0        0        0     1064 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Cmwd.py
+-rw-rw-rw-   0        0        0     2859 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/FreqCorrection.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.293605 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/FreqCorrection_/
+-rw-rw-rw-   0        0        0     2473 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/FreqCorrection_/Activate.py
+-rw-rw-rw-   0        0        0     2112 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/FreqCorrection_/Usage.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/FreqCorrection_/__init__.py
+-rw-rw-rw-   0        0        0     3448 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Mutex.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.311557 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Mutex_/
+-rw-rw-rw-   0        0        0     1173 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Mutex_/Define.py
+-rw-rw-rw-   0        0        0     1134 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Mutex_/Lock.py
+-rw-rw-rw-   0        0        0     1857 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Mutex_/State.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Mutex_/__init__.py
+-rw-rw-rw-   0        0        0     3315 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Semaphore.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.334495 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Semaphore_/
+-rw-rw-rw-   0        0        0      850 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Semaphore_/Acquire.py
+-rw-rw-rw-   0        0        0      840 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Semaphore_/Count.py
+-rw-rw-rw-   0        0        0     1328 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Semaphore_/Define.py
+-rw-rw-rw-   0        0        0      990 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Semaphore_/Release.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Semaphore_/__init__.py
+-rw-rw-rw-   0        0        0     1077 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.343472 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/
+-rw-rw-rw-   0        0        0     2057 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.361424 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/
+-rw-rw-rw-   0        0        0     1182 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Activate.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.375386 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Activate_/
+-rw-rw-rw-   0        0        0     1772 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Activate_/Rx.py
+-rw-rw-rw-   0        0        0     1772 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Activate_/Tx.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Activate_/__init__.py
+-rw-rw-rw-   0        0        0     1196 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.389928 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/
+-rw-rw-rw-   0        0        0     1413 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Rx.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.398903 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Rx_/
+-rw-rw-rw-   0        0        0      876 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Rx_/All.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Rx_/__init__.py
+-rw-rw-rw-   0        0        0     1413 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Tx.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.408877 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Tx_/
+-rw-rw-rw-   0        0        0      876 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Tx_/All.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Tx_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/__init__.py
+-rw-rw-rw-   0        0        0     1504 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Usage.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/__init__.py
+-rw-rw-rw-   0        0        0     3013 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Spoint.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.427827 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Spoint_/
+-rw-rw-rw-   0        0        0     1319 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Spoint_/Define.py
+-rw-rw-rw-   0        0        0     2049 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Spoint_/Join.py
+-rw-rw-rw-   0        0        0     1440 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Spoint_/Rewait.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Spoint_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/__init__.py
+-rw-rw-rw-   0        0        0     4902 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.507627 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/
+-rw-rw-rw-   0        0        0     1222 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Base.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.520592 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Base_/
+-rw-rw-rw-   0        0        0      783 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Base_/Mmi.py
+-rw-rw-rw-   0        0        0     1005 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.528570 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment_/
+-rw-rw-rw-   0        0        0     1178 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment_/Path.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.542533 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment_/Path_/
+-rw-rw-rw-   0        0        0     1976 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment_/Path_/Iq.py
+-rw-rw-rw-   0        0        0     2021 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment_/Path_/Level.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment_/Path_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Base_/__init__.py
+-rw-rw-rw-   0        0        0      782 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/BgInfo.py
+-rw-rw-rw-   0        0        0     1851 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Cmw.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.551509 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Cmw_/
+-rw-rw-rw-   0        0        0     1173 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Cmw_/LedTest.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.565472 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Cmw_/LedTest_/
+-rw-rw-rw-   0        0        0     1055 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Cmw_/LedTest_/Rx.py
+-rw-rw-rw-   0        0        0     1055 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Cmw_/LedTest_/Tx.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Cmw_/LedTest_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Cmw_/__init__.py
+-rw-rw-rw-   0        0        0     2575 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.584421 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/
+-rw-rw-rw-   0        0        0     1263 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.598384 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/
+-rw-rw-rw-   0        0        0     3562 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/Rlogging.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.608358 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/Rlogging_/
+-rw-rw-rw-   0        0        0      959 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/Rlogging_/Protocol.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/Rlogging_/__init__.py
+-rw-rw-rw-   0        0        0     2924 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/TaLogging.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.623319 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/TaLogging_/
+-rw-rw-rw-   0        0        0     1689 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/TaLogging_/Mode.py
+-rw-rw-rw-   0        0        0      910 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/TaLogging_/Protocol.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/TaLogging_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/__init__.py
+-rw-rw-rw-   0        0        0     1110 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Debug.py
+-rw-rw-rw-   0        0        0     1029 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Statistics.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.632294 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Statistics_/
+-rw-rw-rw-   0        0        0      943 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Statistics_/Process.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Statistics_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/__init__.py
+-rw-rw-rw-   0        0        0     1212 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Eeprom.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.646257 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Eeprom_/
+-rw-rw-rw-   0        0        0     1513 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Eeprom_/Data.py
+-rw-rw-rw-   0        0        0     1408 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Eeprom_/Header.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Eeprom_/__init__.py
+-rw-rw-rw-   0        0        0      981 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Error.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.653239 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Error_/
+-rw-rw-rw-   0        0        0     2365 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Error_/Queue.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.662214 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Error_/Queue_/
+-rw-rw-rw-   0        0        0     1189 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Error_/Queue_/Push.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Error_/Queue_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Error_/__init__.py
+-rw-rw-rw-   0        0        0     1469 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.682161 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/
+-rw-rw-rw-   0        0        0     2160 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.705100 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/
+-rw-rw-rw-   0        0        0     1023 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Connection.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.713078 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Connection_/
+-rw-rw-rw-   0        0        0      977 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Connection_/Target.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.722054 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Connection_/Target_/
+-rw-rw-rw-   0        0        0     1006 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Connection_/Target_/Ids.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Connection_/Target_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Connection_/__init__.py
+-rw-rw-rw-   0        0        0     1591 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Data.py
+-rw-rw-rw-   0        0        0     1280 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Properties.py
+-rw-rw-rw-   0        0        0     1279 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/References.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/__init__.py
+-rw-rw-rw-   0        0        0      989 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Li.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.732028 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Li_/
+-rw-rw-rw-   0        0        0      934 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Li_/Usecases.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Li_/__init__.py
+-rw-rw-rw-   0        0        0     1354 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/UseCase.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.741003 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/UseCase_/
+-rw-rw-rw-   0        0        0     1456 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/UseCase_/Data.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/UseCase_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/__init__.py
+-rw-rw-rw-   0        0        0     1285 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Help.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.749979 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Help_/
+-rw-rw-rw-   0        0        0     1200 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Help_/Syntax.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Help_/__init__.py
+-rw-rw-rw-   0        0        0     1899 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Instrument.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.757959 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Instrument_/
+-rw-rw-rw-   0        0        0      907 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Instrument_/Consistency.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Instrument_/__init__.py
+-rw-rw-rw-   0        0        0      961 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Log.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.764940 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Log_/
+-rw-rw-rw-   0        0        0      942 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Log_/Dump.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Log_/__init__.py
+-rw-rw-rw-   0        0        0     1851 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Pias.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.777905 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Pias_/
+-rw-rw-rw-   0        0        0     1783 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Pias_/Connect.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.786882 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Pias_/Connect_/
+-rw-rw-rw-   0        0        0      928 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Pias_/Connect_/Multiple.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Pias_/Connect_/__init__.py
+-rw-rw-rw-   0        0        0     1518 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Pias_/Scan.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Pias_/__init__.py
+-rw-rw-rw-   0        0        0     4332 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Product.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.800845 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Product_/
+-rw-rw-rw-   0        0        0     1688 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Product_/MacAddress.py
+-rw-rw-rw-   0        0        0      782 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Product_/Time.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Product_/__init__.py
+-rw-rw-rw-   0        0        0      987 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Record.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.810817 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Record_/
+-rw-rw-rw-   0        0        0      975 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Record_/Macro.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.818796 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Record_/Macro_/
+-rw-rw-rw-   0        0        0     3246 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Record_/Macro_/File.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Record_/Macro_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Record_/__init__.py
+-rw-rw-rw-   0        0        0     1410 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Routing.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.828770 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Routing_/
+-rw-rw-rw-   0        0        0      989 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Routing_/Expert.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.839741 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Routing_/Expert_/
+-rw-rw-rw-   0        0        0     1768 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Routing_/Expert_/Setup.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Routing_/Expert_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Routing_/__init__.py
+-rw-rw-rw-   0        0        0      749 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/SingleCmw.py
+-rw-rw-rw-   0        0        0     1697 2021-05-16 18:22:13.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Status.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/__init__.py
+-rw-rw-rw-   0        0        0     1667 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Display.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.848717 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Display_/
+-rw-rw-rw-   0        0        0     1817 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Display_/Window.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.858690 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Display_/Window_/
+-rw-rw-rw-   0        0        0     1520 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Display_/Window_/Select.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Display_/Window_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Display_/__init__.py
+-rw-rw-rw-   0        0        0      800 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/FirmwareUpdate.py
+-rw-rw-rw-   0        0        0      989 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/FormatPy.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.868663 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/FormatPy_/
+-rw-rw-rw-   0        0        0     5053 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/FormatPy_/Base.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/FormatPy_/__init__.py
+-rw-rw-rw-   0        0        0      687 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Get.py
+-rw-rw-rw-   0        0        0      917 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/GlobalClearStatus.py
+-rw-rw-rw-   0        0        0      882 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/GlobalWait.py
+-rw-rw-rw-   0        0        0      873 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/GotoLocal.py
+-rw-rw-rw-   0        0        0     1849 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/HardCopy.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.885618 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/HardCopy_/
+-rw-rw-rw-   0        0        0     1271 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/HardCopy_/Device.py
+-rw-rw-rw-   0        0        0     1036 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/HardCopy_/Interior.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/HardCopy_/__init__.py
+-rw-rw-rw-   0        0        0     1905 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Instrument.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.904569 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Instrument_/
+-rw-rw-rw-   0        0        0     2807 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Instrument_/Display.py
+-rw-rw-rw-   0        0        0     2533 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Instrument_/Select.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Instrument_/__init__.py
+-rw-rw-rw-   0        0        0     2143 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MacroCreate.py
+-rw-rw-rw-   0        0        0     9381 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.941469 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/
+-rw-rw-rw-   0        0        0     1763 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Attribute.py
+-rw-rw-rw-   0        0        0     2606 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Catalog.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.950445 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Catalog_/
+-rw-rw-rw-   0        0        0     1581 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Catalog_/Length.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Catalog_/__init__.py
+-rw-rw-rw-   0        0        0     1777 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/CurrentDirectory.py
+-rw-rw-rw-   0        0        0     2036 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Dcatalog.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.960418 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Dcatalog_/
+-rw-rw-rw-   0        0        0     1539 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Dcatalog_/Length.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Dcatalog_/__init__.py
+-rw-rw-rw-   0        0        0     1413 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Load.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.981363 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Load_/
+-rw-rw-rw-   0        0        0     1216 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Load_/Item.py
+-rw-rw-rw-   0        0        0     1359 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Load_/Macro.py
+-rw-rw-rw-   0        0        0     1392 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Load_/State.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Load_/__init__.py
+-rw-rw-rw-   0        0        0     1421 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Store.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:19.999316 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Store_/
+-rw-rw-rw-   0        0        0     1505 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Store_/Item.py
+-rw-rw-rw-   0        0        0     1206 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Store_/Macro.py
+-rw-rw-rw-   0        0        0     1499 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Store_/State.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Store_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/__init__.py
+-rw-rw-rw-   0        0        0     1094 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Procedure.py
+-rw-rw-rw-   0        0        0     1019 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/RecallState.py
+-rw-rw-rw-   0        0        0      981 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/SaveState.py
+-rw-rw-rw-   0        0        0     1268 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.013277 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/
+-rw-rw-rw-   0        0        0     1502 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.035219 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/
+-rw-rw-rw-   0        0        0     1247 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/IpSet.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.052176 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/IpSet_/
+-rw-rw-rw-   0        0        0     2265 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/IpSet_/Snode.py
+-rw-rw-rw-   0        0        0     1889 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/IpSet_/SubMonitor.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/IpSet_/__init__.py
+-rw-rw-rw-   0        0        0     1039 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/Reference.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.063145 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/Reference_/
+-rw-rw-rw-   0        0        0      865 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/Reference_/Frequency.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/Reference_/__init__.py
+-rw-rw-rw-   0        0        0     1706 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/Temperature.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.079102 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/Temperature_/
+-rw-rw-rw-   0        0        0     2058 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/Temperature_/Exceeded.py
+-rw-rw-rw-   0        0        0      815 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/Temperature_/Operating.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/Temperature_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/__init__.py
+-rw-rw-rw-   0        0        0      758 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/FirmwareUpdate.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/__init__.py
+-rw-rw-rw-   0        0        0      977 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Source.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.088078 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Source_/
+-rw-rw-rw-   0        0        0     1015 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Source_/Base.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.098051 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Source_/Base_/
+-rw-rw-rw-   0        0        0     1013 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Source_/Base_/Adjustment.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.108024 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Source_/Base_/Adjustment_/
+-rw-rw-rw-   0        0        0     1205 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Source_/Base_/Adjustment_/State.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Source_/Base_/Adjustment_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Source_/Base_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Source_/__init__.py
+-rw-rw-rw-   0        0        0     3065 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.145923 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/
+-rw-rw-rw-   0        0        0      997 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Condition.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.154899 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Condition_/
+-rw-rw-rw-   0        0        0     1431 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Condition_/Bits.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.174846 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Condition_/Bits_/
+-rw-rw-rw-   0        0        0     1278 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Condition_/Bits_/All.py
+-rw-rw-rw-   0        0        0     1308 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Condition_/Bits_/Cataloge.py
+-rw-rw-rw-   0        0        0     1250 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Condition_/Bits_/Count.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Condition_/Bits_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Condition_/__init__.py
+-rw-rw-rw-   0        0        0      973 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Event.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.182824 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Event_/
+-rw-rw-rw-   0        0        0     2106 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Event_/Bits.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.200777 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Event_/Bits_/
+-rw-rw-rw-   0        0        0     1266 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Event_/Bits_/All.py
+-rw-rw-rw-   0        0        0     1238 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Event_/Bits_/Count.py
+-rw-rw-rw-   0        0        0     1241 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Event_/Bits_/Next.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Event_/Bits_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Event_/__init__.py
+-rw-rw-rw-   0        0        0     1037 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Generator.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.210750 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Generator_/
+-rw-rw-rw-   0        0        0     1439 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Generator_/Condition.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.228703 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Generator_/Condition_/
+-rw-rw-rw-   0        0        0     1266 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Generator_/Condition_/Off.py
+-rw-rw-rw-   0        0        0     1260 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Generator_/Condition_/On.py
+-rw-rw-rw-   0        0        0     1290 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Generator_/Condition_/Pending.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Generator_/Condition_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Generator_/__init__.py
+-rw-rw-rw-   0        0        0     1049 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Measurement.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.236682 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Measurement_/
+-rw-rw-rw-   0        0        0     1895 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Measurement_/Condition.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.266601 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/
+-rw-rw-rw-   0        0        0     1272 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/Off.py
+-rw-rw-rw-   0        0        0     1278 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/Qued.py
+-rw-rw-rw-   0        0        0     1272 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/Rdy.py
+-rw-rw-rw-   0        0        0     1272 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/Run.py
+-rw-rw-rw-   0        0        0     1308 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/SdReached.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Measurement_/__init__.py
+-rw-rw-rw-   0        0        0     3805 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Operation.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.277572 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Operation_/
+-rw-rw-rw-   0        0        0     2805 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Operation_/Bit.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.304501 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/
+-rw-rw-rw-   0        0        0     1052 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/Condition.py
+-rw-rw-rw-   0        0        0     1653 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/Enable.py
+-rw-rw-rw-   0        0        0     1030 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/Event.py
+-rw-rw-rw-   0        0        0     1687 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/Ntransition.py
+-rw-rw-rw-   0        0        0     1687 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/Ptransition.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Operation_/__init__.py
+-rw-rw-rw-   0        0        0     3895 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Questionable.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.312479 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Questionable_/
+-rw-rw-rw-   0        0        0     2805 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Questionable_/Bit.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.343396 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/
+-rw-rw-rw-   0        0        0     1061 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/Condition.py
+-rw-rw-rw-   0        0        0     1660 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/Enable.py
+-rw-rw-rw-   0        0        0     1039 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/Event.py
+-rw-rw-rw-   0        0        0     1705 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/Ntransition.py
+-rw-rw-rw-   0        0        0     1705 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/Ptransition.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Questionable_/__init__.py
+-rw-rw-rw-   0        0        0     1282 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Queue.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/__init__.py
+-rw-rw-rw-   0        0        0    11912 2021-05-16 18:22:14.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.438145 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/
+-rw-rw-rw-   0        0        0     3096 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.482026 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/
+-rw-rw-rw-   0        0        0     7286 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Device.py
+-rw-rw-rw-   0        0        0     4431 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Display.py
+-rw-rw-rw-   0        0        0     1023 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/IpSet.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.491004 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/IpSet_/
+-rw-rw-rw-   0        0        0     1031 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/IpSet_/SubMonitor.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.498981 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/IpSet_/SubMonitor_/
+-rw-rw-rw-   0        0        0     1049 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/IpSet_/SubMonitor_/Refresh.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/IpSet_/SubMonitor_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/IpSet_/__init__.py
+-rw-rw-rw-   0        0        0     1511 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Option.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.517931 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Option_/
+-rw-rw-rw-   0        0        0     1673 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Option_/Description.py
+-rw-rw-rw-   0        0        0     2558 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Option_/ListPy.py
+-rw-rw-rw-   0        0        0     1742 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Option_/Version.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Option_/__init__.py
+-rw-rw-rw-   0        0        0     1479 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Password.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.526907 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Password_/
+-rw-rw-rw-   0        0        0     1567 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Password_/Cenable.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Password_/__init__.py
+-rw-rw-rw-   0        0        0     1471 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Reference.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.544859 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Reference_/
+-rw-rw-rw-   0        0        0      975 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Reference_/Dc.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.554833 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Reference_/Dc_/
+-rw-rw-rw-   0        0        0     1207 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Reference_/Dc_/Offset.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Reference_/Dc_/__init__.py
+-rw-rw-rw-   0        0        0     3738 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Reference_/Frequency.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.562811 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Reference_/Frequency_/
+-rw-rw-rw-   0        0        0     1013 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Reference_/Frequency_/Advanced.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.572785 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Reference_/Frequency_/Advanced_/
+-rw-rw-rw-   0        0        0     1995 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Reference_/Frequency_/Advanced_/Source.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Reference_/Frequency_/Advanced_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Reference_/Frequency_/__init__.py
+-rw-rw-rw-   0        0        0     1168 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Reference_/Phase.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Reference_/__init__.py
+-rw-rw-rw-   0        0        0     1845 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Ssync.py
+-rw-rw-rw-   0        0        0     2248 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/StIcon.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/__init__.py
+-rw-rw-rw-   0        0        0     1843 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Cmw.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.582758 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Cmw_/
+-rw-rw-rw-   0        0        0     1166 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Cmw_/Device.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.596721 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Cmw_/Device_/
+-rw-rw-rw-   0        0        0     1042 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Cmw_/Device_/Id.py
+-rw-rw-rw-   0        0        0     1060 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Cmw_/Device_/Vi.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Cmw_/Device_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Cmw_/__init__.py
+-rw-rw-rw-   0        0        0     2350 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.633623 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/
+-rw-rw-rw-   0        0        0     2117 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Gpib.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.647589 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/
+-rw-rw-rw-   0        0        0     1202 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/Self.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.663542 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/Self_/
+-rw-rw-rw-   0        0        0     1796 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/Self_/Addr.py
+-rw-rw-rw-   0        0        0     1798 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/Self_/Enable.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/Self_/__init__.py
+-rw-rw-rw-   0        0        0     1135 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/Vresource.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/__init__.py
+-rw-rw-rw-   0        0        0     1936 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Hislip.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.672519 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Hislip_/
+-rw-rw-rw-   0        0        0     1193 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Hislip_/Vresource.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Hislip_/__init__.py
+-rw-rw-rw-   0        0        0     6239 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Net.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.686483 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Net_/
+-rw-rw-rw-   0        0        0     2372 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Net_/Dns.py
+-rw-rw-rw-   0        0        0     1743 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Net_/Subnet.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Net_/__init__.py
+-rw-rw-rw-   0        0        0     1902 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Rsib.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.695457 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Rsib_/
+-rw-rw-rw-   0        0        0     1135 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Rsib_/Vresource.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Rsib_/__init__.py
+-rw-rw-rw-   0        0        0     2370 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Socket.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.713409 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Socket_/
+-rw-rw-rw-   0        0        0     2231 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Socket_/Mode.py
+-rw-rw-rw-   0        0        0     1886 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Socket_/Port.py
+-rw-rw-rw-   0        0        0     1201 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Socket_/Vresource.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Socket_/__init__.py
+-rw-rw-rw-   0        0        0      804 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Usb.py
+-rw-rw-rw-   0        0        0     2091 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Vxi.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.727372 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Vxi_/
+-rw-rw-rw-   0        0        0     1824 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Vxi_/Gtr.py
+-rw-rw-rw-   0        0        0     1154 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Vxi_/Vresource.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Vxi_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/__init__.py
+-rw-rw-rw-   0        0        0     1053 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Connector.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.734353 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Connector_/
+-rw-rw-rw-   0        0        0     1494 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Connector_/Translation.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Connector_/__init__.py
+-rw-rw-rw-   0        0        0     4086 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Date.py
+-rw-rw-rw-   0        0        0      793 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Device.py
+-rw-rw-rw-   0        0        0     1219 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/DeviceFootprint.py
+-rw-rw-rw-   0        0        0     1713 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Display.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.744327 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Display_/
+-rw-rw-rw-   0        0        0     1340 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Display_/Monitor.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.755298 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Display_/Monitor_/
+-rw-rw-rw-   0        0        0      983 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Display_/Monitor_/Off.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Display_/Monitor_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Display_/__init__.py
+-rw-rw-rw-   0        0        0     3084 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Error.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.763276 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Error_/
+-rw-rw-rw-   0        0        0     1411 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Error_/Code.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Error_/__init__.py
+-rw-rw-rw-   0        0        0      989 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Generator.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.772252 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Generator_/
+-rw-rw-rw-   0        0        0      955 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Generator_/All.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.780233 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Generator_/All_/
+-rw-rw-rw-   0        0        0     1053 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Generator_/All_/Off.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Generator_/All_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Generator_/__init__.py
+-rw-rw-rw-   0        0        0     1453 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Help.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.797186 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Help_/
+-rw-rw-rw-   0        0        0      994 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Help_/Headers.py
+-rw-rw-rw-   0        0        0     1124 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Help_/Status.py
+-rw-rw-rw-   0        0        0     1118 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Help_/Syntax.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Help_/__init__.py
+-rw-rw-rw-   0        0        0     1001 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Measurement.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.807160 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Measurement_/
+-rw-rw-rw-   0        0        0      955 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Measurement_/All.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.815139 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Measurement_/All_/
+-rw-rw-rw-   0        0        0     1065 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Measurement_/All_/Off.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Measurement_/All_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Measurement_/__init__.py
+-rw-rw-rw-   0        0        0      983 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Password.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.825112 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Password_/
+-rw-rw-rw-   0        0        0     1060 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Password_/New.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Password_/__init__.py
+-rw-rw-rw-   0        0        0      987 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Record.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.832092 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Record_/
+-rw-rw-rw-   0        0        0      975 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Record_/Macro.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.841068 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Record_/Macro_/
+-rw-rw-rw-   0        0        0     1584 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Record_/Macro_/File.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Record_/Macro_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Record_/__init__.py
+-rw-rw-rw-   0        0        0     1017 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Routing.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.850044 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Routing_/
+-rw-rw-rw-   0        0        0     1086 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Routing_/Possible.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Routing_/__init__.py
+-rw-rw-rw-   0        0        0      989 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Signaling.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.860019 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Signaling_/
+-rw-rw-rw-   0        0        0      955 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Signaling_/All.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.868994 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Signaling_/All_/
+-rw-rw-rw-   0        0        0     1053 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Signaling_/All_/Off.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Signaling_/All_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Signaling_/__init__.py
+-rw-rw-rw-   0        0        0     1013 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/SingleCmw.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.878967 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/SingleCmw_/
+-rw-rw-rw-   0        0        0      739 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/SingleCmw_/Device.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/SingleCmw_/__init__.py
+-rw-rw-rw-   0        0        0     1009 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Startup.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.889938 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Startup_/
+-rw-rw-rw-   0        0        0     1116 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Startup_/Prepare.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Startup_/__init__.py
+-rw-rw-rw-   0        0        0     5125 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Time.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.901906 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Time_/
+-rw-rw-rw-   0        0        0     2541 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Time_/DaylightSavingTime.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.909885 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Time_/DaylightSavingTime_/
+-rw-rw-rw-   0        0        0     2490 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Time_/DaylightSavingTime_/Rule.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Time_/DaylightSavingTime_/__init__.py
+-rw-rw-rw-   0        0        0     1595 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Time_/HrTimer.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.918861 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Time_/HrTimer_/
+-rw-rw-rw-   0        0        0     2300 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Time_/HrTimer_/Absolute.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.928835 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Time_/HrTimer_/Absolute_/
+-rw-rw-rw-   0        0        0     2990 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Time_/HrTimer_/Absolute_/Set.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Time_/HrTimer_/Absolute_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Time_/HrTimer_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Time_/__init__.py
+-rw-rw-rw-   0        0        0     1406 2021-05-16 18:22:15.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Update.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/__init__.py
+-rw-rw-rw-   0        0        0      988 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.936814 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/
+-rw-rw-rw-   0        0        0      980 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.944792 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/
+-rw-rw-rw-   0        0        0     1210 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:20.958754 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/
+-rw-rw-rw-   0        0        0     1962 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/Display.py
+-rw-rw-rw-   0        0        0     4194 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:21.013608 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/
+-rw-rw-rw-   0        0        0     1041 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Dexecution.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:21.023583 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Dexecution_/
+-rw-rw-rw-   0        0        0     1756 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Dexecution_/Duration.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Dexecution_/__init__.py
+-rw-rw-rw-   0        0        0     1663 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Enable.py
+-rw-rw-rw-   0        0        0     3053 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/FilterPy.py
+-rw-rw-rw-   0        0        0     1897 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/FormatPy.py
+-rw-rw-rw-   0        0        0     1690 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Functions.py
+-rw-rw-rw-   0        0        0     1722 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Name.py
+-rw-rw-rw-   0        0        0     1663 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Parser.py
+-rw-rw-rw-   0        0        0     1636 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Rpc.py
+-rw-rw-rw-   0        0        0     1661 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Size.py
+-rw-rw-rw-   0        0        0     1927 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/StartMode.py
+-rw-rw-rw-   0        0        0     1907 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/StopMode.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/__init__.py
+-rw-rw-rw-   0        0        0      984 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger.py
+-rw-rw-rw-   0        0        0      893 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/TriggerInvoke.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:21.030563 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/
+-rw-rw-rw-   0        0        0     1661 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:21.053502 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/
+-rw-rw-rw-   0        0        0     2029 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/Eout.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:21.066467 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/
+-rw-rw-rw-   0        0        0     1005 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/Catalog.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:21.075444 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/Catalog_/
+-rw-rw-rw-   0        0        0     1081 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/Catalog_/Source.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/Catalog_/__init__.py
+-rw-rw-rw-   0        0        0     1625 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/Source.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/__init__.py
+-rw-rw-rw-   0        0        0     4136 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/ExtA.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:21.084420 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/ExtA_/
+-rw-rw-rw-   0        0        0      921 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/ExtA_/Catalog.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/ExtA_/__init__.py
+-rw-rw-rw-   0        0        0     4136 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/ExtB.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:21.094393 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/ExtB_/
+-rw-rw-rw-   0        0        0      921 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/ExtB_/Catalog.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/ExtB_/__init__.py
+-rw-rw-rw-   0        0        0     1864 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/Uinitiated.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:21.104367 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/Uinitiated_/
+-rw-rw-rw-   0        0        0     1604 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/Uinitiated_/Execute.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/Uinitiated_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/__init__.py
+-rw-rw-rw-   0        0        0    11186 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Unit.py
+-rw-rw-rw-   0        0        0      987 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Write.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:21.114340 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Write_/
+-rw-rw-rw-   0        0        0      979 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Write_/Eeprom.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:21.123316 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Write_/Eeprom_/
+-rw-rw-rw-   0        0        0      972 2021-05-16 18:22:16.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Write_/Eeprom_/Data.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Write_/Eeprom_/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Write_/__init__.py
+-rw-rw-rw-   0        0        0        0 2019-11-18 07:28:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:21.273916 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/
+-rw-rw-rw-   0        0        0      541 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/ArgLinkedEventArgs.py
+-rw-rw-rw-   0        0        0     4003 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/ArgSingle.py
+-rw-rw-rw-   0        0        0     1061 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/ArgSingleList.py
+-rw-rw-rw-   0        0        0     1000 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/ArgSingleSuppressed.py
+-rw-rw-rw-   0        0        0     9026 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/ArgStringComposer.py
+-rw-rw-rw-   0        0        0     5624 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/ArgStruct.py
+-rw-rw-rw-   0        0        0     3354 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/ArgStructList.py
+-rw-rw-rw-   0        0        0     2446 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/ArgStructStringParser.py
+-rw-rw-rw-   0        0        0     5176 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/CommandsGroup.py
+-rw-rw-rw-   0        0        0    20227 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/Conversions.py
+-rw-rw-rw-   0        0        0     3618 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/ConverterFromScpiString.py
+-rw-rw-rw-   0        0        0     4409 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/ConverterToScpiString.py
+-rw-rw-rw-   0        0        0    10299 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/Core.py
+-rw-rw-rw-   0        0        0    38340 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/Instrument.py
+-rw-rw-rw-   0        0        0     3918 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/InstrumentErrors.py
+-rw-rw-rw-   0        0        0     2081 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/InstrumentOptions.py
+-rw-rw-rw-   0        0        0     5101 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/InstrumentSettings.py
+-rw-rw-rw-   0        0        0     3380 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/InternalLinker.py
+-rw-rw-rw-   0        0        0     4331 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/IoTransferEventArgs.py
+-rw-rw-rw-   0        0        0     3841 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/RepeatedCapability.py
+-rw-rw-rw-   0        0        0     4719 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/StreamReader.py
+-rw-rw-rw-   0        0        0     4938 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/StreamWriter.py
+-rw-rw-rw-   0        0        0     1040 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/StructBase.py
+-rw-rw-rw-   0        0        0     2893 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/Types.py
+-rw-rw-rw-   0        0        0     4530 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/Utilities.py
+-rw-rw-rw-   0        0        0     4850 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/VisaPluginSocketIo.py
+-rw-rw-rw-   0        0        0    44232 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/VisaSession.py
+-rw-rw-rw-   0        0        0     6999 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/VisaSessionSim.py
+-rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/__init__.py
+-rw-rw-rw-   0        0        0    16335 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/RsCMPX_Base.py
+-rw-rw-rw-   0        0        0      823 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/__init__.py
+-rw-rw-rw-   0        0        0    11436 2021-05-16 18:22:11.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/enums.py
+-rw-rw-rw-   0        0        0     5833 2021-05-16 18:22:11.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base/repcap.py
+drwxrwxrwx   0        0        0        0 2021-05-16 18:22:18.355197 RsCMPX_Base-4.0.7.9/RsCMPX_Base.egg-info/
+-rw-rw-rw-   0        0        0     2474 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    36887 2021-05-16 18:22:18.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/RsCMPX_Base.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-05-16 18:22:21.284885 RsCMPX_Base-4.0.7.9/setup.cfg
+-rw-rw-rw-   0        0        0      856 2021-05-16 18:22:17.000000 RsCMPX_Base-4.0.7.9/setup.py
```

### Comparing `RsCMPX_Base-4.0.7.8/PKG-INFO` & `RsCMPX_Base-4.0.7.9/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,47 @@
-Metadata-Version: 2.1
-Name: RsCMPX_Base
-Version: 4.0.7.8
-Summary: CMX/CMP Base System Remote-control Module
-Home-page: UNKNOWN
-Author: Rohde & Schwarz GmbH & Co. KG
-Author-email: Customer.Support@rohde-schwarz.com
-License: MIT
-Description: Rohde & Schwarz CMX/CMP Base System RsCMPX_Base instrument driver Version 4.0.7.8
-        
-        Check out the module documentation on https://RsCMPX_Base.readthedocs.io/
-        
-        --------------------------------------------------------------------------------
-        
-        Currently supported CMX/CMP subsystems:
-        
-        - Base: `RsCmpx_Base <https://RsCmpx_Base.readthedocs.io/>`_
-        - GPRF: `RsCmpx_Gprf <https://RsCmpx_Gprf.readthedocs.io/>`_
-        - LTE Measurement: `RsCmpx_LteMeas <https://RsCmpx_LteMeas.readthedocs.io/>`_
-        - New Radio FR1 Measurement: `RsCmpx_NrFr1Meas <https://RsCmpx_NrFr1Meas.readthedocs.io/>`_
-        - New Radio FR2 Measurement: `RsCmpx_NrFr2Meas <https://RsCmpx_NrFr2Meas.readthedocs.io/>`_
-        - CMP Ultra Wideband Measurement: `RsCMPX_UwbMeas <https://RsCMPX_UwbMeas.readthedocs.io/>`_
-        - CMX/P Signaling: `RsCMX_Signaling <https://RsCMX_Signaling.readthedocs.io/>`_
-        
-        In case you require support for more subsystems, please contact our customer support on customersupport@rohde-schwarz.com
-        with the topic "Auto-generated Python drivers" in the email subject. This will speed up the response process
-        
-        --------------------------------------------------------------------------------
-        
-        Release Notes: for the whole RsCmpx_xxx group:
-        
-        Latest release notes summary: Added documentation on ReadTheDocs.io
-        
-        Version 4.0.7.4
-        
-        - Added documentation on ReadTheDocs.io
-        
-        Version 4.0.7.3
-        
-        - Added new subsystems NrFr2Meas, UwbMeas, Signaling
-        
-        Version 4.0.7.2
-        
-        - Added new UDF integer number recognition
-        - Added RsCMPX_Gprf
-        
-        Version 4.0.7.1
-        
-        - First released version
-        
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/markdown
+Rohde & Schwarz CMX/CMP Base System RsCMPX_Base instrument driver.
+
+Supported instruments: CMX500, CMP200
+
+The package is hosted here: https://pypi.org/project/RsCMPX_Base/
+
+Documentation: https://RsCMPX_Base.readthedocs.io/
+
+Examples: https://github.com/Rohde-Schwarz/Examples/
+
+--------------------------------------------------------------------------------
+
+Currently supported CMX/CMP subsystems:
+
+- Base: `RsCmpx_Base <https://RsCmpx_Base.readthedocs.io/>`_
+- GPRF: `RsCmpx_Gprf <https://RsCmpx_Gprf.readthedocs.io/>`_
+- LTE Measurement: `RsCmpx_LteMeas <https://RsCmpx_LteMeas.readthedocs.io/>`_
+- New Radio FR1 Measurement: `RsCmpx_NrFr1Meas <https://RsCmpx_NrFr1Meas.readthedocs.io/>`_
+- New Radio FR2 Measurement: `RsCmpx_NrFr2Meas <https://RsCmpx_NrFr2Meas.readthedocs.io/>`_
+- CMP Ultra Wideband Measurement: `RsCMPX_UwbMeas <https://RsCMPX_UwbMeas.readthedocs.io/>`_
+- CMX/P Signaling: `RsCMX_Signaling <https://RsCMX_Signaling.readthedocs.io/>`_
+
+In case you require support for more subsystems, please contact our customer support on customersupport@rohde-schwarz.com
+with the topic "Auto-generated Python drivers" in the email subject. This will speed up the response process
+
+--------------------------------------------------------------------------------
+
+Release Notes: for the whole RsCmpx_xxx group:
+
+Latest release notes summary: Added documentation on ReadTheDocs
+
+Version 4.0.7.4
+
+- Added documentation on ReadTheDocs
+
+Version 4.0.7.3
+
+- Added new subsystems NrFr2Meas, UwbMeas, Signaling
+
+Version 4.0.7.2
+
+- Added new UDF integer number recognition
+- Added RsCMPX_Gprf
+
+Version 4.0.7.1
+
+- First released version
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/CustomFiles/events.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/CustomFiles/events.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,23 +17,37 @@
 	@io_events_include_data.setter
 	def io_events_include_data(self, value: bool) -> None:
 		"""If True, the on_write and on_read events include also the sent/received data.
 		Default value is False, to avoid handling potentially big data."""
 		self._core.io.io_events_include_data = value
 
 	@property
+	def before_write_handler(self) -> Callable:
+		"""Returns the handler of before_write events. \n
+		:return: current before_write_handler"""
+		return self._core.io.before_write_handler
+
+	@before_write_handler.setter
+	def before_write_handler(self, handler: Callable) -> None:
+		"""Sets handler for before_write events.
+		The before_write event is invoked before each write operation (only once, not for every chunk)
+		Event prototype: handler(io: Instrument, cmd: str)
+		:param handler: new handler"""
+		self._core.io.before_write_handler = handler
+
+	@property
 	def on_write_handler(self) -> Callable:
 		"""Returns the handler of on_write events. \n
 		:return: current on_write_handler"""
 		return self._core.io.on_write_handler
 
 	@on_write_handler.setter
 	def on_write_handler(self, handler: Callable) -> None:
 		"""Sets handler for on_write events.
-		The on_write event is invoked every time the driver performs a write operation to the instrument.
+		The on_write event is invoked every time the driver performs a write operation to the instrument (for each write chunk)
 		Event arguments type: IoTransferEventArgs
 		By default, the event_args do not contain the actual data sent. If you wish to receive them, set the driver.Events.io_events_include_data to True \n
 		:param handler: new handler for all write operations"""
 		self._core.io.on_write_handler = handler
 
 	@property
 	def on_read_handler(self) -> Callable:
@@ -45,7 +59,21 @@
 	def on_read_handler(self, handler: Callable) -> None:
 		"""Sets handler for on_read events.
 		The on_read event is invoked every time the driver performs a read operation to the instrument.
 		Event arguments type: IoTransferEventArgs
 		By default, the event_args do not contain the actual data sent. If you wish to receive them, set the driver.Events.io_events_include_data to True \n
 		:param handler: new handler for all read operations"""
 		self._core.io.on_read_handler = handler
+
+	@property
+	def before_query_handler(self) -> Callable:
+		"""Returns the handler of before_query events. \n
+		:return: current before_query_handler"""
+		return self._core.io.before_query_handler
+
+	@before_query_handler.setter
+	def before_query_handler(self, handler: Callable) -> None:
+		"""Sets handler for before_query events.
+		The before_query event is invoked before each query operation (only once, not for every chunk)
+		Event prototype: handler(io: Instrument, query: str)
+		:param handler: new handler"""
+		self._core.io.before_query_handler = handler
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/CustomFiles/reliability.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/CustomFiles/reliability.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-import time
-from typing import Callable
-
-from ..Internal import ArgLinkedEventArgs
-from ..Internal import Core
-
-codes_table = {
-				0:       'OK',
-				1:       'Measurement Timeout',
-				2:       'Capture Buffer Overflow',
-				3:       'Over-driven',
-				4:       'Under-driven',
-				6:       'Trigger Timeout',
-				7:       'Acquisition Error',
-				8:       'Sync Error',
-				9:       'Uncalibrated',
-				15:      'Reference Frequency Error',
-				16:      'RF Not Available',
-				17:      'RF Level not Settled',
-				18:      'RF Frequency not Settled',
-				19:      'Call not Established',
-				20:      'Call Type not Usable',
-				21:      'Call Lost',
-				23:      'Missing Option',
-				24:      'Invalid RF Setting',
-				26:      'Resource Conflict',
-				27:      'No Sensor Connected',
-				28:      'Unexpected Parameter Change',
-				30:      'File not Found',
-				31:      'No DTM reply',
-				32:      'ACL Disconnected',
-				40:      'ARB File CRC Error',
-				42:      'ARB Header Tag Invalid',
-				43:      'ARB Segment Overflow',
-				44:      'ARB File not Found',
-				45:      'ARB Memory Overflow',
-				46:      'ARB Sample Rate out of Range',
-				47:      'ARB Cycles out of Range',
-				50:      'Startup Error',
-				51:      'No Reply',
-				52:      'Connection Error',
-				53:      'Configuration Error',
-				54:      'Filesystem Error',
-				60:      'Invalid RF-Connector Setting',
-				93:      'OCXO Oven Temperature too low',
-				101:     'Firmware Error',
-				102:     'Unidentified Error',
-				103:     'Parameter Error',
-				104:     'Not Functional'}
-
-
-class ReliabilityEventArgs:
-	"""Arguments for reliability indicator event."""
-
-	def __init__(self, timestamp, code: int, message: str, context: str):
-		self.timestamp = timestamp
-		self.message = message
-		self.code = code
-		self.message = message
-		self.context = context
-
-
-class Reliability:
-	"""Reliability class that handles all the necessary tasks related to reliability indicator."""
-
-	def __init__(self, core: Core):
-		self._core = core
-		self._last_value = 0
-		self._last_context = ''
-		self._last_timestamp = None
-		self._exception_on_error = False
-		# noinspection PyTypeChecker
-		self._on_update_handler: Callable = None
-		self._core.set_link_handler('Reliability', self._permanent_on_update_handler)
-
-	@property
-	def last_value(self):
-		"""Returns the last updated Reliability code."""
-		return self._last_value
-
-	@property
-	def last_context(self) -> str:
-		"""Returns the last updated Context of the reliability code - usually the SCPI query on which the instrument responded with the Reliability code."""
-		return self._last_context
-
-	@property
-	def last_timestamp(self) -> time:
-		"""Returns the time of the last Reliability update."""
-		return self._last_timestamp
-
-	@property
-	def last_message(self) -> str:
-		"""Returns the LastValue of the reliability table converted to human-readable string."""
-		if self._last_value in codes_table:
-			return codes_table[self._last_value]
-		else:
-			return f'Undefined reliability code {self._last_value}.'
-
-	@property
-	def exception_on_error(self) -> bool:
-		"""see the exception_on_error.setter."""
-		return self._exception_on_error
-
-	@exception_on_error.setter
-	def exception_on_error(self, value) -> None:
-		"""If True, (default is False) the object throws an exception if the updated reliability is not 0 (non-OK)."""
-		self._exception_on_error = value
-
-	def on_update_handler(self, handler: Callable) -> None:
-		"""Register the handler for on_update event.
-		This handler is invoked with each update of the reliability indicator.
-		Handler API: handler(event_args: ReliabilityEventArgs)"""
-		self._on_update_handler = handler
-
-	def _permanent_on_update_handler(self, event_args: ArgLinkedEventArgs):
-		"""Permanent on_update handler. Takes care of updating all the 'last_xxx' values and calling a user-defined updated_handler."""
-		self._last_value = int(str(event_args.value))
-		self._last_context = event_args.context
-		self._last_timestamp = event_args.timestamp
-
-		if self._on_update_handler:
-			# Call the additional handler if registered
-			rel_events_args = ReliabilityEventArgs(self._last_timestamp, self._last_value, self.last_message, self._last_context)
-			self._on_update_handler(rel_events_args)
-
-		if self._exception_on_error and self._last_value != 0:
-			raise Exception(
-				f'Reliability indicator error. Time: {time.strftime("%H:%M:%S", time.localtime(self._last_timestamp))}, '
-				f'Context: {self._last_context}, Value {self._last_value}: {self.last_message}')
+import time
+from typing import Callable
+
+from ..Internal import ArgLinkedEventArgs
+from ..Internal import Core
+
+codes_table = {
+				0:       'OK',
+				1:       'Measurement Timeout',
+				2:       'Capture Buffer Overflow',
+				3:       'Over-driven',
+				4:       'Under-driven',
+				6:       'Trigger Timeout',
+				7:       'Acquisition Error',
+				8:       'Sync Error',
+				9:       'Uncalibrated',
+				15:      'Reference Frequency Error',
+				16:      'RF Not Available',
+				17:      'RF Level not Settled',
+				18:      'RF Frequency not Settled',
+				19:      'Call not Established',
+				20:      'Call Type not Usable',
+				21:      'Call Lost',
+				23:      'Missing Option',
+				24:      'Invalid RF Setting',
+				26:      'Resource Conflict',
+				27:      'No Sensor Connected',
+				28:      'Unexpected Parameter Change',
+				30:      'File not Found',
+				31:      'No DTM reply',
+				32:      'ACL Disconnected',
+				40:      'ARB File CRC Error',
+				42:      'ARB Header Tag Invalid',
+				43:      'ARB Segment Overflow',
+				44:      'ARB File not Found',
+				45:      'ARB Memory Overflow',
+				46:      'ARB Sample Rate out of Range',
+				47:      'ARB Cycles out of Range',
+				50:      'Startup Error',
+				51:      'No Reply',
+				52:      'Connection Error',
+				53:      'Configuration Error',
+				54:      'Filesystem Error',
+				60:      'Invalid RF-Connector Setting',
+				93:      'OCXO Oven Temperature too low',
+				101:     'Firmware Error',
+				102:     'Unidentified Error',
+				103:     'Parameter Error',
+				104:     'Not Functional'}
+
+
+class ReliabilityEventArgs:
+	"""Arguments for reliability indicator event."""
+
+	def __init__(self, timestamp, code: int, message: str, context: str):
+		self.timestamp = timestamp
+		self.message = message
+		self.code = code
+		self.message = message
+		self.context = context
+
+
+class Reliability:
+	"""Reliability class that handles all the necessary tasks related to reliability indicator."""
+
+	def __init__(self, core: Core):
+		self._core = core
+		self._last_value = 0
+		self._last_context = ''
+		self._last_timestamp = None
+		self._exception_on_error = False
+		# noinspection PyTypeChecker
+		self._on_update_handler: Callable = None
+		self._core.set_link_handler('Reliability', self._permanent_on_update_handler)
+
+	@property
+	def last_value(self):
+		"""Returns the last updated Reliability code."""
+		return self._last_value
+
+	@property
+	def last_context(self) -> str:
+		"""Returns the last updated Context of the reliability code - usually the SCPI query on which the instrument responded with the Reliability code."""
+		return self._last_context
+
+	@property
+	def last_timestamp(self) -> time:
+		"""Returns the time of the last Reliability update."""
+		return self._last_timestamp
+
+	@property
+	def last_message(self) -> str:
+		"""Returns the LastValue of the reliability table converted to human-readable string."""
+		if self._last_value in codes_table:
+			return codes_table[self._last_value]
+		else:
+			return f'Undefined reliability code {self._last_value}.'
+
+	@property
+	def exception_on_error(self) -> bool:
+		"""see the exception_on_error.setter."""
+		return self._exception_on_error
+
+	@exception_on_error.setter
+	def exception_on_error(self, value) -> None:
+		"""If True, (default is False) the object throws an exception if the updated reliability is not 0 (non-OK)."""
+		self._exception_on_error = value
+
+	def on_update_handler(self, handler: Callable) -> None:
+		"""Register the handler for on_update event.
+		This handler is invoked with each update of the reliability indicator.
+		Handler API: handler(event_args: ReliabilityEventArgs)"""
+		self._on_update_handler = handler
+
+	def _permanent_on_update_handler(self, event_args: ArgLinkedEventArgs):
+		"""Permanent on_update handler. Takes care of updating all the 'last_xxx' values and calling a user-defined updated_handler."""
+		self._last_value = int(str(event_args.value))
+		self._last_context = event_args.context
+		self._last_timestamp = event_args.timestamp
+
+		if self._on_update_handler:
+			# Call the additional handler if registered
+			rel_events_args = ReliabilityEventArgs(self._last_timestamp, self._last_value, self.last_message, self._last_context)
+			self._on_update_handler(rel_events_args)
+
+		if self._exception_on_error and self._last_value != 0:
+			raise Exception(
+				f'Reliability indicator error. Time: {time.strftime("%H:%M:%S", time.localtime(self._last_timestamp))}, '
+				f'Context: {self._last_context}, Value {self._last_value}: {self.last_message}')
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/CustomFiles/utilities.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/CustomFiles/utilities.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,18 +48,19 @@
 		return self._core.io.firmware_version
 
 	@property
 	def instrument_serial_number(self) -> str:
 		"""Returns instrument's serial_number."""
 		return self._core.io.serial_number
 
-	def query_opc(self) -> int:
+	def query_opc(self, timeout: int = 0) -> int:
 		"""SCPI command: *OPC?
-		Queries the instrument's OPC bit and hence it waits until the instrument reports operation complete."""
-		return self._core.io.query_opc()
+		Queries the instrument's OPC bit and hence it waits until the instrument reports operation complete.
+		If you define timeout > 0, the VISA timeout is set to that value just for this method call."""
+		return self._core.io.query_opc(timeout)
 
 	@property
 	def instrument_status_checking(self) -> bool:
 		"""See the instrument_status_checking.setter."""
 		return self._core.io.query_instr_status
 
 	@instrument_status_checking.setter
@@ -175,14 +176,19 @@
 		Stops further commands processing until all commands sent before *WAI have been executed."""
 		return self._core.io.write('*WAI')
 
 	def write_str(self, cmd: str) -> None:
 		"""Writes the command to the instrument."""
 		self._core.io.write(cmd)
 
+	def write(self, cmd: str) -> None:
+		"""This method is an alias to the write_str().
+		Writes the command to the instrument as string."""
+		self._core.io.write(cmd)
+
 	def write_int(self, cmd: str, param: int) -> None:
 		"""Writes the command to the instrument followed by the integer parameter:
 		e.g.: cmd = 'SELECT:INPUT' param = '2', result command = 'SELECT:INPUT 2'"""
 		self._core.io.write(f'{cmd} {param}')
 
 	def write_int_with_opc(self, cmd: str, param: int, timeout: int = None) -> None:
 		"""Writes the command with OPC to the instrument followed by the integer parameter:
@@ -213,14 +219,20 @@
 		self._core.io.write_with_opc(f'{cmd} {Conv.bool_to_str(param)}', timeout)
 
 	def query_str(self, query: str) -> str:
 		"""Sends the query to the instrument and returns the response as string.
 		The response is trimmed of any trailing LF characters and has no length limit."""
 		return self._core.io.query_str(query)
 
+	def query(self, query: str) -> str:
+		"""This method is an alias to the query_str().
+		Sends the query to the instrument and returns the response as string.
+		The response is trimmed of any trailing LF characters and has no length limit."""
+		return self._core.io.query_str(query)
+
 	def query_bool(self, query: str) -> bool:
 		"""Sends the query to the instrument and returns the response as boolean."""
 		return self._core.io.query_bool(query)
 
 	def query_int(self, query: str) -> int:
 		"""Sends the query to the instrument and returns the response as integer."""
 		return self._core.io.query_int(query)
@@ -230,20 +242,33 @@
 		return self._core.io.query_float(query)
 
 	def write_str_with_opc(self, cmd: str, timeout: int = None) -> None:
 		"""Writes the opc-synced command to the instrument.
 		If you do not provide timeout, the method uses current opc_timeout."""
 		self._core.io.write_with_opc(cmd, timeout)
 
+	def write_with_opc(self, cmd: str, timeout: int = None) -> None:
+		"""This method is an alias to the write_str_with_opc().
+		Writes the opc-synced command to the instrument.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		self._core.io.write_with_opc(cmd, timeout)
+
 	def query_str_with_opc(self, query: str, timeout: int = None) -> str:
 		"""Sends the opc-synced query to the instrument and returns the response as string.
 		The response is trimmed of any trailing LF characters and has no length limit.
 		If you do not provide timeout, the method uses current opc_timeout."""
 		return self._core.io.query_str_with_opc(query, timeout)
 
+	def query_with_opc(self, query: str, timeout: int = None) -> str:
+		"""This method is an alias to the query_str_with_opc().
+		Sends the opc-synced query to the instrument and returns the response as string.
+		The response is trimmed of any trailing LF characters and has no length limit.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		return self._core.io.query_str_with_opc(query, timeout)
+
 	def query_bool_with_opc(self, query: str, timeout: int = None) -> bool:
 		"""Sends the opc-synced query to the instrument and returns the response as boolean.
 		If you do not provide timeout, the method uses current opc_timeout."""
 		return self._core.io.query_bool_with_opc(query, timeout)
 
 	def query_int_with_opc(self, query: str, timeout: int = None) -> int:
 		"""Sends the opc-synced query to the instrument and returns the response as integer.
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Buffer.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Buffer.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,24 +74,24 @@
 		Snippet: driver.base.buffer.clear(buffer = '1') \n
 		Clears the contents of a buffer. You get an empty buffer that you can fill with new commands. \n
 			:param buffer: No help available
 		"""
 		param = Conversions.value_to_quoted_str(buffer)
 		self._core.io.write(f'CLEar:BASE:BUFFer {param}')
 
-	def fetch(self, buffer: str, lineno: int) -> str:
+	def fetch(self, buffer: str, line_number: int) -> str:
 		"""SCPI: FETCh:BASE:BUFFer \n
-		Snippet: value: str = driver.base.buffer.fetch(buffer = '1', lineno = 1) \n
+		Snippet: value: str = driver.base.buffer.fetch(buffer = '1', line_number = 1) \n
 		Reads the contents of a buffer line. Buffer contents are stored line by line. Every query generates a new buffer line.
 		The queries are not stored together with the results. Reading buffer contents is non-destructive. The lines can be read
 		in arbitrary order. \n
 			:param buffer: No help available
-			:param lineno: Line number, selects the line to be read.
+			:param line_number: Line number, selects the line to be read.
 			:return: line: Returned line contents."""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('buffer', buffer, DataType.String), ArgSingle('lineno', lineno, DataType.Integer))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('buffer', buffer, DataType.String), ArgSingle('line_number', line_number, DataType.Integer))
 		response = self._core.io.query_str(f'FETCh:BASE:BUFFer? {param}'.rstrip())
 		return trim_str_response(response)
 
 	def clone(self) -> 'Buffer':
 		"""Clones the group by creating new object from it and its whole existing sub-groups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Buffer_/LineCount.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Buffer_/LineCount.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Slot.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Slot.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Slot_/RxFilter.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Slot_/RxFilter.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Slot_/TxFilter.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Slot_/TxFilter.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/State.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected_/Slot.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected_/Slot.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected_/Slot_/RxFilter.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected_/Slot_/RxFilter.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected_/Slot_/TxFilter.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Corrected_/Slot_/TxFilter.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected_/Slot.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected_/Slot.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected_/Slot_/RxFilter.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected_/Slot_/RxFilter.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected_/Slot_/TxFilter.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Gdelay_/Uncorrected_/Slot_/TxFilter.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected_/Slot.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected_/Slot.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected_/Slot_/RxFilter.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected_/Slot_/RxFilter.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected_/Slot_/TxFilter.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Corrected_/Slot_/TxFilter.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected_/Slot.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected_/Slot.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected_/Slot_/RxFilter.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected_/Slot_/RxFilter.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected_/Slot_/TxFilter.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Correction_/IfEqualizer_/Trace_/Magnitude_/Uncorrected_/Slot_/TxFilter.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Ipc.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Ipc.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Ipc_/Result.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Ipc_/Result.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/MultiCmw.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/MultiCmw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/MultiCmw_/Identify.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/MultiCmw_/Identify.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/MultiCmw_/State.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/MultiCmw_/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,20 +25,20 @@
 		"""lvalid commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_lvalid'):
 			from .Salignment_.Lvalid import Lvalid
 			self._lvalid = Lvalid(self._core, self._base)
 		return self._lvalid
 
 	@property
-	def reliabiliy(self):
-		"""reliabiliy commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_reliabiliy'):
-			from .Salignment_.Reliabiliy import Reliabiliy
-			self._reliabiliy = Reliabiliy(self._core, self._base)
-		return self._reliabiliy
+	def reliability(self):
+		"""reliability commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_reliability'):
+			from .Salignment_.Reliability import Reliability
+			self._reliability = Reliability(self._core, self._base)
+		return self._reliability
 
 	@property
 	def trace(self):
 		"""trace commands group. 4 Sub-classes, 0 commands."""
 		if not hasattr(self, '_trace'):
 			from .Salignment_.Trace import Trace
 			self._trace = Trace(self._core, self._base)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit_/RxDc.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit_/RxDc.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit_/RxImage.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit_/RxImage.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit_/TxDc.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit_/TxDc.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit_/TxImage.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Llimit_/TxImage.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Lvalid.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Lvalid.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Reliabiliy.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/Rlogging_/Protocol.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal import Conversions
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
+from ......Internal import Conversions
+from ......Internal.Utilities import trim_str_response
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Reliabiliy:
-	"""Reliabiliy commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class Protocol:
+	"""Protocol commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("reliabiliy", core, parent)
+		self._base = CommandsGroup("protocol", core, parent)
 
-	def fetch(self) -> int:
-		"""SCPI: FETCh:BASE:SALignment:RELiabiliy \n
-		Snippet: value: int = driver.base.salignment.reliabiliy.fetch() \n
+	def get(self, file: str) -> str:
+		"""SCPI: DIAGnostic:COMPass:DBASe:RLOGging:PROTocol \n
+		Snippet: value: str = driver.diagnostic.compass.dbase.rlogging.protocol.get(file = '1') \n
 		No command help available \n
-			:return: reliability: No help available"""
-		response = self._core.io.query_str(f'FETCh:BASE:SALignment:RELiabiliy?')
-		return Conversions.str_to_int(response)
+			:param file: No help available
+			:return: protocol: No help available"""
+		param = Conversions.value_to_quoted_str(file)
+		response = self._core.io.query_str(f'DIAGnostic:COMPass:DBASe:RLOGging:PROTocol? {param}')
+		return trim_str_response(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/State.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Trace.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Trace.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Trace_/RxDc.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Trace_/RxDc.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Trace_/RxImage.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Trace_/RxImage.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Trace_/TxDc.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Trace_/TxDc.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Trace_/TxImage.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Trace_/TxImage.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit_/RxDc.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit_/RxDc.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit_/RxImage.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit_/RxImage.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit_/TxDc.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit_/TxDc.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit_/TxImage.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit_/TxImage.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues_/RxDc.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues_/RxDc.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues_/RxImage.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues_/RxImage.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues_/TxDc.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues_/TxDc.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues_/TxImage.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues_/TxImage.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Calibration.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Calibration.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Calibration_/Base.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Calibration_/Base.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Calibration_/Base_/Ipc.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Calibration_/Base_/Ipc.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Calibration_/Base_/Ipcr.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Calibration_/Base_/Ipcr.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Calibration_/Base_/Latest.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Calibration_/Base_/Latest.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Calibration_/Base_/Latest_/Specific.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Calibration_/Base_/Latest_/Specific.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/Base.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/Base.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/Base_/Correction.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/Base_/Correction.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer_/Slot.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer_/Slot.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer_/Slot_/RxFilter.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer_/Slot_/RxFilter.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer_/Slot_/TxFilter.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/Base_/Correction_/IfEqualizer_/Slot_/TxFilter.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Catalog_/Base_/Salignment.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Catalog_/Base_/Salignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 		self._core = core
 		self._base = CommandsGroup("salignment", core, parent)
 
 	def get_slot(self) -> str:
 		"""SCPI: CATalog:BASE:SALignment:SLOT \n
 		Snippet: value: str = driver.catalog.base.salignment.get_slot() \n
 		No command help available \n
-			:return: slotlist: No help available
+			:return: slot_list: No help available
 		"""
 		response = self._core.io.query_str('CATalog:BASE:SALignment:SLOT?')
 		return trim_str_response(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Cmwd.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Cmwd.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Cmwd_/State.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Cmwd_/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 		"""multiCmw commands group. 1 Sub-classes, 1 commands."""
 		if not hasattr(self, '_multiCmw'):
 			from .Base_.MultiCmw import MultiCmw
 			self._multiCmw = MultiCmw(self._core, self._base)
 		return self._multiCmw
 
 	@property
-	def ipSubnet(self):
-		"""ipSubnet commands group. 1 Sub-classes, 0 commands."""
-		if not hasattr(self, '_ipSubnet'):
-			from .Base_.IpSubnet import IpSubnet
-			self._ipSubnet = IpSubnet(self._core, self._base)
-		return self._ipSubnet
+	def ipSet(self):
+		"""ipSet commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_ipSet'):
+			from .Base_.IpSet import IpSet
+			self._ipSet = IpSet(self._core, self._base)
+		return self._ipSet
 
 	@property
 	def adjustment(self):
 		"""adjustment commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_adjustment'):
 			from .Base_.Adjustment import Adjustment
 			self._adjustment = Adjustment(self._core, self._base)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Adjustment.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Adjustment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/RxFilter.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/RxFilter.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/RxFilter_/Select.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/RxFilter_/Select.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/TxFilter.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/TxFilter.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/TxFilter_/Select.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/TxFilter_/Select.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("freqCorrection", core, parent)
 
 	@property
 	def correctionTable(self):
-		"""correctionTable commands group. 8 Sub-classes, 2 commands."""
+		"""correctionTable commands group. 5 Sub-classes, 5 commands."""
 		if not hasattr(self, '_correctionTable'):
 			from .FreqCorrection_.CorrectionTable import CorrectionTable
 			self._correctionTable = CorrectionTable(self._core, self._base)
 		return self._correctionTable
 
 	def save(self, table_path: str = None) -> None:
 		"""SCPI: CONFigure:BASE:FDCorrection:SAV \n
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,104 +1,122 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
-from .....Internal import Conversions
+from .....Internal.RepeatedCapability import RepeatedCapability
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class CorrectionTable:
-	"""CorrectionTable commands group definition. 10 total commands, 8 Sub-groups, 2 group commands"""
+class File:
+	"""File commands group definition. 11 total commands, 11 Sub-groups, 0 group commands
+	Repeated Capability: FileNr, default value after init: FileNr.Nr1"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("correctionTable", core, parent)
+		self._base = CommandsGroup("file", core, parent)
+		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_fileNr_get', 'repcap_fileNr_set', repcap.FileNr.Nr1)
 
-	@property
-	def create(self):
-		"""create commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_create'):
-			from .CorrectionTable_.Create import Create
-			self._create = Create(self._core, self._base)
-		return self._create
-
-	@property
-	def erase(self):
-		"""erase commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_erase'):
-			from .CorrectionTable_.Erase import Erase
-			self._erase = Erase(self._core, self._base)
-		return self._erase
-
-	@property
-	def add(self):
-		"""add commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_add'):
-			from .CorrectionTable_.Add import Add
-			self._add = Add(self._core, self._base)
-		return self._add
-
-	@property
-	def length(self):
-		"""length commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_length'):
-			from .CorrectionTable_.Length import Length
-			self._length = Length(self._core, self._base)
-		return self._length
-
-	@property
-	def details(self):
-		"""details commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_details'):
-			from .CorrectionTable_.Details import Details
-			self._details = Details(self._core, self._base)
-		return self._details
-
-	@property
-	def catalog(self):
-		"""catalog commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_catalog'):
-			from .CorrectionTable_.Catalog import Catalog
-			self._catalog = Catalog(self._core, self._base)
-		return self._catalog
-
-	@property
-	def count(self):
-		"""count commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_count'):
-			from .CorrectionTable_.Count import Count
-			self._count = Count(self._core, self._base)
-		return self._count
-
-	@property
-	def exist(self):
-		"""exist commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_exist'):
-			from .CorrectionTable_.Exist import Exist
-			self._exist = Exist(self._core, self._base)
-		return self._exist
-
-	def delete(self, table_name: str) -> None:
-		"""SCPI: CONFigure:BASE:FDCorrection:CTABle:DELete \n
-		Snippet: driver.configure.base.freqCorrection.correctionTable.delete(table_name = '1') \n
-		No command help available \n
-			:param table_name: No help available
-		"""
-		param = Conversions.value_to_quoted_str(table_name)
-		self._core.io.write(f'CONFigure:BASE:FDCorrection:CTABle:DELete {param}')
-
-	def delete_all(self, table_path: str = None) -> None:
-		"""SCPI: CONFigure:BASE:FDCorrection:CTABle:DELete:ALL \n
-		Snippet: driver.configure.base.freqCorrection.correctionTable.delete_all(table_path = '1') \n
-		No command help available \n
-			:param table_path: No help available
-		"""
-		param = ''
-		if table_path:
-			param = Conversions.value_to_quoted_str(table_path)
-		self._core.io.write(f'CONFigure:BASE:FDCorrection:CTABle:DELete:ALL {param}'.strip())
+	def repcap_fileNr_set(self, enum_value: repcap.FileNr) -> None:
+		"""Repeated Capability default value numeric suffix.
+		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to FileNr.Default
+		Default value after init: FileNr.Nr1"""
+		self._base.set_repcap_enum_value(enum_value)
+
+	def repcap_fileNr_get(self) -> repcap.FileNr:
+		"""Returns the current default repeated capability for the child set/get methods"""
+		# noinspection PyTypeChecker
+		return self._base.get_repcap_enum_value()
+
+	@property
+	def dexecution(self):
+		"""dexecution commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_dexecution'):
+			from .File_.Dexecution import Dexecution
+			self._dexecution = Dexecution(self._core, self._base)
+		return self._dexecution
+
+	@property
+	def stopMode(self):
+		"""stopMode commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_stopMode'):
+			from .File_.StopMode import StopMode
+			self._stopMode = StopMode(self._core, self._base)
+		return self._stopMode
+
+	@property
+	def startMode(self):
+		"""startMode commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_startMode'):
+			from .File_.StartMode import StartMode
+			self._startMode = StartMode(self._core, self._base)
+		return self._startMode
+
+	@property
+	def name(self):
+		"""name commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_name'):
+			from .File_.Name import Name
+			self._name = Name(self._core, self._base)
+		return self._name
+
+	@property
+	def formatPy(self):
+		"""formatPy commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_formatPy'):
+			from .File_.FormatPy import FormatPy
+			self._formatPy = FormatPy(self._core, self._base)
+		return self._formatPy
+
+	@property
+	def size(self):
+		"""size commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_size'):
+			from .File_.Size import Size
+			self._size = Size(self._core, self._base)
+		return self._size
+
+	@property
+	def rpc(self):
+		"""rpc commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_rpc'):
+			from .File_.Rpc import Rpc
+			self._rpc = Rpc(self._core, self._base)
+		return self._rpc
+
+	@property
+	def functions(self):
+		"""functions commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_functions'):
+			from .File_.Functions import Functions
+			self._functions = Functions(self._core, self._base)
+		return self._functions
+
+	@property
+	def parser(self):
+		"""parser commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_parser'):
+			from .File_.Parser import Parser
+			self._parser = Parser(self._core, self._base)
+		return self._parser
+
+	@property
+	def filterPy(self):
+		"""filterPy commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_filterPy'):
+			from .File_.FilterPy import FilterPy
+			self._filterPy = FilterPy(self._core, self._base)
+		return self._filterPy
+
+	@property
+	def enable(self):
+		"""enable commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_enable'):
+			from .File_.Enable import Enable
+			self._enable = Enable(self._core, self._base)
+		return self._enable
 
-	def clone(self) -> 'CorrectionTable':
+	def clone(self) -> 'File':
 		"""Clones the group by creating new object from it and its whole existing sub-groups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = CorrectionTable(self._core, self._base.parent)
+		new_group = File(self._core, self._base.parent)
 		self._base.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Add.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Condition_/Bits_/Cataloge.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from typing import List
 
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal.Types import DataType
-from ......Internal.ArgSingleList import ArgSingleList
-from ......Internal.ArgSingle import ArgSingle
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from .....Internal.Types import DataType
+from .....Internal.ArgSingleList import ArgSingleList
+from .....Internal.ArgSingle import ArgSingle
+from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Add:
-	"""Add commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class Cataloge:
+	"""Cataloge commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("add", core, parent)
+		self._base = CommandsGroup("cataloge", core, parent)
 
-	def set(self, table_name: str, frequency: List[float] = None, correction: List[float] = None) -> None:
-		"""SCPI: CONFigure:BASE:FDCorrection:CTABle:ADD \n
-		Snippet: driver.configure.base.freqCorrection.correctionTable.add.set(table_name = '1', frequency = [1.1, 2.2, 3.3], correction = [1.1, 2.2, 3.3]) \n
+	def get(self, filter_py: str = None, mode: enums.ExpressionMode = None) -> List[str]:
+		"""SCPI: STATus:CONDition:BITS:CATaloge \n
+		Snippet: value: List[str] = driver.status.condition.bits.cataloge.get(filter_py = '1', mode = enums.ExpressionMode.REGex) \n
 		No command help available \n
-			:param table_name: No help available
-			:param frequency: No help available
-			:param correction: No help available
-		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('table_name', table_name, DataType.String), ArgSingle('frequency', frequency, DataType.FloatList, True, True, 1), ArgSingle('correction', correction, DataType.FloatList, True, True, 1))
-		self._core.io.write(f'CONFigure:BASE:FDCorrection:CTABle:ADD {param}'.rstrip())
+			:param filter_py: No help available
+			:param mode: No help available
+			:return: bit: No help available"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('filter_py', filter_py, DataType.String, True), ArgSingle('mode', mode, DataType.Enum, True))
+		response = self._core.io.query_str(f'STATus:CONDition:BITS:CATaloge? {param}'.rstrip())
+		return Conversions.str_to_str_list(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Catalog.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,11 +17,11 @@
 		self._base = CommandsGroup("catalog", core, parent)
 
 	def get(self, table_path: str = None) -> List[str]:
 		"""SCPI: CONFigure:BASE:FDCorrection:CTABle:CATalog \n
 		Snippet: value: List[str] = driver.configure.base.freqCorrection.correctionTable.catalog.get(table_path = '1') \n
 		No command help available \n
 			:param table_path: No help available
-			:return: tablename: No help available"""
+			:return: table_name: No help available"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('table_path', table_path, DataType.String, True))
 		response = self._core.io.query_str(f'CONFigure:BASE:FDCorrection:CTABle:CATalog? {param}'.rstrip())
 		return Conversions.str_to_str_list(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Count.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Count.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,11 +15,11 @@
 		self._base = CommandsGroup("count", core, parent)
 
 	def get(self, table_path: str = None) -> int:
 		"""SCPI: CONFigure:BASE:FDCorrection:CTABle:COUNt \n
 		Snippet: value: int = driver.configure.base.freqCorrection.correctionTable.count.get(table_path = '1') \n
 		No command help available \n
 			:param table_path: No help available
-			:return: tablecount: No help available"""
+			:return: table_count: No help available"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('table_path', table_path, DataType.String, True))
 		response = self._core.io.query_str(f'CONFigure:BASE:FDCorrection:CTABle:COUNt? {param}'.rstrip())
 		return Conversions.str_to_int(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Create.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/Run.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from typing import List
-
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal.Types import DataType
-from ......Internal.ArgSingleList import ArgSingleList
-from ......Internal.ArgSingle import ArgSingle
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal.Types import DataType
+from .....Internal.Utilities import trim_str_response
+from .....Internal.ArgSingleList import ArgSingleList
+from .....Internal.ArgSingle import ArgSingle
+from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Create:
-	"""Create commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class Run:
+	"""Run commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("create", core, parent)
+		self._base = CommandsGroup("run", core, parent)
 
-	def set(self, table_name: str, frequency: List[float] = None, correction: List[float] = None) -> None:
-		"""SCPI: CONFigure:BASE:FDCorrection:CTABle:CREate \n
-		Snippet: driver.configure.base.freqCorrection.correctionTable.create.set(table_name = '1', frequency = [1.1, 2.2, 3.3], correction = [1.1, 2.2, 3.3]) \n
+	def get(self, filter_py: str = None, mode: enums.ExpressionMode = None) -> str:
+		"""SCPI: STATus:MEASurement:CONDition:RUN \n
+		Snippet: value: str = driver.status.measurement.condition.run.get(filter_py = '1', mode = enums.ExpressionMode.REGex) \n
 		No command help available \n
-			:param table_name: No help available
-			:param frequency: No help available
-			:param correction: No help available
-		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('table_name', table_name, DataType.String), ArgSingle('frequency', frequency, DataType.FloatList, True, True, 1), ArgSingle('correction', correction, DataType.FloatList, True, True, 1))
-		self._core.io.write(f'CONFigure:BASE:FDCorrection:CTABle:CREate {param}'.rstrip())
+			:param filter_py: No help available
+			:param mode: No help available
+			:return: bitname: No help available"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('filter_py', filter_py, DataType.String, True), ArgSingle('mode', mode, DataType.Enum, True))
+		response = self._core.io.query_str(f'STATus:MEASurement:CONDition:RUN? {param}'.rstrip())
+		return trim_str_response(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Details.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Details.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Erase.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Generator_/Condition_/Pending.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-from typing import List
-
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal.Types import DataType
-from ......Internal.ArgSingleList import ArgSingleList
-from ......Internal.ArgSingle import ArgSingle
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal.Types import DataType
+from .....Internal.Utilities import trim_str_response
+from .....Internal.ArgSingleList import ArgSingleList
+from .....Internal.ArgSingle import ArgSingle
+from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Erase:
-	"""Erase commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class Pending:
+	"""Pending commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("erase", core, parent)
+		self._base = CommandsGroup("pending", core, parent)
 
-	def set(self, table_name: str, frequency: List[float] = None) -> None:
-		"""SCPI: CONFigure:BASE:FDCorrection:CTABle:ERASe \n
-		Snippet: driver.configure.base.freqCorrection.correctionTable.erase.set(table_name = '1', frequency = [1.1, 2.2, 3.3]) \n
+	def get(self, filter_py: str = None, mode: enums.ExpressionMode = None) -> str:
+		"""SCPI: STATus:GENerator:CONDition:PENDing \n
+		Snippet: value: str = driver.status.generator.condition.pending.get(filter_py = '1', mode = enums.ExpressionMode.REGex) \n
 		No command help available \n
-			:param table_name: No help available
-			:param frequency: No help available
-		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('table_name', table_name, DataType.String), ArgSingle('frequency', frequency, DataType.FloatList, True, True, 1))
-		self._core.io.write(f'CONFigure:BASE:FDCorrection:CTABle:ERASe {param}'.rstrip())
+			:param filter_py: No help available
+			:param mode: No help available
+			:return: bitname: No help available"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('filter_py', filter_py, DataType.String, True), ArgSingle('mode', mode, DataType.Enum, True))
+		response = self._core.io.query_str(f'STATus:GENerator:CONDition:PENDing? {param}'.rstrip())
+		return trim_str_response(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Exist.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Exist.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Length.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Length.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/IpSubnet.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Startup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
+from ...Internal.Core import Core
+from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class IpSubnet:
-	"""IpSubnet commands group definition. 1 total commands, 1 Sub-groups, 0 group commands"""
+class Startup:
+	"""Startup commands group definition. 1 total commands, 1 Sub-groups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ipSubnet", core, parent)
+		self._base = CommandsGroup("startup", core, parent)
 
 	@property
-	def nwAdapter(self):
-		"""nwAdapter commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_nwAdapter'):
-			from .IpSubnet_.NwAdapter import NwAdapter
-			self._nwAdapter = NwAdapter(self._core, self._base)
-		return self._nwAdapter
+	def prepare(self):
+		"""prepare commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_prepare'):
+			from .Startup_.Prepare import Prepare
+			self._prepare = Prepare(self._core, self._base)
+		return self._prepare
 
-	def clone(self) -> 'IpSubnet':
+	def clone(self) -> 'Startup':
 		"""Clones the group by creating new object from it and its whole existing sub-groups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = IpSubnet(self._core, self._base.parent)
+		new_group = Startup(self._core, self._base.parent)
 		self._base.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/IpSubnet_/NwAdapter.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/IpSet_/NwAdapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 	def repcap_nwAdapter_get(self) -> repcap.NwAdapter:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
 		return self._base.get_repcap_enum_value()
 
 	def set(self, set_subnet_conform: bool, nwAdapter=repcap.NwAdapter.Default) -> None:
 		"""SCPI: CONFigure:BASE:IPSet:NWADapter<n> \n
-		Snippet: driver.configure.base.ipSubnet.nwAdapter.set(set_subnet_conform = False, nwAdapter = repcap.NwAdapter.Default) \n
+		Snippet: driver.configure.base.ipSet.nwAdapter.set(set_subnet_conform = False, nwAdapter = repcap.NwAdapter.Default) \n
 		No command help available \n
 			:param set_subnet_conform: No help available
 			:param nwAdapter: optional repeated capability selector. Default value: Adapter1 (settable in the interface 'NwAdapter')"""
 		param = Conversions.bool_to_str(set_subnet_conform)
 		nwAdapter_cmd_val = self._base.get_repcap_cmd_value(nwAdapter, repcap.NwAdapter)
 		self._core.io.write(f'CONFigure:BASE:IPSet:NWADapter{nwAdapter_cmd_val} {param}')
 
@@ -57,15 +57,15 @@
 			self.Nw_Adapter_Name: str = None
 			self.Set_Subnet_Conform: bool = None
 			self.Ip_Address: str = None
 			self.Status: enums.AdjustStatus = None
 
 	def get(self, nwAdapter=repcap.NwAdapter.Default) -> GetStruct:
 		"""SCPI: CONFigure:BASE:IPSet:NWADapter<n> \n
-		Snippet: value: GetStruct = driver.configure.base.ipSubnet.nwAdapter.get(nwAdapter = repcap.NwAdapter.Default) \n
+		Snippet: value: GetStruct = driver.configure.base.ipSet.nwAdapter.get(nwAdapter = repcap.NwAdapter.Default) \n
 		No command help available \n
 			:param nwAdapter: optional repeated capability selector. Default value: Adapter1 (settable in the interface 'NwAdapter')
 			:return: structure: for return value, see the help for GetStruct structure arguments."""
 		nwAdapter_cmd_val = self._base.get_repcap_cmd_value(nwAdapter, repcap.NwAdapter)
 		return self._core.io.query_struct(f'CONFigure:BASE:IPSet:NWADapter{nwAdapter_cmd_val}?', self.__class__.GetStruct())
 
 	def clone(self) -> 'NwAdapter':
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Ipcr.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Ipcr.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Mmonitor.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Mmonitor.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Mmonitor_/IpAddress.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Mmonitor_/IpAddress.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/MultiCmw.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/MultiCmw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/MultiCmw_/Identify.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/MultiCmw_/Identify.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Base_/Salignment.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/Salignment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Cmwd.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Cmwd.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/FreqCorrection.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/FreqCorrection.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/FreqCorrection_/Activate.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/FreqCorrection_/Activate.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 class Activate:
 	"""Activate commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("activate", core, parent)
 
-	def set(self, connector: str, table: str, direction: enums.RxTxDirection = None, rfconverter: enums.RfConverterInPath = None) -> None:
+	def set(self, connector: str, table: str, direction: enums.RxTxDirection = None, rf_converter: enums.RfConverterInPath = None) -> None:
 		"""SCPI: CONFigure:FDCorrection:ACTivate \n
-		Snippet: driver.configure.freqCorrection.activate.set(connector = r1, table = '1', direction = enums.RxTxDirection.RX, rfconverter = enums.RfConverterInPath.RF1) \n
+		Snippet: driver.configure.freqCorrection.activate.set(connector = r1, table = '1', direction = enums.RxTxDirection.RX, rf_converter = enums.RfConverterInPath.RF1) \n
 		No command help available \n
 			:param connector: No help available
 			:param table: No help available
 			:param direction: No help available
-			:param rfconverter: No help available
+			:param rf_converter: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('connector', connector, DataType.RawString), ArgSingle('table', table, DataType.String), ArgSingle('direction', direction, DataType.Enum, True), ArgSingle('rfconverter', rfconverter, DataType.Enum, True))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('connector', connector, DataType.RawString), ArgSingle('table', table, DataType.String), ArgSingle('direction', direction, DataType.Enum, True), ArgSingle('rf_converter', rf_converter, DataType.Enum, True))
 		self._core.io.write(f'CONFigure:FDCorrection:ACTivate {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class GetStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Table_Rx: str: No parameter help available
 			- Table_Tx: str: No parameter help available"""
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/FreqCorrection_/Usage.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/FreqCorrection_/Usage.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Mutex.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Mutex.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Mutex_/Define.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Mutex_/Define.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Mutex_/Lock.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Mutex_/Lock.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Mutex_/State.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Mutex_/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Semaphore.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Semaphore.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Semaphore_/Acquire.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Semaphore_/Acquire.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Semaphore_/Count.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Semaphore_/Count.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Semaphore_/Define.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Semaphore_/Define.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Semaphore_/Release.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Semaphore_/Release.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("freqCorrection", core, parent)
 
 	@property
 	def activate(self):
-		"""activate commands group. 0 Sub-classes, 2 commands."""
+		"""activate commands group. 2 Sub-classes, 0 commands."""
 		if not hasattr(self, '_activate'):
 			from .FreqCorrection_.Activate import Activate
 			self._activate = Activate(self._core, self._base)
 		return self._activate
 
 	@property
 	def deactivate(self):
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Rx.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Tx.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Rx:
-	"""Rx commands group definition. 2 total commands, 1 Sub-groups, 1 group commands"""
+class Tx:
+	"""Tx commands group definition. 2 total commands, 1 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("rx", core, parent)
+		self._base = CommandsGroup("tx", core, parent)
 
 	@property
 	def all(self):
 		"""all commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_all'):
-			from .Rx_.All import All
+			from .Tx_.All import All
 			self._all = All(self._core, self._base)
 		return self._all
 
-	def set_value(self, connectorbench: str) -> None:
-		"""SCPI: CONFigure:CMWS:FDCorrection:DEACtivate:RX \n
-		Snippet: driver.configure.singleCmw.freqCorrection.deactivate.rx.set_value(connectorbench = r1) \n
+	def set_value(self, connector_bench: str) -> None:
+		"""SCPI: CONFigure:CMWS:FDCorrection:DEACtivate:TX \n
+		Snippet: driver.configure.singleCmw.freqCorrection.deactivate.tx.set_value(connector_bench = r1) \n
 		No command help available \n
-			:param connectorbench: No help available
+			:param connector_bench: No help available
 		"""
-		param = Conversions.value_to_str(connectorbench)
-		self._core.io.write(f'CONFigure:CMWS:FDCorrection:DEACtivate:RX {param}')
+		param = Conversions.value_to_str(connector_bench)
+		self._core.io.write(f'CONFigure:CMWS:FDCorrection:DEACtivate:TX {param}')
 
-	def clone(self) -> 'Rx':
+	def clone(self) -> 'Tx':
 		"""Clones the group by creating new object from it and its whole existing sub-groups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Rx(self._core, self._base.parent)
+		new_group = Tx(self._core, self._base.parent)
 		self._base.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Rx_/All.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Rx_/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Tx.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Rx.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Tx:
-	"""Tx commands group definition. 2 total commands, 1 Sub-groups, 1 group commands"""
+class Rx:
+	"""Rx commands group definition. 2 total commands, 1 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("tx", core, parent)
+		self._base = CommandsGroup("rx", core, parent)
 
 	@property
 	def all(self):
 		"""all commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_all'):
-			from .Tx_.All import All
+			from .Rx_.All import All
 			self._all = All(self._core, self._base)
 		return self._all
 
-	def set_value(self, connectorbench: str) -> None:
-		"""SCPI: CONFigure:CMWS:FDCorrection:DEACtivate:TX \n
-		Snippet: driver.configure.singleCmw.freqCorrection.deactivate.tx.set_value(connectorbench = r1) \n
+	def set_value(self, connector_bench: str) -> None:
+		"""SCPI: CONFigure:CMWS:FDCorrection:DEACtivate:RX \n
+		Snippet: driver.configure.singleCmw.freqCorrection.deactivate.rx.set_value(connector_bench = r1) \n
 		No command help available \n
-			:param connectorbench: No help available
+			:param connector_bench: No help available
 		"""
-		param = Conversions.value_to_str(connectorbench)
-		self._core.io.write(f'CONFigure:CMWS:FDCorrection:DEACtivate:TX {param}')
+		param = Conversions.value_to_str(connector_bench)
+		self._core.io.write(f'CONFigure:CMWS:FDCorrection:DEACtivate:RX {param}')
 
-	def clone(self) -> 'Tx':
+	def clone(self) -> 'Rx':
 		"""Clones the group by creating new object from it and its whole existing sub-groups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Tx(self._core, self._base.parent)
+		new_group = Rx(self._core, self._base.parent)
 		self._base.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Tx_/All.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Tx_/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Usage.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Usage.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Spoint.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Spoint.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Spoint_/Define.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Spoint_/Define.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Spoint_/Join.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Spoint_/Join.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Configure_/Spoint_/Rewait.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Spoint_/Rewait.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Base.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Base.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Base_/Mmi.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Base_/Mmi.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment_/Path.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment_/Path.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment_/Path_/Iq.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment_/Path_/Iq.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,11 +41,11 @@
 		response = self._core.io.query_str('DIAGnostic:BASE:SALignment:PATH:IQ:STATe?')
 		return Conversions.str_to_str_list(response)
 
 	def get_value(self) -> List[str]:
 		"""SCPI: DIAGnostic:BASE:SALignment:PATH:IQ \n
 		Snippet: value: List[str] = driver.diagnostic.base.salignment.path.iq.get_value() \n
 		No command help available \n
-			:return: pathlist: No help available
+			:return: path_list: No help available
 		"""
 		response = self._core.io.query_str('DIAGnostic:BASE:SALignment:PATH:IQ?')
 		return Conversions.str_to_str_list(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment_/Path_/Level.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Base_/Salignment_/Path_/Level.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,11 +41,11 @@
 		response = self._core.io.query_str('DIAGnostic:BASE:SALignment:PATH:LEVel:STATe?')
 		return Conversions.str_to_str_list(response)
 
 	def get_value(self) -> List[str]:
 		"""SCPI: DIAGnostic:BASE:SALignment:PATH:LEVel \n
 		Snippet: value: List[str] = driver.diagnostic.base.salignment.path.level.get_value() \n
 		No command help available \n
-			:return: pathlist: No help available
+			:return: path_list: No help available
 		"""
 		response = self._core.io.query_str('DIAGnostic:BASE:SALignment:PATH:LEVel?')
 		return Conversions.str_to_str_list(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/BgInfo.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/BgInfo.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Cmw.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Cmw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Cmw_/LedTest.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Cmw_/LedTest.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Cmw_/LedTest_/Rx.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Cmw_/LedTest_/Rx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Cmw_/LedTest_/Tx.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Cmw_/LedTest_/Tx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/Rlogging.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/Rlogging.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/Rlogging_/Protocol.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/TaLogging_/Protocol.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
-from ......Internal.Utilities import trim_str_response
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class Protocol:
 	"""Protocol commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("protocol", core, parent)
 
-	def get(self, file: str) -> str:
-		"""SCPI: DIAGnostic:COMPass:DBASe:RLOGging:PROTocol \n
-		Snippet: value: str = driver.diagnostic.compass.dbase.rlogging.protocol.get(file = '1') \n
+	def get(self, file: str) -> int:
+		"""SCPI: DIAGnostic:COMPass:DBASe:TALogging:PROTocol \n
+		Snippet: value: int = driver.diagnostic.compass.dbase.taLogging.protocol.get(file = '1') \n
 		No command help available \n
 			:param file: No help available
-			:return: protocol: No help available"""
+			:return: result: No help available"""
 		param = Conversions.value_to_quoted_str(file)
-		response = self._core.io.query_str(f'DIAGnostic:COMPass:DBASe:RLOGging:PROTocol? {param}')
-		return trim_str_response(response)
+		response = self._core.io.query_str(f'DIAGnostic:COMPass:DBASe:TALogging:PROTocol? {param}')
+		return Conversions.str_to_int(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/TaLogging.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/TaLogging.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/TaLogging_/Mode.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/TaLogging_/Mode.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Dbase_/TaLogging_/Protocol.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Pias_/Connect_/Multiple.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
+from typing import List
+
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Protocol:
-	"""Protocol commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class Multiple:
+	"""Multiple commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("protocol", core, parent)
+		self._base = CommandsGroup("multiple", core, parent)
 
-	def get(self, file: str) -> int:
-		"""SCPI: DIAGnostic:COMPass:DBASe:TALogging:PROTocol \n
-		Snippet: value: int = driver.diagnostic.compass.dbase.taLogging.protocol.get(file = '1') \n
+	def get(self, handle: List[str]) -> int:
+		"""SCPI: DIAGnostic:PIAS:CONNect:MULTiple \n
+		Snippet: value: int = driver.diagnostic.pias.connect.multiple.get(handle = ['1', '2', '3']) \n
 		No command help available \n
-			:param file: No help available
+			:param handle: No help available
 			:return: result: No help available"""
-		param = Conversions.value_to_quoted_str(file)
-		response = self._core.io.query_str(f'DIAGnostic:COMPass:DBASe:TALogging:PROTocol? {param}')
+		param = Conversions.list_to_csv_quoted_str(handle)
+		response = self._core.io.query_str(f'DIAGnostic:PIAS:CONNect:MULTiple? {param}')
 		return Conversions.str_to_int(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Debug.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Debug.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Statistics.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Statistics.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Statistics_/Process.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Compass_/Statistics_/Process.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Eeprom.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Eeprom.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Eeprom_/Data.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Eeprom_/Data.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 class Data:
 	"""Data commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("data", core, parent)
 
-	def set(self, board: str, tableid: int, board_instance: int = None) -> None:
+	def set(self, board: str, table_id: int, board_instance: int = None) -> None:
 		"""SCPI: DIAGnostic:EEPRom:DATA \n
-		Snippet: driver.diagnostic.eeprom.data.set(board = '1', tableid = 1, board_instance = 1) \n
+		Snippet: driver.diagnostic.eeprom.data.set(board = '1', table_id = 1, board_instance = 1) \n
 		No command help available \n
 			:param board: No help available
-			:param tableid: No help available
+			:param table_id: No help available
 			:param board_instance: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('board', board, DataType.String), ArgSingle('tableid', tableid, DataType.Integer), ArgSingle('board_instance', board_instance, DataType.Integer, True))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('board', board, DataType.String), ArgSingle('table_id', table_id, DataType.Integer), ArgSingle('board_instance', board_instance, DataType.Integer, True))
 		self._core.io.write(f'DIAGnostic:EEPRom:DATA {param}'.rstrip())
 
 	def get(self) -> str:
 		"""SCPI: DIAGnostic:EEPRom:DATA \n
 		Snippet: value: str = driver.diagnostic.eeprom.data.get() \n
 		No command help available \n
-			:return: datafolder: No help available"""
+			:return: data_folder: No help available"""
 		response = self._core.io.query_str(f'DIAGnostic:EEPRom:DATA?')
 		return trim_str_response(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Eeprom_/Header.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Eeprom_/Header.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Error.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Error.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Error_/Queue.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Error_/Queue.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Error_/Queue_/Push.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Error_/Queue_/Push.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Connection.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Connection.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Connection_/Target.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Connection_/Target.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Connection_/Target_/Ids.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Connection_/Target_/Ids.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Data.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Data.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Properties.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/Properties.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/References.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Element_/References.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Li.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Li.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Li_/Usecases.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/Li_/Usecases.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/UseCase.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/UseCase.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/UseCase_/Data.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/FootPrint_/UseCase_/Data.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Help.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Help.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Help_/Syntax.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Help_/Syntax.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Instrument.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Instrument.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,30 +15,30 @@
 	def consistency(self):
 		"""consistency commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_consistency'):
 			from .Instrument_.Consistency import Consistency
 			self._consistency = Consistency(self._core, self._base)
 		return self._consistency
 
-	def load(self, appl_name_and_li_nr: str) -> None:
+	def load(self, appl_name_and_li_number: str) -> None:
 		"""SCPI: DIAGnostic:INSTrument:LOAD \n
-		Snippet: driver.diagnostic.instrument.load(appl_name_and_li_nr = '1') \n
+		Snippet: driver.diagnostic.instrument.load(appl_name_and_li_number = '1') \n
 		No command help available \n
-			:param appl_name_and_li_nr: No help available
+			:param appl_name_and_li_number: No help available
 		"""
-		param = Conversions.value_to_quoted_str(appl_name_and_li_nr)
+		param = Conversions.value_to_quoted_str(appl_name_and_li_number)
 		self._core.io.write(f'DIAGnostic:INSTrument:LOAD {param}')
 
-	def set_unload(self, appl_name_and_li_nr: str) -> None:
+	def set_unload(self, appl_name_and_li_number: str) -> None:
 		"""SCPI: DIAGnostic:INSTrument:UNLoad \n
-		Snippet: driver.diagnostic.instrument.set_unload(appl_name_and_li_nr = '1') \n
+		Snippet: driver.diagnostic.instrument.set_unload(appl_name_and_li_number = '1') \n
 		No command help available \n
-			:param appl_name_and_li_nr: No help available
+			:param appl_name_and_li_number: No help available
 		"""
-		param = Conversions.value_to_quoted_str(appl_name_and_li_nr)
+		param = Conversions.value_to_quoted_str(appl_name_and_li_number)
 		self._core.io.write(f'DIAGnostic:INSTrument:UNLoad {param}')
 
 	def clone(self) -> 'Instrument':
 		"""Clones the group by creating new object from it and its whole existing sub-groups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
 		new_group = Instrument(self._core, self._base.parent)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Instrument_/Consistency.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Instrument_/Consistency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Log.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Log.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Log_/Dump.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Log_/Dump.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Pias.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Pias.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Pias_/Connect.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Pias_/Connect.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Pias_/Connect_/Multiple.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/Event.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-from typing import List
-
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal import Conversions
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Multiple:
-	"""Multiple commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class Event:
+	"""Event commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("multiple", core, parent)
+		self._base = CommandsGroup("event", core, parent)
 
-	def get(self, handle: List[str]) -> int:
-		"""SCPI: DIAGnostic:PIAS:CONNect:MULTiple \n
-		Snippet: value: int = driver.diagnostic.pias.connect.multiple.get(handle = ['1', '2', '3']) \n
+	def get(self, bitNr=repcap.BitNr.Default) -> bool:
+		"""SCPI: STATus:QUEStionable:BIT<bitno>[:EVENt] \n
+		Snippet: value: bool = driver.status.questionable.bit.event.get(bitNr = repcap.BitNr.Default) \n
 		No command help available \n
-			:param handle: No help available
-			:return: result: No help available"""
-		param = Conversions.list_to_csv_quoted_str(handle)
-		response = self._core.io.query_str(f'DIAGnostic:PIAS:CONNect:MULTiple? {param}')
-		return Conversions.str_to_int(response)
+			:param bitNr: optional repeated capability selector. Default value: Nr8 (settable in the interface 'Bit')
+			:return: register_bit: No help available"""
+		bitNr_cmd_val = self._base.get_repcap_cmd_value(bitNr, repcap.BitNr)
+		response = self._core.io.query_str(f'STATus:QUEStionable:BIT{bitNr_cmd_val}:EVENt?')
+		return Conversions.str_to_bool(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Pias_/Scan.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Pias_/Scan.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Product.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Product.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Product_/MacAddress.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Product_/MacAddress.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Product_/Time.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Product_/Time.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Record.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Record.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Record_/Macro.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Record_/Macro.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Record_/Macro_/File.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Record_/Macro_/File.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Routing.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Routing.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Routing_/Expert.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Routing_/Expert.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Routing_/Expert_/Setup.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Routing_/Expert_/Setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 class Setup:
 	"""Setup commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("setup", core, parent)
 
-	def set(self, routingname: str, data: List[enums.ExpertSetup]) -> None:
+	def set(self, routing_name: str, data: List[enums.ExpertSetup]) -> None:
 		"""SCPI: DIAGnostic:ROUTing:EXPert:SETup \n
-		Snippet: driver.diagnostic.routing.expert.setup.set(routingname = '1', data = [ExpertSetup.BBG1, ExpertSetup.SUW7]) \n
+		Snippet: driver.diagnostic.routing.expert.setup.set(routing_name = '1', data = [ExpertSetup.BBG1, ExpertSetup.SUW7]) \n
 		No command help available \n
-			:param routingname: No help available
+			:param routing_name: No help available
 			:param data: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('routingname', routingname, DataType.String), ArgSingle.as_open_list('data', data, DataType.EnumList))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('routing_name', routing_name, DataType.String), ArgSingle.as_open_list('data', data, DataType.EnumList))
 		self._core.io.write(f'DIAGnostic:ROUTing:EXPert:SETup {param}'.rstrip())
 
 	# noinspection PyTypeChecker
-	def get(self, routingname: str) -> List[enums.ExpertSetup]:
+	def get(self, routing_name: str) -> List[enums.ExpertSetup]:
 		"""SCPI: DIAGnostic:ROUTing:EXPert:SETup \n
-		Snippet: value: List[enums.ExpertSetup] = driver.diagnostic.routing.expert.setup.get(routingname = '1') \n
+		Snippet: value: List[enums.ExpertSetup] = driver.diagnostic.routing.expert.setup.get(routing_name = '1') \n
 		No command help available \n
-			:param routingname: No help available
+			:param routing_name: No help available
 			:return: data: No help available"""
-		param = Conversions.value_to_quoted_str(routingname)
+		param = Conversions.value_to_quoted_str(routing_name)
 		response = self._core.io.query_str(f'DIAGnostic:ROUTing:EXPert:SETup? {param}')
 		return Conversions.str_to_list_enum(response, enums.ExpertSetup)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/SingleCmw.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/SingleCmw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Diagnostic_/Status.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Diagnostic_/Status.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Display.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Display.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Display_/Window.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Display_/Window.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Display_/Window_/Select.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Display_/Window_/Select.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/FirmwareUpdate.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/FirmwareUpdate.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/FormatPy.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/FormatPy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/FormatPy_/Base.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/FormatPy_/Base.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Get.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Get.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/GlobalClearStatus.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/GlobalClearStatus.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/GlobalWait.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/GlobalWait.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/GoToLocal.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/GotoLocal.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from ..Internal.Core import Core
 from ..Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class GoToLocal:
-	"""GoToLocal commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class GotoLocal:
+	"""GotoLocal commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("goToLocal", core, parent)
+		self._base = CommandsGroup("gotoLocal", core, parent)
 
 	def set(self) -> None:
 		"""SCPI: *GTL \n
-		Snippet: driver.goToLocal.set() \n
+		Snippet: driver.gotoLocal.set() \n
 		No command help available \n
 		"""
 		self._core.io.write(f'*GTL')
 
 	def set_with_opc(self) -> None:
 		"""SCPI: *GTL \n
-		Snippet: driver.goToLocal.set_with_opc() \n
+		Snippet: driver.gotoLocal.set_with_opc() \n
 		No command help available \n
 		Same as set, but waits for the operation to complete before continuing further. Use the RsCMPX_Base.utilities.opc_timeout_set() to set the timeout value. \n
 		"""
 		self._core.io.write_with_opc(f'*GTL')
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/HardCopy.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/HardCopy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/HardCopy_/Device.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/HardCopy_/Device.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/HardCopy_/Interior.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/HardCopy_/Interior.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Instrument.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Instrument.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Instrument_/Display.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Instrument_/Display.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Instrument_/Select.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Instrument_/Select.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MacroCreate.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MacroCreate.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,21 +73,21 @@
 		Copies an existing file. The target directory must exist. \n
 			:param file_source: Name of the file to be copied. Wildcards ? and * are allowed if FileDestination contains a path without filename.
 			:param file_destination: Path and/or name of the new file If no file destination is specified, the source file is written to the current directory (see method RsCMPX_Base.MassMemory.CurrentDirectory.set) . Wildcards are not allowed.
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('file_source', file_source, DataType.String), ArgSingle('file_destination', file_destination, DataType.String, True))
 		self._core.io.write(f'MMEMory:COPY {param}'.rstrip())
 
-	def delete(self, file_name: str) -> None:
+	def delete(self, filename: str) -> None:
 		"""SCPI: MMEMory:DELete \n
-		Snippet: driver.massMemory.delete(file_name = '1') \n
+		Snippet: driver.massMemory.delete(filename = '1') \n
 		Deletes the specified files. \n
-			:param file_name: File to be deleted. The wildcards * and ? are allowed. Specifying a directory instead of a file is not allowed.
+			:param filename: File to be deleted. The wildcards * and ? are allowed. Specifying a directory instead of a file is not allowed.
 		"""
-		param = Conversions.value_to_quoted_str(file_name)
+		param = Conversions.value_to_quoted_str(filename)
 		self._core.io.write(f'MMEMory:DELete {param}')
 
 	def get_drives(self) -> List[str]:
 		"""SCPI: MMEMory:DRIVes \n
 		Snippet: value: List[str] = driver.massMemory.get_drives() \n
 		Returns a list of the available drives. \n
 			:return: drive: Comma-separated list of strings, one string per drive
@@ -110,28 +110,28 @@
 		Moves or renames an existing object (file or directory) to a new location. \n
 			:param file_source: Name of the object to be moved or renamed. Wildcards ? and * are only allowed for moving files without renaming.
 			:param file_destination: New name and/or path of the object. Wildcards are not allowed. If a new object name without path is specified, the object is renamed. If a new path without object name is specified, the object is moved to this path. If a new path and a new object name are specified, the object is moved to this path and renamed.
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('file_source', file_source, DataType.String), ArgSingle('file_destination', file_destination, DataType.String))
 		self._core.io.write(f'MMEMory:MOVE {param}'.rstrip())
 
-	def get_store_unit(self) -> str:
+	def get_msis(self) -> str:
 		"""SCPI: MMEMory:MSIS \n
-		Snippet: value: str = driver.massMemory.get_store_unit() \n
+		Snippet: value: str = driver.massMemory.get_msis() \n
 		Changes the default storage unit (drive or server) for mass memory storage. When the default storage unit is changed, it
 		is checked whether the current directory (see method RsCMPX_Base.MassMemory.CurrentDirectory.set) is also available on
 		the new storage unit. If not, the current directory is automatically set to '/'. \n
 			:return: msus: No help available
 		"""
 		response = self._core.io.query_str('MMEMory:MSIS?')
 		return trim_str_response(response)
 
-	def set_store_unit(self, msus: str) -> None:
+	def set_msis(self, msus: str) -> None:
 		"""SCPI: MMEMory:MSIS \n
-		Snippet: driver.massMemory.set_store_unit(msus = '1') \n
+		Snippet: driver.massMemory.set_msis(msus = '1') \n
 		Changes the default storage unit (drive or server) for mass memory storage. When the default storage unit is changed, it
 		is checked whether the current directory (see method RsCMPX_Base.MassMemory.CurrentDirectory.set) is also available on
 		the new storage unit. If not, the current directory is automatically set to '/'. \n
 			:param msus: Default storage unit
 		"""
 		param = Conversions.value_to_quoted_str(msus)
 		self._core.io.write(f'MMEMory:MSIS {param}')
@@ -141,34 +141,34 @@
 		Snippet: driver.massMemory.delete_directory(directory_name = '1') \n
 		Removes an existing empty directory from the mass memory storage system. \n
 			:param directory_name: Wildcards are not allowed.
 		"""
 		param = Conversions.value_to_quoted_str(directory_name)
 		self._core.io.write(f'MMEMory:RDIRectory {param}')
 
-	def save(self, file_name: str, msus: str = None) -> None:
+	def save(self, filename: str, msus: str = None) -> None:
 		"""SCPI: MMEMory:SAV \n
-		Snippet: driver.massMemory.save(file_name = '1', msus = '1') \n
+		Snippet: driver.massMemory.save(filename = '1', msus = '1') \n
 		Stores the current instrument settings to the specified file. This command has the same effect as the combination of *SAV
 		and method RsCMPX_Base.MassMemory.Store.State.set. \n
-			:param file_name: No help available
+			:param filename: No help available
 			:param msus: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('file_name', file_name, DataType.String), ArgSingle('msus', msus, DataType.String, True))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('filename', filename, DataType.String), ArgSingle('msus', msus, DataType.String, True))
 		self._core.io.write(f'MMEMory:SAV {param}'.rstrip())
 
-	def recall(self, file_name: str, msus: str = None) -> None:
+	def recall(self, filename: str, msus: str = None) -> None:
 		"""SCPI: MMEMory:RCL \n
-		Snippet: driver.massMemory.recall(file_name = '1', msus = '1') \n
+		Snippet: driver.massMemory.recall(filename = '1', msus = '1') \n
 		Restores the instrument settings from the specified file. This command has the same effect as the combination of method
 		RsCMPX_Base.MassMemory.Load.State.set and *RCL. \n
-			:param file_name: No help available
+			:param filename: No help available
 			:param msus: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('file_name', file_name, DataType.String), ArgSingle('msus', msus, DataType.String, True))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('filename', filename, DataType.String), ArgSingle('msus', msus, DataType.String, True))
 		self._core.io.write(f'MMEMory:RCL {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class AliasesStruct(StructBase):
 		"""Structure for reading output parameters. Fields: \n
 			- Alias: List[str]: No parameter help available
 			- Path: List[str]: No parameter help available"""
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Attribute.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Attribute.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Catalog.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Catalog_/Length.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Catalog_/Length.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/CurrentDirectory.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/CurrentDirectory.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Dcatalog.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Dcatalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Dcatalog_/Length.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Dcatalog_/Length.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Load.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Load.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Load_/Item.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Load_/Item.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 class Item:
 	"""Item commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("item", core, parent)
 
-	def set(self, item_path: str, file_name: str) -> None:
+	def set(self, item_path: str, filename: str) -> None:
 		"""SCPI: MMEMory:LOAD:ITEM \n
-		Snippet: driver.massMemory.load.item.set(item_path = '1', file_name = '1') \n
+		Snippet: driver.massMemory.load.item.set(item_path = '1', filename = '1') \n
 		Executes a partial recall. That means, restores a selected part of a save file. You can restore all settings of a
 		specific application instance. Or you can restore the list mode settings of a specific measurement application instance. \n
 			:param item_path: No help available
-			:param file_name: No help available
+			:param filename: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('item_path', item_path, DataType.String), ArgSingle('file_name', file_name, DataType.String))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('item_path', item_path, DataType.String), ArgSingle('filename', filename, DataType.String))
 		self._core.io.write(f'MMEMory:LOAD:ITEM {param}'.rstrip())
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Load_/Macro.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Load_/Macro.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 class Macro:
 	"""Macro commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("macro", core, parent)
 
-	def set(self, label: str, file_name: str, msus: str = None) -> None:
+	def set(self, label: str, filename: str, msus: str = None) -> None:
 		"""SCPI: MMEMory:LOAD:MACRo \n
-		Snippet: driver.massMemory.load.macro.set(label = '1', file_name = '1', msus = '1') \n
+		Snippet: driver.massMemory.load.macro.set(label = '1', filename = '1', msus = '1') \n
 		Creates a macro, reading the macro contents from a file. If the label exists already, the macro contents are overwritten.
 		Avoid using labels which are identical with supported remote control commands. In contrast to SCPI stipulations, remote
 		commands have priority over macros. \n
 			:param label: No help available
-			:param file_name: No help available
+			:param filename: No help available
 			:param msus: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('label', label, DataType.String), ArgSingle('file_name', file_name, DataType.String), ArgSingle('msus', msus, DataType.String, True))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('label', label, DataType.String), ArgSingle('filename', filename, DataType.String), ArgSingle('msus', msus, DataType.String, True))
 		self._core.io.write(f'MMEMory:LOAD:MACRo {param}'.rstrip())
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Load_/State.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Load_/State.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 class State:
 	"""State commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("state", core, parent)
 
-	def set(self, sav_rcl_state_number: float, file_name: str, msus: str = None) -> None:
+	def set(self, sav_rcl_state_number: float, filename: str, msus: str = None) -> None:
 		"""SCPI: MMEMory:LOAD:STATe \n
-		Snippet: driver.massMemory.load.state.set(sav_rcl_state_number = 1.0, file_name = '1', msus = '1') \n
+		Snippet: driver.massMemory.load.state.set(sav_rcl_state_number = 1.0, filename = '1', msus = '1') \n
 		Loads the instrument settings from the specified file to the specified internal memory. After the file has been loaded,
 		the settings must be activated using a *RCL command. For more convenience, see method RsCMPX_Base.MassMemory.recall. \n
 			:param sav_rcl_state_number: No help available
-			:param file_name: No help available
+			:param filename: No help available
 			:param msus: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('sav_rcl_state_number', sav_rcl_state_number, DataType.Float), ArgSingle('file_name', file_name, DataType.String), ArgSingle('msus', msus, DataType.String, True))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('sav_rcl_state_number', sav_rcl_state_number, DataType.Float), ArgSingle('filename', filename, DataType.String), ArgSingle('msus', msus, DataType.String, True))
 		self._core.io.write(f'MMEMory:LOAD:STATe {param}'.rstrip())
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Store.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Store.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Store_/Item.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Store_/Item.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 class Item:
 	"""Item commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("item", core, parent)
 
-	def set(self, item_name: str, file_name: str) -> None:
+	def set(self, item_name: str, filename: str) -> None:
 		"""SCPI: MMEMory:STORe:ITEM \n
-		Snippet: driver.massMemory.store.item.set(item_name = '1', file_name = '1') \n
+		Snippet: driver.massMemory.store.item.set(item_name = '1', filename = '1') \n
 		Executes a partial save, i.e. stores a part of the instrument settings to the specified file. You can store all settings
 		of a specific application instance. Or you can store the list mode settings of a specific measurement application
 		instance. \n
 			:param item_name: Part to be saved. ItemName = Application[i][:MEV:LIST] For Application, see method RsCMPX_Base.MassMemory.Load.Item.set. i is the instance of the application. Omitting i stores instance 1. Appending :MEV:LIST stores only the list mode settings.
-			:param file_name: Path and filename of the target file. Wildcards are not allowed.
+			:param filename: Path and filename of the target file. Wildcards are not allowed.
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('item_name', item_name, DataType.String), ArgSingle('file_name', file_name, DataType.String))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('item_name', item_name, DataType.String), ArgSingle('filename', filename, DataType.String))
 		self._core.io.write(f'MMEMory:STORe:ITEM {param}'.rstrip())
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Store_/Macro.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Store_/Macro.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 class Macro:
 	"""Macro commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("macro", core, parent)
 
-	def set(self, label: str, file_name: str, msus: str = None) -> None:
+	def set(self, label: str, filename: str, msus: str = None) -> None:
 		"""SCPI: MMEMory:STORe:MACRo \n
-		Snippet: driver.massMemory.store.macro.set(label = '1', file_name = '1', msus = '1') \n
+		Snippet: driver.massMemory.store.macro.set(label = '1', filename = '1', msus = '1') \n
 		Stores the contents of a macro to a file. If the file exists, it is overwritten. If the file does not exist, it is
 		created. \n
 			:param label: No help available
-			:param file_name: No help available
+			:param filename: No help available
 			:param msus: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('label', label, DataType.String), ArgSingle('file_name', file_name, DataType.String), ArgSingle('msus', msus, DataType.String, True))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('label', label, DataType.String), ArgSingle('filename', filename, DataType.String), ArgSingle('msus', msus, DataType.String, True))
 		self._core.io.write(f'MMEMory:STORe:MACRo {param}'.rstrip())
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/MassMemory_/Store_/State.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/MassMemory_/Store_/State.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 class State:
 	"""State commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("state", core, parent)
 
-	def set(self, sav_rcl_state_number: int, file_name: str, msus: str = None) -> None:
+	def set(self, sav_rcl_state_number: int, filename: str, msus: str = None) -> None:
 		"""SCPI: MMEMory:STORe:STATe \n
-		Snippet: driver.massMemory.store.state.set(sav_rcl_state_number = 1, file_name = '1', msus = '1') \n
+		Snippet: driver.massMemory.store.state.set(sav_rcl_state_number = 1, filename = '1', msus = '1') \n
 		Stores the instrument settings from the specified internal memory to the specified file. To store the current instrument
 		settings to a file, use first *SAV <MemoryNumber> to store the settings to the memory. Then use this command to store the
 		settings from the memory to a file. For more convenience, see method RsCMPX_Base.MassMemory.save. \n
 			:param sav_rcl_state_number: No help available
-			:param file_name: No help available
+			:param filename: No help available
 			:param msus: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('sav_rcl_state_number', sav_rcl_state_number, DataType.Integer), ArgSingle('file_name', file_name, DataType.String), ArgSingle('msus', msus, DataType.String, True))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('sav_rcl_state_number', sav_rcl_state_number, DataType.Integer), ArgSingle('filename', filename, DataType.String), ArgSingle('msus', msus, DataType.String, True))
 		self._core.io.write(f'MMEMory:STORe:STATe {param}'.rstrip())
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Procedure.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Procedure.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/RecallState.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/RecallState.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/SaveState.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/SaveState.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 	"""Base commands group definition. 12 total commands, 3 Sub-groups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("base", core, parent)
 
 	@property
-	def ipSubnet(self):
-		"""ipSubnet commands group. 2 Sub-classes, 0 commands."""
-		if not hasattr(self, '_ipSubnet'):
-			from .Base_.IpSubnet import IpSubnet
-			self._ipSubnet = IpSubnet(self._core, self._base)
-		return self._ipSubnet
+	def ipSet(self):
+		"""ipSet commands group. 2 Sub-classes, 0 commands."""
+		if not hasattr(self, '_ipSet'):
+			from .Base_.IpSet import IpSet
+			self._ipSet = IpSet(self._core, self._base)
+		return self._ipSet
 
 	@property
 	def temperature(self):
 		"""temperature commands group. 2 Sub-classes, 1 commands."""
 		if not hasattr(self, '_temperature'):
 			from .Base_.Temperature import Temperature
 			self._temperature = Temperature(self._core, self._base)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/IpSubnet.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/IpSet.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from ....Internal.Core import Core
 from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class IpSubnet:
-	"""IpSubnet commands group definition. 7 total commands, 2 Sub-groups, 0 group commands"""
+class IpSet:
+	"""IpSet commands group definition. 7 total commands, 2 Sub-groups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ipSubnet", core, parent)
+		self._base = CommandsGroup("ipSet", core, parent)
 
 	@property
 	def snode(self):
 		"""snode commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_snode'):
-			from .IpSubnet_.Snode import Snode
+			from .IpSet_.Snode import Snode
 			self._snode = Snode(self._core, self._base)
 		return self._snode
 
 	@property
 	def subMonitor(self):
 		"""subMonitor commands group. 0 Sub-classes, 4 commands."""
 		if not hasattr(self, '_subMonitor'):
-			from .IpSubnet_.SubMonitor import SubMonitor
+			from .IpSet_.SubMonitor import SubMonitor
 			self._subMonitor = SubMonitor(self._core, self._base)
 		return self._subMonitor
 
-	def clone(self) -> 'IpSubnet':
+	def clone(self) -> 'IpSet':
 		"""Clones the group by creating new object from it and its whole existing sub-groups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = IpSubnet(self._core, self._base.parent)
+		new_group = IpSet(self._core, self._base.parent)
 		self._base.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/IpSubnet_/Snode.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/IpSet_/Snode.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("snode", core, parent)
 
 	def get_nname(self) -> str:
 		"""SCPI: SENSe:BASE:IPSet:SNODe:NNAMe \n
-		Snippet: value: str = driver.sense.base.ipSubnet.snode.get_nname() \n
+		Snippet: value: str = driver.sense.base.ipSet.snode.get_nname() \n
 		No command help available \n
 			:return: name: No help available
 		"""
 		response = self._core.io.query_str('SENSe:BASE:IPSet:SNODe:NNAMe?')
 		return trim_str_response(response)
 
 	def get_ntype(self) -> str:
 		"""SCPI: SENSe:BASE:IPSet:SNODe:NTYPe \n
-		Snippet: value: str = driver.sense.base.ipSubnet.snode.get_ntype() \n
+		Snippet: value: str = driver.sense.base.ipSet.snode.get_ntype() \n
 		No command help available \n
 			:return: type_py: No help available
 		"""
 		response = self._core.io.query_str('SENSe:BASE:IPSet:SNODe:NTYPe?')
 		return trim_str_response(response)
 
 	# noinspection PyTypeChecker
@@ -48,12 +48,12 @@
 			self.Selected_Segment: enums.Segment = None
 			self.Ip_Address: str = None
 			self.Subnet_Mask: str = None
 
 	# noinspection PyTypeChecker
 	def get_nsegment(self) -> NsegmentStruct:
 		"""SCPI: SENSe:BASE:IPSet:SNODe:NSEGment \n
-		Snippet: value: NsegmentStruct = driver.sense.base.ipSubnet.snode.get_nsegment() \n
+		Snippet: value: NsegmentStruct = driver.sense.base.ipSet.snode.get_nsegment() \n
 		No command help available \n
 			:return: structure: for return value, see the help for NsegmentStruct structure arguments.
 		"""
 		return self._core.io.query_struct('SENSe:BASE:IPSet:SNODe:NSEGment?', self.__class__.NsegmentStruct())
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/IpSubnet_/SubMonitor.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/IpSet_/SubMonitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,40 +11,40 @@
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("subMonitor", core, parent)
 
 	def get_name(self) -> List[str]:
 		"""SCPI: SENSe:BASE:IPSet:SMONitor:NAME \n
-		Snippet: value: List[str] = driver.sense.base.ipSubnet.subMonitor.get_name() \n
+		Snippet: value: List[str] = driver.sense.base.ipSet.subMonitor.get_name() \n
 		No command help available \n
 			:return: names: No help available
 		"""
 		response = self._core.io.query_str('SENSe:BASE:IPSet:SMONitor:NAME?')
 		return Conversions.str_to_str_list(response)
 
 	def get_type_py(self) -> List[str]:
 		"""SCPI: SENSe:BASE:IPSet:SMONitor:TYPE \n
-		Snippet: value: List[str] = driver.sense.base.ipSubnet.subMonitor.get_type_py() \n
+		Snippet: value: List[str] = driver.sense.base.ipSet.subMonitor.get_type_py() \n
 		No command help available \n
 			:return: types: No help available
 		"""
 		response = self._core.io.query_str('SENSe:BASE:IPSet:SMONitor:TYPE?')
 		return Conversions.str_to_str_list(response)
 
 	def get_id(self) -> List[int]:
 		"""SCPI: SENSe:BASE:IPSet:SMONitor:ID \n
-		Snippet: value: List[int] = driver.sense.base.ipSubnet.subMonitor.get_id() \n
+		Snippet: value: List[int] = driver.sense.base.ipSet.subMonitor.get_id() \n
 		No command help available \n
 			:return: ids: No help available
 		"""
 		response = self._core.io.query_bin_or_ascii_int_list('SENSe:BASE:IPSet:SMONitor:ID?')
 		return response
 
 	def get_description(self) -> List[str]:
 		"""SCPI: SENSe:BASE:IPSet:SMONitor:DESCription \n
-		Snippet: value: List[str] = driver.sense.base.ipSubnet.subMonitor.get_description() \n
+		Snippet: value: List[str] = driver.sense.base.ipSet.subMonitor.get_description() \n
 		No command help available \n
 			:return: descriptions: No help available
 		"""
 		response = self._core.io.query_str('SENSe:BASE:IPSet:SMONitor:DESCription?')
 		return Conversions.str_to_str_list(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/Reference.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/Reference.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/Reference_/Frequency.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/Reference_/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/Temperature.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/Temperature.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/Temperature_/Exceeded.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/Temperature_/Exceeded.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/Base_/Temperature_/Operating.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/Base_/Temperature_/Operating.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Sense_/FirmwareUpdate.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Sense_/FirmwareUpdate.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Source.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Source.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Source_/Base.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Source_/Base.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Source_/Base_/Adjustment.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Source_/Base_/Adjustment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Source_/Base_/Adjustment_/State.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Source_/Base_/Adjustment_/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Condition.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Condition.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Condition_/Bits.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Condition_/Bits.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Condition_/Bits_/All.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Condition_/Bits_/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Condition_/Bits_/Cataloge.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Event_/Bits_/Next.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-from typing import List
-
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
-from .....Internal import Conversions
 from .....Internal.Types import DataType
+from .....Internal.Utilities import trim_str_response
 from .....Internal.ArgSingleList import ArgSingleList
 from .....Internal.ArgSingle import ArgSingle
 from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Cataloge:
-	"""Cataloge commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class Next:
+	"""Next commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("cataloge", core, parent)
+		self._base = CommandsGroup("next", core, parent)
 
-	def get(self, filter_py: str = None, mode: enums.ExpressionMode = None) -> List[str]:
-		"""SCPI: STATus:CONDition:BITS:CATaloge \n
-		Snippet: value: List[str] = driver.status.condition.bits.cataloge.get(filter_py = '1', mode = enums.ExpressionMode.REGex) \n
+	def get(self, filter_py: str = None, mode: enums.ExpressionMode = None) -> str:
+		"""SCPI: STATus:EVENt:BITS:NEXT \n
+		Snippet: value: str = driver.status.event.bits.next.get(filter_py = '1', mode = enums.ExpressionMode.REGex) \n
 		No command help available \n
 			:param filter_py: No help available
 			:param mode: No help available
 			:return: bit: No help available"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('filter_py', filter_py, DataType.String, True), ArgSingle('mode', mode, DataType.Enum, True))
-		response = self._core.io.query_str(f'STATus:CONDition:BITS:CATaloge? {param}'.rstrip())
-		return Conversions.str_to_str_list(response)
+		response = self._core.io.query_str(f'STATus:EVENt:BITS:NEXT? {param}'.rstrip())
+		return trim_str_response(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Condition_/Bits_/Count.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Condition_/Bits_/Count.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Event.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Event.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Event_/Bits.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Event_/Bits.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Event_/Bits_/All.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Event_/Bits_/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Event_/Bits_/Count.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Event_/Bits_/Count.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Event_/Bits_/Next.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/Off.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 from .....Internal.Utilities import trim_str_response
 from .....Internal.ArgSingleList import ArgSingleList
 from .....Internal.ArgSingle import ArgSingle
 from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Next:
-	"""Next commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class Off:
+	"""Off commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("next", core, parent)
+		self._base = CommandsGroup("off", core, parent)
 
 	def get(self, filter_py: str = None, mode: enums.ExpressionMode = None) -> str:
-		"""SCPI: STATus:EVENt:BITS:NEXT \n
-		Snippet: value: str = driver.status.event.bits.next.get(filter_py = '1', mode = enums.ExpressionMode.REGex) \n
+		"""SCPI: STATus:MEASurement:CONDition:OFF \n
+		Snippet: value: str = driver.status.measurement.condition.off.get(filter_py = '1', mode = enums.ExpressionMode.REGex) \n
 		No command help available \n
 			:param filter_py: No help available
 			:param mode: No help available
-			:return: bit: No help available"""
+			:return: bitname: No help available"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('filter_py', filter_py, DataType.String, True), ArgSingle('mode', mode, DataType.Enum, True))
-		response = self._core.io.query_str(f'STATus:EVENt:BITS:NEXT? {param}'.rstrip())
+		response = self._core.io.query_str(f'STATus:MEASurement:CONDition:OFF? {param}'.rstrip())
 		return trim_str_response(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Generator.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Generator.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Generator_/Condition.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Generator_/Condition.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Generator_/Condition_/Off.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Generator_/Condition_/Off.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Generator_/Condition_/On.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Generator_/Condition_/On.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Generator_/Condition_/Pending.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/Rdy.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 from .....Internal.Utilities import trim_str_response
 from .....Internal.ArgSingleList import ArgSingleList
 from .....Internal.ArgSingle import ArgSingle
 from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Pending:
-	"""Pending commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class Rdy:
+	"""Rdy commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("pending", core, parent)
+		self._base = CommandsGroup("rdy", core, parent)
 
 	def get(self, filter_py: str = None, mode: enums.ExpressionMode = None) -> str:
-		"""SCPI: STATus:GENerator:CONDition:PENDing \n
-		Snippet: value: str = driver.status.generator.condition.pending.get(filter_py = '1', mode = enums.ExpressionMode.REGex) \n
+		"""SCPI: STATus:MEASurement:CONDition:RDY \n
+		Snippet: value: str = driver.status.measurement.condition.rdy.get(filter_py = '1', mode = enums.ExpressionMode.REGex) \n
 		No command help available \n
 			:param filter_py: No help available
 			:param mode: No help available
 			:return: bitname: No help available"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('filter_py', filter_py, DataType.String, True), ArgSingle('mode', mode, DataType.Enum, True))
-		response = self._core.io.query_str(f'STATus:GENerator:CONDition:PENDing? {param}'.rstrip())
+		response = self._core.io.query_str(f'STATus:MEASurement:CONDition:RDY? {param}'.rstrip())
 		return trim_str_response(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Measurement.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Measurement_/Condition.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Measurement_/Condition.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/Off.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/Qued.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 from .....Internal.Utilities import trim_str_response
 from .....Internal.ArgSingleList import ArgSingleList
 from .....Internal.ArgSingle import ArgSingle
 from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Off:
-	"""Off commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class Qued:
+	"""Qued commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("off", core, parent)
+		self._base = CommandsGroup("qued", core, parent)
 
 	def get(self, filter_py: str = None, mode: enums.ExpressionMode = None) -> str:
-		"""SCPI: STATus:MEASurement:CONDition:OFF \n
-		Snippet: value: str = driver.status.measurement.condition.off.get(filter_py = '1', mode = enums.ExpressionMode.REGex) \n
+		"""SCPI: STATus:MEASurement:CONDition:QUED \n
+		Snippet: value: str = driver.status.measurement.condition.qued.get(filter_py = '1', mode = enums.ExpressionMode.REGex) \n
 		No command help available \n
 			:param filter_py: No help available
 			:param mode: No help available
 			:return: bitname: No help available"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('filter_py', filter_py, DataType.String, True), ArgSingle('mode', mode, DataType.Enum, True))
-		response = self._core.io.query_str(f'STATus:MEASurement:CONDition:OFF? {param}'.rstrip())
+		response = self._core.io.query_str(f'STATus:MEASurement:CONDition:QUED? {param}'.rstrip())
 		return trim_str_response(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/Qued.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Help_/Headers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
-from .....Internal.Types import DataType
-from .....Internal.Utilities import trim_str_response
-from .....Internal.ArgSingleList import ArgSingleList
-from .....Internal.ArgSingle import ArgSingle
-from ..... import enums
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
+from ....Internal.Types import DataType
+from ....Internal.ArgSingleList import ArgSingleList
+from ....Internal.ArgSingle import ArgSingle
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Qued:
-	"""Qued commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class Headers:
+	"""Headers commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("qued", core, parent)
+		self._base = CommandsGroup("headers", core, parent)
 
-	def get(self, filter_py: str = None, mode: enums.ExpressionMode = None) -> str:
-		"""SCPI: STATus:MEASurement:CONDition:QUED \n
-		Snippet: value: str = driver.status.measurement.condition.qued.get(filter_py = '1', mode = enums.ExpressionMode.REGex) \n
+	def get(self, parser: str = None) -> bytes:
+		"""SCPI: SYSTem:HELP:HEADers \n
+		Snippet: value: bytes = driver.system.help.headers.get(parser = '1') \n
 		No command help available \n
-			:param filter_py: No help available
-			:param mode: No help available
-			:return: bitname: No help available"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('filter_py', filter_py, DataType.String, True), ArgSingle('mode', mode, DataType.Enum, True))
-		response = self._core.io.query_str(f'STATus:MEASurement:CONDition:QUED? {param}'.rstrip())
-		return trim_str_response(response)
+			:param parser: No help available
+			:return: headers: No help available"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('parser', parser, DataType.String, True))
+		response = self._core.io.query_bin_block_ERROR(f'SYSTem:HELP:HEADers? {param}'.rstrip())
+		return response
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/Rdy.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Write_/Eeprom_/Data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
-from .....Internal.Types import DataType
-from .....Internal.Utilities import trim_str_response
-from .....Internal.ArgSingleList import ArgSingleList
-from .....Internal.ArgSingle import ArgSingle
-from ..... import enums
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
+from ....Internal.Types import DataType
+from ....Internal.ArgSingleList import ArgSingleList
+from ....Internal.ArgSingle import ArgSingle
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Rdy:
-	"""Rdy commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class Data:
+	"""Data commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("rdy", core, parent)
+		self._base = CommandsGroup("data", core, parent)
 
-	def get(self, filter_py: str = None, mode: enums.ExpressionMode = None) -> str:
-		"""SCPI: STATus:MEASurement:CONDition:RDY \n
-		Snippet: value: str = driver.status.measurement.condition.rdy.get(filter_py = '1', mode = enums.ExpressionMode.REGex) \n
+	def set(self, path: str, reserve: str) -> None:
+		"""SCPI: WRITe:EEPRom:DATA \n
+		Snippet: driver.write.eeprom.data.set(path = '1', reserve = '1') \n
 		No command help available \n
-			:param filter_py: No help available
-			:param mode: No help available
-			:return: bitname: No help available"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('filter_py', filter_py, DataType.String, True), ArgSingle('mode', mode, DataType.Enum, True))
-		response = self._core.io.query_str(f'STATus:MEASurement:CONDition:RDY? {param}'.rstrip())
-		return trim_str_response(response)
+			:param path: No help available
+			:param reserve: No help available
+		"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('path', path, DataType.String), ArgSingle('reserve', reserve, DataType.String))
+		self._core.io.write(f'WRITe:EEPRom:DATA {param}'.rstrip())
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/Run.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/SdReached.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 from .....Internal.Utilities import trim_str_response
 from .....Internal.ArgSingleList import ArgSingleList
 from .....Internal.ArgSingle import ArgSingle
 from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Run:
-	"""Run commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class SdReached:
+	"""SdReached commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("run", core, parent)
+		self._base = CommandsGroup("sdReached", core, parent)
 
 	def get(self, filter_py: str = None, mode: enums.ExpressionMode = None) -> str:
-		"""SCPI: STATus:MEASurement:CONDition:RUN \n
-		Snippet: value: str = driver.status.measurement.condition.run.get(filter_py = '1', mode = enums.ExpressionMode.REGex) \n
+		"""SCPI: STATus:MEASurement:CONDition:SDReached \n
+		Snippet: value: str = driver.status.measurement.condition.sdReached.get(filter_py = '1', mode = enums.ExpressionMode.REGex) \n
 		No command help available \n
 			:param filter_py: No help available
 			:param mode: No help available
 			:return: bitname: No help available"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('filter_py', filter_py, DataType.String, True), ArgSingle('mode', mode, DataType.Enum, True))
-		response = self._core.io.query_str(f'STATus:MEASurement:CONDition:RUN? {param}'.rstrip())
+		response = self._core.io.query_str(f'STATus:MEASurement:CONDition:SDReached? {param}'.rstrip())
 		return trim_str_response(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Measurement_/Condition_/SdReached.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Option_/Description.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 from .....Internal.Utilities import trim_str_response
 from .....Internal.ArgSingleList import ArgSingleList
 from .....Internal.ArgSingle import ArgSingle
 from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class SdReached:
-	"""SdReached commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class Description:
+	"""Description commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("sdReached", core, parent)
+		self._base = CommandsGroup("description", core, parent)
 
-	def get(self, filter_py: str = None, mode: enums.ExpressionMode = None) -> str:
-		"""SCPI: STATus:MEASurement:CONDition:SDReached \n
-		Snippet: value: str = driver.status.measurement.condition.sdReached.get(filter_py = '1', mode = enums.ExpressionMode.REGex) \n
+	def get(self, product_type: enums.ProductType = None, validity: enums.ValidityScope = None, scope: enums.ValidityScopeB = None, instrument_no: float = None) -> str:
+		"""SCPI: SYSTem:BASE:OPTion:DESCription \n
+		Snippet: value: str = driver.system.base.option.description.get(product_type = enums.ProductType.ALL, validity = enums.ValidityScope.ALL, scope = enums.ValidityScopeB.INSTrument, instrument_no = 1.0) \n
 		No command help available \n
-			:param filter_py: No help available
-			:param mode: No help available
-			:return: bitname: No help available"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('filter_py', filter_py, DataType.String, True), ArgSingle('mode', mode, DataType.Enum, True))
-		response = self._core.io.query_str(f'STATus:MEASurement:CONDition:SDReached? {param}'.rstrip())
+			:param product_type: No help available
+			:param validity: No help available
+			:param scope: No help available
+			:param instrument_no: No help available
+			:return: option_list: No help available"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('product_type', product_type, DataType.Enum, True), ArgSingle('validity', validity, DataType.Enum, True), ArgSingle('scope', scope, DataType.Enum, True), ArgSingle('instrument_no', instrument_no, DataType.Float, True))
+		response = self._core.io.query_str(f'SYSTem:BASE:OPTion:DESCription? {param}'.rstrip())
 		return trim_str_response(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Operation.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Operation.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Operation_/Bit.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Operation_/Bit.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/Condition.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/Condition.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/Enable.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/Enable.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/Event.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/Event.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/Ntransition.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/Ntransition.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/Ptransition.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Operation_/Bit_/Ptransition.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Questionable.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Questionable.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Questionable_/Bit.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Questionable_/Bit.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/Condition.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/Condition.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/Enable.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/Enable.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/Event.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Cmw_/Device_/Id.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
-from .....Internal import Conversions
+from .....Internal.Utilities import trim_str_response
 from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Event:
-	"""Event commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class Id:
+	"""Id commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("event", core, parent)
+		self._base = CommandsGroup("id", core, parent)
 
-	def get(self, bitNr=repcap.BitNr.Default) -> bool:
-		"""SCPI: STATus:QUEStionable:BIT<bitno>[:EVENt] \n
-		Snippet: value: bool = driver.status.questionable.bit.event.get(bitNr = repcap.BitNr.Default) \n
+	def get(self, cmwVariant=repcap.CmwVariant.Default) -> str:
+		"""SCPI: SYSTem:CMW<n>:DEVice:ID \n
+		Snippet: value: str = driver.system.cmw.device.id.get(cmwVariant = repcap.CmwVariant.Default) \n
 		No command help available \n
-			:param bitNr: optional repeated capability selector. Default value: Nr8 (settable in the interface 'Bit')
-			:return: register_bit: No help available"""
-		bitNr_cmd_val = self._base.get_repcap_cmd_value(bitNr, repcap.BitNr)
-		response = self._core.io.query_str(f'STATus:QUEStionable:BIT{bitNr_cmd_val}:EVENt?')
-		return Conversions.str_to_bool(response)
+			:param cmwVariant: optional repeated capability selector. Default value: Cmw1 (settable in the interface 'Cmw')
+			:return: idn: No help available"""
+		cmwVariant_cmd_val = self._base.get_repcap_cmd_value(cmwVariant, repcap.CmwVariant)
+		response = self._core.io.query_str(f'SYSTem:CMW{cmwVariant_cmd_val}:DEVice:ID?')
+		return trim_str_response(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/Ntransition.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/Ntransition.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/Ptransition.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Questionable_/Bit_/Ptransition.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Status_/Queue.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Status_/Queue.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,23 +197,23 @@
 		Snippet: driver.system.set_klock(klock = False) \n
 		No command help available \n
 			:param klock: No help available
 		"""
 		param = Conversions.bool_to_str(klock)
 		self._core.io.write(f'SYSTem:KLOCk {param}')
 
-	def preset(self, applname_and_linumber: str = None) -> None:
+	def preset(self, appl_name_and_li_number: str = None) -> None:
 		"""SCPI: SYSTem:PRESet \n
-		Snippet: driver.system.preset(applname_and_linumber = '1') \n
+		Snippet: driver.system.preset(appl_name_and_li_number = '1') \n
 		No command help available \n
-			:param applname_and_linumber: No help available
+			:param appl_name_and_li_number: No help available
 		"""
 		param = ''
-		if applname_and_linumber:
-			param = Conversions.value_to_quoted_str(applname_and_linumber)
+		if appl_name_and_li_number:
+			param = Conversions.value_to_quoted_str(appl_name_and_li_number)
 		self._core.io.write(f'SYSTem:PRESet {param}'.strip())
 
 	def preset_all(self) -> None:
 		"""SCPI: SYSTem:PRESet:ALL \n
 		Snippet: driver.system.preset_all() \n
 		No command help available \n
 		"""
@@ -238,23 +238,23 @@
 		"""SCPI: SYSTem:PRESet:BASE \n
 		Snippet: driver.system.preset_base_with_opc() \n
 		No command help available \n
 		Same as preset_base, but waits for the operation to complete before continuing further. Use the RsCMPX_Base.utilities.opc_timeout_set() to set the timeout value. \n
 		"""
 		self._core.io.write_with_opc(f'SYSTem:PRESet:BASE')
 
-	def reset(self, applname_and_linumber: str = None) -> None:
+	def reset(self, appl_name_and_li_number: str = None) -> None:
 		"""SCPI: SYSTem:RESet \n
-		Snippet: driver.system.reset(applname_and_linumber = '1') \n
+		Snippet: driver.system.reset(appl_name_and_li_number = '1') \n
 		No command help available \n
-			:param applname_and_linumber: No help available
+			:param appl_name_and_li_number: No help available
 		"""
 		param = ''
-		if applname_and_linumber:
-			param = Conversions.value_to_quoted_str(applname_and_linumber)
+		if appl_name_and_li_number:
+			param = Conversions.value_to_quoted_str(appl_name_and_li_number)
 		self._core.io.write(f'SYSTem:RESet {param}'.strip())
 
 	def reset_all(self) -> None:
 		"""SCPI: SYSTem:RESet:ALL \n
 		Snippet: driver.system.reset_all() \n
 		No command help available \n
 		"""
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 	"""Base commands group definition. 30 total commands, 8 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("base", core, parent)
 
 	@property
-	def ipSubnet(self):
-		"""ipSubnet commands group. 1 Sub-classes, 0 commands."""
-		if not hasattr(self, '_ipSubnet'):
-			from .Base_.IpSubnet import IpSubnet
-			self._ipSubnet = IpSubnet(self._core, self._base)
-		return self._ipSubnet
+	def ipSet(self):
+		"""ipSet commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_ipSet'):
+			from .Base_.IpSet import IpSet
+			self._ipSet = IpSet(self._core, self._base)
+		return self._ipSet
 
 	@property
 	def device(self):
 		"""device commands group. 0 Sub-classes, 7 commands."""
 		if not hasattr(self, '_device'):
 			from .Base_.Device import Device
 			self._device = Device(self._core, self._base)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Device.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Device.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Display.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Display.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,26 +31,26 @@
 		self._core.io.write(f'SYSTem:BASE:DISPlay:MWINdow {param}')
 
 	# noinspection PyTypeChecker
 	def get_color_set(self) -> enums.ColorSet:
 		"""SCPI: SYSTem:BASE:DISPlay:COLorset \n
 		Snippet: value: enums.ColorSet = driver.system.base.display.get_color_set() \n
 		No command help available \n
-			:return: colorset: No help available
+			:return: color_set: No help available
 		"""
 		response = self._core.io.query_str('SYSTem:BASE:DISPlay:COLorset?')
 		return Conversions.str_to_scalar_enum(response, enums.ColorSet)
 
-	def set_color_set(self, colorset: enums.ColorSet) -> None:
+	def set_color_set(self, color_set: enums.ColorSet) -> None:
 		"""SCPI: SYSTem:BASE:DISPlay:COLorset \n
-		Snippet: driver.system.base.display.set_color_set(colorset = enums.ColorSet.DEF) \n
+		Snippet: driver.system.base.display.set_color_set(color_set = enums.ColorSet.DEF) \n
 		No command help available \n
-			:param colorset: No help available
+			:param color_set: No help available
 		"""
-		param = Conversions.enum_scalar_to_str(colorset, enums.ColorSet)
+		param = Conversions.enum_scalar_to_str(color_set, enums.ColorSet)
 		self._core.io.write(f'SYSTem:BASE:DISPlay:COLorset {param}')
 
 	# noinspection PyTypeChecker
 	def get_font_set(self) -> enums.FontType:
 		"""SCPI: SYSTem:BASE:DISPlay:FONTset \n
 		Snippet: value: enums.FontType = driver.system.base.display.get_font_set() \n
 		No command help available \n
@@ -65,30 +65,30 @@
 		No command help available \n
 			:param fonset: No help available
 		"""
 		param = Conversions.enum_scalar_to_str(fonset, enums.FontType)
 		self._core.io.write(f'SYSTem:BASE:DISPlay:FONTset {param}')
 
 	# noinspection PyTypeChecker
-	def get_roll_keymode(self) -> enums.RollkeyMode:
+	def get_rollkey_mode(self) -> enums.RollkeyMode:
 		"""SCPI: SYSTem:BASE:DISPlay:ROLLkeymode \n
-		Snippet: value: enums.RollkeyMode = driver.system.base.display.get_roll_keymode() \n
+		Snippet: value: enums.RollkeyMode = driver.system.base.display.get_rollkey_mode() \n
 		No command help available \n
-			:return: rollkeymode: No help available
+			:return: rollkey_mode: No help available
 		"""
 		response = self._core.io.query_str('SYSTem:BASE:DISPlay:ROLLkeymode?')
 		return Conversions.str_to_scalar_enum(response, enums.RollkeyMode)
 
-	def set_roll_keymode(self, rollkeymode: enums.RollkeyMode) -> None:
+	def set_rollkey_mode(self, rollkey_mode: enums.RollkeyMode) -> None:
 		"""SCPI: SYSTem:BASE:DISPlay:ROLLkeymode \n
-		Snippet: driver.system.base.display.set_roll_keymode(rollkeymode = enums.RollkeyMode.CURSors) \n
+		Snippet: driver.system.base.display.set_rollkey_mode(rollkey_mode = enums.RollkeyMode.CURSors) \n
 		No command help available \n
-			:param rollkeymode: No help available
+			:param rollkey_mode: No help available
 		"""
-		param = Conversions.enum_scalar_to_str(rollkeymode, enums.RollkeyMode)
+		param = Conversions.enum_scalar_to_str(rollkey_mode, enums.RollkeyMode)
 		self._core.io.write(f'SYSTem:BASE:DISPlay:ROLLkeymode {param}')
 
 	# noinspection PyTypeChecker
 	def get_language(self) -> enums.DisplayLanguage:
 		"""SCPI: SYSTem:BASE:DISPlay:LANGuage \n
 		Snippet: value: enums.DisplayLanguage = driver.system.base.display.get_language() \n
 		No command help available \n
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/IpSubnet.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/IpSet.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from ....Internal.Core import Core
 from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class IpSubnet:
-	"""IpSubnet commands group definition. 1 total commands, 1 Sub-groups, 0 group commands"""
+class IpSet:
+	"""IpSet commands group definition. 1 total commands, 1 Sub-groups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ipSubnet", core, parent)
+		self._base = CommandsGroup("ipSet", core, parent)
 
 	@property
 	def subMonitor(self):
 		"""subMonitor commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_subMonitor'):
-			from .IpSubnet_.SubMonitor import SubMonitor
+			from .IpSet_.SubMonitor import SubMonitor
 			self._subMonitor = SubMonitor(self._core, self._base)
 		return self._subMonitor
 
-	def clone(self) -> 'IpSubnet':
+	def clone(self) -> 'IpSet':
 		"""Clones the group by creating new object from it and its whole existing sub-groups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = IpSubnet(self._core, self._base.parent)
+		new_group = IpSet(self._core, self._base.parent)
 		self._base.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/IpSubnet_/SubMonitor.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/IpSet_/SubMonitor.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/IpSubnet_/SubMonitor_/Refresh.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/IpSet_/SubMonitor_/Refresh.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("refresh", core, parent)
 
 	def set(self) -> None:
 		"""SCPI: SYSTem:BASE:IPSet:SMONitor:REFResh \n
-		Snippet: driver.system.base.ipSubnet.subMonitor.refresh.set() \n
+		Snippet: driver.system.base.ipSet.subMonitor.refresh.set() \n
 		No command help available \n
 		"""
 		self._core.io.write(f'SYSTem:BASE:IPSet:SMONitor:REFResh')
 
 	def set_with_opc(self) -> None:
 		"""SCPI: SYSTem:BASE:IPSet:SMONitor:REFResh \n
-		Snippet: driver.system.base.ipSubnet.subMonitor.refresh.set_with_opc() \n
+		Snippet: driver.system.base.ipSet.subMonitor.refresh.set_with_opc() \n
 		No command help available \n
 		Same as set, but waits for the operation to complete before continuing further. Use the RsCMPX_Base.utilities.opc_timeout_set() to set the timeout value. \n
 		"""
 		self._core.io.write_with_opc(f'SYSTem:BASE:IPSet:SMONitor:REFResh')
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Option.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Option.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Option_/Description.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Password_/Cenable.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
 from .....Internal.Types import DataType
-from .....Internal.Utilities import trim_str_response
 from .....Internal.ArgSingleList import ArgSingleList
 from .....Internal.ArgSingle import ArgSingle
 from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Description:
-	"""Description commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class Cenable:
+	"""Cenable commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("description", core, parent)
+		self._base = CommandsGroup("cenable", core, parent)
 
-	def get(self, producttype: enums.ProductType = None, validity: enums.ValidityScope = None, scope: enums.ValidityScopeB = None, instrumentno: float = None) -> str:
-		"""SCPI: SYSTem:BASE:OPTion:DESCription \n
-		Snippet: value: str = driver.system.base.option.description.get(producttype = enums.ProductType.ALL, validity = enums.ValidityScope.ALL, scope = enums.ValidityScopeB.INSTrument, instrumentno = 1.0) \n
+	# noinspection PyTypeChecker
+	def get_state(self) -> enums.UserRole:
+		"""SCPI: SYSTem:BASE:PASSword[:CENable]:STATe \n
+		Snippet: value: enums.UserRole = driver.system.base.password.cenable.get_state() \n
 		No command help available \n
-			:param producttype: No help available
-			:param validity: No help available
-			:param scope: No help available
-			:param instrumentno: No help available
-			:return: optionlist: No help available"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('producttype', producttype, DataType.Enum, True), ArgSingle('validity', validity, DataType.Enum, True), ArgSingle('scope', scope, DataType.Enum, True), ArgSingle('instrumentno', instrumentno, DataType.Float, True))
-		response = self._core.io.query_str(f'SYSTem:BASE:OPTion:DESCription? {param}'.rstrip())
-		return trim_str_response(response)
+			:return: user_mode: No help available
+		"""
+		response = self._core.io.query_str('SYSTem:BASE:PASSword:CENable:STATe?')
+		return Conversions.str_to_scalar_enum(response, enums.UserRole)
+
+	def set(self, user_mode: enums.UserRole, password: str) -> None:
+		"""SCPI: SYSTem:BASE:PASSword[:CENable] \n
+		Snippet: driver.system.base.password.cenable.set(user_mode = enums.UserRole.ADMin, password = '1') \n
+		No command help available \n
+			:param user_mode: No help available
+			:param password: No help available
+		"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('user_mode', user_mode, DataType.Enum), ArgSingle('password', password, DataType.String))
+		self._core.io.write(f'SYSTem:BASE:PASSword:CENable {param}'.rstrip())
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Option_/ListPy.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Option_/ListPy.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 class ListPy:
 	"""ListPy commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("listPy", core, parent)
 
-	def get(self, producttype: enums.ProductType = None, validity: enums.ValidityScope = None, scope: enums.ValidityScopeB = None, instrumentno: float = None) -> str:
+	def get(self, product_type: enums.ProductType = None, validity: enums.ValidityScope = None, scope: enums.ValidityScopeB = None, instrument_no: float = None) -> str:
 		"""SCPI: SYSTem:BASE:OPTion:LIST \n
-		Snippet: value: str = driver.system.base.option.listPy.get(producttype = enums.ProductType.ALL, validity = enums.ValidityScope.ALL, scope = enums.ValidityScopeB.INSTrument, instrumentno = 1.0) \n
+		Snippet: value: str = driver.system.base.option.listPy.get(product_type = enums.ProductType.ALL, validity = enums.ValidityScope.ALL, scope = enums.ValidityScopeB.INSTrument, instrument_no = 1.0) \n
 		Returns a list of installed software options (licenses) , hardware options, software packages and firmware applications.
 		The list can be filtered using the described parameters. If filtering results in an empty list, a '0' is returned.
 			INTRO_CMD_HELP: The meaning of the filter <Validity> depends on the <OptionType> as follows: \n
 			- A software option is valid if there is an active license key for it. The value 'FUNCtional' is not relevant.
 			- A hardware option is functional if the corresponding hardware and all its components can be used (no defect detected) . The value 'VALid' is not relevant.
 			- A firmware application is functional if the required hardware, software and license keys are available and functional. The value 'VALid' is not relevant.
 			- For software packages, the filter has no effect.  \n
-			:param producttype: No help available
+			:param product_type: No help available
 			:param validity: List only functional entries or only valid entries. By default or if ALL is selected, the list is not filtered according to the validity.
 			:param scope: No help available
-			:param instrumentno: No help available
-			:return: optionlist: No help available"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('producttype', producttype, DataType.Enum, True), ArgSingle('validity', validity, DataType.Enum, True), ArgSingle('scope', scope, DataType.Enum, True), ArgSingle('instrumentno', instrumentno, DataType.Float, True))
+			:param instrument_no: No help available
+			:return: option_list: No help available"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('product_type', product_type, DataType.Enum, True), ArgSingle('validity', validity, DataType.Enum, True), ArgSingle('scope', scope, DataType.Enum, True), ArgSingle('instrument_no', instrument_no, DataType.Float, True))
 		response = self._core.io.query_str(f'SYSTem:BASE:OPTion:LIST? {param}'.rstrip())
 		return trim_str_response(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Option_/Version.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Option_/Version.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,11 +18,11 @@
 		"""SCPI: SYSTem:BASE:OPTion:VERSion \n
 		Snippet: value: str = driver.system.base.option.version.get(applicname = '1') \n
 		Returns version information for installed software packages.
 			INTRO_CMD_HELP: You can either query a list of all installed packages and their versions or you can query the version of a single package specified via <Application>: \n
 			- <Application> specified: A string is returned, indicating the version of the <Application>. If the specified <Application> is unknown / not installed, '0' is returned.
 			- <Application> omitted: A string is returned, containing a list of all installed software packages and their version in the format '<PackageName1>,<Version1>;<PackageName2>,<Version2>;...'  \n
 			:param applicname: Software package for which the version is queried
-			:return: optionlist: Single version or list of applications and versions"""
+			:return: option_list: Single version or list of applications and versions"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('applicname', applicname, DataType.String, True))
 		response = self._core.io.query_str(f'SYSTem:BASE:OPTion:VERSion? {param}'.rstrip())
 		return trim_str_response(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Password.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Password.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 	def cenable(self):
 		"""cenable commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_cenable'):
 			from .Password_.Cenable import Cenable
 			self._cenable = Cenable(self._core, self._base)
 		return self._cenable
 
-	def set_cdisable(self, usermode: enums.UserRole) -> None:
+	def set_cdisable(self, user_mode: enums.UserRole) -> None:
 		"""SCPI: SYSTem:BASE:PASSword:CDISable \n
-		Snippet: driver.system.base.password.set_cdisable(usermode = enums.UserRole.ADMin) \n
+		Snippet: driver.system.base.password.set_cdisable(user_mode = enums.UserRole.ADMin) \n
 		No command help available \n
-			:param usermode: No help available
+			:param user_mode: No help available
 		"""
-		param = Conversions.enum_scalar_to_str(usermode, enums.UserRole)
+		param = Conversions.enum_scalar_to_str(user_mode, enums.UserRole)
 		self._core.io.write(f'SYSTem:BASE:PASSword:CDISable {param}')
 
 	def clone(self) -> 'Password':
 		"""Clones the group by creating new object from it and its whole existing sub-groups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
 		new_group = Password(self._core, self._base.parent)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Password_/Cenable.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Help_/Status.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,32 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
-from .....Internal import Conversions
-from .....Internal.Types import DataType
-from .....Internal.ArgSingleList import ArgSingleList
-from .....Internal.ArgSingle import ArgSingle
-from ..... import enums
+from typing import List
+
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
+from ....Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Cenable:
-	"""Cenable commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class Status:
+	"""Status commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("cenable", core, parent)
+		self._base = CommandsGroup("status", core, parent)
 
-	# noinspection PyTypeChecker
-	def get_state(self) -> enums.UserRole:
-		"""SCPI: SYSTem:BASE:PASSword[:CENable]:STATe \n
-		Snippet: value: enums.UserRole = driver.system.base.password.cenable.get_state() \n
+	def get_bits(self) -> List[str]:
+		"""SCPI: SYSTem:HELP:STATus:BITS \n
+		Snippet: value: List[str] = driver.system.help.status.get_bits() \n
 		No command help available \n
-			:return: usermode: No help available
+			:return: bits: No help available
 		"""
-		response = self._core.io.query_str('SYSTem:BASE:PASSword:CENable:STATe?')
-		return Conversions.str_to_scalar_enum(response, enums.UserRole)
+		response = self._core.io.query_str('SYSTem:HELP:STATus:BITS?')
+		return Conversions.str_to_str_list(response)
 
-	def set(self, usermode: enums.UserRole, password: str) -> None:
-		"""SCPI: SYSTem:BASE:PASSword[:CENable] \n
-		Snippet: driver.system.base.password.cenable.set(usermode = enums.UserRole.ADMin, password = '1') \n
+	def get_register(self) -> List[str]:
+		"""SCPI: SYSTem:HELP:STATus[:REGister] \n
+		Snippet: value: List[str] = driver.system.help.status.get_register() \n
 		No command help available \n
-			:param usermode: No help available
-			:param password: No help available
+			:return: register: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('usermode', usermode, DataType.Enum), ArgSingle('password', password, DataType.String))
-		self._core.io.write(f'SYSTem:BASE:PASSword:CENable {param}'.rstrip())
+		response = self._core.io.query_str('SYSTem:HELP:STATus:REGister?')
+		return Conversions.str_to_str_list(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Reference.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Reference.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Reference_/Dc.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Reference_/Dc.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Reference_/Dc_/Offset.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Reference_/Dc_/Offset.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Reference_/Frequency.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Reference_/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Reference_/Frequency_/Advanced.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Reference_/Frequency_/Advanced.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Reference_/Frequency_/Advanced_/Source.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Reference_/Frequency_/Advanced_/Source.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Reference_/Phase.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Reference_/Phase.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/Ssync.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/Ssync.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Base_/StIcon.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Base_/StIcon.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Cmw.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Cmw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Cmw_/Device.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Cmw_/Device.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Cmw_/Device_/Id.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Update.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,33 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
-from .....Internal.Utilities import trim_str_response
-from ..... import repcap
+from ...Internal.Core import Core
+from ...Internal.CommandsGroup import CommandsGroup
+from ...Internal import Conversions
+from ...Internal.Utilities import trim_str_response
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Id:
-	"""Id commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class Update:
+	"""Update commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("id", core, parent)
+		self._base = CommandsGroup("update", core, parent)
 
-	def get(self, cmwVariant=repcap.CmwVariant.Default) -> str:
-		"""SCPI: SYSTem:CMW<n>:DEVice:ID \n
-		Snippet: value: str = driver.system.cmw.device.id.get(cmwVariant = repcap.CmwVariant.Default) \n
-		No command help available \n
-			:param cmwVariant: optional repeated capability selector. Default value: Cmw1 (settable in the interface 'Cmw')
-			:return: idn: No help available"""
-		cmwVariant_cmd_val = self._base.get_repcap_cmd_value(cmwVariant, repcap.CmwVariant)
-		response = self._core.io.query_str(f'SYSTem:CMW{cmwVariant_cmd_val}:DEVice:ID?')
+	def get_dgroup(self) -> str:
+		"""SCPI: SYSTem:UPDate:DGRoup \n
+		Snippet: value: str = driver.system.update.get_dgroup() \n
+		Sets the Device Group that the instrument belongs to. For remote installation, this setting must match the corresponding
+		setting in the R&S Software Distributor options. \n
+			:return: devicegroup: No help available
+		"""
+		response = self._core.io.query_str('SYSTem:UPDate:DGRoup?')
 		return trim_str_response(response)
+
+	def set_dgroup(self, devicegroup: str) -> None:
+		"""SCPI: SYSTem:UPDate:DGRoup \n
+		Snippet: driver.system.update.set_dgroup(devicegroup = '1') \n
+		Sets the Device Group that the instrument belongs to. For remote installation, this setting must match the corresponding
+		setting in the R&S Software Distributor options. \n
+			:param devicegroup: No help available
+		"""
+		param = Conversions.value_to_quoted_str(devicegroup)
+		self._core.io.write(f'SYSTem:UPDate:DGRoup {param}')
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Cmw_/Device_/Vi.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Cmw_/Device_/Vi.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Gpib.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Gpib.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/Self.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/Self.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/Self_/Addr.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/Self_/Addr.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/Self_/Enable.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/Self_/Enable.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/Vresource.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Gpib_/Vresource.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,11 +13,11 @@
 		self._base = CommandsGroup("vresource", core, parent)
 
 	def get(self, gpibInstance=repcap.GpibInstance.Default) -> str:
 		"""SCPI: SYSTem:COMMunicate:GPIB<inst>:VRESource \n
 		Snippet: value: str = driver.system.communicate.gpib.vresource.get(gpibInstance = repcap.GpibInstance.Default) \n
 		No command help available \n
 			:param gpibInstance: optional repeated capability selector. Default value: Inst1 (settable in the interface 'Gpib')
-			:return: visaresource: No help available"""
+			:return: visa_resource: No help available"""
 		gpibInstance_cmd_val = self._base.get_repcap_cmd_value(gpibInstance, repcap.GpibInstance)
 		response = self._core.io.query_str(f'SYSTem:COMMunicate:GPIB{gpibInstance_cmd_val}:VRESource?')
 		return trim_str_response(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Hislip.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Hislip.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Hislip_/Vresource.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Hislip_/Vresource.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,11 +13,11 @@
 		self._base = CommandsGroup("vresource", core, parent)
 
 	def get(self, hislipInstance=repcap.HislipInstance.Default) -> str:
 		"""SCPI: SYSTem:COMMunicate:HISLip<inst>:VRESource \n
 		Snippet: value: str = driver.system.communicate.hislip.vresource.get(hislipInstance = repcap.HislipInstance.Default) \n
 		Queries the VISA resource string for the HiSLIP protocol. \n
 			:param hislipInstance: optional repeated capability selector. Default value: Inst1 (settable in the interface 'Hislip')
-			:return: visaresource: No help available"""
+			:return: visa_resource: No help available"""
 		hislipInstance_cmd_val = self._base.get_repcap_cmd_value(hislipInstance, repcap.HislipInstance)
 		response = self._core.io.query_str(f'SYSTem:COMMunicate:HISLip{hislipInstance_cmd_val}:VRESource?')
 		return trim_str_response(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Net.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Net.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,26 +30,26 @@
 			self._subnet = Subnet(self._core, self._base)
 		return self._subnet
 
 	def get_adapter(self) -> str:
 		"""SCPI: SYSTem:COMMunicate:NET:ADAPter \n
 		Snippet: value: str = driver.system.communicate.net.get_adapter() \n
 		Selects a LAN network adapter for configuration via other SYSTem:COMMunicate:NET... commands. \n
-			:return: networkadapter: No help available
+			:return: network_adapter: No help available
 		"""
 		response = self._core.io.query_str('SYSTem:COMMunicate:NET:ADAPter?')
 		return trim_str_response(response)
 
-	def set_adapter(self, networkadapter: str) -> None:
+	def set_adapter(self, network_adapter: str) -> None:
 		"""SCPI: SYSTem:COMMunicate:NET:ADAPter \n
-		Snippet: driver.system.communicate.net.set_adapter(networkadapter = '1') \n
+		Snippet: driver.system.communicate.net.set_adapter(network_adapter = '1') \n
 		Selects a LAN network adapter for configuration via other SYSTem:COMMunicate:NET... commands. \n
-			:param networkadapter: No help available
+			:param network_adapter: No help available
 		"""
-		param = Conversions.value_to_quoted_str(networkadapter)
+		param = Conversions.value_to_quoted_str(network_adapter)
 		self._core.io.write(f'SYSTem:COMMunicate:NET:ADAPter {param}')
 
 	def get_gateway(self) -> List[str]:
 		"""SCPI: SYSTem:COMMunicate:NET:GATeway \n
 		Snippet: value: List[str] = driver.system.communicate.net.get_gateway() \n
 		Manually defines IPv4 addresses of default gateways. A query returns the currently defined addresses, irrespective of
 		whether they have been specified manually or via DHCP. \n
@@ -69,27 +69,27 @@
 		self._core.io.write(f'SYSTem:COMMunicate:NET:GATeway {param}')
 
 	def get_ip_address(self) -> List[str]:
 		"""SCPI: SYSTem:COMMunicate:NET:IPADdress \n
 		Snippet: value: List[str] = driver.system.communicate.net.get_ip_address() \n
 		Manually assigns one or more IPv4 addresses to the network adapter. A query returns the currently assigned addresses,
 		irrespective of whether they have been assigned manually or via DHCP. \n
-			:return: ipaddresses: No help available
+			:return: ip_addresses: No help available
 		"""
 		response = self._core.io.query_str('SYSTem:COMMunicate:NET:IPADdress?')
 		return Conversions.str_to_str_list(response)
 
-	def set_ip_address(self, ipaddresses: List[str]) -> None:
+	def set_ip_address(self, ip_addresses: List[str]) -> None:
 		"""SCPI: SYSTem:COMMunicate:NET:IPADdress \n
-		Snippet: driver.system.communicate.net.set_ip_address(ipaddresses = ['1', '2', '3']) \n
+		Snippet: driver.system.communicate.net.set_ip_address(ip_addresses = ['1', '2', '3']) \n
 		Manually assigns one or more IPv4 addresses to the network adapter. A query returns the currently assigned addresses,
 		irrespective of whether they have been assigned manually or via DHCP. \n
-			:param ipaddresses: IPv4 address consisting of four blocks (octets) separated by dots Several strings separated by commas can be entered or several addresses separated by commas can be included in one string.
+			:param ip_addresses: IPv4 address consisting of four blocks (octets) separated by dots Several strings separated by commas can be entered or several addresses separated by commas can be included in one string.
 		"""
-		param = Conversions.list_to_csv_quoted_str(ipaddresses)
+		param = Conversions.list_to_csv_quoted_str(ip_addresses)
 		self._core.io.write(f'SYSTem:COMMunicate:NET:IPADdress {param}')
 
 	def get_hostname(self) -> str:
 		"""SCPI: SYSTem:COMMunicate:NET:HOSTname \n
 		Snippet: value: str = driver.system.communicate.net.get_hostname() \n
 		Queries the host name (computer name) of the R&S CMX500. The host name is part of the VISA address string for LAN-based
 		connections. \n
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Net_/Dns.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Net_/Dns.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,21 +32,21 @@
 		self._core.io.write(f'SYSTem:COMMunicate:NET:DNS:ENABle {param}')
 
 	def get_value(self) -> List[str]:
 		"""SCPI: SYSTem:COMMunicate:NET:DNS \n
 		Snippet: value: List[str] = driver.system.communicate.net.dns.get_value() \n
 		Manually defines the DNS server IPv4 addresses to be used. A query returns the defined DNS addresses, irrespective of
 		whether they have been specified manually or via DHCP. \n
-			:return: ipaddresses: No help available
+			:return: ip_addresses: No help available
 		"""
 		response = self._core.io.query_str('SYSTem:COMMunicate:NET:DNS?')
 		return Conversions.str_to_str_list(response)
 
-	def set_value(self, ipaddresses: List[str]) -> None:
+	def set_value(self, ip_addresses: List[str]) -> None:
 		"""SCPI: SYSTem:COMMunicate:NET:DNS \n
-		Snippet: driver.system.communicate.net.dns.set_value(ipaddresses = ['1', '2', '3']) \n
+		Snippet: driver.system.communicate.net.dns.set_value(ip_addresses = ['1', '2', '3']) \n
 		Manually defines the DNS server IPv4 addresses to be used. A query returns the defined DNS addresses, irrespective of
 		whether they have been specified manually or via DHCP. \n
-			:param ipaddresses: DNS server IPv4 addresses consisting of four blocks separated by dots. Several strings separated by commas can be entered or several addresses separated by commas can be included in one string.
+			:param ip_addresses: DNS server IPv4 addresses consisting of four blocks separated by dots. Several strings separated by commas can be entered or several addresses separated by commas can be included in one string.
 		"""
-		param = Conversions.list_to_csv_quoted_str(ipaddresses)
+		param = Conversions.list_to_csv_quoted_str(ip_addresses)
 		self._core.io.write(f'SYSTem:COMMunicate:NET:DNS {param}')
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Net_/Subnet.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Net_/Subnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 		self._base = CommandsGroup("subnet", core, parent)
 
 	def get_mask(self) -> List[str]:
 		"""SCPI: SYSTem:COMMunicate:NET:SUBNet:MASK \n
 		Snippet: value: List[str] = driver.system.communicate.net.subnet.get_mask() \n
 		Manually defines the subnet masks to be used for the network adapter IPv4 addresses. A query returns the currently used
 		subnet masks, irrespective of whether they have been assigned manually or via DHCP. \n
-			:return: subnetmasks: No help available
+			:return: subnet_masks: No help available
 		"""
 		response = self._core.io.query_str('SYSTem:COMMunicate:NET:SUBNet:MASK?')
 		return Conversions.str_to_str_list(response)
 
-	def set_mask(self, subnetmasks: List[str]) -> None:
+	def set_mask(self, subnet_masks: List[str]) -> None:
 		"""SCPI: SYSTem:COMMunicate:NET:SUBNet:MASK \n
-		Snippet: driver.system.communicate.net.subnet.set_mask(subnetmasks = ['1', '2', '3']) \n
+		Snippet: driver.system.communicate.net.subnet.set_mask(subnet_masks = ['1', '2', '3']) \n
 		Manually defines the subnet masks to be used for the network adapter IPv4 addresses. A query returns the currently used
 		subnet masks, irrespective of whether they have been assigned manually or via DHCP. \n
-			:param subnetmasks: IPv4 subnet mask consisting of four blocks separated by dots Several strings separated by commas can be entered or several masks separated by commas can be included in one string.
+			:param subnet_masks: IPv4 subnet mask consisting of four blocks separated by dots Several strings separated by commas can be entered or several masks separated by commas can be included in one string.
 		"""
-		param = Conversions.list_to_csv_quoted_str(subnetmasks)
+		param = Conversions.list_to_csv_quoted_str(subnet_masks)
 		self._core.io.write(f'SYSTem:COMMunicate:NET:SUBNet:MASK {param}')
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Rsib.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Rsib.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Rsib_/Vresource.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Rsib_/Vresource.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,11 +13,11 @@
 		self._base = CommandsGroup("vresource", core, parent)
 
 	def get(self, rsibInstance=repcap.RsibInstance.Default) -> str:
 		"""SCPI: SYSTem:COMMunicate:RSIB<inst>:VRESource \n
 		Snippet: value: str = driver.system.communicate.rsib.vresource.get(rsibInstance = repcap.RsibInstance.Default) \n
 		No command help available \n
 			:param rsibInstance: optional repeated capability selector. Default value: Inst1 (settable in the interface 'Rsib')
-			:return: visaresource: No help available"""
+			:return: visa_resource: No help available"""
 		rsibInstance_cmd_val = self._base.get_repcap_cmd_value(rsibInstance, repcap.RsibInstance)
 		response = self._core.io.query_str(f'SYSTem:COMMunicate:RSIB{rsibInstance_cmd_val}:VRESource?')
 		return trim_str_response(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Socket.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Socket.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Socket_/Mode.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Socket_/Mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 class Mode:
 	"""Mode commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("mode", core, parent)
 
-	def set(self, protocolmode: enums.SocketProtocol, socketInstance=repcap.SocketInstance.Default) -> None:
+	def set(self, protocol_mode: enums.SocketProtocol, socketInstance=repcap.SocketInstance.Default) -> None:
 		"""SCPI: SYSTem:COMMunicate:SOCKet<inst>:MODE \n
-		Snippet: driver.system.communicate.socket.mode.set(protocolmode = enums.SocketProtocol.AGILent, socketInstance = repcap.SocketInstance.Default) \n
+		Snippet: driver.system.communicate.socket.mode.set(protocol_mode = enums.SocketProtocol.AGILent, socketInstance = repcap.SocketInstance.Default) \n
 		Sets the protocol operation mode for direct socket communication. \n
-			:param protocolmode: RAW: no support of control messages AGILent: emulation codes via control connection (control port) IEEE1174: emulation codes via data connection (data port)
+			:param protocol_mode: RAW: no support of control messages AGILent: emulation codes via control connection (control port) IEEE1174: emulation codes via data connection (data port)
 			:param socketInstance: optional repeated capability selector. Default value: Inst1 (settable in the interface 'Socket')"""
-		param = Conversions.enum_scalar_to_str(protocolmode, enums.SocketProtocol)
+		param = Conversions.enum_scalar_to_str(protocol_mode, enums.SocketProtocol)
 		socketInstance_cmd_val = self._base.get_repcap_cmd_value(socketInstance, repcap.SocketInstance)
 		self._core.io.write(f'SYSTem:COMMunicate:SOCKet{socketInstance_cmd_val}:MODE {param}')
 
 	# noinspection PyTypeChecker
 	def get(self, socketInstance=repcap.SocketInstance.Default) -> enums.SocketProtocol:
 		"""SCPI: SYSTem:COMMunicate:SOCKet<inst>:MODE \n
 		Snippet: value: enums.SocketProtocol = driver.system.communicate.socket.mode.get(socketInstance = repcap.SocketInstance.Default) \n
 		Sets the protocol operation mode for direct socket communication. \n
 			:param socketInstance: optional repeated capability selector. Default value: Inst1 (settable in the interface 'Socket')
-			:return: protocolmode: No help available"""
+			:return: protocol_mode: No help available"""
 		socketInstance_cmd_val = self._base.get_repcap_cmd_value(socketInstance, repcap.SocketInstance)
 		response = self._core.io.query_str(f'SYSTem:COMMunicate:SOCKet{socketInstance_cmd_val}:MODE?')
 		return Conversions.str_to_scalar_enum(response, enums.SocketProtocol)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Socket_/Port.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Socket_/Port.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 class Port:
 	"""Port commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("port", core, parent)
 
-	def set(self, portnumber: int, socketInstance=repcap.SocketInstance.Default) -> None:
+	def set(self, port_number: int, socketInstance=repcap.SocketInstance.Default) -> None:
 		"""SCPI: SYSTem:COMMunicate:SOCKet<inst>:PORT \n
-		Snippet: driver.system.communicate.socket.port.set(portnumber = 1, socketInstance = repcap.SocketInstance.Default) \n
+		Snippet: driver.system.communicate.socket.port.set(port_number = 1, socketInstance = repcap.SocketInstance.Default) \n
 		Sets the data port number for direct socket communication. \n
-			:param portnumber: No help available
+			:param port_number: No help available
 			:param socketInstance: optional repeated capability selector. Default value: Inst1 (settable in the interface 'Socket')"""
-		param = Conversions.decimal_value_to_str(portnumber)
+		param = Conversions.decimal_value_to_str(port_number)
 		socketInstance_cmd_val = self._base.get_repcap_cmd_value(socketInstance, repcap.SocketInstance)
 		self._core.io.write(f'SYSTem:COMMunicate:SOCKet{socketInstance_cmd_val}:PORT {param}')
 
 	def get(self, socketInstance=repcap.SocketInstance.Default) -> int:
 		"""SCPI: SYSTem:COMMunicate:SOCKet<inst>:PORT \n
 		Snippet: value: int = driver.system.communicate.socket.port.get(socketInstance = repcap.SocketInstance.Default) \n
 		Sets the data port number for direct socket communication. \n
 			:param socketInstance: optional repeated capability selector. Default value: Inst1 (settable in the interface 'Socket')
-			:return: portnumber: No help available"""
+			:return: port_number: No help available"""
 		socketInstance_cmd_val = self._base.get_repcap_cmd_value(socketInstance, repcap.SocketInstance)
 		response = self._core.io.query_str(f'SYSTem:COMMunicate:SOCKet{socketInstance_cmd_val}:PORT?')
 		return Conversions.str_to_int(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Socket_/Vresource.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Socket_/Vresource.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,11 +13,11 @@
 		self._base = CommandsGroup("vresource", core, parent)
 
 	def get(self, socketInstance=repcap.SocketInstance.Default) -> str:
 		"""SCPI: SYSTem:COMMunicate:SOCKet<inst>:VRESource \n
 		Snippet: value: str = driver.system.communicate.socket.vresource.get(socketInstance = repcap.SocketInstance.Default) \n
 		Queries the VISA resource string for direct socket communication. \n
 			:param socketInstance: optional repeated capability selector. Default value: Inst1 (settable in the interface 'Socket')
-			:return: visaresource: No help available"""
+			:return: visa_resource: No help available"""
 		socketInstance_cmd_val = self._base.get_repcap_cmd_value(socketInstance, repcap.SocketInstance)
 		response = self._core.io.query_str(f'SYSTem:COMMunicate:SOCKet{socketInstance_cmd_val}:VRESource?')
 		return trim_str_response(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Usb.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Usb.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 		self._core = core
 		self._base = CommandsGroup("usb", core, parent)
 
 	def get_vresource(self) -> str:
 		"""SCPI: SYSTem:COMMunicate:USB:VRESource \n
 		Snippet: value: str = driver.system.communicate.usb.get_vresource() \n
 		Queries the VISA resource string of the USB interface. \n
-			:return: visaresource: No help available
+			:return: visa_resource: No help available
 		"""
 		response = self._core.io.query_str('SYSTem:COMMunicate:USB:VRESource?')
 		return trim_str_response(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Vxi.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Vxi.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Vxi_/Gtr.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Vxi_/Gtr.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Communicate_/Vxi_/Vresource.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Communicate_/Vxi_/Vresource.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,11 +13,11 @@
 		self._base = CommandsGroup("vresource", core, parent)
 
 	def get(self, vxiInstance=repcap.VxiInstance.Default) -> str:
 		"""SCPI: SYSTem:COMMunicate:VXI<inst>:VRESource \n
 		Snippet: value: str = driver.system.communicate.vxi.vresource.get(vxiInstance = repcap.VxiInstance.Default) \n
 		Queries the VISA resource string for the VXI-11 protocol. \n
 			:param vxiInstance: optional repeated capability selector. Default value: Inst1 (settable in the interface 'Vxi')
-			:return: visaresource: No help available"""
+			:return: visa_resource: No help available"""
 		vxiInstance_cmd_val = self._base.get_repcap_cmd_value(vxiInstance, repcap.VxiInstance)
 		response = self._core.io.query_str(f'SYSTem:COMMunicate:VXI{vxiInstance_cmd_val}:VRESource?')
 		return trim_str_response(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Connector.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Connector.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Connector_/Translation.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Connector_/Translation.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Date.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Date.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Device.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Device.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/DeviceFootprint.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/DeviceFootprint.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Display.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Display.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,26 +19,26 @@
 			self._monitor = Monitor(self._core, self._base)
 		return self._monitor
 
 	def get_update(self) -> bool:
 		"""SCPI: SYSTem:DISPlay:UPDate \n
 		Snippet: value: bool = driver.system.display.get_update() \n
 		No command help available \n
-			:return: displayupdate: No help available
+			:return: display_update: No help available
 		"""
 		response = self._core.io.query_str('SYSTem:DISPlay:UPDate?')
 		return Conversions.str_to_bool(response)
 
-	def set_update(self, displayupdate: bool) -> None:
+	def set_update(self, display_update: bool) -> None:
 		"""SCPI: SYSTem:DISPlay:UPDate \n
-		Snippet: driver.system.display.set_update(displayupdate = False) \n
+		Snippet: driver.system.display.set_update(display_update = False) \n
 		No command help available \n
-			:param displayupdate: No help available
+			:param display_update: No help available
 		"""
-		param = Conversions.bool_to_str(displayupdate)
+		param = Conversions.bool_to_str(display_update)
 		self._core.io.write(f'SYSTem:DISPlay:UPDate {param}')
 
 	def clone(self) -> 'Display':
 		"""Clones the group by creating new object from it and its whole existing sub-groups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
 		new_group = Display(self._core, self._base.parent)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Display_/Monitor.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Display_/Monitor.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Display_/Monitor_/Off.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Display_/Monitor_/Off.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Error.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Error.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Error_/Code.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Error_/Code.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Generator.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Generator.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Generator_/All.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Generator_/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Generator_/All_/Off.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Generator_/All_/Off.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Help.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Help.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Help_/Headers.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Routing_/Possible.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,27 @@
+from typing import List
+
 from ....Internal.Core import Core
 from ....Internal.CommandsGroup import CommandsGroup
+from ....Internal import Conversions
 from ....Internal.Types import DataType
 from ....Internal.ArgSingleList import ArgSingleList
 from ....Internal.ArgSingle import ArgSingle
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Headers:
-	"""Headers commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class Possible:
+	"""Possible commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("headers", core, parent)
+		self._base = CommandsGroup("possible", core, parent)
 
-	def get(self, parser: str = None) -> bytes:
-		"""SCPI: SYSTem:HELP:HEADers \n
-		Snippet: value: bytes = driver.system.help.headers.get(parser = '1') \n
+	def get(self, item: str = None) -> List[str]:
+		"""SCPI: SYSTem:ROUTing:POSSible \n
+		Snippet: value: List[str] = driver.system.routing.possible.get(item = '1') \n
 		No command help available \n
-			:param parser: No help available
-			:return: headers: No help available"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('parser', parser, DataType.String, True))
-		response = self._core.io.query_bin_block_ERROR(f'SYSTem:HELP:HEADers? {param}'.rstrip())
-		return response
+			:param item: No help available
+			:return: routing: No help available"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('item', item, DataType.String, True))
+		response = self._core.io.query_str(f'SYSTem:ROUTing:POSSible? {param}'.rstrip())
+		return Conversions.str_to_str_list(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Help_/Status.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Measurement_/All_/Off.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,26 @@
-from typing import List
-
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal import Conversions
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Status:
-	"""Status commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class Off:
+	"""Off commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("status", core, parent)
+		self._base = CommandsGroup("off", core, parent)
 
-	def get_bits(self) -> List[str]:
-		"""SCPI: SYSTem:HELP:STATus:BITS \n
-		Snippet: value: List[str] = driver.system.help.status.get_bits() \n
-		No command help available \n
-			:return: bits: No help available
+	def set(self) -> None:
+		"""SCPI: SYSTem:MEASurement:ALL:OFF \n
+		Snippet: driver.system.measurement.all.off.set() \n
+		Switch off all signaling applications, generators or measurements. \n
 		"""
-		response = self._core.io.query_str('SYSTem:HELP:STATus:BITS?')
-		return Conversions.str_to_str_list(response)
+		self._core.io.write(f'SYSTem:MEASurement:ALL:OFF')
 
-	def get_register(self) -> List[str]:
-		"""SCPI: SYSTem:HELP:STATus[:REGister] \n
-		Snippet: value: List[str] = driver.system.help.status.get_register() \n
-		No command help available \n
-			:return: register: No help available
+	def set_with_opc(self) -> None:
+		"""SCPI: SYSTem:MEASurement:ALL:OFF \n
+		Snippet: driver.system.measurement.all.off.set_with_opc() \n
+		Switch off all signaling applications, generators or measurements. \n
+		Same as set, but waits for the operation to complete before continuing further. Use the RsCMPX_Base.utilities.opc_timeout_set() to set the timeout value. \n
 		"""
-		response = self._core.io.query_str('SYSTem:HELP:STATus:REGister?')
-		return Conversions.str_to_str_list(response)
+		self._core.io.write_with_opc(f'SYSTem:MEASurement:ALL:OFF')
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Help_/Syntax.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Help_/Syntax.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Measurement.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Measurement_/All.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Measurement_/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Measurement_/All_/Off.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Signaling_/All_/Off.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 	"""Off commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("off", core, parent)
 
 	def set(self) -> None:
-		"""SCPI: SYSTem:MEASurement:ALL:OFF \n
-		Snippet: driver.system.measurement.all.off.set() \n
+		"""SCPI: SYSTem:SIGNaling:ALL:OFF \n
+		Snippet: driver.system.signaling.all.off.set() \n
 		Switch off all signaling applications, generators or measurements. \n
 		"""
-		self._core.io.write(f'SYSTem:MEASurement:ALL:OFF')
+		self._core.io.write(f'SYSTem:SIGNaling:ALL:OFF')
 
 	def set_with_opc(self) -> None:
-		"""SCPI: SYSTem:MEASurement:ALL:OFF \n
-		Snippet: driver.system.measurement.all.off.set_with_opc() \n
+		"""SCPI: SYSTem:SIGNaling:ALL:OFF \n
+		Snippet: driver.system.signaling.all.off.set_with_opc() \n
 		Switch off all signaling applications, generators or measurements. \n
 		Same as set, but waits for the operation to complete before continuing further. Use the RsCMPX_Base.utilities.opc_timeout_set() to set the timeout value. \n
 		"""
-		self._core.io.write_with_opc(f'SYSTem:MEASurement:ALL:OFF')
+		self._core.io.write_with_opc(f'SYSTem:SIGNaling:ALL:OFF')
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Password.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Password.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Password_/New.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Password_/New.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Record.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Record.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Record_/Macro.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Record_/Macro.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Record_/Macro_/File.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Record_/Macro_/File.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Routing.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Routing.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Routing_/Possible.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/ExtB_/Catalog.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 from typing import List
 
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal import Conversions
-from ....Internal.Types import DataType
-from ....Internal.ArgSingleList import ArgSingleList
-from ....Internal.ArgSingle import ArgSingle
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Possible:
-	"""Possible commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class Catalog:
+	"""Catalog commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("possible", core, parent)
+		self._base = CommandsGroup("catalog", core, parent)
 
-	def get(self, item: str = None) -> List[str]:
-		"""SCPI: SYSTem:ROUTing:POSSible \n
-		Snippet: value: List[str] = driver.system.routing.possible.get(item = '1') \n
-		No command help available \n
-			:param item: No help available
-			:return: routing: No help available"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('item', item, DataType.String, True))
-		response = self._core.io.query_str(f'SYSTem:ROUTing:POSSible? {param}'.rstrip())
+	def get_source(self) -> List[str]:
+		"""SCPI: TRIGger:BASE:EXTB:CATalog:SOURce \n
+		Snippet: value: List[str] = driver.trigger.base.extB.catalog.get_source() \n
+		Lists all trigger source values that can be set using TRIGger:BASE:EXTA|EXTB:SOURce. \n
+			:return: source_list: Comma-separated list of strings, one string per supported value
+		"""
+		response = self._core.io.query_str('TRIGger:BASE:EXTB:CATalog:SOURce?')
 		return Conversions.str_to_str_list(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Signaling.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Signaling.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Signaling_/All.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Signaling_/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/SingleCmw.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/SingleCmw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/SingleCmw_/Device.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/SingleCmw_/Device.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Startup.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,35 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Startup:
-	"""Startup commands group definition. 1 total commands, 1 Sub-groups, 0 group commands"""
+class Mode:
+	"""Mode commands group definition. 13 total commands, 2 Sub-groups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("startup", core, parent)
+		self._base = CommandsGroup("mode", core, parent)
 
 	@property
-	def prepare(self):
-		"""prepare commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_prepare'):
-			from .Startup_.Prepare import Prepare
-			self._prepare = Prepare(self._core, self._base)
-		return self._prepare
+	def display(self):
+		"""display commands group. 0 Sub-classes, 2 commands."""
+		if not hasattr(self, '_display'):
+			from .Mode_.Display import Display
+			self._display = Display(self._core, self._base)
+		return self._display
 
-	def clone(self) -> 'Startup':
+	@property
+	def file(self):
+		"""file commands group. 11 Sub-classes, 0 commands."""
+		if not hasattr(self, '_file'):
+			from .Mode_.File import File
+			self._file = File(self._core, self._base)
+		return self._file
+
+	def clone(self) -> 'Mode':
 		"""Clones the group by creating new object from it and its whole existing sub-groups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Startup(self._core, self._base.parent)
+		new_group = Mode(self._core, self._base.parent)
 		self._base.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Startup_/Prepare.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Startup_/Prepare.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Time.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Time.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Time_/DaylightSavingTime.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Time_/DaylightSavingTime.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Time_/DaylightSavingTime_/Rule.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Time_/DaylightSavingTime_/Rule.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Time_/HrTimer.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Time_/HrTimer.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Time_/HrTimer_/Absolute.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Time_/HrTimer_/Absolute.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/System_/Time_/HrTimer_/Absolute_/Set.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/System_/Time_/HrTimer_/Absolute_/Set.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Write_/Eeprom.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,27 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
+from ...Internal.Core import Core
+from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Mode:
-	"""Mode commands group definition. 13 total commands, 2 Sub-groups, 0 group commands"""
+class Eeprom:
+	"""Eeprom commands group definition. 1 total commands, 1 Sub-groups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("mode", core, parent)
+		self._base = CommandsGroup("eeprom", core, parent)
 
 	@property
-	def display(self):
-		"""display commands group. 0 Sub-classes, 2 commands."""
-		if not hasattr(self, '_display'):
-			from .Mode_.Display import Display
-			self._display = Display(self._core, self._base)
-		return self._display
+	def data(self):
+		"""data commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_data'):
+			from .Eeprom_.Data import Data
+			self._data = Data(self._core, self._base)
+		return self._data
 
-	@property
-	def file(self):
-		"""file commands group. 11 Sub-classes, 0 commands."""
-		if not hasattr(self, '_file'):
-			from .Mode_.File import File
-			self._file = File(self._core, self._base)
-		return self._file
-
-	def clone(self) -> 'Mode':
+	def clone(self) -> 'Eeprom':
 		"""Clones the group by creating new object from it and its whole existing sub-groups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Mode(self._core, self._base.parent)
+		new_group = Eeprom(self._core, self._base.parent)
 		self._base.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/Display.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/Display.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Dexecution.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Dexecution.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Dexecution_/Duration.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Dexecution_/Duration.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Enable.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Enable.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/FilterPy.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/FilterPy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/FormatPy.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/FormatPy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Functions.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Functions.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Name.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Name.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Parser.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Parser.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Rpc.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Rpc.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Size.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Size.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/StartMode.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/StartMode.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/StopMode.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/StopMode.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/TriggerInvoke.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/TriggerInvoke.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 		"""extB commands group. 1 Sub-classes, 3 commands."""
 		if not hasattr(self, '_extB'):
 			from .Base_.ExtB import ExtB
 			self._extB = ExtB(self._core, self._base)
 		return self._extB
 
 	@property
-	def userInitiated(self):
-		"""userInitiated commands group. 1 Sub-classes, 0 commands."""
-		if not hasattr(self, '_userInitiated'):
-			from .Base_.UserInitiated import UserInitiated
-			self._userInitiated = UserInitiated(self._core, self._base)
-		return self._userInitiated
+	def uinitiated(self):
+		"""uinitiated commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_uinitiated'):
+			from .Base_.Uinitiated import Uinitiated
+			self._uinitiated = Uinitiated(self._core, self._base)
+		return self._uinitiated
 
 	@property
 	def eout(self):
 		"""eout commands group. 2 Sub-classes, 0 commands."""
 		if not hasattr(self, '_eout'):
 			from .Base_.Eout import Eout
 			self._eout = Eout(self._core, self._base)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/Eout.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/Eout.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/Catalog.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/Catalog_/Source.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/Catalog_/Source.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,11 +15,11 @@
 		self._base = CommandsGroup("source", core, parent)
 
 	def get(self, eout=repcap.Eout.Default) -> List[str]:
 		"""SCPI: TRIGger:BASE:EOUT<n>:CATalog:SOURce \n
 		Snippet: value: List[str] = driver.trigger.base.eout.catalog.source.get(eout = repcap.Eout.Default) \n
 		No command help available \n
 			:param eout: optional repeated capability selector. Default value: Eout1 (settable in the interface 'Eout')
-			:return: sourcelist: No help available"""
+			:return: source_list: No help available"""
 		eout_cmd_val = self._base.get_repcap_cmd_value(eout, repcap.Eout)
 		response = self._core.io.query_str(f'TRIGger:BASE:EOUT{eout_cmd_val}:CATalog:SOURce?')
 		return Conversions.str_to_str_list(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/Source.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/Source.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/ExtA.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/ExtA.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/ExtA_/Catalog.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/ExtA_/Catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,11 +13,11 @@
 		self._core = core
 		self._base = CommandsGroup("catalog", core, parent)
 
 	def get_source(self) -> List[str]:
 		"""SCPI: TRIGger:BASE:EXTA:CATalog:SOURce \n
 		Snippet: value: List[str] = driver.trigger.base.extA.catalog.get_source() \n
 		Lists all trigger source values that can be set using TRIGger:BASE:EXTA|EXTB:SOURce. \n
-			:return: sourcelist: Comma-separated list of strings, one string per supported value
+			:return: source_list: Comma-separated list of strings, one string per supported value
 		"""
 		response = self._core.io.query_str('TRIGger:BASE:EXTA:CATalog:SOURce?')
 		return Conversions.str_to_str_list(response)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/ExtB.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/ExtB.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/UserInitiated.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/Uinitiated.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from ....Internal.Core import Core
 from ....Internal.CommandsGroup import CommandsGroup
 from ....Internal.RepeatedCapability import RepeatedCapability
 from .... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class UserInitiated:
-	"""UserInitiated commands group definition. 1 total commands, 1 Sub-groups, 0 group commands
+class Uinitiated:
+	"""Uinitiated commands group definition. 1 total commands, 1 Sub-groups, 0 group commands
 	Repeated Capability: Trigger, default value after init: Trigger.Trg1"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("userInitiated", core, parent)
+		self._base = CommandsGroup("uinitiated", core, parent)
 		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_trigger_get', 'repcap_trigger_set', repcap.Trigger.Trg1)
 
 	def repcap_trigger_set(self, enum_value: repcap.Trigger) -> None:
 		"""Repeated Capability default value numeric suffix.
 		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to Trigger.Default
 		Default value after init: Trigger.Trg1"""
 		self._base.set_repcap_enum_value(enum_value)
@@ -25,18 +25,18 @@
 		# noinspection PyTypeChecker
 		return self._base.get_repcap_enum_value()
 
 	@property
 	def execute(self):
 		"""execute commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_execute'):
-			from .UserInitiated_.Execute import Execute
+			from .Uinitiated_.Execute import Execute
 			self._execute = Execute(self._core, self._base)
 		return self._execute
 
-	def clone(self) -> 'UserInitiated':
+	def clone(self) -> 'Uinitiated':
 		"""Clones the group by creating new object from it and its whole existing sub-groups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = UserInitiated(self._core, self._base.parent)
+		new_group = Uinitiated(self._core, self._base.parent)
 		self._base.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Trigger_/Base_/UserInitiated_/Execute.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Trigger_/Base_/Uinitiated_/Execute.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("execute", core, parent)
 
 	def set(self, trigger=repcap.Trigger.Default) -> None:
 		"""SCPI: TRIGger:BASE:UINitiated<n>:EXECute \n
-		Snippet: driver.trigger.base.userInitiated.execute.set(trigger = repcap.Trigger.Default) \n
+		Snippet: driver.trigger.base.uinitiated.execute.set(trigger = repcap.Trigger.Default) \n
 		No command help available \n
-			:param trigger: optional repeated capability selector. Default value: Trg1 (settable in the interface 'UserInitiated')"""
+			:param trigger: optional repeated capability selector. Default value: Trg1 (settable in the interface 'Uinitiated')"""
 		trigger_cmd_val = self._base.get_repcap_cmd_value(trigger, repcap.Trigger)
 		self._core.io.write(f'TRIGger:BASE:UINitiated{trigger_cmd_val}:EXECute')
 
 	def set_with_opc(self, trigger=repcap.Trigger.Default) -> None:
 		trigger_cmd_val = self._base.get_repcap_cmd_value(trigger, repcap.Trigger)
 		"""SCPI: TRIGger:BASE:UINitiated<n>:EXECute \n
-		Snippet: driver.trigger.base.userInitiated.execute.set_with_opc(trigger = repcap.Trigger.Default) \n
+		Snippet: driver.trigger.base.uinitiated.execute.set_with_opc(trigger = repcap.Trigger.Default) \n
 		No command help available \n
 		Same as set, but waits for the operation to complete before continuing further. Use the RsCMPX_Base.utilities.opc_timeout_set() to set the timeout value. \n
-			:param trigger: optional repeated capability selector. Default value: Trg1 (settable in the interface 'UserInitiated')"""
+			:param trigger: optional repeated capability selector. Default value: Trg1 (settable in the interface 'Uinitiated')"""
 		self._core.io.write_with_opc(f'TRIGger:BASE:UINitiated{trigger_cmd_val}:EXECute')
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Unit.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Unit.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Write.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Write.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Implementations/Write_/Eeprom.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Implementations/Configure_/Base_/IpSet.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Eeprom:
-	"""Eeprom commands group definition. 1 total commands, 1 Sub-groups, 0 group commands"""
+class IpSet:
+	"""IpSet commands group definition. 1 total commands, 1 Sub-groups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("eeprom", core, parent)
+		self._base = CommandsGroup("ipSet", core, parent)
 
 	@property
-	def data(self):
-		"""data commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_data'):
-			from .Eeprom_.Data import Data
-			self._data = Data(self._core, self._base)
-		return self._data
+	def nwAdapter(self):
+		"""nwAdapter commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_nwAdapter'):
+			from .IpSet_.NwAdapter import NwAdapter
+			self._nwAdapter = NwAdapter(self._core, self._base)
+		return self._nwAdapter
 
-	def clone(self) -> 'Eeprom':
+	def clone(self) -> 'IpSet':
 		"""Clones the group by creating new object from it and its whole existing sub-groups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Eeprom(self._core, self._base.parent)
+		new_group = IpSet(self._core, self._base.parent)
 		self._base.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/ArgSingle.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/ArgSingle.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-from .ConverterFromScpiString import ConverterFromScpiString
-from .ConverterToScpiString import ConverterToScpiString
-from .Types import DataType
-
-
-class ArgSingle(object):
-	"""Single Argument outside a structure - used for composing query arguments.
-	Contains the argument value as well (self.value)."""
-
-	def __init__(self, name: str, value, data_type: DataType, is_optional: bool = False, is_open_list: bool = False, repetition: int = 1, intern_link: str = None):
-		self.name = name if name else ''
-		self.argument_ix = None
-		self.value = value
-		self.data_type = data_type
-		self.is_optional = is_optional
-		self.is_open_list = is_open_list
-		self.repetition = repetition
-		self.intern_link = intern_link
-		self.conv_from_scpi_string = None
-		self.conv_to_scpi_string = None
-
-		if self.data_type == DataType.Enum:
-			self.assert_mandatory_has_value(self)
-			if self.value is not None:
-				self.enum_type = type(self.value)
-				self.conv_from_scpi_string = ConverterFromScpiString(self.data_type, self.enum_type)
-				self.conv_to_scpi_string = ConverterToScpiString(self.data_type, self.enum_type)
-		elif self.data_type == DataType.EnumList:
-			self.assert_mandatory_has_value(self)
-			if self.value is not None:
-				self.enum_type = type(self.value[0])
-				self.conv_from_scpi_string = ConverterFromScpiString(self.data_type, self.enum_type)
-				self.conv_to_scpi_string = ConverterToScpiString(self.data_type, self.enum_type)
-		else:
-			self.conv_from_scpi_string = ConverterFromScpiString(self.data_type)
-			self.conv_to_scpi_string = ConverterToScpiString(self.data_type)
-
-		self.check_consistency()
-
-	@classmethod
-	def as_open_list(cls, name: str, value: object, data_type: DataType) -> 'ArgSingle':
-		"""Creates new ArgSingle of open list type.Use this method for all non-interleaved list types. \n
-		:param name: name of the argument.
-		:param value: value of the argument.
-		:param data_type: data type of the argument.
-		:return: ArgSingle object of an open list type."""
-		return cls(name, value, data_type, False, True, 1, None)
-
-	def __str__(self):
-		opt = '~' if self.is_optional else ''
-		name = f" '{self.name}'" if self.name != '' else ''
-		out = f"SingleArg {opt}{self.data_type.name}{name}"
-
-		if self.is_open_list is False and self.repetition > 1:
-			out += f' [{self.repetition}]'
-		elif self.is_open_list is True:
-			out += f' [{self.repetition}...]'
-		if self.intern_link:
-			out += f", Linking: '{self.intern_link}'"
-		if self.value:
-			out += f', value: {self.value}'
-		else:
-			out += ", <no value>"
-		if self.intern_link:
-			out += f", Linking: '{self.intern_link}'"
-		return out
-
-	# noinspection PyUnusedLocal
-	def has_value(self, value_obj=None) -> bool:
-		"""Returns true, if the argument has value."""
-		return self.value is not None
-
-	# noinspection PyUnusedLocal
-	def assert_is_optional(self, obj=None) -> None:
-		"""Asserts that the parameter is optional.
-		If not, the method throws an exception."""
-		if self.is_optional:
-			return
-		raise Exception(f'Single argument is not optional: {self}')
-
-	# noinspection PyUnusedLocal
-	def assert_mandatory_has_value(self, value_obj=None) -> None:
-		"""Asserts that if the parameter is mandatory, it must have value assigned.
-		If not, the method throws an exception."""
-		if self.is_optional:
-			return
-		if self.value is None:
-			raise ValueError(f'Mandatory single argument has no value: {self}')
-
-	def set_scalar_value_from_str(self, string: str) -> None:
-		"""Sets scalar value from input string"""
-		self.value = self.conv_from_scpi_string.get_value(string)
-
-	def check_consistency(self) -> None:
-		"""Checks the consistency of the object"""
-		if self.value is None:
-			return
-		if isinstance(self.value, list):
-			if self.data_type.is_scalar:
-				raise Exception(f'Argument real data type is list, but it is declared as {self.data_type}. Value: {self.value}')
-		else:
-			if self.data_type.is_list:
-				raise Exception(f'Argument real data type is scalar, but it is declared as {self.data_type}. Value: {self.value}')
+from .ConverterFromScpiString import ConverterFromScpiString
+from .ConverterToScpiString import ConverterToScpiString
+from .Types import DataType
+
+
+class ArgSingle(object):
+	"""Single Argument outside a structure - used for composing query arguments.
+	Contains the argument value as well (self.value)."""
+
+	def __init__(self, name: str, value, data_type: DataType, is_optional: bool = False, is_open_list: bool = False, repetition: int = 1, intern_link: str = None):
+		self.name = name if name else ''
+		self.argument_ix = None
+		self.value = value
+		self.data_type = data_type
+		self.is_optional = is_optional
+		self.is_open_list = is_open_list
+		self.repetition = repetition
+		self.intern_link = intern_link
+		self.conv_from_scpi_string = None
+		self.conv_to_scpi_string = None
+
+		if self.data_type == DataType.Enum:
+			self.assert_mandatory_has_value(self)
+			if self.value is not None:
+				self.enum_type = type(self.value)
+				self.conv_from_scpi_string = ConverterFromScpiString(self.data_type, self.enum_type)
+				self.conv_to_scpi_string = ConverterToScpiString(self.data_type, self.enum_type)
+		elif self.data_type == DataType.EnumList:
+			self.assert_mandatory_has_value(self)
+			if self.value is not None:
+				self.enum_type = type(self.value[0])
+				self.conv_from_scpi_string = ConverterFromScpiString(self.data_type, self.enum_type)
+				self.conv_to_scpi_string = ConverterToScpiString(self.data_type, self.enum_type)
+		else:
+			self.conv_from_scpi_string = ConverterFromScpiString(self.data_type)
+			self.conv_to_scpi_string = ConverterToScpiString(self.data_type)
+
+		self.check_consistency()
+
+	@classmethod
+	def as_open_list(cls, name: str, value: object, data_type: DataType) -> 'ArgSingle':
+		"""Creates new ArgSingle of open list type.Use this method for all non-interleaved list types. \n
+		:param name: name of the argument.
+		:param value: value of the argument.
+		:param data_type: data type of the argument.
+		:return: ArgSingle object of an open list type."""
+		return cls(name, value, data_type, False, True, 1, None)
+
+	def __str__(self):
+		opt = '~' if self.is_optional else ''
+		name = f" '{self.name}'" if self.name != '' else ''
+		out = f"SingleArg {opt}{self.data_type.name}{name}"
+
+		if self.is_open_list is False and self.repetition > 1:
+			out += f' [{self.repetition}]'
+		elif self.is_open_list is True:
+			out += f' [{self.repetition}...]'
+		if self.intern_link:
+			out += f", Linking: '{self.intern_link}'"
+		if self.value:
+			out += f', value: {self.value}'
+		else:
+			out += ", <no value>"
+		if self.intern_link:
+			out += f", Linking: '{self.intern_link}'"
+		return out
+
+	# noinspection PyUnusedLocal
+	def has_value(self, value_obj=None) -> bool:
+		"""Returns true, if the argument has value."""
+		return self.value is not None
+
+	# noinspection PyUnusedLocal
+	def assert_is_optional(self, obj=None) -> None:
+		"""Asserts that the parameter is optional.
+		If not, the method throws an exception."""
+		if self.is_optional:
+			return
+		raise Exception(f'Single argument is not optional: {self}')
+
+	# noinspection PyUnusedLocal
+	def assert_mandatory_has_value(self, value_obj=None) -> None:
+		"""Asserts that if the parameter is mandatory, it must have value assigned.
+		If not, the method throws an exception."""
+		if self.is_optional:
+			return
+		if self.value is None:
+			raise ValueError(f'Mandatory single argument has no value: {self}')
+
+	def set_scalar_value_from_str(self, string: str) -> None:
+		"""Sets scalar value from input string"""
+		self.value = self.conv_from_scpi_string.get_value(string)
+
+	def check_consistency(self) -> None:
+		"""Checks the consistency of the object"""
+		if self.value is None:
+			return
+		if isinstance(self.value, list):
+			if self.data_type.is_scalar:
+				raise Exception(f'Argument real data type is list, but it is declared as {self.data_type}. Value: {self.value}')
+		else:
+			if self.data_type.is_list:
+				raise Exception(f'Argument real data type is scalar, but it is declared as {self.data_type}. Value: {self.value}')
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/ArgSingleList.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/ArgSingleList.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from .ArgSingle import ArgSingle
-from .ArgStringComposer import compose_cmd_string_from_single_args
-
-
-class ArgSingleList(object):
-	"""Contains methods for composing cmd string for the list of single arguments.
-	Used in methods with 1+ set or query arguments.
-	The instance does not have a fixed args list, you can use the instance method compose_cmd_string with different arguments."""
-
-	def __init__(self):
-		self.args = None
-
-	def compose_cmd_string(self, arg1: ArgSingle, arg2: ArgSingle = None, arg3: ArgSingle = None, arg4: ArgSingle = None, arg5: ArgSingle = None, arg6: ArgSingle = None, arg7: ArgSingle = None, arg8: ArgSingle = None, arg9: ArgSingle = None):
-		"""Composes the string cmd argument from the arguments list.
-		Same treatment as in the ArgStructList.compose_cmd_string().
-		The difference is in handling the value of the argument."""
-		self.args = dict()
-
-		ix = 0
-		for arg in [arg1, arg2, arg3, arg4, arg5, arg6, arg7, arg8, arg9]:
-			if arg:
-				self.args[ix] = arg
-				ix += 1
-
-		return compose_cmd_string_from_single_args(self.args)
+from .ArgSingle import ArgSingle
+from .ArgStringComposer import compose_cmd_string_from_single_args
+
+
+class ArgSingleList(object):
+	"""Contains methods for composing cmd string for the list of single arguments.
+	Used in methods with 1+ set or query arguments.
+	The instance does not have a fixed args list, you can use the instance method compose_cmd_string with different arguments."""
+
+	def __init__(self):
+		self.args = None
+
+	def compose_cmd_string(self, arg1: ArgSingle, arg2: ArgSingle = None, arg3: ArgSingle = None, arg4: ArgSingle = None, arg5: ArgSingle = None, arg6: ArgSingle = None, arg7: ArgSingle = None, arg8: ArgSingle = None, arg9: ArgSingle = None):
+		"""Composes the string cmd argument from the arguments list.
+		Same treatment as in the ArgStructList.compose_cmd_string().
+		The difference is in handling the value of the argument."""
+		self.args = dict()
+
+		ix = 0
+		for arg in [arg1, arg2, arg3, arg4, arg5, arg6, arg7, arg8, arg9]:
+			if arg:
+				self.args[ix] = arg
+				ix += 1
+
+		return compose_cmd_string_from_single_args(self.args)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/ArgSingleSuppressed.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/ArgSingleSuppressed.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from .Types import DataType
-
-
-class ArgSingleSuppressed(object):
-	"""Single suppressed Argument - used in Query_XxXx_Suppressed() to remove it from the returned value.
-	It does not contain:
-	- 'value' attribute, since this is discarded or linked internally directly  in the Query_XxXx_Suppressed().
-	- 'is_optional' attribute, since it is always mandatory."""
-
-	def __init__(self, argument_ix: int, data_type: DataType, is_open_list: bool = False, repetition: int = 1, intern_link: str = None):
-		self.name = ''
-		self.argument_ix = argument_ix
-		self.data_type = data_type
-		self.is_open_list = is_open_list
-		self.repetition = repetition
-		self.intern_link = intern_link
-
-	def __str__(self):
-		out = f"{self.data_type.name} '{self.name}' SuppressedArg"
-		if self.is_open_list is False and self.repetition > 1:
-			out += f' [{self.repetition}]'
-		elif self.is_open_list is True:
-			out += f' [{self.repetition}...]'
-
-		if self.intern_link:
-			out += f", Linking: '{self.intern_link}'"
-
-		return out
+from .Types import DataType
+
+
+class ArgSingleSuppressed(object):
+	"""Single suppressed Argument - used in Query_XxXx_Suppressed() to remove it from the returned value.
+	It does not contain:
+	- 'value' attribute, since this is discarded or linked internally directly  in the Query_XxXx_Suppressed().
+	- 'is_optional' attribute, since it is always mandatory."""
+
+	def __init__(self, argument_ix: int, data_type: DataType, is_open_list: bool = False, repetition: int = 1, intern_link: str = None):
+		self.name = ''
+		self.argument_ix = argument_ix
+		self.data_type = data_type
+		self.is_open_list = is_open_list
+		self.repetition = repetition
+		self.intern_link = intern_link
+
+	def __str__(self):
+		out = f"{self.data_type.name} '{self.name}' SuppressedArg"
+		if self.is_open_list is False and self.repetition > 1:
+			out += f' [{self.repetition}]'
+		elif self.is_open_list is True:
+			out += f' [{self.repetition}...]'
+
+		if self.intern_link:
+			out += f", Linking: '{self.intern_link}'"
+
+		return out
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/ArgStringComposer.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/ArgStringComposer.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,215 +1,215 @@
-"""Provides:
-- class SingleComposer - for composing SCPI string parameters from ArgSingle
-- class StructComposer - for composing SCPI string parameters from ArgStruct
-- function compose_cmd_string_from_struct_args - takes ArgStruct values and converts it to a SCPI string parameter.
-- function compose_cmd_string_from_single_args - takes ArgSingle[] values and converts them to a SCPI string parameter.
-The composing of the SCPI parameter string is similar for the ArgStruct and ArgSingle[] objects, therefore they share the same module."""
-
-from typing import Dict
-
-from .ArgSingle import ArgSingle
-from .ArgStruct import ArgStruct
-from .Utilities import get_plural_string
-
-
-class SingleComposer:
-	"""Composes strings for single argument.
-	Provides Composer interface with 3 functions:
-	- from_scalar_arg
-	- from_list_arg
-	- get_arg_list_size"""
-
-	@staticmethod
-	def from_scalar_arg(arg: ArgSingle) -> str:
-		"""Takes argument's scalar value and converts it to a SCPI parameter string."""
-		if not arg.is_optional and arg.value is None:
-			raise ValueError(f"StructArgComposer.from_scalar_arg() - mandatory argument's '{arg.name}' value is None")
-		assert arg.data_type.is_scalar, f"StructArgComposer.from_scalar_arg() - argument '{arg.name}' must be scalar. Data type: '{arg.data_type}'"
-		if arg.value is None:
-			return ''
-		return arg.conv_to_scpi_string.get_value(arg.value)
-
-	@staticmethod
-	def from_list_arg(arg: ArgSingle, start_ix=0, items_count=-1) -> str:
-		"""Takes argument's List of elements and converts it to a csv-string of SCPI parameters.
-		start_ix defines where to start in the list.
-		items_count defines how many items to take. -1 means all of them"""
-		if not arg.is_optional and arg.value is None:
-			raise ValueError(f"StructArgComposer.from_list_arg() - mandatory argument's '{arg.name}' value is None")
-		assert arg.data_type.is_list, f"StructArgComposer.from_list_arg() - argument must be list. Data type: '{arg.data_type}'"
-		if not arg.is_optional:
-			assert arg.value is not None, f"StructArgComposer.from_list_arg() - mandatory argument's '{arg.name}' value is None"
-		if arg.value is None:
-			return ''
-		if start_ix == 0 and items_count < 0:
-			return arg.conv_to_scpi_string.get_value(arg.value)
-		elif items_count < 0:
-			return arg.conv_to_scpi_string.get_value(arg.value[start_ix])
-		elif items_count == 0:
-			return ''
-		elif items_count > 0:
-			return arg.conv_to_scpi_string.get_value(arg.value[start_ix: start_ix + items_count])
-
-	@staticmethod
-	def get_arg_list_size(arg: ArgSingle) -> int:
-		"""Returns list size of the argument assuming it is a list.
-		If the argument is not a list, the method returns -1."""
-		if arg.data_type.is_scalar:
-			return -1
-		else:
-			return len(arg.value)
-
-
-class StructComposer:
-	"""Composes strings for structure arguments.
-	Provides Composer interface with 3 functions:
-	- from_scalar_arg
-	- from_list_arg
-	- get_arg_list_size \n
-	The StructComposer constructor has the owning struct instance as parameter, because this is needed to access the argument value."""
-
-	def __init__(self, struct):
-		self.struct = struct
-
-	def from_scalar_arg(self, arg: ArgStruct) -> str:
-		"""Returns a single argument value converted to string."""
-		assert arg.data_type.is_scalar, f"StructArgComposer.from_scalar_arg() - argument must be scalar. Data type: '{arg.data_type}'"
-		return arg.conv_to_scpi_string.get_value(getattr(self.struct, arg.name))
-
-	def from_list_arg(self, arg: ArgStruct, start_ix=0, items_count=-1) -> str:
-		"""Returns csv-string with all the elements from the argument value."""
-		assert arg.data_type.is_list, f"StructArgComposer.from_list_arg() - argument must be list. Data type: '{arg.data_type}'"
-		if start_ix == 0 and items_count < 0:
-			return arg.conv_to_scpi_string.get_value(getattr(self.struct, arg.name))
-		elif items_count < 0:
-			return arg.conv_to_scpi_string.get_value(getattr(self.struct, arg.name)[start_ix])
-		elif items_count == 0:
-			return ''
-		elif items_count > 0:
-			return arg.conv_to_scpi_string.get_value(getattr(self.struct, arg.name)[start_ix: start_ix + items_count])
-
-	def get_arg_list_size(self, arg: ArgStruct) -> int:
-		"""Returns list size of the argument assuming it is a list.
-		If the argument is not a list, the method returns -1."""
-		if arg.data_type.is_scalar:
-			return -1
-		else:
-			return len(getattr(self.struct, arg.name))
-
-
-def compose_cmd_string_from_struct_args(args: Dict[int, ArgStruct], composer: StructComposer, values_obj: object) -> str:
-	"""Returns SCPI-composed string based on the structure args specification."""
-	arg_count = len(args)
-	string_arg = []
-	arg_ix = 0
-	opt_null_ix = -1
-
-	# Non-repeated arguments - single values or arrays which are not open lists
-	# Non-open lists or scalars must be at the beginning of the definition
-	# Once the first open list argument is detected, continue further
-	while arg_ix < arg_count and args[arg_ix].is_open_list is False:
-		arg = args[arg_ix]
-		if arg.has_value(values_obj) is False:
-			arg.assert_is_optional(values_obj)
-			# The optional argument, which has no value. End the entire string_arg composition
-			opt_null_ix = arg_ix
-			break
-
-		if arg.repetition <= 1:
-			# No list, but scalar value
-			string_arg.append(composer.from_scalar_arg(arg))
-		else:
-			string_arg.append(composer.from_list_arg(arg, 0, arg.repetition))
-
-		arg_ix += 1
-	# End of non-repeated arguments
-
-	# If the optional argument without a value was not found, check if there are some more arguments to go through
-	if opt_null_ix < 0 and arg_ix < arg_count:
-		# Still some args to go
-		arg = args[arg_ix]
-		if arg.is_open_list:
-			# The previous loop ended because the next argument had is_open_list = True
-			if arg_ix == (arg_count - 1):
-				if arg.has_value(values_obj):
-					# The last argument, ignore the repetitions and convert the whole list to string
-					string_arg.append(composer.from_list_arg(arg))
-				else:
-					# The optional argument, which has no value. End the entire string_arg composition
-					arg.assert_is_optional(values_obj)
-					opt_null_ix = arg_ix
-			else:
-				# More than one arguments remaining. Loop through them interleaving the result strings
-				# Interleaving arguments must all have values
-
-				# Check if each list has at least Repetition number of elements
-				cycles_error = False
-				alignments_error = False
-				cycle = -1
-				data = {}
-				for x in range(arg_ix, arg_count):
-					arg = args[x]
-					curr_size: int = composer.get_arg_list_size(arg)
-					curr_cycle: int = curr_size // arg.repetition
-					curr_align: int = curr_size % arg.repetition
-					data[x] = (curr_size, curr_cycle, curr_align)
-
-					if curr_size < 0:
-						raise Exception(
-							f"Argument '{arg.name}' has repetitions, therefore it must be declared as a list. Current Declaration: '{arg.data_type}'")
-
-					if arg.repetition > curr_size:
-						raise Exception(f"Argument '{arg.name}' has repetitions {arg.repetition}, but its list size is only {curr_size}")
-
-					# noinspection PyChainedComparisons
-					if cycle >= 0 and curr_cycle != cycle:
-						cycles_error = True
-
-					cycle = curr_cycle
-
-					if curr_align != 0:
-						alignments_error = True
-
-				if cycles_error:
-					message = 'Arguments interleaving is not aligned - all the cycles must be the same. Actual cycles:\n'
-					for x in range(arg_ix, arg_count):
-						message += f'{args[x].name}[{data[x][0]}] sliced by {get_plural_string("element", args[x].repetition)} ' \
-							f'results in {data[x][0] / args[x].repetition} cycles\n'
-
-					raise Exception(message)
-
-				if alignments_error:
-					message = 'At least one argument has a list size not dividable by the defined repetitions:\n'
-					for x in range(arg_ix, arg_count):
-						message += f'{args[x].name}[{data[x][0]}] modulo {args[x].repetition}x results in {data[x][0] % args[x].repetition}\n'
-
-					raise Exception(message)
-
-				for x in range(cycle):
-					for y in range(arg_ix, arg_count):
-						arg = args[y]
-						string_arg.append(composer.from_list_arg(arg, arg.repetition * x, arg.repetition))
-
-	if opt_null_ix >= 0:
-		# Check the rest of the optional values, all of them must be without a value
-		rest = []
-		for y in range(opt_null_ix, arg_count):
-			arg = args[y]
-			if arg.has_value(values_obj):
-				rest.append(arg.name)
-
-		if len(rest):
-			msg = f"Optional Argument '{args[opt_null_ix].name}' has no value, but the further ones do. " \
-				f"If you skip an optional argument, you have to skip all the ones following it. " \
-				f"Clear the values for the rest of the argument(s):\n{', '.join(rest)}"
-			raise Exception(msg)
-
-	return ','.join(string_arg)
-
-
-def compose_cmd_string_from_single_args(args: Dict[int, ArgSingle]) -> str:
-	"""Returns SCPI-composed string based on the single args specification.
-	We can use the same function as for the struct arguments, with the difference of providing a SingleComposer.
-	Parameter value_obj is set to None, since each argument holds the value itself."""
-	# noinspection PyTypeChecker
-	return compose_cmd_string_from_struct_args(args, SingleComposer(), None)
+"""Provides:
+- class SingleComposer - for composing SCPI string parameters from ArgSingle
+- class StructComposer - for composing SCPI string parameters from ArgStruct
+- function compose_cmd_string_from_struct_args - takes ArgStruct values and converts it to a SCPI string parameter.
+- function compose_cmd_string_from_single_args - takes ArgSingle[] values and converts them to a SCPI string parameter.
+The composing of the SCPI parameter string is similar for the ArgStruct and ArgSingle[] objects, therefore they share the same module."""
+
+from typing import Dict
+
+from .ArgSingle import ArgSingle
+from .ArgStruct import ArgStruct
+from .Utilities import get_plural_string
+
+
+class SingleComposer:
+	"""Composes strings for single argument.
+	Provides Composer interface with 3 functions:
+	- from_scalar_arg
+	- from_list_arg
+	- get_arg_list_size"""
+
+	@staticmethod
+	def from_scalar_arg(arg: ArgSingle) -> str:
+		"""Takes argument's scalar value and converts it to a SCPI parameter string."""
+		if not arg.is_optional and arg.value is None:
+			raise ValueError(f"StructArgComposer.from_scalar_arg() - mandatory argument's '{arg.name}' value is None")
+		assert arg.data_type.is_scalar, f"StructArgComposer.from_scalar_arg() - argument '{arg.name}' must be scalar. Data type: '{arg.data_type}'"
+		if arg.value is None:
+			return ''
+		return arg.conv_to_scpi_string.get_value(arg.value)
+
+	@staticmethod
+	def from_list_arg(arg: ArgSingle, start_ix=0, items_count=-1) -> str:
+		"""Takes argument's List of elements and converts it to a csv-string of SCPI parameters.
+		start_ix defines where to start in the list.
+		items_count defines how many items to take. -1 means all of them"""
+		if not arg.is_optional and arg.value is None:
+			raise ValueError(f"StructArgComposer.from_list_arg() - mandatory argument's '{arg.name}' value is None")
+		assert arg.data_type.is_list, f"StructArgComposer.from_list_arg() - argument must be list. Data type: '{arg.data_type}'"
+		if not arg.is_optional:
+			assert arg.value is not None, f"StructArgComposer.from_list_arg() - mandatory argument's '{arg.name}' value is None"
+		if arg.value is None:
+			return ''
+		if start_ix == 0 and items_count < 0:
+			return arg.conv_to_scpi_string.get_value(arg.value)
+		elif items_count < 0:
+			return arg.conv_to_scpi_string.get_value(arg.value[start_ix])
+		elif items_count == 0:
+			return ''
+		elif items_count > 0:
+			return arg.conv_to_scpi_string.get_value(arg.value[start_ix: start_ix + items_count])
+
+	@staticmethod
+	def get_arg_list_size(arg: ArgSingle) -> int:
+		"""Returns list size of the argument assuming it is a list.
+		If the argument is not a list, the method returns -1."""
+		if arg.data_type.is_scalar:
+			return -1
+		else:
+			return len(arg.value)
+
+
+class StructComposer:
+	"""Composes strings for structure arguments.
+	Provides Composer interface with 3 functions:
+	- from_scalar_arg
+	- from_list_arg
+	- get_arg_list_size \n
+	The StructComposer constructor has the owning struct instance as parameter, because this is needed to access the argument value."""
+
+	def __init__(self, struct):
+		self.struct = struct
+
+	def from_scalar_arg(self, arg: ArgStruct) -> str:
+		"""Returns a single argument value converted to string."""
+		assert arg.data_type.is_scalar, f"StructArgComposer.from_scalar_arg() - argument must be scalar. Data type: '{arg.data_type}'"
+		return arg.conv_to_scpi_string.get_value(getattr(self.struct, arg.name))
+
+	def from_list_arg(self, arg: ArgStruct, start_ix=0, items_count=-1) -> str:
+		"""Returns csv-string with all the elements from the argument value."""
+		assert arg.data_type.is_list, f"StructArgComposer.from_list_arg() - argument must be list. Data type: '{arg.data_type}'"
+		if start_ix == 0 and items_count < 0:
+			return arg.conv_to_scpi_string.get_value(getattr(self.struct, arg.name))
+		elif items_count < 0:
+			return arg.conv_to_scpi_string.get_value(getattr(self.struct, arg.name)[start_ix])
+		elif items_count == 0:
+			return ''
+		elif items_count > 0:
+			return arg.conv_to_scpi_string.get_value(getattr(self.struct, arg.name)[start_ix: start_ix + items_count])
+
+	def get_arg_list_size(self, arg: ArgStruct) -> int:
+		"""Returns list size of the argument assuming it is a list.
+		If the argument is not a list, the method returns -1."""
+		if arg.data_type.is_scalar:
+			return -1
+		else:
+			return len(getattr(self.struct, arg.name))
+
+
+def compose_cmd_string_from_struct_args(args: Dict[int, ArgStruct], composer: StructComposer, values_obj: object) -> str:
+	"""Returns SCPI-composed string based on the structure args specification."""
+	arg_count = len(args)
+	string_arg = []
+	arg_ix = 0
+	opt_null_ix = -1
+
+	# Non-repeated arguments - single values or arrays which are not open lists
+	# Non-open lists or scalars must be at the beginning of the definition
+	# Once the first open list argument is detected, continue further
+	while arg_ix < arg_count and args[arg_ix].is_open_list is False:
+		arg = args[arg_ix]
+		if arg.has_value(values_obj) is False:
+			arg.assert_is_optional(values_obj)
+			# The optional argument, which has no value. End the entire string_arg composition
+			opt_null_ix = arg_ix
+			break
+
+		if arg.repetition <= 1:
+			# No list, but scalar value
+			string_arg.append(composer.from_scalar_arg(arg))
+		else:
+			string_arg.append(composer.from_list_arg(arg, 0, arg.repetition))
+
+		arg_ix += 1
+	# End of non-repeated arguments
+
+	# If the optional argument without a value was not found, check if there are some more arguments to go through
+	if opt_null_ix < 0 and arg_ix < arg_count:
+		# Still some args to go
+		arg = args[arg_ix]
+		if arg.is_open_list:
+			# The previous loop ended because the next argument had is_open_list = True
+			if arg_ix == (arg_count - 1):
+				if arg.has_value(values_obj):
+					# The last argument, ignore the repetitions and convert the whole list to string
+					string_arg.append(composer.from_list_arg(arg))
+				else:
+					# The optional argument, which has no value. End the entire string_arg composition
+					arg.assert_is_optional(values_obj)
+					opt_null_ix = arg_ix
+			else:
+				# More than one arguments remaining. Loop through them interleaving the result strings
+				# Interleaving arguments must all have values
+
+				# Check if each list has at least Repetition number of elements
+				cycles_error = False
+				alignments_error = False
+				cycle = -1
+				data = {}
+				for x in range(arg_ix, arg_count):
+					arg = args[x]
+					curr_size: int = composer.get_arg_list_size(arg)
+					curr_cycle: int = curr_size // arg.repetition
+					curr_align: int = curr_size % arg.repetition
+					data[x] = (curr_size, curr_cycle, curr_align)
+
+					if curr_size < 0:
+						raise Exception(
+							f"Argument '{arg.name}' has repetitions, therefore it must be declared as a list. Current Declaration: '{arg.data_type}'")
+
+					if arg.repetition > curr_size:
+						raise Exception(f"Argument '{arg.name}' has repetitions {arg.repetition}, but its list size is only {curr_size}")
+
+					# noinspection PyChainedComparisons
+					if cycle >= 0 and curr_cycle != cycle:
+						cycles_error = True
+
+					cycle = curr_cycle
+
+					if curr_align != 0:
+						alignments_error = True
+
+				if cycles_error:
+					message = 'Arguments interleaving is not aligned - all the cycles must be the same. Actual cycles:\n'
+					for x in range(arg_ix, arg_count):
+						message += f'{args[x].name}[{data[x][0]}] sliced by {get_plural_string("element", args[x].repetition)} ' \
+							f'results in {data[x][0] / args[x].repetition} cycles\n'
+
+					raise Exception(message)
+
+				if alignments_error:
+					message = 'At least one argument has a list size not dividable by the defined repetitions:\n'
+					for x in range(arg_ix, arg_count):
+						message += f'{args[x].name}[{data[x][0]}] modulo {args[x].repetition}x results in {data[x][0] % args[x].repetition}\n'
+
+					raise Exception(message)
+
+				for x in range(cycle):
+					for y in range(arg_ix, arg_count):
+						arg = args[y]
+						string_arg.append(composer.from_list_arg(arg, arg.repetition * x, arg.repetition))
+
+	if opt_null_ix >= 0:
+		# Check the rest of the optional values, all of them must be without a value
+		rest = []
+		for y in range(opt_null_ix, arg_count):
+			arg = args[y]
+			if arg.has_value(values_obj):
+				rest.append(arg.name)
+
+		if len(rest):
+			msg = f"Optional Argument '{args[opt_null_ix].name}' has no value, but the further ones do. " \
+				f"If you skip an optional argument, you have to skip all the ones following it. " \
+				f"Clear the values for the rest of the argument(s):\n{', '.join(rest)}"
+			raise Exception(msg)
+
+	return ','.join(string_arg)
+
+
+def compose_cmd_string_from_single_args(args: Dict[int, ArgSingle]) -> str:
+	"""Returns SCPI-composed string based on the single args specification.
+	We can use the same function as for the struct arguments, with the difference of providing a SingleComposer.
+	Parameter value_obj is set to None, since each argument holds the value itself."""
+	# noinspection PyTypeChecker
+	return compose_cmd_string_from_struct_args(args, SingleComposer(), None)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/ArgStruct.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/ArgStruct.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-from .ConverterFromScpiString import ConverterFromScpiString
-from .ConverterToScpiString import ConverterToScpiString
-from .Types import DataType
-
-
-class ArgStruct(object):
-	"""Describes an argument in data structures.
-	This info is used to parse a string query response to the output structure,
-	or to parse the output structure to the string parameter for writing.
-	Contains reference to the value in the owning structure."""
-
-	def __init__(self, name: str, data_type: DataType, enum_type=None, is_optional=False, is_open_list=False, repetition=1, intern_link: str = None):
-		self.argument_ix = None
-		self.name = name
-		self.data_type = data_type
-		self.is_optional = is_optional
-		self.is_open_list = is_open_list
-		self.repetition = repetition
-		self.intern_link = intern_link
-		self.enum_type = enum_type
-		self.conv_from_scpi_string = ConverterFromScpiString(self.data_type, self.enum_type)
-		self.conv_to_scpi_string = ConverterToScpiString(self.data_type, self.enum_type)
-
-	@classmethod
-	def scalar_int(cls, name: str, intern_link: str = None):
-		"""Describes mandatory scalar integer argument."""
-		return cls(name, DataType.Integer, None, False, False, 1, intern_link)
-
-	@classmethod
-	def scalar_int_ext(cls, name: str, intern_link: str = None):
-		"""Describes mandatory scalar extended integer argument."""
-		return cls(name, DataType.IntegerExt, None, False, False, 1, intern_link)
-
-	@classmethod
-	def scalar_str(cls, name: str, intern_link: str = None):
-		"""Describes mandatory scalar string argument."""
-		return cls(name, DataType.String, None, False, False, 1, intern_link)
-
-	@classmethod
-	def scalar_raw_str(cls, name: str, intern_link: str = None):
-		"""Describes mandatory scalar raw string argument."""
-		return cls(name, DataType.RawString, None, False, False, 1, intern_link)
-
-	@classmethod
-	def scalar_bool(cls, name: str, intern_link: str = None):
-		"""Describes mandatory scalar boolean argument."""
-		return cls(name, DataType.Boolean, None, False, False, 1, intern_link)
-
-	@classmethod
-	def scalar_float(cls, name: str, intern_link: str = None):
-		"""Describes mandatory scalar float argument."""
-		return cls(name, DataType.Float, None, False, False, 1, intern_link)
-
-	@classmethod
-	def scalar_float_ext(cls, name: str, intern_link: str = None):
-		"""Describes mandatory scalar extended float argument."""
-		return cls(name, DataType.FloatExt, None, False, False, 1, intern_link)
-
-	@classmethod
-	def scalar_enum(cls, name: str, enum_type, intern_link: str = None):
-		"""Describes mandatory scalar float argument."""
-		return cls(name, DataType.Enum, enum_type, False, False, 1, intern_link)
-
-	@classmethod
-	def scalar_str_optional(cls, name: str, intern_link: str = None):
-		"""Describes optional scalar string argument."""
-		return cls(name, DataType.String, None, True, False, 1, intern_link)
-
-	@classmethod
-	def scalar_raw_str_optional(cls, name: str, intern_link: str = None):
-		"""Describes optional scalar raw string argument."""
-		return cls(name, DataType.RawString, None, True, False, 1, intern_link)
-
-	@classmethod
-	def scalar_bool_optional(cls, name: str, intern_link: str = None):
-		"""Describes optional scalar boolean argument."""
-		return cls(name, DataType.Boolean, None, True, False, 1, intern_link)
-
-	@classmethod
-	def scalar_int_optional(cls, name: str, intern_link: str = None):
-		"""Describes optional scalar integer argument."""
-		return cls(name, DataType.Integer, None, True, False, 1, intern_link)
-
-	@classmethod
-	def scalar_int_ext_optional(cls, name: str, intern_link: str = None):
-		"""Describes optional scalar extended integer argument."""
-		return cls(name, DataType.IntegerExt, None, True, False, 1, intern_link)
-
-	@classmethod
-	def scalar_float_optional(cls, name: str, intern_link: str = None):
-		"""Describes optional scalar float argument."""
-		return cls(name, DataType.Float, None, True, False, 1, intern_link)
-
-	@classmethod
-	def scalar_float_ext_optional(cls, name: str, intern_link: str = None):
-		"""Describes optional scalar extended float argument."""
-		return cls(name, DataType.FloatExt, None, True, False, 1, intern_link)
-
-	@classmethod
-	def scalar_enum_optional(cls, name: str, enum_type, intern_link: str = None):
-		"""Describes optional scalar float argument."""
-		return cls(name, DataType.Enum, enum_type, True, False, 1, intern_link)
-
-	def __str__(self):
-		opt = '~' if self.is_optional else ''
-		name = f" '{self.name}'" if self.name != '' else ''
-		out = f"StructArg {opt}{self.data_type.name}{name}"
-
-		if self.is_open_list is False and self.repetition > 1:
-			out += f' [{self.repetition}]'
-		elif self.is_open_list is True:
-			out += f' [{self.repetition}...]'
-		if self.intern_link:
-			out += f", Linking: '{self.intern_link}'"
-		return out
-
-	def has_value(self, obj) -> bool:
-		"""Returns True, if the entered object attribute has value."""
-		return getattr(obj, self.name) is not None
-
-	def assert_is_optional(self, obj) -> None:
-		"""Asserts that the parameter is optional.
-		If not, the method throws an exception."""
-		if self.is_optional:
-			return
-		value = getattr(obj, self.name)
-		if value is None:
-			raise Exception(f"Structure '{obj}', argument without value is not optional: {self}")
-		else:
-			raise Exception(f"Structure '{obj}', argument is not optional: {self}', value '{value}'")
-
-	def assert_mandatory_has_value(self, obj) -> None:
-		"""Asserts that if the parameter is mandatory, it must have value assigned.
-		If not, the method throws an exception."""
-		if self.is_optional:
-			return
-		if getattr(obj, self.name) is None:
-			raise ValueError(f"Mandatory structure '{obj}' argument '{self.name}' has no value.")
+from .ConverterFromScpiString import ConverterFromScpiString
+from .ConverterToScpiString import ConverterToScpiString
+from .Types import DataType
+
+
+class ArgStruct(object):
+	"""Describes an argument in data structures.
+	This info is used to parse a string query response to the output structure,
+	or to parse the output structure to the string parameter for writing.
+	Contains reference to the value in the owning structure."""
+
+	def __init__(self, name: str, data_type: DataType, enum_type=None, is_optional=False, is_open_list=False, repetition=1, intern_link: str = None):
+		self.argument_ix = None
+		self.name = name
+		self.data_type = data_type
+		self.is_optional = is_optional
+		self.is_open_list = is_open_list
+		self.repetition = repetition
+		self.intern_link = intern_link
+		self.enum_type = enum_type
+		self.conv_from_scpi_string = ConverterFromScpiString(self.data_type, self.enum_type)
+		self.conv_to_scpi_string = ConverterToScpiString(self.data_type, self.enum_type)
+
+	@classmethod
+	def scalar_int(cls, name: str, intern_link: str = None):
+		"""Describes mandatory scalar integer argument."""
+		return cls(name, DataType.Integer, None, False, False, 1, intern_link)
+
+	@classmethod
+	def scalar_int_ext(cls, name: str, intern_link: str = None):
+		"""Describes mandatory scalar extended integer argument."""
+		return cls(name, DataType.IntegerExt, None, False, False, 1, intern_link)
+
+	@classmethod
+	def scalar_str(cls, name: str, intern_link: str = None):
+		"""Describes mandatory scalar string argument."""
+		return cls(name, DataType.String, None, False, False, 1, intern_link)
+
+	@classmethod
+	def scalar_raw_str(cls, name: str, intern_link: str = None):
+		"""Describes mandatory scalar raw string argument."""
+		return cls(name, DataType.RawString, None, False, False, 1, intern_link)
+
+	@classmethod
+	def scalar_bool(cls, name: str, intern_link: str = None):
+		"""Describes mandatory scalar boolean argument."""
+		return cls(name, DataType.Boolean, None, False, False, 1, intern_link)
+
+	@classmethod
+	def scalar_float(cls, name: str, intern_link: str = None):
+		"""Describes mandatory scalar float argument."""
+		return cls(name, DataType.Float, None, False, False, 1, intern_link)
+
+	@classmethod
+	def scalar_float_ext(cls, name: str, intern_link: str = None):
+		"""Describes mandatory scalar extended float argument."""
+		return cls(name, DataType.FloatExt, None, False, False, 1, intern_link)
+
+	@classmethod
+	def scalar_enum(cls, name: str, enum_type, intern_link: str = None):
+		"""Describes mandatory scalar float argument."""
+		return cls(name, DataType.Enum, enum_type, False, False, 1, intern_link)
+
+	@classmethod
+	def scalar_str_optional(cls, name: str, intern_link: str = None):
+		"""Describes optional scalar string argument."""
+		return cls(name, DataType.String, None, True, False, 1, intern_link)
+
+	@classmethod
+	def scalar_raw_str_optional(cls, name: str, intern_link: str = None):
+		"""Describes optional scalar raw string argument."""
+		return cls(name, DataType.RawString, None, True, False, 1, intern_link)
+
+	@classmethod
+	def scalar_bool_optional(cls, name: str, intern_link: str = None):
+		"""Describes optional scalar boolean argument."""
+		return cls(name, DataType.Boolean, None, True, False, 1, intern_link)
+
+	@classmethod
+	def scalar_int_optional(cls, name: str, intern_link: str = None):
+		"""Describes optional scalar integer argument."""
+		return cls(name, DataType.Integer, None, True, False, 1, intern_link)
+
+	@classmethod
+	def scalar_int_ext_optional(cls, name: str, intern_link: str = None):
+		"""Describes optional scalar extended integer argument."""
+		return cls(name, DataType.IntegerExt, None, True, False, 1, intern_link)
+
+	@classmethod
+	def scalar_float_optional(cls, name: str, intern_link: str = None):
+		"""Describes optional scalar float argument."""
+		return cls(name, DataType.Float, None, True, False, 1, intern_link)
+
+	@classmethod
+	def scalar_float_ext_optional(cls, name: str, intern_link: str = None):
+		"""Describes optional scalar extended float argument."""
+		return cls(name, DataType.FloatExt, None, True, False, 1, intern_link)
+
+	@classmethod
+	def scalar_enum_optional(cls, name: str, enum_type, intern_link: str = None):
+		"""Describes optional scalar float argument."""
+		return cls(name, DataType.Enum, enum_type, True, False, 1, intern_link)
+
+	def __str__(self):
+		opt = '~' if self.is_optional else ''
+		name = f" '{self.name}'" if self.name != '' else ''
+		out = f"StructArg {opt}{self.data_type.name}{name}"
+
+		if self.is_open_list is False and self.repetition > 1:
+			out += f' [{self.repetition}]'
+		elif self.is_open_list is True:
+			out += f' [{self.repetition}...]'
+		if self.intern_link:
+			out += f", Linking: '{self.intern_link}'"
+		return out
+
+	def has_value(self, obj) -> bool:
+		"""Returns True, if the entered object attribute has value."""
+		return getattr(obj, self.name) is not None
+
+	def assert_is_optional(self, obj) -> None:
+		"""Asserts that the parameter is optional.
+		If not, the method throws an exception."""
+		if self.is_optional:
+			return
+		value = getattr(obj, self.name)
+		if value is None:
+			raise Exception(f"Structure '{obj}', argument without value is not optional: {self}")
+		else:
+			raise Exception(f"Structure '{obj}', argument is not optional: {self}', value '{value}'")
+
+	def assert_mandatory_has_value(self, obj) -> None:
+		"""Asserts that if the parameter is mandatory, it must have value assigned.
+		If not, the method throws an exception."""
+		if self.is_optional:
+			return
+		if getattr(obj, self.name) is None:
+			raise ValueError(f"Mandatory structure '{obj}' argument '{self.name}' has no value.")
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/ArgStructList.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/ArgStructList.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-from .ArgStringComposer import StructComposer, compose_cmd_string_from_struct_args
-from .ArgStructStringParser import ArgStructStringParser
-from .StructBase import StructBase
-
-
-class ArgStructList(object):
-	"""Contains methods for composing cmd string and parsing cmd response to the provided structure instance."""
-
-	RAW_DATA_PROP_NAME = 'RawReturnData'
-
-	def __init__(self, struct):
-		self.__struct = struct
-		self.args = self.__get_struct_arg_attrs()
-
-	def __str__(self):
-		return f"'{self.__struct.__class__.__name__}', {len(self.args)} args: [ {', '.join([self.args[x].name for x in self.args])} ]"
-
-	def __get_struct_arg_attrs(self):
-		"""Fills self.args with the dictionary of ArgStruct list.
-		Dictionary key is the argument order (argument_ix)."""
-		# noinspection PyUnresolvedReferences,PyProtectedMember
-		args_list = StructBase._StructBase__get_meta_args_list(None, self.__struct)
-		# meta_data = getattr(self.__struct, '_{}__meta_args_list'.format(self.__struct.__class__.__name__))
-		args = dict()
-		for x in args_list:
-			args[x.argument_ix] = x
-
-		return args
-
-	def parse_from_cmd_response(self, content: str):
-		"""Fills the structure from the entered string content (command response)."""
-		if hasattr(self.__struct, ArgStructList.RAW_DATA_PROP_NAME):
-			setattr(self.__struct, ArgStructList.RAW_DATA_PROP_NAME, content)
-
-		parser = ArgStructStringParser(self.__struct, content)
-		arg_count = len(self.args)
-		arg_ix = 0
-
-		# Non-repeated arguments
-		while arg_ix < arg_count and self.args[arg_ix].is_open_list is False:
-			arg = self.args[arg_ix]
-			if arg.repetition <= 1:
-				# No list, but scalar value
-				parser.to_scalar_value(arg)
-			else:
-				# List with a fixed size, not repeated
-				parser.to_list_value(arg, True, 0, arg.repetition, arg.repetition, 1)
-
-			arg_ix += 1
-
-		if arg_ix < arg_count:
-			arg = self.args[arg_ix]
-			# Still some args to go
-			if arg.is_open_list is True:
-				# The previous loop ended because the next argument had is_open_list True
-				if arg_ix == (arg_count - 1):
-					# This is the last argument, ignore the repetitions and take the whole rest of the elements
-					parser.to_list_value(arg, True, 0, parser.remaining, parser.remaining, 1)
-				else:
-					# More than one arguments remaining. Loop through them interleaving the result strings
-					open_list_args = {key: value for key, value in self.args.items() if key >= arg_ix}
-
-					# Accumulate the number of repetitions from all the open_list_args
-					period: int = sum(open_list_args[ix].repetition for ix in open_list_args)
-					reminder: int = parser.remaining % period
-					if reminder != 0:
-						raise Exception(
-							f'Arguments parsing is not aligned - source string elements remaining to parse {parser.remaining}'
-							f'is not dividable by the summary Period {period} of all the open list arguments:\n' + '\n'.join(['{}'.format(x) for x in open_list_args]))
-					# Go through the arguments and accumulate the list content
-					offset = 0
-					for x in open_list_args:
-						arg = open_list_args[x]
-						parser.to_list_value(arg, False, offset, arg.repetition, period, -1)
-						offset += arg.repetition
-
-	def compose_cmd_string(self):
-		"""Composes the string argument from the structure for sending to the instrument."""
-		return compose_cmd_string_from_struct_args(self.args, StructComposer(self.__struct), self.__struct)
+from .ArgStringComposer import StructComposer, compose_cmd_string_from_struct_args
+from .ArgStructStringParser import ArgStructStringParser
+from .StructBase import StructBase
+
+
+class ArgStructList(object):
+	"""Contains methods for composing cmd string and parsing cmd response to the provided structure instance."""
+
+	RAW_DATA_PROP_NAME = 'RawReturnData'
+
+	def __init__(self, struct):
+		self.__struct = struct
+		self.args = self.__get_struct_arg_attrs()
+
+	def __str__(self):
+		return f"'{self.__struct.__class__.__name__}', {len(self.args)} args: [ {', '.join([self.args[x].name for x in self.args])} ]"
+
+	def __get_struct_arg_attrs(self):
+		"""Fills self.args with the dictionary of ArgStruct list.
+		Dictionary key is the argument order (argument_ix)."""
+		# noinspection PyUnresolvedReferences,PyProtectedMember
+		args_list = StructBase._StructBase__get_meta_args_list(None, self.__struct)
+		# meta_data = getattr(self.__struct, '_{}__meta_args_list'.format(self.__struct.__class__.__name__))
+		args = dict()
+		for x in args_list:
+			args[x.argument_ix] = x
+
+		return args
+
+	def parse_from_cmd_response(self, content: str):
+		"""Fills the structure from the entered string content (command response)."""
+		if hasattr(self.__struct, ArgStructList.RAW_DATA_PROP_NAME):
+			setattr(self.__struct, ArgStructList.RAW_DATA_PROP_NAME, content)
+
+		parser = ArgStructStringParser(self.__struct, content)
+		arg_count = len(self.args)
+		arg_ix = 0
+
+		# Non-repeated arguments
+		while arg_ix < arg_count and self.args[arg_ix].is_open_list is False:
+			arg = self.args[arg_ix]
+			if arg.repetition <= 1:
+				# No list, but scalar value
+				parser.to_scalar_value(arg)
+			else:
+				# List with a fixed size, not repeated
+				parser.to_list_value(arg, True, 0, arg.repetition, arg.repetition, 1)
+
+			arg_ix += 1
+
+		if arg_ix < arg_count:
+			arg = self.args[arg_ix]
+			# Still some args to go
+			if arg.is_open_list is True:
+				# The previous loop ended because the next argument had is_open_list True
+				if arg_ix == (arg_count - 1):
+					# This is the last argument, ignore the repetitions and take the whole rest of the elements
+					parser.to_list_value(arg, True, 0, parser.remaining, parser.remaining, 1)
+				else:
+					# More than one arguments remaining. Loop through them interleaving the result strings
+					open_list_args = {key: value for key, value in self.args.items() if key >= arg_ix}
+
+					# Accumulate the number of repetitions from all the open_list_args
+					period: int = sum(open_list_args[ix].repetition for ix in open_list_args)
+					reminder: int = parser.remaining % period
+					if reminder != 0:
+						raise Exception(
+							f'Arguments parsing is not aligned - source string elements remaining to parse {parser.remaining}'
+							f'is not dividable by the summary Period {period} of all the open list arguments:\n' + '\n'.join(['{}'.format(x) for x in open_list_args]))
+					# Go through the arguments and accumulate the list content
+					offset = 0
+					for x in open_list_args:
+						arg = open_list_args[x]
+						parser.to_list_value(arg, False, offset, arg.repetition, period, -1)
+						offset += arg.repetition
+
+	def compose_cmd_string(self):
+		"""Composes the string argument from the structure for sending to the instrument."""
+		return compose_cmd_string_from_struct_args(self.args, StructComposer(self.__struct), self.__struct)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/ArgStructStringParser.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/ArgStructStringParser.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from . import Utilities
-from .ArgStruct import ArgStruct
-
-
-class ArgStructStringParser:
-	"""Class for parsing a response from the instrument to an output structure of arguments.
-	It is used by the ArgStructList class for filling structures with return values."""
-
-	def __init__(self, struct, value: str):
-		self.struct = struct
-		self.elements = value.split(',')
-		self.count = len(self.elements)
-		self.position = 0
-
-	@property
-	def remaining(self) -> int:
-		"""Remaining items to parse."""
-		return self.count - self.position
-
-	def to_scalar_value(self, arg: ArgStruct):
-		"""Parses the current element to a scalar argument."""
-		assert arg.data_type.is_scalar, f'to_scalar_value() method only works with scalar values. Data type: {arg.data_type}'
-		if self.position >= self.count:
-			raise Exception(
-				f"Cannot parse a scalar value to structure argument. Response contains only {self.count} elements, "
-				f"argument '{arg.name}' has position {self.position + 1}.\n"
-				f"Response (commas replaced by new lines):\n" + Utilities.truncate_string_from_end('\n'.join(self.elements), 1000))
-		string = self.elements[self.position]
-		value = arg.conv_from_scpi_string.get_one_element_value(string)
-		setattr(self.struct, arg.name, value)
-		self.position += 1
-
-	def to_list_value(self, arg: ArgStruct, increase_pos: bool, offset: int, count: int, period: int, cycles: int) -> None:
-		"""Parses more elements to the list argument - slicing."""
-		assert arg.data_type.is_list, f'to_list_value method only works with list values. Data type: {arg.data_type}'
-		if cycles < 0:
-			cycles = self.remaining // period
-		if self.position >= self.count:
-			raise Exception(
-				f"Cannot parse an list value to the argument '{arg.name}', "
-				f"because the element position {self.position} is over the parsed list length {self.count}")
-		if (self.position + offset + count) > self.count:
-			raise Exception(
-				f"Cannot parse the whole list value to the argument '{arg.name}', because the element position {self.position} "
-				f"plus the argument offset {offset} and argument length {count} would be over the parsed list length {self.count}")
-
-		result = []
-		for cycle in range(cycles):
-			start_ix = self.position + (cycle * period) + offset
-			for i in range(count):
-				result.append(arg.conv_from_scpi_string.get_one_element_value(self.elements[start_ix + i]))
-
-		if increase_pos:
-			self.position += count
-
-		setattr(self.struct, arg.name, result)
+from . import Utilities
+from .ArgStruct import ArgStruct
+
+
+class ArgStructStringParser:
+	"""Class for parsing a response from the instrument to an output structure of arguments.
+	It is used by the ArgStructList class for filling structures with return values."""
+
+	def __init__(self, struct, value: str):
+		self.struct = struct
+		self.elements = value.split(',')
+		self.count = len(self.elements)
+		self.position = 0
+
+	@property
+	def remaining(self) -> int:
+		"""Remaining items to parse."""
+		return self.count - self.position
+
+	def to_scalar_value(self, arg: ArgStruct):
+		"""Parses the current element to a scalar argument."""
+		assert arg.data_type.is_scalar, f'to_scalar_value() method only works with scalar values. Data type: {arg.data_type}'
+		if self.position >= self.count:
+			raise Exception(
+				f"Cannot parse a scalar value to structure argument. Response contains only {self.count} elements, "
+				f"argument '{arg.name}' has position {self.position + 1}.\n"
+				f"Response (commas replaced by new lines):\n" + Utilities.truncate_string_from_end('\n'.join(self.elements), 1000))
+		string = self.elements[self.position]
+		value = arg.conv_from_scpi_string.get_one_element_value(string)
+		setattr(self.struct, arg.name, value)
+		self.position += 1
+
+	def to_list_value(self, arg: ArgStruct, increase_pos: bool, offset: int, count: int, period: int, cycles: int) -> None:
+		"""Parses more elements to the list argument - slicing."""
+		assert arg.data_type.is_list, f'to_list_value method only works with list values. Data type: {arg.data_type}'
+		if cycles < 0:
+			cycles = self.remaining // period
+		if self.position >= self.count:
+			raise Exception(
+				f"Cannot parse an list value to the argument '{arg.name}', "
+				f"because the element position {self.position} is over the parsed list length {self.count}")
+		if (self.position + offset + count) > self.count:
+			raise Exception(
+				f"Cannot parse the whole list value to the argument '{arg.name}', because the element position {self.position} "
+				f"plus the argument offset {offset} and argument length {count} would be over the parsed list length {self.count}")
+
+		result = []
+		for cycle in range(cycles):
+			start_ix = self.position + (cycle * period) + offset
+			for i in range(count):
+				result.append(arg.conv_from_scpi_string.get_one_element_value(self.elements[start_ix + i]))
+
+		if increase_pos:
+			self.position += count
+
+		setattr(self.struct, arg.name, result)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/CommandsGroup.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/CommandsGroup.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-from enum import Enum
-from typing import List
-from .Core import Core
-from .RepeatedCapability import RepeatedCapability as RepCap
-from .InstrumentErrors import DriverValueError
-
-
-class CommandsGroup:
-	"""Contains methods dealing with RepCaps and Group object cloning"""
-
-	def __init__(self, group_name: str, core: Core, parent: 'CommandsGroup'):
-		"""Constructor with header name, group property name and the start value"""
-
-		self.group_name = group_name
-		self._core = core
-		self.parent = parent
-		self.io = core.io
-		self.existing_children = []
-		self.rep_cap: RepCap or None = None
-		self.multi_repcap_types: str = ''
-		if parent:
-			parent.existing_children.append(self)
-
-	def __str__(self):
-		"""String representation of the CommandsGroup"""
-		out = f"SCPI Commands Group {self.group_name}"
-		if self.has_repcap():
-			out += f', RepCap {self.rep_cap.name} = {self.rep_cap.get_enum_value()}'
-		return out
-
-	def has_repcap(self) -> bool:
-		"""Returns True, if the group has a RepCap.
-		Returns False for a group with MultiRepCaps"""
-		return self.rep_cap is not None
-
-	def has_multi_repcaps(self) -> bool:
-		"""Returns True for a group with MultiRepCaps"""
-		return self.multi_repcap_types != ''
-
-	def add_existing_child(self, child: 'CommandsGroup') -> None:
-		"""Adds the child to the parent's list of created children.
-		This is used when the group is cloned, where the whole existing tree of groups have to be recreated"""
-		self.existing_children.append(child)
-
-	def set_repcap_enum_value(self, enum_value: Enum) -> None:
-		"""Sets RepCap value as enum
-		Default is not allowed."""
-		try:
-			self.rep_cap.set_enum_value(enum_value)
-		except ValueError:
-			raise DriverValueError(self.io.resource_name, f"Commands group RepCap value '{self.rep_cap.name}.Default' cannot be set. Please select a concrete value.")
-
-	def get_repcap_enum_value(self) -> Enum:
-		"""Returns RepCap value as enum"""
-		return self.rep_cap.get_enum_value()
-
-	def get_repcap_cmd_value(self, enum_value: Enum, enum_type) -> str:
-		"""Returns the current string of RepCapCmdValue for the entered RepCapEnumName
-		The enum_value can be a repcap of the current CommandsGroup or any of their parents"""
-		# Use the static functions of the RepeatedCapability to get the non-default value
-		# It is faster, since there is no need to use the RepCap instance
-		if not RepCap.clsm_is_default_value(enum_value, enum_type):
-			return RepCap.clsm_get_cmd_string_value(enum_value, enum_type)
-		# Default value - get it from the group or the parent groups
-		group = self
-		while group is not None:
-			if group.has_repcap():
-				if group.rep_cap.matches_type(enum_type):
-					return group.rep_cap.get_cmd_string_value()
-			group = group.parent
-
-		# repCapEnumName not found in single repcaps. Check the multiRepCaps
-		group = self
-		while group is not None:
-			if group.has_multi_repcaps():
-				if str(enum_type.__name__) in group.multi_repcap_types.split(','):
-					# Found in the multiple repcaps, create more fitting exception message
-					raise DriverValueError(
-						self.io.resource_name,
-						f"You can not use the RepCap value '{enum_value}', "
-						f"because its real value is not defined in any of the parent command groups. Please select a concrete value.")
-			group = group.parent
-
-		# repCapEnumName not found, create exception message
-		group = self
-		groups = []
-		while group is not None:
-			item = group.group_name
-			if group.has_repcap():
-				item += f' => {group.rep_cap.name}'
-			groups.insert(0, item)
-			group = group.parent
-
-		groups_chain = str.join("\n", groups)
-		raise DriverValueError(
-			self.io.resource_name,
-			f"Error replacing RepCaps in the SCPI command:"
-			f"RepCap '{enum_type}' not found in the group chain:\n{groups_chain}")
-
-	def get_owners_chain(self, stop: 'CommandsGroup' = None) -> List['CommandsGroup']:
-		"""Returns the owners chain including itself up to the entered point or up to the root by default"""
-		chain = []
-		group = self
-		while group != stop:
-			chain.append(group)
-			group = group.parent
-		return chain
-
-	def get_self_and_desc_existing_children(self) -> List['CommandsGroup']:
-		"""Get all the existing descendant groups recursively"""
-		all_descendants = [self]
-		for x in self.existing_children:
-			all_descendants.extend(x.get_self_and_desc_existing_children())
-		return all_descendants
-
-	def synchronize_repcaps(self, new_group) -> None:
-		"""Clones the existing group repeated capabilities to the new one.
-		Because of the lazy group properties, the group clones are created by accessing the repcaps in them"""
-		all_existing = filter(lambda grp: grp.has_repcap(), self.get_self_and_desc_existing_children())
-		for x in all_existing:
-			chain = x.get_owners_chain(self)
-			chain.reverse()
-			group = new_group
-			for item in chain:
-				group = getattr(group, item.group_name)
-			fnc = getattr(group, x.rep_cap.method_set_name)
-			fnc(x.rep_cap.get_enum_value())
-
-	def restore_repcaps(self) -> None:
-		"""Sets RepCaps of the Group and its children groups to their initial values"""
-		all_existing = filter(lambda grp: grp.has_repcap(), self.get_self_and_desc_existing_children())
-		for x in all_existing:
-			x.rep_cap.set_to_start_value()
+from enum import Enum
+from typing import List
+from .Core import Core
+from .RepeatedCapability import RepeatedCapability as RepCap
+from .InstrumentErrors import DriverValueError
+
+
+class CommandsGroup:
+	"""Contains methods dealing with RepCaps and Group object cloning"""
+
+	def __init__(self, group_name: str, core: Core, parent: 'CommandsGroup'):
+		"""Constructor with header name, group property name and the start value"""
+
+		self.group_name = group_name
+		self._core = core
+		self.parent = parent
+		self.io = core.io
+		self.existing_children = []
+		self.rep_cap: RepCap or None = None
+		self.multi_repcap_types: str = ''
+		if parent:
+			parent.existing_children.append(self)
+
+	def __str__(self):
+		"""String representation of the CommandsGroup"""
+		out = f"SCPI Commands Group {self.group_name}"
+		if self.has_repcap():
+			out += f', RepCap {self.rep_cap.name} = {self.rep_cap.get_enum_value()}'
+		return out
+
+	def has_repcap(self) -> bool:
+		"""Returns True, if the group has a RepCap.
+		Returns False for a group with MultiRepCaps"""
+		return self.rep_cap is not None
+
+	def has_multi_repcaps(self) -> bool:
+		"""Returns True for a group with MultiRepCaps"""
+		return self.multi_repcap_types != ''
+
+	def add_existing_child(self, child: 'CommandsGroup') -> None:
+		"""Adds the child to the parent's list of created children.
+		This is used when the group is cloned, where the whole existing tree of groups have to be recreated"""
+		self.existing_children.append(child)
+
+	def set_repcap_enum_value(self, enum_value: Enum) -> None:
+		"""Sets RepCap value as enum
+		Default is not allowed."""
+		try:
+			self.rep_cap.set_enum_value(enum_value)
+		except ValueError:
+			raise DriverValueError(self.io.resource_name, f"Commands group RepCap value '{self.rep_cap.name}.Default' cannot be set. Please select a concrete value.")
+
+	def get_repcap_enum_value(self) -> Enum:
+		"""Returns RepCap value as enum"""
+		return self.rep_cap.get_enum_value()
+
+	def get_repcap_cmd_value(self, enum_value: Enum, enum_type) -> str:
+		"""Returns the current string of RepCapCmdValue for the entered RepCapEnumName
+		The enum_value can be a repcap of the current CommandsGroup or any of their parents"""
+		# Use the static functions of the RepeatedCapability to get the non-default value
+		# It is faster, since there is no need to use the RepCap instance
+		if not RepCap.clsm_is_default_value(enum_value, enum_type):
+			return RepCap.clsm_get_cmd_string_value(enum_value, enum_type)
+		# Default value - get it from the group or the parent groups
+		group = self
+		while group is not None:
+			if group.has_repcap():
+				if group.rep_cap.matches_type(enum_type):
+					return group.rep_cap.get_cmd_string_value()
+			group = group.parent
+
+		# repCapEnumName not found in single repcaps. Check the multiRepCaps
+		group = self
+		while group is not None:
+			if group.has_multi_repcaps():
+				if str(enum_type.__name__) in group.multi_repcap_types.split(','):
+					# Found in the multiple repcaps, create more fitting exception message
+					raise DriverValueError(
+						self.io.resource_name,
+						f"You can not use the RepCap value '{enum_value}', "
+						f"because its real value is not defined in any of the parent command groups. Please select a concrete value.")
+			group = group.parent
+
+		# repCapEnumName not found, create exception message
+		group = self
+		groups = []
+		while group is not None:
+			item = group.group_name
+			if group.has_repcap():
+				item += f' => {group.rep_cap.name}'
+			groups.insert(0, item)
+			group = group.parent
+
+		groups_chain = str.join("\n", groups)
+		raise DriverValueError(
+			self.io.resource_name,
+			f"Error replacing RepCaps in the SCPI command:"
+			f"RepCap '{enum_type}' not found in the group chain:\n{groups_chain}")
+
+	def get_owners_chain(self, stop: 'CommandsGroup' = None) -> List['CommandsGroup']:
+		"""Returns the owners chain including itself up to the entered point or up to the root by default"""
+		chain = []
+		group = self
+		while group != stop:
+			chain.append(group)
+			group = group.parent
+		return chain
+
+	def get_self_and_desc_existing_children(self) -> List['CommandsGroup']:
+		"""Get all the existing descendant groups recursively"""
+		all_descendants = [self]
+		for x in self.existing_children:
+			all_descendants.extend(x.get_self_and_desc_existing_children())
+		return all_descendants
+
+	def synchronize_repcaps(self, new_group) -> None:
+		"""Clones the existing group repeated capabilities to the new one.
+		Because of the lazy group properties, the group clones are created by accessing the repcaps in them"""
+		all_existing = filter(lambda grp: grp.has_repcap(), self.get_self_and_desc_existing_children())
+		for x in all_existing:
+			chain = x.get_owners_chain(self)
+			chain.reverse()
+			group = new_group
+			for item in chain:
+				group = getattr(group, item.group_name)
+			fnc = getattr(group, x.rep_cap.method_set_name)
+			fnc(x.rep_cap.get_enum_value())
+
+	def restore_repcaps(self) -> None:
+		"""Sets RepCaps of the Group and its children groups to their initial values"""
+		all_existing = filter(lambda grp: grp.has_repcap(), self.get_self_and_desc_existing_children())
+		for x in all_existing:
+			x.rep_cap.set_to_start_value()
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/Conversions.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/Conversions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,589 +1,606 @@
-import math
-import struct
-import sys
-from enum import Enum
-from typing import List
-
-from . import Utilities
-
-
-class BinFloatFormat(Enum):
-	"""Binary format of a float number."""
-	Single_4bytes = 1
-	Single_4bytes_swapped = 2
-	Double_8bytes = 3
-	Double_8bytes_swapped = 4
-
-
-class BinIntFormat(Enum):
-	"""Binary format of an integer number."""
-	Integer32_4bytes = 1
-	Integer32_4bytes_swapped = 2
-	Integer16_2bytes = 3
-	Integer16_2bytes_swapped = 4
-
-
-def assert_string_data(value: str) -> None:
-	"""Asserts value is string type."""
-	assert isinstance(value, str), f"Input value type must be string. Actual type: {type(value)}, value: {value}"
-
-
-def assert_list_data(value: list) -> None:
-	"""Asserts value is list type."""
-	assert isinstance(value, list), f"Input value type must be a list. Actual type: {type(value)}, value: {value}"
-
-
-def _get_endianness_symbol(swap_endianness: bool) -> str:
-	"""Based on the current endianness returns the symbol used in the 'struct' module."""
-	if swap_endianness is False:
-		return '@'
-	elif swap_endianness is True and sys.byteorder == 'little':
-		return '>'
-	else:
-		return '<'
-
-
-def bytes_to_float32_list(data: bytes, swap_endianness=False) -> List[float]:
-	"""Converts bytes to list of floats - one number is represented by 4 bytes."""
-	fmt = f'{_get_endianness_symbol(swap_endianness)}{len(data) // 4}f'
-	return list(struct.unpack(fmt, data))
-
-
-def bytes_to_double64_list(data: bytes, swap_endianness=False) -> List[float]:
-	"""Converts bytes to list of doubles - one number is represented by 8 bytes."""
-	fmt = f'{_get_endianness_symbol(swap_endianness)}{len(data) // 8}d'
-	return list(struct.unpack(fmt, data))
-
-
-def bytes_to_int32_list(data: bytes, swap_endianness=False) -> List[int]:
-	"""Converts bytes to list of integer32 - one number is represented by 4 bytes."""
-	fmt = f'{_get_endianness_symbol(swap_endianness)}{len(data) // 4}i'
-	return list(struct.unpack(fmt, data))
-
-
-def bytes_to_int16_list(data: bytes, swap_endianness=False) -> List[int]:
-	"""Converts bytes to list of integer16 - one number is represented by 2 bytes."""
-	fmt = f'{_get_endianness_symbol(swap_endianness)}{len(data) // 2}h'
-	return list(struct.unpack(fmt, data))
-
-
-def bytes_to_list_of_floats(data: bytes, fmt: BinFloatFormat) -> List[float]:
-	"""Decodes binary data to a list of floating-point numbers based on the entered format."""
-	if fmt == BinFloatFormat.Single_4bytes:
-		return bytes_to_float32_list(data)
-	elif fmt == BinFloatFormat.Single_4bytes_swapped:
-		return bytes_to_float32_list(data, True)
-	elif fmt == BinFloatFormat.Double_8bytes:
-		return bytes_to_double64_list(data)
-	elif fmt == BinFloatFormat.Double_8bytes_swapped:
-		return bytes_to_double64_list(data, True)
-
-
-def bytes_to_list_of_integers(data: bytes, fmt: BinIntFormat) -> List[int]:
-	"""Decodes binary data to a list of integer numbers based on the entered format."""
-	if fmt == BinIntFormat.Integer32_4bytes:
-		return bytes_to_int32_list(data)
-	elif fmt == BinIntFormat.Integer32_4bytes_swapped:
-		return bytes_to_int32_list(data, True)
-	elif fmt == BinIntFormat.Integer16_2bytes:
-		return bytes_to_int16_list(data)
-	elif fmt == BinIntFormat.Integer16_2bytes_swapped:
-		return bytes_to_int16_list(data, True)
-
-
-def double64_list_to_bytes(data: List[float], swap_endianness=False) -> bytes:
-	"""Converts list of doubles to bytes - one number is converted to 8 bytes."""
-	fmt = f'{_get_endianness_symbol(swap_endianness)}{str(len(data))}d'
-	return struct.pack(fmt, *data)
-
-
-def float32_list_to_bytes(data: List[float], swap_endianness=False) -> bytes:
-	"""Converts list of floats to bytes - one number is converted to 4 bytes."""
-	fmt = f'{_get_endianness_symbol(swap_endianness)}{str(len(data))}f'
-	return struct.pack(fmt, *data)
-
-
-def int32_list_to_bytes(data: List[int], swap_endianness=False) -> bytes:
-	"""Converts list of integers 32 to bytes - one number is converted to 4 bytes."""
-	fmt = f'{_get_endianness_symbol(swap_endianness)}{str(len(data))}i'
-	return struct.pack(fmt, *data)
-
-
-def int16_list_to_bytes(data: List[float], swap_endianness=False) -> bytes:
-	"""Converts list of integers 16 to bytes - one number is converted to 2 bytes."""
-	fmt = f'{_get_endianness_symbol(swap_endianness)}{str(len(data))}h'
-	return struct.pack(fmt, *data)
-
-
-def list_of_integers_to_bytes(ints: List[int], fmt: BinIntFormat) -> bytes:
-	"""Encodes list of integers to binary data based on the entered format."""
-	if fmt == BinIntFormat.Integer32_4bytes:
-		return int32_list_to_bytes(ints)
-	elif fmt == BinIntFormat.Integer32_4bytes_swapped:
-		return int32_list_to_bytes(ints, True)
-	elif fmt == BinIntFormat.Integer16_2bytes:
-		return int16_list_to_bytes(ints)
-	elif fmt == BinIntFormat.Integer16_2bytes_swapped:
-		return int16_list_to_bytes(ints, True)
-
-
-def list_of_floats_to_bytes(floats: List[float], fmt: BinFloatFormat) -> bytes:
-	"""Encodes list of floats to binary data based on the entered format."""
-	if fmt == BinFloatFormat.Single_4bytes:
-		return float32_list_to_bytes(floats)
-	elif fmt == BinFloatFormat.Single_4bytes_swapped:
-		return float32_list_to_bytes(floats, True)
-	elif fmt == BinFloatFormat.Double_8bytes:
-		return double64_list_to_bytes(floats)
-	elif fmt == BinFloatFormat.Double_8bytes_swapped:
-		return double64_list_to_bytes(floats, True)
-
-
-pure_bool_true_lookup = frozenset(['on', 'On', 'ON', 'true', 'True', 'TRUE'])
-bool_true_lookup = frozenset(['1', 'on', 'On', 'ON', 'true', 'True', 'TRUE'])
-bool_false_lookup = frozenset(['0', 'off', 'Off', 'OFF', 'false', 'False', 'FALSE'])
-pure_bool_false_lookup = frozenset(['off', 'Off', 'OFF', 'false', 'False', 'FALSE'])
-
-
-def str_to_bool(string: str) -> bool:
-	"""Converts string to boolean value.
-	The function robust, and case insensitive.
-	If the string can not be converted to a boolean, the function returns False."""
-	assert_string_data(string)
-	if string in bool_true_lookup:
-		return True
-	if string in bool_false_lookup:
-		return False
-	# If leading/trailing spaces
-	string = string.strip()
-	if string in bool_true_lookup:
-		return True
-	if string in bool_false_lookup:
-		return False
-	# If enclosed by brackets
-	string = Utilities.trim_str_response(string)
-	if string in bool_true_lookup:
-		return True
-	if string in bool_false_lookup:
-		return False
-	return False
-
-
-def string_to_pure_bool(string: str) -> bool or None:
-	"""Converts string to boolean value. Compare to str_to_bool(), the values '1' and '0' are not considered boolean.
-	Also, if the method can not convert the string to boolean, it returns None."""
-	assert_string_data(string)
-	if string in pure_bool_true_lookup:
-		return True
-	if string in pure_bool_false_lookup:
-		return False
-	# If leading/trailing spaces
-	string = string.strip()
-	if string in pure_bool_true_lookup:
-		return True
-	if string in pure_bool_false_lookup:
-		return False
-	# If enclosed by brackets
-	string = Utilities.trim_str_response(string)
-	if string in pure_bool_true_lookup:
-		return True
-	if string in pure_bool_false_lookup:
-		return False
-	return None
-
-
-number_plus_inf_lookup = frozenset(['Inf', 'INF', 'INFINITY', '+Inf', '+INF', '+inf', '+INFINITY', '+Infinity', '+infinity'])
-number_minus_inf_lookup = frozenset(['-Inf', '-INF', '-inf', '-INFINITY', '-Infinity', '-infinity'])
-number_nan_lookup = frozenset(['Nan', 'NAN', 'nan', 'NaN', 'NAV', 'NaV', 'NCAP', 'INV', 'NONE', 'none', 'None', 'DTX', 'UND', 'und'])
-number_max_lookup = frozenset(['OFL', 'ofl', 'Ofl'])
-number_min_lookup = frozenset(['UFL', 'ufl', 'Ufl'])
-int_neg_inf = -(sys.maxsize - 1)
-enum_spec_prefixes = {'_minus': '-', '_plus': '+', '_': ''}
-enum_spec_strings = {'_dash_': '-', '_dot_': '.'}
-
-
-def str_to_int(string: str) -> int:
-	"""Converts string to integer value. Float values are coerced to integer.
-	Also recognizes case insensitive special values like NaN, INV, NCAP..."""
-	assert_string_data(string)
-	string = string.strip()
-	if string == '':
-		return 0
-	value = str_special_values_to_int(string)
-	if value:
-		return value
-
-	# Hexadecimal numbers
-	if string.startswith('#H') or string.startswith('0x'):
-		if ',' in string:
-			return int(string[2:string.find(',')], 16)
-		else:
-			return int(string[2:], 16)
-
-	# Binary numbers
-	if string.startswith('#B') or string.startswith('0b'):
-		if ',' in string:
-			return int(string[2:string.find(',')], 2)
-		else:
-			return int(string[2:], 2)
-
-	# Octal numbers
-	if string.startswith('#Q') or string.startswith('0o'):
-		if ',' in string:
-			return int(string[2:string.find(',')], 8)
-		else:
-			return int(string[2:], 8)
-	# Simulation
-	if string == 'Simulating':
-		return 0
-	return int(round(float(string)))
-
-
-def str_special_values_to_int(string: str) -> int:
-	"""Converts special string values to integer. Returns None if no special value was found."""
-	assert_string_data(string)
-	if string in number_plus_inf_lookup or string in number_max_lookup:
-		return sys.maxsize
-	if string in number_minus_inf_lookup or string in number_min_lookup or string in number_nan_lookup:
-		return int_neg_inf
-	if string == 'OFF':
-		return int_neg_inf + 1
-	if string == 'ON':
-		return int_neg_inf + 2
-	if string == 'OK':
-		return sys.maxsize - 1
-	if string == 'DC':
-		# noinspection PyTypeChecker
-		return int_neg_inf / 100
-	if string == 'ULEU':
-		return int(sys.maxsize / 10)
-	if string == 'ULEL':
-		# noinspection PyTypeChecker
-		return int_neg_inf / 10
-	# noinspection PyTypeChecker
-	return None
-
-
-def str_to_int_or_bool(string: str) -> int or bool:
-	"""Similar to str_to_int, but for special values "ON/OFF" the function returns boolean"""
-	result = string_to_pure_bool(string)
-	if result is not None:
-		return result
-	return str_to_int(string)
-
-
-def str_to_float(string: str) -> float:
-	"""Converts string to float value.
-	Also recognizes case insensitive special values like NaN, INV, NCAP..."""
-	assert_string_data(string)
-	string = string.strip()
-	if string == '':
-		return 0.0
-	if string in number_plus_inf_lookup:
-		return math.inf
-	if string in number_minus_inf_lookup:
-		return -math.inf
-	if string in number_nan_lookup:
-		return math.nan
-	if string in number_max_lookup:
-		return sys.float_info.max
-	if string in number_min_lookup:
-		return -sys.float_info.max
-	if string == 'OFF':
-		return -sys.float_info.epsilon
-	if string == 'ON':
-		return -2*sys.float_info.epsilon
-	if string == 'OK':
-		return sys.float_info.epsilon
-	if string == 'DC' or string == '':
-		return -sys.float_info.max / 100
-	if string == 'ULEU':
-		return sys.float_info.max / 10
-	if string == 'ULEL':
-		return -sys.float_info.max / 10
-	if string == 'Simulating':
-		return 0.0
-	return float(string)
-
-
-def str_to_float_or_bool(string: str) -> float or bool:
-	"""Similar to str_to_float, but for special values "ON/OFF" the function returns boolean"""
-	result = string_to_pure_bool(string)
-	if result is not None:
-		return result
-	return str_to_float(string)
-
-
-def float_to_str(value: float) -> str:
-	"""Converts double number to string using {.12g} formatter."""
-	return format(value, ".12g")
-
-
-def bool_to_str(value: bool) -> str:
-	"""Converts boolean to 'ON' or 'OFF' string."""
-	if type(value) is bool:
-		return 'ON' if value is True else 'OFF'
-	else:
-		raise Exception(f"bool_to_str: unsupported variable type '{type(value)}', value '{value}'. Only boolean values are supported.")
-
-
-def str_enclose_by_quotes(string: str) -> str:
-	"""Returns string enclosed by single quotes."""
-	assert_string_data(string)
-	return "'" + string + "'"
-
-
-def list_to_csv_str(value: list) -> str:
-	"""Converts list of elements to strings separated by commas.
-	Element types can differ on an individual basis.
-	Supported element types:
-	- int
-	- bool
-	- float
-	- string -> string no quotes
-	- enum"""
-	assert_list_data(value)
-	result = []
-	for x in value:
-		el = value_to_str(x)
-		if not el:
-			raise TypeError(f"List element type is not supported by Conversions.list_to_csv_str: '{x}'")
-		result.append(el)
-	return ','.join(result)
-
-
-def list_to_csv_quoted_str(value: list) -> str:
-	"""Converts list of elements to quoted strings separated by commas.
-	Only string elements are enclosed by single quotes
-	Element types can differ on an individual basis.
-	Supported element types:
-	- int
-	- bool
-	- float
-	- string -> string enclosed by quotes
-	- enum"""
-	assert_list_data(value)
-	result = []
-	for x in value:
-		if isinstance(x, str):
-			el = str_enclose_by_quotes(x)
-		else:
-			el = value_to_str(x)
-		if not el:
-			raise TypeError(f"List element type is not supported by Conversions.list_to_csv_quoted_str: '{x}'")
-		result.append(el)
-
-	return ','.join(result)
-
-
-def decimal_value_to_str(x: int or float) -> str:
-	"""Converts scalar decimal value to string.
-	Supported element types:
-	- int
-	- float"""
-	if isinstance(x, int) and type(x) is not bool:
-		return str(x)
-	elif isinstance(x, float):
-		return float_to_str(x)
-	else:
-		raise Exception(f"decimal_value_to_str: unsupported variable type '{type(x)}', value '{x}'. Only integer and float types are supported.")
-
-
-def decimal_or_bool_value_to_str(x: int or float or bool) -> str:
-	"""Converts scalar decimal value to string.
-	Supported element types:
-	- int
-	- float
-	- boolean"""
-	if type(x) is bool:
-		return bool_to_str(x)
-	if isinstance(x, int):
-		return str(x)
-	elif isinstance(x, float):
-		return float_to_str(x)
-	else:
-		raise Exception(f"decimal_or_bool_value_to_str: unsupported variable type '{type(x)}', value '{x}'. Only integer, float and boolean types are supported.")
-
-
-def value_to_str(x: int or bool or float or str or Enum) -> str:
-	"""Converts scalar value to string.
-	Supported element types:
-	- int
-	- bool
-	- float
-	- string
-	- enum"""
-	if isinstance(x, bool):
-		return bool_to_str(x)
-	elif isinstance(x, int):
-		return str(x)
-	elif isinstance(x, float):
-		return float_to_str(x)
-	elif isinstance(x, str):
-		return x
-	elif isinstance(x, Enum):
-		return enum_value_to_scpi_string(x.name)
-	else:
-		raise Exception(f"value_to_str: unsupported variable type '{type(x)}', value '{x}'. Supported types: int, bool, float, str, enum.")
-
-
-def enum_value_to_scpi_string(enum_value: str) -> str:
-	"""Conversion EnumValue -> SCPI_String
-	Unescapes all the special characters that can not be contained in the enum member definition, but can be sent to the instrument as enum string.
-	Use this to send the scpi enum value to the instrument."""
-	for key in enum_spec_prefixes:
-		if enum_value.startswith(key):
-			enum_value = enum_spec_prefixes[key] + enum_value[len(key):]
-	for key in enum_spec_strings:
-		enum_value = enum_value.replace(key, enum_spec_strings[key])
-	return enum_value
-
-
-def value_to_quoted_str(x: int or bool or float or str or Enum) -> str:
-	"""Converts scalar value to string enclosed by single quotes.
-	Supported element types:
-	- int
-	- bool
-	- float
-	- string
-	- enum"""
-	return f"'{value_to_str(x)}'"
-
-
-def str_to_float_list(string: str) -> List[float]:
-	"""Converts string with comma-separated values to list of Floats."""
-	assert_string_data(string)
-	if not string:
-		return []
-	result = [*map(str_to_float, string.split(','))]
-	return result
-
-
-def str_to_float_or_bool_list(string: str) -> List[float or bool]:
-	"""Converts string with comma-separated values to list of float or boolean values."""
-	assert_string_data(string)
-	if not string:
-		return []
-	result = [*map(str_to_float_or_bool, string.split(','))]
-	return result
-
-
-def str_to_int_list(string: str) -> List[int]:
-	"""Converts string with comma-separated values to list of Integers."""
-	assert_string_data(string)
-	if not string:
-		return []
-	result = [*map(str_to_int, string.split(','))]
-	return result
-
-
-def str_to_int_or_bool_list(string: str) -> List[int or bool]:
-	"""Converts string with comma-separated values to list of integer or boolean values."""
-	assert_string_data(string)
-	if not string:
-		return []
-	result = [*map(str_to_int_or_bool, string.split(','))]
-	return result
-
-
-def str_to_bool_list(string: str) -> List[bool]:
-	"""Converts string with comma-separated values to list of booleans."""
-	assert_string_data(string)
-	if not string:
-		return []
-	result = [*map(str_to_bool, string.split(','))]
-	return result
-
-
-def str_to_str_list(string: str, clear_one_empty_item: bool = False) -> List[str]:
-	"""Converts string with comma-separated values to list of strings.
-	Each element is trimmed by trim_str_response().
-	If the clear_one_empty_item is set to True (default is False), and the result is exactly one empty string item, the method returns empty list."""
-	assert_string_data(string)
-	if not string:
-		return []
-	result = [*map(Utilities.trim_str_response, string.split(','))]
-	if clear_one_empty_item and len(result) == 1 and result[0] == '':
-		return []
-	return result
-
-
-def _find_in_enum_members(item: str, enum_members: List[str]) -> int:
-	"""Matches a string in the provided list of member strings.
-	The item must be not fully matched.
-	The item is matched if a member string starts with the item (the item is a prefix of the member).
-	Example: item='CONN' will match the enum_member 'CONNected'
-	If the item contains a comma, only the value before comma is considered
-	Returns found index in the enum_members list"""
-	if ',' in item:
-		item = item[:item.index(',')].strip()
-	ix = -1
-	i = 0
-	for x in enum_members:
-		if x.startswith(item):
-			return i
-		i += 1
-	return ix
-
-
-def str_to_scalar_enum_helper(string: str, enum_type: Enum, enum_members=None) -> Enum:
-	"""Converts string to one enum element.
-	enum_members are optional to improve the performance for repeated conversions.
-	If you do not provide them, they are generated inside the function."""
-	value = Utilities.trim_str_response(string)
-	if not enum_members:
-		# noinspection PyTypeChecker
-		enum_members = [x.name for x in enum_type]
-
-	# Search in the enum member and return the index of the matched item
-	ix = _find_in_enum_members(value, enum_members)
-	if ix >= 0:
-		return enum_type[enum_members[ix]]
-
-	# If the result is -1 (not found), try to replace the special values and search again
-	# This is done to improve the performance, since most of the enums have no special values
-	enum_members_conv = [enum_value_to_scpi_string(x) for x in enum_members]
-	ix = _find_in_enum_members(value, enum_members_conv)
-	if ix >= 0:
-		return enum_type[enum_members[ix]]
-
-	# If not found, search in the special integer numbers:
-	spec_value = str_special_values_to_int(value)
-	if not spec_value:
-		raise Exception(f"String '{value}' can not be found in the enum type '{enum_type}'")
-	# noinspection PyTypeChecker
-	return spec_value
-
-
-def str_to_list_enum_helper(string: str, enum_type: Enum, enum_members=None) -> List[Enum]:
-	"""Converts string to list of enum elements.
-	enum_members are optional to improve the performance for repeated conversions.
-	If you do not provide them, they are generated inside the function."""
-	if not enum_members:
-		# noinspection PyTypeChecker
-		enum_members = [x.name for x in enum_type]
-	elements = string.split(',')
-	return [str_to_scalar_enum_helper(x, enum_type, enum_members) for x in elements]
-
-
-def enum_scalar_to_str(data, enum_type) -> str:
-	"""Converts enum scalar value to string."""
-	assert isinstance(data, enum_type), f"Expected command parameter {enum_type}, actual data type: {type(data)}. Value: {data}"
-	return value_to_str(data)
-
-
-def enum_list_to_str(data: List, enum_type) -> str:
-	"""Converts enum list to csv-string."""
-	# For enums, check that each element is an enum
-	assert all(isinstance(x, enum_type) for x in data), f"Expected command parameter list of {enum_type}, detected one or more elements of non-enum type. Value: {data}"
-	return list_to_csv_str(data)
-
-
-def str_to_scalar_enum(string: str, enum_type) -> Enum:
-	"""Converts string to one enum element."""
-	return str_to_scalar_enum_helper(string, enum_type)
-
-
-def str_to_list_enum(string: str, enum_type) -> List[Enum]:
-	"""Converts string to list of enum elements."""
-	return str_to_list_enum_helper(string, enum_type)
+import math
+import struct
+import sys
+from enum import Enum
+from typing import List
+
+from . import Utilities
+
+
+class BinFloatFormat(Enum):
+	"""Binary format of a float number."""
+	Single_4bytes = 1
+	Single_4bytes_swapped = 2
+	Double_8bytes = 3
+	Double_8bytes_swapped = 4
+
+
+class BinIntFormat(Enum):
+	"""Binary format of an integer number."""
+	Integer32_4bytes = 1
+	Integer32_4bytes_swapped = 2
+	Integer16_2bytes = 3
+	Integer16_2bytes_swapped = 4
+
+
+def assert_string_data(value: str) -> None:
+	"""Asserts value is string type."""
+	assert isinstance(value, str), f"Input value type must be string. Actual type: {type(value)}, value: {value}"
+
+
+def assert_list_data(value: list) -> None:
+	"""Asserts value is list type."""
+	assert isinstance(value, list), f"Input value type must be a list. Actual type: {type(value)}, value: {value}"
+
+
+def _get_endianness_symbol(swap_endianness: bool) -> str:
+	"""Based on the current endianness returns the symbol used in the 'struct' module."""
+	if swap_endianness is False:
+		return '@'
+	elif swap_endianness is True and sys.byteorder == 'little':
+		return '>'
+	else:
+		return '<'
+
+
+def bytes_to_float32_list(data: bytes, swap_endianness=False) -> List[float]:
+	"""Converts bytes to list of floats - one number is represented by 4 bytes."""
+	fmt = f'{_get_endianness_symbol(swap_endianness)}{len(data) // 4}f'
+	return list(struct.unpack(fmt, data))
+
+
+def bytes_to_double64_list(data: bytes, swap_endianness=False) -> List[float]:
+	"""Converts bytes to list of doubles - one number is represented by 8 bytes."""
+	fmt = f'{_get_endianness_symbol(swap_endianness)}{len(data) // 8}d'
+	return list(struct.unpack(fmt, data))
+
+
+def bytes_to_int32_list(data: bytes, swap_endianness=False) -> List[int]:
+	"""Converts bytes to list of integer32 - one number is represented by 4 bytes."""
+	fmt = f'{_get_endianness_symbol(swap_endianness)}{len(data) // 4}i'
+	return list(struct.unpack(fmt, data))
+
+
+def bytes_to_int16_list(data: bytes, swap_endianness=False) -> List[int]:
+	"""Converts bytes to list of integer16 - one number is represented by 2 bytes."""
+	fmt = f'{_get_endianness_symbol(swap_endianness)}{len(data) // 2}h'
+	return list(struct.unpack(fmt, data))
+
+
+def bytes_to_list_of_floats(data: bytes, fmt: BinFloatFormat) -> List[float]:
+	"""Decodes binary data to a list of floating-point numbers based on the entered format."""
+	if fmt == BinFloatFormat.Single_4bytes:
+		return bytes_to_float32_list(data)
+	elif fmt == BinFloatFormat.Single_4bytes_swapped:
+		return bytes_to_float32_list(data, True)
+	elif fmt == BinFloatFormat.Double_8bytes:
+		return bytes_to_double64_list(data)
+	elif fmt == BinFloatFormat.Double_8bytes_swapped:
+		return bytes_to_double64_list(data, True)
+
+
+def bytes_to_list_of_integers(data: bytes, fmt: BinIntFormat) -> List[int]:
+	"""Decodes binary data to a list of integer numbers based on the entered format."""
+	if fmt == BinIntFormat.Integer32_4bytes:
+		return bytes_to_int32_list(data)
+	elif fmt == BinIntFormat.Integer32_4bytes_swapped:
+		return bytes_to_int32_list(data, True)
+	elif fmt == BinIntFormat.Integer16_2bytes:
+		return bytes_to_int16_list(data)
+	elif fmt == BinIntFormat.Integer16_2bytes_swapped:
+		return bytes_to_int16_list(data, True)
+
+
+def double64_list_to_bytes(data: List[float], swap_endianness=False) -> bytes:
+	"""Converts list of doubles to bytes - one number is converted to 8 bytes."""
+	fmt = f'{_get_endianness_symbol(swap_endianness)}{str(len(data))}d'
+	return struct.pack(fmt, *data)
+
+
+def float32_list_to_bytes(data: List[float], swap_endianness=False) -> bytes:
+	"""Converts list of floats to bytes - one number is converted to 4 bytes."""
+	fmt = f'{_get_endianness_symbol(swap_endianness)}{str(len(data))}f'
+	return struct.pack(fmt, *data)
+
+
+def int32_list_to_bytes(data: List[int], swap_endianness=False) -> bytes:
+	"""Converts list of integers 32 to bytes - one number is converted to 4 bytes."""
+	fmt = f'{_get_endianness_symbol(swap_endianness)}{str(len(data))}i'
+	return struct.pack(fmt, *data)
+
+
+def int16_list_to_bytes(data: List[float], swap_endianness=False) -> bytes:
+	"""Converts list of integers 16 to bytes - one number is converted to 2 bytes."""
+	fmt = f'{_get_endianness_symbol(swap_endianness)}{str(len(data))}h'
+	return struct.pack(fmt, *data)
+
+
+def list_of_integers_to_bytes(ints: List[int], fmt: BinIntFormat) -> bytes:
+	"""Encodes list of integers to binary data based on the entered format."""
+	if fmt == BinIntFormat.Integer32_4bytes:
+		return int32_list_to_bytes(ints)
+	elif fmt == BinIntFormat.Integer32_4bytes_swapped:
+		return int32_list_to_bytes(ints, True)
+	elif fmt == BinIntFormat.Integer16_2bytes:
+		return int16_list_to_bytes(ints)
+	elif fmt == BinIntFormat.Integer16_2bytes_swapped:
+		return int16_list_to_bytes(ints, True)
+
+
+def list_of_floats_to_bytes(floats: List[float], fmt: BinFloatFormat) -> bytes:
+	"""Encodes list of floats to binary data based on the entered format."""
+	if fmt == BinFloatFormat.Single_4bytes:
+		return float32_list_to_bytes(floats)
+	elif fmt == BinFloatFormat.Single_4bytes_swapped:
+		return float32_list_to_bytes(floats, True)
+	elif fmt == BinFloatFormat.Double_8bytes:
+		return double64_list_to_bytes(floats)
+	elif fmt == BinFloatFormat.Double_8bytes_swapped:
+		return double64_list_to_bytes(floats, True)
+
+
+pure_bool_true_lookup = frozenset(['on', 'On', 'ON', 'true', 'True', 'TRUE'])
+bool_true_lookup = frozenset(['1', 'on', 'On', 'ON', 'true', 'True', 'TRUE'])
+bool_false_lookup = frozenset(['0', 'off', 'Off', 'OFF', 'false', 'False', 'FALSE'])
+pure_bool_false_lookup = frozenset(['off', 'Off', 'OFF', 'false', 'False', 'FALSE'])
+
+
+def str_to_bool(string: str) -> bool:
+	"""Converts string to boolean value.
+	The function robust, and case insensitive.
+	If the string can not be converted to a boolean, the function returns False."""
+	assert_string_data(string)
+	if string in bool_true_lookup:
+		return True
+	if string in bool_false_lookup:
+		return False
+	# If leading/trailing spaces
+	string = string.strip()
+	if string in bool_true_lookup:
+		return True
+	if string in bool_false_lookup:
+		return False
+	# If enclosed by brackets
+	string = Utilities.trim_str_response(string)
+	if string in bool_true_lookup:
+		return True
+	if string in bool_false_lookup:
+		return False
+	return False
+
+
+def string_to_pure_bool(string: str) -> bool or None:
+	"""Converts string to boolean value. Compare to str_to_bool(), the values '1' and '0' are not considered boolean.
+	Also, if the method can not convert the string to boolean, it returns None."""
+	assert_string_data(string)
+	if string in pure_bool_true_lookup:
+		return True
+	if string in pure_bool_false_lookup:
+		return False
+	# If leading/trailing spaces
+	string = string.strip()
+	if string in pure_bool_true_lookup:
+		return True
+	if string in pure_bool_false_lookup:
+		return False
+	# If enclosed by brackets
+	string = Utilities.trim_str_response(string)
+	if string in pure_bool_true_lookup:
+		return True
+	if string in pure_bool_false_lookup:
+		return False
+	return None
+
+
+number_plus_inf_lookup = frozenset(['Inf', 'INF', 'INFINITY', '+Inf', '+INF', '+inf', '+INFINITY', '+Infinity', '+infinity'])
+number_minus_inf_lookup = frozenset(['-Inf', '-INF', '-inf', '-INFINITY', '-Infinity', '-infinity'])
+number_nan_lookup = frozenset(['Nan', 'NAN', 'nan', 'NaN', 'NAV', 'NaV', 'NCAP', 'INV', 'NONE', 'none', 'None', 'DTX', 'UND', 'und'])
+number_max_lookup = frozenset(['OFL', 'ofl', 'Ofl'])
+number_min_lookup = frozenset(['UFL', 'ufl', 'Ufl'])
+int_neg_inf = -(sys.maxsize - 1)
+enum_spec_prefixes = {'_minus': '-', '_plus': '+', '_': ''}
+enum_spec_strings = {'_dash_': '-', '_dot_': '.'}
+
+
+def str_to_int(string: str) -> int:
+	"""Converts string to integer value. Float values are coerced to integer.
+	Also recognizes case insensitive special values like NaN, INV, NCAP..."""
+	assert_string_data(string)
+	string = string.strip()
+	if string == '':
+		return 0
+	value = str_special_values_to_int(string)
+	if value:
+		return value
+
+	# Hexadecimal numbers
+	if string.startswith('#H') or string.startswith('0x'):
+		if ',' in string:
+			return int(string[2:string.find(',')], 16)
+		else:
+			return int(string[2:], 16)
+
+	# Binary numbers
+	if string.startswith('#B') or string.startswith('0b'):
+		if ',' in string:
+			return int(string[2:string.find(',')], 2)
+		else:
+			return int(string[2:], 2)
+
+	# Octal numbers
+	if string.startswith('#Q') or string.startswith('0o'):
+		if ',' in string:
+			return int(string[2:string.find(',')], 8)
+		else:
+			return int(string[2:], 8)
+	# Simulation
+	if string == 'Simulating':
+		return 0
+	return int(round(float(string)))
+
+
+def str_special_values_to_int(string: str) -> int:
+	"""Converts special string values to integer. Returns None if no special value was found."""
+	assert_string_data(string)
+	if string in number_plus_inf_lookup or string in number_max_lookup:
+		return sys.maxsize
+	if string in number_minus_inf_lookup or string in number_min_lookup or string in number_nan_lookup:
+		return int_neg_inf
+	if string == 'OFF':
+		return int_neg_inf + 1
+	if string == 'ON':
+		return int_neg_inf + 2
+	if string == 'OK':
+		return sys.maxsize - 1
+	if string == 'DC':
+		# noinspection PyTypeChecker
+		return int_neg_inf / 100
+	if string == 'ULEU':
+		return int(sys.maxsize / 10)
+	if string == 'ULEL':
+		# noinspection PyTypeChecker
+		return int_neg_inf / 10
+	# noinspection PyTypeChecker
+	return None
+
+
+def str_to_int_or_bool(string: str) -> int or bool:
+	"""Similar to str_to_int, but for special values "ON/OFF" the function returns boolean"""
+	result = string_to_pure_bool(string)
+	if result is not None:
+		return result
+	return str_to_int(string)
+
+
+def str_to_float(string: str) -> float:
+	"""Converts string to float value.
+	Also recognizes case insensitive special values like NaN, INV, NCAP..."""
+	assert_string_data(string)
+	string = string.strip()
+	if string == '':
+		return 0.0
+	if string in number_plus_inf_lookup:
+		return math.inf
+	if string in number_minus_inf_lookup:
+		return -math.inf
+	if string in number_nan_lookup:
+		return math.nan
+	if string in number_max_lookup:
+		return sys.float_info.max
+	if string in number_min_lookup:
+		return -sys.float_info.max
+	if string == 'OFF':
+		return -sys.float_info.epsilon
+	if string == 'ON':
+		return -2*sys.float_info.epsilon
+	if string == 'OK':
+		return sys.float_info.epsilon
+	if string == 'DC' or string == '':
+		return -sys.float_info.max / 100
+	if string == 'ULEU':
+		return sys.float_info.max / 10
+	if string == 'ULEL':
+		return -sys.float_info.max / 10
+	if string == 'Simulating':
+		return 0.0
+	return float(string)
+
+
+def str_to_float_or_bool(string: str) -> float or bool:
+	"""Similar to str_to_float, but for special values "ON/OFF" the function returns boolean"""
+	result = string_to_pure_bool(string)
+	if result is not None:
+		return result
+	return str_to_float(string)
+
+
+def float_to_str(value: float) -> str:
+	"""Converts double number to string using {.12g} formatter."""
+	return format(value, ".12g")
+
+
+def bool_to_str(value: bool) -> str:
+	"""Converts boolean to 'ON' or 'OFF' string."""
+	if type(value) is bool:
+		return 'ON' if value is True else 'OFF'
+	else:
+		raise Exception(f"bool_to_str: unsupported variable type '{type(value)}', value '{value}'. Only boolean values are supported.")
+
+
+def str_enclose_by_quotes(string: str) -> str:
+	"""Returns string enclosed by single quotes."""
+	assert_string_data(string)
+	return "'" + string + "'"
+
+
+def list_to_csv_str(value: list) -> str:
+	"""Converts list of elements to strings separated by commas.
+	Element types can differ on an individual basis.
+	Supported element types:
+	- int
+	- bool
+	- float
+	- string -> string no quotes
+	- enum"""
+	assert_list_data(value)
+	result = []
+	for x in value:
+		el = value_to_str(x)
+		if not el:
+			raise TypeError(f"List element type is not supported by Conversions.list_to_csv_str: '{x}'")
+		result.append(el)
+	return ','.join(result)
+
+
+def list_to_csv_quoted_str(value: list) -> str:
+	"""Converts list of elements to quoted strings separated by commas.
+	Only string elements are enclosed by single quotes
+	Element types can differ on an individual basis.
+	Supported element types:
+	- int
+	- bool
+	- float
+	- string -> string enclosed by quotes
+	- enum"""
+	assert_list_data(value)
+	result = []
+	for x in value:
+		if isinstance(x, str):
+			el = str_enclose_by_quotes(x)
+		else:
+			el = value_to_str(x)
+		if not el:
+			raise TypeError(f"List element type is not supported by Conversions.list_to_csv_quoted_str: '{x}'")
+		result.append(el)
+
+	return ','.join(result)
+
+
+def decimal_value_to_str(x: int or float) -> str:
+	"""Converts scalar decimal value to string.
+	Supported element types:
+	- int
+	- float"""
+	if isinstance(x, int) and type(x) is not bool:
+		return str(x)
+	elif isinstance(x, float):
+		return float_to_str(x)
+	else:
+		raise Exception(f"decimal_value_to_str: unsupported variable type '{type(x)}', value '{x}'. Only integer and float types are supported.")
+
+
+def decimal_or_bool_value_to_str(x: int or float or bool) -> str:
+	"""Converts scalar decimal value to string.
+	Supported element types:
+	- int
+	- float
+	- boolean"""
+	if type(x) is bool:
+		return bool_to_str(x)
+	if isinstance(x, int):
+		return str(x)
+	elif isinstance(x, float):
+		return float_to_str(x)
+	else:
+		raise Exception(f"decimal_or_bool_value_to_str: unsupported variable type '{type(x)}', value '{x}'. Only integer, float and boolean types are supported.")
+
+
+def value_to_str(x: int or bool or float or str or Enum) -> str:
+	"""Converts scalar value to string.
+	Supported element types:
+	- int
+	- bool
+	- float
+	- string
+	- enum"""
+	if isinstance(x, bool):
+		return bool_to_str(x)
+	elif isinstance(x, int):
+		return str(x)
+	elif isinstance(x, float):
+		return float_to_str(x)
+	elif isinstance(x, str):
+		return x
+	elif isinstance(x, Enum):
+		return enum_value_to_scpi_string(x.name)
+	else:
+		raise Exception(f"value_to_str: unsupported variable type '{type(x)}', value '{x}'. Supported types: int, bool, float, str, enum.")
+
+
+def enum_value_to_scpi_string(enum_value: str) -> str:
+	"""Conversion EnumValue -> SCPI_String
+	Unescapes all the special characters that can not be contained in the enum member definition, but can be sent to the instrument as enum string.
+	Use this to send the scpi enum value to the instrument."""
+	for key in enum_spec_prefixes:
+		if enum_value.startswith(key):
+			enum_value = enum_spec_prefixes[key] + enum_value[len(key):]
+	for key in enum_spec_strings:
+		enum_value = enum_value.replace(key, enum_spec_strings[key])
+	return enum_value
+
+
+def value_to_quoted_str(x: int or bool or float or str or Enum) -> str:
+	"""Converts scalar value to string enclosed by single quotes.
+	Supported element types:
+	- int
+	- bool
+	- float
+	- string
+	- enum"""
+	return f"'{value_to_str(x)}'"
+
+
+def str_to_float_list(string: str) -> List[float]:
+	"""Converts string with comma-separated values to list of Floats."""
+	assert_string_data(string)
+	if not string:
+		return []
+	result = [*map(str_to_float, string.split(','))]
+	return result
+
+
+def str_to_float_or_bool_list(string: str) -> List[float or bool]:
+	"""Converts string with comma-separated values to list of float or boolean values."""
+	assert_string_data(string)
+	if not string:
+		return []
+	result = [*map(str_to_float_or_bool, string.split(','))]
+	return result
+
+
+def str_to_int_list(string: str) -> List[int]:
+	"""Converts string with comma-separated values to list of Integers."""
+	assert_string_data(string)
+	if not string:
+		return []
+	result = [*map(str_to_int, string.split(','))]
+	return result
+
+
+def str_to_int_or_bool_list(string: str) -> List[int or bool]:
+	"""Converts string with comma-separated values to list of integer or boolean values."""
+	assert_string_data(string)
+	if not string:
+		return []
+	result = [*map(str_to_int_or_bool, string.split(','))]
+	return result
+
+
+def str_to_bool_list(string: str) -> List[bool]:
+	"""Converts string with comma-separated values to list of booleans."""
+	assert_string_data(string)
+	if not string:
+		return []
+	result = [*map(str_to_bool, string.split(','))]
+	return result
+
+
+def str_to_str_list(string: str, clear_one_empty_item: bool = False) -> List[str]:
+	"""Converts string with comma-separated values to list of strings.
+	Each element is trimmed by trim_str_response().
+	If the clear_one_empty_item is set to True (default is False), and the result is exactly one empty string item, the method returns empty list."""
+	assert_string_data(string)
+	if not string:
+		return []
+	result = [*map(Utilities.trim_str_response, string.split(','))]
+	if clear_one_empty_item and len(result) == 1 and result[0] == '':
+		return []
+	return result
+
+
+def _find_in_enum_members(item: str, enum_members: List[str]) -> int:
+	"""Matches a string in the provided list of member strings.
+	The item must be not fully matched.
+	The item is matched if a member string starts with the item (the item is a prefix of the member).
+	Example: item='CONN' will match the enum_member 'CONNected'
+	If the item contains a comma, only the value before comma is considered
+	Returns found index in the enum_members list"""
+	if ',' in item:
+		item = item[:item.index(',')].strip()
+	i = 0
+	for x in enum_members:
+		if x.startswith(item):
+			return i
+		i += 1
+
+	# smart matching:
+	# item = 'MAX' matches enum 'MAXpeak'
+	# item = 'SPECtrum1' matches enum 'SPEC1'
+	# item = 'SPEC' matches enum 'SPECtrum1'
+
+	item = ''.join([c for c in item if not c.islower()])
+	# item must be longer than 1 character
+	if len(item) < 2:
+		return -1
+	i = 0
+	for x in enum_members:
+		x_uc = ''.join([c for c in x if not c.islower()])
+		if x_uc == item:
+			return i
+		i += 1
+	return -1
+
+
+def str_to_scalar_enum_helper(string: str, enum_type: Enum, enum_members=None) -> Enum:
+	"""Converts string to one enum element.
+	enum_members are optional to improve the performance for repeated conversions.
+	If you do not provide them, they are generated inside the function."""
+	value = Utilities.trim_str_response(string)
+	if not enum_members:
+		# noinspection PyTypeChecker
+		enum_members = [x.name for x in enum_type]
+
+	# Search in the enum member and return the index of the matched item
+	ix = _find_in_enum_members(value, enum_members)
+	if ix >= 0:
+		# noinspection PyUnresolvedReferences
+		return enum_type[enum_members[ix]]
+
+	# If the result is -1 (not found), try to replace the special values and search again
+	# This is done to improve the performance, since most of the enums have no special values
+	enum_members_conv = [enum_value_to_scpi_string(x) for x in enum_members]
+	ix = _find_in_enum_members(value, enum_members_conv)
+	if ix >= 0:
+		# noinspection PyUnresolvedReferences
+		return enum_type[enum_members[ix]]
+
+	# If not found, search in the special integer numbers:
+	spec_value = str_special_values_to_int(value)
+	if not spec_value:
+		raise Exception(f"String '{value}' can not be found in the enum type '{enum_type}'")
+	# noinspection PyTypeChecker
+	return spec_value
+
+
+def str_to_list_enum_helper(string: str, enum_type: Enum, enum_members=None) -> List[Enum]:
+	"""Converts string to list of enum elements.
+	enum_members are optional to improve the performance for repeated conversions.
+	If you do not provide them, they are generated inside the function."""
+	if not enum_members:
+		# noinspection PyTypeChecker
+		enum_members = [x.name for x in enum_type]
+	elements = string.split(',')
+	return [str_to_scalar_enum_helper(x, enum_type, enum_members) for x in elements]
+
+
+def enum_scalar_to_str(data, enum_type) -> str:
+	"""Converts enum scalar value to string."""
+	assert isinstance(data, enum_type), f"Expected command parameter {enum_type}, actual data type: {type(data)}. Value: {data}"
+	return value_to_str(data)
+
+
+def enum_list_to_str(data: List, enum_type) -> str:
+	"""Converts enum list to csv-string."""
+	# For enums, check that each element is an enum
+	assert all(isinstance(x, enum_type) for x in data), f"Expected command parameter list of {enum_type}, detected one or more elements of non-enum type. Value: {data}"
+	return list_to_csv_str(data)
+
+
+def str_to_scalar_enum(string: str, enum_type) -> Enum:
+	"""Converts string to one enum element."""
+	return str_to_scalar_enum_helper(string, enum_type)
+
+
+def str_to_list_enum(string: str, enum_type) -> List[Enum]:
+	"""Converts string to list of enum elements."""
+	return str_to_list_enum_helper(string, enum_type)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/ConverterFromScpiString.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/ConverterFromScpiString.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-from enum import Enum
-
-from .Conversions import str_to_bool, str_to_int, str_to_int_or_bool, str_to_float, str_to_float_or_bool, str_to_scalar_enum_helper
-from .Conversions import str_to_str_list, str_to_bool_list, str_to_int_list, str_to_int_or_bool_list, str_to_float_list, str_to_float_or_bool_list, str_to_list_enum_helper
-from .Types import DataType
-from .Utilities import trim_str_response
-
-
-class ConverterFromScpiString:
-	"""Converter from SCPI response string to argument value
-	For list argument types, you must use the method get_one_element_value in a loop for each element.
-	Provides methods:
-	- get_one_element_value(str): returns one scalar value converted from the SCPI string.
-	- get_list_value(str): return complete list value converted from the SCPI string.
-	- get_value(str): calls either get_one_element_value or get_list_value() depending on the data type. \n
-	The reason for the different methods is, that sometimes the list data are interleaved with other arguments.
-	In order to parse them properly, the ArgStructStringParser module must be able to set the argument value element-by-element.
-	On the other side, the driver methods might want to set the whole argument value, because the result scpi string is a single argument response."""
-
-	def __init__(self, data_type: DataType, enum_type: Enum = None):
-		self.enum_type = enum_type
-		self.data_type = data_type
-		self.element_type = self.data_type.element_type
-
-		if self.element_type == DataType.RawString:
-			self.converter = trim_str_response
-			self.list_converter = str_to_str_list
-
-		elif self.element_type == DataType.String:
-			self.converter = trim_str_response
-			self.list_converter = str_to_str_list
-
-		elif self.element_type == DataType.Boolean:
-			self.converter = str_to_bool
-			self.list_converter = str_to_bool_list
-
-		elif self.element_type == DataType.Integer:
-			self.converter = str_to_int
-			self.list_converter = str_to_int_list
-
-		elif self.element_type == DataType.IntegerExt:
-			self.converter = str_to_int_or_bool
-			self.list_converter = str_to_int_or_bool_list
-
-		elif self.element_type == DataType.Float:
-			self.converter = str_to_float
-			self.list_converter = str_to_float_list
-
-		elif self.element_type == DataType.FloatExt:
-			self.converter = str_to_float_or_bool
-			self.list_converter = str_to_float_or_bool_list
-
-		elif self.element_type == DataType.Enum:
-			assert self.enum_type, f"For data type enum, you have to define the enum_type variable."
-			# noinspection PyTypeChecker
-			self.enum_members = [x.name for x in self.enum_type]
-		else:
-			raise Exception(f"Unsupported data type '{data_type}'")
-
-	def get_one_element_value(self, scpi_string: str):
-		"""Returns single element !!! of the argument value converted from the SCPI string (single element)"""
-		assert isinstance(scpi_string, str), f"Input parameter scpi_string must be string. Actual parameter: {type(scpi_string)}, value: {scpi_string}"
-		if self.element_type is DataType.Enum:
-			return str_to_scalar_enum_helper(scpi_string, self.enum_type, self.enum_members)
-		return self.converter(scpi_string)
-
-	def get_value(self, scpi_string: str):
-		"""Returns complete value of the argument converted from the SCPI string (list or scalar)"""
-		if not self.data_type.is_list:
-			return self.get_one_element_value(scpi_string)
-
-		assert isinstance(scpi_string, str), f"Input parameter scpi_string must be string. Actual parameter: {type(scpi_string)}, value: {scpi_string}"
-		if self.element_type is DataType.Enum:
-			return str_to_list_enum_helper(scpi_string, self.enum_type, self.enum_members)
-		return self.list_converter(scpi_string)
+from enum import Enum
+
+from .Conversions import str_to_bool, str_to_int, str_to_int_or_bool, str_to_float, str_to_float_or_bool, str_to_scalar_enum_helper
+from .Conversions import str_to_str_list, str_to_bool_list, str_to_int_list, str_to_int_or_bool_list, str_to_float_list, str_to_float_or_bool_list, str_to_list_enum_helper
+from .Types import DataType
+from .Utilities import trim_str_response
+
+
+class ConverterFromScpiString:
+	"""Converter from SCPI response string to argument value
+	For list argument types, you must use the method get_one_element_value in a loop for each element.
+	Provides methods:
+	- get_one_element_value(str): returns one scalar value converted from the SCPI string.
+	- get_list_value(str): return complete list value converted from the SCPI string.
+	- get_value(str): calls either get_one_element_value or get_list_value() depending on the data type. \n
+	The reason for the different methods is, that sometimes the list data are interleaved with other arguments.
+	In order to parse them properly, the ArgStructStringParser module must be able to set the argument value element-by-element.
+	On the other side, the driver methods might want to set the whole argument value, because the result scpi string is a single argument response."""
+
+	def __init__(self, data_type: DataType, enum_type: Enum = None):
+		self.enum_type = enum_type
+		self.data_type = data_type
+		self.element_type = self.data_type.element_type
+
+		if self.element_type == DataType.RawString:
+			self.converter = trim_str_response
+			self.list_converter = str_to_str_list
+
+		elif self.element_type == DataType.String:
+			self.converter = trim_str_response
+			self.list_converter = str_to_str_list
+
+		elif self.element_type == DataType.Boolean:
+			self.converter = str_to_bool
+			self.list_converter = str_to_bool_list
+
+		elif self.element_type == DataType.Integer:
+			self.converter = str_to_int
+			self.list_converter = str_to_int_list
+
+		elif self.element_type == DataType.IntegerExt:
+			self.converter = str_to_int_or_bool
+			self.list_converter = str_to_int_or_bool_list
+
+		elif self.element_type == DataType.Float:
+			self.converter = str_to_float
+			self.list_converter = str_to_float_list
+
+		elif self.element_type == DataType.FloatExt:
+			self.converter = str_to_float_or_bool
+			self.list_converter = str_to_float_or_bool_list
+
+		elif self.element_type == DataType.Enum:
+			assert self.enum_type, f"For data type enum, you have to define the enum_type variable."
+			# noinspection PyTypeChecker
+			self.enum_members = [x.name for x in self.enum_type]
+		else:
+			raise Exception(f"Unsupported data type '{data_type}'")
+
+	def get_one_element_value(self, scpi_string: str):
+		"""Returns single element !!! of the argument value converted from the SCPI string (single element)"""
+		assert isinstance(scpi_string, str), f"Input parameter scpi_string must be string. Actual parameter: {type(scpi_string)}, value: {scpi_string}"
+		if self.element_type is DataType.Enum:
+			return str_to_scalar_enum_helper(scpi_string, self.enum_type, self.enum_members)
+		return self.converter(scpi_string)
+
+	def get_value(self, scpi_string: str):
+		"""Returns complete value of the argument converted from the SCPI string (list or scalar)"""
+		if not self.data_type.is_list:
+			return self.get_one_element_value(scpi_string)
+
+		assert isinstance(scpi_string, str), f"Input parameter scpi_string must be string. Actual parameter: {type(scpi_string)}, value: {scpi_string}"
+		if self.element_type is DataType.Enum:
+			return str_to_list_enum_helper(scpi_string, self.enum_type, self.enum_members)
+		return self.list_converter(scpi_string)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/ConverterToScpiString.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/ConverterToScpiString.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-from enum import Enum
-
-from .Conversions import list_to_csv_quoted_str, value_to_quoted_str, list_to_csv_str, value_to_str, enum_list_to_str, enum_scalar_to_str
-from .Types import DataType
-
-
-def value_to_scpi_string(data, data_type: DataType):
-	"""Method to be used in the driver implementation.
-	Convert data to SCPI string parameter: data -> str"""
-	if data_type.is_list:
-		assert isinstance(data, list), f"Expected command parameter list, actual data type: {type(data)}. Value: {data}"
-	else:
-		assert not isinstance(data, list), f"Expected command parameter scalar, actual data type: {type(data)}. Value: {data}"
-	# Strings are enclosed by single quotes
-	if data_type == DataType.StringList:
-		assert all(isinstance(x, str) for x in data), f"Expected command parameter list of strings, detected one or more elements of non-string type. Value: {data}"
-		return list_to_csv_quoted_str(data)
-	elif data_type == DataType.String:
-		assert isinstance(data, str), f"Expected command parameter string, actual data type: {type(data)}. Value: {data}"
-		return value_to_quoted_str(data)
-
-	# Raw string is not enclosed by quotes
-	elif data_type == DataType.RawStringList:
-		assert all(isinstance(x, str) for x in data), f"Expected command parameter list of strings, detected one or more elements of non-string type. Value: {data}"
-		return list_to_csv_str(data)
-	elif data_type == DataType.RawString:
-		assert isinstance(data, str), f"Expected command parameter string, actual data type: {type(data)}. Value: {data}"
-		return value_to_str(data)
-
-	elif data_type == DataType.BooleanList:
-		assert all(type(x) == bool for x in data), f"Expected command parameter list of booleans, detected one or more elements of non-boolean type. Value: {data}"
-		return list_to_csv_str(data)
-	elif data_type == DataType.Boolean:
-		assert type(data) == bool, f"Expected command parameter boolean, actual data type: {type(data)}. Value: {data}"
-		return value_to_str(data)
-
-	# For integer and float, allow them to be mixed
-	elif data_type == DataType.IntegerList or data_type == DataType.FloatList:
-		assert all((isinstance(x, int) or isinstance(x, float)) and type(x) != bool for x in data), f"Expected command parameter list of numbers, detected one or more elements of non-number type. Value: {data}"
-		return list_to_csv_str(data)
-	elif data_type == DataType.Integer or data_type == DataType.Float:
-		assert (isinstance(data, int) or isinstance(data, float)) and type(data) != bool, f"Expected command parameter number, actual data type: {type(data)}. Value: {data}"
-		return value_to_str(data)
-
-	# For integer and float extended, allow them to be mixed including the boolean type
-	elif data_type == DataType.IntegerExtList or data_type == DataType.FloatExtList:
-		assert all((isinstance(x, int) or isinstance(x, float) or isinstance(x, bool)) for x in data), f"Expected command parameter list of numbers or booleans, detected one or more elements of non-number type. Value: {data}"
-		return list_to_csv_str(data)
-	elif data_type == DataType.IntegerExt or data_type == DataType.FloatExt:
-		assert (isinstance(data, int) or isinstance(data, float) or isinstance(data, bool)), f"Expected command parameter number or boolean, actual data type: {type(data)}. Value: {data}"
-		return value_to_str(data)
-	else:
-		raise Exception(f"Unsupported data type: '{type(data_type)}'.")
-
-
-class ConverterToScpiString:
-	"""Converter from argument value to SCPI string.
-	Provides method get_value(arg_value) -> str
-	"""
-
-	def __init__(self, data_type: DataType, enum_type: Enum = None):
-		self.enum_type = enum_type
-		self.data_type = data_type
-		self.element_type = self.data_type.element_type
-		if self.element_type == DataType.Enum:
-			assert self.enum_type, f"For data_type {data_type.name}, you have to define the enum_type variable."
-
-	def get_value(self, data) -> str:
-		"""Returns SCPI string converted from the argument data."""
-		if self.data_type.is_list:
-			assert isinstance(data, list), f"Expected command parameter list, actual data type: {type(data)}. Value: {data}"
-		else:
-			assert not isinstance(data, list), f"Expected command parameter scalar, actual data type: {type(data)}. Value: {data}"
-
-		if self.data_type == DataType.Enum:
-			return enum_scalar_to_str(data, self.enum_type)
-		elif self.data_type == DataType.EnumList:
-			return enum_list_to_str(data, self.enum_type)
-
-		return value_to_scpi_string(data, self.data_type)
+from enum import Enum
+
+from .Conversions import list_to_csv_quoted_str, value_to_quoted_str, list_to_csv_str, value_to_str, enum_list_to_str, enum_scalar_to_str
+from .Types import DataType
+
+
+def value_to_scpi_string(data, data_type: DataType):
+	"""Method to be used in the driver implementation.
+	Convert data to SCPI string parameter: data -> str"""
+	if data_type.is_list:
+		assert isinstance(data, list), f"Expected command parameter list, actual data type: {type(data)}. Value: {data}"
+	else:
+		assert not isinstance(data, list), f"Expected command parameter scalar, actual data type: {type(data)}. Value: {data}"
+	# Strings are enclosed by single quotes
+	if data_type == DataType.StringList:
+		assert all(isinstance(x, str) for x in data), f"Expected command parameter list of strings, detected one or more elements of non-string type. Value: {data}"
+		return list_to_csv_quoted_str(data)
+	elif data_type == DataType.String:
+		assert isinstance(data, str), f"Expected command parameter string, actual data type: {type(data)}. Value: {data}"
+		return value_to_quoted_str(data)
+
+	# Raw string is not enclosed by quotes
+	elif data_type == DataType.RawStringList:
+		assert all(isinstance(x, str) for x in data), f"Expected command parameter list of strings, detected one or more elements of non-string type. Value: {data}"
+		return list_to_csv_str(data)
+	elif data_type == DataType.RawString:
+		assert isinstance(data, str), f"Expected command parameter string, actual data type: {type(data)}. Value: {data}"
+		return value_to_str(data)
+
+	elif data_type == DataType.BooleanList:
+		assert all(type(x) == bool for x in data), f"Expected command parameter list of booleans, detected one or more elements of non-boolean type. Value: {data}"
+		return list_to_csv_str(data)
+	elif data_type == DataType.Boolean:
+		assert type(data) == bool, f"Expected command parameter boolean, actual data type: {type(data)}. Value: {data}"
+		return value_to_str(data)
+
+	# For integer and float, allow them to be mixed
+	elif data_type == DataType.IntegerList or data_type == DataType.FloatList:
+		assert all((isinstance(x, int) or isinstance(x, float)) and type(x) != bool for x in data), f"Expected command parameter list of numbers, detected one or more elements of non-number type. Value: {data}"
+		return list_to_csv_str(data)
+	elif data_type == DataType.Integer or data_type == DataType.Float:
+		assert (isinstance(data, int) or isinstance(data, float)) and type(data) != bool, f"Expected command parameter number, actual data type: {type(data)}. Value: {data}"
+		return value_to_str(data)
+
+	# For integer and float extended, allow them to be mixed including the boolean type
+	elif data_type == DataType.IntegerExtList or data_type == DataType.FloatExtList:
+		assert all((isinstance(x, int) or isinstance(x, float) or isinstance(x, bool)) for x in data), f"Expected command parameter list of numbers or booleans, detected one or more elements of non-number type. Value: {data}"
+		return list_to_csv_str(data)
+	elif data_type == DataType.IntegerExt or data_type == DataType.FloatExt:
+		assert (isinstance(data, int) or isinstance(data, float) or isinstance(data, bool)), f"Expected command parameter number or boolean, actual data type: {type(data)}. Value: {data}"
+		return value_to_str(data)
+	else:
+		raise Exception(f"Unsupported data type: '{type(data_type)}'.")
+
+
+class ConverterToScpiString:
+	"""Converter from argument value to SCPI string.
+	Provides method get_value(arg_value) -> str
+	"""
+
+	def __init__(self, data_type: DataType, enum_type: Enum = None):
+		self.enum_type = enum_type
+		self.data_type = data_type
+		self.element_type = self.data_type.element_type
+		if self.element_type == DataType.Enum:
+			assert self.enum_type, f"For data_type {data_type.name}, you have to define the enum_type variable."
+
+	def get_value(self, data) -> str:
+		"""Returns SCPI string converted from the argument data."""
+		if self.data_type.is_list:
+			assert isinstance(data, list), f"Expected command parameter list, actual data type: {type(data)}. Value: {data}"
+		else:
+			assert not isinstance(data, list), f"Expected command parameter scalar, actual data type: {type(data)}. Value: {data}"
+
+		if self.data_type == DataType.Enum:
+			return enum_scalar_to_str(data, self.enum_type)
+		elif self.data_type == DataType.EnumList:
+			return enum_list_to_str(data, self.enum_type)
+
+		return value_to_scpi_string(data, self.data_type)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/Core.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/Core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,252 +1,264 @@
-import re
-from typing import Callable
-
-from . import InstrumentOptions as Options, Conversions as Conv
-from .ArgSingle import ArgSingle
-from .ArgSingleList import ArgSingleList
-from .Conversions import BinFloatFormat, BinIntFormat
-from .Instrument import Instrument
-from .InstrumentSettings import InstrViClearMode, InstrumentSettings, WaitForOpcMode
-from .Utilities import parse_token_to_key_and_value, trim_str_response
-
-
-class Core(object):
-	"""Main driver component. Provides: \n
-		- Main core constructor
-		- 'io' interface for all the write / query operations
-		- Command parameters string composer for single arguments...
-		- Link handlers adding / changing / deleting
-
-		1.7.7 (build 42) 26.11.2020
-			- Extended ArgSingleList.compose_cmd_string() to 9 arguments
-
-		1.7.6 (build 41) 23.11.2020
-			- Extended data types for IntegerExt, FloatExt, IntegerExtArray, FloatExtArray
-
-		1.7.5 (build 40) 12.11.2020
-			- Extended Conversions method str_to_str_list() by parameter 'clear_one_empty_item' with default value False
-
-		1.7.4 (build 39) 11.09.2020
-			- Fixed parsing of the instrument errors when an error message contains two double quotes
-
-		1.7.3 (build 38) 21.10.2020
-			- Added 'UND' to the list of float numbers that are represented as NaN
-
-		1.7.2 (build 37) 10.10.2020
-			- SCPI response string conversion to scalar enum: if the string contains ',', the content after it inclusive the comma is ignored
-
-		1.7.1 (build 36) 08.10.2020
-			- Fixed Python 3.8.5+ warnings
-
-		1.7.0 (build 34) 30.09.2020
-			- Added option to set the termination characters for reading and writing. Until now, it was fixed to '\n' (Linefeed)
-			- Replaced 'import visa' with 'import pyvisa' to remove Python 3.8 pyvisa warnings
-
-		Version History:
-		1.6.0 (build 33) 17.09.2020
-			- Added special characters encoding/decoding in enums
-
-		1.4.0 (build 32) 17.09.2020
-			- Added recognition of RsVisa library location for linux when using options string 'SelectVisa=rs'
-			- Fixed bug in reading binary data 16 bit
-
-		1.3.0 (build 31) 04.09.2020
-			- added DRIVERSETUP_QUERYOPT to the driver's option string
-			- *OPT? is no longer performed at the init, but only at the first access to options string.
-				In addition, the *OPT? query is executed with 1000 ms timeout, and the errors are suppressed
-
-		1.2.0 (build 30), 03.08.2020
-			- Fixed NRP-Z session parameters: vxi_capable = False, io_segment_size = 1000000
-
-		1.1.0 (build 29), 20.06.2020
-			- Added RepeatedCapability and base class CommandsGroup
-			- Fixed simulation mode switching
-
-		0.9.3 (build 25), 23.04.2020 - Fixed composition of optional arguments in ArgSingleList and ArgSingle
-		0.9.2 (build 24), 13.11.2019 - Added recognition of special values for enum return strings
-		0.9.1 - Added read / write to file, refactored internals to work with streams
-		0.9.0 - First Version created."""
-
-	driver_version: str = ''
-	"""Placeholder for the driver version string."""
-
-	def __init__(
-			self,
-			resource_name: str,
-			id_query: bool = True,
-			reset: bool = False,
-			driver_options: str = None,
-			user_options: str = None,
-			direct_session: object = None):
-		"""Initializes new driver session. For cleaner code, use the class methods: \n
-		- Core.from_existing_session() - initializes a new Core with an existing pyvisa session."""
-
-		self.core_version = '1.7.6'
-		self.simulating = False
-		self.supported_idn_patterns = []
-		self.supported_instr_models = []
-
-		self._args_single_list = ArgSingleList()
-		sett_dr = self._parse_init_settings_string(driver_options)
-		self._apply_settings_to_core(sett_dr)
-		sett_user = self._parse_init_settings_string(user_options)
-		self._apply_settings_to_core(sett_user)
-
-		# Typical settings for the Core
-		self._instrumentSettings = InstrumentSettings(
-			InstrViClearMode.execute_on_all,  # Instrument viClear mode
-			False,  # Full model name. True: SMW200A, False: SMW
-			0,  # Delay by each write
-			0,  # Delay by each read
-			100000,  # Max chunk read / write size in bytes
-			WaitForOpcMode.stb_poll,  # Waiting for OPC Mode: Status byte polling
-			30000,  # OPC timeout
-			10000,  # VISA timeout
-			60000,  # Self-test timeout
-			Options.ParseMode.Auto,  # *OPT? response parsing mode
-			BinFloatFormat.Single_4bytes,  # Format for parsing of binary float numbers
-			BinIntFormat.Integer32_4bytes,  # Format for parsing of binary integer numbers
-			False  # OPC query after each setting
-		)
-
-		self._instrumentSettings.apply_option_settings(sett_dr)
-		self._instrumentSettings.apply_option_settings(sett_user)
-
-		# Resolve the direct_session to handle. Options for direct_session type:
-		# - VisaSession object, retrieved from the driver's RsInstrument.get_session_handle() method
-		# - string in case of a simulation session
-		handle = direct_session
-		if handle:
-			# Check if the entered 'direct_session' is either the driver object or the Visa session
-			if hasattr(direct_session, 'get_session_handle'):
-				assert hasattr(direct_session, '_core'), f"Direct session is a class type. It must be an instance of the top-level driver class."
-				handle = direct_session.get_session_handle()
-			# Check if the handle is not a simulation mode string
-			if isinstance(handle, str):
-				if "Simulating session, resource name " in handle:
-					self.simulating = True
-					handle = None
-
-		self.io = Instrument(resource_name, self.simulating, self._instrumentSettings, handle)
-		self.io.query_instr_status = True
-
-		self._apply_settings_to_instrument(sett_dr)
-		self._apply_settings_to_instrument(sett_user)
-
-		self.io.set_simulating_cmds()
-
-		if id_query:
-			self.io.fits_idn_pattern(self.supported_idn_patterns, self.supported_instr_models)
-
-		if reset:
-			self.io.reset()
-		else:
-			self.io.check_status()
-
-	@classmethod
-	def from_existing_session(cls, session: object, driver_options: str = None) -> 'Core':
-		"""Creates a new Core object with the entered 'session' reused."""
-		# noinspection PyTypeChecker
-		return cls(None, False, False, driver_options, None, session)
-
-	def __str__(self):
-		return f"Core session '{self.io.resource_name}'"
-
-	def set_link_handler(self, link_name: str, handler: Callable) -> Callable:
-		"""Adds / Updates link handler for the entered link_name.
-		Handler API: handler(event_args: ArgLinkedEventArgs)
-		Returns the previous registered handler, or None if no handler was registered before."""
-		return self.io.set_link_handler(link_name, handler)
-
-	def del_link_handler(self, link_name: str) -> Callable:
-		"""Deletes link handler for the link_name.
-		Returns the deleted handler, or None if none existed."""
-		return self.io.del_link_handler(link_name)
-
-	def del_all_link_handlers(self) -> int:
-		"""Deletes all the link handlers.
-		Returns number of deleted links."""
-		return self.io.del_all_link_handlers()
-
-	# noinspection PyMethodMayBeStatic
-	def _parse_init_settings_string(self, text: str) -> dict:
-		"""Parses init string to a dictionary of settings: name -> value."""
-		tokens = {}
-		if not text:
-			return tokens
-
-		# Text enclosed in single brackets '' must have the commas escaped
-		literal_pattern = r"'([^']+)'"
-		while True:
-			# literal loop
-			m = re.search(literal_pattern, text)
-			if not m:
-				break
-			lit_part = '"' + m.group(1).replace(',', '<COMMA_ESC>') + '"'
-			text = text.replace(m.group(0), lit_part)
-
-		# Remove all the class-options enclosed by round brackets e.g. "<groupName>=(<groupTokens>)"
-		group_pattern = r'(\w+)\s*=\s*\(([^\)]*)\)'
-		# Match class-settings, add them as separate keys with groupName_Key
-		while True:
-			# Group loop
-			m = re.search(group_pattern, text)
-			if not m:
-				break
-			text = text.replace(m.group(0), '')
-			group_name = m.group(1).upper()
-			group_tokens = m.group(2).strip().split(',')
-			for token in group_tokens:
-				key, value = parse_token_to_key_and_value(token)
-				if value:
-					tokens[f'{group_name}_{key.upper()}'] = value
-
-		# All groups are removed from the text, now we can use splitting on commas and remove white-space-only elements
-		for token in text.split(','):
-			key, value = parse_token_to_key_and_value(token.replace('<COMMA_ESC>', ','))
-			if value:
-				tokens[key.upper()] = value
-		return tokens
-
-	def _apply_settings_to_core(self, settings: dict) -> None:
-		"""Applies settings relevant for the Core from the dictionary."""
-		value = settings.get('SIMULATE')
-		if value:
-			self.simulating = Conv.str_to_bool(value)
-
-		value = settings.get('SUPPORTEDINSTRMODELS')
-		if value:
-			self.supported_instr_models = [*map(trim_str_response, value.split('/'))]
-
-		value = settings.get('SUPPORTEDIDNPATTERNS')
-		if value:
-			self.supported_idn_patterns = [*map(trim_str_response, value.split('/'))]
-
-	def _apply_settings_to_instrument(self, settings: dict) -> None:
-		"""Applies settings relevant for the Instrument from the dictionary."""
-		value = settings.get('QUERYINSTRUMENTSTATUS')
-		if value:
-			self.io.query_instr_status = Conv.str_to_bool(value)
-
-		value = settings.get('SIMULATIONIDNSTRING')
-		if value and self.simulating:
-			# Use the '*' instead of the ',' in the value to avoid comma as token delimiter
-			self.io.idn_string = value.replace('*', ',')
-
-	def compose_cmd_arg_param(
-			self, arg1: ArgSingle, arg2: ArgSingle = None, arg3: ArgSingle = None, arg4: ArgSingle = None, arg5: ArgSingle = None, arg6: ArgSingle = None) -> str:
-		"""Composes command parameter string based on the single arguments definition."""
-		return self._args_single_list.compose_cmd_string(arg1, arg2, arg3, arg4, arg5, arg6)
-
-	def get_last_sent_cmd(self) -> str:
-		"""Returns the last commands sent to the instrument. Only works in simulation mode"""
-		return self.io.get_last_sent_cmd()
-
-	def get_session_handle(self):
-		"""Returns the underlying pyvisa session."""
-		return self.io.get_session_handle()
-
-	def close(self):
-		"""Closes the Core session."""
-		self.io.close()
-		self.io = None
+import re
+from typing import Callable
+
+from . import InstrumentOptions as Options, Conversions as Conv
+from .ArgSingle import ArgSingle
+from .ArgSingleList import ArgSingleList
+from .Conversions import BinFloatFormat, BinIntFormat
+from .Instrument import Instrument
+from .InstrumentSettings import InstrViClearMode, InstrumentSettings, WaitForOpcMode
+from .Utilities import parse_token_to_key_and_value, trim_str_response
+
+
+class Core(object):
+	"""Main driver component. Provides: \n
+		- Main core constructor
+		- 'io' interface for all the write / query operations
+		- Command parameters string composer for single arguments...
+		- Link handlers adding / changing / deleting
+
+		Version history:
+
+		1.10.0 (build 46) 03.05.2021
+			- Added methods to Instrument: query_struct_with_opc(), query_str_suppressed_with_opc()
+
+		1.9.0 (build 45) 13.04.2021
+			- Added option to set callbacks before_write and before_query
+			- When a RepCap has a member with integer number 0 defined, the command string interpretation of such member is '0', not empty string
+
+		1.8.0 (build 43) 19.01.2021
+			- Added matching of Enum instrument responses also in short/long form
+
+		1.7.7 (build 42) 26.11.2020
+			- Extended ArgSingleList.compose_cmd_string() to 9 arguments
+
+		1.7.6 (build 41) 23.11.2020
+			- Extended data types for IntegerExt, FloatExt, IntegerExtArray, FloatExtArray
+
+		1.7.5 (build 40) 12.11.2020
+			- Extended Conversions method str_to_str_list() by parameter 'clear_one_empty_item' with default value False
+
+		1.7.4 (build 39) 11.09.2020
+			- Fixed parsing of the instrument errors when an error message contains two double quotes
+
+		1.7.3 (build 38) 21.10.2020
+			- Added 'UND' to the list of float numbers that are represented as NaN
+
+		1.7.2 (build 37) 10.10.2020
+			- SCPI response string conversion to scalar enum: if the string contains ',', the content after it inclusive the comma is ignored
+
+		1.7.1 (build 36) 08.10.2020
+			- Fixed Python 3.8.5+ warnings
+
+		1.7.0 (build 34) 30.09.2020
+			- Added option to set the termination characters for reading and writing. Until now, it was fixed to '\n' (Linefeed)
+			- Replaced 'import visa' with 'import pyvisa' to remove Python 3.8 pyvisa warnings
+
+		Version History:
+		1.6.0 (build 33) 17.09.2020
+			- Added special characters encoding/decoding in enums
+
+		1.4.0 (build 32) 17.09.2020
+			- Added recognition of RsVisa library location for linux when using options string 'SelectVisa=rs'
+			- Fixed bug in reading binary data 16 bit
+
+		1.3.0 (build 31) 04.09.2020
+			- added DRIVERSETUP_QUERYOPT to the driver's option string
+			- *OPT? is no longer performed at the init, but only at the first access to options string.
+				In addition, the *OPT? query is executed with 1000 ms timeout, and the errors are suppressed
+
+		1.2.0 (build 30), 03.08.2020
+			- Fixed NRP-Z session parameters: vxi_capable = False, io_segment_size = 1000000
+
+		1.1.0 (build 29), 20.06.2020
+			- Added RepeatedCapability and base class CommandsGroup
+			- Fixed simulation mode switching
+
+		0.9.3 (build 25), 23.04.2020 - Fixed composition of optional arguments in ArgSingleList and ArgSingle
+		0.9.2 (build 24), 13.11.2019 - Added recognition of special values for enum return strings
+		0.9.1 - Added read / write to file, refactored internals to work with streams
+		0.9.0 - First Version created."""
+
+	driver_version: str = ''
+	"""Placeholder for the driver version string."""
+
+	def __init__(
+			self,
+			resource_name: str,
+			id_query: bool = True,
+			reset: bool = False,
+			driver_options: str = None,
+			user_options: str = None,
+			direct_session: object = None):
+		"""Initializes new driver session. For cleaner code, use the class methods: \n
+		- Core.from_existing_session() - initializes a new Core with an existing pyvisa session."""
+
+		self.core_version = '1.9.0'
+		self.simulating = False
+		self.supported_idn_patterns = []
+		self.supported_instr_models = []
+
+		self._args_single_list = ArgSingleList()
+		sett_dr = self._parse_init_settings_string(driver_options)
+		self._apply_settings_to_core(sett_dr)
+		sett_user = self._parse_init_settings_string(user_options)
+		self._apply_settings_to_core(sett_user)
+
+		# Typical settings for the Core
+		self._instrumentSettings = InstrumentSettings(
+			InstrViClearMode.execute_on_all,  # Instrument viClear mode
+			False,  # Full model name. True: SMW200A, False: SMW
+			0,  # Delay by each write
+			0,  # Delay by each read
+			100000,  # Max chunk read / write size in bytes
+			WaitForOpcMode.stb_poll,  # Waiting for OPC Mode: Status byte polling
+			30000,  # OPC timeout
+			10000,  # VISA timeout
+			60000,  # Self-test timeout
+			Options.ParseMode.Auto,  # *OPT? response parsing mode
+			BinFloatFormat.Single_4bytes,  # Format for parsing of binary float numbers
+			BinIntFormat.Integer32_4bytes,  # Format for parsing of binary integer numbers
+			False  # OPC query after each setting
+		)
+
+		self._instrumentSettings.apply_option_settings(sett_dr)
+		self._instrumentSettings.apply_option_settings(sett_user)
+
+		# Resolve the direct_session to handle. Options for direct_session type:
+		# - VisaSession object, retrieved from the driver's RsInstrument.get_session_handle() method
+		# - string in case of a simulation session
+		handle = direct_session
+		if handle:
+			# Check if the entered 'direct_session' is either the driver object or the Visa session
+			if hasattr(direct_session, 'get_session_handle'):
+				assert hasattr(direct_session, '_core'), f"Direct session is a class type. It must be an instance of the top-level driver class."
+				handle = direct_session.get_session_handle()
+			# Check if the handle is not a simulation mode string
+			if isinstance(handle, str):
+				if "Simulating session, resource name " in handle:
+					self.simulating = True
+					handle = None
+
+		self.io = Instrument(resource_name, self.simulating, self._instrumentSettings, handle)
+		self.io.query_instr_status = True
+
+		self._apply_settings_to_instrument(sett_dr)
+		self._apply_settings_to_instrument(sett_user)
+
+		self.io.set_simulating_cmds()
+
+		if id_query:
+			self.io.fits_idn_pattern(self.supported_idn_patterns, self.supported_instr_models)
+
+		if reset:
+			self.io.reset()
+		else:
+			self.io.check_status()
+
+	@classmethod
+	def from_existing_session(cls, session: object, driver_options: str = None) -> 'Core':
+		"""Creates a new Core object with the entered 'session' reused."""
+		# noinspection PyTypeChecker
+		return cls(None, False, False, driver_options, None, session)
+
+	def __str__(self):
+		return f"Core session '{self.io.resource_name}'"
+
+	def set_link_handler(self, link_name: str, handler: Callable) -> Callable:
+		"""Adds / Updates link handler for the entered link_name.
+		Handler API: handler(event_args: ArgLinkedEventArgs)
+		Returns the previous registered handler, or None if no handler was registered before."""
+		return self.io.set_link_handler(link_name, handler)
+
+	def del_link_handler(self, link_name: str) -> Callable:
+		"""Deletes link handler for the link_name.
+		Returns the deleted handler, or None if none existed."""
+		return self.io.del_link_handler(link_name)
+
+	def del_all_link_handlers(self) -> int:
+		"""Deletes all the link handlers.
+		Returns number of deleted links."""
+		return self.io.del_all_link_handlers()
+
+	# noinspection PyMethodMayBeStatic
+	def _parse_init_settings_string(self, text: str) -> dict:
+		"""Parses init string to a dictionary of settings: name -> value."""
+		tokens = {}
+		if not text:
+			return tokens
+
+		# Text enclosed in single brackets '' must have the commas escaped
+		literal_pattern = r"'([^']+)'"
+		while True:
+			# literal loop
+			m = re.search(literal_pattern, text)
+			if not m:
+				break
+			lit_part = '"' + m.group(1).replace(',', '<COMMA_ESC>') + '"'
+			text = text.replace(m.group(0), lit_part)
+
+		# Remove all the class-options enclosed by round brackets e.g. "<groupName>=(<groupTokens>)"
+		group_pattern = r'(\w+)\s*=\s*\(([^\)]*)\)'
+		# Match class-settings, add them as separate keys with groupName_Key
+		while True:
+			# Group loop
+			m = re.search(group_pattern, text)
+			if not m:
+				break
+			text = text.replace(m.group(0), '')
+			group_name = m.group(1).upper()
+			group_tokens = m.group(2).strip().split(',')
+			for token in group_tokens:
+				key, value = parse_token_to_key_and_value(token)
+				if value:
+					tokens[f'{group_name}_{key.upper()}'] = value
+
+		# All groups are removed from the text, now we can use splitting on commas and remove white-space-only elements
+		for token in text.split(','):
+			key, value = parse_token_to_key_and_value(token.replace('<COMMA_ESC>', ','))
+			if value:
+				tokens[key.upper()] = value
+		return tokens
+
+	def _apply_settings_to_core(self, settings: dict) -> None:
+		"""Applies settings relevant for the Core from the dictionary."""
+		value = settings.get('SIMULATE')
+		if value:
+			self.simulating = Conv.str_to_bool(value)
+
+		value = settings.get('SUPPORTEDINSTRMODELS')
+		if value:
+			self.supported_instr_models = [*map(trim_str_response, value.split('/'))]
+
+		value = settings.get('SUPPORTEDIDNPATTERNS')
+		if value:
+			self.supported_idn_patterns = [*map(trim_str_response, value.split('/'))]
+
+	def _apply_settings_to_instrument(self, settings: dict) -> None:
+		"""Applies settings relevant for the Instrument from the dictionary."""
+		value = settings.get('QUERYINSTRUMENTSTATUS')
+		if value:
+			self.io.query_instr_status = Conv.str_to_bool(value)
+
+		value = settings.get('SIMULATIONIDNSTRING')
+		if value and self.simulating:
+			# Use the '*' instead of the ',' in the value to avoid comma as token delimiter
+			self.io.idn_string = value.replace('*', ',')
+
+	def compose_cmd_arg_param(
+			self, arg1: ArgSingle, arg2: ArgSingle = None, arg3: ArgSingle = None, arg4: ArgSingle = None, arg5: ArgSingle = None, arg6: ArgSingle = None) -> str:
+		"""Composes command parameter string based on the single arguments definition."""
+		return self._args_single_list.compose_cmd_string(arg1, arg2, arg3, arg4, arg5, arg6)
+
+	def get_last_sent_cmd(self) -> str:
+		"""Returns the last commands sent to the instrument. Only works in simulation mode"""
+		return self.io.get_last_sent_cmd()
+
+	def get_session_handle(self):
+		"""Returns the underlying pyvisa session."""
+		return self.io.get_session_handle()
+
+	def close(self):
+		"""Closes the Core session."""
+		self.io.close()
+		self.io = None
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/Instrument.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/Instrument.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,781 +1,854 @@
-import re
-import threading
-from enum import Enum
-from typing import List, Callable, Tuple, Dict
-
-from . import Utilities, InstrumentSettings, InstrumentOptions, InstrumentErrors, Conversions as Conv
-from .ArgSingleSuppressed import ArgSingleSuppressed
-from .ArgStructList import ArgStructList
-from .InternalLinker import InternalLinker
-from .IoTransferEventArgs import IoTransferEventArgs
-from .StreamReader import StreamReader
-from .StreamWriter import StreamWriter
-from .Utilities import trim_str_response
-from .VisaSession import VisaSession, EventArgsChunk
-from .VisaSessionSim import VisaSessionSim
-from .RepeatedCapability import RepeatedCapability
-
-
-class Instrument(object):
-	"""Model of an Instrument with VISA interface."""
-
-	def __init__(self, resource_name: str, simulate: bool, settings: InstrumentSettings, direct_session=None):
-		"""Opening an instrument session.
-		If simulate is true, it cannot be later switched to false anymore."""
-		self._simulating: bool = simulate
-		self._session = None
-		self._global_repcaps: Dict[str, RepeatedCapability] = {}
-		self._linker = InternalLinker()
-		# noinspection PyTypeChecker
-		self.on_write_handler: Callable = None
-		# noinspection PyTypeChecker
-		self.on_read_handler: Callable = None
-		self._io_events_include_data: bool = False
-		self._lock = None
-
-		# Fixed settings
-		self.selftest_timeout = 100000 if settings.selftest_timeout == 0 else settings.selftest_timeout
-		self.idn_model_full_name = settings.idn_model_full_name
-		self.instr_options_parse_mode = settings.instr_options_parse_mode
-
-		# Changeable settings
-		self.resource_name: str = resource_name
-		self._instr_options: InstrumentOptions = None  # Internal private property for the lazy property self.instr_options - see the getter for self.instr_options. Initialized by the first access
-		self.query_instr_status: bool = True
-		self.opc_query_after_write: bool = False
-		self.bin_float_numbers_format = settings.bin_float_numbers_format
-		self.bin_int_numbers_format = settings.bin_int_numbers_format
-		self.opc_query_after_write: bool = settings.opc_query_after_write
-		self.stb_in_error_check: bool = settings.stb_in_error_check
-
-		self.manufacturer: str = 'Rohde&Schwarz'
-		self.model: str = 'R&S Instrument'
-		self.serial_number: str = '100001'
-		self.firmware_version: str = '1.00'
-
-		if self._simulating:
-			self._session = VisaSessionSim(resource_name, settings, direct_session)
-			self._lock = self._session.get_lock()
-			self._instr_options = InstrumentOptions.Options('K0', InstrumentOptions.ParseMode.KeepOriginal)
-			self._session.write("*OPT K0")
-			return
-
-		self._session = VisaSession(resource_name, settings, direct_session)
-		self._lock = self._session.get_lock()
-		with self._lock:
-			self._session.clear_before_read()
-			self.idn_string = Utilities.trim_str_response(self._session.query_str('*IDN?')).strip()
-
-			# NRP-Z session coercing
-			if self._session.is_rsnrp_session():
-				settings.instr_options_parse_mode = InstrumentOptions.ParseMode.Skip
-				self.stb_in_error_check = False
-			self.instr_options_parse_mode = settings.instr_options_parse_mode
-
-	def __str__(self):
-		if self._simulating:
-			return f"Simulated, Model: '{self.model}', ResourceName: '{self.resource_name}'"
-		else:
-			return f"Instrument Model: '{self.model}', ResourceName: '{self.resource_name}'"
-
-	def set_simulating_cmds(self) -> None:
-		"""Updated cached values in the simulating VISA session to properly respond to *IDN? or *OPT?"""
-		if self._simulating:
-			self.write(f'*idn {self.idn_string}')
-			self.write(f'*opt {Conv.list_to_csv_str(self.instr_options.get_all())}')
-			self.write(f'*opc 1')
-			self.write(f'*stb 0')
-			self.write(f'*tst 0,"Passed"')
-			self.write(f'syst:err 0,"No Error"')
-			self.write(f'system:error 0,"No Error"')
-
-	def get_last_sent_cmd(self) -> str:
-		"""Returns the last commands sent to the instrument. Only works in simulation mode"""
-		if self._simulating:
-			# noinspection PyUnresolvedReferences
-			return self._session.get_last_sent_cmd()
-		raise Exception("get_last_sent_cmd() can only be used in simulation mode")
-
-	def assign_lock(self, lock: threading.RLock) -> None:
-		"""Assigns the thread lock provided from by the user. Trickles down to the VisaSession."""
-		self._lock = lock
-		self._session.assign_lock(lock)
-
-	def get_lock(self) -> threading.RLock:
-		"""Returns the current RLock object."""
-		return self._lock
-
-	def clear_lock(self):
-		"""Clears the existing thread lock, making the current session thread-independent from others that might share the current thread lock."""
-		self.assign_lock(threading.RLock())
-
-	@property
-	def visa_manufacturer(self) -> str:
-		"""Returns the visa manufacturer of the current session."""
-		return self._session.manufacturer
-
-	def set_link_handler(self, link_name: str, handler: Callable) -> Callable:
-		"""Adds / Updates link handler for the entered link_name.
-		Handler API: handler(event_args: ArgLinkedEventArgs)
-		Returns the previous registered handler, or None if no handler was registered before."""
-		return self._linker.set_handler(link_name, handler)
-
-	def del_link_handler(self, link_name: str) -> Callable:
-		"""Deletes link handler for the link_name.
-		Returns the deleted handler, or None if none existed."""
-		return self._linker.del_handler(link_name)
-
-	def del_all_link_handlers(self) -> int:
-		"""Deletes all the link handlers.
-		Returns number of deleted links."""
-		return self._linker.del_all_handlers()
-
-	@property
-	def idn_string(self) -> str:
-		return self._idn_string
-
-	@idn_string.setter
-	def idn_string(self, value: str) -> None:
-		"""IDN string. Set it to force a different IDN string than the default *IDN? response."""
-		self._idn_string = value
-		self._parse_idn_string(self._idn_string)
-
-	@property
-	def instr_options(self) -> InstrumentOptions:
-		"""Public getter for the lazy property instr_options"""
-		if self._instr_options is None:
-			self._query_options_and_parse(self.instr_options_parse_mode)
-		return self._instr_options
-
-	@property
-	def opc_timeout(self) -> int:
-		"""See the opc_timeout.setter."""
-		return self._session.opc_timeout
-
-	@opc_timeout.setter
-	def opc_timeout(self, value: int) -> None:
-		"""Sets / Gets timeout in milliseconds for all the operations that use OPC synchronization."""
-		self._session.opc_timeout = value
-
-	@property
-	def visa_timeout(self) -> int:
-		"""See the visa_timeout.setter."""
-		return self._session.visa_timeout
-
-	@visa_timeout.setter
-	def visa_timeout(self, value: int) -> None:
-		"""Sets / Gets visa IO timeout in milliseconds."""
-		self._session.visa_timeout = value
-
-	@property
-	def data_chunk_size(self) -> int:
-		"""Returns max chunk size of one data block."""
-		return self._session.data_chunk_size
-
-	@data_chunk_size.setter
-	def data_chunk_size(self, chunk_size: int) -> None:
-		"""Sets the maximum size of one block transferred during write/read operations."""
-		self._session.data_chunk_size = int(chunk_size)
-
-	# noinspection PyMethodMayBeStatic
-	def _sim_cached_value_found(self, value) -> bool:
-		return value != 'Simulating'
-
-	# noinspection PyMethodMayBeStatic
-	def _sim_cached_value_not_found(self, value) -> bool:
-		return value == 'Simulating'
-
-	def _parse_idn_string(self, idn_string: str) -> None:
-		"""Parse the *IDN? response to:
-		- Manufacturer
-		- Model
-		- SerialNumber
-		- FirmwareRevision"""
-		idn_string = idn_string.strip()
-		m = re.search(r'([\w& ]+),([a-zA-Z ]+)([\-0-9a-zA-Z ]*),([^,]+),([\w .\-/]+)', idn_string)
-		if not m:
-			raise Exception(f"The instrument *IDN? string parsing failed. Parsed *IDN? response: '{idn_string}'")
-		self.manufacturer = m.group(1).strip()
-		self.model = m.group(2).strip()
-		self.full_model_name = self.model + m.group(3).strip()
-		self.serial_number = m.group(4).strip()
-		self.firmware_version = m.group(5).strip()
-		if self.idn_model_full_name:
-			self.model = self.full_model_name
-
-	def fits_idn_pattern(self, patterns: List[str], supported_models: List[str]) -> None:
-		"""Throws exception if the current instrument model does not fit  any of the patterns.
-		The supported_models argument is only used for exception messages"""
-		matches = False
-		assert self._idn_string, f'*IDN? was not assigned yet.'
-		for x in patterns:
-			matches = re.search(x, self.idn_string, re.IGNORECASE)
-			if matches:
-				break
-		if not matches:
-			message = f"Instrument is not supported.\n*IDN? string: '{self.idn_string}'"
-			if len(supported_models) > 0:
-				message += f"\nSupported models: '{', '.join(supported_models)}'"
-			if len(patterns) == 1:
-				message += f"\nSupported IDN pattern: '{patterns[0]}'"
-			if len(patterns) > 1:
-				message += "\nSupported IDN patterns:\n" + '\n'.join(patterns)
-			raise InstrumentErrors.UnexpectedResponseException(self.resource_name, message)
-
-	def _query_options_and_parse(self, mode: InstrumentOptions.ParseMode) -> None:
-		"""Queries *OPT? and parses it based on the ParseMode."""
-		if mode == InstrumentOptions.ParseMode.Skip:
-			self._instr_options = InstrumentOptions.Options('', mode)
-			return
-		if self._simulating is False:
-			with self._lock:
-				opts = self._session.query_str_no_tout_err('*OPT?', 1000)
-				if opts is None:
-					opts = 'Cannot read the instrument options - *OPT? query is not supported'
-				self._instr_options = InstrumentOptions.Options(opts, mode)
-
-	@staticmethod
-	def _parse_err_query_response(response: str) -> str:
-		"""Parses entered response string to string error message without the error code.
-		E.g.: response = '-110,"Command error"' returns: 'Command error'."""
-		m = re.match(r'(-?[\d]+).*?"(.*)"', response)
-		if m:
-			return m.group(2)
-		else:
-			return response
-
-	def add_global_repcap(self, name: str, rep_cap: RepeatedCapability) -> None:
-		"""Adds the global repcap name to the list of global repcaps
-		and sets its value to the provided default value."""
-		if name in self._global_repcaps:
-			raise Exception(f"Error adding new global repcap: '{name}' already exists in the list.")
-		self._global_repcaps[name] = rep_cap
-
-	def set_global_repcap_value(self, name: str, enum_value: Enum) -> None:
-		"""Updates the existing global repcap value as enum"""
-		if name not in self._global_repcaps:
-			raise Exception(f"Error updating global repcap: '{name}' does not exist in the list.")
-		self._global_repcaps[name].set_enum_value(enum_value)
-
-	def get_global_repcap_value(self, name: str) -> Enum:
-		"""Returns the current global repcap value as enum"""
-		if name not in self._global_repcaps:
-			raise Exception(f"Error retrieving global repcap: '{name}' does not exist in the list.")
-		return self._global_repcaps[name].get_enum_value()
-
-	def _replace_global_repcaps(self, cmd: str) -> str:
-		"""Replaces all the global repcaps in the command: e.g. '<instance>' => '1'.
-		Returns the replaced command."""
-		for name, value in self._global_repcaps.items():
-			cmd_value = value.get_cmd_string_value()
-			cmd = cmd.replace(name, cmd_value)
-		return cmd
-
-	def query_opc(self) -> bool:
-		"""Sends *OPC? query and returns the result."""
-		with self._lock:
-			self.start_send_read_event('*OPC?', False)
-			opc: bool = self._session.query_opc()
-			self.end_send_read_event()
-			return opc
-
-	def query_all_syst_errors(self, include_codes=True) -> List[str]:
-		"""Returns all errors in the instrument's error queue.
-		If include_codes is False, you only get the error messages without the error codes."""
-		with self._lock:
-			self.start_send_read_event('SYST:ERROR?', False)
-			errors = self._session.query_all_syst_errors()
-			if include_codes is False and errors is not None:
-				errors = [self._parse_err_query_response(x) for x in errors]
-			self.end_send_read_event()
-			return errors
-
-	def check_status(self) -> None:
-		"""Throws InstrumentStatusException in case of an error in the instrument's error queue.
-		The procedure is skipped, if the QueryInstrumentStatus is set to false."""
-		with self._lock:
-			if not self.query_instr_status:
-				return
-			call_syst_error = self._session.error_in_error_queue() if self.stb_in_error_check else True
-			if call_syst_error:
-				errors = self.query_all_syst_errors(False)
-				InstrumentErrors.assert_no_instrument_status_errors(self.resource_name, errors)
-
-	def clear_status(self) -> None:
-		"""Clears instrument's status subsystem."""
-		with self._lock:
-			self._session.clear()
-			self._session.clear_before_read()
-
-	def reset(self) -> None:
-		"""Resets the instrument and clears its status."""
-		with self._lock:
-			self.write("*RST")
-			self.query_opc()
-			self.clear_status()
-			self.check_status()
-
-	def write(self, cmd: str) -> None:
-		"""Writes string command to the instrument."""
-		with self._lock:
-			cmd = self._replace_global_repcaps(cmd)
-			self._session.write(cmd)
-			if self.opc_query_after_write:
-				self._session.query_opc()
-			if self.on_write_handler:
-				self.send_write_str_event(cmd, False)
-			self.check_status()
-
-	def write_with_opc(self, cmd: str, timeout: int = None) -> None:
-		"""Writes a OPC-synced command.
-		Also performs error checking if the property self.query_instr_status is set to True.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			cmd = self._replace_global_repcaps(cmd)
-			self._session.write_with_opc(cmd, timeout)
-			self._session.query_and_clear_esr()
-			if self.on_write_handler:
-				self.send_write_str_event(cmd, True)
-			self.check_status()
-
-	def write_struct(self, cmd: str, struct: object) -> None:
-		"""Writes command to the instrument with the parameter composed from the entered structure."""
-		with self._lock:
-			worker = ArgStructList(struct)
-			param = worker.compose_cmd_string()
-			cmd += f' {param}'.rstrip()
-			self.write(cmd)
-
-	def write_struct_with_opc(self, cmd: str, struct: object, timeout: int = None) -> None:
-		"""Writes OPC-synced command to the instrument with the parameter composed from the entered structure.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			worker = ArgStructList(struct)
-			param = worker.compose_cmd_string()
-			cmd += f' {param}'.rstrip()
-			self.write_with_opc(cmd, timeout)
-
-	def query_str(self, query: str) -> str:
-		"""Sends a query and reads response from the instrument.
-		The response is trimmed of any trailing LF characters and has no length limit."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, False)
-			response = self._session.query_str(query)
-			self.end_send_read_event()
-			self.check_status()
-			return response
-
-	def query_str_with_opc(self, query: str, timeout: int = None) -> str:
-		"""Sends a OPC-synced query.
-		Also performs error checking if the self.query_instr_status is true.
-		The response is trimmed of any trailing LF characters and has no length limit.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, True)
-			response = self._session.query_str_with_opc(query, timeout)
-			self.end_send_read_event()
-			self._session.query_and_clear_esr()
-			self.check_status()
-			return response
-
-	def query_bin_block_to_stream(self, query: str, stream: StreamWriter) -> None:
-		"""Queries binary data block to the provided stream.
-		Use it for querying data from instrument to a variable or a file.
-		Throws an exception if the returned data was not a binary data."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, False)
-			self._session.query_bin_block(query, stream, True)
-			self.end_send_read_event()
-			self.check_status()
-
-	def query_bin_block(self, query: str) -> bytes:
-		"""Queries binary data block to bytes and returns data as bytes.
-		Throws an exception if the returned data was not a binary data."""
-		with self._lock:
-			writer = StreamWriter.as_bin_var()
-			self.query_bin_block_to_stream(query, writer)
-			return writer.content
-
-	def query_bin_block_to_file(self, cmd: str, file_path: str, append: bool = False) -> None:
-		"""Queries binary data block to the provided file.
-		If append is False, any existing file content is discarded.
-		If append is True, the new content is added to the end of the existing file, or if the file does not exit, it is created.
-		Throws an exception if the returned data was not a binary data."""
-		with self._lock:
-			with StreamWriter.as_bin_file(file_path, append) as writer:
-				self.query_bin_block_to_stream(cmd, writer)
-
-	def query_bin_block_to_stream_with_opc(self, query: str, stream: StreamWriter, timeout: int = None) -> None:
-		"""Sends a OPC-synced query and returns data the provided stream.
-		Use it for querying data from instrument to a variable or a file.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, True)
-			self._session.query_bin_block_with_opc(query, stream, True, timeout)
-			self.end_send_read_event()
-			self._session.query_and_clear_esr()
-			self.check_status()
-
-	def query_bin_block_with_opc(self, query: str, timeout: int = None) -> bytes:
-		"""Sends a OPC-synced query and returns data as bytes.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			with StreamWriter.as_bin_var() as stream:
-				self.query_bin_block_to_stream_with_opc(query, stream, timeout)
-				return stream.content
-
-	def query_bin_block_to_file_with_opc(self, cmd: str, file_path: str, append: bool = False, timeout: int = None) -> None:
-		"""Sends a OPC-synced query and writes the returned data to the provided file.
-		If append is False, any existing file content is discarded.
-		If append is True, the new content is added to the end of the existing file, or if the file does not exit, it is created.
-		Throws an exception if the returned data was not a binary data."""
-		with self._lock:
-			with StreamWriter.as_bin_file(file_path, append) as writer:
-				self.query_bin_block_to_stream_with_opc(cmd, writer, timeout)
-
-	def query_int(self, query: str) -> int:
-		"""Sends a query and reads response from the instrument as integer."""
-		with self._lock:
-			string = self.query_str(query)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return 0
-			return Conv.str_to_int(string)
-
-	def query_int_with_opc(self, query: str, timeout: int = None) -> int:
-		"""Sends a OPC-synced query and reads response from the instrument as integer number.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			string = self.query_str_with_opc(query, timeout)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return 0
-			return Conv.str_to_int(string)
-
-	def query_float(self, query: str) -> float:
-		"""Sends a query and reads response from the instrument as float number."""
-		with self._lock:
-			string = self.query_str(query)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return 0.0
-			return Conv.str_to_float(string)
-
-	def query_float_with_opc(self, query: str, timeout: int = None) -> float:
-		"""Sends a OPC-synced query and reads response from the instrument as float number.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			string = self.query_str_with_opc(query, timeout)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return 0.0
-			return Conv.str_to_float(string)
-
-	def query_bool(self, query: str) -> bool:
-		"""Sends a query and reads response from the instrument as boolean value."""
-		with self._lock:
-			string = self.query_str(query)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return False
-			return Conv.str_to_bool(string)
-
-	def query_bool_with_opc(self, query: str, timeout: int = None) -> bool:
-		"""Sends a OPC-synced query and reads response from the instrument as boolean value.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			string = self.query_str_with_opc(query, timeout)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return False
-			return Conv.str_to_bool(string)
-
-	def query_str_list(self, query: str) -> List[str]:
-		"""Sends a query and reads response from the instrument as csv-list."""
-		with self._lock:
-			string = self.query_str(query)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				string = 'AAA,BBB,CCC,DDD,EEE,FFF,GGG,HHH,III,JJJ'
-			response = [trim_str_response(x) for x in string.split(',')]
-			return response
-
-	def query_str_list_with_opc(self, query: str, timeout: int = None) -> List[str]:
-		"""Sends a OPC-synced query and reads response from the instrument as csv-list.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			string = self.query_str_with_opc(query, timeout)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				string = 'AAA,BBB,CCC,DDD,EEE,FFF,GGG,HHH,III,JJJ'
-			response = [trim_str_response(x) for x in string.split(',')]
-			return response
-
-	def write_bin_block_from_stream(self, cmd: str, stream: StreamReader) -> None:
-		"""Writes all the stream content as binary data block to the instrument.
-		Use it for writing data to instrument from a variable or a file.
-		The binary data header is added at the beginning of the transmission automatically, do not include it in the payload!!!"""
-		with self._lock:
-			if self.on_write_handler:
-				self.start_send_write_bin_event(cmd)
-			self._session.write_bin_block(cmd, stream)
-			self.end_send_write_bin_event()
-			self.check_status()
-
-	def write_bin_block(self, cmd: str, payload: bytes) -> None:
-		"""Writes all the payload as binary data block to the instrument.
-		The binary data header is added at the beginning of the transmission automatically, do not include it in the payload!!!"""
-		self.write_bin_block_from_stream(cmd, StreamReader.as_bin_var(payload))
-
-	def write_bin_block_from_file(self, cmd: str, file_path: str) -> None:
-		"""Writes all the file content as binary data block to the instrument.
-		The binary data header is added at the beginning of the transmission automatically, do not include it in the file content!!!"""
-		with StreamReader.as_bin_file(file_path) as reader:
-			self.write_bin_block_from_stream(cmd, reader)
-
-	def query_bin_or_ascii_float_list(self, query: str) -> List[float]:
-		"""Queries a list of floating-point numbers that can be returned in ASCII format or in binary format.
-		- For ASCII format, the list numbers are decoded as comma-separated values.
-		- For Binary Format, the numbers are decoded based on the property BinFloatFormat, usually float 32-bit (FORM REAL,32)."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, False)
-			stream = StreamWriter.as_bin_var()
-			self._session.query_bin_block(query, stream, False)
-			self.end_send_read_event()
-			if self._simulating and not self._session.cached_to_stream:
-				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
-			if stream.binary:
-				result = Conv.bytes_to_list_of_floats(stream.content, self.bin_float_numbers_format)
-			else:
-				result = Conv.str_to_float_list(stream.content)
-			self.check_status()
-			return result
-
-	def query_bin_or_ascii_float_list_with_opc(self, query: str, timeout: int = None) -> List[float]:
-		"""Sends a OPC-synced query and reads a list of floating-point numbers that can be returned in ASCII format or in binary format.
-		- For ASCII format, the list numbers are decoded as comma-separated values.
-		- For Binary Format, the numbers are decoded based on the property BinFloatFormat, usually float 32-bit (FORM REAL,32).
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, True)
-			stream = StreamWriter.as_bin_var()
-			self._session.query_bin_block_with_opc(query, stream, False, timeout)
-			self.end_send_read_event()
-			if self._simulating and not self._session.cached_to_stream:
-				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
-			if stream.binary:
-				result = Conv.bytes_to_list_of_floats(stream.content, self.bin_float_numbers_format)
-			else:
-				result = Conv.str_to_float_list(stream.content)
-			self._session.query_and_clear_esr()
-			self.check_status()
-			return result
-
-	def query_bin_or_ascii_float_list_suppressed(self, query: str, suppressed: ArgSingleSuppressed) -> List[float]:
-		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of floats.
-		The current implementation allows for the rest of the string to be only ASCII format."""
-		with self._lock:
-			string = self.query_str(query)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
-			response = self._linker.cut_from_response_string(suppressed, string, query)
-			return Conv.str_to_float_list(response)
-
-	def query_bin_or_ascii_float_list_suppressed_with_opc(self, query: str, suppressed: ArgSingleSuppressed, timeout: int = None) -> List[float]:
-		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of floats.
-		If you do not provide timeout, the method uses current opc_timeout.
-		The current implementation allows for the rest of the string to be only ASCII format."""
-		with self._lock:
-			string = self.query_str_with_opc(query, timeout)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
-			response = self._linker.cut_from_response_string(suppressed, string, query)
-			return Conv.str_to_float_list(response)
-
-	def query_bin_or_ascii_int_list(self, query: str) -> List[int]:
-		"""Queries a list of integer numbers that can be returned in ASCII format or in binary format.
-		- For ASCII format, the list numbers are decoded as comma-separated values.
-		- For Binary Format, the numbers are decoded based on the property BinIntFormat, usually int 32-bit (FORM REAL,32)."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, False)
-			stream = StreamWriter.as_bin_var()
-			self._session.query_bin_block(query, stream, False)
-			self.end_send_read_event()
-			if self._simulating and not self._session.cached_to_stream:
-				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
-			if stream.binary:
-				result = Conv.bytes_to_list_of_integers(stream.content, self.bin_int_numbers_format)
-			else:
-				result = Conv.str_to_int_list(stream.content)
-			self.check_status()
-			return result
-
-	def query_bin_or_ascii_int_list_with_opc(self, query: str, timeout: int = None) -> List[int]:
-		"""Sends a OPC-synced query and reads a list of integer numbers that can be returned in ASCII format or in binary format.
-		- For ASCII format, the list numbers are decoded as comma-separated values.
-		- For Binary Format, the numbers are decoded based on the property BinIntFormat, usually int 32-bit (FORM REAL,32).
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, True)
-			stream = StreamWriter.as_bin_var()
-			self._session.query_bin_block_with_opc(query, stream, False, timeout)
-			self.end_send_read_event()
-			if self._simulating and not self._session.cached_to_stream:
-				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
-			if stream.binary:
-				result = Conv.bytes_to_list_of_integers(stream.content, self.bin_int_numbers_format)
-			else:
-				result = Conv.str_to_int_list(stream.content)
-			self._session.query_and_clear_esr()
-			self.check_status()
-			return result
-
-	def query_bin_or_ascii_int_list_suppressed(self, query: str, suppressed: ArgSingleSuppressed) -> List[int]:
-		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of integers.
-		The current implementation allows for the rest of the string to be only ASCII format."""
-		with self._lock:
-			response = self.query_str(query)
-			if self._simulating:
-				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
-			response = self._linker.cut_from_response_string(suppressed, response, query)
-			return Conv.str_to_int_list(response)
-
-	def query_bin_or_ascii_int_list_suppressed_with_opc(self, query: str, suppressed: ArgSingleSuppressed, timeout: int = None) -> List[int]:
-		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of integers.
-		If you do not provide timeout, the method uses current opc_timeout.
-		The current implementation allows for the rest of the string to be only ASCII format."""
-		with self._lock:
-			response = self.query_str_with_opc(query, timeout)
-			if self._simulating:
-				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
-			response = self._linker.cut_from_response_string(suppressed, response, query)
-			return Conv.str_to_int_list(response)
-
-	def query_struct(self, query: str, struct: object) -> object:
-		"""Queries string of from instrument, and parses it based on the provided structure object.
-		THe method returns the copy of the entered object that it had modified."""
-		with self._lock:
-			string = self.query_str(query)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return struct
-			struct_list = ArgStructList(struct)
-			struct_list.parse_from_cmd_response(string)
-			self._linker.invoke_struct_intern_links(struct, struct_list.args, query)
-			return struct
-
-	def query_str_suppressed(self, query: str, suppressed: ArgSingleSuppressed) -> str:
-		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument."""
-		with self._lock:
-			string = self.query_str(query)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return string
-			response = self._linker.cut_from_response_string(suppressed, string, query)
-			return response
-
-	def self_test(self, timeout: int = None) -> Tuple[int, str]:
-		"""Performs instrument's selftest (*TST?).
-		Returns tuple (code:int, message: str). . Code 0 means the self-test passed.
-		You can define the custom timeout in milliseconds. If you do not define it, the default selftest timeout is used (usually 60 secs)."""
-		with self._lock:
-			if timeout is None or timeout == 0:
-				timeout = self.selftest_timeout
-			response = self.query_str_with_opc('*TST?', timeout)
-			m = re.search(r'^(-?[\d]+)(,(.*))?', response)
-			if not m:
-				raise InstrumentErrors.UnexpectedResponseException(self.resource_name, f"Unexpected response to a '*TST?' self-test query: '{response}'")
-			code = Conv.str_to_int(m.group(1))
-			msg = Utilities.trim_str_response(m.group(3))
-			self.check_status()
-			return code, msg
-
-	def get_session_handle(self) -> object:
-		"""Returns the underlying pyvisa session."""
-		return self._session.get_session_handle()
-
-	def close(self) -> None:
-		"""Closes the Instrument session."""
-		with self._lock:
-			self._session.close()
-			self._session = None
-
-	# Events part
-
-	@property
-	def io_events_include_data(self) -> bool:
-		"""If true, the read and write handlers also include read and written data."""
-		return self._io_events_include_data
-
-	@io_events_include_data.setter
-	def io_events_include_data(self, value: bool) -> None:
-		"""If true, the read and write handlers also include read and written data."""
-		self._io_events_include_data = value
-		self._session.io_events_include_data = value
-
-	def event_args_append_instr_info(self, args: IoTransferEventArgs) -> IoTransferEventArgs:
-		"""Appends instrument-related information to the read/write event argument"""
-		args.chunk_size = self.data_chunk_size
-		args.resource_name = self.resource_name
-		return args
-
-	def send_write_str_event(self, cmd: str, opc_sync: bool) -> None:
-		"""Creates and sends write string event. The transfer is marked as done (end_of_transfer = True)."""
-		args = IoTransferEventArgs.write_str(opc_sync, len(cmd), cmd)
-		args.transferred_size = args.total_size
-		args.chunk_ix = 0
-		args.end_of_transfer = True
-		args = self.event_args_append_instr_info(args)
-		if self._io_events_include_data:
-			args.data = cmd
-		self.on_write_handler(args)
-
-	def start_send_read_event(self, query: str, opc_sync: bool) -> None:
-		"""Registers VisaSession.on_read_chunk_handler() which then generates events with each chunk transfer.
-		Event handler for these events is the local function of this method, which sends IoTransferEventArgs further up to the Instrument.on_read_handler()"""
-		if not self.on_read_handler:
-			return
-
-		def _read_chunk_handler(visa_args: EventArgsChunk) -> None:
-			"""Receives events from VisaSession on read chunk transfers, and sends them as IoTransferEventArgs to the Instrument.on_read_handler()"""
-			args.end_of_transfer = visa_args.end_of_transfer
-			args.chunk_ix = visa_args.chunk_ix
-			args.total_chunks = visa_args.total_chunks
-			args.chunk_size = visa_args.chunk_size
-			args.transferred_size = visa_args.transferred_size
-			args.total_size = visa_args.total_size
-			args.data = visa_args.data
-			args.binary = visa_args.binary
-			self.on_read_handler(args)
-
-		args = IoTransferEventArgs.read_chunk(opc_sync, query)
-		args = self.event_args_append_instr_info(args)
-		self._session.on_read_chunk_handler = _read_chunk_handler
-
-	def end_send_read_event(self):
-		"""Unregisters VisaSession.on_read_chunk_handler()"""
-		self._session.on_read_chunk_handler = None
-
-	def start_send_write_bin_event(self, cmd: str) -> None:
-		"""Registers VisaSession.on_write_chunk_handler() which then generates events with each chunk transfer.
-		Event handler for these events is the local function of this method, which sends IoTransferEventArgs further up to the Instrument.on_write_handler()"""
-		if not self.on_write_handler:
-			return
-
-		def _write_chunk_handler(visa_args: EventArgsChunk) -> None:
-			"""Receives events from VisaSession on write chunk transfers, and sends them as IoTransferEventArgs to the Instrument.on_write_handler()"""
-			args.end_of_transfer = visa_args.end_of_transfer
-			args.chunk_ix = visa_args.chunk_ix
-			args.total_chunks = visa_args.total_chunks
-			args.chunk_size = visa_args.chunk_size
-			args.transferred_size = visa_args.transferred_size
-			args.total_size = visa_args.total_size
-			args.data = visa_args.data
-			args.binary = visa_args.binary
-			self.on_write_handler(args)
-
-		args = IoTransferEventArgs.write_bin(cmd)
-		args = self.event_args_append_instr_info(args)
-		self._session.on_write_chunk_handler = _write_chunk_handler
-
-	def end_send_write_bin_event(self):
-		"""Unregisters VisaSession.on_write_chunk_handler()"""
-		self._session.on_write_chunk_handler = None
+import re
+import threading
+from enum import Enum
+from typing import List, Callable, Tuple, Dict
+
+from . import Utilities, InstrumentSettings, InstrumentOptions, InstrumentErrors, Conversions as Conv
+from .ArgSingleSuppressed import ArgSingleSuppressed
+from .ArgStructList import ArgStructList
+from .InternalLinker import InternalLinker
+from .IoTransferEventArgs import IoTransferEventArgs
+from .StreamReader import StreamReader
+from .StreamWriter import StreamWriter
+from .Utilities import trim_str_response
+from .VisaSession import VisaSession, EventArgsChunk
+from .VisaSessionSim import VisaSessionSim
+from .RepeatedCapability import RepeatedCapability
+
+
+class Instrument(object):
+	"""Model of an Instrument with VISA interface."""
+
+	def __init__(self, resource_name: str, simulate: bool, settings: InstrumentSettings, direct_session=None):
+		"""Opening an instrument session.
+		If simulate is true, it cannot be later switched to false anymore."""
+		self._simulating: bool = simulate
+		self._session = None
+		self._global_repcaps: Dict[str, RepeatedCapability] = {}
+		self._linker = InternalLinker()
+		# noinspection PyTypeChecker
+		self.on_write_handler: Callable = None
+		# noinspection PyTypeChecker
+		self.on_read_handler: Callable = None
+		self._io_events_include_data: bool = False
+		self._lock = None
+		self._before_query_handler = None
+		self._before_write_handler = None
+
+		# Fixed settings
+		self.selftest_timeout = 100000 if settings.selftest_timeout == 0 else settings.selftest_timeout
+		self.idn_model_full_name = settings.idn_model_full_name
+		self.instr_options_parse_mode = settings.instr_options_parse_mode
+
+		# Changeable settings
+		self.resource_name: str = resource_name
+		self._instr_options: InstrumentOptions = None  # Internal private property for the lazy property self.instr_options - see the getter for self.instr_options. Initialized by the first access
+		self.query_instr_status: bool = True
+		self.opc_query_after_write: bool = False
+		self.bin_float_numbers_format = settings.bin_float_numbers_format
+		self.bin_int_numbers_format = settings.bin_int_numbers_format
+		self.opc_query_after_write: bool = settings.opc_query_after_write
+		self.stb_in_error_check: bool = settings.stb_in_error_check
+
+		self.manufacturer: str = 'Rohde&Schwarz'
+		self.model: str = 'R&S Instrument'
+		self.serial_number: str = '100001'
+		self.firmware_version: str = '1.00'
+
+		if self._simulating:
+			self._session = VisaSessionSim(resource_name, settings, direct_session)
+			self._lock = self._session.get_lock()
+			self._instr_options = InstrumentOptions.Options('K0', InstrumentOptions.ParseMode.KeepOriginal)
+			self._session.write('*OPT K0')
+			return
+
+		self._session = VisaSession(resource_name, settings, direct_session)
+		self._lock = self._session.get_lock()
+		with self._lock:
+			self._session.clear_before_read()
+			self.idn_string = Utilities.trim_str_response(self._session.query_str('*IDN?')).strip()
+
+			# NRP-Z session coercing
+			if self._session.is_rsnrp_session():
+				settings.instr_options_parse_mode = InstrumentOptions.ParseMode.Skip
+				self.stb_in_error_check = False
+			self.instr_options_parse_mode = settings.instr_options_parse_mode
+
+	def __str__(self):
+		if self._simulating:
+			return f"Simulated, Model: '{self.model}', ResourceName: '{self.resource_name}'"
+		else:
+			return f"Instrument Model: '{self.model}', ResourceName: '{self.resource_name}'"
+
+	def set_simulating_cmds(self) -> None:
+		"""Updated cached values in the simulating VISA session to properly respond to *IDN? or *OPT?"""
+		if self._simulating:
+			self.write(f'*idn {self.idn_string}')
+			self.write(f'*opt {Conv.list_to_csv_str(self.instr_options.get_all())}')
+			self.write(f'*opc 1')
+			self.write(f'*stb 0')
+			self.write(f'*tst 0,"Passed"')
+			self.write(f'syst:err 0,"No Error"')
+			self.write(f'system:error 0,"No Error"')
+
+	def get_last_sent_cmd(self) -> str:
+		"""Returns the last commands sent to the instrument. Only works in simulation mode"""
+		if self._simulating:
+			# noinspection PyUnresolvedReferences
+			return self._session.get_last_sent_cmd()
+		raise Exception('get_last_sent_cmd() can only be used in simulation mode')
+
+	def assign_lock(self, lock: threading.RLock) -> None:
+		"""Assigns the thread lock provided from by the user. Trickles down to the VisaSession."""
+		self._lock = lock
+		self._session.assign_lock(lock)
+
+	def get_lock(self) -> threading.RLock:
+		"""Returns the current RLock object."""
+		return self._lock
+
+	def clear_lock(self):
+		"""Clears the existing thread lock, making the current session thread-independent from others that might share the current thread lock."""
+		self.assign_lock(threading.RLock())
+
+	@property
+	def visa_manufacturer(self) -> str:
+		"""Returns the visa manufacturer of the current session."""
+		return self._session.manufacturer
+
+	def set_link_handler(self, link_name: str, handler: Callable) -> Callable:
+		"""Adds / Updates link handler for the entered link_name.
+		Handler API: handler(event_args: ArgLinkedEventArgs)
+		Returns the previous registered handler, or None if no handler was registered before."""
+		return self._linker.set_handler(link_name, handler)
+
+	def del_link_handler(self, link_name: str) -> Callable:
+		"""Deletes link handler for the link_name.
+		Returns the deleted handler, or None if none existed."""
+		return self._linker.del_handler(link_name)
+
+	def del_all_link_handlers(self) -> int:
+		"""Deletes all the link handlers.
+		Returns number of deleted links."""
+		return self._linker.del_all_handlers()
+
+	@property
+	def idn_string(self) -> str:
+		return self._idn_string
+
+	@idn_string.setter
+	def idn_string(self, value: str) -> None:
+		"""IDN string. Set it to force a different IDN string than the default *IDN? response."""
+		self._idn_string = value
+		self._parse_idn_string(self._idn_string)
+
+	@property
+	def instr_options(self) -> InstrumentOptions:
+		"""Public getter for the lazy property instr_options"""
+		if self._instr_options is None:
+			self._query_options_and_parse(self.instr_options_parse_mode)
+		return self._instr_options
+
+	@property
+	def opc_timeout(self) -> int:
+		"""See the opc_timeout.setter."""
+		return self._session.opc_timeout
+
+	@opc_timeout.setter
+	def opc_timeout(self, value: int) -> None:
+		"""Sets / Gets timeout in milliseconds for all the operations that use OPC synchronization."""
+		self._session.opc_timeout = value
+
+	@property
+	def visa_timeout(self) -> int:
+		"""See the visa_timeout.setter."""
+		return self._session.visa_timeout
+
+	@visa_timeout.setter
+	def visa_timeout(self, value: int) -> None:
+		"""Sets / Gets visa IO timeout in milliseconds."""
+		self._session.visa_timeout = value
+
+	@property
+	def data_chunk_size(self) -> int:
+		"""Returns max chunk size of one data block."""
+		return self._session.data_chunk_size
+
+	@data_chunk_size.setter
+	def data_chunk_size(self, chunk_size: int) -> None:
+		"""Sets the maximum size of one block transferred during write/read operations."""
+		self._session.data_chunk_size = int(chunk_size)
+
+	# noinspection PyMethodMayBeStatic
+	def _sim_cached_value_found(self, value) -> bool:
+		return value != 'Simulating'
+
+	# noinspection PyMethodMayBeStatic
+	def _sim_cached_value_not_found(self, value) -> bool:
+		return value == 'Simulating'
+
+	def _parse_idn_string(self, idn_string: str) -> None:
+		"""Parse the *IDN? response to:
+		- Manufacturer
+		- Model
+		- SerialNumber
+		- FirmwareRevision"""
+		idn_string = idn_string.strip()
+		m = re.search(r'([\w& ]+),([a-zA-Z ]+)([\-0-9a-zA-Z ]*),([^,]+),([\w .\-/]+)', idn_string)
+		if not m:
+			raise Exception(f"The instrument *IDN? string parsing failed. Parsed *IDN? response: '{idn_string}'")
+		self.manufacturer = m.group(1).strip()
+		self.model = m.group(2).strip()
+		self.full_model_name = self.model + m.group(3).strip()
+		self.serial_number = m.group(4).strip()
+		self.firmware_version = m.group(5).strip()
+		if self.idn_model_full_name:
+			self.model = self.full_model_name
+
+	def fits_idn_pattern(self, patterns: List[str], supported_models: List[str]) -> None:
+		"""Throws exception if the current instrument model does not fit  any of the patterns.
+		The supported_models argument is only used for exception messages"""
+		matches = False
+		assert self._idn_string, f'*IDN? was not assigned yet.'
+		for x in patterns:
+			matches = re.search(x, self.idn_string, re.IGNORECASE)
+			if matches:
+				break
+		if not matches:
+			message = f"Instrument is not supported.\n*IDN? string: '{self.idn_string}'"
+			if len(supported_models) > 0:
+				message += f"\nSupported models: '{', '.join(supported_models)}'"
+			if len(patterns) == 1:
+				message += f"\nSupported IDN pattern: '{patterns[0]}'"
+			if len(patterns) > 1:
+				message += "\nSupported IDN patterns:\n" + '\n'.join(patterns)
+			raise InstrumentErrors.UnexpectedResponseException(self.resource_name, message)
+
+	def _query_options_and_parse(self, mode: InstrumentOptions.ParseMode) -> None:
+		"""Queries *OPT? and parses it based on the ParseMode."""
+		if mode == InstrumentOptions.ParseMode.Skip:
+			self._instr_options = InstrumentOptions.Options('', mode)
+			return
+		if self._simulating is False:
+			with self._lock:
+				opts = self._session.query_str_no_tout_err('*OPT?', 1000)
+				if opts is None:
+					opts = 'Cannot read the instrument options - *OPT? query is not supported'
+				self._instr_options = InstrumentOptions.Options(opts, mode)
+
+	@staticmethod
+	def _parse_err_query_response(response: str) -> str:
+		"""Parses entered response string to string error message without the error code.
+		E.g.: response = '-110,"Command error"' returns: 'Command error'."""
+		m = re.match(r'(-?[\d]+).*?"(.*)"', response)
+		if m:
+			return m.group(2)
+		else:
+			return response
+
+	def add_global_repcap(self, name: str, rep_cap: RepeatedCapability) -> None:
+		"""Adds the global repcap name to the list of global repcaps
+		and sets its value to the provided default value."""
+		if name in self._global_repcaps:
+			raise Exception(f"Error adding new global repcap: '{name}' already exists in the list.")
+		self._global_repcaps[name] = rep_cap
+
+	def set_global_repcap_value(self, name: str, enum_value: Enum) -> None:
+		"""Updates the existing global repcap value as enum"""
+		if name not in self._global_repcaps:
+			raise Exception(f"Error updating global repcap: '{name}' does not exist in the list.")
+		self._global_repcaps[name].set_enum_value(enum_value)
+
+	def get_global_repcap_value(self, name: str) -> Enum:
+		"""Returns the current global repcap value as enum"""
+		if name not in self._global_repcaps:
+			raise Exception(f"Error retrieving global repcap: '{name}' does not exist in the list.")
+		return self._global_repcaps[name].get_enum_value()
+
+	def _replace_global_repcaps(self, cmd: str) -> str:
+		"""Replaces all the global repcaps in the command: e.g. '<instance>' => '1'.
+		Returns the replaced command."""
+		for name, value in self._global_repcaps.items():
+			cmd_value = value.get_cmd_string_value()
+			cmd = cmd.replace(name, cmd_value)
+		return cmd
+
+	def query_opc(self, timeout: int = 0) -> bool:
+		"""Sends *OPC? query and returns the result.
+		If you define timeout > 0, the VISA timeout is set to that value just for this method call."""
+		with self._lock:
+			self.start_send_read_event('*OPC?', False)
+			opc: bool = self._session.query_opc(timeout)
+			self.end_send_read_event()
+			return opc
+
+	def query_all_syst_errors(self, include_codes=True) -> List[str]:
+		"""Returns all errors in the instrument's error queue.
+		If include_codes is False, you only get the error messages without the error codes."""
+		with self._lock:
+			self.start_send_read_event('SYST:ERROR?', False)
+			errors = self._session.query_all_syst_errors()
+			if include_codes is False and errors is not None:
+				errors = [self._parse_err_query_response(x) for x in errors]
+			self.end_send_read_event()
+			return errors
+
+	def check_status(self) -> None:
+		"""Throws InstrumentStatusException in case of an error in the instrument's error queue.
+		The procedure is skipped, if the QueryInstrumentStatus is set to false."""
+		with self._lock:
+			if not self.query_instr_status:
+				return
+			call_syst_error = self._session.error_in_error_queue() if self.stb_in_error_check else True
+			if call_syst_error:
+				errors = self.query_all_syst_errors(False)
+				InstrumentErrors.assert_no_instrument_status_errors(self.resource_name, errors)
+
+	def clear_status(self) -> None:
+		"""Clears instrument's status subsystem."""
+		with self._lock:
+			self._session.clear()
+			self._session.clear_before_read()
+
+	def reset(self) -> None:
+		"""Resets the instrument and clears its status."""
+		with self._lock:
+			self.write('*RST', True)
+			self.query_opc()
+			self.clear_status()
+			self.check_status()
+
+	def write(self, cmd: str, block_callback: bool = False) -> None:
+		"""Writes string command to the instrument."""
+		with self._lock:
+			cmd = self._replace_global_repcaps(cmd)
+			self._call_before_write_handler(cmd, block_callback)
+			self._session.write(cmd)
+			if self.opc_query_after_write:
+				self._session.query_opc()
+			if self.on_write_handler:
+				self.send_write_str_event(cmd, False)
+			self.check_status()
+
+	def write_with_opc(self, cmd: str, timeout: int = None, block_callback: bool = False) -> None:
+		"""Writes a OPC-synced command.
+		Also performs error checking if the property self.query_instr_status is set to True.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		with self._lock:
+			cmd = self._replace_global_repcaps(cmd)
+			self._call_before_write_handler(cmd, block_callback)
+			self._session.write_with_opc(cmd, timeout)
+			self._session.query_and_clear_esr()
+			if self.on_write_handler:
+				self.send_write_str_event(cmd, True)
+			self.check_status()
+
+	def write_struct(self, cmd: str, struct: object) -> None:
+		"""Writes command to the instrument with the parameter composed from the entered structure."""
+		with self._lock:
+			worker = ArgStructList(struct)
+			param = worker.compose_cmd_string()
+			cmd += f' {param}'.rstrip()
+			self.write(cmd)
+
+	def write_struct_with_opc(self, cmd: str, struct: object, timeout: int = None) -> None:
+		"""Writes OPC-synced command to the instrument with the parameter composed from the entered structure.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		with self._lock:
+			worker = ArgStructList(struct)
+			param = worker.compose_cmd_string()
+			cmd += f' {param}'.rstrip()
+			self.write_with_opc(cmd, timeout)
+
+	def query_str(self, query: str, block_callback: bool = False) -> str:
+		"""Sends a query and reads response from the instrument.
+		The response is trimmed of any trailing LF characters and has no length limit."""
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, False)
+			self._call_pre_query_handler(query, block_callback)
+			response = self._session.query_str(query)
+			self.end_send_read_event()
+			self.check_status()
+			return response
+
+	def query_str_with_opc(self, query: str, timeout: int = None, block_callback: bool = False) -> str:
+		"""Sends a OPC-synced query.
+		Also performs error checking if the self.query_instr_status is true.
+		The response is trimmed of any trailing LF characters and has no length limit.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, True)
+			self._call_pre_query_handler(query, block_callback)
+			response = self._session.query_str_with_opc(query, timeout)
+			self.end_send_read_event()
+			self._session.query_and_clear_esr()
+			self.check_status()
+			return response
+
+	def query_bin_block_to_stream(self, query: str, stream: StreamWriter) -> None:
+		"""Queries binary data block to the provided stream.
+		Use it for querying data from instrument to a variable or a file.
+		Throws an exception if the returned data was not a binary data."""
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, False)
+			self._call_pre_query_handler(query, False)
+			self._session.query_bin_block(query, stream, True)
+			self.end_send_read_event()
+			self.check_status()
+
+	def query_bin_block(self, query: str) -> bytes:
+		"""Queries binary data block to bytes and returns data as bytes.
+		Throws an exception if the returned data was not a binary data."""
+		with self._lock:
+			writer = StreamWriter.as_bin_var()
+			self.query_bin_block_to_stream(query, writer)
+			return writer.content
+
+	def query_bin_block_to_file(self, cmd: str, file_path: str, append: bool = False) -> None:
+		"""Queries binary data block to the provided file.
+		If append is False, any existing file content is discarded.
+		If append is True, the new content is added to the end of the existing file, or if the file does not exit, it is created.
+		Throws an exception if the returned data was not a binary data."""
+		with self._lock:
+			with StreamWriter.as_bin_file(file_path, append) as writer:
+				self.query_bin_block_to_stream(cmd, writer)
+
+	def query_bin_block_to_stream_with_opc(self, query: str, stream: StreamWriter, timeout: int = None) -> None:
+		"""Sends a OPC-synced query and returns data the provided stream.
+		Use it for querying data from instrument to a variable or a file.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, True)
+			self._call_pre_query_handler(query, False)
+			self._session.query_bin_block_with_opc(query, stream, True, timeout)
+			self.end_send_read_event()
+			self._session.query_and_clear_esr()
+			self.check_status()
+
+	def query_bin_block_with_opc(self, query: str, timeout: int = None) -> bytes:
+		"""Sends a OPC-synced query and returns data as bytes.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		with self._lock:
+			with StreamWriter.as_bin_var() as stream:
+				self.query_bin_block_to_stream_with_opc(query, stream, timeout)
+				return stream.content
+
+	def query_bin_block_to_file_with_opc(self, cmd: str, file_path: str, append: bool = False, timeout: int = None) -> None:
+		"""Sends a OPC-synced query and writes the returned data to the provided file.
+		If append is False, any existing file content is discarded.
+		If append is True, the new content is added to the end of the existing file, or if the file does not exit, it is created.
+		Throws an exception if the returned data was not a binary data."""
+		with self._lock:
+			with StreamWriter.as_bin_file(file_path, append) as writer:
+				self.query_bin_block_to_stream_with_opc(cmd, writer, timeout)
+
+	def query_int(self, query: str) -> int:
+		"""Sends a query and reads response from the instrument as integer."""
+		with self._lock:
+			string = self.query_str(query)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return 0
+			return Conv.str_to_int(string)
+
+	def query_int_with_opc(self, query: str, timeout: int = None) -> int:
+		"""Sends a OPC-synced query and reads response from the instrument as integer number.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		with self._lock:
+			string = self.query_str_with_opc(query, timeout)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return 0
+			return Conv.str_to_int(string)
+
+	def query_float(self, query: str) -> float:
+		"""Sends a query and reads response from the instrument as float number."""
+		with self._lock:
+			string = self.query_str(query)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return 0.0
+			return Conv.str_to_float(string)
+
+	def query_float_with_opc(self, query: str, timeout: int = None) -> float:
+		"""Sends a OPC-synced query and reads response from the instrument as float number.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		with self._lock:
+			string = self.query_str_with_opc(query, timeout)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return 0.0
+			return Conv.str_to_float(string)
+
+	def query_bool(self, query: str) -> bool:
+		"""Sends a query and reads response from the instrument as boolean value."""
+		with self._lock:
+			string = self.query_str(query)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return False
+			return Conv.str_to_bool(string)
+
+	def query_bool_with_opc(self, query: str, timeout: int = None) -> bool:
+		"""Sends a OPC-synced query and reads response from the instrument as boolean value.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		with self._lock:
+			string = self.query_str_with_opc(query, timeout)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return False
+			return Conv.str_to_bool(string)
+
+	def query_str_list(self, query: str) -> List[str]:
+		"""Sends a query and reads response from the instrument as csv-list."""
+		with self._lock:
+			string = self.query_str(query)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				string = 'AAA,BBB,CCC,DDD,EEE,FFF,GGG,HHH,III,JJJ'
+			response = [trim_str_response(x) for x in string.split(',')]
+			return response
+
+	def query_str_list_with_opc(self, query: str, timeout: int = None) -> List[str]:
+		"""Sends a OPC-synced query and reads response from the instrument as csv-list.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		with self._lock:
+			string = self.query_str_with_opc(query, timeout)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				string = 'AAA,BBB,CCC,DDD,EEE,FFF,GGG,HHH,III,JJJ'
+			response = [trim_str_response(x) for x in string.split(',')]
+			return response
+
+	def write_bin_block_from_stream(self, cmd: str, stream: StreamReader) -> None:
+		"""Writes all the stream content as binary data block to the instrument.
+		Use it for writing data to instrument from a variable or a file.
+		The binary data header is added at the beginning of the transmission automatically, do not include it in the payload!!!"""
+		with self._lock:
+			if self.on_write_handler:
+				self.start_send_write_bin_event(cmd)
+			self._call_pre_query_handler(cmd, False)
+			self._session.write_bin_block(cmd, stream)
+			self.end_send_write_bin_event()
+			self.check_status()
+
+	def write_bin_block(self, cmd: str, payload: bytes) -> None:
+		"""Writes all the payload as binary data block to the instrument.
+		The binary data header is added at the beginning of the transmission automatically, do not include it in the payload!!!"""
+		self.write_bin_block_from_stream(cmd, StreamReader.as_bin_var(payload))
+
+	def write_bin_block_from_file(self, cmd: str, file_path: str) -> None:
+		"""Writes all the file content as binary data block to the instrument.
+		The binary data header is added at the beginning of the transmission automatically, do not include it in the file content!!!"""
+		with StreamReader.as_bin_file(file_path) as reader:
+			self.write_bin_block_from_stream(cmd, reader)
+
+	def query_bin_or_ascii_float_list(self, query: str) -> List[float]:
+		"""Queries a list of floating-point numbers that can be returned in ASCII format or in binary format.
+		- For ASCII format, the list numbers are decoded as comma-separated values.
+		- For Binary Format, the numbers are decoded based on the property BinFloatFormat, usually float 32-bit (FORM REAL,32)."""
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, False)
+			stream = StreamWriter.as_bin_var()
+			self._call_pre_query_handler(query, False)
+			self._session.query_bin_block(query, stream, False)
+			self.end_send_read_event()
+			if self._simulating and not self._session.cached_to_stream:
+				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
+			if stream.binary:
+				result = Conv.bytes_to_list_of_floats(stream.content, self.bin_float_numbers_format)
+			else:
+				result = Conv.str_to_float_list(stream.content)
+			self.check_status()
+			return result
+
+	def query_bin_or_ascii_float_list_with_opc(self, query: str, timeout: int = None) -> List[float]:
+		"""Sends a OPC-synced query and reads a list of floating-point numbers that can be returned in ASCII format or in binary format.
+		- For ASCII format, the list numbers are decoded as comma-separated values.
+		- For Binary Format, the numbers are decoded based on the property BinFloatFormat, usually float 32-bit (FORM REAL,32).
+		If you do not provide timeout, the method uses current opc_timeout."""
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, True)
+			stream = StreamWriter.as_bin_var()
+			self._call_pre_query_handler(query, False)
+			self._session.query_bin_block_with_opc(query, stream, False, timeout)
+			self.end_send_read_event()
+			if self._simulating and not self._session.cached_to_stream:
+				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
+			if stream.binary:
+				result = Conv.bytes_to_list_of_floats(stream.content, self.bin_float_numbers_format)
+			else:
+				result = Conv.str_to_float_list(stream.content)
+			self._session.query_and_clear_esr()
+			self.check_status()
+			return result
+
+	def query_bin_or_ascii_float_list_suppressed(self, query: str, suppressed: ArgSingleSuppressed) -> List[float]:
+		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of floats.
+		The current implementation allows for the rest of the string to be only ASCII format."""
+		with self._lock:
+			string = self.query_str(query)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
+			response = self._linker.cut_from_response_string(suppressed, string, query)
+			return Conv.str_to_float_list(response)
+
+	def query_bin_or_ascii_float_list_suppressed_with_opc(self, query: str, suppressed: ArgSingleSuppressed, timeout: int = None) -> List[float]:
+		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of floats.
+		If you do not provide timeout, the method uses current opc_timeout.
+		The current implementation allows for the rest of the string to be only ASCII format."""
+		with self._lock:
+			string = self.query_str_with_opc(query, timeout)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
+			response = self._linker.cut_from_response_string(suppressed, string, query)
+			return Conv.str_to_float_list(response)
+
+	def query_bin_or_ascii_int_list(self, query: str) -> List[int]:
+		"""Queries a list of integer numbers that can be returned in ASCII format or in binary format.
+		- For ASCII format, the list numbers are decoded as comma-separated values.
+		- For Binary Format, the numbers are decoded based on the property BinIntFormat, usually int 32-bit (FORM REAL,32)."""
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, False)
+			stream = StreamWriter.as_bin_var()
+			self._call_pre_query_handler(query, False)
+			self._session.query_bin_block(query, stream, False)
+			self.end_send_read_event()
+			if self._simulating and not self._session.cached_to_stream:
+				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
+			if stream.binary:
+				result = Conv.bytes_to_list_of_integers(stream.content, self.bin_int_numbers_format)
+			else:
+				result = Conv.str_to_int_list(stream.content)
+			self.check_status()
+			return result
+
+	def query_bin_or_ascii_int_list_with_opc(self, query: str, timeout: int = None) -> List[int]:
+		"""Sends a OPC-synced query and reads a list of integer numbers that can be returned in ASCII format or in binary format.
+		- For ASCII format, the list numbers are decoded as comma-separated values.
+		- For Binary Format, the numbers are decoded based on the property BinIntFormat, usually int 32-bit (FORM REAL,32).
+		If you do not provide timeout, the method uses current opc_timeout."""
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, True)
+			stream = StreamWriter.as_bin_var()
+			self._call_pre_query_handler(query, False)
+			self._session.query_bin_block_with_opc(query, stream, False, timeout)
+			self.end_send_read_event()
+			if self._simulating and not self._session.cached_to_stream:
+				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
+			if stream.binary:
+				result = Conv.bytes_to_list_of_integers(stream.content, self.bin_int_numbers_format)
+			else:
+				result = Conv.str_to_int_list(stream.content)
+			self._session.query_and_clear_esr()
+			self.check_status()
+			return result
+
+	def query_bin_or_ascii_int_list_suppressed(self, query: str, suppressed: ArgSingleSuppressed) -> List[int]:
+		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of integers.
+		The current implementation allows for the rest of the string to be only ASCII format."""
+		with self._lock:
+			response = self.query_str(query)
+			if self._simulating:
+				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
+			response = self._linker.cut_from_response_string(suppressed, response, query)
+			return Conv.str_to_int_list(response)
+
+	def query_bin_or_ascii_int_list_suppressed_with_opc(self, query: str, suppressed: ArgSingleSuppressed, timeout: int = None) -> List[int]:
+		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of integers.
+		If you do not provide timeout, the method uses current opc_timeout.
+		The current implementation allows for the rest of the string to be only ASCII format."""
+		with self._lock:
+			response = self.query_str_with_opc(query, timeout)
+			if self._simulating:
+				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
+			response = self._linker.cut_from_response_string(suppressed, response, query)
+			return Conv.str_to_int_list(response)
+
+	def query_struct(self, query: str, struct: object) -> object:
+		"""Queries string of from instrument, and parses it based on the provided structure object.
+		THe method returns the copy of the entered object that it had modified."""
+		with self._lock:
+			string = self.query_str(query)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return struct
+			struct_list = ArgStructList(struct)
+			struct_list.parse_from_cmd_response(string)
+			self._linker.invoke_struct_intern_links(struct, struct_list.args, query)
+			return struct
+
+	def query_struct_with_opc(self, query: str, struct: object, timeout: int = None) -> object:
+		"""Queries string of from instrument, and parses it based on the provided structure object.
+		THe method returns the copy of the entered object that it had modified."""
+		with self._lock:
+			string = self.query_str_with_opc(query, timeout)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return struct
+			struct_list = ArgStructList(struct)
+			struct_list.parse_from_cmd_response(string)
+			self._linker.invoke_struct_intern_links(struct, struct_list.args, query)
+			return struct
+
+	def query_str_suppressed(self, query: str, suppressed: ArgSingleSuppressed) -> str:
+		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument."""
+		with self._lock:
+			string = self.query_str(query)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return string
+			response = self._linker.cut_from_response_string(suppressed, string, query)
+			return response
+
+	def query_str_suppressed_with_opc(self, query: str, suppressed: ArgSingleSuppressed, timeout: int = None) -> str:
+		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument."""
+		with self._lock:
+			string = self.query_str_with_opc(query, timeout)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return string
+			response = self._linker.cut_from_response_string(suppressed, string, query)
+			return response
+
+	def self_test(self, timeout: int = None) -> Tuple[int, str]:
+		"""Performs instrument's selftest (*TST?).
+		Returns tuple (code:int, message: str). . Code 0 means the self-test passed.
+		You can define the custom timeout in milliseconds. If you do not define it, the default selftest timeout is used (usually 60 secs)."""
+		with self._lock:
+			if timeout is None or timeout == 0:
+				timeout = self.selftest_timeout
+			response = self.query_str_with_opc('*TST?', timeout)
+			m = re.search(r'^(-?[\d]+)(,(.*))?', response)
+			if not m:
+				raise InstrumentErrors.UnexpectedResponseException(self.resource_name, f"Unexpected response to a '*TST?' self-test query: '{response}'")
+			code = Conv.str_to_int(m.group(1))
+			msg = Utilities.trim_str_response(m.group(3))
+			self.check_status()
+			return code, msg
+
+	def get_session_handle(self) -> object:
+		"""Returns the underlying pyvisa session."""
+		return self._session.get_session_handle()
+
+	def close(self) -> None:
+		"""Closes the Instrument session."""
+		with self._lock:
+			self._session.close()
+			self._session = None
+
+	# Events part
+
+	@property
+	def io_events_include_data(self) -> bool:
+		"""If true, the read and write handlers also include read and written data."""
+		return self._io_events_include_data
+
+	@io_events_include_data.setter
+	def io_events_include_data(self, value: bool) -> None:
+		"""If true, the read and write handlers also include read and written data."""
+		self._io_events_include_data = value
+		self._session.io_events_include_data = value
+
+	def event_args_append_instr_info(self, args: IoTransferEventArgs) -> IoTransferEventArgs:
+		"""Appends instrument-related information to the read/write event argument"""
+		args.chunk_size = self.data_chunk_size
+		args.resource_name = self.resource_name
+		return args
+
+	def send_write_str_event(self, cmd: str, opc_sync: bool) -> None:
+		"""Creates and sends write string event. The transfer is marked as done (end_of_transfer = True)."""
+		args = IoTransferEventArgs.write_str(opc_sync, len(cmd), cmd)
+		args.transferred_size = args.total_size
+		args.chunk_ix = 0
+		args.end_of_transfer = True
+		args = self.event_args_append_instr_info(args)
+		if self._io_events_include_data:
+			args.data = cmd
+		self.on_write_handler(args)
+
+	def start_send_read_event(self, query: str, opc_sync: bool) -> None:
+		"""Registers VisaSession.on_read_chunk_handler() which then generates events with each chunk transfer.
+		Event handler for these events is the local function of this method, which sends IoTransferEventArgs further up to the Instrument.on_read_handler()"""
+		if not self.on_read_handler:
+			return
+
+		def _read_chunk_handler(visa_args: EventArgsChunk) -> None:
+			"""Receives events from VisaSession on read chunk transfers, and sends them as IoTransferEventArgs to the Instrument.on_read_handler()"""
+			args.end_of_transfer = visa_args.end_of_transfer
+			args.chunk_ix = visa_args.chunk_ix
+			args.total_chunks = visa_args.total_chunks
+			args.chunk_size = visa_args.chunk_size
+			args.transferred_size = visa_args.transferred_size
+			args.total_size = visa_args.total_size
+			args.data = visa_args.data
+			args.binary = visa_args.binary
+			self.on_read_handler(args)
+
+		args = IoTransferEventArgs.read_chunk(opc_sync, query)
+		args = self.event_args_append_instr_info(args)
+		self._session.on_read_chunk_handler = _read_chunk_handler
+
+	def end_send_read_event(self):
+		"""Unregisters VisaSession.on_read_chunk_handler()"""
+		self._session.on_read_chunk_handler = None
+
+	def start_send_write_bin_event(self, cmd: str) -> None:
+		"""Registers VisaSession.on_write_chunk_handler() which then generates events with each chunk transfer.
+		Event handler for these events is the local function of this method, which sends IoTransferEventArgs further up to the Instrument.on_write_handler()"""
+		if not self.on_write_handler:
+			return
+
+		def _write_chunk_handler(visa_args: EventArgsChunk) -> None:
+			"""Receives events from VisaSession on write chunk transfers, and sends them as IoTransferEventArgs to the Instrument.on_write_handler()"""
+			args.end_of_transfer = visa_args.end_of_transfer
+			args.chunk_ix = visa_args.chunk_ix
+			args.total_chunks = visa_args.total_chunks
+			args.chunk_size = visa_args.chunk_size
+			args.transferred_size = visa_args.transferred_size
+			args.total_size = visa_args.total_size
+			args.data = visa_args.data
+			args.binary = visa_args.binary
+			self.on_write_handler(args)
+
+		args = IoTransferEventArgs.write_bin(cmd)
+		args = self.event_args_append_instr_info(args)
+		self._session.on_write_chunk_handler = _write_chunk_handler
+
+	def end_send_write_bin_event(self):
+		"""Unregisters VisaSession.on_write_chunk_handler()"""
+		self._session.on_write_chunk_handler = None
+
+	def _call_before_write_handler(self, cmd: str, block_callback: bool) -> None:
+		"""Calls the _pre_write_handler if defined. Used in all the base write methods."""
+		if block_callback is False and self._before_write_handler:
+			self._before_write_handler(self, cmd)
+
+	def _call_pre_query_handler(self, query: str, block_callback: bool) -> None:
+		"""Calls the _pre_query_handler if defined. Used in all the base query methods."""
+		if block_callback is False and self._before_query_handler:
+			self._before_query_handler(self, query)
+
+	@property
+	def before_write_handler(self) -> Callable:
+		"""Returns the handler of before_write events. \n
+		:return: current before_write_handler"""
+		return self._before_write_handler
+
+	@before_write_handler.setter
+	def before_write_handler(self, handler: Callable) -> None:
+		"""Sets handler for before_write events.
+		The before_write event is invoked before each write operation (only once, not for every chunk)
+		Event prototype: handler(io: Instrument, cmd: str)
+		:param handler: new handler"""
+		self._before_write_handler = handler
+
+	@property
+	def before_query_handler(self) -> Callable:
+		"""Returns the handler of before_query events. \n
+		:return: current before_query_handler"""
+		return self._before_query_handler
+
+	@before_query_handler.setter
+	def before_query_handler(self, handler: Callable) -> None:
+		"""Sets handler for before_query events.
+		The before_query event is invoked before each query operation (only once, not for every chunk)
+		Event prototype: handler(io: Instrument, query: str)
+		:param handler: new handler"""
+		self._before_query_handler = handler
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/InstrumentErrors.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/InstrumentErrors.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-class RsInstrException(Exception):
-	"""Exception base class for all the RsInstrument exceptions."""
-	def __init__(self, message: str):
-		super(RsInstrException, self).__init__(message)
-
-
-class TimeoutException(RsInstrException):
-	"""Exception for timeout errors."""
-	def __init__(self, message: str):
-		super(TimeoutException, self).__init__(message)
-
-
-class StatusException(RsInstrException):
-	"""Exception for instrument status errors."""
-	def __init__(self, rsrc_name: str, message: str):
-		self.rsrc_name = rsrc_name
-		super(StatusException, self).__init__(message)
-
-
-class UnexpectedResponseException(RsInstrException):
-	"""Exception for instrument unexpected responses."""
-	def __init__(self, rsrc_name: str, message: str):
-		self.rsrc_name = rsrc_name
-		super(UnexpectedResponseException, self).__init__(message)
-
-
-class ResourceError(RsInstrException):
-	"""Exception for resource name - e.g. resource not found."""
-	def __init__(self, rsrc_name: str, message: str):
-		self.rsrc_name = rsrc_name
-		super(ResourceError, self).__init__(message)
-
-
-class DriverValueError(RsInstrException):
-	"""Exception for different driver value settings e.g. RepCap values or Enum values."""
-	def __init__(self, rsrc_name: str, message: str):
-		self.rsrc_name = rsrc_name
-		super(DriverValueError, self).__init__(message)
-
-
-def assert_no_instrument_status_errors(rsrc_name: str, errors: list, context: str = '') -> None:
-	"""Checks the errors list and of it contains at least one element, it throws StatusException."""
-	if errors is None:
-		return
-	if len(errors) == 0:
-		return
-	if context:
-		message = f"'{rsrc_name}': {context} "
-	else:
-		message = f"'{rsrc_name}': "
-	if len(errors) == 1:
-		message += f'Instrument error detected: {errors[0]}'
-		raise StatusException(rsrc_name, message)
-	if len(errors) > 1:
-		message += '{} Instrument errors detected:\n{}'.format(len(errors), '\n'.join(errors))
-		raise StatusException(rsrc_name, message)
-
-
-def throw_opc_tout_exception(opc_tout: int, used_tout: int, context: str = '') -> None:
-	"""Throws TimeoutException - use it for any timeout error."""
-	if not context:
-		message = ''
-	else:
-		message = f'{context} '
-	if used_tout < 0 or used_tout == opc_tout:
-		message = message + f"Timeout expired before the operation completed. Current OPC timeout is set to {opc_tout} milliseconds. " \
-							"Change it with the property '_driver.UtilityFunctions.opc_timeout'. " \
-							"Optionally, if the method API contains an optional timeout parameter, set it there."
-	else:
-		message = message + f"Timeout expired before the operation completed. Used timeout: {used_tout} ms"
-	raise TimeoutException(message)
-
-
-def throw_bin_block_unexp_resp_exception(rsrc_name: str, received_data: str) -> None:
-	"""Throws InvalidDataException - use it in case an instrument response is not a binary block."""
-	if received_data.endswith('\n'):
-		raise UnexpectedResponseException(
-			rsrc_name, "Expected binary data header starting with #(hash), received data '{}'".format(received_data.replace('\n', '\\n')))
-	else:
-		raise UnexpectedResponseException(
-			rsrc_name, f"Expected binary data header starting with #(hash), received data starting with '{received_data}'...")
-
-
-def assert_query_has_qmark(query: str, context: str = '') -> None:
-	"""Throws Exception if the query does not contain any question marks."""
-	if '?' in query:
-		return
-	message = ''
-	if context:
-		message = ' ' + context
-	message = message + "Query commands must contain question-marks. Sent query: '{0}'".format(query.strip('\n'))
-	raise Exception(message)
-
-
-def assert_cmd_has_no_qmark(command: str, context: str = '') -> None:
-	"""Throws Exception if the query contains a question marks."""
-	if '?' not in command:
-		return
-	message = ''
-	if context:
-		message = ' ' + context
-	message = message + "Set commands must not contain question-marks. Sent command: '{0}'".format(command.strip('\n'))
-	raise Exception(message)
+class RsInstrException(Exception):
+	"""Exception base class for all the RsInstrument exceptions."""
+	def __init__(self, message: str):
+		super(RsInstrException, self).__init__(message)
+
+
+class TimeoutException(RsInstrException):
+	"""Exception for timeout errors."""
+	def __init__(self, message: str):
+		super(TimeoutException, self).__init__(message)
+
+
+class StatusException(RsInstrException):
+	"""Exception for instrument status errors."""
+	def __init__(self, rsrc_name: str, message: str):
+		self.rsrc_name = rsrc_name
+		super(StatusException, self).__init__(message)
+
+
+class UnexpectedResponseException(RsInstrException):
+	"""Exception for instrument unexpected responses."""
+	def __init__(self, rsrc_name: str, message: str):
+		self.rsrc_name = rsrc_name
+		super(UnexpectedResponseException, self).__init__(message)
+
+
+class ResourceError(RsInstrException):
+	"""Exception for resource name - e.g. resource not found."""
+	def __init__(self, rsrc_name: str, message: str):
+		self.rsrc_name = rsrc_name
+		super(ResourceError, self).__init__(message)
+
+
+class DriverValueError(RsInstrException):
+	"""Exception for different driver value settings e.g. RepCap values or Enum values."""
+	def __init__(self, rsrc_name: str, message: str):
+		self.rsrc_name = rsrc_name
+		super(DriverValueError, self).__init__(message)
+
+
+def assert_no_instrument_status_errors(rsrc_name: str, errors: list, context: str = '') -> None:
+	"""Checks the errors list and of it contains at least one element, it throws StatusException."""
+	if errors is None:
+		return
+	if len(errors) == 0:
+		return
+	if context:
+		message = f"'{rsrc_name}': {context} "
+	else:
+		message = f"'{rsrc_name}': "
+	if len(errors) == 1:
+		message += f'Instrument error detected: {errors[0]}'
+		raise StatusException(rsrc_name, message)
+	if len(errors) > 1:
+		message += '{} Instrument errors detected:\n{}'.format(len(errors), '\n'.join(errors))
+		raise StatusException(rsrc_name, message)
+
+
+def throw_opc_tout_exception(opc_tout: int, used_tout: int, context: str = '') -> None:
+	"""Throws TimeoutException - use it for any timeout error."""
+	if not context:
+		message = ''
+	else:
+		message = f'{context} '
+	if used_tout < 0 or used_tout == opc_tout:
+		message = message + f"Timeout expired before the operation completed. Current OPC timeout is set to {opc_tout} milliseconds. " \
+							"Change it with the property '_driver.UtilityFunctions.opc_timeout'. " \
+							"Optionally, if the method API contains an optional timeout parameter, set it there."
+	else:
+		message = message + f"Timeout expired before the operation completed. Used timeout: {used_tout} ms"
+	raise TimeoutException(message)
+
+
+def throw_bin_block_unexp_resp_exception(rsrc_name: str, received_data: str) -> None:
+	"""Throws InvalidDataException - use it in case an instrument response is not a binary block."""
+	if received_data.endswith('\n'):
+		raise UnexpectedResponseException(
+			rsrc_name, "Expected binary data header starting with #(hash), received data '{}'".format(received_data.replace('\n', '\\n')))
+	else:
+		raise UnexpectedResponseException(
+			rsrc_name, f"Expected binary data header starting with #(hash), received data starting with '{received_data}'...")
+
+
+def assert_query_has_qmark(query: str, context: str = '') -> None:
+	"""Throws Exception if the query does not contain any question marks."""
+	if '?' in query:
+		return
+	message = ''
+	if context:
+		message = ' ' + context
+	message = message + "Query commands must contain question-marks. Sent query: '{0}'".format(query.strip('\n'))
+	raise Exception(message)
+
+
+def assert_cmd_has_no_qmark(command: str, context: str = '') -> None:
+	"""Throws Exception if the query contains a question marks."""
+	if '?' not in command:
+		return
+	message = ''
+	if context:
+		message = ' ' + context
+	message = message + "Set commands must not contain question-marks. Sent command: '{0}'".format(command.strip('\n'))
+	raise Exception(message)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/InstrumentOptions.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/InstrumentOptions.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-import re
-from enum import Enum
-
-from .Utilities import trim_str_response
-
-
-class ParseMode(Enum):
-	"""Options parse mode enum."""
-	Skip = 0
-	KeepOriginal = 1
-	KeepBeforeDash = 2
-	KeepAfterDash = 3
-	Auto = 4
-
-
-class Options(object):
-	_optionsList = []
-
-	def __init__(self, options_str: str, mode=ParseMode.Auto):
-		"""Initializes the options with the *OPT? return string."""
-		self._initialize_from_string(options_str, mode)
-
-	def __str__(self):
-		return ','.join(self._optionsList)
-
-	def _initialize_from_string(self, options_str: str, mode: ParseMode):
-		"""Fills the self._optionsList from the entered 'options_str'."""
-		if mode == ParseMode.Skip:
-			return
-
-		parse_patt = r'(.?)(K|B)(\d+)(.*)$'
-		options = trim_str_response(options_str).split(',')
-		new_opts = []
-		for x in options:
-			has_dash = '-' in x
-			if has_dash:
-				dash_ix = x.index('-')
-				before = x[0:dash_ix + 1].strip('-')
-				after = x[dash_ix:].strip('-')
-
-				if mode is ParseMode.KeepBeforeDash:
-					x = before
-
-				elif mode is ParseMode.KeepAfterDash:
-					x = after
-
-				elif mode is ParseMode.Auto:
-					found_before = re.match(parse_patt, before)
-					found_after = re.match(parse_patt, after)
-					if found_before is not None and found_after is not None:
-						x = after if len(found_after.group(0)) >= len(found_before.group(0)) else before
-					elif found_before is not None:
-						x = before
-					elif found_after is not None:
-						x = after
-
-			if len(x) > 0:
-				new_opts.append(x)
-
-		# Remove duplicates
-		new_opts = set(new_opts)
-
-		# Create a weighting number
-		result = []
-		for x in new_opts:
-			sort_value = x
-			m = re.match(parse_patt, x)
-			if m:
-				kb_weight = '02' if m.group(2) == 'B' else '01'
-				sort_value = '{0}{1}{2:09d}{3}'.format(m.group(1), kb_weight, int(m.group(3)), m.group(4))
-
-			result.append('{0} -> {1}'.format(sort_value, x))
-
-		# Sort keys in that dictionary and then reconstruct the original options
-		result.sort()
-		self._optionsList = [x.split(' -> ')[1] for x in result]
-
-	def get_all(self):
-		"""Returns all the options."""
-		return self._optionsList
+import re
+from enum import Enum
+
+from .Utilities import trim_str_response
+
+
+class ParseMode(Enum):
+	"""Options parse mode enum."""
+	Skip = 0
+	KeepOriginal = 1
+	KeepBeforeDash = 2
+	KeepAfterDash = 3
+	Auto = 4
+
+
+class Options(object):
+	_optionsList = []
+
+	def __init__(self, options_str: str, mode=ParseMode.Auto):
+		"""Initializes the options with the *OPT? return string."""
+		self._initialize_from_string(options_str, mode)
+
+	def __str__(self):
+		return ','.join(self._optionsList)
+
+	def _initialize_from_string(self, options_str: str, mode: ParseMode):
+		"""Fills the self._optionsList from the entered 'options_str'."""
+		if mode == ParseMode.Skip:
+			return
+
+		parse_patt = r'(.?)(K|B)(\d+)(.*)$'
+		options = trim_str_response(options_str).split(',')
+		new_opts = []
+		for x in options:
+			has_dash = '-' in x
+			if has_dash:
+				dash_ix = x.index('-')
+				before = x[0:dash_ix + 1].strip('-')
+				after = x[dash_ix:].strip('-')
+
+				if mode is ParseMode.KeepBeforeDash:
+					x = before
+
+				elif mode is ParseMode.KeepAfterDash:
+					x = after
+
+				elif mode is ParseMode.Auto:
+					found_before = re.match(parse_patt, before)
+					found_after = re.match(parse_patt, after)
+					if found_before is not None and found_after is not None:
+						x = after if len(found_after.group(0)) >= len(found_before.group(0)) else before
+					elif found_before is not None:
+						x = before
+					elif found_after is not None:
+						x = after
+
+			if len(x) > 0:
+				new_opts.append(x)
+
+		# Remove duplicates
+		new_opts = set(new_opts)
+
+		# Create a weighting number
+		result = []
+		for x in new_opts:
+			sort_value = x
+			m = re.match(parse_patt, x)
+			if m:
+				kb_weight = '02' if m.group(2) == 'B' else '01'
+				sort_value = '{0}{1}{2:09d}{3}'.format(m.group(1), kb_weight, int(m.group(3)), m.group(4))
+
+			result.append('{0} -> {1}'.format(sort_value, x))
+
+		# Sort keys in that dictionary and then reconstruct the original options
+		result.sort()
+		self._optionsList = [x.split(' -> ')[1] for x in result]
+
+	def get_all(self):
+		"""Returns all the options."""
+		return self._optionsList
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/InstrumentSettings.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/InstrumentSettings.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-from enum import Enum
-from enum import Flag
-
-from . import InstrumentOptions as Opts, Conversions as Conv
-
-
-class InstrViClearMode(Flag):
-	disabled = 0x00
-	ignore_error = 0x01
-	execute_on_all = 0x02
-	execute_on_socket = 0x04
-	execute_on_serial = 0x08
-	execute_on_usb = 0x10
-	execute_on_gpib = 0x20
-	execute_on_tcpvxi = 0x40
-
-
-class WaitForOpcMode(Enum):
-	"""Mode that is used for OPC-sync commands/queries"""
-	stb_poll = 1
-	stb_poll_slow = 2
-	stb_poll_superslow = 3
-	opc_query = 4
-
-
-class InstrumentSettings(object):
-	"""Defines settings of the instrument."""
-
-	def __init__(
-			self,
-			viclear_exe_mode: InstrViClearMode,
-			idn_model_full_name: bool,
-			write_delay: int,
-			read_delay: int,
-			io_segment_size: int,
-			opc_wait_mode: WaitForOpcMode,
-			opc_timeout: int,
-			visa_timeout: int,
-			self_test_timeout: int,
-			instr_options_parse_mode: Opts.ParseMode,
-			bin_float_numbers_format: Conv.BinFloatFormat,
-			bin_int_numbers_format: Conv.BinIntFormat,
-			opc_query_after_write: bool):
-
-		self.viclear_exe_mode = viclear_exe_mode
-		self.idn_model_full_name = idn_model_full_name
-		self.write_delay = write_delay
-		self.read_delay = read_delay
-		self.io_segment_size = io_segment_size
-		self.opc_wait_mode = opc_wait_mode
-		self.opc_timeout = opc_timeout
-		self.visa_timeout = visa_timeout
-		self.selftest_timeout = self_test_timeout
-		self.instr_options_parse_mode = instr_options_parse_mode
-		self.bin_float_numbers_format = bin_float_numbers_format
-		self.bin_int_numbers_format = bin_int_numbers_format
-		self.opc_query_after_write = opc_query_after_write
-
-		self.assure_write_with_tc = False
-		self.term_char = '\n'
-		self.add_term_char_to_write_bin_block = False
-
-		self.stb_in_error_check = True
-		self.disable_opc_query = False
-		self.visa_select = None
-
-	def apply_option_settings(self, settings: dict) -> None:
-
-		value = settings.get('SELECTVISA')
-		if value is not None:
-			self.visa_select = value
-
-		value = settings.get('DRIVERSETUP_WRITEDELAY')
-		if value is not None:
-			self.write_delay = Conv.str_to_int(value)
-
-		value = settings.get('DRIVERSETUP_READDELAY')
-		if value is not None:
-			self.read_delay = Conv.str_to_int(value)
-
-		value = settings.get('DRIVERSETUP_OPCWAITMODE')
-		if value is not None:
-			value = value.upper()
-			if value == 'STBPOLLING':
-				self.opc_wait_mode = WaitForOpcMode.stb_poll
-			elif value == 'STBPOLLINGSLOW':
-				self.opc_wait_mode = WaitForOpcMode.stb_poll_slow
-			elif value == 'STBPOLLINGSUPERSLOW':
-				self.opc_wait_mode = WaitForOpcMode.stb_poll_superslow
-			elif value == 'OPCQUERY':
-				self.opc_wait_mode = WaitForOpcMode.opc_query
-			else:
-				raise ValueError(
-					f"Unknown value in InitWithOptions string DriverSetup key 'WaitForOPC'. Value '{value}' is not recognized. "
-					"Valid values: 'StbPolling', 'StbPollingSlow', 'StbPollingSuperSlow', 'OpcQuery'")
-
-		value = settings.get('DRIVERSETUP_ADDTERMCHARTOWRITEBINBLOCK')
-		if value is not None:
-			self.add_term_char_to_write_bin_block = Conv.str_to_bool(value)
-
-		# Obsolete, use the DRIVERSETUP_ASSUREWRITEWITHTERMCHAR
-		value = settings.get('DRIVERSETUP_ASSUREWRITEWITHLF')
-		if value is not None:
-			self.assure_write_with_tc = Conv.str_to_bool(value)
-		value = settings.get('DRIVERSETUP_ASSUREWRITEWITHTERMCHAR')
-		if value is not None:
-			self.assure_write_with_tc = Conv.str_to_bool(value)
-
-		value = settings.get('DRIVERSETUP_TERMINATIONCHARACTER')
-		if value is not None:
-			self.term_char = value
-
-		value = settings.get('DRIVERSETUP_IOSEGMENTSIZE')
-		if value is not None:
-			self.io_segment_size = Conv.str_to_int(value)
-
-		value = settings.get('DRIVERSETUP_OPCTIMEOUT')
-		if value is not None:
-			self.opc_timeout = Conv.str_to_int(value)
-
-		value = settings.get('DRIVERSETUP_VISATIMEOUT')
-		if value is not None:
-			self.visa_timeout = Conv.str_to_int(value)
-
-		value = settings.get('DRIVERSETUP_VICLEAREXEMODE')
-		if value is not None:
-			self.viclear_exe_mode = value
-
-		value = settings.get('DRIVERSETUP_OPCQUERYAFTERWRITE')
-		if value is not None:
-			self.opc_query_after_write = Conv.str_to_bool(value)
-
-		value = settings.get('DRIVERSETUP_STBINERRORCHECK')
-		if value is not None:
-			self.stb_in_error_check = Conv.str_to_bool(value)
-
-		value = settings.get('DRIVERSETUP_DISABLEOPCQUERY')
-		if value is not None:
-			self.disable_opc_query = Conv.str_to_bool(value)
-
-		value = settings.get('DRIVERSETUP_QUERYOPT')
-		if value is not None:
-			value = value.upper()
-			if value == 'SKIP':
-				self.instr_options_parse_mode = Opts.ParseMode.Skip
-			elif value == 'AUTO':
-				self.instr_options_parse_mode = Opts.ParseMode.Auto
-			elif value == 'KEEPORIGINAL':
-				self.instr_options_parse_mode = Opts.ParseMode.KeepOriginal
-			elif value == 'KEEPBEFOREDASH':
-				self.instr_options_parse_mode = Opts.ParseMode.KeepBeforeDash
-			elif value == 'KEEPAFTERDASH':
-				self.instr_options_parse_mode = Opts.ParseMode.KeepAfterDash
-			else:
-				raise ValueError(
-					f"Unknown value in InitWithOptions string DriverSetup key 'QueryOpt'. Value '{value}' is not recognized. "
-					"Valid values: 'Skip', 'Auto', 'KeepOriginal', 'KeepBeforeDash', 'KeepAfterDash'")
+from enum import Enum
+from enum import Flag
+
+from . import InstrumentOptions as Opts, Conversions as Conv
+
+
+class InstrViClearMode(Flag):
+	disabled = 0x00
+	ignore_error = 0x01
+	execute_on_all = 0x02
+	execute_on_socket = 0x04
+	execute_on_serial = 0x08
+	execute_on_usb = 0x10
+	execute_on_gpib = 0x20
+	execute_on_tcpvxi = 0x40
+
+
+class WaitForOpcMode(Enum):
+	"""Mode that is used for OPC-sync commands/queries"""
+	stb_poll = 1
+	stb_poll_slow = 2
+	stb_poll_superslow = 3
+	opc_query = 4
+
+
+class InstrumentSettings(object):
+	"""Defines settings of the instrument."""
+
+	def __init__(
+			self,
+			viclear_exe_mode: InstrViClearMode,
+			idn_model_full_name: bool,
+			write_delay: int,
+			read_delay: int,
+			io_segment_size: int,
+			opc_wait_mode: WaitForOpcMode,
+			opc_timeout: int,
+			visa_timeout: int,
+			self_test_timeout: int,
+			instr_options_parse_mode: Opts.ParseMode,
+			bin_float_numbers_format: Conv.BinFloatFormat,
+			bin_int_numbers_format: Conv.BinIntFormat,
+			opc_query_after_write: bool):
+
+		self.viclear_exe_mode = viclear_exe_mode
+		self.idn_model_full_name = idn_model_full_name
+		self.write_delay = write_delay
+		self.read_delay = read_delay
+		self.io_segment_size = io_segment_size
+		self.opc_wait_mode = opc_wait_mode
+		self.opc_timeout = opc_timeout
+		self.visa_timeout = visa_timeout
+		self.selftest_timeout = self_test_timeout
+		self.instr_options_parse_mode = instr_options_parse_mode
+		self.bin_float_numbers_format = bin_float_numbers_format
+		self.bin_int_numbers_format = bin_int_numbers_format
+		self.opc_query_after_write = opc_query_after_write
+
+		self.assure_write_with_tc = False
+		self.term_char = '\n'
+		self.add_term_char_to_write_bin_block = False
+
+		self.stb_in_error_check = True
+		self.disable_opc_query = False
+		self.visa_select = None
+
+	def apply_option_settings(self, settings: dict) -> None:
+
+		value = settings.get('SELECTVISA')
+		if value is not None:
+			self.visa_select = value
+
+		value = settings.get('DRIVERSETUP_WRITEDELAY')
+		if value is not None:
+			self.write_delay = Conv.str_to_int(value)
+
+		value = settings.get('DRIVERSETUP_READDELAY')
+		if value is not None:
+			self.read_delay = Conv.str_to_int(value)
+
+		value = settings.get('DRIVERSETUP_OPCWAITMODE')
+		if value is not None:
+			value = value.upper()
+			if value == 'STBPOLLING':
+				self.opc_wait_mode = WaitForOpcMode.stb_poll
+			elif value == 'STBPOLLINGSLOW':
+				self.opc_wait_mode = WaitForOpcMode.stb_poll_slow
+			elif value == 'STBPOLLINGSUPERSLOW':
+				self.opc_wait_mode = WaitForOpcMode.stb_poll_superslow
+			elif value == 'OPCQUERY':
+				self.opc_wait_mode = WaitForOpcMode.opc_query
+			else:
+				raise ValueError(
+					f"Unknown value in InitWithOptions string DriverSetup key 'WaitForOPC'. Value '{value}' is not recognized. "
+					"Valid values: 'StbPolling', 'StbPollingSlow', 'StbPollingSuperSlow', 'OpcQuery'")
+
+		value = settings.get('DRIVERSETUP_ADDTERMCHARTOWRITEBINBLOCK')
+		if value is not None:
+			self.add_term_char_to_write_bin_block = Conv.str_to_bool(value)
+
+		# Obsolete, use the DRIVERSETUP_ASSUREWRITEWITHTERMCHAR
+		value = settings.get('DRIVERSETUP_ASSUREWRITEWITHLF')
+		if value is not None:
+			self.assure_write_with_tc = Conv.str_to_bool(value)
+		value = settings.get('DRIVERSETUP_ASSUREWRITEWITHTERMCHAR')
+		if value is not None:
+			self.assure_write_with_tc = Conv.str_to_bool(value)
+
+		value = settings.get('DRIVERSETUP_TERMINATIONCHARACTER')
+		if value is not None:
+			self.term_char = value
+
+		value = settings.get('DRIVERSETUP_IOSEGMENTSIZE')
+		if value is not None:
+			self.io_segment_size = Conv.str_to_int(value)
+
+		value = settings.get('DRIVERSETUP_OPCTIMEOUT')
+		if value is not None:
+			self.opc_timeout = Conv.str_to_int(value)
+
+		value = settings.get('DRIVERSETUP_VISATIMEOUT')
+		if value is not None:
+			self.visa_timeout = Conv.str_to_int(value)
+
+		value = settings.get('DRIVERSETUP_VICLEAREXEMODE')
+		if value is not None:
+			self.viclear_exe_mode = value
+
+		value = settings.get('DRIVERSETUP_OPCQUERYAFTERWRITE')
+		if value is not None:
+			self.opc_query_after_write = Conv.str_to_bool(value)
+
+		value = settings.get('DRIVERSETUP_STBINERRORCHECK')
+		if value is not None:
+			self.stb_in_error_check = Conv.str_to_bool(value)
+
+		value = settings.get('DRIVERSETUP_DISABLEOPCQUERY')
+		if value is not None:
+			self.disable_opc_query = Conv.str_to_bool(value)
+
+		value = settings.get('DRIVERSETUP_QUERYOPT')
+		if value is not None:
+			value = value.upper()
+			if value == 'SKIP':
+				self.instr_options_parse_mode = Opts.ParseMode.Skip
+			elif value == 'AUTO':
+				self.instr_options_parse_mode = Opts.ParseMode.Auto
+			elif value == 'KEEPORIGINAL':
+				self.instr_options_parse_mode = Opts.ParseMode.KeepOriginal
+			elif value == 'KEEPBEFOREDASH':
+				self.instr_options_parse_mode = Opts.ParseMode.KeepBeforeDash
+			elif value == 'KEEPAFTERDASH':
+				self.instr_options_parse_mode = Opts.ParseMode.KeepAfterDash
+			else:
+				raise ValueError(
+					f"Unknown value in InitWithOptions string DriverSetup key 'QueryOpt'. Value '{value}' is not recognized. "
+					"Valid values: 'Skip', 'Auto', 'KeepOriginal', 'KeepBeforeDash', 'KeepAfterDash'")
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/InternalLinker.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/InternalLinker.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from time import time
-from typing import Dict, Callable
-
-from . import ArgSingle, ArgSingleSuppressed
-from .ArgLinkedEventArgs import ArgLinkedEventArgs
-from .Utilities import get_plural_string
-
-
-class InternalLinker(object):
-	"""Class for:
-		- cutting out suppressed arguments from a device response.
-		- invoking a handler if the argument has InternalLinking defined.
-		- holds dictionary of handlers where the dict_key is the InternalLinking string.
-	Handlers registration/deleting is done with:
-		- set_handler()
-		- del_handler()
-		- del_all_handlers()"""
-
-	def __init__(self):
-		self._handlers = {}
-
-	def __str__(self):
-		if len(self._handlers) == 0:
-			return 'Linker, no handlers'
-		return f"Linker, {get_plural_string('handler', len(self._handlers))}: {','.join(self._handlers)}"
-
-	def set_handler(self, link_name: str, handler: Callable) -> Callable:
-		"""Adds / Updates handler for the link_name.
-		Returns the previous registered handler, or None if no handler was registered before."""
-		previous = None if link_name not in self._handlers else self._handlers[link_name]
-		self._handlers[link_name] = handler
-		return previous
-
-	def del_handler(self, link_name: str) -> Callable:
-		"""Deletes handler for the link_name.
-		Returns the deleted handler, or None if none existed."""
-		current = None if link_name not in self._handlers else self._handlers[link_name]
-		if current:
-			del self._handlers[link_name]
-		return current
-
-	def del_all_handlers(self) -> int:
-		"""Deletes all the handlers.
-		Returns number of deleted links."""
-		count = len(self._handlers)
-		self._handlers = {}
-		return count
-
-	def cut_from_response_string(self, arg: ArgSingleSuppressed, response: str, context: str) -> str:
-		"""Takes the string 'response', removes the suppressed argument value from it and returns the rest.
-		The cut out part is sent via handler if the internal linking exists for that argument exists."""
-		result = ''
-		if arg.argument_ix is None:
-			raise Exception(f'Argument has argument_ix attribute not assigned (equals None). Argument: {arg}')
-		if arg.argument_ix != 0:
-			raise Exception(f'Only arguments with index 0 can be suppressed. Argument: {arg}')
-		if arg.is_open_list:
-			raise Exception(f'Open List arguments can not be suppressed. Argument: {arg}')
-		repetition = 0
-		i = 0
-		for c in response:
-			if c == ',':
-				repetition += 1
-			if repetition == arg.repetition:
-				break
-			i += 1
-
-		suppressed_part = response[0:i]
-		i += 1
-		if i < len(response):
-			result = response[i:]
-
-		self.invoke_single_intern_link(arg, context, suppressed_part)
-		return result
-
-	def invoke_single_intern_link(self, arg: ArgSingleSuppressed or ArgSingle, context: str, value: str) -> None:
-		"""Invokes the registered handler for the internal linked argument."""
-		if arg.intern_link and arg.intern_link in self._handlers:
-			event_args = ArgLinkedEventArgs(arg.intern_link, arg.name, value, context, time())
-			self._handlers[arg.intern_link](event_args)
-
-	def invoke_struct_intern_links(self, struct, args: Dict, context: str) -> None:
-		"""Invokes handler for each of the Structure arguments that have internal linking."""
-		for arg in args.values():
-			if arg.intern_link and arg.intern_link in self._handlers:
-				event_args = ArgLinkedEventArgs(arg.intern_link, arg.name, getattr(struct, arg.name), context, time())
-				self._handlers[arg.intern_link](event_args)
+from time import time
+from typing import Dict, Callable
+
+from . import ArgSingle, ArgSingleSuppressed
+from .ArgLinkedEventArgs import ArgLinkedEventArgs
+from .Utilities import get_plural_string
+
+
+class InternalLinker(object):
+	"""Class for:
+		- cutting out suppressed arguments from a device response.
+		- invoking a handler if the argument has InternalLinking defined.
+		- holds dictionary of handlers where the dict_key is the InternalLinking string.
+	Handlers registration/deleting is done with:
+		- set_handler()
+		- del_handler()
+		- del_all_handlers()"""
+
+	def __init__(self):
+		self._handlers = {}
+
+	def __str__(self):
+		if len(self._handlers) == 0:
+			return 'Linker, no handlers'
+		return f"Linker, {get_plural_string('handler', len(self._handlers))}: {','.join(self._handlers)}"
+
+	def set_handler(self, link_name: str, handler: Callable) -> Callable:
+		"""Adds / Updates handler for the link_name.
+		Returns the previous registered handler, or None if no handler was registered before."""
+		previous = None if link_name not in self._handlers else self._handlers[link_name]
+		self._handlers[link_name] = handler
+		return previous
+
+	def del_handler(self, link_name: str) -> Callable:
+		"""Deletes handler for the link_name.
+		Returns the deleted handler, or None if none existed."""
+		current = None if link_name not in self._handlers else self._handlers[link_name]
+		if current:
+			del self._handlers[link_name]
+		return current
+
+	def del_all_handlers(self) -> int:
+		"""Deletes all the handlers.
+		Returns number of deleted links."""
+		count = len(self._handlers)
+		self._handlers = {}
+		return count
+
+	def cut_from_response_string(self, arg: ArgSingleSuppressed, response: str, context: str) -> str:
+		"""Takes the string 'response', removes the suppressed argument value from it and returns the rest.
+		The cut out part is sent via handler if the internal linking exists for that argument exists."""
+		result = ''
+		if arg.argument_ix is None:
+			raise Exception(f'Argument has argument_ix attribute not assigned (equals None). Argument: {arg}')
+		if arg.argument_ix != 0:
+			raise Exception(f'Only arguments with index 0 can be suppressed. Argument: {arg}')
+		if arg.is_open_list:
+			raise Exception(f'Open List arguments can not be suppressed. Argument: {arg}')
+		repetition = 0
+		i = 0
+		for c in response:
+			if c == ',':
+				repetition += 1
+			if repetition == arg.repetition:
+				break
+			i += 1
+
+		suppressed_part = response[0:i]
+		i += 1
+		if i < len(response):
+			result = response[i:]
+
+		self.invoke_single_intern_link(arg, context, suppressed_part)
+		return result
+
+	def invoke_single_intern_link(self, arg: ArgSingleSuppressed or ArgSingle, context: str, value: str) -> None:
+		"""Invokes the registered handler for the internal linked argument."""
+		if arg.intern_link and arg.intern_link in self._handlers:
+			event_args = ArgLinkedEventArgs(arg.intern_link, arg.name, value, context, time())
+			self._handlers[arg.intern_link](event_args)
+
+	def invoke_struct_intern_links(self, struct, args: Dict, context: str) -> None:
+		"""Invokes handler for each of the Structure arguments that have internal linking."""
+		for arg in args.values():
+			if arg.intern_link and arg.intern_link in self._handlers:
+				event_args = ArgLinkedEventArgs(arg.intern_link, arg.name, getattr(struct, arg.name), context, time())
+				self._handlers[arg.intern_link](event_args)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/RepeatedCapability.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/RepeatedCapability.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,92 +1,96 @@
-from enum import Enum
-
-
-# Command integer value that signals Default value "DEFAULT"
-VALUE_DEFAULT = -1
-
-# Command integer value that signals "EMPTY"
-VALUE_EMPTY = -2
-
-
-class RepeatedCapability(object):
-	"""Represents Repeated Capability value and type"""
-
-	def __init__(self, header_name: str, method_get_name: str, method_set_name: str, start_value: Enum):
-		"""Constructor with header name, group property name and the start value"""
-
-		self._enum_value = None
-		self.enum_type = start_value.__class__
-		self.name = self.enum_type.__name__
-		self.header_name = header_name
-		self.method_get_name = method_get_name
-		self.method_set_name = method_set_name
-		self._start_value = start_value
-		self.set_to_start_value()
-
-	def __str__(self) -> str:
-		out = f'RepCap {self.name}'
-		if self._enum_value is not None:
-			out += f" = {self._enum_value}"
-		return out
-
-	@classmethod
-	def clsm_assert_type(cls, enum_value: Enum, enum_type) -> None:
-		"""Static assertion function to check if the entered value is a member of the defined repcap enum"""
-		if not isinstance(enum_value, enum_type):
-			raise TypeError(f"RepCap value must be of type '{enum_type}'. Entered value type: {type(enum_value)}, value '{enum_value}'")
-
-	@classmethod
-	def clsm_get_direct_cmd_value_int(cls, enum_value: Enum, enum_type) -> int:
-		"""Static function to get an integer interpretation of a direct enum value
-		Does not work with Empty or Default"""
-		RepeatedCapability.clsm_assert_type(enum_value, enum_type)
-		return enum_value.value
-
-	@classmethod
-	def clsm_is_default_value(cls, enum_value: Enum, enum_type) -> bool:
-		"""Returns True, if the entered value is enum.Default"""
-		return cls.clsm_get_direct_cmd_value_int(enum_value, enum_type) == VALUE_DEFAULT
-
-	def is_default_value(self) -> bool:
-		"""Returns True, if the repcap value is enum.Default"""
-		return RepeatedCapability.clsm_is_default_value(self._enum_value, self.enum_type)
-
-	def set_enum_value(self, enum_value: Enum) -> None:
-		"""Sets new enum value. Can not be Default"""
-		if RepeatedCapability.clsm_is_default_value(enum_value, self.enum_type):
-			raise ValueError(f"Setting RepCap enum value '{enum_value}' is not allowed. Please select a concrete value")
-		self._enum_value = enum_value
-
-	def get_enum_value(self) -> Enum:
-		"""Returns the actual enum value"""
-		return self._enum_value
-
-	def set_to_start_value(self) -> None:
-		"""Sets back to the value entered in the constructor"""
-		self.set_enum_value(self._start_value)
-
-	def matches_type(self, enum_type) -> bool:
-		"""Returns true, if the entered type matches the EnumType"""
-		return self.enum_type == enum_type
-
-	@classmethod
-	def clsm_get_cmd_string_value(cls, enum_value: Enum, enum_type) -> str:
-		"""Converts RepCap integer value to string
-		ValueEmpty is converted to "" (Not valid, but tolerated)
-		ValueDefault throws an exception
-		0 is converted to "" (Not valid, but tolerated)
-		Positive numbers are converted to integer strings e.g. 1 => '1' """
-		number = cls.clsm_get_direct_cmd_value_int(enum_value, enum_type)
-		if number == VALUE_EMPTY or number == 0:
-			return ''
-		if number == VALUE_DEFAULT:
-			raise ValueError(f"RepCap enum value Default can not be converted to the command string value. RepCap: {enum_type}")
-		return str(number)
-
-	def get_cmd_string_value(self) -> str:
-		"""Converts RepCap integer value to string
-		ValueEmpty is converted to "" (Not valid, but tolerated)
-		ValueDefault throws an exception
-		0 is converted to "" (Not valid, but tolerated)
-		Positive numbers are converted to integer strings e.g. 1 => '1' """
-		return RepeatedCapability.clsm_get_cmd_string_value(self._enum_value, self.enum_type)
+from enum import Enum
+
+
+# Command integer value that signals Default value "DEFAULT"
+VALUE_DEFAULT = -1
+
+# Command integer value that signals "EMPTY"
+VALUE_EMPTY = -2
+
+
+class RepeatedCapability(object):
+	"""Represents Repeated Capability value and type"""
+
+	def __init__(self, header_name: str, method_get_name: str, method_set_name: str, start_value: Enum):
+		"""Constructor with header name, group property name and the start value"""
+
+		self._enum_value = None
+		self.enum_type = start_value.__class__
+		self.name = self.enum_type.__name__
+		self.header_name = header_name
+		self.method_get_name = method_get_name
+		self.method_set_name = method_set_name
+		self._start_value = start_value
+		self.set_to_start_value()
+
+	def __str__(self) -> str:
+		out = f'RepCap {self.name}'
+		if self._enum_value is not None:
+			out += f" = {self._enum_value}"
+		return out
+
+	@classmethod
+	def clsm_assert_type(cls, enum_value: Enum, enum_type) -> None:
+		"""Static assertion function to check if the entered value is a member of the defined repcap enum"""
+		if not isinstance(enum_value, enum_type):
+			raise TypeError(f"RepCap value must be of type '{enum_type}'. Entered value type: {type(enum_value)}, value '{enum_value}'")
+
+	@classmethod
+	def clsm_get_direct_cmd_value_int(cls, enum_value: Enum, enum_type) -> int:
+		"""Static function to get an integer interpretation of a direct enum value
+		Does not work with Empty or Default"""
+		RepeatedCapability.clsm_assert_type(enum_value, enum_type)
+		return enum_value.value
+
+	@classmethod
+	def clsm_is_default_value(cls, enum_value: Enum, enum_type) -> bool:
+		"""Returns True, if the entered value is enum.Default"""
+		return cls.clsm_get_direct_cmd_value_int(enum_value, enum_type) == VALUE_DEFAULT
+
+	def is_default_value(self) -> bool:
+		"""Returns True, if the repcap value is enum.Default"""
+		return RepeatedCapability.clsm_is_default_value(self._enum_value, self.enum_type)
+
+	def set_enum_value(self, enum_value: Enum) -> None:
+		"""Sets new enum value. Can not be Default"""
+		if RepeatedCapability.clsm_is_default_value(enum_value, self.enum_type):
+			raise ValueError(f"Setting RepCap enum value '{enum_value}' is not allowed. Please select a concrete value")
+		self._enum_value = enum_value
+
+	def get_enum_value(self) -> Enum:
+		"""Returns the actual enum value"""
+		return self._enum_value
+
+	def set_to_start_value(self) -> None:
+		"""Sets back to the value entered in the constructor"""
+		self.set_enum_value(self._start_value)
+
+	def matches_type(self, enum_type) -> bool:
+		"""Returns true, if the entered type matches the EnumType"""
+		return self.enum_type == enum_type
+
+	@classmethod
+	def clsm_get_cmd_string_value(cls, enum_value: Enum, enum_type) -> str:
+		"""Converts RepCap integer value to string
+		ValueEmpty is converted to "" (Not valid, but tolerated)
+		ValueDefault throws an exception
+		0 is converted to "" (Not valid, but tolerated)
+		Positive numbers are converted to integer strings e.g. 1 => '1' """
+		number = cls.clsm_get_direct_cmd_value_int(enum_value, enum_type)
+		if number == VALUE_EMPTY:
+			return ''
+		if number == 0:
+			# return empty string, if the enum definition does not contain a valid element with value 0
+			enum_values = [x.value for x in enum_type]
+			return '0' if 0 in enum_values else ''
+		if number == VALUE_DEFAULT:
+			raise ValueError(f"RepCap enum value Default can not be converted to the command string value. RepCap: {enum_type}")
+		return str(number)
+
+	def get_cmd_string_value(self) -> str:
+		"""Converts RepCap integer value to string
+		ValueEmpty is converted to "" (Not valid, but tolerated)
+		ValueDefault throws an exception
+		0 is converted to "" (Not valid, but tolerated)
+		Positive numbers are converted to integer strings e.g. 1 => '1' """
+		return RepeatedCapability.clsm_get_cmd_string_value(self._enum_value, self.enum_type)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/StreamReader.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/StreamReader.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-from enum import Enum
-from os import path
-from typing import AnyStr
-
-from .Utilities import size_to_kb_mb_string
-
-
-class Type(Enum):
-	Variable = 1
-	File = 2
-
-
-class StreamReader:
-	"""Lightweight stream reader implementation. Data source can be: \n
-	- variable
-	- file"""
-
-	def __init__(self, binary: bool, source: Type, data: AnyStr):
-		"""Initializes StreamReader instance.\n
-		:param binary: True: Binary data, False: ASCII data
-		:param source: Source type for the stream. Variable / File
-		:param data: Depending on the 'binary' and 'source':
-		For source type Variable the data must be either bytes() or str
-		For source type File data must be string with existing file path."""
-		self._source = source
-		self._binary = binary
-		self._start_ptr = 0
-
-		if self._source == Type.Variable:
-			if self._binary:
-				assert isinstance(data, bytes), f'Data must be of bytes type. Actual type: {type(data)}'
-			else:
-				assert isinstance(data, str), f'Data must be of string type. Actual type: {type(data)}'
-			self._data = data
-			self._full_len = len(self._data)
-		elif self._source == Type.File:
-			assert isinstance(data, str), f'Data must be of string type (file path). Actual type: {type(data)}'
-			if not path.isfile(data):
-				raise Exception(f'File does not exist. File path: {data}')
-			self.file_path = data
-			self._data = open(self.file_path, 'rb' if self._binary else 'r')
-			self._full_len = path.getsize(self.file_path)
-		else:
-			raise Exception(f'StreamReader unknown type {source}')
-
-	@classmethod
-	def as_bin_var(cls, data: bytes) -> 'StreamReader':
-		"""Creates new StreamReader from bytes.
-		:param data: [bytes] data for the stream."""
-		return cls(True, Type.Variable, data)
-
-	@classmethod
-	def as_string_var(cls, data: str) -> 'StreamReader':
-		"""Creates new StreamReader from string.
-		:param data: [str] data for the stream."""
-		return cls(False, Type.Variable, data)
-
-	@classmethod
-	def as_bin_file(cls, file_path: str) -> 'StreamReader':
-		"""Creates new StreamReader from binary file. The file must exist at this time.
-		:param file_path: [str] Path to the file."""
-		return cls(True, Type.File, file_path)
-
-	@classmethod
-	def as_text_file(cls, file_path: str) -> 'StreamReader':
-		"""Creates new StreamReader from text file. The file must exist at this time.
-		:param file_path: [str] Path to the file."""
-		return cls(False, Type.File, file_path)
-
-	def __str__(self):
-		if self._source == Type.Variable:
-			mode = 'binary' if self._binary else 'string'
-			return f'StreamReader {mode} data, full size {size_to_kb_mb_string(self._full_len, True)}, remaining size {size_to_kb_mb_string(len(self), True)}'
-		if self._source == Type.File:
-			mode = 'binary' if self._binary else 'text'
-			return f'StreamReader {mode}, full size {size_to_kb_mb_string(self._full_len, True)}, remaining size {size_to_kb_mb_string(len(self), True)}'
-
-	def __len__(self):
-		"""Returns remaining length."""
-		return self._full_len - self._start_ptr
-
-	def __enter__(self):
-		return self
-
-	def __exit__(self, exception_type, exception_value, traceback):
-		self.close()
-
-	@property
-	def full_len(self) -> int:
-		"""Returns original full length."""
-		return self._full_len
-
-	@property
-	def binary(self) -> bool:
-		"""Returns true, if the data provided is binary."""
-		return self._binary
-
-	def read(self, chunk_size: int = None) -> AnyStr:
-		"""Read chunk from the data and moves the data pointer behind it.
-		If the remaining length is smaller than the chunk_size, the method returns the remaining length only.
-		:param chunk_size: chunk to read. If not set, the method reads the entire data."""
-		assert self._data is not None, 'StreamReader buffer is invalid. You have probably closed it already.'
-		chunk_size = len(self) if chunk_size is None else chunk_size
-		chunk_size = min(chunk_size, len(self))
-		if chunk_size < 0:
-			raise ValueError(f'Chunk size can not be negative number: {chunk_size}')
-
-		if self._source == Type.Variable:
-			self._start_ptr += chunk_size
-			return self._data[self._start_ptr - chunk_size: self._start_ptr]
-		elif self._source == Type.File:
-			self._start_ptr += chunk_size
-			return self._data.read(chunk_size)
-
-	def read_as_binary(self, chunk_size: int = None) -> bytes:
-		"""Same as read(), but always returns the data in binary format.
-		Practically works exactly as read() for binary streams.
-		For string streams, the method converts the returned data using utf-8 encoding to bytes()."""
-		if self._binary:
-			return self.read(chunk_size)
-		else:
-			return self.read(chunk_size).encode('utf-8')
-
-	def close(self):
-		"""Closes the StreamReader. You can not use its instance afterwards."""
-		if self._source == Type.File and self._data:
-			self._data.close()
-		self._data = None
+from enum import Enum
+from os import path
+from typing import AnyStr
+
+from .Utilities import size_to_kb_mb_string
+
+
+class Type(Enum):
+	Variable = 1
+	File = 2
+
+
+class StreamReader:
+	"""Lightweight stream reader implementation. Data source can be: \n
+	- variable
+	- file"""
+
+	def __init__(self, binary: bool, source: Type, data: AnyStr):
+		"""Initializes StreamReader instance.\n
+		:param binary: True: Binary data, False: ASCII data
+		:param source: Source type for the stream. Variable / File
+		:param data: Depending on the 'binary' and 'source':
+		For source type Variable the data must be either bytes() or str
+		For source type File data must be string with existing file path."""
+		self._source = source
+		self._binary = binary
+		self._start_ptr = 0
+
+		if self._source == Type.Variable:
+			if self._binary:
+				assert isinstance(data, bytes), f'Data must be of bytes type. Actual type: {type(data)}'
+			else:
+				assert isinstance(data, str), f'Data must be of string type. Actual type: {type(data)}'
+			self._data = data
+			self._full_len = len(self._data)
+		elif self._source == Type.File:
+			assert isinstance(data, str), f'Data must be of string type (file path). Actual type: {type(data)}'
+			if not path.isfile(data):
+				raise Exception(f'File does not exist. File path: {data}')
+			self.file_path = data
+			self._data = open(self.file_path, 'rb' if self._binary else 'r')
+			self._full_len = path.getsize(self.file_path)
+		else:
+			raise Exception(f'StreamReader unknown type {source}')
+
+	@classmethod
+	def as_bin_var(cls, data: bytes) -> 'StreamReader':
+		"""Creates new StreamReader from bytes.
+		:param data: [bytes] data for the stream."""
+		return cls(True, Type.Variable, data)
+
+	@classmethod
+	def as_string_var(cls, data: str) -> 'StreamReader':
+		"""Creates new StreamReader from string.
+		:param data: [str] data for the stream."""
+		return cls(False, Type.Variable, data)
+
+	@classmethod
+	def as_bin_file(cls, file_path: str) -> 'StreamReader':
+		"""Creates new StreamReader from binary file. The file must exist at this time.
+		:param file_path: [str] Path to the file."""
+		return cls(True, Type.File, file_path)
+
+	@classmethod
+	def as_text_file(cls, file_path: str) -> 'StreamReader':
+		"""Creates new StreamReader from text file. The file must exist at this time.
+		:param file_path: [str] Path to the file."""
+		return cls(False, Type.File, file_path)
+
+	def __str__(self):
+		if self._source == Type.Variable:
+			mode = 'binary' if self._binary else 'string'
+			return f'StreamReader {mode} data, full size {size_to_kb_mb_string(self._full_len, True)}, remaining size {size_to_kb_mb_string(len(self), True)}'
+		if self._source == Type.File:
+			mode = 'binary' if self._binary else 'text'
+			return f'StreamReader {mode}, full size {size_to_kb_mb_string(self._full_len, True)}, remaining size {size_to_kb_mb_string(len(self), True)}'
+
+	def __len__(self):
+		"""Returns remaining length."""
+		return self._full_len - self._start_ptr
+
+	def __enter__(self):
+		return self
+
+	def __exit__(self, exception_type, exception_value, traceback):
+		self.close()
+
+	@property
+	def full_len(self) -> int:
+		"""Returns original full length."""
+		return self._full_len
+
+	@property
+	def binary(self) -> bool:
+		"""Returns true, if the data provided is binary."""
+		return self._binary
+
+	def read(self, chunk_size: int = None) -> AnyStr:
+		"""Read chunk from the data and moves the data pointer behind it.
+		If the remaining length is smaller than the chunk_size, the method returns the remaining length only.
+		:param chunk_size: chunk to read. If not set, the method reads the entire data."""
+		assert self._data is not None, 'StreamReader buffer is invalid. You have probably closed it already.'
+		chunk_size = len(self) if chunk_size is None else chunk_size
+		chunk_size = min(chunk_size, len(self))
+		if chunk_size < 0:
+			raise ValueError(f'Chunk size can not be negative number: {chunk_size}')
+
+		if self._source == Type.Variable:
+			self._start_ptr += chunk_size
+			return self._data[self._start_ptr - chunk_size: self._start_ptr]
+		elif self._source == Type.File:
+			self._start_ptr += chunk_size
+			return self._data.read(chunk_size)
+
+	def read_as_binary(self, chunk_size: int = None) -> bytes:
+		"""Same as read(), but always returns the data in binary format.
+		Practically works exactly as read() for binary streams.
+		For string streams, the method converts the returned data using utf-8 encoding to bytes()."""
+		if self._binary:
+			return self.read(chunk_size)
+		else:
+			return self.read(chunk_size).encode('utf-8')
+
+	def close(self):
+		"""Closes the StreamReader. You can not use its instance afterwards."""
+		if self._source == Type.File and self._data:
+			self._data.close()
+		self._data = None
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/StreamWriter.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/StreamWriter.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-from enum import Flag
-from typing import AnyStr
-
-from .Utilities import size_to_kb_mb_string
-
-
-class Type(Flag):
-	Variable = 1
-	File = 2
-	FileAppend = 6
-
-
-class StreamWriter:
-	"""Lightweight stream writer implementation. Data target can be: \n
-	- bytes
-	- string
-	- file"""
-
-	def __init__(self, binary: bool, target: Type, meta_data=None):
-		"""Initializes StreamWriter instance.\n
-		:param binary: True: Binary data, False: ASCII data
-		:param target: Target for the stream. Variable / File (FileAppend)
-		:param meta_data: Only valid for File and FileAppend - define file path as string:
-		For Type.File, data must be string with file path. If the file exists, it will be overwritten.
-		For Type.FileAppend, data must be string with file path. If the file exists, it will be appended."""
-		self._binary = binary
-		self._written_len = 0
-		self._target = target
-
-		if Type.Variable in self._target:
-			assert meta_data is None, f'You can not define input meta_data for a Variable StreamWriter.'
-			self._data: AnyStr = bytes() if binary else ''
-		elif Type.File in self._target:
-			assert isinstance(meta_data, str), f'Additional data must be of string type (file path). Actual type: {type(meta_data)}'
-			self._file_path = meta_data
-			mode = 'w' if self._target == Type.File else 'a'
-			mode += 'b' if self._binary else ''
-			self._data = open(self._file_path, mode)
-		else:
-			raise Exception(f'StreamWriter unknown target {target}')
-
-	@classmethod
-	def as_bin_var(cls) -> 'StreamWriter':
-		"""Creates new StreamWriter with bytes variable."""
-		return cls(True, Type.Variable)
-
-	@classmethod
-	def as_string_var(cls) -> 'StreamWriter':
-		"""Creates new StreamWriter with string variable."""
-		return cls(False, Type.Variable)
-
-	@classmethod
-	def as_bin_file(cls, file_path: str, append: bool = False) -> 'StreamWriter':
-		"""Creates new StreamWriter to binary file.
-		:param file_path: [str] Path to the file.
-		:param append: Optional [bool] If True, the content is appended to the existing content."""
-		return cls(True, Type.FileAppend if append else Type.File, file_path)
-
-	@classmethod
-	def as_text_file(cls, file_path: str, append: bool = False) -> 'StreamWriter':
-		"""Creates new StreamWriter to text file.
-		:param file_path: [str] Path to the file.
-		:param append: Optional [bool] If True, the content is appended to the existing content."""
-		return cls(False, Type.FileAppend if append else Type.File, file_path)
-
-	def __str__(self):
-		if Type.Variable in self._target:
-			mode = 'binary' if self._binary else 'string'
-			return f'StreamWriter {mode} variable, current size {size_to_kb_mb_string(len(self), True)}'
-		if Type.File in self._target:
-			mode = 'binary' if self._binary else 'text'
-			append = ' appended' if Type.FileAppend in self._target else ''
-			return f'StreamWriter {mode} file{append}, current{append} size {size_to_kb_mb_string(len(self), True)}, file: {self._file_path}'
-
-	def __len__(self):
-		"""Returns remaining length."""
-		return self._written_len
-
-	def __enter__(self):
-		return self
-
-	def __exit__(self, exception_type, exception_value, traceback):
-		self.close()
-
-	@property
-	def binary(self) -> bool:
-		"""Returns true, if the data held is binary.
-		File streams are always binary."""
-		return self._binary
-
-	def write(self, data: AnyStr) -> None:
-		"""Writes chunk to the stream.
-			- For Type.Bytes data must be bytes.
-			- For Type.String, data must be string.
-			- For Type.File and Type.FileAppend, data must be bytes"""
-		assert self._data is not None, 'StreamWriter buffer is invalid. You have probably closed it already.'
-		if self._binary:
-			assert isinstance(data, bytes), f'Bytes data is required. Actual type: {type(data)}. {self}'
-		else:
-			assert isinstance(data, str), f'String data is required. Actual type: {type(data)}. {self}'
-
-		if Type.Variable in self._target:
-			self._data += data
-		elif Type.File in self._target:
-			self._data.write(data)
-		self._written_len += len(data)
-
-	def switch_to_string_data(self) -> None:
-		"""Switches from binary to string data.
-		For variables, the current content is converted.
-		For files, they are closed and reopened as for appended text writing."""
-		if self._binary is False:
-			return
-		self._binary = False
-		if Type.Variable in self._target:
-			if len(self) == 0:
-				self._data = ''
-			else:
-				# noinspection PyUnresolvedReferences
-				self._data = self._data.decode('utf-8')
-		elif Type.File in self._target:
-			self._data.close()
-			self._data = open(self._file_path, 'a')
-
-	@property
-	def content(self) -> AnyStr:
-		"""Returns content of the writer. Does only work with variable types."""
-		assert Type.Variable in self._target, f'Can not return content for the current {self}'
-		# noinspection PyTypeChecker
-		return self._data
-
-	def close(self) -> None:
-		"""Closes the StreamWriter. You can not use its instance afterwards."""
-		if Type.File in self._target and self._data:
-			self._data.close()
-		self._data = None
+from enum import Flag
+from typing import AnyStr
+
+from .Utilities import size_to_kb_mb_string
+
+
+class Type(Flag):
+	Variable = 1
+	File = 2
+	FileAppend = 6
+
+
+class StreamWriter:
+	"""Lightweight stream writer implementation. Data target can be: \n
+	- bytes
+	- string
+	- file"""
+
+	def __init__(self, binary: bool, target: Type, meta_data=None):
+		"""Initializes StreamWriter instance.\n
+		:param binary: True: Binary data, False: ASCII data
+		:param target: Target for the stream. Variable / File (FileAppend)
+		:param meta_data: Only valid for File and FileAppend - define file path as string:
+		For Type.File, data must be string with file path. If the file exists, it will be overwritten.
+		For Type.FileAppend, data must be string with file path. If the file exists, it will be appended."""
+		self._binary = binary
+		self._written_len = 0
+		self._target = target
+
+		if Type.Variable in self._target:
+			assert meta_data is None, f'You can not define input meta_data for a Variable StreamWriter.'
+			self._data: AnyStr = bytes() if binary else ''
+		elif Type.File in self._target:
+			assert isinstance(meta_data, str), f'Additional data must be of string type (file path). Actual type: {type(meta_data)}'
+			self._file_path = meta_data
+			mode = 'w' if self._target == Type.File else 'a'
+			mode += 'b' if self._binary else ''
+			self._data = open(self._file_path, mode)
+		else:
+			raise Exception(f'StreamWriter unknown target {target}')
+
+	@classmethod
+	def as_bin_var(cls) -> 'StreamWriter':
+		"""Creates new StreamWriter with bytes variable."""
+		return cls(True, Type.Variable)
+
+	@classmethod
+	def as_string_var(cls) -> 'StreamWriter':
+		"""Creates new StreamWriter with string variable."""
+		return cls(False, Type.Variable)
+
+	@classmethod
+	def as_bin_file(cls, file_path: str, append: bool = False) -> 'StreamWriter':
+		"""Creates new StreamWriter to binary file.
+		:param file_path: [str] Path to the file.
+		:param append: Optional [bool] If True, the content is appended to the existing content."""
+		return cls(True, Type.FileAppend if append else Type.File, file_path)
+
+	@classmethod
+	def as_text_file(cls, file_path: str, append: bool = False) -> 'StreamWriter':
+		"""Creates new StreamWriter to text file.
+		:param file_path: [str] Path to the file.
+		:param append: Optional [bool] If True, the content is appended to the existing content."""
+		return cls(False, Type.FileAppend if append else Type.File, file_path)
+
+	def __str__(self):
+		if Type.Variable in self._target:
+			mode = 'binary' if self._binary else 'string'
+			return f'StreamWriter {mode} variable, current size {size_to_kb_mb_string(len(self), True)}'
+		if Type.File in self._target:
+			mode = 'binary' if self._binary else 'text'
+			append = ' appended' if Type.FileAppend in self._target else ''
+			return f'StreamWriter {mode} file{append}, current{append} size {size_to_kb_mb_string(len(self), True)}, file: {self._file_path}'
+
+	def __len__(self):
+		"""Returns remaining length."""
+		return self._written_len
+
+	def __enter__(self):
+		return self
+
+	def __exit__(self, exception_type, exception_value, traceback):
+		self.close()
+
+	@property
+	def binary(self) -> bool:
+		"""Returns true, if the data held is binary.
+		File streams are always binary."""
+		return self._binary
+
+	def write(self, data: AnyStr) -> None:
+		"""Writes chunk to the stream.
+			- For Type.Bytes data must be bytes.
+			- For Type.String, data must be string.
+			- For Type.File and Type.FileAppend, data must be bytes"""
+		assert self._data is not None, 'StreamWriter buffer is invalid. You have probably closed it already.'
+		if self._binary:
+			assert isinstance(data, bytes), f'Bytes data is required. Actual type: {type(data)}. {self}'
+		else:
+			assert isinstance(data, str), f'String data is required. Actual type: {type(data)}. {self}'
+
+		if Type.Variable in self._target:
+			self._data += data
+		elif Type.File in self._target:
+			self._data.write(data)
+		self._written_len += len(data)
+
+	def switch_to_string_data(self) -> None:
+		"""Switches from binary to string data.
+		For variables, the current content is converted.
+		For files, they are closed and reopened as for appended text writing."""
+		if self._binary is False:
+			return
+		self._binary = False
+		if Type.Variable in self._target:
+			if len(self) == 0:
+				self._data = ''
+			else:
+				# noinspection PyUnresolvedReferences
+				self._data = self._data.decode('utf-8')
+		elif Type.File in self._target:
+			self._data.close()
+			self._data = open(self._file_path, 'a')
+
+	@property
+	def content(self) -> AnyStr:
+		"""Returns content of the writer. Does only work with variable types."""
+		assert Type.Variable in self._target, f'Can not return content for the current {self}'
+		# noinspection PyTypeChecker
+		return self._data
+
+	def close(self) -> None:
+		"""Closes the StreamWriter. You can not use its instance afterwards."""
+		if Type.File in self._target and self._data:
+			self._data.close()
+		self._data = None
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/StructBase.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/StructBase.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from .Types import DataType
-
-
-class StructBase:
-	"""Base class for all the driver's argument structures."""
-	def __init__(self, owner):
-		self.__meta_args_link = dict()
-		ix = 0
-		for arg in self.__get_meta_args_list(owner):
-			arg.argument_ix = ix
-			ix += 1
-
-			if arg.data_type == DataType.Enum or arg.data_type == DataType.EnumList:
-				assert arg.enum_type, f"Struct Argument '{arg.name}' is of enum type, you must define the parameter 'enum_type'"
-			else:
-				assert not arg.enum_type, f"Struct Argument '{arg.name}' data type is '{arg.data_type.name}'. You must set the parameter 'enum_type' to None"
-
-			if arg.is_optional:
-				# set all optional values to None
-				setattr(self, arg.name, None)
-			else:
-				# set all mandatory values to their default values
-				default = arg.data_type.get_default_value(arg.enum_type)
-				setattr(self, arg.name, default)
-
-	# noinspection PyMethodMayBeStatic
-	def __get_meta_args_list(self, owner):
-		args_list = getattr(owner, f'_{owner.__class__.__name__}__meta_args_list')
-		return args_list
+from .Types import DataType
+
+
+class StructBase:
+	"""Base class for all the driver's argument structures."""
+	def __init__(self, owner):
+		self.__meta_args_link = dict()
+		ix = 0
+		for arg in self.__get_meta_args_list(owner):
+			arg.argument_ix = ix
+			ix += 1
+
+			if arg.data_type == DataType.Enum or arg.data_type == DataType.EnumList:
+				assert arg.enum_type, f"Struct Argument '{arg.name}' is of enum type, you must define the parameter 'enum_type'"
+			else:
+				assert not arg.enum_type, f"Struct Argument '{arg.name}' data type is '{arg.data_type.name}'. You must set the parameter 'enum_type' to None"
+
+			if arg.is_optional:
+				# set all optional values to None
+				setattr(self, arg.name, None)
+			else:
+				# set all mandatory values to their default values
+				default = arg.data_type.get_default_value(arg.enum_type)
+				setattr(self, arg.name, default)
+
+	# noinspection PyMethodMayBeStatic
+	def __get_meta_args_list(self, owner):
+		args_list = getattr(owner, f'_{owner.__class__.__name__}__meta_args_list')
+		return args_list
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/Types.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/Types.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-from enum import Enum, auto
-from typing import Any
-
-
-class DataType(Enum):
-	"""Data type of a variable in the driver."""
-	String = auto()
-	RawString = auto()
-	Integer = auto()
-	IntegerExt = auto()
-	Boolean = auto()
-	Float = auto()
-	FloatExt = auto()
-	Enum = auto()
-	StringList = auto()
-	RawStringList = auto()
-	IntegerList = auto()
-	IntegerExtList = auto()
-	BooleanList = auto()
-	FloatList = auto()
-	FloatExtList = auto()
-	EnumList = auto()
-
-	@property
-	def is_list(self) -> bool:
-		"""Returns True, if the data type is a list."""
-		return self in frozenset(
-			{
-				DataType.StringList,
-				DataType.RawStringList,
-				DataType.IntegerList,
-				DataType.IntegerExtList,
-				DataType.BooleanList,
-				DataType.FloatList,
-				DataType.FloatExtList,
-				DataType.EnumList
-			})
-
-	@property
-	def is_scalar(self) -> bool:
-		"""Returns True, if the data type is a scalar."""
-		return not self.is_list
-
-	@property
-	def is_enum(self) -> bool:
-		"""Returns True, if the data type is enum or enum array."""
-		return self == DataType.Enum or self == DataType.EnumList
-
-	@property
-	def is_raw_string(self) -> bool:
-		"""Returns True for raw string and raw string list."""
-		return self == DataType.RawString or self == DataType.RawStringList
-
-	@property
-	def is_boolean(self) -> bool:
-		"""Returns True for boolean and boolean list."""
-		return self == DataType.Boolean or self == DataType.BooleanList
-
-	@property
-	def is_string(self) -> bool:
-		"""Returns True for string and string list."""
-		return self == DataType.String or self == DataType.StringList
-
-	@property
-	def element_type(self):
-		"""For lists, the property returns type of the element.
-		For scalars, it returns the same type."""
-		if self.is_scalar:
-			return self
-		elif self == DataType.StringList:
-			return DataType.String
-		elif self == DataType.RawStringList:
-			return DataType.RawString
-		elif self == DataType.RawStringList:
-			return DataType.RawString
-		elif self == DataType.BooleanList:
-			return DataType.Boolean
-		elif self == DataType.IntegerList:
-			return DataType.Integer
-		elif self == DataType.IntegerExtList:
-			return DataType.IntegerExt
-		elif self == DataType.FloatList:
-			return DataType.Float
-		elif self == DataType.FloatExtList:
-			return DataType.FloatExt
-		elif self == DataType.EnumList:
-			return DataType.Enum
-
-	def get_default_value(self, enm: Enum = None) -> Any:
-		"""Returns default value for the current type.
-		If the data type is Enum or EnumString, you have to provide the enum class."""
-		if self.is_list:
-			return []
-		if self == DataType.RawString:
-			return ''
-		elif self == DataType.String:
-			return ''
-		elif self == DataType.Boolean:
-			return False
-		elif self == DataType.Integer:
-			return 0
-		elif self == DataType.IntegerExt:
-			return 0
-		elif self == DataType.Float:
-			return 0.0
-		elif self == DataType.FloatExt:
-			return 0.0
-		elif self == DataType.Enum:
-			return enm(0)
+from enum import Enum, auto
+from typing import Any
+
+
+class DataType(Enum):
+	"""Data type of a variable in the driver."""
+	String = auto()
+	RawString = auto()
+	Integer = auto()
+	IntegerExt = auto()
+	Boolean = auto()
+	Float = auto()
+	FloatExt = auto()
+	Enum = auto()
+	StringList = auto()
+	RawStringList = auto()
+	IntegerList = auto()
+	IntegerExtList = auto()
+	BooleanList = auto()
+	FloatList = auto()
+	FloatExtList = auto()
+	EnumList = auto()
+
+	@property
+	def is_list(self) -> bool:
+		"""Returns True, if the data type is a list."""
+		return self in frozenset(
+			{
+				DataType.StringList,
+				DataType.RawStringList,
+				DataType.IntegerList,
+				DataType.IntegerExtList,
+				DataType.BooleanList,
+				DataType.FloatList,
+				DataType.FloatExtList,
+				DataType.EnumList
+			})
+
+	@property
+	def is_scalar(self) -> bool:
+		"""Returns True, if the data type is a scalar."""
+		return not self.is_list
+
+	@property
+	def is_enum(self) -> bool:
+		"""Returns True, if the data type is enum or enum array."""
+		return self == DataType.Enum or self == DataType.EnumList
+
+	@property
+	def is_raw_string(self) -> bool:
+		"""Returns True for raw string and raw string list."""
+		return self == DataType.RawString or self == DataType.RawStringList
+
+	@property
+	def is_boolean(self) -> bool:
+		"""Returns True for boolean and boolean list."""
+		return self == DataType.Boolean or self == DataType.BooleanList
+
+	@property
+	def is_string(self) -> bool:
+		"""Returns True for string and string list."""
+		return self == DataType.String or self == DataType.StringList
+
+	@property
+	def element_type(self):
+		"""For lists, the property returns type of the element.
+		For scalars, it returns the same type."""
+		if self.is_scalar:
+			return self
+		elif self == DataType.StringList:
+			return DataType.String
+		elif self == DataType.RawStringList:
+			return DataType.RawString
+		elif self == DataType.RawStringList:
+			return DataType.RawString
+		elif self == DataType.BooleanList:
+			return DataType.Boolean
+		elif self == DataType.IntegerList:
+			return DataType.Integer
+		elif self == DataType.IntegerExtList:
+			return DataType.IntegerExt
+		elif self == DataType.FloatList:
+			return DataType.Float
+		elif self == DataType.FloatExtList:
+			return DataType.FloatExt
+		elif self == DataType.EnumList:
+			return DataType.Enum
+
+	def get_default_value(self, enm: Enum = None) -> Any:
+		"""Returns default value for the current type.
+		If the data type is Enum or EnumString, you have to provide the enum class."""
+		if self.is_list:
+			return []
+		if self == DataType.RawString:
+			return ''
+		elif self == DataType.String:
+			return ''
+		elif self == DataType.Boolean:
+			return False
+		elif self == DataType.Integer:
+			return 0
+		elif self == DataType.IntegerExt:
+			return 0
+		elif self == DataType.Float:
+			return 0.0
+		elif self == DataType.FloatExt:
+			return 0.0
+		elif self == DataType.Enum:
+			return enm(0)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/Utilities.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/Utilities.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-from enum import Flag
-from typing import Tuple
-
-
-class TrimStringMode(Flag):
-	"""Trimming mode for strings."""
-	white_chars_only = 1
-	white_chars_single_quotes = 2
-	white_chars_double_quotes = 3
-	white_chars_all_quotes = 4
-
-
-def trim_str_response(text: str, mode=TrimStringMode.white_chars_all_quotes) -> str:
-	"""Trims instrument string response.
-	In modes white_chars_all_quotes, white_chars_single_quotes, white_chars_double_quotes:
-	All the symmetrical leading and trailing quotation marks are trimmed,
-	but only if there are none in the remaining text."""
-	first_sq_ix = -1
-	first_dq_ix = -1
-	rem_sq = True if (mode == TrimStringMode.white_chars_all_quotes or mode == TrimStringMode.white_chars_single_quotes) else False
-	rem_dq = True if (mode == TrimStringMode.white_chars_all_quotes or mode == TrimStringMode.white_chars_double_quotes) else False
-
-	if not text:
-		return text
-	text = text.strip()
-	if rem_sq and text == "''":
-		return ''
-	if rem_dq and text == '""':
-		return ''
-	start_ix = 0
-	end_ix: int = len(text) - 1
-	if end_ix - 2 < start_ix:
-		return text
-	if mode is not TrimStringMode.white_chars_only:
-		# Loop to cut the outer paired quotation marks
-		trimmed = True
-		while trimmed:
-			trimmed = False
-			if rem_sq and text[start_ix] == "'" and text[end_ix] == "'":
-				if first_sq_ix < 0:
-					first_sq_ix = start_ix
-				start_ix += 1
-				end_ix -= 1
-				trimmed = True
-			if end_ix - 2 < start_ix:
-				break
-			if rem_dq and text[start_ix] == '"' and text[end_ix] == '"':
-				if first_dq_ix < 0:
-					first_dq_ix = start_ix
-				start_ix += 1
-				end_ix -= 1
-				trimmed = True
-			if end_ix - 2 < start_ix:
-				break
-		if start_ix == 0:
-			return text
-
-		final_cut_ix = start_ix
-		shortened_text = text[start_ix: -start_ix]
-		if first_sq_ix >= 0 and "'" in shortened_text:
-			# The cut quotes are also in the shortened string, do not removed the quotes, and set the cutting to start_ix
-			final_cut_ix = first_sq_ix
-		if first_dq_ix >= 0 and '"' in shortened_text:
-			if final_cut_ix > first_dq_ix:
-				final_cut_ix = first_dq_ix
-
-		if final_cut_ix == 0:
-			return text
-
-		text = text[final_cut_ix: -final_cut_ix]
-
-	return text
-
-
-def truncate_string_from_end(string: str, max_len: int) -> str:
-	"""If the string len is below the max_len, the function returns the same string.
-	If the string is above the max len, the function returns only the last max_len characters plus '...' at the beginning."""
-	if len(string) <= max_len:
-		return string
-	return f'Last {max_len} chars: "...{string[-max_len:]}"'
-
-
-def get_plural_string(word: str, amount: int) -> str:
-	"""Returns singular or plural of the word depending on the amount.
-	Example:
-		word = 'piece', amount = 0 -> '0 pieces'
-		word = 'piece', amount = 1 -> '1 piece'
-		word = 'piece', amount = 5 -> '5 pieces'"""
-	if amount == 1:
-		return f'1 {word}'
-	else:
-		return f'{amount} {word}s'
-
-
-def parse_token_to_key_and_value(token: str) -> Tuple[str, str]:
-	"""Parses entered string to name and value with the delimiter '='.
-	If the token is empty: name = None, value = None.
-	If the '=' is not found: name = token, value = None.
-	name is trimmed for white spaces.
-	value is trimmed with trim_str_response()."""
-	token = token.strip()
-	if not token:
-		# noinspection PyTypeChecker
-		return None, None
-	if '=' in token:
-		data = token.split('=')
-		name = data[0].strip()
-		value = trim_str_response(data[1])
-		return name, value
-
-	# noinspection PyTypeChecker
-	return token.strip(), None
-
-
-def size_to_kb_mb_string(data_size: int, as_additional_info: bool = False) -> str:
-	"""Returns human-readable string with kilobytes or megabytes depending on the data_size range. \n
-		:param data_size: data size in bytes to convert
-		:param as_additional_info:
-		if True, the dynamic data appear in round bracket after the number in bytes. e.g. '12345678 bytes (11.7 MB)'
-		if False, only the dynamic data is returned e.g. '11.7 MB' """
-	if data_size < 1024:
-		as_additional_info = False
-		dynamic = f'{data_size} bytes'
-	elif data_size < 1048576:
-		dynamic = f'{data_size / 1024:0.1f} kB'
-	else:
-		dynamic = f'{data_size / 1048576:0.1f} MB'
-
-	if as_additional_info:
-		return f'{data_size} bytes ({dynamic})'
-	else:
-		return dynamic
-
-
-def calculate_chunks_count(data_size: int, chunk_size: int) -> int:
-	"""Returns number of chunks needed to transfer the data_size split to maximum of chunk_size blocks. \n
-	:param data_size: total data size
-	:param chunk_size: maximum size of one block"""
-	return (data_size // chunk_size) + (1 if (data_size % chunk_size) > 0 else 0)
+from enum import Flag
+from typing import Tuple
+
+
+class TrimStringMode(Flag):
+	"""Trimming mode for strings."""
+	white_chars_only = 1
+	white_chars_single_quotes = 2
+	white_chars_double_quotes = 3
+	white_chars_all_quotes = 4
+
+
+def trim_str_response(text: str, mode=TrimStringMode.white_chars_all_quotes) -> str:
+	"""Trims instrument string response.
+	In modes white_chars_all_quotes, white_chars_single_quotes, white_chars_double_quotes:
+	All the symmetrical leading and trailing quotation marks are trimmed,
+	but only if there are none in the remaining text."""
+	first_sq_ix = -1
+	first_dq_ix = -1
+	rem_sq = True if (mode == TrimStringMode.white_chars_all_quotes or mode == TrimStringMode.white_chars_single_quotes) else False
+	rem_dq = True if (mode == TrimStringMode.white_chars_all_quotes or mode == TrimStringMode.white_chars_double_quotes) else False
+
+	if not text:
+		return text
+	text = text.strip()
+	if rem_sq and text == "''":
+		return ''
+	if rem_dq and text == '""':
+		return ''
+	start_ix = 0
+	end_ix: int = len(text) - 1
+	if end_ix - 2 < start_ix:
+		return text
+	if mode is not TrimStringMode.white_chars_only:
+		# Loop to cut the outer paired quotation marks
+		trimmed = True
+		while trimmed:
+			trimmed = False
+			if rem_sq and text[start_ix] == "'" and text[end_ix] == "'":
+				if first_sq_ix < 0:
+					first_sq_ix = start_ix
+				start_ix += 1
+				end_ix -= 1
+				trimmed = True
+			if end_ix - 2 < start_ix:
+				break
+			if rem_dq and text[start_ix] == '"' and text[end_ix] == '"':
+				if first_dq_ix < 0:
+					first_dq_ix = start_ix
+				start_ix += 1
+				end_ix -= 1
+				trimmed = True
+			if end_ix - 2 < start_ix:
+				break
+		if start_ix == 0:
+			return text
+
+		final_cut_ix = start_ix
+		shortened_text = text[start_ix: -start_ix]
+		if first_sq_ix >= 0 and "'" in shortened_text:
+			# The cut quotes are also in the shortened string, do not removed the quotes, and set the cutting to start_ix
+			final_cut_ix = first_sq_ix
+		if first_dq_ix >= 0 and '"' in shortened_text:
+			if final_cut_ix > first_dq_ix:
+				final_cut_ix = first_dq_ix
+
+		if final_cut_ix == 0:
+			return text
+
+		text = text[final_cut_ix: -final_cut_ix]
+
+	return text
+
+
+def truncate_string_from_end(string: str, max_len: int) -> str:
+	"""If the string len is below the max_len, the function returns the same string.
+	If the string is above the max len, the function returns only the last max_len characters plus '...' at the beginning."""
+	if len(string) <= max_len:
+		return string
+	return f'Last {max_len} chars: "...{string[-max_len:]}"'
+
+
+def get_plural_string(word: str, amount: int) -> str:
+	"""Returns singular or plural of the word depending on the amount.
+	Example:
+		word = 'piece', amount = 0 -> '0 pieces'
+		word = 'piece', amount = 1 -> '1 piece'
+		word = 'piece', amount = 5 -> '5 pieces'"""
+	if amount == 1:
+		return f'1 {word}'
+	else:
+		return f'{amount} {word}s'
+
+
+def parse_token_to_key_and_value(token: str) -> Tuple[str, str]:
+	"""Parses entered string to name and value with the delimiter '='.
+	If the token is empty: name = None, value = None.
+	If the '=' is not found: name = token, value = None.
+	name is trimmed for white spaces.
+	value is trimmed with trim_str_response()."""
+	token = token.strip()
+	if not token:
+		# noinspection PyTypeChecker
+		return None, None
+	if '=' in token:
+		data = token.split('=')
+		name = data[0].strip()
+		value = trim_str_response(data[1])
+		return name, value
+
+	# noinspection PyTypeChecker
+	return token.strip(), None
+
+
+def size_to_kb_mb_string(data_size: int, as_additional_info: bool = False) -> str:
+	"""Returns human-readable string with kilobytes or megabytes depending on the data_size range. \n
+		:param data_size: data size in bytes to convert
+		:param as_additional_info:
+		if True, the dynamic data appear in round bracket after the number in bytes. e.g. '12345678 bytes (11.7 MB)'
+		if False, only the dynamic data is returned e.g. '11.7 MB' """
+	if data_size < 1024:
+		as_additional_info = False
+		dynamic = f'{data_size} bytes'
+	elif data_size < 1048576:
+		dynamic = f'{data_size / 1024:0.1f} kB'
+	else:
+		dynamic = f'{data_size / 1048576:0.1f} MB'
+
+	if as_additional_info:
+		return f'{data_size} bytes ({dynamic})'
+	else:
+		return dynamic
+
+
+def calculate_chunks_count(data_size: int, chunk_size: int) -> int:
+	"""Returns number of chunks needed to transfer the data_size split to maximum of chunk_size blocks. \n
+	:param data_size: total data size
+	:param chunk_size: maximum size of one block"""
+	return (data_size // chunk_size) + (1 if (data_size % chunk_size) > 0 else 0)
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/VisaSession.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/VisaSession.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1111 +1,1131 @@
-import time
-from enum import Enum, Flag
-from typing import Tuple, Callable, AnyStr
-import os.path
-import re
-import threading
-
-# noinspection PyPackageRequirements
-import pyvisa
-
-from .VisaPluginSocketIo import ResourceManager, SocketIo
-from . import InstrumentSettings, InstrumentErrors, Conversions as Conv
-from .InstrumentSettings import WaitForOpcMode, InstrViClearMode as ViClearMode
-from .StreamReader import StreamReader
-from .StreamWriter import StreamWriter
-from .Utilities import size_to_kb_mb_string, calculate_chunks_count
-import platform
-import struct
-
-
-class SessionKind(Enum):
-	"""Visa instrument session type."""
-	unsupported = 0
-	gpib = 1
-	serial = 2
-	vxi11 = 3
-	socket = 5
-	usb = 6
-	rs_nrp = 7
-
-
-class ReadDataType(Enum):
-	"""Data type returned by the instrument."""
-	unknown = 0
-	ascii = 1
-	null = 2
-	bin_known_len = 3
-	bin_unknown_len = 4
-
-
-class StatusByte(Flag):
-	"""Status Byte flags."""
-	NONE = 0x00
-	error_queue_not_empty = 0x04
-	questionable_status_reg = 0x08
-	message_available = 0x10
-	event_status_byte = 0x20
-	request_service = 0x40
-	operation_status_reg = 0x80
-
-
-class EventStatusRegister(Flag):
-	"""Event Status Register flags."""
-	null = 0x00
-	operation_complete = 0x01
-
-
-# noinspection PyUnresolvedReferences
-class VisaSession(object):
-	"""Extended VISA class."""
-
-	def __init__(self, resource_name: str, settings: InstrumentSettings, direct_session=None):
-		self.reusing_session = direct_session is not None
-		# noinspection PyTypeChecker
-		self._data_chunk_size: int = None
-		self._std_bin_block_header_max_len: int = 999999999
-		self._lock = None
-		self.disable_opc_query: bool = settings.disable_opc_query
-		self.last_status = None
-		self.visa_library_name = None
-
-		# Implemented for interface compatibility with VisaSessionSim
-		self.cached_to_stream = False
-
-		# Event handlers
-		# noinspection PyTypeChecker
-		self.on_read_chunk_handler: Callable = None
-		"""If assigned a handler, the VisaSession sends it event on each read chunk transfer."""
-		# noinspection PyTypeChecker
-		self.on_write_chunk_handler: Callable = None
-		"""If assigned a handler, the VisaSession sends it event on each write chunk transfer."""
-		self.io_events_include_data: bool = False
-		"""If true, the VisaSession events sent to on_read_chunk_handler and on_write_chunk_handler contain transferred data."""
-
-		if self.reusing_session:
-			# Reuse the session
-			assert isinstance(direct_session, pyvisa.Resource) or isinstance(direct_session, SocketIo), f"Direct_session must be a VISA resource object. Actual type: '{type(direct_session)}', value: '{direct_session}'"
-			self._session = direct_session
-			self._resource_name = self._session.resource_name
-		else:
-			# Create new session
-			# Check resource_name for the trailing (SelectVisa=..)
-			pure_resource_name, visa_select = self._get_pure_resource_name(resource_name)
-			if settings.visa_select is not None:
-				visa_select = settings.visa_select
-			self._rm = VisaSession.get_resource_manager(visa_select)
-			self.manufacturer = self._get_visa_manufacturer()
-
-			# Resource manager opening
-			try:
-				self._session = self._rm.open_resource(pure_resource_name)
-			except pyvisa.VisaIOError as e:
-				if e.error_code != pyvisa.constants.StatusCode.error_resource_not_found:
-					raise e
-				message = e.description
-				message += f"\nLibrary: {self._rm.visalib}\nManufacturer: {self.manufacturer}\nResource Name: '{resource_name}'"
-				raise InstrumentErrors.ResourceError(resource_name, message)
-			self._resource_name = resource_name
-
-		# Decide, whether to create a new thread lock or the existing one from the session
-		if hasattr(self._session, 'session_thread_rlock'):
-			rlock = self._session.session_thread_rlock
-			if isinstance(rlock, type(threading.RLock())):
-				self.assign_lock(rlock)
-		if self.get_lock() is None:
-			# The existing session did not have a thread lock, assign a new one
-			self.assign_lock(threading.RLock())
-
-		self._interface_type = SessionKind.unsupported
-		if self._session.interface_type == pyvisa.constants.InterfaceType.gpib or self._session.interface_type == pyvisa.constants.InterfaceType.gpib:
-			self._interface_type = SessionKind.gpib
-
-		elif self._session.interface_type == pyvisa.constants.InterfaceType.rsnrp:
-			self._interface_type = SessionKind.rs_nrp
-
-		elif self._session.interface_type == pyvisa.constants.InterfaceType.asrl:
-			self._interface_type = SessionKind.serial
-
-		elif self._session.interface_type == pyvisa.constants.InterfaceType.usb:
-			# Check whether it is not the NRP-Z
-			intf_type = self._session.get_visa_attribute(pyvisa.constants.VI_ATTR_INTF_TYPE)
-			if intf_type == pyvisa.constants.InterfaceType.rsnrp:
-				self._interface_type = SessionKind.rs_nrp
-
-		elif self._session.interface_type == pyvisa.constants.InterfaceType.tcpip:
-			self._interface_type = SessionKind.vxi11
-			if self._session.resource_class == 'SOCKET':
-				self._interface_type = SessionKind.socket
-
-		# Specifics for different interfaces
-		self._assure_write_with_tc = settings.assure_write_with_tc
-		self._term_char = settings.term_char
-		self._term_char_bin = self._term_char.encode('utf-8')
-		self._session.write_termination = ''
-		self.vxi_capable = True
-
-		if self._interface_type == SessionKind.serial:
-			self._session.read_termination = self._term_char
-			self.vxi_capable = False
-			self._assure_write_with_tc = True
-		elif self._interface_type == SessionKind.socket:
-			self._session.read_termination = self._term_char
-			self.vxi_capable = False
-			self._assure_write_with_tc = True
-		else:
-			self._session.read_termination = ''
-
-		# NRP-Z specific settings
-		if self.is_rsnrp_session():
-			self.disable_opc_query = True
-			# NRP-Z does not support chunk reading, therefore the segment must be in one piece
-			settings.io_segment_size = 1000000
-			self.vxi_capable = False
-
-		self.write_delay = settings.write_delay
-		self.read_delay = settings.read_delay
-		self._viclear_exe_mode = settings.viclear_exe_mode
-		self._opc_wait_mode = settings.opc_wait_mode
-
-		# Parameters that need to be coerced based on Vxi-capability
-		if self.vxi_capable:
-			self._add_term_char_to_write_bin_block = settings.add_term_char_to_write_bin_block
-		else:
-			self._add_term_char_to_write_bin_block = True
-
-		# Changeable settings
-		self.opc_timeout = 10000 if settings.opc_timeout == 0 else settings.opc_timeout
-		self.visa_timeout = settings.visa_timeout
-		self._session.chunk_size = settings.io_segment_size
-		self._data_chunk_size = settings.io_segment_size
-
-		# Must call the VISA viClear() before the any communication with the instrument
-		self.clear()
-
-		# Further steps are for NRP-Z session not valid
-		if self.is_rsnrp_session():
-			return
-
-		# Clear instrument status
-		self.write("*CLS")
-		if self.vxi_capable:
-			stb = self._read_stb()
-			if stb & StatusByte.message_available:
-				self._flush_junk_data()
-
-		# Apply settings for ESE and SRE, plus coerce the _opcWaitMode if necessary
-		self._opc_wait_mode = self._set_regs_ese_sre(self._opc_wait_mode)
-
-	@staticmethod
-	def _get_pure_resource_name(resource_name: str):
-		"""Returns pure resource name stripped of the (SelectVisa) part and the visa_select string"""
-		m = re.search(r'(.+)\(SelectVisa=([^),]+)\)', resource_name)
-		if not m:
-			return resource_name, None
-		resource_name = m.group(1).strip()
-		visa_select = m.group(2).strip()
-		return resource_name, visa_select
-
-	@classmethod
-	def get_resource_manager(cls, visa_select: str) -> pyvisa.ResourceManager:
-		"""Returns resource manager for the desired VISA implementation"""
-		operating_system = platform.system().lower()
-		bittness = struct.calcsize("P") * 8
-		if visa_select is None or visa_select in ['@default', '@standard', 'default', 'standard', 'defaultvisa', 'standardvisa', '@defaultvisa', '@standardvisa']:
-			return pyvisa.ResourceManager()
-		if visa_select.lower() in ['@ni', 'ni', 'visa-ni', 'nivisa', 'ni-visa', 'nationalinstruments', 'nationalinstrumentsvisa']:
-			return pyvisa.ResourceManager('@ni')
-		if visa_select.lower() in ['@py', 'pyvisa', 'visa-py', 'pyvisa-py']:
-			return pyvisa.ResourceManager('@py')
-		if 'rohde&schwarz' in visa_select.lower() or 'rohdeschwarz' in visa_select.lower() or visa_select.lower() == 'rsvisa' or visa_select.lower() == 'rs' or visa_select.lower() == 'r&s':
-			if operating_system == 'windows':
-				if bittness == 32:
-					visa_select = r'c:\Windows\SysWOW64\RsVisa32.dll'
-				else:
-					visa_select = r'c:\Windows\system32\RsVisa32.dll'
-				return pyvisa.ResourceManager(visa_select)
-			elif operating_system == 'linux':
-				# The default install location may be different
-				# for debian/red hat/opensuse derived distributions
-				check_visa = [f'/usr/lib{bittness}/librsvisa.so', r'/usr/lib/librsvisa.so']
-				for check in check_visa:
-					if os.path.isfile(check):
-						return pyvisa.ResourceManager(check)
-
-		if visa_select.lower() in ['socketio', 'socket', 'none']:
-			return ResourceManager()
-		return pyvisa.ResourceManager(visa_select)
-
-	def _get_visa_manufacturer(self) -> str:
-		"""Returns manufacturer of the current VISA"""
-		if hasattr(self._rm, 'VisaManufacturerName'):
-			return self._rm.VisaManufacturerName
-		try:
-			return self._rm.visalib.get_attribute(self._rm.session, pyvisa.constants.VI_ATTR_RSRC_MANF_NAME)[0]
-		except TypeError:
-			return self._rm.visalib.__class__.__name__
-
-	def is_rsnrp_session(self) -> bool:
-		"""Returns True, if the current session is a NRP-Z session"""
-		return self._interface_type == SessionKind.rs_nrp
-
-	def assign_lock(self, lock: threading.RLock) -> None:
-		"""Assigns the provided thread lock by setting the pyvisa runtime session attribute 'session_thread_rlock'
-		This is done, because if the session is to be entered as an existing session to another RsInstrument object,
-		the lock must be shared as well. The lock is only used by the parent class Instrument."""
-		setattr(self._session, 'session_thread_rlock', lock)
-		self._lock = lock
-
-	def get_lock(self) -> threading.RLock:
-		"""Returns the current RLock object."""
-		return self._lock
-
-	@property
-	def visa_timeout(self) -> int:
-		"""See the visa_timeout.setter."""
-		return int(self._session.timeout)
-
-	@visa_timeout.setter
-	def visa_timeout(self, value: int) -> None:
-		"""Sets / Gets visa IO timeout in milliseconds."""
-		self._session.timeout = int(value)
-
-	@property
-	def data_chunk_size(self) -> int:
-		"""Returns max chunk size of one data block."""
-		return self._data_chunk_size
-
-	@data_chunk_size.setter
-	def data_chunk_size(self, chunk_size: int) -> None:
-		"""Sets the maximum size of one block transferred during write/read operations."""
-		self._data_chunk_size = int(chunk_size)
-		self._session.chunk_size = int(chunk_size)
-
-	def _resolve_opc_timeout(self, timeout: int) -> int:
-		"""Resolves entered timeout value - if the input value is less than 1, it is replaces with opc_timeout."""
-		if timeout is None or timeout < 1:
-			return self.opc_timeout
-		else:
-			return timeout
-
-	def _set_regs_ese_sre(self, mode: WaitForOpcMode) -> WaitForOpcMode:
-		"""Based on the WaitForOpcMode, it sets the ESE and SRE register masks.
-		Returns coerced WaitForOpcMode."""
-		# Set the SRE and ESE registers accordingly
-		# No SRE is supported
-		self._set_ese_mask(EventStatusRegister.operation_complete)
-		self._set_sre_mask(StatusByte.NONE)
-		return mode
-
-	def _set_ese_mask(self, mask: EventStatusRegister, reset: bool = True) -> None:
-		"""Sends *ESE command with mask parameter."""
-		if reset is False:
-			current_value = int(self._query_str_no_events("*ESE?"))
-			mask = current_value | mask.value
-		self.write("*ESE %d" % mask.value)
-
-	def _set_sre_mask(self, mask: StatusByte, reset: bool = True) -> None:
-		"""Sends *SRE command with StatusByte mask parameter."""
-		if reset is False:
-			current_value = int(self._query_str_no_events("*SRE?"))
-			mask = current_value | mask.value
-		# Also affect the _opc_wait_mode:
-		# If the mask has event_status_byte == false, and the _opc_wait_mode is service_request, set it to stb_poll
-		# If the mask has event_status_byte == true, do not change anything
-		self.write("*SRE %d" % mask.value)
-
-	def _write_and_poll_stb_vxi(self, command: str, is_query: bool, timeout: int, end_mask: StatusByte) -> StatusByte:
-		"""Reads Status Byte Register and ends if the ESB bit (5) is set to 1.
-		Also works with the SOCKET and SERIAL interface by sending *STB? query.
-		In that case however, command cannot be a query.
-		Returns the last read Status Byte value."""
-		timeout_secs = timeout / 1000
-		self.clear_before_read()
-		if command.endswith(self._term_char):
-			command = command.rstrip(self._term_char)
-		self.write(command + ';*OPC')
-		# Use catch to return the VISA Timeout back
-		start = time.time()
-		# STB polling loop
-		while True:
-			stb = self._read_stb()
-			elapsed = self._polling_delay(start)
-			if elapsed > timeout_secs:
-				self._narrow_down_opc_tout_error(command, is_query, timeout)
-			if end_mask & stb:
-				break
-		return stb
-
-	def _write_and_poll_stb_non_vxi(self, command: str, timeout: int, end_mask: StatusByte) -> StatusByte:
-		"""Queries Status Byte Register (*STB?) and ends if the ESB bit (5) is set to 1.
-			The command must not be a query. Also works with the SOCKET and SERIAL interface.
-			Returns the last read Status Byte value."""
-		timeout_secs = timeout / 1000
-		self.clear_before_read()
-		if command.endswith(self._term_char):
-			command = command.rstrip(self._term_char)
-		self.write(command + ';*OPC')
-		start = time.time()
-		# STB polling loop
-		while True:
-			stb = self._query_stb()
-			elapsed = self._polling_delay(start)
-			if elapsed > timeout_secs:
-				InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout)
-			if stb & end_mask:
-				break
-		return stb
-
-	def _narrow_down_opc_tout_error(self, command: str, is_query: bool, timeout: int) -> None:
-		"""Called by the _write_and_poll_stb_vxi when the timeout expires.
-		The method tries to closer identify the cause of the timeout."""
-		stb = self._read_stb()
-		timeout = self._resolve_opc_timeout(timeout)
-		if is_query:
-			if stb & StatusByte.error_queue_not_empty:
-				self.clear()
-				context = f"Sending query '{command.strip()}' with OPC Wait resulted in timeout. OPC Timeout is set to {timeout} ms. Additionally, "
-				InstrumentErrors.assert_no_instrument_status_errors(self._resource_name, self.query_all_syst_errors(), context)
-			InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout, f"Sending query '{command.strip()}'.")
-		else:
-			if stb & StatusByte.error_queue_not_empty:
-				self.clear()
-				context = f"Sending command '{command.strip()}' with OPC Wait resulted in timeout. OPC Timeout is set to {timeout} ms. Additionally, "
-				InstrumentErrors.assert_no_instrument_status_errors(self._resource_name, self.query_all_syst_errors(), context)
-			InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout, f"Sending command '{command.strip()}'.")
-
-	def _narrow_down_io_tout_error(self, context: str) -> None:
-		"""Called internally after IOTimeoutException can narrow down the error to more specific exception."""
-		if self.vxi_capable:
-			stb = self._read_stb()
-		else:
-			# Non-Vxi session
-			old_tout = self.visa_timeout
-			try:
-				self.visa_timeout = 500
-				stb = self._query_stb()
-			finally:
-				self.visa_timeout = old_tout
-		context = context + f"VISA Timeout error occurred ({self.visa_timeout} milliseconds)"
-		if stb & StatusByte.error_queue_not_empty:
-			InstrumentErrors.assert_no_instrument_status_errors(self._resource_name, self.query_all_syst_errors(), context + " and ...")
-		# In case the previous exception is not thrown
-		raise InstrumentErrors.TimeoutException(context)
-
-	def _polling_delay(self, start):
-		"""Generates progressive polling delay."""
-
-		elapsed = time.time() - start
-		if self._opc_wait_mode == WaitForOpcMode.stb_poll:
-			if elapsed < 0.01:
-				return elapsed
-			if elapsed < 0.1:
-				time.sleep(0.005)
-				return elapsed
-			if elapsed < 1:
-				time.sleep(0.02)
-				return elapsed
-			if elapsed < 5:
-				time.sleep(0.05)
-				return elapsed
-			if elapsed < 10:
-				time.sleep(0.1)
-				return elapsed
-			if elapsed < 50:
-				time.sleep(0.5)
-				return elapsed
-			time.sleep(1)
-		elif self._opc_wait_mode == WaitForOpcMode.stb_poll_slow:
-			if elapsed < 0.01:
-				time.sleep(0.001)
-				return elapsed
-			if elapsed < 1:
-				time.sleep(0.02)
-				return elapsed
-			if elapsed < 5:
-				time.sleep(0.1)
-				return elapsed
-			if elapsed < 10:
-				time.sleep(0.2)
-				return elapsed
-			if elapsed < 20:
-				time.sleep(0.5)
-				return elapsed
-			time.sleep(1)
-		elif self._opc_wait_mode == WaitForOpcMode.stb_poll_superslow:
-			if elapsed < 1:
-				time.sleep(0.1)
-				return elapsed
-			if elapsed < 10:
-				time.sleep(0.5)
-				return elapsed
-			if elapsed < 20:
-				time.sleep(1)
-				return elapsed
-			time.sleep(2)
-
-		return elapsed
-
-	def query_syst_error(self) -> str or None:
-		"""Returns one response to the SYSTEM:ERROR? query."""
-		error = self.query_str("SYST:ERR?")
-		if error.startswith('0,'):
-			return None
-		return error.strip()
-
-	def query_all_syst_errors(self) -> list or None:
-		"""Returns all errors in the instrument's error queue."""
-		errors = []
-		while True:
-			entry = self.query_syst_error()
-			if entry is None:
-				break
-			errors.append(entry)
-			if len(errors) > 50:
-				# Safety stop
-				errors.append('query_all_syst_errors - max limit 50 of SYST:ERR? sent.')
-				break
-
-		if len(errors) == 0:
-			return None
-		else:
-			return errors
-
-	def _query_stb(self) -> StatusByte:
-		"""Sends *STB? query and reads the result."""
-		return StatusByte(int(self._query_str_no_events('*STB?')))
-
-	def _read_stb(self) -> StatusByte:
-		"""Calls viReadStb and returns the result."""
-		return StatusByte(self._session.read_stb())
-
-	def clear_before_read(self) -> None:
-		"""Clears IO buffers and the ESR register before reading/writing responses synchronized with *OPC."""
-
-		# For NRP-Z sessions, skip this completely
-		if self.is_rsnrp_session():
-			return
-
-		if not self.vxi_capable:
-			# Non-Vxi session must use *CLS in any case
-			self.write("*CLS")
-			correct = False
-			opc = self._query_str_no_events('*OPC?')
-			repeat = 0
-			while not correct:
-				if len(opc) <= 2:
-					opc = opc.strip()
-					correct = opc == '0' or opc == '1'
-				if not correct:
-					# Read again with a small VISA timeout
-					opc = self._read_str_timed(5, True)
-				repeat += 1
-				if repeat > 10:
-					break
-
-		stb = self._query_stb()
-		condition = StatusByte.error_queue_not_empty | StatusByte.message_available | StatusByte.event_status_byte
-		if not stb & condition:
-			return
-		repeat = 0
-		# Loop more times to clear the status subsystem
-		while stb & condition:
-			if stb & StatusByte.error_queue_not_empty:
-				self.write("*CLS")
-				_ = self.query_all_syst_errors()
-			if stb & StatusByte.message_available:
-				# Clear output buffer
-				self._flush_junk_data()
-			if stb & StatusByte.event_status_byte:
-				# OPC or error bits in the ESR
-				self.write("*CLS")
-				self.query_and_clear_esr()
-			# Check if the status byte value changed
-			previous_stb = stb
-			stb = self._query_stb()
-			if stb == previous_stb:
-				repeat += 1
-				if repeat > 10:
-					raise Exception(f"Cannot clear the instrument's status subsystem. Status Byte: '{stb}'")
-
-	def _flush_junk_data(self) -> None:
-		"""Reads junk bytes to clear the instrument's output buffer."""
-		if self.read_delay > 0:
-			time.sleep(self.read_delay / 1000)
-		self._read_unknown_len(StreamWriter.as_bin_var(), False)
-
-	def clear(self) -> None:
-		"""Perform VISA viClear conditionally based on the instrument settings."""
-		perform_all = ViClearMode.execute_on_all in self._viclear_exe_mode
-		perform = False
-		if perform_all:
-			perform = True
-		else:
-			# Perform on all is blocked, use the SessionKind to decide
-			if self._interface_type == SessionKind.gpib:
-				perform = ViClearMode.execute_on_gpib in self._viclear_exe_mode
-
-			elif self._interface_type == SessionKind.serial:
-				perform = ViClearMode.execute_on_serial in self._viclear_exe_mode
-
-			elif self._interface_type == SessionKind.socket:
-				perform = ViClearMode.execute_on_socket in self._viclear_exe_mode
-
-			elif self._interface_type == SessionKind.usb:
-				perform = ViClearMode.execute_on_usb in self._viclear_exe_mode
-
-			elif self._interface_type == SessionKind.vxi11:
-				perform = ViClearMode.execute_on_tcpvxi in self._viclear_exe_mode
-
-		if not perform:
-			return
-
-		if ViClearMode.ignore_error in self._viclear_exe_mode:
-			# noinspection PyBroadException
-			try:
-				self._session.clear()
-			except Exception:
-				pass
-		else:
-			self._session.clear()
-
-	def _write_and_wait_for_opc(self, command: str, is_query: bool, timeout: int) -> StatusByte:
-		"""Internal method to synchronise a command with OPC timeout.
-		Timeout value 0 means the OPC timeout is used."""
-		timeout = self._resolve_opc_timeout(timeout)
-
-		if command.endswith(self._term_char):
-			command = command.rstrip(self._term_char)
-		if is_query:
-			InstrumentErrors.assert_query_has_qmark(command, "Query with OPC")
-		else:
-			InstrumentErrors.assert_cmd_has_no_qmark(command, "Write with OPC")
-
-		if self._opc_wait_mode == WaitForOpcMode.opc_query:
-			if is_query:
-				raise Exception("Sending a query with OpcQuery synchronization is not possible")
-			stb = self._write_and_query_opc(command, timeout)
-		else:
-			# STB polling
-			end_stb_mask = StatusByte.error_queue_not_empty | StatusByte.event_status_byte
-			if is_query:
-				end_stb_mask |= StatusByte.message_available
-			if self.vxi_capable:
-				stb = self._write_and_poll_stb_vxi(command, is_query, timeout, end_stb_mask)
-			else:
-				stb = self._write_and_poll_stb_non_vxi(command, timeout, end_stb_mask)
-
-		return stb
-
-	def _write_and_query_opc(self, cmd: str, timeout: int) -> StatusByte:
-		"""Internal method to write a command followed by query_opc().
-		Used for opc-synchronization if the mode is set to WaitForOpcMode.opc_query or the session is not-vxi.
-		Timeout value 0 means the OPC timeout is used."""
-		old_tout = self.visa_timeout
-
-		# Change VISA Timeout if necessary
-		if old_tout != timeout:
-			self.visa_timeout = timeout
-		try:
-			# try-catch to set the VISA timeout back
-			self.write(cmd)
-			self.query_opc()
-		finally:
-			if old_tout != timeout:
-				self.visa_timeout = old_tout
-		return self._query_stb()
-
-	def write(self, cmd: str) -> None:
-		"""Writes command to the instrument."""
-		if self.write_delay > 0:
-			time.sleep(self.write_delay / 1000)
-		add_tc = False
-		if self._assure_write_with_tc and not cmd.endswith(self._term_char):
-			add_tc = True
-		if add_tc:
-			self._session.write(cmd + self._term_char)
-		else:
-			self._session.write(cmd)
-
-	def _read_unknown_len(self, stream: StreamWriter, allow_chunk_events: bool, prepend_data: AnyStr = None) -> None:
-		"""Reads data of unknown length to the provided WriteStream.
-		The read is performed in an incremental chunk steps to optimize memory use (for NRP-Z session it is set to fixed self._data_chunk_size):
-			- The first read is performed with the fixed size of 1024 bytes
-			- The 2nd one reads 64 kBytes
-			- The 3rd one reads 128 kBytes
-			- The 4th one reads 256 kBytes and so on, with the max cap of self._data_chunk_size
-		:param stream: [StreamWriter] target for the read data
-		:param allow_chunk_events: [bool] if True, the method can send the chunk_events. If False, sending events is blocked.
-		:param prepend_data: Optional[bytes or string] You can prepend this data to the beginning. It will be considered part of the first chunk read
-		:return: read data [bytes or string], depending on the parameter binary."""
-		with self._session.ignore_warning(pyvisa.constants.StatusCode.success_max_count_read):
-			if prepend_data and isinstance(prepend_data, str):
-				prepend_data = prepend_data.encode('utf-8')
-			chunk_ix = 0
-			eot = False
-			while not eot:
-				if self.is_rsnrp_session():
-					chunk_size = self._data_chunk_size
-				else:
-					if chunk_ix == 0:
-						# First read, set 1024 bytes read size
-						chunk_size = 1024
-					elif chunk_ix == 1:
-						chunk_size = 65536
-					else:
-						chunk_size *= 2
-				if chunk_size > self._data_chunk_size:
-					chunk_size = self._data_chunk_size
-				chunk, self.last_status = self._session.visalib.read(self._session.session, chunk_size)
-				if chunk_ix == 0 and prepend_data:
-					chunk = prepend_data + chunk
-				eot = not self._last_status_more_data_available()
-				if not stream.binary:
-					chunk = chunk.decode('utf-8')
-					if eot:
-						chunk = chunk.rstrip(self._term_char)
-				stream.write(chunk)
-				if self.on_read_chunk_handler and allow_chunk_events:
-					total_size = len(stream) if eot is True else None
-					event_args = EventArgsChunk(stream.binary, chunk_ix, len(chunk), total_size, len(stream), eot, None, chunk if self.io_events_include_data else None)
-					self.on_read_chunk_handler(event_args)
-				chunk_ix += 1
-
-	def _last_status_more_data_available(self):
-		"""Returns True, if the last status signalled that more data is available"""
-		return self.last_status == pyvisa.constants.StatusCode.success_max_count_read
-
-	def _read_str_no_events(self) -> str:
-		"""Reads response from the instrument. The response is then trimmed for trailing LF. \n
-		Sending of any read events is blocked."""
-		if self.read_delay > 0:
-			time.sleep(self.read_delay / 1000)
-		stream = StreamWriter.as_string_var()
-		self._read_unknown_len(stream, False)
-		return stream.content
-
-	def _query_str_no_events(self, query: str) -> str:
-		"""Queries the instrument and reads the response as string.
-		The length of the string is not limited. The response is then trimmed for trailing LF.
-		Sending of any read events is blocked. Use this method for all the service VisaSession queries."""
-		response = ''
-		self.write(query)
-		try:
-			response = self._read_str_no_events()
-		except pyvisa.VisaIOError:
-			self._narrow_down_io_tout_error("Querying '{}' - ".format(query.rstrip(self._term_char)))
-		return response
-
-	def _read_str_timed(self, timeout: int, suppress_read_tout: bool = False) -> str:
-		"""Reads response from the instrument with a VISA timeout temporarily set for the read.
-		The VISA timeout is set back to the previous value before the method finishes even if an exception occurs.
-		Sending of any read events is blocked."""
-		old_visa_tout = self.visa_timeout
-		if suppress_read_tout:
-			try:
-				if timeout != old_visa_tout:
-					self.visa_timeout = timeout
-				data = self._read_str_no_events()
-				return data
-			except TimeoutError:
-				pass
-			finally:
-				self.visa_timeout = old_visa_tout
-		else:
-			try:
-				if timeout != old_visa_tout:
-					self.visa_timeout = timeout
-				data = self._read_str_no_events()
-				return data
-			finally:
-				self.visa_timeout = old_visa_tout
-
-	def _read_str(self) -> str:
-		"""Reads response from the instrument. The response is then trimmed for trailing LF."""
-		if self.read_delay > 0:
-			time.sleep(self.read_delay / 1000)
-		stream = StreamWriter.as_string_var()
-		self._read_unknown_len(stream, True)
-		return stream.content
-
-	def query_str(self, query: str) -> str:
-		"""Queries the instrument and reads the response as string.
-		The length of the string is not limited. The response is then trimmed for trailing LF."""
-		response = ''
-		self.write(query)
-		try:
-			response = self._read_str()
-		except pyvisa.VisaIOError:
-			self._narrow_down_io_tout_error("Querying '{}' - ".format(query.rstrip(self._term_char)))
-		return response
-
-	def query_str_no_tout_err(self, query: str, tout: int) -> str:
-		"""Same as query_str, but you can set the timeout just for this one call.
-		If the timeout exception occurs, it is suppressed and the method returns Null"""
-		response = None
-		old_tout = self.visa_timeout
-		try:
-			self.visa_timeout = tout
-			response = self.query_str(query)
-		except (pyvisa.VisaIOError, InstrumentErrors.StatusException):
-			pass
-		finally:
-			self.visa_timeout = old_tout
-		return response
-
-	def write_with_opc(self, command: str, timeout: int = None) -> None:
-		"""Sends command with OPC-sync.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		self._write_and_wait_for_opc(command, False, timeout)
-
-	def query_str_with_opc(self, query: str, timeout: int = None) -> str:
-		"""Query string with OPC synchronization.
-		The response is trimmed for any trailing LF.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		timeout = self._resolve_opc_timeout(timeout)
-		if self.vxi_capable and self._opc_wait_mode is not WaitForOpcMode.opc_query:
-			# For Vxi session, use the STB poll or SRQ wait and then read the response
-			stb = self._write_and_wait_for_opc(query, True, timeout)
-			self._check_msg_available_after_opc_wait(stb, query, timeout, "Query String With OPC")
-			response = self._read_str()
-		else:
-			# For non-Vxi sessions, use the longer VISA Timeout without the *OPC?
-			# Same is valid for WaitForOpcMode.OpcQuery
-			InstrumentErrors.assert_query_has_qmark(query, "Query with VISA timeout")
-			self.write(query)
-			old_tout = self.visa_timeout
-			# Change VISA Timeout if necessary
-			if old_tout != timeout:
-				self.visa_timeout = timeout
-			try:
-				# try-catch to set the VISA timeout back
-				response = self._read_str()
-				if self._opc_wait_mode is WaitForOpcMode.opc_query:
-					self.query_opc()
-			finally:
-				if old_tout != timeout:
-					self.visa_timeout = old_tout
-
-		return response
-
-	def query_opc(self) -> bool:
-		"""Sends *OPC? query and reads the result."""
-		if self.disable_opc_query:
-			return True
-		response = self._query_str_no_events("*OPC?")
-		return Conv.str_to_bool(response)
-
-	def query_and_clear_esr(self) -> int:
-		"""Sends *ESR? query and reads the result."""
-		response = self._query_str_no_events("*ESR?")
-		return int(response)
-
-	def _check_msg_available_after_opc_wait(self, stb: StatusByte, query: str, timeout: int, context: str) -> None:
-		"""Used internally after _StbPolling() to check if the message is available.
-		Throws an exception in case of MAV not available."""
-		if not self.vxi_capable:
-			return
-		if stb & StatusByte.message_available:
-			return
-		# Message not available
-		context = context + " SCPI query '{}'".format(query.rstrip(self._term_char))
-		if stb & StatusByte.error_queue_not_empty:
-			# Instrument reports an error
-			InstrumentErrors.assert_no_instrument_status_errors(self._resource_name, self.query_all_syst_errors(), context)
-		else:
-			# Sometimes even if the StatusByte.MessageAvailable is false, the message is available.
-			# Try to read the STB again
-			stb = self._read_stb()
-			if not stb & StatusByte.event_status_byte:
-				# Instrument did not respond within the defined time
-				InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout, "{} No response from the instrument.".format(context))
-
-	def error_in_error_queue(self) -> bool:
-		"""Returns true, if error queue contains at least one error."""
-		stb = self._query_stb()
-		return stb & StatusByte.error_queue_not_empty
-
-	def reset_ese_sre(self) -> None:
-		"""Resets the status of ESE and SRE registers to default values."""
-		self._set_regs_ese_sre(self._opc_wait_mode)
-
-	def write_bin_block(self, cmd: str, data_stream: StreamReader) -> None:
-		"""Writes all the payload as binary data block to the instrument.
-		The binary data header is added at the beginning of the transmission automatically.
-		:param cmd: [str] SCPI command with which to send the data
-		:param data_stream: [StreamReader] data provider for the payload"""
-		data_size = len(data_stream)
-		len_str = f'{data_size}'
-		cmd = cmd.rstrip(self._term_char)
-		if '#' in cmd:
-			raise Exception(
-				f"Command '{cmd}' must be provided without the binary data header. "
-				f"The method 'write_bin_block' composes and prepends the binary data header automatically.")
-		if data_size <= self._std_bin_block_header_max_len:
-			# Standard bin data header for sizes below 1E9 bytes, e.g.: '#512345'
-			cmd_plus_header = f'{cmd}#{len(len_str)}{len_str}'.encode('utf-8')
-		else:
-			# Big sizes bin data header: e.g.: '#(3000000000)'
-			cmd_plus_header = f'{cmd}#({len_str})'.encode('utf-8')
-
-		if data_size <= self._data_chunk_size:
-			# Write all in one step
-			full_chunk = data_stream.read_as_binary()
-			write_buf = cmd_plus_header + full_chunk
-			if self._add_term_char_to_write_bin_block:
-				write_buf += self._term_char_bin
-			self._session.write_raw(write_buf)
-			# Event sending
-			if self.on_write_chunk_handler:
-				event_args = EventArgsChunk(True, 0, data_size, data_size, data_size, True, 1, full_chunk if self.io_events_include_data else None)
-				self.on_write_chunk_handler(event_args)
-		else:
-			# Write in chunks
-			try:
-				# Use finally to set the session send_end back to True
-				self._session.send_end = False
-				total_chunks = calculate_chunks_count(data_size, self._data_chunk_size)
-				chunk_ix = 0
-				if self.write_delay > 0:
-					time.sleep(self.write_delay / 1000)
-				# Write bin header
-				self._session.write_raw(cmd_plus_header)
-				# Write chunks
-				while True:
-					if len(data_stream) > self._data_chunk_size:
-						#  Not the last segment
-						chunk = data_stream.read_as_binary(self._data_chunk_size)
-						self._session.write_raw(chunk)
-						# Event sending
-						if self.on_write_chunk_handler:
-							event_args = EventArgsChunk(
-								True, chunk_ix, self._data_chunk_size, data_size, data_size - len(data_stream), False, total_chunks, chunk if self.io_events_include_data else None)
-							self.on_write_chunk_handler(event_args)
-					else:
-						# Last segment, indicate end of message again
-						chunk = data_stream.read_as_binary()
-						if self._add_term_char_to_write_bin_block:
-							# Append LF
-							self._session.write_raw(chunk)
-							self._session.send_end = True
-							self._session.write_raw(self._term_char_bin)
-						else:
-							self._session.send_end = True
-							self._session.write_raw(chunk)
-
-						# Event sending
-						if self.on_write_chunk_handler:
-							event_args = EventArgsChunk(True, chunk_ix, len(chunk), data_size, data_size, True, total_chunks, chunk if self.io_events_include_data else None)
-							self.on_write_chunk_handler(event_args)
-						break
-					chunk_ix += 1
-			finally:
-				self._session.send_end = True
-
-	def _parse_bin_data_header(self, exc_if_not_bin: bool) -> Tuple[ReadDataType, str, int]:
-		"""Parses the binary data block and returns the expected length of the following data block. \n
-		:param exc_if_not_bin: [bool] if True, the method throws exception in case the data is not binary.
-		:return: read_data_type: [ReadDataType], parsed_header: [string], bin_data_len: [integer]"""
-		length = -1
-		if self.read_delay > 0:
-			time.sleep(self.read_delay / 1000)
-
-		char: AnyStr = self._session.read_bytes(1, break_on_termchar=True)
-		if char == b'#':
-			# binary transfer
-			char = self._session.read_bytes(1, break_on_termchar=True)
-			if char == b'0':
-				data_type = ReadDataType.bin_unknown_len
-				return data_type, '#0', -1
-			if char == b'(':
-				# format for big lengths i.e. > 1E9 bytes: '#(1234567890123)...'
-				data_type = ReadDataType.bin_known_len
-				len_str = (self.read_up_to_char(b')', 100)[:-1]).decode("utf-8")
-				whole_hdr = '#(' + len_str + ')'
-				length = int(len_str)
-				return data_type, whole_hdr, length
-
-			# classic format for < 1E9 bytes: '#9123456789...'
-			data_type = ReadDataType.bin_known_len
-			len_of_len = int(char)
-			len_str = self._session.read_bytes(len_of_len).decode("utf-8")
-			length = int(len_str)
-			whole_hdr = '#' + char.decode("utf-8") + len_str
-			return data_type, whole_hdr, length
-
-		data_type = ReadDataType.ascii
-		if char == self._term_char_bin:
-			data_type = ReadDataType.null
-		if self.vxi_capable:
-			# For Vxi session, to be sure, check whether there are more chars in the read buffer
-			stb = self._read_stb()
-			if stb & StatusByte.message_available:
-				data_type = ReadDataType.ascii
-		whole_hdr = char.decode("utf-8")
-		if exc_if_not_bin:
-			if data_type == ReadDataType.null:
-				InstrumentErrors.throw_bin_block_unexp_resp_exception(self._resource_name, self._term_char)
-			# Read 20 more characters to compose a better exception message
-			whole_hdr += self.read_up_to_char(self._term_char_bin, 20).decode("utf-8")
-			if self.last_status == pyvisa.constants.StatusCode.success_max_count_read:
-				self._flush_junk_data()
-			InstrumentErrors.throw_bin_block_unexp_resp_exception(self._resource_name, whole_hdr)
-		return data_type, whole_hdr, length
-
-	def read_bin_block(self, stream: StreamWriter, exc_if_not_bin: bool) -> None:
-		"""Reads binary data block to the provided stream. \n
-		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
-		:param exc_if_not_bin: if True, the method throws exception if the received data is not binary"""
-		data_type, header, length = self._parse_bin_data_header(exc_if_not_bin)
-		if data_type == ReadDataType.ascii:
-			stream.switch_to_string_data()
-			self._read_unknown_len(stream, True, header)
-		elif data_type == ReadDataType.null:
-			# No data, consider it ASCII, Return empty string, and False (signaling ASCII transfer)
-			stream.switch_to_string_data()
-		elif data_type == ReadDataType.bin_unknown_len:
-			if not self.vxi_capable:
-				raise Exception(f'Non-Vxi11 sessions can not read binary data block of unknown length.')
-			self._read_unknown_len(stream, True)
-		elif length == 0:
-			self._flush_junk_data()
-		else:
-			self._read_bin_block_known_len(stream, length)
-
-	def _read_bin_block_known_len(self, stream: StreamWriter, length: int) -> None:
-		"""Reads binary data of defined length. All remaining data above the length are disposed of. \n
-		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
-		:param length: [int] expected length of the data"""
-		# Use try-catch to switch the termination character back ON in case of an exception (for non-Vxi sessions)
-		try:
-			# Binary transmission, for non-Vxi session, set the termination character to OFF
-			if not self.vxi_capable:
-				self._session.read_termination = False
-			# Binary data of known length
-			left_to_read = length
-			self.last_status = pyvisa.constants.StatusCode.success
-			with self._session.ignore_warning(pyvisa.constants.StatusCode.success_max_count_read):
-				chunk_ix = 0
-				total_chunks = calculate_chunks_count(length, self._data_chunk_size)
-				while len(stream) < length:
-					chunk_size = min(self._data_chunk_size, left_to_read)
-					chunk, self.last_status = self._session.visalib.read(self._session.session, chunk_size)
-					left_to_read -= len(chunk)
-					stream.write(chunk)
-					if self.on_read_chunk_handler:
-						event_args = EventArgsChunk(True, chunk_ix, chunk_size, length, len(stream), left_to_read == 0, total_chunks, chunk if self.io_events_include_data else None)
-						self.on_read_chunk_handler(event_args)
-					chunk_ix += 1
-			if self._last_status_more_data_available():
-				if not self.vxi_capable:
-					self._session.read_termination = self._term_char
-				self._flush_junk_data()
-		finally:
-			# Make sure that in any case the self._session.read_termination is ON again for non-Vxi sessions
-			if not self.vxi_capable:
-				self._session.read_termination = self._term_char
-
-	def query_bin_block(self, query: str, stream: StreamWriter, exc_if_not_bin: bool = True) -> None:
-		"""Query binary data block and returns it as byte data. \n
-		:param query: [str] query to send to the instrument
-		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
-		:param exc_if_not_bin: [Boolean] if True, the method throws exception if the received data is not binary"""
-		self.write(query)
-		self.read_bin_block(stream, exc_if_not_bin)
-		return
-
-	def query_bin_block_with_opc(self, query: str, stream: StreamWriter, exc_if_not_bin: bool = True, timeout: int = None) -> None:
-		"""Query binary data block with OPC and returns it as byte data.
-		:param query: [str] query to send to the instrument
-		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
-		:param exc_if_not_bin: [Boolean] if True, the method throws exception if the received data is not binary
-		:param timeout: Optional[Integer] timeout for the operation. If you skip it, the method uses the current opc timeout."""
-		timeout = self._resolve_opc_timeout(timeout)
-		if self.vxi_capable and self._opc_wait_mode != WaitForOpcMode.opc_query:
-			# For Vxi session, use the STB poll and read the response
-			stb = self._write_and_wait_for_opc(query, True, timeout)
-			self._check_msg_available_after_opc_wait(stb, query, timeout, 'query_bin_block_with_opc')
-			self.read_bin_block(stream, exc_if_not_bin)
-		else:
-			# For non-Vxi session, use the longer VISA Timeout without the *OPC
-			InstrumentErrors.assert_query_has_qmark(query, "query_bin_block_with_opc")
-			self.write(query)
-			old_visa_timeout = self.visa_timeout
-			# Change VISA Timeout if necessary
-			if old_visa_timeout != timeout:
-				self.visa_timeout = timeout
-			try:
-				# try-catch to set the VISA timeout back
-				self.read_bin_block(stream, exc_if_not_bin)
-				if self._opc_wait_mode == WaitForOpcMode.opc_query:
-					self.query_opc()
-			finally:
-				# Change VISA Timeout back if necessary
-				if old_visa_timeout != timeout:
-					self.visa_timeout = old_visa_timeout
-
-	def read_up_to_char(self, stop_chars: bytes, max_cnt: int) -> bytes:
-		"""Reads until one of the stop_chars is read or the max_cnt is reached, or EOT is detected.
-		Returns the read data including the stop character."""
-		response = b''
-		for i in range(max_cnt):
-			char, self.last_status = self._session.visalib.read(self._session.session, 1)
-			response += char
-			if char in stop_chars:
-				break
-			if self.last_status != pyvisa.constants.StatusCode.success_max_count_read:
-				break
-		return response
-
-	def get_session_handle(self) -> object:
-		"""Returns the underlying pyvisa session."""
-		return self._session
-
-	def close(self) -> None:
-		"""Closes the Visa session.
-		If the object was created with the direct session input, the session is not closed."""
-		if not self.reusing_session:
-			self._session.close()
-
-	# Events
-
-
-class EventArgsChunk:
-	"""Event arguments for chunk io event."""
-
-	def __init__(
-			self,
-			binary: bool,
-			chunk_ix: int,
-			chunk_size: int,
-			total_size: int,
-			transferred_size: int,
-			end_of_transfer: bool,
-			total_chunks: int or None,
-			data: AnyStr = None):
-
-		self.binary = binary
-		self.chunk_ix = chunk_ix
-		self.total_chunks = total_chunks
-		self.chunk_size = chunk_size
-		self.transferred_size = transferred_size
-		self.total_size = total_size
-		self.end_of_transfer = end_of_transfer
-		self.data = data
-
-	def __str__(self):
-		if self.binary:
-			type_info = 'binary'
-		else:
-			type_info = 'ascii'
-		if not self.total_chunks:
-			chunk_info = f' chunk nr. {self.chunk_ix + 1}'
-		elif self.total_chunks > 1:
-			chunk_info = f' chunk nr. {self.chunk_ix + 1}/{self.total_chunks}'
-		else:
-			chunk_info = ' chunk nr. 1/1'
-		eot = ' (EOT)' if self.end_of_transfer else ''
-		result = \
-			f'EventArgsChunk {type_info},{chunk_info}, {size_to_kb_mb_string(self.chunk_size, True)}, ' \
-			f'sum {size_to_kb_mb_string(self.transferred_size, True)} / {size_to_kb_mb_string(self.total_size, True) if self.total_size else "<N.A.>"}{eot}.'
-		return result
+import time
+from enum import Enum, Flag
+from typing import Tuple, Callable, AnyStr
+import os.path
+import re
+import threading
+
+# noinspection PyPackageRequirements
+import pyvisa
+
+from .VisaPluginSocketIo import ResourceManager, SocketIo
+from . import InstrumentSettings, InstrumentErrors, Conversions as Conv
+from .InstrumentSettings import WaitForOpcMode, InstrViClearMode as ViClearMode
+from .StreamReader import StreamReader
+from .StreamWriter import StreamWriter
+from .Utilities import size_to_kb_mb_string, calculate_chunks_count
+import platform
+import struct
+
+
+class SessionKind(Enum):
+	"""Visa instrument session type."""
+	unsupported = 0
+	gpib = 1
+	serial = 2
+	vxi11 = 3
+	socket = 5
+	usb = 6
+	rs_nrp = 7
+
+
+class ReadDataType(Enum):
+	"""Data type returned by the instrument."""
+	unknown = 0
+	ascii = 1
+	null = 2
+	bin_known_len = 3
+	bin_unknown_len = 4
+
+
+class StatusByte(Flag):
+	"""Status Byte flags."""
+	NONE = 0x00
+	error_queue_not_empty = 0x04
+	questionable_status_reg = 0x08
+	message_available = 0x10
+	event_status_byte = 0x20
+	request_service = 0x40
+	operation_status_reg = 0x80
+
+
+class EventStatusRegister(Flag):
+	"""Event Status Register flags."""
+	null = 0x00
+	operation_complete = 0x01
+
+
+# noinspection PyUnresolvedReferences
+class VisaSession(object):
+	"""Extended VISA class."""
+
+	def __init__(self, resource_name: str, settings: InstrumentSettings, direct_session=None):
+		self.reusing_session = direct_session is not None
+		# noinspection PyTypeChecker
+		self._data_chunk_size: int = None
+		self._std_bin_block_header_max_len: int = 999999999
+		self._lock = None
+		self.disable_opc_query: bool = settings.disable_opc_query
+		self.last_status = None
+		self.visa_library_name = None
+
+		# Implemented for interface compatibility with VisaSessionSim
+		self.cached_to_stream = False
+
+		# Event handlers
+		# noinspection PyTypeChecker
+		self.on_read_chunk_handler: Callable = None
+		"""If assigned a handler, the VisaSession sends it event on each read chunk transfer."""
+		# noinspection PyTypeChecker
+		self.on_write_chunk_handler: Callable = None
+		"""If assigned a handler, the VisaSession sends it event on each write chunk transfer."""
+		self.io_events_include_data: bool = False
+		"""If true, the VisaSession events sent to on_read_chunk_handler and on_write_chunk_handler contain transferred data."""
+
+		if self.reusing_session:
+			# Reuse the session
+			assert isinstance(direct_session, pyvisa.Resource) or isinstance(direct_session, SocketIo), f"Direct_session must be a VISA resource object. Actual type: '{type(direct_session)}', value: '{direct_session}'"
+			self._session = direct_session
+			self._resource_name = self._session.resource_name
+		else:
+			# Create new session
+			# Check resource_name for the trailing (SelectVisa=..)
+			pure_resource_name, visa_select = self._get_pure_resource_name(resource_name)
+			if settings.visa_select is not None:
+				visa_select = settings.visa_select
+			self._rm = VisaSession.get_resource_manager(visa_select)
+			self.manufacturer = self._get_visa_manufacturer()
+
+			# Resource manager opening
+			try:
+				self._session = self._rm.open_resource(pure_resource_name)
+			except pyvisa.VisaIOError as e:
+				if e.error_code != pyvisa.constants.StatusCode.error_resource_not_found:
+					raise e
+				message = e.description
+				message += f"\nLibrary: {self._rm.visalib}\nManufacturer: {self.manufacturer}\nResource Name: '{resource_name}'"
+				raise InstrumentErrors.ResourceError(resource_name, message)
+			self._resource_name = resource_name
+
+		# Decide, whether to create a new thread lock or the existing one from the session
+		if hasattr(self._session, 'session_thread_rlock'):
+			rlock = self._session.session_thread_rlock
+			if isinstance(rlock, type(threading.RLock())):
+				self.assign_lock(rlock)
+		if self.get_lock() is None:
+			# The existing session did not have a thread lock, assign a new one
+			self.assign_lock(threading.RLock())
+
+		self._interface_type = SessionKind.unsupported
+		if self._session.interface_type == pyvisa.constants.InterfaceType.gpib or self._session.interface_type == pyvisa.constants.InterfaceType.gpib:
+			self._interface_type = SessionKind.gpib
+
+		elif self._session.interface_type == pyvisa.constants.InterfaceType.rsnrp:
+			self._interface_type = SessionKind.rs_nrp
+
+		elif self._session.interface_type == pyvisa.constants.InterfaceType.asrl:
+			self._interface_type = SessionKind.serial
+
+		elif self._session.interface_type == pyvisa.constants.InterfaceType.usb:
+			# Check whether it is not the NRP-Z
+			intf_type = self._session.get_visa_attribute(pyvisa.constants.VI_ATTR_INTF_TYPE)
+			if intf_type == pyvisa.constants.InterfaceType.rsnrp:
+				self._interface_type = SessionKind.rs_nrp
+
+		elif self._session.interface_type == pyvisa.constants.InterfaceType.tcpip:
+			self._interface_type = SessionKind.vxi11
+			if self._session.resource_class == 'SOCKET':
+				self._interface_type = SessionKind.socket
+
+		# Specifics for different interfaces
+		self._assure_write_with_tc = settings.assure_write_with_tc
+		self._term_char = settings.term_char
+		self._term_char_bin = self._term_char.encode('utf-8')
+		self._session.write_termination = ''
+		self.vxi_capable = True
+
+		if self._interface_type == SessionKind.serial:
+			self._session.read_termination = self._term_char
+			self.vxi_capable = False
+			self._assure_write_with_tc = True
+		elif self._interface_type == SessionKind.socket:
+			self._session.read_termination = self._term_char
+			self.vxi_capable = False
+			self._assure_write_with_tc = True
+		else:
+			self._session.read_termination = ''
+
+		# NRP-Z specific settings
+		if self.is_rsnrp_session():
+			self.disable_opc_query = True
+			# NRP-Z does not support chunk reading, therefore the segment must be in one piece
+			settings.io_segment_size = 1000000
+			self.vxi_capable = False
+
+		self.write_delay = settings.write_delay
+		self.read_delay = settings.read_delay
+		self._viclear_exe_mode = settings.viclear_exe_mode
+		self._opc_wait_mode = settings.opc_wait_mode
+
+		# Parameters that need to be coerced based on Vxi-capability
+		if self.vxi_capable:
+			self._add_term_char_to_write_bin_block = settings.add_term_char_to_write_bin_block
+		else:
+			self._add_term_char_to_write_bin_block = True
+
+		# Changeable settings
+		self.opc_timeout = 10000 if settings.opc_timeout == 0 else settings.opc_timeout
+		self.visa_timeout = settings.visa_timeout
+		self._session.chunk_size = settings.io_segment_size
+		self._data_chunk_size = settings.io_segment_size
+
+		# Must call the VISA viClear() before the any communication with the instrument
+		self.clear()
+
+		# Further steps are for NRP-Z session not valid
+		if self.is_rsnrp_session():
+			return
+
+		# Clear instrument status
+		self.write('*CLS')
+		if self.vxi_capable:
+			stb = self._read_stb()
+			if stb & StatusByte.message_available:
+				self._flush_junk_data()
+
+		# Apply settings for ESE and SRE, plus coerce the _opcWaitMode if necessary
+		self._opc_wait_mode = self._set_regs_ese_sre(self._opc_wait_mode)
+
+	@staticmethod
+	def _get_pure_resource_name(resource_name: str):
+		"""Returns pure resource name stripped of the (SelectVisa) part and the visa_select string"""
+		m = re.search(r'(.+)\(SelectVisa=([^),]+)\)', resource_name)
+		if not m:
+			return resource_name, None
+		resource_name = m.group(1).strip()
+		visa_select = m.group(2).strip()
+		return resource_name, visa_select
+
+	@classmethod
+	def get_resource_manager(cls, visa_select: str) -> pyvisa.ResourceManager:
+		"""Returns resource manager for the desired VISA implementation"""
+		operating_system = platform.system().lower()
+		bittness = struct.calcsize('P') * 8
+		if visa_select is None or visa_select in ['@default', '@standard', 'default', 'standard', 'defaultvisa', 'standardvisa', '@defaultvisa', '@standardvisa']:
+			return pyvisa.ResourceManager()
+		if visa_select.lower() in ['@ni', 'ni', 'visa-ni', 'nivisa', 'ni-visa', 'nationalinstruments', 'nationalinstrumentsvisa']:
+			return pyvisa.ResourceManager('@ni')
+		if visa_select.lower() in ['@py', 'pyvisa', 'visa-py', 'pyvisa-py']:
+			return pyvisa.ResourceManager('@py')
+		if 'rohde&schwarz' in visa_select.lower() or 'rohdeschwarz' in visa_select.lower() or visa_select.lower() == 'rsvisa' or visa_select.lower() == 'rs' or visa_select.lower() == 'r&s':
+			if operating_system == 'windows':
+				if bittness == 32:
+					visa_select = r'c:\Windows\SysWOW64\RsVisa32.dll'
+				else:
+					visa_select = r'c:\Windows\system32\RsVisa32.dll'
+				return pyvisa.ResourceManager(visa_select)
+			elif operating_system == 'linux':
+				# The default install location may be different
+				# for debian/red hat/opensuse derived distributions
+				check_visa = [f'/usr/lib{bittness}/librsvisa.so', r'/usr/lib/librsvisa.so']
+				for check in check_visa:
+					if os.path.isfile(check):
+						return pyvisa.ResourceManager(check)
+
+		if visa_select.lower() in ['socketio', 'socket', 'none']:
+			return ResourceManager()
+		return pyvisa.ResourceManager(visa_select)
+
+	def _get_visa_manufacturer(self) -> str:
+		"""Returns manufacturer of the current VISA"""
+		if hasattr(self._rm, 'VisaManufacturerName'):
+			return self._rm.VisaManufacturerName
+		try:
+			return self._rm.visalib.get_attribute(self._rm.session, pyvisa.constants.VI_ATTR_RSRC_MANF_NAME)[0]
+		except TypeError:
+			return self._rm.visalib.__class__.__name__
+
+	def is_rsnrp_session(self) -> bool:
+		"""Returns True, if the current session is a NRP-Z session"""
+		return self._interface_type == SessionKind.rs_nrp
+
+	def assign_lock(self, lock: threading.RLock) -> None:
+		"""Assigns the provided thread lock by setting the pyvisa runtime session attribute 'session_thread_rlock'
+		This is done, because if the session is to be entered as an existing session to another RsInstrument object,
+		the lock must be shared as well. The lock is only used by the parent class Instrument."""
+		setattr(self._session, 'session_thread_rlock', lock)
+		self._lock = lock
+
+	def get_lock(self) -> threading.RLock:
+		"""Returns the current RLock object."""
+		return self._lock
+
+	@property
+	def visa_timeout(self) -> int:
+		"""See the visa_timeout.setter."""
+		return int(self._session.timeout)
+
+	@visa_timeout.setter
+	def visa_timeout(self, value: int) -> None:
+		"""Sets / Gets visa IO timeout in milliseconds."""
+		self._session.timeout = int(value)
+
+	@property
+	def data_chunk_size(self) -> int:
+		"""Returns max chunk size of one data block."""
+		return self._data_chunk_size
+
+	@data_chunk_size.setter
+	def data_chunk_size(self, chunk_size: int) -> None:
+		"""Sets the maximum size of one block transferred during write/read operations."""
+		self._data_chunk_size = int(chunk_size)
+		self._session.chunk_size = int(chunk_size)
+
+	def _resolve_opc_timeout(self, timeout: int) -> int:
+		"""Resolves entered timeout value - if the input value is less than 1, it is replaces with opc_timeout."""
+		if timeout is None or timeout < 1:
+			return self.opc_timeout
+		else:
+			return timeout
+
+	def _set_regs_ese_sre(self, mode: WaitForOpcMode) -> WaitForOpcMode:
+		"""Based on the WaitForOpcMode, it sets the ESE and SRE register masks.
+		Returns coerced WaitForOpcMode."""
+		# Set the SRE and ESE registers accordingly
+		# No SRE is supported
+		self._set_ese_mask(EventStatusRegister.operation_complete)
+		self._set_sre_mask(StatusByte.NONE)
+		return mode
+
+	def _set_ese_mask(self, mask: EventStatusRegister, reset: bool = True) -> None:
+		"""Sends *ESE command with mask parameter."""
+		if reset is False:
+			current_value = int(self._query_str_no_events('*ESE?'))
+			mask = current_value | mask.value
+		self.write("*ESE %d" % mask.value)
+
+	def _set_sre_mask(self, mask: StatusByte, reset: bool = True) -> None:
+		"""Sends *SRE command with StatusByte mask parameter."""
+		if reset is False:
+			current_value = int(self._query_str_no_events('*SRE?'))
+			mask = current_value | mask.value
+		# Also affect the _opc_wait_mode:
+		# If the mask has event_status_byte == false, and the _opc_wait_mode is service_request, set it to stb_poll
+		# If the mask has event_status_byte == true, do not change anything
+		self.write(f'*SRE {mask.value}')
+
+	def _write_and_poll_stb_vxi(self, command: str, is_query: bool, timeout: int, end_mask: StatusByte) -> StatusByte:
+		"""Reads Status Byte Register and ends if the ESB bit (5) is set to 1.
+		Also works with the SOCKET and SERIAL interface by sending *STB? query.
+		In that case however, command cannot be a query.
+		Returns the last read Status Byte value."""
+		timeout_secs = timeout / 1000
+		self.clear_before_read()
+		if command.endswith(self._term_char):
+			command = command.rstrip(self._term_char)
+		self.write(command + ';*OPC')
+		# Use catch to return the VISA Timeout back
+		start = time.time()
+		# STB polling loop
+		while True:
+			stb = self._read_stb()
+			elapsed = self._polling_delay(start)
+			if elapsed > timeout_secs:
+				self._narrow_down_opc_tout_error(command, is_query, timeout)
+			if end_mask & stb:
+				break
+		return stb
+
+	def _write_and_poll_stb_non_vxi(self, command: str, timeout: int, end_mask: StatusByte) -> StatusByte:
+		"""Queries Status Byte Register (*STB?) and ends if the ESB bit (5) is set to 1.
+			The command must not be a query. Also works with the SOCKET and SERIAL interface.
+			Returns the last read Status Byte value."""
+		timeout_secs = timeout / 1000
+		self.clear_before_read()
+		if command.endswith(self._term_char):
+			command = command.rstrip(self._term_char)
+		self.write(command + ';*OPC')
+		start = time.time()
+		# STB polling loop
+		while True:
+			stb = self._query_stb()
+			elapsed = self._polling_delay(start)
+			if elapsed > timeout_secs:
+				InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout)
+			if stb & end_mask:
+				break
+		return stb
+
+	def _narrow_down_opc_tout_error(self, command: str, is_query: bool, timeout: int) -> None:
+		"""Called by the _write_and_poll_stb_vxi when the timeout expires.
+		The method tries to closer identify the cause of the timeout."""
+		stb = self._read_stb()
+		timeout = self._resolve_opc_timeout(timeout)
+		if is_query:
+			if stb & StatusByte.error_queue_not_empty:
+				self.clear()
+				context = f"Sending query '{command.strip()}' with OPC Wait resulted in timeout. OPC Timeout is set to {timeout} ms. Additionally, "
+				InstrumentErrors.assert_no_instrument_status_errors(self._resource_name, self.query_all_syst_errors(), context)
+			InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout, f"Sending query '{command.strip()}'.")
+		else:
+			if stb & StatusByte.error_queue_not_empty:
+				self.clear()
+				context = f"Sending command '{command.strip()}' with OPC Wait resulted in timeout. OPC Timeout is set to {timeout} ms. Additionally, "
+				InstrumentErrors.assert_no_instrument_status_errors(self._resource_name, self.query_all_syst_errors(), context)
+			InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout, f"Sending command '{command.strip()}'.")
+
+	def _narrow_down_io_tout_error(self, context: str, visa_timeout: int = 0) -> None:
+		"""Called internally after IOTimeoutException can narrow down the error to more specific exception.
+		You can define the visa_timeout value for the error message. Otherwise the current visa_timeout is reported."""
+		if self.vxi_capable:
+			stb = self._read_stb()
+		else:
+			# Non-Vxi session
+			old_tout = self.visa_timeout
+			try:
+				self.visa_timeout = 500
+				stb = self._query_stb()
+			finally:
+				self.visa_timeout = old_tout
+		if visa_timeout <= 0:
+			visa_timeout = self.visa_timeout
+		context = context + f'VISA Timeout error occurred ({visa_timeout} milliseconds)'
+		if stb & StatusByte.error_queue_not_empty:
+			InstrumentErrors.assert_no_instrument_status_errors(self._resource_name, self.query_all_syst_errors(), context + ' and ...')
+		# In case the previous exception is not thrown
+		raise InstrumentErrors.TimeoutException(context)
+
+	def _polling_delay(self, start):
+		"""Generates progressive polling delay."""
+
+		elapsed = time.time() - start
+		if self._opc_wait_mode == WaitForOpcMode.stb_poll:
+			if elapsed < 0.01:
+				return elapsed
+			if elapsed < 0.1:
+				time.sleep(0.005)
+				return elapsed
+			if elapsed < 1:
+				time.sleep(0.02)
+				return elapsed
+			if elapsed < 5:
+				time.sleep(0.05)
+				return elapsed
+			if elapsed < 10:
+				time.sleep(0.1)
+				return elapsed
+			if elapsed < 50:
+				time.sleep(0.5)
+				return elapsed
+			time.sleep(1)
+		elif self._opc_wait_mode == WaitForOpcMode.stb_poll_slow:
+			if elapsed < 0.01:
+				time.sleep(0.001)
+				return elapsed
+			if elapsed < 1:
+				time.sleep(0.02)
+				return elapsed
+			if elapsed < 5:
+				time.sleep(0.1)
+				return elapsed
+			if elapsed < 10:
+				time.sleep(0.2)
+				return elapsed
+			if elapsed < 20:
+				time.sleep(0.5)
+				return elapsed
+			time.sleep(1)
+		elif self._opc_wait_mode == WaitForOpcMode.stb_poll_superslow:
+			if elapsed < 1:
+				time.sleep(0.1)
+				return elapsed
+			if elapsed < 10:
+				time.sleep(0.5)
+				return elapsed
+			if elapsed < 20:
+				time.sleep(1)
+				return elapsed
+			time.sleep(2)
+
+		return elapsed
+
+	def query_syst_error(self) -> str or None:
+		"""Returns one response to the SYSTEM:ERROR? query."""
+		error = self.query_str('SYST:ERR?')
+		if error.startswith('0,'):
+			return None
+		return error.strip()
+
+	def query_all_syst_errors(self) -> list or None:
+		"""Returns all errors in the instrument's error queue."""
+		errors = []
+		while True:
+			entry = self.query_syst_error()
+			if entry is None:
+				break
+			errors.append(entry)
+			if len(errors) > 50:
+				# Safety stop
+				errors.append('query_all_syst_errors - max limit 50 of SYST:ERR? sent.')
+				break
+
+		if len(errors) == 0:
+			return None
+		else:
+			return errors
+
+	def _query_stb(self) -> StatusByte:
+		"""Sends *STB? query and reads the result."""
+		return StatusByte(int(self._query_str_no_events('*STB?')))
+
+	def _read_stb(self) -> StatusByte:
+		"""Calls viReadStb and returns the result."""
+		return StatusByte(self._session.read_stb())
+
+	def clear_before_read(self) -> None:
+		"""Clears IO buffers and the ESR register before reading/writing responses synchronized with *OPC."""
+
+		# For NRP-Z sessions, skip this completely
+		if self.is_rsnrp_session():
+			return
+
+		if not self.vxi_capable:
+			# Non-Vxi session must use *CLS in any case
+			self.write('*CLS')
+			correct = False
+			opc = self._query_str_no_events('*OPC?')
+			repeat = 0
+			while not correct:
+				if len(opc) <= 2:
+					opc = opc.strip()
+					correct = opc == '0' or opc == '1'
+				if not correct:
+					# Read again with a small VISA timeout
+					opc = self._read_str_timed(5, True)
+				repeat += 1
+				if repeat > 10:
+					break
+
+		stb = self._query_stb()
+		condition = StatusByte.error_queue_not_empty | StatusByte.message_available | StatusByte.event_status_byte
+		if not stb & condition:
+			return
+		repeat = 0
+		# Loop more times to clear the status subsystem
+		while stb & condition:
+			if stb & StatusByte.error_queue_not_empty:
+				self.write('*CLS')
+				_ = self.query_all_syst_errors()
+			if stb & StatusByte.message_available:
+				# Clear output buffer
+				self._flush_junk_data()
+			if stb & StatusByte.event_status_byte:
+				# OPC or error bits in the ESR
+				self.write('*CLS')
+				self.query_and_clear_esr()
+			# Check if the status byte value changed
+			previous_stb = stb
+			stb = self._query_stb()
+			if stb == previous_stb:
+				repeat += 1
+				if repeat > 10:
+					raise Exception(f"Cannot clear the instrument's status subsystem. Status Byte: '{stb}'")
+
+	def _flush_junk_data(self) -> None:
+		"""Reads junk bytes to clear the instrument's output buffer."""
+		if self.read_delay > 0:
+			time.sleep(self.read_delay / 1000)
+		self._read_unknown_len(StreamWriter.as_bin_var(), False)
+
+	def clear(self) -> None:
+		"""Perform VISA viClear conditionally based on the instrument settings."""
+		perform_all = ViClearMode.execute_on_all in self._viclear_exe_mode
+		perform = False
+		if perform_all:
+			perform = True
+		else:
+			# Perform on all is blocked, use the SessionKind to decide
+			if self._interface_type == SessionKind.gpib:
+				perform = ViClearMode.execute_on_gpib in self._viclear_exe_mode
+
+			elif self._interface_type == SessionKind.serial:
+				perform = ViClearMode.execute_on_serial in self._viclear_exe_mode
+
+			elif self._interface_type == SessionKind.socket:
+				perform = ViClearMode.execute_on_socket in self._viclear_exe_mode
+
+			elif self._interface_type == SessionKind.usb:
+				perform = ViClearMode.execute_on_usb in self._viclear_exe_mode
+
+			elif self._interface_type == SessionKind.vxi11:
+				perform = ViClearMode.execute_on_tcpvxi in self._viclear_exe_mode
+
+		if not perform:
+			return
+
+		if ViClearMode.ignore_error in self._viclear_exe_mode:
+			# noinspection PyBroadException
+			try:
+				self._session.clear()
+			except Exception:
+				pass
+		else:
+			self._session.clear()
+
+	def _write_and_wait_for_opc(self, command: str, is_query: bool, timeout: int) -> StatusByte:
+		"""Internal method to synchronise a command with OPC timeout.
+		Timeout value 0 means the OPC timeout is used."""
+		timeout = self._resolve_opc_timeout(timeout)
+
+		if command.endswith(self._term_char):
+			command = command.rstrip(self._term_char)
+		if is_query:
+			InstrumentErrors.assert_query_has_qmark(command, 'Query with OPC')
+		else:
+			InstrumentErrors.assert_cmd_has_no_qmark(command, 'Write with OPC')
+
+		if self._opc_wait_mode == WaitForOpcMode.opc_query:
+			if is_query:
+				raise Exception('Sending a query with OpcQuery synchronization is not possible')
+			stb = self._write_and_query_opc(command, timeout)
+		else:
+			# STB polling
+			end_stb_mask = StatusByte.error_queue_not_empty | StatusByte.event_status_byte
+			if is_query:
+				end_stb_mask |= StatusByte.message_available
+			if self.vxi_capable:
+				stb = self._write_and_poll_stb_vxi(command, is_query, timeout, end_stb_mask)
+			else:
+				stb = self._write_and_poll_stb_non_vxi(command, timeout, end_stb_mask)
+
+		return stb
+
+	def _write_and_query_opc(self, cmd: str, timeout: int) -> StatusByte:
+		"""Internal method to write a command followed by query_opc().
+		Used for opc-synchronization if the mode is set to WaitForOpcMode.opc_query or the session is not-vxi.
+		Timeout value 0 means the OPC timeout is used."""
+		old_tout = self.visa_timeout
+
+		# Change VISA Timeout if necessary
+		if old_tout != timeout:
+			self.visa_timeout = timeout
+		try:
+			# try-catch to set the VISA timeout back
+			self.write(cmd)
+			self.query_opc()
+		finally:
+			if old_tout != timeout:
+				self.visa_timeout = old_tout
+		return self._query_stb()
+
+	def write(self, cmd: str) -> None:
+		"""Writes command to the instrument."""
+		if self.write_delay > 0:
+			time.sleep(self.write_delay / 1000)
+		add_tc = False
+		if self._assure_write_with_tc and not cmd.endswith(self._term_char):
+			add_tc = True
+		if add_tc:
+			self._session.write(cmd + self._term_char)
+		else:
+			self._session.write(cmd)
+
+	def _read_unknown_len(self, stream: StreamWriter, allow_chunk_events: bool, prepend_data: AnyStr = None) -> None:
+		"""Reads data of unknown length to the provided WriteStream.
+		The read is performed in an incremental chunk steps to optimize memory use (for NRP-Z session it is set to fixed self._data_chunk_size):
+			- The first read is performed with the fixed size of 1024 bytes
+			- The 2nd one reads 64 kBytes
+			- The 3rd one reads 128 kBytes
+			- The 4th one reads 256 kBytes and so on, with the max cap of self._data_chunk_size
+		:param stream: [StreamWriter] target for the read data
+		:param allow_chunk_events: [bool] if True, the method can send the chunk_events. If False, sending events is blocked.
+		:param prepend_data: Optional[bytes or string] You can prepend this data to the beginning. It will be considered part of the first chunk read
+		:return: read data [bytes or string], depending on the parameter binary."""
+		with self._session.ignore_warning(pyvisa.constants.StatusCode.success_max_count_read):
+			if prepend_data and isinstance(prepend_data, str):
+				prepend_data = prepend_data.encode('utf-8')
+			chunk_ix = 0
+			eot = False
+			while not eot:
+				if self.is_rsnrp_session():
+					chunk_size = self._data_chunk_size
+				else:
+					if chunk_ix == 0:
+						# First read, set 1024 bytes read size
+						chunk_size = 1024
+					elif chunk_ix == 1:
+						chunk_size = 65536
+					else:
+						chunk_size *= 2
+				if chunk_size > self._data_chunk_size:
+					chunk_size = self._data_chunk_size
+				chunk, self.last_status = self._session.visalib.read(self._session.session, chunk_size)
+				if chunk_ix == 0 and prepend_data:
+					chunk = prepend_data + chunk
+				eot = not self._last_status_more_data_available()
+				if not stream.binary:
+					chunk = chunk.decode('utf-8')
+					if eot:
+						chunk = chunk.rstrip(self._term_char)
+				stream.write(chunk)
+				if self.on_read_chunk_handler and allow_chunk_events:
+					total_size = len(stream) if eot is True else None
+					event_args = EventArgsChunk(stream.binary, chunk_ix, len(chunk), total_size, len(stream), eot, None, chunk if self.io_events_include_data else None)
+					self.on_read_chunk_handler(event_args)
+				chunk_ix += 1
+
+	def _last_status_more_data_available(self):
+		"""Returns True, if the last status signalled that more data is available"""
+		return self.last_status == pyvisa.constants.StatusCode.success_max_count_read
+
+	def _read_str_no_events(self) -> str:
+		"""Reads response from the instrument. The response is then trimmed for trailing LF. \n
+		Sending of any read events is blocked."""
+		if self.read_delay > 0:
+			time.sleep(self.read_delay / 1000)
+		stream = StreamWriter.as_string_var()
+		self._read_unknown_len(stream, False)
+		return stream.content
+
+	def _query_str_no_events(self, query: str) -> str:
+		"""Queries the instrument and reads the response as string.
+		The length of the string is not limited. The response is then trimmed for trailing LF.
+		Sending of any read events is blocked. Use this method for all the service VisaSession queries."""
+		response = ''
+		self.write(query)
+		try:
+			response = self._read_str_no_events()
+		except pyvisa.VisaIOError:
+			self._narrow_down_io_tout_error(f"Querying '{query.rstrip(self._term_char)}' - ")
+		return response
+
+	def _query_str_no_events_timed(self, query: str, timeout: int, suppress_read_tout: bool = False) -> str:
+		"""Queries the instrument and reads the response as string.
+		The entered timeout sets the VISA timeout just for this call. You can suppress the timeout error.
+		The length of the string is not limited. The response is then trimmed for trailing LF.
+		Sending of any read events is blocked. Use this method for all the service VisaSession queries."""
+		response = ''
+		self.write(query)
+		try:
+			response = self._read_str_timed(timeout, suppress_read_tout)
+		except pyvisa.VisaIOError:
+			self._narrow_down_io_tout_error(f"Querying with timeout {timeout} ms '{query.rstrip(self._term_char)}' - ", timeout)
+		return response
+
+	def _read_str_timed(self, timeout: int, suppress_read_tout: bool = False) -> str:
+		"""Reads response from the instrument with a VISA timeout temporarily set for the read.
+		The VISA timeout is set back to the previous value before the method finishes even if an exception occurs.
+		Sending of any read events is blocked."""
+		old_visa_tout = self.visa_timeout
+		if suppress_read_tout:
+			try:
+				if timeout != old_visa_tout:
+					self.visa_timeout = timeout
+				data = self._read_str_no_events()
+				return data
+			except TimeoutError:
+				pass
+			finally:
+				self.visa_timeout = old_visa_tout
+		else:
+			try:
+				if timeout != old_visa_tout:
+					self.visa_timeout = timeout
+				data = self._read_str_no_events()
+				return data
+			finally:
+				self.visa_timeout = old_visa_tout
+
+	def _read_str(self) -> str:
+		"""Reads response from the instrument. The response is then trimmed for trailing LF."""
+		if self.read_delay > 0:
+			time.sleep(self.read_delay / 1000)
+		stream = StreamWriter.as_string_var()
+		self._read_unknown_len(stream, True)
+		return stream.content
+
+	def query_str(self, query: str) -> str:
+		"""Queries the instrument and reads the response as string.
+		The length of the string is not limited. The response is then trimmed for trailing LF."""
+		response = ''
+		self.write(query)
+		try:
+			response = self._read_str()
+		except pyvisa.VisaIOError:
+			self._narrow_down_io_tout_error(f"Querying '{query.rstrip(self._term_char)}' - ")
+		return response
+
+	def query_str_no_tout_err(self, query: str, tout: int) -> str:
+		"""Same as query_str, but you can set the timeout just for this one call.
+		If the timeout exception occurs, it is suppressed and the method returns Null"""
+		response = None
+		old_tout = self.visa_timeout
+		try:
+			self.visa_timeout = tout
+			response = self.query_str(query)
+		except (pyvisa.VisaIOError, InstrumentErrors.StatusException):
+			pass
+		finally:
+			self.visa_timeout = old_tout
+		return response
+
+	def write_with_opc(self, command: str, timeout: int = None) -> None:
+		"""Sends command with OPC-sync.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		self._write_and_wait_for_opc(command, False, timeout)
+
+	def query_str_with_opc(self, query: str, timeout: int = None) -> str:
+		"""Query string with OPC synchronization.
+		The response is trimmed for any trailing LF.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		timeout = self._resolve_opc_timeout(timeout)
+		if self.vxi_capable and self._opc_wait_mode is not WaitForOpcMode.opc_query:
+			# For Vxi session, use the STB poll or SRQ wait and then read the response
+			stb = self._write_and_wait_for_opc(query, True, timeout)
+			self._check_msg_available_after_opc_wait(stb, query, timeout, 'Query String With OPC')
+			response = self._read_str()
+		else:
+			# For non-Vxi sessions, use the longer VISA Timeout without the *OPC?
+			# Same is valid for WaitForOpcMode.OpcQuery
+			InstrumentErrors.assert_query_has_qmark(query, 'Query with VISA timeout')
+			self.write(query)
+			old_tout = self.visa_timeout
+			# Change VISA Timeout if necessary
+			if old_tout != timeout:
+				self.visa_timeout = timeout
+			try:
+				# try-catch to set the VISA timeout back
+				response = self._read_str()
+				if self._opc_wait_mode is WaitForOpcMode.opc_query:
+					self.query_opc()
+			finally:
+				if old_tout != timeout:
+					self.visa_timeout = old_tout
+
+		return response
+
+	def query_opc(self, timeout: int = 0) -> bool:
+		"""Sends *OPC? query and reads the result.
+		If you define timeout > 0, the VISA timeout is set to that value just for this method call."""
+		if self.disable_opc_query:
+			return True
+		if timeout > 0:
+			response = self._query_str_no_events_timed('*OPC?', timeout)
+		else:
+			response = self._query_str_no_events('*OPC?')
+		return Conv.str_to_bool(response)
+
+	def query_and_clear_esr(self) -> int:
+		"""Sends *ESR? query and reads the result."""
+		response = self._query_str_no_events('*ESR?')
+		return int(response)
+
+	def _check_msg_available_after_opc_wait(self, stb: StatusByte, query: str, timeout: int, context: str) -> None:
+		"""Used internally after _StbPolling() to check if the message is available.
+		Throws an exception in case of MAV not available."""
+		if not self.vxi_capable:
+			return
+		if stb & StatusByte.message_available:
+			return
+		# Message not available
+		context = context + f" SCPI query '{query.rstrip(self._term_char)}'"
+		if stb & StatusByte.error_queue_not_empty:
+			# Instrument reports an error
+			InstrumentErrors.assert_no_instrument_status_errors(self._resource_name, self.query_all_syst_errors(), context)
+		else:
+			# Sometimes even if the StatusByte.MessageAvailable is false, the message is available.
+			# Try to read the STB again
+			stb = self._read_stb()
+			if not stb & StatusByte.event_status_byte:
+				# Instrument did not respond within the defined time
+				InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout, f'{context} No response from the instrument.')
+
+	def error_in_error_queue(self) -> bool:
+		"""Returns true, if error queue contains at least one error."""
+		stb = self._query_stb()
+		return (stb & StatusByte.error_queue_not_empty) != 0
+
+	def reset_ese_sre(self) -> None:
+		"""Resets the status of ESE and SRE registers to default values."""
+		self._set_regs_ese_sre(self._opc_wait_mode)
+
+	def write_bin_block(self, cmd: str, data_stream: StreamReader) -> None:
+		"""Writes all the payload as binary data block to the instrument.
+		The binary data header is added at the beginning of the transmission automatically.
+		:param cmd: [str] SCPI command with which to send the data
+		:param data_stream: [StreamReader] data provider for the payload"""
+		data_size = len(data_stream)
+		len_str = f'{data_size}'
+		cmd = cmd.rstrip(self._term_char)
+		if '#' in cmd:
+			raise Exception(
+				f"Command '{cmd}' must be provided without the binary data header. "
+				f"The method 'write_bin_block' composes and prepends the binary data header automatically.")
+		if data_size <= self._std_bin_block_header_max_len:
+			# Standard bin data header for sizes below 1E9 bytes, e.g.: '#512345'
+			cmd_plus_header = f'{cmd}#{len(len_str)}{len_str}'.encode('utf-8')
+		else:
+			# Big sizes bin data header: e.g.: '#(3000000000)'
+			cmd_plus_header = f'{cmd}#({len_str})'.encode('utf-8')
+
+		if data_size <= self._data_chunk_size:
+			# Write all in one step
+			full_chunk = data_stream.read_as_binary()
+			write_buf = cmd_plus_header + full_chunk
+			if self._add_term_char_to_write_bin_block:
+				write_buf += self._term_char_bin
+			self._session.write_raw(write_buf)
+			# Event sending
+			if self.on_write_chunk_handler:
+				event_args = EventArgsChunk(True, 0, data_size, data_size, data_size, True, 1, full_chunk if self.io_events_include_data else None)
+				self.on_write_chunk_handler(event_args)
+		else:
+			# Write in chunks
+			try:
+				# Use finally to set the session send_end back to True
+				self._session.send_end = False
+				total_chunks = calculate_chunks_count(data_size, self._data_chunk_size)
+				chunk_ix = 0
+				if self.write_delay > 0:
+					time.sleep(self.write_delay / 1000)
+				# Write bin header
+				self._session.write_raw(cmd_plus_header)
+				# Write chunks
+				while True:
+					if len(data_stream) > self._data_chunk_size:
+						#  Not the last segment
+						chunk = data_stream.read_as_binary(self._data_chunk_size)
+						self._session.write_raw(chunk)
+						# Event sending
+						if self.on_write_chunk_handler:
+							event_args = EventArgsChunk(
+								True, chunk_ix, self._data_chunk_size, data_size, data_size - len(data_stream), False, total_chunks, chunk if self.io_events_include_data else None)
+							self.on_write_chunk_handler(event_args)
+					else:
+						# Last segment, indicate end of message again
+						chunk = data_stream.read_as_binary()
+						if self._add_term_char_to_write_bin_block:
+							# Append LF
+							self._session.write_raw(chunk)
+							self._session.send_end = True
+							self._session.write_raw(self._term_char_bin)
+						else:
+							self._session.send_end = True
+							self._session.write_raw(chunk)
+
+						# Event sending
+						if self.on_write_chunk_handler:
+							event_args = EventArgsChunk(True, chunk_ix, len(chunk), data_size, data_size, True, total_chunks, chunk if self.io_events_include_data else None)
+							self.on_write_chunk_handler(event_args)
+						break
+					chunk_ix += 1
+			finally:
+				self._session.send_end = True
+
+	def _parse_bin_data_header(self, exc_if_not_bin: bool) -> Tuple[ReadDataType, str, int]:
+		"""Parses the binary data block and returns the expected length of the following data block. \n
+		:param exc_if_not_bin: [bool] if True, the method throws exception in case the data is not binary.
+		:return: read_data_type: [ReadDataType], parsed_header: [string], bin_data_len: [integer]"""
+		length = -1
+		if self.read_delay > 0:
+			time.sleep(self.read_delay / 1000)
+
+		char: AnyStr = self._session.read_bytes(1, break_on_termchar=True)
+		if char == b'#':
+			# binary transfer
+			char = self._session.read_bytes(1, break_on_termchar=True)
+			if char == b'0':
+				data_type = ReadDataType.bin_unknown_len
+				return data_type, '#0', -1
+			if char == b'(':
+				# format for big lengths i.e. > 1E9 bytes: '#(1234567890123)...'
+				data_type = ReadDataType.bin_known_len
+				len_str = (self.read_up_to_char(b')', 100)[:-1]).decode('utf-8')
+				whole_hdr = '#(' + len_str + ')'
+				length = int(len_str)
+				return data_type, whole_hdr, length
+
+			# classic format for < 1E9 bytes: '#9123456789...'
+			data_type = ReadDataType.bin_known_len
+			len_of_len = int(char)
+			len_str = self._session.read_bytes(len_of_len).decode('utf-8')
+			length = int(len_str)
+			whole_hdr = '#' + char.decode('utf-8') + len_str
+			return data_type, whole_hdr, length
+
+		data_type = ReadDataType.ascii
+		if char == self._term_char_bin:
+			data_type = ReadDataType.null
+		if self.vxi_capable:
+			# For Vxi session, to be sure, check whether there are more chars in the read buffer
+			stb = self._read_stb()
+			if stb & StatusByte.message_available:
+				data_type = ReadDataType.ascii
+		whole_hdr = char.decode('utf-8')
+		if exc_if_not_bin:
+			if data_type == ReadDataType.null:
+				InstrumentErrors.throw_bin_block_unexp_resp_exception(self._resource_name, self._term_char)
+			# Read 20 more characters to compose a better exception message
+			whole_hdr += self.read_up_to_char(self._term_char_bin, 20).decode('utf-8')
+			if self.last_status == pyvisa.constants.StatusCode.success_max_count_read:
+				self._flush_junk_data()
+			InstrumentErrors.throw_bin_block_unexp_resp_exception(self._resource_name, whole_hdr)
+		return data_type, whole_hdr, length
+
+	def read_bin_block(self, stream: StreamWriter, exc_if_not_bin: bool) -> None:
+		"""Reads binary data block to the provided stream. \n
+		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
+		:param exc_if_not_bin: if True, the method throws exception if the received data is not binary"""
+		data_type, header, length = self._parse_bin_data_header(exc_if_not_bin)
+		if data_type == ReadDataType.ascii:
+			stream.switch_to_string_data()
+			self._read_unknown_len(stream, True, header)
+		elif data_type == ReadDataType.null:
+			# No data, consider it ASCII, Return empty string, and False (signaling ASCII transfer)
+			stream.switch_to_string_data()
+		elif data_type == ReadDataType.bin_unknown_len:
+			if not self.vxi_capable:
+				raise Exception(f'Non-Vxi11 sessions can not read binary data block of unknown length.')
+			self._read_unknown_len(stream, True)
+		elif length == 0:
+			self._flush_junk_data()
+		else:
+			self._read_bin_block_known_len(stream, length)
+
+	def _read_bin_block_known_len(self, stream: StreamWriter, length: int) -> None:
+		"""Reads binary data of defined length. All remaining data above the length are disposed of. \n
+		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
+		:param length: [int] expected length of the data"""
+		# Use try-catch to switch the termination character back ON in case of an exception (for non-Vxi sessions)
+		try:
+			# Binary transmission, for non-Vxi session, set the termination character to OFF
+			if not self.vxi_capable:
+				self._session.read_termination = False
+			# Binary data of known length
+			left_to_read = length
+			self.last_status = pyvisa.constants.StatusCode.success
+			with self._session.ignore_warning(pyvisa.constants.StatusCode.success_max_count_read):
+				chunk_ix = 0
+				total_chunks = calculate_chunks_count(length, self._data_chunk_size)
+				while len(stream) < length:
+					chunk_size = min(self._data_chunk_size, left_to_read)
+					chunk, self.last_status = self._session.visalib.read(self._session.session, chunk_size)
+					left_to_read -= len(chunk)
+					stream.write(chunk)
+					if self.on_read_chunk_handler:
+						event_args = EventArgsChunk(True, chunk_ix, chunk_size, length, len(stream), left_to_read == 0, total_chunks, chunk if self.io_events_include_data else None)
+						self.on_read_chunk_handler(event_args)
+					chunk_ix += 1
+			if self._last_status_more_data_available():
+				if not self.vxi_capable:
+					self._session.read_termination = self._term_char
+				self._flush_junk_data()
+		finally:
+			# Make sure that in any case the self._session.read_termination is ON again for non-Vxi sessions
+			if not self.vxi_capable:
+				self._session.read_termination = self._term_char
+
+	def query_bin_block(self, query: str, stream: StreamWriter, exc_if_not_bin: bool = True) -> None:
+		"""Query binary data block and returns it as byte data. \n
+		:param query: [str] query to send to the instrument
+		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
+		:param exc_if_not_bin: [Boolean] if True, the method throws exception if the received data is not binary"""
+		self.write(query)
+		self.read_bin_block(stream, exc_if_not_bin)
+		return
+
+	def query_bin_block_with_opc(self, query: str, stream: StreamWriter, exc_if_not_bin: bool = True, timeout: int = None) -> None:
+		"""Query binary data block with OPC and returns it as byte data.
+		:param query: [str] query to send to the instrument
+		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
+		:param exc_if_not_bin: [Boolean] if True, the method throws exception if the received data is not binary
+		:param timeout: Optional[Integer] timeout for the operation. If you skip it, the method uses the current opc timeout."""
+		timeout = self._resolve_opc_timeout(timeout)
+		if self.vxi_capable and self._opc_wait_mode != WaitForOpcMode.opc_query:
+			# For Vxi session, use the STB poll and read the response
+			stb = self._write_and_wait_for_opc(query, True, timeout)
+			self._check_msg_available_after_opc_wait(stb, query, timeout, 'query_bin_block_with_opc')
+			self.read_bin_block(stream, exc_if_not_bin)
+		else:
+			# For non-Vxi session, use the longer VISA Timeout without the *OPC
+			InstrumentErrors.assert_query_has_qmark(query, 'query_bin_block_with_opc')
+			self.write(query)
+			old_visa_timeout = self.visa_timeout
+			# Change VISA Timeout if necessary
+			if old_visa_timeout != timeout:
+				self.visa_timeout = timeout
+			try:
+				# try-catch to set the VISA timeout back
+				self.read_bin_block(stream, exc_if_not_bin)
+				if self._opc_wait_mode == WaitForOpcMode.opc_query:
+					self.query_opc()
+			finally:
+				# Change VISA Timeout back if necessary
+				if old_visa_timeout != timeout:
+					self.visa_timeout = old_visa_timeout
+
+	def read_up_to_char(self, stop_chars: bytes, max_cnt: int) -> bytes:
+		"""Reads until one of the stop_chars is read or the max_cnt is reached, or EOT is detected.
+		Returns the read data including the stop character."""
+		response = b''
+		for i in range(max_cnt):
+			char, self.last_status = self._session.visalib.read(self._session.session, 1)
+			response += char
+			if char in stop_chars:
+				break
+			if self.last_status != pyvisa.constants.StatusCode.success_max_count_read:
+				break
+		return response
+
+	def get_session_handle(self) -> object:
+		"""Returns the underlying pyvisa session."""
+		return self._session
+
+	def close(self) -> None:
+		"""Closes the Visa session.
+		If the object was created with the direct session input, the session is not closed."""
+		if not self.reusing_session:
+			self._session.close()
+
+	# Events
+
+
+class EventArgsChunk:
+	"""Event arguments for chunk io event."""
+
+	def __init__(
+			self,
+			binary: bool,
+			chunk_ix: int,
+			chunk_size: int,
+			total_size: int,
+			transferred_size: int,
+			end_of_transfer: bool,
+			total_chunks: int or None,
+			data: AnyStr = None):
+
+		self.binary = binary
+		self.chunk_ix = chunk_ix
+		self.total_chunks = total_chunks
+		self.chunk_size = chunk_size
+		self.transferred_size = transferred_size
+		self.total_size = total_size
+		self.end_of_transfer = end_of_transfer
+		self.data = data
+
+	def __str__(self):
+		if self.binary:
+			type_info = 'binary'
+		else:
+			type_info = 'ascii'
+		if not self.total_chunks:
+			chunk_info = f' chunk nr. {self.chunk_ix + 1}'
+		elif self.total_chunks > 1:
+			chunk_info = f' chunk nr. {self.chunk_ix + 1}/{self.total_chunks}'
+		else:
+			chunk_info = ' chunk nr. 1/1'
+		eot = ' (EOT)' if self.end_of_transfer else ''
+		result = \
+			f'EventArgsChunk {type_info},{chunk_info}, {size_to_kb_mb_string(self.chunk_size, True)}, ' \
+			f'sum {size_to_kb_mb_string(self.transferred_size, True)} / {size_to_kb_mb_string(self.total_size, True) if self.total_size else "<N.A.>"}{eot}.'
+		return result
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/Internal/VisaSessionSim.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/Internal/VisaSessionSim.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,187 +1,187 @@
-import threading
-from typing import Callable, Dict, AnyStr
-
-from . import InstrumentSettings
-from .StreamReader import StreamReader
-from .StreamWriter import StreamWriter
-
-
-# noinspection PyMethodMayBeStatic,PyUnusedLocal
-class VisaSessionSim(object):
-	"""Visa session in simulation mode.
-	Provides the properties for the simulation mode.
-	Also serves as a cache for the SCPI command values: If you query a SCPI command value, it returns the last set value by that SCPI command."""
-
-	def __init__(self, resource_name: str, settings: InstrumentSettings, direct_session=None):
-		# noinspection PyTypeChecker
-		self._data_chunk_size: int = None
-		# noinspection PyTypeChecker
-		self._lock: threading.RLock = None
-
-		# Event handlers
-		# noinspection PyTypeChecker
-		self.on_read_chunk_handler: Callable = None
-		"""If assigned a handler, the VisaSession sends it event on each read chunk transfer."""
-		# noinspection PyTypeChecker
-		self.on_write_chunk_handler: Callable = None
-		"""If assigned a handler, the VisaSession sends it event on each write chunk transfer."""
-		self.io_events_include_data: bool = False
-		"""If true, the VisaSession events sent to on_read_chunk_handler and on_write_chunk_handler contain transferred data."""
-
-		self.manufacturer: str = 'Rohde&Schwarz'
-		self._resource_name = resource_name
-		self.vxi_capable = True
-
-		# Changeable settings
-		self.opc_timeout = 10000 if settings.opc_timeout == 0 else settings.opc_timeout
-		self.visa_timeout = settings.visa_timeout
-		self.data_chunk_size = settings.io_segment_size
-
-		self._last_cmd = None
-
-		# If the return value is written to a cache, this flag signals if it was a cached value
-		self.cached_to_stream = False
-
-		# cache command values dictionary
-		self._cmd_vals_cache: Dict[str, AnyStr] = {}
-
-		# Decide, whether to create a new thread lock or the existing one from the direct_session
-		if direct_session and hasattr(direct_session, 'session_thread_rlock'):
-			rlock = direct_session.session_thread_rlock
-			if isinstance(rlock, type(threading.RLock())):
-				self.assign_lock(rlock)
-		if self.get_lock() is None:
-			# The existing session did not have a thread lock, assign a new one
-			self.assign_lock(threading.RLock())
-
-	def assign_lock(self, lock: threading.RLock) -> None:
-		"""Assigns the provided thread lock. The lock is only used by the parent class Instrument."""
-		self._lock = lock
-
-	def get_lock(self) -> threading.RLock:
-		"""Returns the current RLock object."""
-		return self._lock
-
-	def _update_cmd_vals_cache(self, cmd: str, param: AnyStr = None) -> None:
-		"""Parses out the parameter from the command and stores/updates them in the cache"""
-		aux = cmd.split(' ', 1)
-		if len(aux) < 2:
-			return
-		headers = aux[0].strip().lower()
-		param = aux[1].strip()
-		self._cmd_vals_cache[headers] = param
-
-	def _update_cmd_vals_cache_split(self, cmd: str, param: AnyStr) -> None:
-		"""Stores/updates cmd and param in the cache"""
-		headers = cmd.strip().lower()
-		self._cmd_vals_cache[headers] = param
-
-	def _get_cmd_cached_value(self, cmd: str) -> str or None:
-		"""Returns cached parameter to the corresponding command
-		Returns None of the command is not found in the cache"""
-		aux = cmd.split('?', 1)
-		headers = aux[0].strip().lower()
-		return self._cmd_vals_cache.get(headers, None)
-
-	def get_last_sent_cmd(self) -> str:
-		"""Returns the last commands sent to the instrument"""
-		return self._last_cmd
-
-	def is_rsnrp_session(self) -> bool:
-		"""Returns True, if the current session is a NRP-Z session"""
-		return False
-
-	def query_syst_error(self) -> str or None:
-		"""Returns one response to the SYSTEM:ERROR? query."""
-		return None
-
-	def query_all_syst_errors(self) -> list or None:
-		"""Returns all errors in the instrument's error queue."""
-		return []
-
-	def clear_before_read(self) -> None:
-		"""Clears IO buffers and the ESR register before reading/writing responses synchronized with *OPC."""
-		return
-
-	def clear(self) -> None:
-		"""Perform VISA viClear conditionally based on the instrument settings."""
-		return
-
-	def write(self, cmd: str) -> None:
-		"""Writes command to the instrument."""
-		self._last_cmd = cmd
-		self._update_cmd_vals_cache(cmd)
-		return
-
-	def query_str(self, query: str) -> str:
-		"""Queries the instrument and reads the response as string.
-		The length of the string is not limited. The response is then trimmed for trailing LF."""
-		self._last_cmd = query
-		cached = self._get_cmd_cached_value(query)
-		return 'Simulating' if cached is None else cached
-
-	def write_with_opc(self, cmd: str, timeout: int = None) -> None:
-		"""Sends command with OPC-sync.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		self.write(cmd)
-
-	def query_str_with_opc(self, query: str, timeout: int = None) -> str:
-		"""Query string with OPC synchronization.
-		The response is trimmed for any trailing LF.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		return self.query_str(query)
-
-	def query_opc(self) -> bool:
-		"""Sends *OPC? query and reads the result."""
-		return True
-
-	def query_and_clear_esr(self) -> int:
-		"""Sends *ESR? query and reads the result."""
-		return 0
-
-	def error_in_error_queue(self) -> bool:
-		"""Returns true, if error queue contains at least one error."""
-		return False
-
-	def reset_ese_sre(self) -> None:
-		"""Resets the status of ESE and SRE registers to default values."""
-		return
-
-	def write_bin_block(self, cmd: str, data_stream: StreamReader) -> None:
-		"""Writes all the payload as binary data block to the instrument.
-		The binary data header is added at the beginning of the transmission automatically."""
-		self._last_cmd = cmd
-		param = data_stream.read()
-		self._update_cmd_vals_cache_split(cmd, param)
-
-	def query_bin_block(self, query: str, stream: StreamWriter, exc_if_not_bin: bool = True) -> None:
-		"""Query binary data block and returns it as byte data."""
-		self._last_cmd = query
-		cached = self._get_cmd_cached_value(query)
-
-		if cached is None:
-			stream.write(bytes([0, 1, 2, 3, 4, 5, 6, 7, 8, 65, 66]))
-			self.cached_to_stream = False
-		else:
-			if isinstance(cached, str):
-				stream.switch_to_string_data()
-			stream.write(cached)
-			self.cached_to_stream = True
-
-	def query_bin_block_with_opc(self, query: str, stream: StreamWriter, exc_if_not_bin: bool = True, timeout: int = None) -> None:
-		"""Query binary data block with OPC and returns it as byte data."""
-		self.query_bin_block(query, stream)
-
-	def read_up_to_char(self, stop_chars: bytes, max_cnt: int) -> bytes:
-		"""Reads until one of the stop_chars is read or the max_cnt is reached, or EOT is detected.
-		Returns the read data including the stop character."""
-		return b'Simulating'
-
-	def get_session_handle(self) -> object:
-		"""Returns the underlying pyvisa session."""
-		return f"Simulating session, resource name '{self._resource_name}'"
-
-	def close(self) -> None:
-		"""Closes the Visa session.
-		If the object was created with the direct session input, the session is not closed."""
-		return
+import threading
+from typing import Callable, Dict, AnyStr
+
+from . import InstrumentSettings
+from .StreamReader import StreamReader
+from .StreamWriter import StreamWriter
+
+
+# noinspection PyMethodMayBeStatic,PyUnusedLocal
+class VisaSessionSim(object):
+	"""Visa session in simulation mode.
+	Provides the properties for the simulation mode.
+	Also serves as a cache for the SCPI command values: If you query a SCPI command value, it returns the last set value by that SCPI command."""
+
+	def __init__(self, resource_name: str, settings: InstrumentSettings, direct_session=None):
+		# noinspection PyTypeChecker
+		self._data_chunk_size: int = None
+		# noinspection PyTypeChecker
+		self._lock: threading.RLock = None
+
+		# Event handlers
+		# noinspection PyTypeChecker
+		self.on_read_chunk_handler: Callable = None
+		"""If assigned a handler, the VisaSession sends it event on each read chunk transfer."""
+		# noinspection PyTypeChecker
+		self.on_write_chunk_handler: Callable = None
+		"""If assigned a handler, the VisaSession sends it event on each write chunk transfer."""
+		self.io_events_include_data: bool = False
+		"""If true, the VisaSession events sent to on_read_chunk_handler and on_write_chunk_handler contain transferred data."""
+
+		self.manufacturer: str = 'Rohde&Schwarz'
+		self._resource_name = resource_name
+		self.vxi_capable = True
+
+		# Changeable settings
+		self.opc_timeout = 10000 if settings.opc_timeout == 0 else settings.opc_timeout
+		self.visa_timeout = settings.visa_timeout
+		self.data_chunk_size = settings.io_segment_size
+
+		self._last_cmd = None
+
+		# If the return value is written to a cache, this flag signals if it was a cached value
+		self.cached_to_stream = False
+
+		# cache command values dictionary
+		self._cmd_vals_cache: Dict[str, AnyStr] = {}
+
+		# Decide, whether to create a new thread lock or the existing one from the direct_session
+		if direct_session and hasattr(direct_session, 'session_thread_rlock'):
+			rlock = direct_session.session_thread_rlock
+			if isinstance(rlock, type(threading.RLock())):
+				self.assign_lock(rlock)
+		if self.get_lock() is None:
+			# The existing session did not have a thread lock, assign a new one
+			self.assign_lock(threading.RLock())
+
+	def assign_lock(self, lock: threading.RLock) -> None:
+		"""Assigns the provided thread lock. The lock is only used by the parent class Instrument."""
+		self._lock = lock
+
+	def get_lock(self) -> threading.RLock:
+		"""Returns the current RLock object."""
+		return self._lock
+
+	def _update_cmd_vals_cache(self, cmd: str, param: AnyStr = None) -> None:
+		"""Parses out the parameter from the command and stores/updates them in the cache"""
+		aux = cmd.split(' ', 1)
+		if len(aux) < 2:
+			return
+		headers = aux[0].strip().lower()
+		param = aux[1].strip()
+		self._cmd_vals_cache[headers] = param
+
+	def _update_cmd_vals_cache_split(self, cmd: str, param: AnyStr) -> None:
+		"""Stores/updates cmd and param in the cache"""
+		headers = cmd.strip().lower()
+		self._cmd_vals_cache[headers] = param
+
+	def _get_cmd_cached_value(self, cmd: str) -> str or None:
+		"""Returns cached parameter to the corresponding command
+		Returns None of the command is not found in the cache"""
+		aux = cmd.split('?', 1)
+		headers = aux[0].strip().lower()
+		return self._cmd_vals_cache.get(headers, None)
+
+	def get_last_sent_cmd(self) -> str:
+		"""Returns the last commands sent to the instrument"""
+		return self._last_cmd
+
+	def is_rsnrp_session(self) -> bool:
+		"""Returns True, if the current session is a NRP-Z session"""
+		return False
+
+	def query_syst_error(self) -> str or None:
+		"""Returns one response to the SYSTEM:ERROR? query."""
+		return None
+
+	def query_all_syst_errors(self) -> list or None:
+		"""Returns all errors in the instrument's error queue."""
+		return []
+
+	def clear_before_read(self) -> None:
+		"""Clears IO buffers and the ESR register before reading/writing responses synchronized with *OPC."""
+		return
+
+	def clear(self) -> None:
+		"""Perform VISA viClear conditionally based on the instrument settings."""
+		return
+
+	def write(self, cmd: str) -> None:
+		"""Writes command to the instrument."""
+		self._last_cmd = cmd
+		self._update_cmd_vals_cache(cmd)
+		return
+
+	def query_str(self, query: str) -> str:
+		"""Queries the instrument and reads the response as string.
+		The length of the string is not limited. The response is then trimmed for trailing LF."""
+		self._last_cmd = query
+		cached = self._get_cmd_cached_value(query)
+		return 'Simulating' if cached is None else cached
+
+	def write_with_opc(self, cmd: str, timeout: int = None) -> None:
+		"""Sends command with OPC-sync.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		self.write(cmd)
+
+	def query_str_with_opc(self, query: str, timeout: int = None) -> str:
+		"""Query string with OPC synchronization.
+		The response is trimmed for any trailing LF.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		return self.query_str(query)
+
+	def query_opc(self, timeout: int = 0) -> bool:
+		"""Sends *OPC? query and reads the result."""
+		return True
+
+	def query_and_clear_esr(self) -> int:
+		"""Sends *ESR? query and reads the result."""
+		return 0
+
+	def error_in_error_queue(self) -> bool:
+		"""Returns true, if error queue contains at least one error."""
+		return False
+
+	def reset_ese_sre(self) -> None:
+		"""Resets the status of ESE and SRE registers to default values."""
+		return
+
+	def write_bin_block(self, cmd: str, data_stream: StreamReader) -> None:
+		"""Writes all the payload as binary data block to the instrument.
+		The binary data header is added at the beginning of the transmission automatically."""
+		self._last_cmd = cmd
+		param = data_stream.read()
+		self._update_cmd_vals_cache_split(cmd, param)
+
+	def query_bin_block(self, query: str, stream: StreamWriter, exc_if_not_bin: bool = True) -> None:
+		"""Query binary data block and returns it as byte data."""
+		self._last_cmd = query
+		cached = self._get_cmd_cached_value(query)
+
+		if cached is None:
+			stream.write(bytes([0, 1, 2, 3, 4, 5, 6, 7, 8, 65, 66]))
+			self.cached_to_stream = False
+		else:
+			if isinstance(cached, str):
+				stream.switch_to_string_data()
+			stream.write(cached)
+			self.cached_to_stream = True
+
+	def query_bin_block_with_opc(self, query: str, stream: StreamWriter, exc_if_not_bin: bool = True, timeout: int = None) -> None:
+		"""Query binary data block with OPC and returns it as byte data."""
+		self.query_bin_block(query, stream)
+
+	def read_up_to_char(self, stop_chars: bytes, max_cnt: int) -> bytes:
+		"""Reads until one of the stop_chars is read or the max_cnt is reached, or EOT is detected.
+		Returns the read data including the stop character."""
+		return b'Simulating'
+
+	def get_session_handle(self) -> object:
+		"""Returns the underlying pyvisa session."""
+		return f"Simulating session, resource name '{self._resource_name}'"
+
+	def close(self) -> None:
+		"""Closes the Visa session.
+		If the object was created with the direct session input, the session is not closed."""
+		return
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/RsCMPX_Base.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/RsCMPX_Base.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .Internal.VisaSession import VisaSession
 from .Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class RsCMPX_Base:
 	"""433 total commands, 29 Sub-groups, 3 group commands"""
-	driver_options = "SupportedInstrModels = CMX500/CMP/CMW, SupportedIdnPatterns = CMX/CMP/CMW, SimulationIdnString = 'Rohde&Schwarz,CMX,100001,4.0.7.0008'"
+	_driver_options = "SupportedInstrModels = CMX500/CMP/CMW, SupportedIdnPatterns = CMX/CMP/CMW, SimulationIdnString = 'Rohde&Schwarz,CMX,100001,4.0.7.0009'"
 
 	def __init__(self, resource_name: str, id_query: bool = True, reset: bool = False, options: str = None, direct_session: object = None):
 		"""Initializes new RsCMPX_Base session. \n
 		Parameter options tokens examples:
 			- 'Simulate=True' - starts the session in simulation mode. Default: False
 			- 'SelectVisa=socket' - uses no VISA implementation for socket connections - you do not need any VISA-C installation
 			- 'SelectVisa=rs' - forces usage of RohdeSchwarz Visa
@@ -31,25 +31,25 @@
 			- 'DriverSetup=(ViClearExeMode = 255)' - Binary combination where 1 means performing viClear() on a certain interface as the very first command in init
 			- 'DriverSetup=(OpcQueryAfterWrite = True)' - same as driver.utilities.opc_query_after_write = True
 		:param resource_name: VISA resource name, e.g. 'TCPIP::192.168.2.1::INSTR'
 		:param id_query: if True: the instrument's model name is verified against the models supported by the driver and eventually throws an exception.
 		:param reset: Resets the instrument (sends *RST command) and clears its status sybsystem
 		:param options: string tokens alternating the driver settings.
 		:param direct_session: Another driver object or pyVisa object to reuse the session instead of opening a new session."""
-		self._core = Core(resource_name, id_query, reset, RsCMPX_Base.driver_options, options, direct_session)
-		self._core.driver_version = '4.0.7.0008'
+		self._core = Core(resource_name, id_query, reset, RsCMPX_Base._driver_options, options, direct_session)
+		self._core.driver_version = '4.0.7.0009'
 		self._options = options
 		self._add_all_global_repcaps()
 		self._custom_properties_init()
 		# noinspection PyTypeChecker
 		self._base = CommandsGroup("ROOT", self._core, None)
 
 	@classmethod
 	def from_existing_session(cls, session: object, options: str = None) -> 'RsCMPX_Base':
-		"""Creates a new RsCmwBluetoothSig object with the entered 'session' reused. \n
+		"""Creates a new RsCMPX_Base object with the entered 'session' reused. \n
 		:param session: can be an another driver or a direct pyvisa session.
 		:param options: string tokens alternating the driver settings."""
 		# noinspection PyTypeChecker
 		return cls(None, False, False, options, session)
 
 	def __str__(self) -> str:
 		if self._core.io:
@@ -58,25 +58,25 @@
 			return f"RsCMPX_Base with session closed"
 
 	@staticmethod
 	def assert_minimum_version(min_version: str) -> None:
 		"""Asserts that the driver version fulfills the minimum required version you have entered.
 		This way you make sure your installed driver is of the entered version or newer."""
 		min_version_list = min_version.split('.')
-		curr_version_list = '4.0.7.0008'.split('.')
+		curr_version_list = '4.0.7.0009'.split('.')
 		count_min = len(min_version_list)
 		count_curr = len(curr_version_list)
 		count = count_min if count_min < count_curr else count_curr
 		for i in range(count):
 			minimum = int(min_version_list[i])
 			curr = int(curr_version_list[i])
 			if curr > minimum:
 				break
 			if curr < minimum:
-				raise RsInstrException(f"Assertion for minimum RsCMPX_Base version failed. Current version: '4.0.7.0008', minimum required version: '{min_version}'")
+				raise RsInstrException(f"Assertion for minimum RsCMPX_Base version failed. Current version: '4.0.7.0009', minimum required version: '{min_version}'")
 				
 	@staticmethod
 	def list_resources(expression: str = '?*::INSTR', visa_select: str = None) -> List[str]:
 		"""Finds all the resources defined by the expression
 			- '?*' - matches all the available instruments
 			- 'USB::?*' - matches all the USB instruments
 			- "TCPIP::192?*' - matches all the LAN instruments with the IP address starting with 192
@@ -290,20 +290,20 @@
 		"""unit commands group. 0 Sub-classes, 13 commands."""
 		if not hasattr(self, '_unit'):
 			from .Implementations.Unit import Unit
 			self._unit = Unit(self._core, self._base)
 		return self._unit
 
 	@property
-	def goToLocal(self):
-		"""goToLocal commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_goToLocal'):
-			from .Implementations.GoToLocal import GoToLocal
-			self._goToLocal = GoToLocal(self._core, self._base)
-		return self._goToLocal
+	def gotoLocal(self):
+		"""gotoLocal commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_gotoLocal'):
+			from .Implementations.GotoLocal import GotoLocal
+			self._gotoLocal = GotoLocal(self._core, self._base)
+		return self._gotoLocal
 
 	@property
 	def trace(self):
 		"""trace commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_trace'):
 			from .Implementations.Trace import Trace
 			self._trace = Trace(self._core, self._base)
@@ -339,63 +339,64 @@
 		if not hasattr(self, '_massMemory'):
 			from .Implementations.MassMemory import MassMemory
 			self._massMemory = MassMemory(self._core, self._base)
 		return self._massMemory
 
 	def get_macro_enable(self) -> bool:
 		"""SCPI: *EMC \n
-		Snippet: value: bool = driver..get_macro_enable() \n
+		Snippet: value: bool = driver.get_macro_enable() \n
 		Enables or disables the execution of all macros that are defined for the active remote connection. Note: In contrast to
 		SCPI specifications, macro execution is disabled by default. \n
 			:return: enable: No help available
 		"""
 		response = self._core.io.query_str('*EMC?')
 		return Conversions.str_to_bool(response)
 
 	def set_macro_enable(self, enable: bool) -> None:
 		"""SCPI: *EMC \n
-		Snippet: driver..set_macro_enable(enable = False) \n
+		Snippet: driver.set_macro_enable(enable = False) \n
 		Enables or disables the execution of all macros that are defined for the active remote connection. Note: In contrast to
 		SCPI specifications, macro execution is disabled by default. \n
 			:param enable: Boolean value to enable or disable macro execution. In the disabled state (OFF / 0) , macros in a command sequence are not expanded. The R&S CMX500 issues an error message: 113, Undefined header;MacroLabel.
 		"""
 		param = Conversions.bool_to_str(enable)
 		self._core.io.write(f'*EMC {param}')
 
 	def get_device_number(self) -> int:
 		"""SCPI: *DEV \n
-		Snippet: value: int = driver..get_device_number() \n
+		Snippet: value: int = driver.get_device_number() \n
 		Queries the device number. It equals the Assigned Instrument number minus 1. \n
 			:return: instrument_no: No help available
 		"""
 		response = self._core.io.query_str('*DEV?')
 		return Conversions.str_to_int(response)
 
 	def set_device_number(self, instrument_no: int) -> None:
 		"""SCPI: *DEV \n
-		Snippet: driver..set_device_number(instrument_no = 1) \n
+		Snippet: driver.set_device_number(instrument_no = 1) \n
 		Queries the device number. It equals the Assigned Instrument number minus 1. \n
 			:param instrument_no: No help available
 		"""
 		param = Conversions.decimal_value_to_str(instrument_no)
 		self._core.io.write(f'*DEV {param}')
 
 	def get_global_opc(self) -> bool:
 		"""SCPI: *GOPC \n
-		Snippet: value: bool = driver..get_global_opc() \n
+		Snippet: value: bool = driver.get_global_opc() \n
 		No command help available \n
 			:return: gopc: No help available
 		"""
 		response = self._core.io.query_str('*GOPC?')
 		return Conversions.str_to_bool(response)
 
 	def clone(self) -> 'RsCMPX_Base':
 		"""Creates a deep copy of the RsCMPX_Base object. Also copies:
 			- All the existing Global repeated capability values
 			- All the default group repeated capabilities setting \n
+		Does not check the *IDN? response, and does not perform Reset.
 		After cloning, you can set all the repeated capabilities settings independentely from the original group.
 		Calling close() on the new object does not close the original VISA session"""
 		cloned = RsCMPX_Base.from_existing_session(self.get_session_handle(), self._options)
 		self._base.synchronize_repcaps(cloned)
 		
 		return cloned
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/enums.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/enums.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base/repcap.py` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base/repcap.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base.egg-info/PKG-INFO` & `RsCMPX_Base-4.0.7.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
-Name: RsCMPX-Base
-Version: 4.0.7.8
+Name: RsCMPX_Base
+Version: 4.0.7.9
 Summary: CMX/CMP Base System Remote-control Module
 Home-page: UNKNOWN
 Author: Rohde & Schwarz GmbH & Co. KG
 Author-email: Customer.Support@rohde-schwarz.com
 License: MIT
-Description: Rohde & Schwarz CMX/CMP Base System RsCMPX_Base instrument driver Version 4.0.7.8
+Description: Rohde & Schwarz CMX/CMP Base System RsCMPX_Base instrument driver.
         
-        Check out the module documentation on https://RsCMPX_Base.readthedocs.io/
+        Supported instruments: CMX500, CMP200
+        
+        The package is hosted here: https://pypi.org/project/RsCMPX_Base/
+        
+        Documentation: https://RsCMPX_Base.readthedocs.io/
+        
+        Examples: https://github.com/Rohde-Schwarz/Examples/
         
         --------------------------------------------------------------------------------
         
         Currently supported CMX/CMP subsystems:
         
         - Base: `RsCmpx_Base <https://RsCmpx_Base.readthedocs.io/>`_
         - GPRF: `RsCmpx_Gprf <https://RsCmpx_Gprf.readthedocs.io/>`_
@@ -25,19 +31,19 @@
         In case you require support for more subsystems, please contact our customer support on customersupport@rohde-schwarz.com
         with the topic "Auto-generated Python drivers" in the email subject. This will speed up the response process
         
         --------------------------------------------------------------------------------
         
         Release Notes: for the whole RsCmpx_xxx group:
         
-        Latest release notes summary: Added documentation on ReadTheDocs.io
+        Latest release notes summary: Added documentation on ReadTheDocs
         
         Version 4.0.7.4
         
-        - Added documentation on ReadTheDocs.io
+        - Added documentation on ReadTheDocs
         
         Version 4.0.7.3
         
         - Added new subsystems NrFr2Meas, UwbMeas, Signaling
         
         Version 4.0.7.2
```

### Comparing `RsCMPX_Base-4.0.7.8/RsCMPX_Base.egg-info/SOURCES.txt` & `RsCMPX_Base-4.0.7.9/RsCMPX_Base.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 RsCMPX_Base/Implementations/Diagnostic.py
 RsCMPX_Base/Implementations/Display.py
 RsCMPX_Base/Implementations/FirmwareUpdate.py
 RsCMPX_Base/Implementations/FormatPy.py
 RsCMPX_Base/Implementations/Get.py
 RsCMPX_Base/Implementations/GlobalClearStatus.py
 RsCMPX_Base/Implementations/GlobalWait.py
-RsCMPX_Base/Implementations/GoToLocal.py
+RsCMPX_Base/Implementations/GotoLocal.py
 RsCMPX_Base/Implementations/HardCopy.py
 RsCMPX_Base/Implementations/Instrument.py
 RsCMPX_Base/Implementations/MacroCreate.py
 RsCMPX_Base/Implementations/MassMemory.py
 RsCMPX_Base/Implementations/Procedure.py
 RsCMPX_Base/Implementations/RecallState.py
 RsCMPX_Base/Implementations/SaveState.py
@@ -93,15 +93,15 @@
 RsCMPX_Base/Implementations/Base_/Ipc_/__init__.py
 RsCMPX_Base/Implementations/Base_/MultiCmw_/Identify.py
 RsCMPX_Base/Implementations/Base_/MultiCmw_/Snumber.py
 RsCMPX_Base/Implementations/Base_/MultiCmw_/State.py
 RsCMPX_Base/Implementations/Base_/MultiCmw_/__init__.py
 RsCMPX_Base/Implementations/Base_/Salignment_/Llimit.py
 RsCMPX_Base/Implementations/Base_/Salignment_/Lvalid.py
-RsCMPX_Base/Implementations/Base_/Salignment_/Reliabiliy.py
+RsCMPX_Base/Implementations/Base_/Salignment_/Reliability.py
 RsCMPX_Base/Implementations/Base_/Salignment_/State.py
 RsCMPX_Base/Implementations/Base_/Salignment_/Trace.py
 RsCMPX_Base/Implementations/Base_/Salignment_/Ulimit.py
 RsCMPX_Base/Implementations/Base_/Salignment_/Xvalues.py
 RsCMPX_Base/Implementations/Base_/Salignment_/__init__.py
 RsCMPX_Base/Implementations/Base_/Salignment_/Llimit_/RxDc.py
 RsCMPX_Base/Implementations/Base_/Salignment_/Llimit_/RxImage.py
@@ -152,15 +152,15 @@
 RsCMPX_Base/Implementations/Configure_/Semaphore.py
 RsCMPX_Base/Implementations/Configure_/SingleCmw.py
 RsCMPX_Base/Implementations/Configure_/Spoint.py
 RsCMPX_Base/Implementations/Configure_/__init__.py
 RsCMPX_Base/Implementations/Configure_/Base_/Adjustment.py
 RsCMPX_Base/Implementations/Configure_/Base_/Correction.py
 RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection.py
-RsCMPX_Base/Implementations/Configure_/Base_/IpSubnet.py
+RsCMPX_Base/Implementations/Configure_/Base_/IpSet.py
 RsCMPX_Base/Implementations/Configure_/Base_/Ipcr.py
 RsCMPX_Base/Implementations/Configure_/Base_/Mmonitor.py
 RsCMPX_Base/Implementations/Configure_/Base_/MultiCmw.py
 RsCMPX_Base/Implementations/Configure_/Base_/Salignment.py
 RsCMPX_Base/Implementations/Configure_/Base_/__init__.py
 RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer.py
 RsCMPX_Base/Implementations/Configure_/Base_/Correction_/__init__.py
@@ -171,25 +171,22 @@
 RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/__init__.py
 RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/RxFilter_/Select.py
 RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/RxFilter_/__init__.py
 RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/TxFilter_/Select.py
 RsCMPX_Base/Implementations/Configure_/Base_/Correction_/IfEqualizer_/Slot_/TxFilter_/__init__.py
 RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable.py
 RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/__init__.py
-RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Add.py
 RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Catalog.py
 RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Count.py
-RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Create.py
 RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Details.py
-RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Erase.py
 RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Exist.py
 RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/Length.py
 RsCMPX_Base/Implementations/Configure_/Base_/FreqCorrection_/CorrectionTable_/__init__.py
-RsCMPX_Base/Implementations/Configure_/Base_/IpSubnet_/NwAdapter.py
-RsCMPX_Base/Implementations/Configure_/Base_/IpSubnet_/__init__.py
+RsCMPX_Base/Implementations/Configure_/Base_/IpSet_/NwAdapter.py
+RsCMPX_Base/Implementations/Configure_/Base_/IpSet_/__init__.py
 RsCMPX_Base/Implementations/Configure_/Base_/Mmonitor_/IpAddress.py
 RsCMPX_Base/Implementations/Configure_/Base_/Mmonitor_/__init__.py
 RsCMPX_Base/Implementations/Configure_/Base_/MultiCmw_/Identify.py
 RsCMPX_Base/Implementations/Configure_/Base_/MultiCmw_/__init__.py
 RsCMPX_Base/Implementations/Configure_/FreqCorrection_/Activate.py
 RsCMPX_Base/Implementations/Configure_/FreqCorrection_/Usage.py
 RsCMPX_Base/Implementations/Configure_/FreqCorrection_/__init__.py
@@ -204,14 +201,17 @@
 RsCMPX_Base/Implementations/Configure_/Semaphore_/__init__.py
 RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection.py
 RsCMPX_Base/Implementations/Configure_/SingleCmw_/__init__.py
 RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Activate.py
 RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate.py
 RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Usage.py
 RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/__init__.py
+RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Activate_/Rx.py
+RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Activate_/Tx.py
+RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Activate_/__init__.py
 RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Rx.py
 RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Tx.py
 RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/__init__.py
 RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Rx_/All.py
 RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Rx_/__init__.py
 RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Tx_/All.py
 RsCMPX_Base/Implementations/Configure_/SingleCmw_/FreqCorrection_/Deactivate_/Tx_/__init__.py
@@ -339,21 +339,21 @@
 RsCMPX_Base/Implementations/MassMemory_/Store_/Item.py
 RsCMPX_Base/Implementations/MassMemory_/Store_/Macro.py
 RsCMPX_Base/Implementations/MassMemory_/Store_/State.py
 RsCMPX_Base/Implementations/MassMemory_/Store_/__init__.py
 RsCMPX_Base/Implementations/Sense_/Base.py
 RsCMPX_Base/Implementations/Sense_/FirmwareUpdate.py
 RsCMPX_Base/Implementations/Sense_/__init__.py
-RsCMPX_Base/Implementations/Sense_/Base_/IpSubnet.py
+RsCMPX_Base/Implementations/Sense_/Base_/IpSet.py
 RsCMPX_Base/Implementations/Sense_/Base_/Reference.py
 RsCMPX_Base/Implementations/Sense_/Base_/Temperature.py
 RsCMPX_Base/Implementations/Sense_/Base_/__init__.py
-RsCMPX_Base/Implementations/Sense_/Base_/IpSubnet_/Snode.py
-RsCMPX_Base/Implementations/Sense_/Base_/IpSubnet_/SubMonitor.py
-RsCMPX_Base/Implementations/Sense_/Base_/IpSubnet_/__init__.py
+RsCMPX_Base/Implementations/Sense_/Base_/IpSet_/Snode.py
+RsCMPX_Base/Implementations/Sense_/Base_/IpSet_/SubMonitor.py
+RsCMPX_Base/Implementations/Sense_/Base_/IpSet_/__init__.py
 RsCMPX_Base/Implementations/Sense_/Base_/Reference_/Frequency.py
 RsCMPX_Base/Implementations/Sense_/Base_/Reference_/__init__.py
 RsCMPX_Base/Implementations/Sense_/Base_/Temperature_/Exceeded.py
 RsCMPX_Base/Implementations/Sense_/Base_/Temperature_/Operating.py
 RsCMPX_Base/Implementations/Sense_/Base_/Temperature_/__init__.py
 RsCMPX_Base/Implementations/Source_/Base.py
 RsCMPX_Base/Implementations/Source_/__init__.py
@@ -430,25 +430,25 @@
 RsCMPX_Base/Implementations/System_/SingleCmw.py
 RsCMPX_Base/Implementations/System_/Startup.py
 RsCMPX_Base/Implementations/System_/Time.py
 RsCMPX_Base/Implementations/System_/Update.py
 RsCMPX_Base/Implementations/System_/__init__.py
 RsCMPX_Base/Implementations/System_/Base_/Device.py
 RsCMPX_Base/Implementations/System_/Base_/Display.py
-RsCMPX_Base/Implementations/System_/Base_/IpSubnet.py
+RsCMPX_Base/Implementations/System_/Base_/IpSet.py
 RsCMPX_Base/Implementations/System_/Base_/Option.py
 RsCMPX_Base/Implementations/System_/Base_/Password.py
 RsCMPX_Base/Implementations/System_/Base_/Reference.py
 RsCMPX_Base/Implementations/System_/Base_/Ssync.py
 RsCMPX_Base/Implementations/System_/Base_/StIcon.py
 RsCMPX_Base/Implementations/System_/Base_/__init__.py
-RsCMPX_Base/Implementations/System_/Base_/IpSubnet_/SubMonitor.py
-RsCMPX_Base/Implementations/System_/Base_/IpSubnet_/__init__.py
-RsCMPX_Base/Implementations/System_/Base_/IpSubnet_/SubMonitor_/Refresh.py
-RsCMPX_Base/Implementations/System_/Base_/IpSubnet_/SubMonitor_/__init__.py
+RsCMPX_Base/Implementations/System_/Base_/IpSet_/SubMonitor.py
+RsCMPX_Base/Implementations/System_/Base_/IpSet_/__init__.py
+RsCMPX_Base/Implementations/System_/Base_/IpSet_/SubMonitor_/Refresh.py
+RsCMPX_Base/Implementations/System_/Base_/IpSet_/SubMonitor_/__init__.py
 RsCMPX_Base/Implementations/System_/Base_/Option_/Description.py
 RsCMPX_Base/Implementations/System_/Base_/Option_/ListPy.py
 RsCMPX_Base/Implementations/System_/Base_/Option_/Version.py
 RsCMPX_Base/Implementations/System_/Base_/Option_/__init__.py
 RsCMPX_Base/Implementations/System_/Base_/Password_/Cenable.py
 RsCMPX_Base/Implementations/System_/Base_/Password_/__init__.py
 RsCMPX_Base/Implementations/System_/Base_/Reference_/Dc.py
@@ -561,27 +561,27 @@
 RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Dexecution_/Duration.py
 RsCMPX_Base/Implementations/Trace_/Remote_/Mode_/File_/Dexecution_/__init__.py
 RsCMPX_Base/Implementations/Trigger_/Base.py
 RsCMPX_Base/Implementations/Trigger_/__init__.py
 RsCMPX_Base/Implementations/Trigger_/Base_/Eout.py
 RsCMPX_Base/Implementations/Trigger_/Base_/ExtA.py
 RsCMPX_Base/Implementations/Trigger_/Base_/ExtB.py
-RsCMPX_Base/Implementations/Trigger_/Base_/UserInitiated.py
+RsCMPX_Base/Implementations/Trigger_/Base_/Uinitiated.py
 RsCMPX_Base/Implementations/Trigger_/Base_/__init__.py
 RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/Catalog.py
 RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/Source.py
 RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/__init__.py
 RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/Catalog_/Source.py
 RsCMPX_Base/Implementations/Trigger_/Base_/Eout_/Catalog_/__init__.py
 RsCMPX_Base/Implementations/Trigger_/Base_/ExtA_/Catalog.py
 RsCMPX_Base/Implementations/Trigger_/Base_/ExtA_/__init__.py
 RsCMPX_Base/Implementations/Trigger_/Base_/ExtB_/Catalog.py
 RsCMPX_Base/Implementations/Trigger_/Base_/ExtB_/__init__.py
-RsCMPX_Base/Implementations/Trigger_/Base_/UserInitiated_/Execute.py
-RsCMPX_Base/Implementations/Trigger_/Base_/UserInitiated_/__init__.py
+RsCMPX_Base/Implementations/Trigger_/Base_/Uinitiated_/Execute.py
+RsCMPX_Base/Implementations/Trigger_/Base_/Uinitiated_/__init__.py
 RsCMPX_Base/Implementations/Write_/Eeprom.py
 RsCMPX_Base/Implementations/Write_/__init__.py
 RsCMPX_Base/Implementations/Write_/Eeprom_/Data.py
 RsCMPX_Base/Implementations/Write_/Eeprom_/__init__.py
 RsCMPX_Base/Internal/ArgLinkedEventArgs.py
 RsCMPX_Base/Internal/ArgSingle.py
 RsCMPX_Base/Internal/ArgSingleList.py
```

### Comparing `RsCMPX_Base-4.0.7.8/setup.py` & `RsCMPX_Base-4.0.7.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import pathlib
-from setuptools import setup, find_packages
-
-# The directory containing this file
-HERE = pathlib.Path(__file__).parent
-
-# The text of the README file
-README = (HERE / "README.md").read_text()
-
-# This call to setup() does all the work
-setup(
-    name="RsCMPX_Base",
-    version="4.0.7.8",
-    description="CMX/CMP Base System Remote-control Module",
-    long_description=README,
-    long_description_content_type="text/markdown",
-    author="Rohde & Schwarz GmbH & Co. KG",
-    copyright="Copyright © Rohde & Schwarz GmbH & Co. KG 2020",
-    author_email="Customer.Support@rohde-schwarz.com",
-    license="MIT",
-    classifiers=[
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.6",
-    ],
-    packages=(find_packages(include=['RsCMPX_Base', 'RsCMPX_Base.*'])),
-    install_requires=['PyVisa']
+import pathlib
+from setuptools import setup, find_packages
+
+# The directory containing this file
+HERE = pathlib.Path(__file__).parent
+
+# The text of the README file
+README = (HERE / "README.md").read_text()
+
+# This call to setup() does all the work
+setup(
+    name="RsCMPX_Base",
+    version="4.0.7.9",
+    description="CMX/CMP Base System Remote-control Module",
+    long_description=README,
+    long_description_content_type="text/markdown",
+    author="Rohde & Schwarz GmbH & Co. KG",
+    copyright="Copyright © Rohde & Schwarz GmbH & Co. KG 2021",
+    author_email="Customer.Support@rohde-schwarz.com",
+    license="MIT",
+    classifiers=[
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.6",
+    ],
+    packages=(find_packages(include=['RsCMPX_Base', 'RsCMPX_Base.*'])),
+    install_requires=['PyVisa']
 )
```

