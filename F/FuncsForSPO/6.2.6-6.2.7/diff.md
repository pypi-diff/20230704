# Comparing `tmp/FuncsForSPO-6.2.6.tar.gz` & `tmp/FuncsForSPO-6.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-6.2.6.tar", last modified: Fri Jun 30 12:27:56 2023, max compression
+gzip compressed data, was "FuncsForSPO-6.2.7.tar", last modified: Tue Jul  4 20:16:04 2023, max compression
```

## Comparing `FuncsForSPO-6.2.6.tar` & `FuncsForSPO-6.2.7.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:56.072571 FuncsForSPO-6.2.6/
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.632490 FuncsForSPO-6.2.6/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.690636 FuncsForSPO-6.2.6/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-6.2.6/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-6.2.6/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.702637 FuncsForSPO-6.2.6/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.6/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-6.2.6/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.711637 FuncsForSPO-6.2.6/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.6/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-6.2.6/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.732636 FuncsForSPO-6.2.6/FuncsForSPO/fgpt/
--rw-rw-rw-   0        0        0      886 2023-06-24 20:49:12.000000 FuncsForSPO-6.2.6/FuncsForSPO/fgpt/__fgpt.py
--rw-rw-rw-   0        0        0        0 2023-06-24 21:16:46.000000 FuncsForSPO-6.2.6/FuncsForSPO/fgpt/__init__.py
--rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.2.6/FuncsForSPO/fgpt/base.py
--rw-rw-rw-   0        0        0    14672 2023-06-26 14:09:10.000000 FuncsForSPO-6.2.6/FuncsForSPO/fgpt/fgpt.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.739637 FuncsForSPO-6.2.6/FuncsForSPO/flanguage/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.2.6/FuncsForSPO/flanguage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.756645 FuncsForSPO-6.2.6/FuncsForSPO/flanguage/translator/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.2.6/FuncsForSPO/flanguage/translator/__init__.py
--rw-rw-rw-   0        0        0     4400 2023-06-20 16:22:20.000000 FuncsForSPO-6.2.6/FuncsForSPO/flanguage/translator/__translator.py
--rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.2.6/FuncsForSPO/flanguage/translator/base.py
--rw-rw-rw-   0        0        0      829 2023-06-20 16:21:06.000000 FuncsForSPO-6.2.6/FuncsForSPO/flanguage/translator/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.768174 FuncsForSPO-6.2.6/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.6/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-6.2.6/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.774176 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.820820 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/
--rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/__init__.py
--rw-rw-rw-   0        0        0    11162 2023-06-28 17:53:11.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
--rw-rw-rw-   0        0        0     3579 2023-06-28 17:15:41.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/base.py
--rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
--rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
--rw-rw-rw-   0        0        0     1340 2023-06-28 13:21:40.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
--rw-rw-rw-   0        0        0      616 2023-06-29 19:53:08.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v4.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.836817 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.855823 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.860355 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.893360 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     8709 2023-06-18 14:37:35.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     1034 2023-06-18 14:17:07.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/focr/__ocr_online_v2.py
--rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/focr/base.py
--rw-rw-rw-   0        0        0     9951 2023-06-30 12:26:15.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.904444 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/pdfutils/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/pdfutils/__init__.py
--rw-rw-rw-   0        0        0     3357 2023-06-18 14:25:59.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/pdfutils/pdfutils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.918909 FuncsForSPO-6.2.6/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4696 2023-06-24 21:08:38.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.928908 FuncsForSPO-6.2.6/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    55610 2023-06-26 14:09:24.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.940913 FuncsForSPO-6.2.6/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.6/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10378 2023-06-24 21:07:45.000000 FuncsForSPO-6.2.6/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.950923 FuncsForSPO-6.2.6/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.6/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    39081 2023-06-26 14:06:50.000000 FuncsForSPO-6.2.6/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.963437 FuncsForSPO-6.2.6/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.6/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-6.2.6/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.973433 FuncsForSPO-6.2.6/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-6.2.6/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-6.2.6/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.978432 FuncsForSPO-6.2.6/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   122169 2023-06-24 20:59:57.000000 FuncsForSPO-6.2.6/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.678648 FuncsForSPO-6.2.6/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8023 2023-06-30 12:27:55.000000 FuncsForSPO-6.2.6/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2127 2023-06-30 12:27:55.000000 FuncsForSPO-6.2.6/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 12:27:55.000000 FuncsForSPO-6.2.6/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2023-06-30 12:27:55.000000 FuncsForSPO-6.2.6/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      475 2023-06-30 12:27:55.000000 FuncsForSPO-6.2.6/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-6.2.6/LICENSE
--rw-rw-rw-   0        0        0     8023 2023-06-30 12:27:56.069297 FuncsForSPO-6.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     7604 2023-06-20 16:05:40.000000 FuncsForSPO-6.2.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 12:27:56.073574 FuncsForSPO-6.2.6/setup.cfg
--rw-rw-rw-   0        0        0     2663 2023-06-30 12:27:44.000000 FuncsForSPO-6.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:04.019993 FuncsForSPO-6.2.7/
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.504599 FuncsForSPO-6.2.7/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.588350 FuncsForSPO-6.2.7/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-6.2.7/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-6.2.7/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.599235 FuncsForSPO-6.2.7/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.7/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-6.2.7/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.608266 FuncsForSPO-6.2.7/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.7/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-6.2.7/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.628019 FuncsForSPO-6.2.7/FuncsForSPO/fgpt/
+-rw-rw-rw-   0        0        0      886 2023-06-24 20:49:12.000000 FuncsForSPO-6.2.7/FuncsForSPO/fgpt/__fgpt.py
+-rw-rw-rw-   0        0        0        0 2023-06-24 21:16:46.000000 FuncsForSPO-6.2.7/FuncsForSPO/fgpt/__init__.py
+-rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.2.7/FuncsForSPO/fgpt/base.py
+-rw-rw-rw-   0        0        0    14672 2023-06-26 14:09:10.000000 FuncsForSPO-6.2.7/FuncsForSPO/fgpt/fgpt.py
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.634030 FuncsForSPO-6.2.7/FuncsForSPO/flanguage/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.2.7/FuncsForSPO/flanguage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.658398 FuncsForSPO-6.2.7/FuncsForSPO/flanguage/translator/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.2.7/FuncsForSPO/flanguage/translator/__init__.py
+-rw-rw-rw-   0        0        0     4400 2023-06-20 16:22:20.000000 FuncsForSPO-6.2.7/FuncsForSPO/flanguage/translator/__translator.py
+-rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.2.7/FuncsForSPO/flanguage/translator/base.py
+-rw-rw-rw-   0        0        0      829 2023-06-20 16:21:06.000000 FuncsForSPO-6.2.7/FuncsForSPO/flanguage/translator/translator.py
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.668397 FuncsForSPO-6.2.7/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.7/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-6.2.7/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.675579 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.720393 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/
+-rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/__init__.py
+-rw-rw-rw-   0        0        0    11162 2023-06-28 17:53:11.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
+-rw-rw-rw-   0        0        0     3579 2023-06-28 17:15:41.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/base.py
+-rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
+-rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
+-rw-rw-rw-   0        0        0     1340 2023-06-28 13:21:40.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
+-rw-rw-rw-   0        0        0      616 2023-06-29 19:53:08.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v4.py
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.738697 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.756227 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.760223 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.790744 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     8709 2023-06-18 14:37:35.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     1034 2023-06-18 14:17:07.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/focr/__ocr_online_v2.py
+-rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/focr/base.py
+-rw-rw-rw-   0        0        0     9951 2023-06-30 12:26:15.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.801751 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/pdfutils/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/pdfutils/__init__.py
+-rw-rw-rw-   0        0        0     3357 2023-06-18 14:25:59.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/pdfutils/pdfutils.py
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.812751 FuncsForSPO-6.2.7/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4696 2023-06-24 21:08:38.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.824274 FuncsForSPO-6.2.7/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    55610 2023-06-26 14:09:24.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.897161 FuncsForSPO-6.2.7/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.7/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10378 2023-06-24 21:07:45.000000 FuncsForSPO-6.2.7/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.917198 FuncsForSPO-6.2.7/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.7/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    38845 2023-07-04 20:15:36.000000 FuncsForSPO-6.2.7/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.933110 FuncsForSPO-6.2.7/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.7/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-6.2.7/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.943282 FuncsForSPO-6.2.7/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-6.2.7/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-6.2.7/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.951277 FuncsForSPO-6.2.7/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   122169 2023-06-24 20:59:57.000000 FuncsForSPO-6.2.7/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.577374 FuncsForSPO-6.2.7/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8023 2023-07-04 20:16:03.000000 FuncsForSPO-6.2.7/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2127 2023-07-04 20:16:03.000000 FuncsForSPO-6.2.7/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 20:16:03.000000 FuncsForSPO-6.2.7/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      220 2023-07-04 20:16:03.000000 FuncsForSPO-6.2.7/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      475 2023-07-04 20:16:03.000000 FuncsForSPO-6.2.7/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-6.2.7/LICENSE
+-rw-rw-rw-   0        0        0     8023 2023-07-04 20:16:04.014471 FuncsForSPO-6.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7604 2023-06-20 16:05:40.000000 FuncsForSPO-6.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-04 20:16:04.019993 FuncsForSPO-6.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     2663 2023-07-04 20:15:51.000000 FuncsForSPO-6.2.7/setup.py
```

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/femails/femails.py` & `FuncsForSPO-6.2.7/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fgpt/__fgpt.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fgpt/__fgpt.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fgpt/base.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fgpt/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fgpt/fgpt.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fgpt/fgpt.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/flanguage/translator/__translator.py` & `FuncsForSPO-6.2.7/FuncsForSPO/flanguage/translator/__translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/flanguage/translator/base.py` & `FuncsForSPO-6.2.7/FuncsForSPO/flanguage/translator/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/flanguage/translator/translator.py` & `FuncsForSPO-6.2.7/FuncsForSPO/flanguage/translator/translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/base.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v4.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v4.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/focr/__ocr_online_v2.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/focr/__ocr_online_v2.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/focr/base.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/focr/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/pdfutils/pdfutils.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/pdfutils/pdfutils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files 1% similar despite different names*

```diff
@@ -611,20 +611,19 @@
 
     Args:
         driver (Webdriver): Webdriver (Chrome, Firefox)
         wdw (WebDriverWait): WebDriver
         num_de_janelas (int): Quantidade de janelas esperadas para abrie. O padrão é 2.
     """
     driver = wdw._driver
-    print(f'Você está na janela -> {driver.current_window_handle}')
-    wdw.until(EC.number_of_windows_to_be(num_de_janelas))
-    print(f'Agora, você tem {len(driver.window_handles)} janelas abertas')
-    todas_as_windows = driver.window_handles
-    driver.switch_to.window(todas_as_windows[-1])
-    print(f'Agora, você está na janela -> {driver.current_window_handle}')
+    try:
+        wdw.until(EC.number_of_windows_to_be(num_de_janelas))
+        return True
+    except TimeoutException:
+        return False
     
     
 def procura_pela_janela_que_contenha_no_titulo(driver, title_contain_switch : str) -> None: # quero que pelo menos um pedaco do titulo que seja str
     """
     ### Essa função muda de janela quando o título tiver pelo menos algo igual ao parametro enviado
     #### Ex -> Minha janela = janela
```

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-6.2.7/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO/utils/utils.py` & `FuncsForSPO-6.2.7/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-6.2.7/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 6.2.6
+Version: 6.2.7
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-6.2.6/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-6.2.7/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/LICENSE` & `FuncsForSPO-6.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/PKG-INFO` & `FuncsForSPO-6.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 6.2.6
+Version: 6.2.7
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-6.2.6/README.md` & `FuncsForSPO-6.2.7/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.6/setup.py` & `FuncsForSPO-6.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '6.2.6'
+version = '6.2.7'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
```

