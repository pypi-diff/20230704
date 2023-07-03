# Comparing `tmp/PointBlaster-0.2.2.tar.gz` & `tmp/PointBlaster-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PointBlaster-0.2.2.tar", last modified: Sat Jul  1 09:53:04 2023, max compression
+gzip compressed data, was "PointBlaster-0.2.3.tar", last modified: Mon Jul  3 22:03:48 2023, max compression
```

## Comparing `PointBlaster-0.2.2.tar` & `PointBlaster-0.2.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-01 09:53:04.727627 PointBlaster-0.2.2/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-07-01 09:04:52.000000 PointBlaster-0.2.2/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       61 2023-06-25 06:30:58.000000 PointBlaster-0.2.2/MANIFEST.in
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-07-01 09:53:04.727498 PointBlaster-0.2.2/PKG-INFO
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-01 09:53:04.706672 PointBlaster-0.2.2/PointBlaster/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-26 05:00:54.000000 PointBlaster-0.2.2/PointBlaster/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    26523 2023-07-01 09:51:37.000000 PointBlaster-0.2.2/PointBlaster/PointBlaster.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      303 2023-07-01 09:05:12.000000 PointBlaster-0.2.2/PointBlaster/__init__.py
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-01 09:53:04.707479 PointBlaster-0.2.2/PointBlaster/db/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-26 05:00:54.000000 PointBlaster-0.2.2/PointBlaster/db/.DS_Store
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-01 09:53:04.707796 PointBlaster-0.2.2/PointBlaster/db/point_mutation/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    10244 2023-06-26 05:03:42.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/.DS_Store
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-01 09:53:04.715642 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:10:09.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2972 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/23S.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        4 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/RNA_genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)  4259822 2023-06-19 06:54:12.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     8705 2023-06-25 07:08:32.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     8657 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:54:12.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.length.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      149 2023-06-19 06:54:12.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.name
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4936 2023-06-19 06:54:12.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       14 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     5272 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2613 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2523 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1961 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      412 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/rpsL.fsa
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-01 09:53:04.723445 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1593 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/RNA_genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     3214 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/acrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2694 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/gyrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2469 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/gyrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2311 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/parC.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1940 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/parE.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     7137 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/phenotypes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      698 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/pmrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1106 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/pmrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     5026 2023-06-25 07:13:32.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)  4318510 2023-06-19 06:54:12.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    16121 2023-06-25 07:08:53.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/salmonella.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    16025 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       72 2023-06-19 06:54:12.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/salmonella.length.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      296 2023-06-19 06:54:12.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/salmonella.name
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     7888 2023-06-19 06:54:12.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-01 09:53:04.707369 PointBlaster-0.2.2/PointBlaster.egg-info/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-07-01 09:53:04.000000 PointBlaster-0.2.2/PointBlaster.egg-info/PKG-INFO
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2350 2023-07-01 09:53:04.000000 PointBlaster-0.2.2/PointBlaster.egg-info/SOURCES.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2023-07-01 09:53:04.000000 PointBlaster-0.2.2/PointBlaster.egg-info/dependency_links.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       65 2023-07-01 09:53:04.000000 PointBlaster-0.2.2/PointBlaster.egg-info/entry_points.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       39 2023-07-01 09:53:04.000000 PointBlaster-0.2.2/PointBlaster.egg-info/requires.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       13 2023-07-01 09:53:04.000000 PointBlaster-0.2.2/PointBlaster.egg-info/top_level.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1611 2023-06-25 06:11:36.000000 PointBlaster-0.2.2/README.md
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-01 09:53:04.725839 PointBlaster-0.2.2/dist/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-27 05:40:56.000000 PointBlaster-0.2.2/dist/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       57 2023-06-25 05:58:37.000000 PointBlaster-0.2.2/requirements.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2023-07-01 09:53:04.727667 PointBlaster-0.2.2/setup.cfg
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2162 2023-06-25 06:43:25.000000 PointBlaster-0.2.2/setup.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-03 22:03:48.884729 PointBlaster-0.2.3/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-07-01 09:04:52.000000 PointBlaster-0.2.3/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       61 2023-06-25 06:30:58.000000 PointBlaster-0.2.3/MANIFEST.in
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-07-03 22:03:48.884579 PointBlaster-0.2.3/PKG-INFO
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-03 22:03:48.862288 PointBlaster-0.2.3/PointBlaster/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-26 05:00:54.000000 PointBlaster-0.2.3/PointBlaster/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    26883 2023-07-03 22:03:19.000000 PointBlaster-0.2.3/PointBlaster/PointBlaster.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      303 2023-07-03 22:03:05.000000 PointBlaster-0.2.3/PointBlaster/__init__.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-03 22:03:48.863092 PointBlaster-0.2.3/PointBlaster/db/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-26 05:00:54.000000 PointBlaster-0.2.3/PointBlaster/db/.DS_Store
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-03 22:03:48.863382 PointBlaster-0.2.3/PointBlaster/db/point_mutation/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    10244 2023-06-26 05:03:42.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/.DS_Store
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-03 22:03:48.872604 PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:10:09.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2972 2023-06-19 06:40:55.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/23S.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        4 2023-06-19 06:40:55.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/RNA_genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)  4259822 2023-06-19 06:54:12.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     8705 2023-06-25 07:08:32.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     8657 2023-06-19 06:40:55.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:54:12.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/campylobacter.length.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      149 2023-06-19 06:54:12.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/campylobacter.name
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4936 2023-06-19 06:54:12.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       14 2023-06-19 06:40:55.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     5272 2023-06-19 06:40:55.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2613 2023-06-19 06:40:55.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2523 2023-06-19 06:40:55.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1961 2023-06-19 06:40:55.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      412 2023-06-19 06:40:55.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/rpsL.fsa
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-03 22:03:48.881458 PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1593 2023-06-19 06:40:55.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2023-06-19 06:40:55.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/RNA_genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     3214 2023-06-19 06:40:55.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/acrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:40:55.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2694 2023-06-19 06:40:55.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/gyrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2469 2023-06-19 06:40:55.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/gyrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2311 2023-06-19 06:40:55.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/parC.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1940 2023-06-19 06:40:55.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/parE.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     7137 2023-06-19 06:40:55.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/phenotypes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      698 2023-06-19 06:40:55.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/pmrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1106 2023-06-19 06:40:55.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/pmrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     5026 2023-06-25 07:13:32.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)  4318510 2023-06-19 06:54:12.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    16121 2023-06-25 07:08:53.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/salmonella.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    16025 2023-06-19 06:40:55.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       72 2023-06-19 06:54:12.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/salmonella.length.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      296 2023-06-19 06:54:12.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/salmonella.name
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     7888 2023-06-19 06:54:12.000000 PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-03 22:03:48.862991 PointBlaster-0.2.3/PointBlaster.egg-info/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-07-03 22:03:48.000000 PointBlaster-0.2.3/PointBlaster.egg-info/PKG-INFO
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2350 2023-07-03 22:03:48.000000 PointBlaster-0.2.3/PointBlaster.egg-info/SOURCES.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2023-07-03 22:03:48.000000 PointBlaster-0.2.3/PointBlaster.egg-info/dependency_links.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       65 2023-07-03 22:03:48.000000 PointBlaster-0.2.3/PointBlaster.egg-info/entry_points.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       39 2023-07-03 22:03:48.000000 PointBlaster-0.2.3/PointBlaster.egg-info/requires.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       13 2023-07-03 22:03:48.000000 PointBlaster-0.2.3/PointBlaster.egg-info/top_level.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1611 2023-06-25 06:11:36.000000 PointBlaster-0.2.3/README.md
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-03 22:03:48.882758 PointBlaster-0.2.3/dist/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-27 05:40:56.000000 PointBlaster-0.2.3/dist/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       57 2023-06-25 05:58:37.000000 PointBlaster-0.2.3/requirements.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2023-07-03 22:03:48.884781 PointBlaster-0.2.3/setup.cfg
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2162 2023-06-25 06:43:25.000000 PointBlaster-0.2.3/setup.py
```

### Comparing `PointBlaster-0.2.2/.DS_Store` & `PointBlaster-0.2.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PKG-INFO` & `PointBlaster-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PointBlaster
-Version: 0.2.2
+Version: 0.2.3
 Summary: find point mutation in assembled genomes
 Home-page: https://github.com/hbucqp/PointBlaster
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,wgs,blastn,pointmutation
 Platform: any
```

### Comparing `PointBlaster-0.2.2/PointBlaster/.DS_Store` & `PointBlaster-0.2.3/PointBlaster/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/PointBlaster.py` & `PointBlaster-0.2.3/PointBlaster/PointBlaster.py`

 * *Files 2% similar despite different names*

```diff
@@ -590,16 +590,18 @@
 
 
 def main():
     # df_all = pd.DataFrame()
     args = args_parse()
     if args.list:
         show_db_list()
+        sys.exit(1)
     elif args.init:
         initialize_db()
+        sys.exit(1)
     else:
         # threads
         threads = args.t
         # print(threads)
 
         minid = args.minid
         mincov = args.mincov
@@ -618,21 +620,28 @@
         # check if the output directory exists
         if not os.path.exists(args.o):
             os.mkdir(args.o)
 
         output_path = os.path.abspath(args.o)
 
         # check if -species var exist
+        species_list = ['salmoenlla', 'campylobacter']
         if args.s is not None:
-            blastdb = os.path.join(os.path.dirname(
-                __file__), f'db/point_mutation/{args.s}/{args.s}')
-            db_mutations_path = os.path.join(os.path.dirname(
-                __file__), f'db/point_mutation/{args.s}/resistens-overview.txt')
-            ref_fasta = os.path.join(os.path.dirname(
-                __file__), f'db/point_mutation/{args.s}/{args.s}.fsa')
+            if args.s in species_list:
+                blastdb = os.path.join(os.path.dirname(
+                    __file__), f'db/point_mutation/{args.s}/{args.s}')
+                db_mutations_path = os.path.join(os.path.dirname(
+                    __file__), f'db/point_mutation/{args.s}/resistens-overview.txt')
+                ref_fasta = os.path.join(os.path.dirname(
+                    __file__), f'db/point_mutation/{args.s}/{args.s}.fsa')
+            else:
+                print(
+                    "Please input the right species in species_list, the supported species are")
+                print(species_list)
+                sys.exit(1)
         else:
             sys.exit(1)
         df_final = pd.DataFrame()
 
         for file in files:
             file_base = str(os.path.basename(os.path.splitext(file)[0]))
             output_filename = file_base + '_tab.txt'
```

### Comparing `PointBlaster-0.2.2/PointBlaster/db/.DS_Store` & `PointBlaster-0.2.3/PointBlaster/db/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/.DS_Store` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/.DS_Store` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/23S.fsa` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/23S.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/acrB.fsa` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/acrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/gyrA.fsa` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/gyrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/gyrB.fsa` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/gyrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/parC.fsa` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/parC.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/parE.fsa` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/parE.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/phenotypes.txt` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/phenotypes.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/pmrA.fsa` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/pmrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/pmrB.fsa` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/pmrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/salmonella.fsa` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/salmonella.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b` & `PointBlaster-0.2.3/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/PointBlaster.egg-info/PKG-INFO` & `PointBlaster-0.2.3/PointBlaster.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PointBlaster
-Version: 0.2.2
+Version: 0.2.3
 Summary: find point mutation in assembled genomes
 Home-page: https://github.com/hbucqp/PointBlaster
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,wgs,blastn,pointmutation
 Platform: any
```

### Comparing `PointBlaster-0.2.2/PointBlaster.egg-info/SOURCES.txt` & `PointBlaster-0.2.3/PointBlaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/README.md` & `PointBlaster-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/dist/.DS_Store` & `PointBlaster-0.2.3/dist/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.2/setup.py` & `PointBlaster-0.2.3/setup.py`

 * *Files identical despite different names*

