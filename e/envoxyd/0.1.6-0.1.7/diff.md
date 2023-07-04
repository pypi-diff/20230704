# Comparing `tmp/envoxyd-0.1.6.tar.gz` & `tmp/envoxyd-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/envoxyd-0.1.6.tar", last modified: Thu Jun 29 19:40:06 2023, max compression
+gzip compressed data, was "dist/envoxyd-0.1.7.tar", last modified: Tue Jul  4 19:25:06 2023, max compression
```

## Comparing `envoxyd-0.1.6.tar` & `envoxyd-0.1.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:06.000000 envoxyd-0.1.6/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:06.000000 envoxyd-0.1.6/envoxyd.egg-info/
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-29 19:40:06.000000 envoxyd-0.1.6/envoxyd.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 19:40:06.000000 envoxyd-0.1.6/envoxyd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-06-29 19:40:06.000000 envoxyd-0.1.6/envoxyd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      371 2023-06-29 19:40:06.000000 envoxyd-0.1.6/envoxyd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      263 2023-06-29 19:40:06.000000 envoxyd-0.1.6/envoxyd.egg-info/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:06.000000 envoxyd-0.1.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:06.000000 envoxyd-0.1.6/src/envoxyd/
--rwxr-xr-x   0 root         (0) root         (0)  1528912 2023-06-29 19:40:03.000000 envoxyd-0.1.6/src/envoxyd/envoxyd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:06.000000 envoxyd-0.1.6/envoxyd/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:06.000000 envoxyd-0.1.6/envoxyd/tools/
--rwxr-xr-x   0 root         (0) root         (0)     2983 2020-01-30 17:54:32.000000 envoxyd-0.1.6/envoxyd/tools/envoxy-cli
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxyd-0.1.6/envoxyd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:06.000000 envoxyd-0.1.6/envoxyd/templates/
--rw-r--r--   0 root         (0) root         (0)     2069 2020-01-30 17:54:32.000000 envoxyd-0.1.6/envoxyd/templates/view.py
--rw-r--r--   0 root         (0) root         (0)      148 2020-01-30 17:54:32.000000 envoxyd-0.1.6/envoxyd/templates/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:06.000000 envoxyd-0.1.6/envoxyd/templates/confs/
--rw-r--r--   0 root         (0) root         (0)     1582 2020-01-30 17:54:32.000000 envoxyd-0.1.6/envoxyd/templates/confs/envoxy.json
--rw-r--r--   0 root         (0) root         (0)       28 2020-01-30 17:54:32.000000 envoxyd-0.1.6/envoxyd/templates/run.py
--rw-rw-r--   0 root         (0) root         (0)     9687 2022-11-17 10:40:18.000000 envoxyd-0.1.6/envoxyd/run.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 19:40:06.000000 envoxyd-0.1.6/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1461 2023-06-29 19:36:41.000000 envoxyd-0.1.6/setup.py
--rw-r--r--   0 root         (0) root         (0)      263 2023-06-29 19:40:06.000000 envoxyd-0.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1064 2020-01-30 17:54:32.000000 envoxyd-0.1.6/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxyd-0.1.7/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxyd-0.1.7/envoxyd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-04 19:25:06.000000 envoxyd-0.1.7/envoxyd.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 19:25:06.000000 envoxyd-0.1.7/envoxyd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-04 19:25:06.000000 envoxyd-0.1.7/envoxyd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      371 2023-07-04 19:25:06.000000 envoxyd-0.1.7/envoxyd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      263 2023-07-04 19:25:06.000000 envoxyd-0.1.7/envoxyd.egg-info/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxyd-0.1.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxyd-0.1.7/src/envoxyd/
+-rwxr-xr-x   0 root         (0) root         (0)  1528912 2023-07-04 19:25:05.000000 envoxyd-0.1.7/src/envoxyd/envoxyd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxyd-0.1.7/envoxyd/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxyd-0.1.7/envoxyd/tools/
+-rwxr-xr-x   0 root         (0) root         (0)     2983 2020-01-30 17:54:32.000000 envoxyd-0.1.7/envoxyd/tools/envoxy-cli
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxyd-0.1.7/envoxyd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxyd-0.1.7/envoxyd/templates/
+-rw-r--r--   0 root         (0) root         (0)     2069 2020-01-30 17:54:32.000000 envoxyd-0.1.7/envoxyd/templates/view.py
+-rw-r--r--   0 root         (0) root         (0)      148 2020-01-30 17:54:32.000000 envoxyd-0.1.7/envoxyd/templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxyd-0.1.7/envoxyd/templates/confs/
+-rw-r--r--   0 root         (0) root         (0)     1582 2020-01-30 17:54:32.000000 envoxyd-0.1.7/envoxyd/templates/confs/envoxy.json
+-rw-r--r--   0 root         (0) root         (0)       28 2020-01-30 17:54:32.000000 envoxyd-0.1.7/envoxyd/templates/run.py
+-rw-rw-r--   0 root         (0) root         (0)     9687 2022-11-17 10:40:18.000000 envoxyd-0.1.7/envoxyd/run.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 19:25:06.000000 envoxyd-0.1.7/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1461 2023-07-04 19:22:00.000000 envoxyd-0.1.7/setup.py
+-rw-r--r--   0 root         (0) root         (0)      263 2023-07-04 19:25:06.000000 envoxyd-0.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1064 2020-01-30 17:54:32.000000 envoxyd-0.1.7/LICENSE.txt
```

### Comparing `envoxyd-0.1.6/src/envoxyd/envoxyd` & `envoxyd-0.1.7/src/envoxyd/envoxyd`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --relocs {}

```diff
@@ -87,182 +87,182 @@
 0000000000341b68  0000000000000008 R_X86_64_RELATIVE                         aea35
 0000000000341b70  0000000000000008 R_X86_64_RELATIVE                         125d25
 0000000000341b78  0000000000000008 R_X86_64_RELATIVE                         aea38
 0000000000341b80  0000000000000008 R_X86_64_RELATIVE                         aea3b
 0000000000341b88  0000000000000008 R_X86_64_RELATIVE                         afcf0
 0000000000341b90  0000000000000008 R_X86_64_RELATIVE                         aea3e
 0000000000341b98  0000000000000008 R_X86_64_RELATIVE                         aea41
-0000000000341ba0  0000000000000008 R_X86_64_RELATIVE                         b9ca7
-0000000000341ba8  0000000000000008 R_X86_64_RELATIVE                         aea44
-0000000000341bb0  0000000000000008 R_X86_64_RELATIVE                         aea47
-0000000000341bb8  0000000000000008 R_X86_64_RELATIVE                         aea4a
-0000000000341bc0  0000000000000008 R_X86_64_RELATIVE                         aea4d
-0000000000341bc8  0000000000000008 R_X86_64_RELATIVE                         aea50
-0000000000341bd0  0000000000000008 R_X86_64_RELATIVE                         aea53
-0000000000341bd8  0000000000000008 R_X86_64_RELATIVE                         aea56
-0000000000341be0  0000000000000008 R_X86_64_RELATIVE                         aea59
-0000000000341be8  0000000000000008 R_X86_64_RELATIVE                         aea5c
-0000000000341bf0  0000000000000008 R_X86_64_RELATIVE                         aea5f
-0000000000341bf8  0000000000000008 R_X86_64_RELATIVE                         aea62
+0000000000341ba0  0000000000000008 R_X86_64_RELATIVE                         aea44
+0000000000341ba8  0000000000000008 R_X86_64_RELATIVE                         aea47
+0000000000341bb0  0000000000000008 R_X86_64_RELATIVE                         aea4a
+0000000000341bb8  0000000000000008 R_X86_64_RELATIVE                         aea4d
+0000000000341bc0  0000000000000008 R_X86_64_RELATIVE                         aea50
+0000000000341bc8  0000000000000008 R_X86_64_RELATIVE                         aea53
+0000000000341bd0  0000000000000008 R_X86_64_RELATIVE                         aea56
+0000000000341bd8  0000000000000008 R_X86_64_RELATIVE                         aea59
+0000000000341be0  0000000000000008 R_X86_64_RELATIVE                         aea5c
+0000000000341be8  0000000000000008 R_X86_64_RELATIVE                         aea5f
+0000000000341bf0  0000000000000008 R_X86_64_RELATIVE                         aea62
+0000000000341bf8  0000000000000008 R_X86_64_RELATIVE                         aea65
 0000000000341c00  0000000000000008 R_X86_64_RELATIVE                         124a94
-0000000000341c08  0000000000000008 R_X86_64_RELATIVE                         aea65
-0000000000341c10  0000000000000008 R_X86_64_RELATIVE                         aea68
-0000000000341c18  0000000000000008 R_X86_64_RELATIVE                         aea6b
+0000000000341c08  0000000000000008 R_X86_64_RELATIVE                         aea68
+0000000000341c10  0000000000000008 R_X86_64_RELATIVE                         aea6b
+0000000000341c18  0000000000000008 R_X86_64_RELATIVE                         aea6e
 0000000000341c20  0000000000000008 R_X86_64_RELATIVE                         125cf6
-0000000000341c28  0000000000000008 R_X86_64_RELATIVE                         aea6e
-0000000000341c30  0000000000000008 R_X86_64_RELATIVE                         aea71
-0000000000341c38  0000000000000008 R_X86_64_RELATIVE                         aea74
-0000000000341c40  0000000000000008 R_X86_64_RELATIVE                         aea77
-0000000000341c48  0000000000000008 R_X86_64_RELATIVE                         aea7a
-0000000000341c50  0000000000000008 R_X86_64_RELATIVE                         aea7d
-0000000000341c58  0000000000000008 R_X86_64_RELATIVE                         aea80
-0000000000341c60  0000000000000008 R_X86_64_RELATIVE                         aea83
-0000000000341c68  0000000000000008 R_X86_64_RELATIVE                         aea86
-0000000000341c70  0000000000000008 R_X86_64_RELATIVE                         aea89
-0000000000341c78  0000000000000008 R_X86_64_RELATIVE                         aea8c
-0000000000341c80  0000000000000008 R_X86_64_RELATIVE                         aea8f
-0000000000341c88  0000000000000008 R_X86_64_RELATIVE                         aea92
-0000000000341c90  0000000000000008 R_X86_64_RELATIVE                         aea95
-0000000000341c98  0000000000000008 R_X86_64_RELATIVE                         aea98
-0000000000341ca0  0000000000000008 R_X86_64_RELATIVE                         aea9b
+0000000000341c28  0000000000000008 R_X86_64_RELATIVE                         aea71
+0000000000341c30  0000000000000008 R_X86_64_RELATIVE                         aea74
+0000000000341c38  0000000000000008 R_X86_64_RELATIVE                         aea77
+0000000000341c40  0000000000000008 R_X86_64_RELATIVE                         aea7a
+0000000000341c48  0000000000000008 R_X86_64_RELATIVE                         aea7d
+0000000000341c50  0000000000000008 R_X86_64_RELATIVE                         aea80
+0000000000341c58  0000000000000008 R_X86_64_RELATIVE                         aea83
+0000000000341c60  0000000000000008 R_X86_64_RELATIVE                         aea86
+0000000000341c68  0000000000000008 R_X86_64_RELATIVE                         aea89
+0000000000341c70  0000000000000008 R_X86_64_RELATIVE                         aea8c
+0000000000341c78  0000000000000008 R_X86_64_RELATIVE                         aea8f
+0000000000341c80  0000000000000008 R_X86_64_RELATIVE                         aea92
+0000000000341c88  0000000000000008 R_X86_64_RELATIVE                         aea95
+0000000000341c90  0000000000000008 R_X86_64_RELATIVE                         aea98
+0000000000341c98  0000000000000008 R_X86_64_RELATIVE                         aea9b
+0000000000341ca0  0000000000000008 R_X86_64_RELATIVE                         aea9e
 0000000000341ca8  0000000000000008 R_X86_64_RELATIVE                         1285c0
-0000000000341cb0  0000000000000008 R_X86_64_RELATIVE                         aea9e
-0000000000341cb8  0000000000000008 R_X86_64_RELATIVE                         aeaa1
-0000000000341cc0  0000000000000008 R_X86_64_RELATIVE                         aeaa4
-0000000000341cc8  0000000000000008 R_X86_64_RELATIVE                         aeaa7
-0000000000341cd0  0000000000000008 R_X86_64_RELATIVE                         aeaaa
-0000000000341cd8  0000000000000008 R_X86_64_RELATIVE                         aeaad
+0000000000341cb0  0000000000000008 R_X86_64_RELATIVE                         aeaa1
+0000000000341cb8  0000000000000008 R_X86_64_RELATIVE                         aeaa4
+0000000000341cc0  0000000000000008 R_X86_64_RELATIVE                         aeaa7
+0000000000341cc8  0000000000000008 R_X86_64_RELATIVE                         aeaaa
+0000000000341cd0  0000000000000008 R_X86_64_RELATIVE                         aeaad
+0000000000341cd8  0000000000000008 R_X86_64_RELATIVE                         aeab0
 0000000000341ce0  0000000000000008 R_X86_64_RELATIVE                         b3ef3
-0000000000341ce8  0000000000000008 R_X86_64_RELATIVE                         aeab0
-0000000000341cf0  0000000000000008 R_X86_64_RELATIVE                         aeab3
-0000000000341cf8  0000000000000008 R_X86_64_RELATIVE                         aeab6
-0000000000341d00  0000000000000008 R_X86_64_RELATIVE                         aeab9
-0000000000341d08  0000000000000008 R_X86_64_RELATIVE                         aeabc
-0000000000341d10  0000000000000008 R_X86_64_RELATIVE                         aeabf
-0000000000341d18  0000000000000008 R_X86_64_RELATIVE                         aeac2
+0000000000341ce8  0000000000000008 R_X86_64_RELATIVE                         aeab3
+0000000000341cf0  0000000000000008 R_X86_64_RELATIVE                         aeab6
+0000000000341cf8  0000000000000008 R_X86_64_RELATIVE                         aeab9
+0000000000341d00  0000000000000008 R_X86_64_RELATIVE                         aeabc
+0000000000341d08  0000000000000008 R_X86_64_RELATIVE                         aeabf
+0000000000341d10  0000000000000008 R_X86_64_RELATIVE                         aeac2
+0000000000341d18  0000000000000008 R_X86_64_RELATIVE                         aeac5
 0000000000341d20  0000000000000008 R_X86_64_RELATIVE                         125cdf
-0000000000341d28  0000000000000008 R_X86_64_RELATIVE                         aeac5
-0000000000341d30  0000000000000008 R_X86_64_RELATIVE                         aeac8
-0000000000341d38  0000000000000008 R_X86_64_RELATIVE                         aeacb
-0000000000341d40  0000000000000008 R_X86_64_RELATIVE                         aeace
-0000000000341d48  0000000000000008 R_X86_64_RELATIVE                         aead1
-0000000000341d50  0000000000000008 R_X86_64_RELATIVE                         aead4
-0000000000341d58  0000000000000008 R_X86_64_RELATIVE                         aead7
-0000000000341d60  0000000000000008 R_X86_64_RELATIVE                         aeada
-0000000000341d68  0000000000000008 R_X86_64_RELATIVE                         aeadd
-0000000000341d70  0000000000000008 R_X86_64_RELATIVE                         aeae0
-0000000000341d78  0000000000000008 R_X86_64_RELATIVE                         aeae3
-0000000000341d80  0000000000000008 R_X86_64_RELATIVE                         aeae6
-0000000000341d88  0000000000000008 R_X86_64_RELATIVE                         aeae9
-0000000000341d90  0000000000000008 R_X86_64_RELATIVE                         aeaec
-0000000000341d98  0000000000000008 R_X86_64_RELATIVE                         aeaef
-0000000000341da0  0000000000000008 R_X86_64_RELATIVE                         aeaf2
-0000000000341da8  0000000000000008 R_X86_64_RELATIVE                         aeaf5
-0000000000341db0  0000000000000008 R_X86_64_RELATIVE                         aeaf8
-0000000000341db8  0000000000000008 R_X86_64_RELATIVE                         aeafb
-0000000000341dc0  0000000000000008 R_X86_64_RELATIVE                         aeafe
-0000000000341dc8  0000000000000008 R_X86_64_RELATIVE                         aeb01
-0000000000341dd0  0000000000000008 R_X86_64_RELATIVE                         aeb04
-0000000000341dd8  0000000000000008 R_X86_64_RELATIVE                         aeb07
-0000000000341de0  0000000000000008 R_X86_64_RELATIVE                         aeb0a
-0000000000341de8  0000000000000008 R_X86_64_RELATIVE                         aeb0d
-0000000000341df0  0000000000000008 R_X86_64_RELATIVE                         aeb10
-0000000000341df8  0000000000000008 R_X86_64_RELATIVE                         aeb13
-0000000000341e00  0000000000000008 R_X86_64_RELATIVE                         aeb16
-0000000000341e08  0000000000000008 R_X86_64_RELATIVE                         aeb19
-0000000000341e10  0000000000000008 R_X86_64_RELATIVE                         aeb1c
-0000000000341e18  0000000000000008 R_X86_64_RELATIVE                         aeb1f
-0000000000341e20  0000000000000008 R_X86_64_RELATIVE                         aeb22
-0000000000341e28  0000000000000008 R_X86_64_RELATIVE                         aeb25
-0000000000341e30  0000000000000008 R_X86_64_RELATIVE                         aeb28
-0000000000341e38  0000000000000008 R_X86_64_RELATIVE                         aeb2b
-0000000000341e40  0000000000000008 R_X86_64_RELATIVE                         aeb2e
+0000000000341d28  0000000000000008 R_X86_64_RELATIVE                         aeac8
+0000000000341d30  0000000000000008 R_X86_64_RELATIVE                         aeacb
+0000000000341d38  0000000000000008 R_X86_64_RELATIVE                         aeace
+0000000000341d40  0000000000000008 R_X86_64_RELATIVE                         aead1
+0000000000341d48  0000000000000008 R_X86_64_RELATIVE                         aead4
+0000000000341d50  0000000000000008 R_X86_64_RELATIVE                         aead7
+0000000000341d58  0000000000000008 R_X86_64_RELATIVE                         aeada
+0000000000341d60  0000000000000008 R_X86_64_RELATIVE                         aeadd
+0000000000341d68  0000000000000008 R_X86_64_RELATIVE                         aeae0
+0000000000341d70  0000000000000008 R_X86_64_RELATIVE                         aeae3
+0000000000341d78  0000000000000008 R_X86_64_RELATIVE                         aeae6
+0000000000341d80  0000000000000008 R_X86_64_RELATIVE                         aeae9
+0000000000341d88  0000000000000008 R_X86_64_RELATIVE                         aeaec
+0000000000341d90  0000000000000008 R_X86_64_RELATIVE                         aeaef
+0000000000341d98  0000000000000008 R_X86_64_RELATIVE                         aeaf2
+0000000000341da0  0000000000000008 R_X86_64_RELATIVE                         aeaf5
+0000000000341da8  0000000000000008 R_X86_64_RELATIVE                         aeaf8
+0000000000341db0  0000000000000008 R_X86_64_RELATIVE                         aeafb
+0000000000341db8  0000000000000008 R_X86_64_RELATIVE                         aeafe
+0000000000341dc0  0000000000000008 R_X86_64_RELATIVE                         aeb01
+0000000000341dc8  0000000000000008 R_X86_64_RELATIVE                         aeb04
+0000000000341dd0  0000000000000008 R_X86_64_RELATIVE                         aeb07
+0000000000341dd8  0000000000000008 R_X86_64_RELATIVE                         aeb0a
+0000000000341de0  0000000000000008 R_X86_64_RELATIVE                         aeb0d
+0000000000341de8  0000000000000008 R_X86_64_RELATIVE                         aeb10
+0000000000341df0  0000000000000008 R_X86_64_RELATIVE                         aeb13
+0000000000341df8  0000000000000008 R_X86_64_RELATIVE                         aeb16
+0000000000341e00  0000000000000008 R_X86_64_RELATIVE                         aeb19
+0000000000341e08  0000000000000008 R_X86_64_RELATIVE                         aeb1c
+0000000000341e10  0000000000000008 R_X86_64_RELATIVE                         aeb1f
+0000000000341e18  0000000000000008 R_X86_64_RELATIVE                         aeb22
+0000000000341e20  0000000000000008 R_X86_64_RELATIVE                         aeb25
+0000000000341e28  0000000000000008 R_X86_64_RELATIVE                         aeb28
+0000000000341e30  0000000000000008 R_X86_64_RELATIVE                         aeb2b
+0000000000341e38  0000000000000008 R_X86_64_RELATIVE                         aeb2e
+0000000000341e40  0000000000000008 R_X86_64_RELATIVE                         aeb31
 0000000000341e48  0000000000000008 R_X86_64_RELATIVE                         b444c
-0000000000341e50  0000000000000008 R_X86_64_RELATIVE                         aeb31
-0000000000341e58  0000000000000008 R_X86_64_RELATIVE                         aeb34
-0000000000341e60  0000000000000008 R_X86_64_RELATIVE                         aeb37
-0000000000341e68  0000000000000008 R_X86_64_RELATIVE                         aeb3a
-0000000000341e70  0000000000000008 R_X86_64_RELATIVE                         aeb3d
-0000000000341e78  0000000000000008 R_X86_64_RELATIVE                         aeb40
-0000000000341e80  0000000000000008 R_X86_64_RELATIVE                         aeb43
-0000000000341e88  0000000000000008 R_X86_64_RELATIVE                         aeb46
-0000000000341e90  0000000000000008 R_X86_64_RELATIVE                         aeb49
-0000000000341e98  0000000000000008 R_X86_64_RELATIVE                         aeb4c
-0000000000341ea0  0000000000000008 R_X86_64_RELATIVE                         aeb4f
-0000000000341ea8  0000000000000008 R_X86_64_RELATIVE                         aeb52
-0000000000341eb0  0000000000000008 R_X86_64_RELATIVE                         aeb55
-0000000000341eb8  0000000000000008 R_X86_64_RELATIVE                         aeb58
-0000000000341ec0  0000000000000008 R_X86_64_RELATIVE                         aeb5b
-0000000000341ec8  0000000000000008 R_X86_64_RELATIVE                         aeb5e
-0000000000341ed0  0000000000000008 R_X86_64_RELATIVE                         aeb61
-0000000000341ed8  0000000000000008 R_X86_64_RELATIVE                         aeb64
-0000000000341ee0  0000000000000008 R_X86_64_RELATIVE                         aeb67
-0000000000341ee8  0000000000000008 R_X86_64_RELATIVE                         aeb6a
-0000000000341ef0  0000000000000008 R_X86_64_RELATIVE                         aeb6d
-0000000000341ef8  0000000000000008 R_X86_64_RELATIVE                         aeb70
-0000000000341f00  0000000000000008 R_X86_64_RELATIVE                         aeb73
-0000000000341f08  0000000000000008 R_X86_64_RELATIVE                         aeb76
-0000000000341f10  0000000000000008 R_X86_64_RELATIVE                         aeb79
-0000000000341f18  0000000000000008 R_X86_64_RELATIVE                         aeb7c
-0000000000341f20  0000000000000008 R_X86_64_RELATIVE                         aeb7f
-0000000000341f28  0000000000000008 R_X86_64_RELATIVE                         aeb82
-0000000000341f30  0000000000000008 R_X86_64_RELATIVE                         aeb85
-0000000000341f38  0000000000000008 R_X86_64_RELATIVE                         aeb88
-0000000000341f40  0000000000000008 R_X86_64_RELATIVE                         aeb8b
-0000000000341f48  0000000000000008 R_X86_64_RELATIVE                         aeb8e
+0000000000341e50  0000000000000008 R_X86_64_RELATIVE                         aeb34
+0000000000341e58  0000000000000008 R_X86_64_RELATIVE                         aeb37
+0000000000341e60  0000000000000008 R_X86_64_RELATIVE                         aeb3a
+0000000000341e68  0000000000000008 R_X86_64_RELATIVE                         aeb3d
+0000000000341e70  0000000000000008 R_X86_64_RELATIVE                         aeb40
+0000000000341e78  0000000000000008 R_X86_64_RELATIVE                         aeb43
+0000000000341e80  0000000000000008 R_X86_64_RELATIVE                         aeb46
+0000000000341e88  0000000000000008 R_X86_64_RELATIVE                         aeb49
+0000000000341e90  0000000000000008 R_X86_64_RELATIVE                         aeb4c
+0000000000341e98  0000000000000008 R_X86_64_RELATIVE                         aeb4f
+0000000000341ea0  0000000000000008 R_X86_64_RELATIVE                         aeb52
+0000000000341ea8  0000000000000008 R_X86_64_RELATIVE                         aeb55
+0000000000341eb0  0000000000000008 R_X86_64_RELATIVE                         aeb58
+0000000000341eb8  0000000000000008 R_X86_64_RELATIVE                         aeb5b
+0000000000341ec0  0000000000000008 R_X86_64_RELATIVE                         aeb5e
+0000000000341ec8  0000000000000008 R_X86_64_RELATIVE                         aeb61
+0000000000341ed0  0000000000000008 R_X86_64_RELATIVE                         aeb64
+0000000000341ed8  0000000000000008 R_X86_64_RELATIVE                         aeb67
+0000000000341ee0  0000000000000008 R_X86_64_RELATIVE                         aeb6a
+0000000000341ee8  0000000000000008 R_X86_64_RELATIVE                         aeb6d
+0000000000341ef0  0000000000000008 R_X86_64_RELATIVE                         aeb70
+0000000000341ef8  0000000000000008 R_X86_64_RELATIVE                         aeb73
+0000000000341f00  0000000000000008 R_X86_64_RELATIVE                         aeb76
+0000000000341f08  0000000000000008 R_X86_64_RELATIVE                         aeb79
+0000000000341f10  0000000000000008 R_X86_64_RELATIVE                         aeb7c
+0000000000341f18  0000000000000008 R_X86_64_RELATIVE                         aeb7f
+0000000000341f20  0000000000000008 R_X86_64_RELATIVE                         aeb82
+0000000000341f28  0000000000000008 R_X86_64_RELATIVE                         aeb85
+0000000000341f30  0000000000000008 R_X86_64_RELATIVE                         aeb88
+0000000000341f38  0000000000000008 R_X86_64_RELATIVE                         aeb8b
+0000000000341f40  0000000000000008 R_X86_64_RELATIVE                         aeb8e
+0000000000341f48  0000000000000008 R_X86_64_RELATIVE                         aeb91
 0000000000341f50  0000000000000008 R_X86_64_RELATIVE                         af7c8
-0000000000341f58  0000000000000008 R_X86_64_RELATIVE                         aeb91
-0000000000341f60  0000000000000008 R_X86_64_RELATIVE                         aeb94
-0000000000341f68  0000000000000008 R_X86_64_RELATIVE                         aeb97
-0000000000341f70  0000000000000008 R_X86_64_RELATIVE                         aeb9a
-0000000000341f78  0000000000000008 R_X86_64_RELATIVE                         aeb9d
-0000000000341f80  0000000000000008 R_X86_64_RELATIVE                         aeba0
-0000000000341f88  0000000000000008 R_X86_64_RELATIVE                         aeba3
-0000000000341f90  0000000000000008 R_X86_64_RELATIVE                         aeba6
-0000000000341f98  0000000000000008 R_X86_64_RELATIVE                         aeba9
-0000000000341fa0  0000000000000008 R_X86_64_RELATIVE                         aebac
-0000000000341fa8  0000000000000008 R_X86_64_RELATIVE                         aebaf
-0000000000341fb0  0000000000000008 R_X86_64_RELATIVE                         aebb2
-0000000000341fb8  0000000000000008 R_X86_64_RELATIVE                         aebb5
-0000000000341fc0  0000000000000008 R_X86_64_RELATIVE                         aebb8
-0000000000341fc8  0000000000000008 R_X86_64_RELATIVE                         aebbb
+0000000000341f58  0000000000000008 R_X86_64_RELATIVE                         aeb94
+0000000000341f60  0000000000000008 R_X86_64_RELATIVE                         aeb97
+0000000000341f68  0000000000000008 R_X86_64_RELATIVE                         aeb9a
+0000000000341f70  0000000000000008 R_X86_64_RELATIVE                         aeb9d
+0000000000341f78  0000000000000008 R_X86_64_RELATIVE                         aeba0
+0000000000341f80  0000000000000008 R_X86_64_RELATIVE                         aeba3
+0000000000341f88  0000000000000008 R_X86_64_RELATIVE                         aeba6
+0000000000341f90  0000000000000008 R_X86_64_RELATIVE                         aeba9
+0000000000341f98  0000000000000008 R_X86_64_RELATIVE                         aebac
+0000000000341fa0  0000000000000008 R_X86_64_RELATIVE                         aebaf
+0000000000341fa8  0000000000000008 R_X86_64_RELATIVE                         aebb2
+0000000000341fb0  0000000000000008 R_X86_64_RELATIVE                         aebb5
+0000000000341fb8  0000000000000008 R_X86_64_RELATIVE                         aebb8
+0000000000341fc0  0000000000000008 R_X86_64_RELATIVE                         aebbb
+0000000000341fc8  0000000000000008 R_X86_64_RELATIVE                         aebbe
 0000000000341fd0  0000000000000008 R_X86_64_RELATIVE                         127625
-0000000000341fd8  0000000000000008 R_X86_64_RELATIVE                         aebbe
-0000000000341fe0  0000000000000008 R_X86_64_RELATIVE                         aebc1
-0000000000341fe8  0000000000000008 R_X86_64_RELATIVE                         aebc4
-0000000000341ff0  0000000000000008 R_X86_64_RELATIVE                         aebc7
-0000000000341ff8  0000000000000008 R_X86_64_RELATIVE                         aebca
-0000000000342000  0000000000000008 R_X86_64_RELATIVE                         aebcd
-0000000000342008  0000000000000008 R_X86_64_RELATIVE                         aebd0
-0000000000342010  0000000000000008 R_X86_64_RELATIVE                         aebd3
-0000000000342018  0000000000000008 R_X86_64_RELATIVE                         aebd6
-0000000000342020  0000000000000008 R_X86_64_RELATIVE                         aebd9
-0000000000342028  0000000000000008 R_X86_64_RELATIVE                         aebdc
-0000000000342030  0000000000000008 R_X86_64_RELATIVE                         aebdf
-0000000000342038  0000000000000008 R_X86_64_RELATIVE                         aebe2
-0000000000342040  0000000000000008 R_X86_64_RELATIVE                         aebe5
-0000000000342048  0000000000000008 R_X86_64_RELATIVE                         aebe8
-0000000000342050  0000000000000008 R_X86_64_RELATIVE                         aebeb
-0000000000342058  0000000000000008 R_X86_64_RELATIVE                         aebee
-0000000000342060  0000000000000008 R_X86_64_RELATIVE                         aebf1
-0000000000342068  0000000000000008 R_X86_64_RELATIVE                         aebf4
-0000000000342070  0000000000000008 R_X86_64_RELATIVE                         aebf7
-0000000000342078  0000000000000008 R_X86_64_RELATIVE                         aebfa
-0000000000342080  0000000000000008 R_X86_64_RELATIVE                         aebfd
-0000000000342088  0000000000000008 R_X86_64_RELATIVE                         aec00
-0000000000342090  0000000000000008 R_X86_64_RELATIVE                         aec03
-0000000000342098  0000000000000008 R_X86_64_RELATIVE                         aec06
-00000000003420a0  0000000000000008 R_X86_64_RELATIVE                         aec09
-00000000003420a8  0000000000000008 R_X86_64_RELATIVE                         aec0c
-00000000003420b0  0000000000000008 R_X86_64_RELATIVE                         aec0f
-00000000003420b8  0000000000000008 R_X86_64_RELATIVE                         aec12
-00000000003420c0  0000000000000008 R_X86_64_RELATIVE                         aec15
+0000000000341fd8  0000000000000008 R_X86_64_RELATIVE                         aebc1
+0000000000341fe0  0000000000000008 R_X86_64_RELATIVE                         aebc4
+0000000000341fe8  0000000000000008 R_X86_64_RELATIVE                         aebc7
+0000000000341ff0  0000000000000008 R_X86_64_RELATIVE                         aebca
+0000000000341ff8  0000000000000008 R_X86_64_RELATIVE                         aebcd
+0000000000342000  0000000000000008 R_X86_64_RELATIVE                         aebd0
+0000000000342008  0000000000000008 R_X86_64_RELATIVE                         aebd3
+0000000000342010  0000000000000008 R_X86_64_RELATIVE                         aebd6
+0000000000342018  0000000000000008 R_X86_64_RELATIVE                         aebd9
+0000000000342020  0000000000000008 R_X86_64_RELATIVE                         aebdc
+0000000000342028  0000000000000008 R_X86_64_RELATIVE                         aebdf
+0000000000342030  0000000000000008 R_X86_64_RELATIVE                         aebe2
+0000000000342038  0000000000000008 R_X86_64_RELATIVE                         aebe5
+0000000000342040  0000000000000008 R_X86_64_RELATIVE                         aebe8
+0000000000342048  0000000000000008 R_X86_64_RELATIVE                         aebeb
+0000000000342050  0000000000000008 R_X86_64_RELATIVE                         aebee
+0000000000342058  0000000000000008 R_X86_64_RELATIVE                         aebf1
+0000000000342060  0000000000000008 R_X86_64_RELATIVE                         aebf4
+0000000000342068  0000000000000008 R_X86_64_RELATIVE                         aebf7
+0000000000342070  0000000000000008 R_X86_64_RELATIVE                         aebfa
+0000000000342078  0000000000000008 R_X86_64_RELATIVE                         aebfd
+0000000000342080  0000000000000008 R_X86_64_RELATIVE                         aec00
+0000000000342088  0000000000000008 R_X86_64_RELATIVE                         aec03
+0000000000342090  0000000000000008 R_X86_64_RELATIVE                         aec06
+0000000000342098  0000000000000008 R_X86_64_RELATIVE                         aec09
+00000000003420a0  0000000000000008 R_X86_64_RELATIVE                         aec0c
+00000000003420a8  0000000000000008 R_X86_64_RELATIVE                         aec0f
+00000000003420b0  0000000000000008 R_X86_64_RELATIVE                         aec12
+00000000003420b8  0000000000000008 R_X86_64_RELATIVE                         aec15
+00000000003420c0  0000000000000008 R_X86_64_RELATIVE                         aec18
 00000000003420c8  0000000000000008 R_X86_64_RELATIVE                         b2d6b
-00000000003420d0  0000000000000008 R_X86_64_RELATIVE                         aec18
-00000000003420d8  0000000000000008 R_X86_64_RELATIVE                         aec1b
+00000000003420d0  0000000000000008 R_X86_64_RELATIVE                         aec1b
+00000000003420d8  0000000000000008 R_X86_64_RELATIVE                         aec1e
 00000000003420e0  0000000000000008 R_X86_64_RELATIVE                         b444f
 00000000003420e8  0000000000000008 R_X86_64_RELATIVE                         b4453
 00000000003420f0  0000000000000008 R_X86_64_RELATIVE                         b4457
 00000000003420f8  0000000000000008 R_X86_64_RELATIVE                         b445b
 0000000000342100  0000000000000008 R_X86_64_RELATIVE                         b445f
 0000000000342108  0000000000000008 R_X86_64_RELATIVE                         b4463
 0000000000342110  0000000000000008 R_X86_64_RELATIVE                         b4467
@@ -276,25 +276,25 @@
 0000000000342158  0000000000000008 R_X86_64_RELATIVE                         b4487
 0000000000342160  0000000000000008 R_X86_64_RELATIVE                         b448b
 0000000000342168  0000000000000008 R_X86_64_RELATIVE                         b448f
 0000000000342170  0000000000000008 R_X86_64_RELATIVE                         b4493
 0000000000342178  0000000000000008 R_X86_64_RELATIVE                         b4497
 0000000000343008  0000000000000008 R_X86_64_RELATIVE                         343008
 0000000000343020  0000000000000008 R_X86_64_RELATIVE                         bba48
-0000000000343030  0000000000000008 R_X86_64_RELATIVE                         aec1e
+0000000000343030  0000000000000008 R_X86_64_RELATIVE                         aec21
 0000000000343040  0000000000000008 R_X86_64_RELATIVE                         bc2f8
 0000000000343050  0000000000000008 R_X86_64_RELATIVE                         128652
-0000000000343060  0000000000000008 R_X86_64_RELATIVE                         aec22
+0000000000343060  0000000000000008 R_X86_64_RELATIVE                         aec25
 0000000000343070  0000000000000008 R_X86_64_RELATIVE                         124eee
 0000000000343080  0000000000000008 R_X86_64_RELATIVE                         b1b72
 0000000000343090  0000000000000008 R_X86_64_RELATIVE                         bb0c1
 00000000003430a0  0000000000000008 R_X86_64_RELATIVE                         bb4e4
-00000000003430b0  0000000000000008 R_X86_64_RELATIVE                         aec29
-00000000003430c0  0000000000000008 R_X86_64_RELATIVE                         aec2d
-00000000003430d0  0000000000000008 R_X86_64_RELATIVE                         aec35
+00000000003430b0  0000000000000008 R_X86_64_RELATIVE                         aec2c
+00000000003430c0  0000000000000008 R_X86_64_RELATIVE                         aec30
+00000000003430d0  0000000000000008 R_X86_64_RELATIVE                         aec38
 00000000003430e0  0000000000000008 R_X86_64_RELATIVE                         ae95d
 0000000000343128  0000000000000008 R_X86_64_RELATIVE                         b440c
 0000000000343140  0000000000000008 R_X86_64_RELATIVE                         b7db0
 0000000000343158  0000000000000008 R_X86_64_RELATIVE                         b7dac
 0000000000343170  0000000000000008 R_X86_64_RELATIVE                         b4d4b
 0000000000343188  0000000000000008 R_X86_64_RELATIVE                         b7ddf
 00000000003431a0  0000000000000008 R_X86_64_RELATIVE                         b43e7
```

#### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.ABI-tag
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_ABI_TAG (ABI version tag)	    OS: Linux, ABI: 3.2.0
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 5d7212ebf2bf0c41fd10b720b24ea92f0679ffb9
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 6b5fe68188ed143e8d720b1bf04177995ea93232
```

#### strings --all --bytes=8 {}

```diff
@@ -3519,15 +3519,15 @@
 running "%s" (asap)...
 --- end of plugins list ---
 --- end of loggers list ---
 *** uWSGI loaded clocks ***
 --- end of clocks list ---
 *** uWSGI loaded alarms ***
 --- end of alarms list ---
-29 June 2023 19:39:58
+04 July 2023 19:25:00
 os: %s-%s %s
 nodename: %s
 machine: %s
 clock source: %s
 detected binary path: %s
 mounting "%s" (pre-jail)...
 running "%s" (pre-jail)...
```

#### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -104,46 +104,46 @@
   0x000ae9d0 44003245 00324600 33300033 33003334 D.2E.2F.30.33.34
   0x000ae9e0 00333500 33360033 37003338 00333900 .35.36.37.38.39.
   0x000ae9f0 33410033 42003343 00334400 33450033 3A.3B.3C.3D.3E.3
   0x000aea00 46003430 00343100 34320034 33003434 F.40.41.42.43.44
   0x000aea10 00343500 34360034 37003438 00343900 .45.46.47.48.49.
   0x000aea20 34410034 42003443 00344400 34450034 4A.4B.4C.4D.4E.4
   0x000aea30 46003530 00353100 35330035 34003536 F.50.51.53.54.56
-  0x000aea40 00353700 35390035 41003542 00354300 .57.59.5A.5B.5C.
-  0x000aea50 35440035 45003546 00363000 36310036 5D.5E.5F.60.61.6
-  0x000aea60 32003633 00363500 36360036 37003639 2.63.65.66.67.69
-  0x000aea70 00364100 36420036 43003644 00364500 .6A.6B.6C.6D.6E.
-  0x000aea80 36460037 30003731 00373200 37330037 6F.70.71.72.73.7
-  0x000aea90 34003735 00373600 37370037 38003741 4.75.76.77.78.7A
-  0x000aeaa0 00374200 37430037 44003745 00374600 .7B.7C.7D.7E.7F.
-  0x000aeab0 38310038 32003833 00383400 38350038 81.82.83.84.85.8
-  0x000aeac0 36003837 00383900 38410038 42003843 6.87.89.8A.8B.8C
-  0x000aead0 00384400 38450038 46003930 00393100 .8D.8E.8F.90.91.
-  0x000aeae0 39320039 33003934 00393500 39360039 92.93.94.95.96.9
-  0x000aeaf0 37003938 00393900 39410039 42003943 7.98.99.9A.9B.9C
-  0x000aeb00 00394400 39450039 46004130 00413100 .9D.9E.9F.A0.A1.
-  0x000aeb10 41320041 33004134 00413500 41360041 A2.A3.A4.A5.A6.A
-  0x000aeb20 37004138 00413900 41410041 42004143 7.A8.A9.AA.AB.AC
-  0x000aeb30 00414500 41460042 30004231 00423200 .AE.AF.B0.B1.B2.
-  0x000aeb40 42330042 34004235 00423600 42370042 B3.B4.B5.B6.B7.B
-  0x000aeb50 38004239 00424100 42420042 43004244 8.B9.BA.BB.BC.BD
-  0x000aeb60 00424500 42460043 30004331 00433200 .BE.BF.C0.C1.C2.
-  0x000aeb70 43330043 34004335 00433600 43370043 C3.C4.C5.C6.C7.C
-  0x000aeb80 38004339 00434100 43420043 43004344 8.C9.CA.CB.CC.CD
-  0x000aeb90 00434600 44300044 31004432 00443300 .CF.D0.D1.D2.D3.
-  0x000aeba0 44340044 35004436 00443700 44380044 D4.D5.D6.D7.D8.D
-  0x000aebb0 39004441 00444200 44430044 44004446 9.DA.DB.DC.DD.DF
-  0x000aebc0 00453000 45310045 32004533 00453400 .E0.E1.E2.E3.E4.
-  0x000aebd0 45350045 36004537 00453800 45390045 E5.E6.E7.E8.E9.E
-  0x000aebe0 41004542 00454300 45440045 45004546 A.EB.EC.ED.EE.EF
-  0x000aebf0 00463000 46310046 32004633 00463400 .F0.F1.F2.F3.F4.
-  0x000aec00 46350046 36004637 00463800 46390046 F5.F6.F7.F8.F9.F
-  0x000aec10 41004642 00464300 46450046 46006970 A.FB.FC.FE.FF.ip
-  0x000aec20 63007061 72656e74 006d6e74 00737973 c.parent.mnt.sys
-  0x000aec30 7673656d 00757473 00000000 00000000 vsem.uts........
+  0x000aea40 00353700 35380035 39003541 00354200 .57.58.59.5A.5B.
+  0x000aea50 35430035 44003545 00354600 36300036 5C.5D.5E.5F.60.6
+  0x000aea60 31003632 00363300 36350036 36003637 1.62.63.65.66.67
+  0x000aea70 00363900 36410036 42003643 00364400 .69.6A.6B.6C.6D.
+  0x000aea80 36450036 46003730 00373100 37320037 6E.6F.70.71.72.7
+  0x000aea90 33003734 00373500 37360037 37003738 3.74.75.76.77.78
+  0x000aeaa0 00374100 37420037 43003744 00374500 .7A.7B.7C.7D.7E.
+  0x000aeab0 37460038 31003832 00383300 38340038 7F.81.82.83.84.8
+  0x000aeac0 35003836 00383700 38390038 41003842 5.86.87.89.8A.8B
+  0x000aead0 00384300 38440038 45003846 00393000 .8C.8D.8E.8F.90.
+  0x000aeae0 39310039 32003933 00393400 39350039 91.92.93.94.95.9
+  0x000aeaf0 36003937 00393800 39390039 41003942 6.97.98.99.9A.9B
+  0x000aeb00 00394300 39440039 45003946 00413000 .9C.9D.9E.9F.A0.
+  0x000aeb10 41310041 32004133 00413400 41350041 A1.A2.A3.A4.A5.A
+  0x000aeb20 36004137 00413800 41390041 41004142 6.A7.A8.A9.AA.AB
+  0x000aeb30 00414300 41450041 46004230 00423100 .AC.AE.AF.B0.B1.
+  0x000aeb40 42320042 33004234 00423500 42360042 B2.B3.B4.B5.B6.B
+  0x000aeb50 37004238 00423900 42410042 42004243 7.B8.B9.BA.BB.BC
+  0x000aeb60 00424400 42450042 46004330 00433100 .BD.BE.BF.C0.C1.
+  0x000aeb70 43320043 33004334 00433500 43360043 C2.C3.C4.C5.C6.C
+  0x000aeb80 37004338 00433900 43410043 42004343 7.C8.C9.CA.CB.CC
+  0x000aeb90 00434400 43460044 30004431 00443200 .CD.CF.D0.D1.D2.
+  0x000aeba0 44330044 34004435 00443600 44370044 D3.D4.D5.D6.D7.D
+  0x000aebb0 38004439 00444100 44420044 43004444 8.D9.DA.DB.DC.DD
+  0x000aebc0 00444600 45300045 31004532 00453300 .DF.E0.E1.E2.E3.
+  0x000aebd0 45340045 35004536 00453700 45380045 E4.E5.E6.E7.E8.E
+  0x000aebe0 39004541 00454200 45430045 44004545 9.EA.EB.EC.ED.EE
+  0x000aebf0 00454600 46300046 31004632 00463300 .EF.F0.F1.F2.F3.
+  0x000aec00 46340046 35004636 00463700 46380046 F4.F5.F6.F7.F8.F
+  0x000aec10 39004641 00464200 46430046 45004646 9.FA.FB.FC.FE.FF
+  0x000aec20 00697063 00706172 656e7400 6d6e7400 .ipc.parent.mnt.
+  0x000aec30 73797376 73656d00 75747300 00000000 sysvsem.uts.....
   0x000aec40 21212120 756e6162 6c652074 6f207365 !!! unable to se
   0x000aec50 74207573 65722068 6172616b 69726920 t user harakiri 
   0x000aec60 77697468 6f757420 74686520 6d617374 without the mast
   0x000aec70 65722070 726f6365 73732021 21210a00 er process !!!..
   0x000aec80 756e6162 6c652074 6f206164 64205557 unable to add UW
   0x000aec90 5347495f 41505049 4420746f 20746865 SGI_APPID to the
   0x000aeca0 20757773 67692062 75666665 722c2063  uwsgi buffer, c
@@ -2957,16 +2957,16 @@
   0x000b9c20 2a2a2075 57534749 206c6f61 64656420 ** uWSGI loaded 
   0x000b9c30 636c6f63 6b73202a 2a2a0a00 2d2d2d20 clocks ***..--- 
   0x000b9c40 656e6420 6f662063 6c6f636b 73206c69 end of clocks li
   0x000b9c50 7374202d 2d2d0a0a 000a2a2a 2a207557 st ---....*** uW
   0x000b9c60 53474920 6c6f6164 65642061 6c61726d SGI loaded alarm
   0x000b9c70 73202a2a 2a0a002d 2d2d2065 6e64206f s ***..--- end o
   0x000b9c80 6620616c 61726d73 206c6973 74202d2d f alarms list --
-  0x000b9c90 2d0a0a00 3239204a 756e6520 32303233 -...29 June 2023
-  0x000b9ca0 2031393a 33393a35 3800372e 352e3000  19:39:58.7.5.0.
+  0x000b9c90 2d0a0a00 3034204a 756c7920 32303233 -...04 July 2023
+  0x000b9ca0 2031393a 32353a30 3000372e 352e3000  19:25:00.7.5.0.
   0x000b9cb0 756e616d 65282900 6f733a20 25732d25 uname().os: %s-%
   0x000b9cc0 73202573 0a006e6f 64656e61 6d653a20 s %s..nodename: 
   0x000b9cd0 25730a00 6d616368 696e653a 2025730a %s..machine: %s.
   0x000b9ce0 00636c6f 636b2073 6f757263 653a2025 .clock source: %
   0x000b9cf0 730a0064 65746563 74656420 62696e61 s..detected bina
   0x000b9d00 72792070 6174683a 2025730a 006d6f75 ry path: %s..mou
   0x000b9d10 6e74696e 67202225 73222028 7072652d nting "%s" (pre-
```

#### readelf --wide --decompress --hex-dump=.data.rel.ro {}

```diff
@@ -40,98 +40,98 @@
   0x00341b30 20ea0a00 00000000 23ea0a00 00000000  .......#.......
   0x00341b40 26ea0a00 00000000 29ea0a00 00000000 &.......).......
   0x00341b50 2cea0a00 00000000 2fea0a00 00000000 ,......./.......
   0x00341b60 32ea0a00 00000000 35ea0a00 00000000 2.......5.......
   0x00341b70 255d1200 00000000 38ea0a00 00000000 %]......8.......
   0x00341b80 3bea0a00 00000000 f0fc0a00 00000000 ;...............
   0x00341b90 3eea0a00 00000000 41ea0a00 00000000 >.......A.......
-  0x00341ba0 a79c0b00 00000000 44ea0a00 00000000 ........D.......
-  0x00341bb0 47ea0a00 00000000 4aea0a00 00000000 G.......J.......
-  0x00341bc0 4dea0a00 00000000 50ea0a00 00000000 M.......P.......
-  0x00341bd0 53ea0a00 00000000 56ea0a00 00000000 S.......V.......
-  0x00341be0 59ea0a00 00000000 5cea0a00 00000000 Y.......\.......
-  0x00341bf0 5fea0a00 00000000 62ea0a00 00000000 _.......b.......
-  0x00341c00 944a1200 00000000 65ea0a00 00000000 .J......e.......
-  0x00341c10 68ea0a00 00000000 6bea0a00 00000000 h.......k.......
-  0x00341c20 f65c1200 00000000 6eea0a00 00000000 .\......n.......
-  0x00341c30 71ea0a00 00000000 74ea0a00 00000000 q.......t.......
-  0x00341c40 77ea0a00 00000000 7aea0a00 00000000 w.......z.......
-  0x00341c50 7dea0a00 00000000 80ea0a00 00000000 }...............
-  0x00341c60 83ea0a00 00000000 86ea0a00 00000000 ................
-  0x00341c70 89ea0a00 00000000 8cea0a00 00000000 ................
-  0x00341c80 8fea0a00 00000000 92ea0a00 00000000 ................
-  0x00341c90 95ea0a00 00000000 98ea0a00 00000000 ................
-  0x00341ca0 9bea0a00 00000000 c0851200 00000000 ................
-  0x00341cb0 9eea0a00 00000000 a1ea0a00 00000000 ................
-  0x00341cc0 a4ea0a00 00000000 a7ea0a00 00000000 ................
-  0x00341cd0 aaea0a00 00000000 adea0a00 00000000 ................
-  0x00341ce0 f33e0b00 00000000 b0ea0a00 00000000 .>..............
-  0x00341cf0 b3ea0a00 00000000 b6ea0a00 00000000 ................
-  0x00341d00 b9ea0a00 00000000 bcea0a00 00000000 ................
-  0x00341d10 bfea0a00 00000000 c2ea0a00 00000000 ................
-  0x00341d20 df5c1200 00000000 c5ea0a00 00000000 .\..............
-  0x00341d30 c8ea0a00 00000000 cbea0a00 00000000 ................
-  0x00341d40 ceea0a00 00000000 d1ea0a00 00000000 ................
-  0x00341d50 d4ea0a00 00000000 d7ea0a00 00000000 ................
-  0x00341d60 daea0a00 00000000 ddea0a00 00000000 ................
-  0x00341d70 e0ea0a00 00000000 e3ea0a00 00000000 ................
-  0x00341d80 e6ea0a00 00000000 e9ea0a00 00000000 ................
-  0x00341d90 ecea0a00 00000000 efea0a00 00000000 ................
-  0x00341da0 f2ea0a00 00000000 f5ea0a00 00000000 ................
-  0x00341db0 f8ea0a00 00000000 fbea0a00 00000000 ................
-  0x00341dc0 feea0a00 00000000 01eb0a00 00000000 ................
-  0x00341dd0 04eb0a00 00000000 07eb0a00 00000000 ................
-  0x00341de0 0aeb0a00 00000000 0deb0a00 00000000 ................
-  0x00341df0 10eb0a00 00000000 13eb0a00 00000000 ................
-  0x00341e00 16eb0a00 00000000 19eb0a00 00000000 ................
-  0x00341e10 1ceb0a00 00000000 1feb0a00 00000000 ................
-  0x00341e20 22eb0a00 00000000 25eb0a00 00000000 ".......%.......
-  0x00341e30 28eb0a00 00000000 2beb0a00 00000000 (.......+.......
-  0x00341e40 2eeb0a00 00000000 4c440b00 00000000 ........LD......
-  0x00341e50 31eb0a00 00000000 34eb0a00 00000000 1.......4.......
-  0x00341e60 37eb0a00 00000000 3aeb0a00 00000000 7.......:.......
-  0x00341e70 3deb0a00 00000000 40eb0a00 00000000 =.......@.......
-  0x00341e80 43eb0a00 00000000 46eb0a00 00000000 C.......F.......
-  0x00341e90 49eb0a00 00000000 4ceb0a00 00000000 I.......L.......
-  0x00341ea0 4feb0a00 00000000 52eb0a00 00000000 O.......R.......
-  0x00341eb0 55eb0a00 00000000 58eb0a00 00000000 U.......X.......
-  0x00341ec0 5beb0a00 00000000 5eeb0a00 00000000 [.......^.......
-  0x00341ed0 61eb0a00 00000000 64eb0a00 00000000 a.......d.......
-  0x00341ee0 67eb0a00 00000000 6aeb0a00 00000000 g.......j.......
-  0x00341ef0 6deb0a00 00000000 70eb0a00 00000000 m.......p.......
-  0x00341f00 73eb0a00 00000000 76eb0a00 00000000 s.......v.......
-  0x00341f10 79eb0a00 00000000 7ceb0a00 00000000 y.......|.......
-  0x00341f20 7feb0a00 00000000 82eb0a00 00000000 ................
-  0x00341f30 85eb0a00 00000000 88eb0a00 00000000 ................
-  0x00341f40 8beb0a00 00000000 8eeb0a00 00000000 ................
-  0x00341f50 c8f70a00 00000000 91eb0a00 00000000 ................
-  0x00341f60 94eb0a00 00000000 97eb0a00 00000000 ................
-  0x00341f70 9aeb0a00 00000000 9deb0a00 00000000 ................
-  0x00341f80 a0eb0a00 00000000 a3eb0a00 00000000 ................
-  0x00341f90 a6eb0a00 00000000 a9eb0a00 00000000 ................
-  0x00341fa0 aceb0a00 00000000 afeb0a00 00000000 ................
-  0x00341fb0 b2eb0a00 00000000 b5eb0a00 00000000 ................
-  0x00341fc0 b8eb0a00 00000000 bbeb0a00 00000000 ................
-  0x00341fd0 25761200 00000000 beeb0a00 00000000 %v..............
-  0x00341fe0 c1eb0a00 00000000 c4eb0a00 00000000 ................
-  0x00341ff0 c7eb0a00 00000000 caeb0a00 00000000 ................
-  0x00342000 cdeb0a00 00000000 d0eb0a00 00000000 ................
-  0x00342010 d3eb0a00 00000000 d6eb0a00 00000000 ................
-  0x00342020 d9eb0a00 00000000 dceb0a00 00000000 ................
-  0x00342030 dfeb0a00 00000000 e2eb0a00 00000000 ................
-  0x00342040 e5eb0a00 00000000 e8eb0a00 00000000 ................
-  0x00342050 ebeb0a00 00000000 eeeb0a00 00000000 ................
-  0x00342060 f1eb0a00 00000000 f4eb0a00 00000000 ................
-  0x00342070 f7eb0a00 00000000 faeb0a00 00000000 ................
-  0x00342080 fdeb0a00 00000000 00ec0a00 00000000 ................
-  0x00342090 03ec0a00 00000000 06ec0a00 00000000 ................
-  0x003420a0 09ec0a00 00000000 0cec0a00 00000000 ................
-  0x003420b0 0fec0a00 00000000 12ec0a00 00000000 ................
-  0x003420c0 15ec0a00 00000000 6b2d0b00 00000000 ........k-......
-  0x003420d0 18ec0a00 00000000 1bec0a00 00000000 ................
+  0x00341ba0 44ea0a00 00000000 47ea0a00 00000000 D.......G.......
+  0x00341bb0 4aea0a00 00000000 4dea0a00 00000000 J.......M.......
+  0x00341bc0 50ea0a00 00000000 53ea0a00 00000000 P.......S.......
+  0x00341bd0 56ea0a00 00000000 59ea0a00 00000000 V.......Y.......
+  0x00341be0 5cea0a00 00000000 5fea0a00 00000000 \......._.......
+  0x00341bf0 62ea0a00 00000000 65ea0a00 00000000 b.......e.......
+  0x00341c00 944a1200 00000000 68ea0a00 00000000 .J......h.......
+  0x00341c10 6bea0a00 00000000 6eea0a00 00000000 k.......n.......
+  0x00341c20 f65c1200 00000000 71ea0a00 00000000 .\......q.......
+  0x00341c30 74ea0a00 00000000 77ea0a00 00000000 t.......w.......
+  0x00341c40 7aea0a00 00000000 7dea0a00 00000000 z.......}.......
+  0x00341c50 80ea0a00 00000000 83ea0a00 00000000 ................
+  0x00341c60 86ea0a00 00000000 89ea0a00 00000000 ................
+  0x00341c70 8cea0a00 00000000 8fea0a00 00000000 ................
+  0x00341c80 92ea0a00 00000000 95ea0a00 00000000 ................
+  0x00341c90 98ea0a00 00000000 9bea0a00 00000000 ................
+  0x00341ca0 9eea0a00 00000000 c0851200 00000000 ................
+  0x00341cb0 a1ea0a00 00000000 a4ea0a00 00000000 ................
+  0x00341cc0 a7ea0a00 00000000 aaea0a00 00000000 ................
+  0x00341cd0 adea0a00 00000000 b0ea0a00 00000000 ................
+  0x00341ce0 f33e0b00 00000000 b3ea0a00 00000000 .>..............
+  0x00341cf0 b6ea0a00 00000000 b9ea0a00 00000000 ................
+  0x00341d00 bcea0a00 00000000 bfea0a00 00000000 ................
+  0x00341d10 c2ea0a00 00000000 c5ea0a00 00000000 ................
+  0x00341d20 df5c1200 00000000 c8ea0a00 00000000 .\..............
+  0x00341d30 cbea0a00 00000000 ceea0a00 00000000 ................
+  0x00341d40 d1ea0a00 00000000 d4ea0a00 00000000 ................
+  0x00341d50 d7ea0a00 00000000 daea0a00 00000000 ................
+  0x00341d60 ddea0a00 00000000 e0ea0a00 00000000 ................
+  0x00341d70 e3ea0a00 00000000 e6ea0a00 00000000 ................
+  0x00341d80 e9ea0a00 00000000 ecea0a00 00000000 ................
+  0x00341d90 efea0a00 00000000 f2ea0a00 00000000 ................
+  0x00341da0 f5ea0a00 00000000 f8ea0a00 00000000 ................
+  0x00341db0 fbea0a00 00000000 feea0a00 00000000 ................
+  0x00341dc0 01eb0a00 00000000 04eb0a00 00000000 ................
+  0x00341dd0 07eb0a00 00000000 0aeb0a00 00000000 ................
+  0x00341de0 0deb0a00 00000000 10eb0a00 00000000 ................
+  0x00341df0 13eb0a00 00000000 16eb0a00 00000000 ................
+  0x00341e00 19eb0a00 00000000 1ceb0a00 00000000 ................
+  0x00341e10 1feb0a00 00000000 22eb0a00 00000000 ........".......
+  0x00341e20 25eb0a00 00000000 28eb0a00 00000000 %.......(.......
+  0x00341e30 2beb0a00 00000000 2eeb0a00 00000000 +...............
+  0x00341e40 31eb0a00 00000000 4c440b00 00000000 1.......LD......
+  0x00341e50 34eb0a00 00000000 37eb0a00 00000000 4.......7.......
+  0x00341e60 3aeb0a00 00000000 3deb0a00 00000000 :.......=.......
+  0x00341e70 40eb0a00 00000000 43eb0a00 00000000 @.......C.......
+  0x00341e80 46eb0a00 00000000 49eb0a00 00000000 F.......I.......
+  0x00341e90 4ceb0a00 00000000 4feb0a00 00000000 L.......O.......
+  0x00341ea0 52eb0a00 00000000 55eb0a00 00000000 R.......U.......
+  0x00341eb0 58eb0a00 00000000 5beb0a00 00000000 X.......[.......
+  0x00341ec0 5eeb0a00 00000000 61eb0a00 00000000 ^.......a.......
+  0x00341ed0 64eb0a00 00000000 67eb0a00 00000000 d.......g.......
+  0x00341ee0 6aeb0a00 00000000 6deb0a00 00000000 j.......m.......
+  0x00341ef0 70eb0a00 00000000 73eb0a00 00000000 p.......s.......
+  0x00341f00 76eb0a00 00000000 79eb0a00 00000000 v.......y.......
+  0x00341f10 7ceb0a00 00000000 7feb0a00 00000000 |...............
+  0x00341f20 82eb0a00 00000000 85eb0a00 00000000 ................
+  0x00341f30 88eb0a00 00000000 8beb0a00 00000000 ................
+  0x00341f40 8eeb0a00 00000000 91eb0a00 00000000 ................
+  0x00341f50 c8f70a00 00000000 94eb0a00 00000000 ................
+  0x00341f60 97eb0a00 00000000 9aeb0a00 00000000 ................
+  0x00341f70 9deb0a00 00000000 a0eb0a00 00000000 ................
+  0x00341f80 a3eb0a00 00000000 a6eb0a00 00000000 ................
+  0x00341f90 a9eb0a00 00000000 aceb0a00 00000000 ................
+  0x00341fa0 afeb0a00 00000000 b2eb0a00 00000000 ................
+  0x00341fb0 b5eb0a00 00000000 b8eb0a00 00000000 ................
+  0x00341fc0 bbeb0a00 00000000 beeb0a00 00000000 ................
+  0x00341fd0 25761200 00000000 c1eb0a00 00000000 %v..............
+  0x00341fe0 c4eb0a00 00000000 c7eb0a00 00000000 ................
+  0x00341ff0 caeb0a00 00000000 cdeb0a00 00000000 ................
+  0x00342000 d0eb0a00 00000000 d3eb0a00 00000000 ................
+  0x00342010 d6eb0a00 00000000 d9eb0a00 00000000 ................
+  0x00342020 dceb0a00 00000000 dfeb0a00 00000000 ................
+  0x00342030 e2eb0a00 00000000 e5eb0a00 00000000 ................
+  0x00342040 e8eb0a00 00000000 ebeb0a00 00000000 ................
+  0x00342050 eeeb0a00 00000000 f1eb0a00 00000000 ................
+  0x00342060 f4eb0a00 00000000 f7eb0a00 00000000 ................
+  0x00342070 faeb0a00 00000000 fdeb0a00 00000000 ................
+  0x00342080 00ec0a00 00000000 03ec0a00 00000000 ................
+  0x00342090 06ec0a00 00000000 09ec0a00 00000000 ................
+  0x003420a0 0cec0a00 00000000 0fec0a00 00000000 ................
+  0x003420b0 12ec0a00 00000000 15ec0a00 00000000 ................
+  0x003420c0 18ec0a00 00000000 6b2d0b00 00000000 ........k-......
+  0x003420d0 1bec0a00 00000000 1eec0a00 00000000 ................
   0x003420e0 4f440b00 00000000 53440b00 00000000 OD......SD......
   0x003420f0 57440b00 00000000 5b440b00 00000000 WD......[D......
   0x00342100 5f440b00 00000000 63440b00 00000000 _D......cD......
   0x00342110 67440b00 00000000 00000000 00000000 gD..............
   0x00342120 6b440b00 00000000 6f440b00 00000000 kD......oD......
   0x00342130 73440b00 00000000 77440b00 00000000 sD......wD......
   0x00342140 7b440b00 00000000 7f440b00 00000000 {D.......D......
```

#### readelf --wide --decompress --hex-dump=.data {}

```diff
@@ -1,23 +1,23 @@
 
 Hex dump of section '.data':
   0x00343000 00000000 00000000 08303400 00000000 .........04.....
   0x00343010 00010000 00000000 00000000 00000000 ................
   0x00343020 48ba0b00 00000000 00040000 00000000 H...............
-  0x00343030 1eec0a00 00000000 00000008 00000000 ................
+  0x00343030 21ec0a00 00000000 00000008 00000000 !...............
   0x00343040 f8c20b00 00000000 00000040 00000000 ...........@....
   0x00343050 52861200 00000000 00000080 00000000 R...............
-  0x00343060 22ec0a00 00000000 00800000 00000000 "...............
+  0x00343060 25ec0a00 00000000 00800000 00000000 %...............
   0x00343070 ee4e1200 00000000 00000020 00000000 .N......... ....
   0x00343080 721b0b00 00000000 00000200 00000000 r...............
   0x00343090 c1b00b00 00000000 00000200 00000000 ................
   0x003430a0 e4b40b00 00000000 00000200 00000000 ................
-  0x003430b0 29ec0a00 00000000 00000200 00000000 )...............
-  0x003430c0 2dec0a00 00000000 00000400 00000000 -...............
-  0x003430d0 35ec0a00 00000000 00000004 00000000 5...............
+  0x003430b0 2cec0a00 00000000 00000200 00000000 ,...............
+  0x003430c0 30ec0a00 00000000 00000400 00000000 0...............
+  0x003430d0 38ec0a00 00000000 00000004 00000000 8...............
   0x003430e0 5de90a00 00000000 00000010 00000000 ]...............
   0x003430f0 00000000 00000000 ffffffff 00000000 ................
   0x00343100 01000000 ffffffff ffffffff ffffffff ................
   0x00343110 00000000 00000000 00000000 00000000 ................
   0x00343120 32303000 00000000 0c440b00 00000000 200......D......
   0x00343130 00000000 00000000 33303200 00000000 ........302.....
   0x00343140 b07d0b00 00000000 00000000 00000000 .}..............
```

### Comparing `envoxyd-0.1.6/envoxyd/tools/envoxy-cli` & `envoxyd-0.1.7/envoxyd/tools/envoxy-cli`

 * *Files identical despite different names*

### Comparing `envoxyd-0.1.6/envoxyd/templates/view.py` & `envoxyd-0.1.7/envoxyd/templates/view.py`

 * *Files identical despite different names*

### Comparing `envoxyd-0.1.6/envoxyd/templates/confs/envoxy.json` & `envoxyd-0.1.7/envoxyd/templates/confs/envoxy.json`

 * *Files identical despite different names*

### Comparing `envoxyd-0.1.6/envoxyd/run.py` & `envoxyd-0.1.7/envoxyd/run.py`

 * *Files identical despite different names*

### Comparing `envoxyd-0.1.6/setup.py` & `envoxyd-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 
     def run(self):
         check_call(["python3", "uwsgiconfig.py", "--build", "flask"], cwd='src/envoxyd')
         install.run(self)
 
 setup(
     name='envoxyd',
-    version='0.1.6',
+    version='0.1.7',
     description='Envoxyd',
     author='Matheus Santos',
     author_email='vorj.dux@gmail.com',
     url='https://github.com/muzzley/envoxy',
     packages=find_packages(exclude=["uwsgi", "templates", "tests"]),
     install_requires=[
-        "envoxy>=0.2.6",
+        "envoxy>=0.2.7",
         "flask_cors==3.0.9",
         "isort>=4.2.5,<5"
     ],
     package_dir={
         'envoxyd': 'envoxyd/',
     },
     data_files=[
```

### Comparing `envoxyd-0.1.6/LICENSE.txt` & `envoxyd-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

