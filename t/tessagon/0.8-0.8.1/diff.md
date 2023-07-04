# Comparing `tmp/tessagon-0.8.tar.gz` & `tmp/tessagon-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tessagon-0.8.tar", last modified: Fri Jun 30 02:05:40 2023, max compression
+gzip compressed data, was "tessagon-0.8.1.tar", last modified: Mon Jul  3 16:49:01 2023, max compression
```

## Comparing `tessagon-0.8.tar` & `tessagon-0.8.1.tar`

### file list

```diff
@@ -1,66 +1,68 @@
-drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2023-06-30 02:05:40.165679 tessagon-0.8/
--rw-rw-r--   0 cwant     (1000) cwant     (1000)    11357 2020-04-19 17:19:18.000000 tessagon-0.8/LICENSE
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     1418 2023-06-30 02:05:40.165679 tessagon-0.8/PKG-INFO
--rw-rw-r--   0 cwant     (1000) cwant     (1000)    22372 2023-06-30 01:55:14.000000 tessagon-0.8/README.md
--rw-rw-r--   0 cwant     (1000) cwant     (1000)       38 2023-06-30 02:05:40.165679 tessagon-0.8/setup.cfg
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     1719 2023-06-30 01:55:14.000000 tessagon-0.8/setup.py
-drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2023-06-30 02:05:40.157678 tessagon-0.8/tessagon/
--rw-rw-r--   0 cwant     (1000) cwant     (1000)      102 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/__init__.py
-drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2023-06-30 02:05:40.157678 tessagon-0.8/tessagon/adaptors/
--rw-rw-r--   0 cwant     (1000) cwant     (1000)        0 2023-06-24 19:27:14.000000 tessagon-0.8/tessagon/adaptors/__init__.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)      589 2020-04-19 17:19:18.000000 tessagon-0.8/tessagon/adaptors/blender_adaptor.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)      869 2020-04-19 17:19:18.000000 tessagon-0.8/tessagon/adaptors/list_adaptor.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     1395 2020-04-19 17:19:18.000000 tessagon-0.8/tessagon/adaptors/vtk_adaptor.py
-drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2023-06-30 02:05:40.161678 tessagon-0.8/tessagon/core/
--rw-rw-r--   0 cwant     (1000) cwant     (1000)      735 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/core/__init__.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     8693 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/core/abstract_tile.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)      500 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/core/alternating_tile.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     3326 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/core/grid_tile_generator.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     7697 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/core/parallelogram_tile_generator.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     5663 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/core/tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     4213 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/core/tessagon_discovery.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     1935 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/core/tessagon_metadata.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)    14420 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/core/tile.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     2564 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/core/tile_generator.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)      878 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/core/tile_utils.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     1606 2020-04-19 17:19:18.000000 tessagon-0.8/tessagon/core/value_blend.py
-drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2023-06-30 02:05:40.161678 tessagon-0.8/tessagon/misc/
--rw-rw-r--   0 cwant     (1000) cwant     (1000)        0 2020-04-19 17:19:18.000000 tessagon-0.8/tessagon/misc/__init__.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     3416 2020-04-19 17:19:18.000000 tessagon-0.8/tessagon/misc/shapes.py
-drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2023-06-30 02:05:40.165679 tessagon-0.8/tessagon/types/
--rw-rw-r--   0 cwant     (1000) cwant     (1000)        0 2023-06-24 19:30:11.000000 tessagon-0.8/tessagon/types/__init__.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     6053 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/big_hex_tri_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     2600 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/brick_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     6289 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/cloverdale_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     7202 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/dissected_hex_quad_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     5748 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/dissected_hex_tri_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     4464 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/dissected_square_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     5530 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/dissected_triangle_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     8887 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/dodeca_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     5911 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/dodeca_tri_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     6808 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/floret_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     4252 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/hex_big_tri_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     7194 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/hex_square_tri_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     4934 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/hex_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     3622 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/hex_tri_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     5932 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/islamic_hex_stars_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     4828 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/islamic_stars_crosses_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     3106 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/octo_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     3224 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/penta2_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     5585 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/penta_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     7230 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/pythagorean_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     3529 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/rhombus_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     3387 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/square_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     3566 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/square_tri2_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     5827 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/square_tri_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     5959 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/stanley_park_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     4939 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/tri_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     4209 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/valemount_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     7582 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/weave_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     6350 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/types/zig_zag_tessagon.py
--rw-rw-r--   0 cwant     (1000) cwant     (1000)       20 2023-06-30 01:55:14.000000 tessagon-0.8/tessagon/version.py
-drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2023-06-30 02:05:40.157678 tessagon-0.8/tessagon.egg-info/
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     1418 2023-06-30 02:05:40.000000 tessagon-0.8/tessagon.egg-info/PKG-INFO
--rw-rw-r--   0 cwant     (1000) cwant     (1000)     1886 2023-06-30 02:05:40.000000 tessagon-0.8/tessagon.egg-info/SOURCES.txt
--rw-rw-r--   0 cwant     (1000) cwant     (1000)        1 2023-06-30 02:05:40.000000 tessagon-0.8/tessagon.egg-info/dependency_links.txt
--rw-rw-r--   0 cwant     (1000) cwant     (1000)        9 2023-06-30 02:05:40.000000 tessagon-0.8/tessagon.egg-info/top_level.txt
+drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2023-07-03 16:49:01.608886 tessagon-0.8.1/
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)    11357 2020-04-19 17:19:18.000000 tessagon-0.8.1/LICENSE
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     1420 2023-07-03 16:49:01.608886 tessagon-0.8.1/PKG-INFO
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)    22564 2023-07-03 16:44:33.000000 tessagon-0.8.1/README.md
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)       38 2023-07-03 16:49:01.608886 tessagon-0.8.1/setup.cfg
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     1719 2023-06-30 01:55:14.000000 tessagon-0.8.1/setup.py
+drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2023-07-03 16:49:01.596885 tessagon-0.8.1/tessagon/
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)      116 2023-07-03 16:44:33.000000 tessagon-0.8.1/tessagon/__init__.py
+drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2023-07-03 16:49:01.600885 tessagon-0.8.1/tessagon/adaptors/
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)        0 2023-06-24 19:27:14.000000 tessagon-0.8.1/tessagon/adaptors/__init__.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)       44 2023-07-03 16:44:33.000000 tessagon-0.8.1/tessagon/adaptors/base_adaptor.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)      657 2023-07-03 16:44:33.000000 tessagon-0.8.1/tessagon/adaptors/blender_adaptor.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)      939 2023-07-03 16:44:33.000000 tessagon-0.8.1/tessagon/adaptors/list_adaptor.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     2689 2023-07-03 16:44:33.000000 tessagon-0.8.1/tessagon/adaptors/svg_adaptor.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     1463 2023-07-03 16:44:33.000000 tessagon-0.8.1/tessagon/adaptors/vtk_adaptor.py
+drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2023-07-03 16:49:01.600885 tessagon-0.8.1/tessagon/core/
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)      735 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/core/__init__.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     8693 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/core/abstract_tile.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)      500 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/core/alternating_tile.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     3326 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/core/grid_tile_generator.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     7697 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/core/parallelogram_tile_generator.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     5922 2023-07-03 16:44:33.000000 tessagon-0.8.1/tessagon/core/tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     4213 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/core/tessagon_discovery.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     1935 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/core/tessagon_metadata.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)    14420 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/core/tile.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     2564 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/core/tile_generator.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)      878 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/core/tile_utils.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     1606 2020-04-19 17:19:18.000000 tessagon-0.8.1/tessagon/core/value_blend.py
+drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2023-07-03 16:49:01.600885 tessagon-0.8.1/tessagon/misc/
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)        0 2020-04-19 17:19:18.000000 tessagon-0.8.1/tessagon/misc/__init__.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     3416 2020-04-19 17:19:18.000000 tessagon-0.8.1/tessagon/misc/shapes.py
+drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2023-07-03 16:49:01.608886 tessagon-0.8.1/tessagon/types/
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)        0 2023-06-24 19:30:11.000000 tessagon-0.8.1/tessagon/types/__init__.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     6053 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/big_hex_tri_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     2600 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/brick_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     6289 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/cloverdale_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     7202 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/dissected_hex_quad_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     5748 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/dissected_hex_tri_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     4464 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/dissected_square_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     5530 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/dissected_triangle_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     8887 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/dodeca_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     5911 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/dodeca_tri_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     6808 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/floret_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     4252 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/hex_big_tri_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     7194 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/hex_square_tri_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     4934 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/hex_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     3622 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/hex_tri_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     5932 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/islamic_hex_stars_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     4828 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/islamic_stars_crosses_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     3106 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/octo_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     3224 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/penta2_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     5585 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/penta_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     7230 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/pythagorean_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     3529 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/rhombus_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     3387 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/square_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     3566 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/square_tri2_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     5827 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/square_tri_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     5959 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/stanley_park_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     4939 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/tri_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     4209 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/valemount_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     7582 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/weave_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     6350 2023-06-30 01:55:14.000000 tessagon-0.8.1/tessagon/types/zig_zag_tessagon.py
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)       22 2023-07-03 16:44:33.000000 tessagon-0.8.1/tessagon/version.py
+drwxrwxr-x   0 cwant     (1000) cwant     (1000)        0 2023-07-03 16:49:01.596885 tessagon-0.8.1/tessagon.egg-info/
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     1420 2023-07-03 16:49:01.000000 tessagon-0.8.1/tessagon.egg-info/PKG-INFO
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)     1953 2023-07-03 16:49:01.000000 tessagon-0.8.1/tessagon.egg-info/SOURCES.txt
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)        1 2023-07-03 16:49:01.000000 tessagon-0.8.1/tessagon.egg-info/dependency_links.txt
+-rw-rw-r--   0 cwant     (1000) cwant     (1000)        9 2023-07-03 16:49:01.000000 tessagon-0.8.1/tessagon.egg-info/top_level.txt
```

### Comparing `tessagon-0.8/LICENSE` & `tessagon-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/PKG-INFO` & `tessagon-0.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tessagon
-Version: 0.8
+Version: 0.8.1
 Summary: Tessellate your favorite 2D manifolds with triangles, hexagons, and other interesting patterns.
 Home-page: https://github.com/cwant/tessagon
 Author: Chris Want
 License: UNKNOWN
 Keywords: tesselation tiling modeling blender vtk
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tessagon-0.8/README.md` & `tessagon-0.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 Tessellate your favorite 3D surfaces (technically, 2D manifolds) with triangles, hexagons, or a number of other curated tiling types!
 
 ![Animation of tessellated torii](https://raw.githubusercontent.com/cwant/tessagon/master/documentation/images/tessagon_demo.gif)
 
 ## News
 
-**Now works with Blender 2.8 (and still works with earlier versions). Todo: check if it works with Blender 3.x.**
+**A nascent Inkscape extension to create tiling patterns: <https://github.com/cwant/inkscape-tiling-extension>**
 
-**Check out my presentation on the creation of Tessagon as an open source Python project here: [https://cwant.github.io/python-os-presentation](https://cwant.github.io/python-os-presentation/#/)**
+**You can find a Blender (3.6) pull request to add support for Tessagon in the "XYZ function" addon here:
+<https://projects.blender.org/blender/blender-addons/pulls/104726>**
 
-**A demo of using Tessagon with Inkscape can be found [here](https://gist.github.com/cwant/697f0c6ce07d9e14e710f5b80ca5eece).**
+**Check out my presentation on the creation of Tessagon as an open source Python project here: <https://cwant.github.io/python-os-presentation>**
 
-**~You can find a Blender pull request to add support for Tessagon in the "XYZ function" addon here:
-[https://developer.blender.org/D3519](https://developer.blender.org/D3519)~** (This didn't really go anywhere, and was for Blender 2.x)
+**A demo of using Tessagon with Inkscape Simple Scripting can be found [here](https://gist.github.com/cwant/697f0c6ce07d9e14e710f5b80ca5eece).**
 
 ## TL;DR
 
 Check out the repository and look in the `demo` directory.
 
 * **Blender**: you'll find a blender file and `tessagon_blender_demo.py` which creates the meshes in the demo. The demo has examples of each tessagon class, and an example that uses tessagon with one of my other projects, [wire_skin](https://github.com/cwant/wire_skin).
 * **VTK**: Take a look at `tessagon_vtk_demo.py` for a script that creates all of the current tessagon classes.
@@ -32,17 +32,18 @@
 
 ## How it works
 
 Three things are needed to use tessagon to tessellate the surface of a 2D-manifold (or more accurately, a patch on a 2D-manifold in 3-space):
 
 * Tessagon provides a bunch of classes (subclasses of a class called `Tessagon`) that will tessellate a portion of UV-space with mesh patterns. Parameters provide the details of the bounds in UV-space, the resolution of the tiling, whether the tiling is cyclic, whether a cyclic domain "twists" (think a topological identification space, like a Mobius strip or a Klein bottle), whether it is rotated, etc. These classes are in the `tessagon.types` module.
 * The programmer must provide a formula that describes the shape of surface of the 3-dimensional object to create. This function maps two-dimensional space (also known as UV-space) into 3-dimensional space. The tiling happens in the input two dimensional space, and the function maps the tiling onto the surface of the 3-dimensional shape. There are some demo functions in `tessagon.misc.shapes`, such as torii (a.k.a. donuts), spheres, cylinders, etc.
-* Finally, an adaptor is chosen to create a mesh in a supported 3D software package. Currently only Blender and VTK are supported, but there is also a generic `ListAdaptor` that does not depend on any external package, and can aid in the creation of importers (and is useful for testing/debugging):
+* Finally, an adaptor is chosen to create a mesh in a supported 3D software package. Currently Blender and VTK are supported applications. There is an adaptor that writes an SVG group to a string, with various options (root SVG node, style options). There is also a generic `ListAdaptor` that does not depend on any external package, and can aid in the creation of importers (and is useful for testing/debugging):
   * adaptor `BlenderAdaptor` from the module `tessagon.adaptors.blender_adaptor`. The output from the adaptor's `get_mesh` method is of type `BMesh`.
   * adaptor `VtkAdaptor` from the module `tessagon.adaptors.vtk_adaptor`. The output from the adaptor's `get_mesh` method is of type `VtkPolydata`.
+  * adaptor `SvgAdaptor` from the module `tessagon.adaptors.svg_adaptor`. The output from the adaptor's `get_mesh` method is a string (by default, an SVG group of polygons).
   * adaptor `ListAdaptor` from the module `tessagon.adaptors.list_adaptor`. The output from the adaptor's `get_mesh` method is a dict with keys `vert_list`, `face_list` and `color_list`, which point to lists of vertices, faces (as indices into the vertex list), and color indices for each face.
 
   (Note that the `get_mesh` methods mentioned above are usually called indirectly through the `Tessagon` method `create_mesh`.)
  
 The reader should check out the demos, but here is some very basic usage using blender:
 
 ```python
```

### Comparing `tessagon-0.8/setup.py` & `tessagon-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/adaptors/blender_adaptor.py` & `tessagon-0.8.1/tessagon/adaptors/blender_adaptor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from tessagon.adaptors.base_adaptor import BaseAdaptor
 import bmesh
 
 
-class BlenderAdaptor:
+class BlenderAdaptor(BaseAdaptor):
     def __init__(self, **kwargs):
         self.bm = None
 
     def create_empty_mesh(self):
         self.bm = bmesh.new()
 
     def initialize_colors(self):
```

### Comparing `tessagon-0.8/tessagon/adaptors/list_adaptor.py` & `tessagon-0.8.1/tessagon/adaptors/list_adaptor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-class ListAdaptor:
+from tessagon.adaptors.base_adaptor import BaseAdaptor
+
+
+class ListAdaptor(BaseAdaptor):
 
     def __init__(self, **kwargs):
         self.vert_list = None
         self.face_list = None
         self.color_list = None
 
     def create_empty_mesh(self):
```

### Comparing `tessagon-0.8/tessagon/adaptors/vtk_adaptor.py` & `tessagon-0.8.1/tessagon/adaptors/vtk_adaptor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from tessagon.adaptors.base_adaptor import BaseAdaptor
 import vtk
 
 
-class VtkAdaptor:
+class VtkAdaptor(BaseAdaptor):
     def __init__(self, **kwargs):
         self.point_count = 0
         self.face_count = 0
         self.points = None
         self.polys = None
         self.poly_data = None
         self.scalars = None
```

### Comparing `tessagon-0.8/tessagon/core/__init__.py` & `tessagon-0.8.1/tessagon/core/__init__.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/core/abstract_tile.py` & `tessagon-0.8.1/tessagon/core/abstract_tile.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/core/grid_tile_generator.py` & `tessagon-0.8.1/tessagon/core/grid_tile_generator.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/core/parallelogram_tile_generator.py` & `tessagon-0.8.1/tessagon/core/parallelogram_tile_generator.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/core/tessagon.py` & `tessagon-0.8.1/tessagon/core/tessagon.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,22 @@
         # Optional post processing function
         self.post_process = None
         if 'post_process' in kwargs:
             self.post_process = kwargs['post_process']
 
         if 'adaptor_class' in kwargs:
             adaptor_class = kwargs['adaptor_class']
-            self.mesh_adaptor = adaptor_class(**kwargs)
+
+            # Get options that are specific to this adaptor
+            adaptor_options = {}
+            for option in adaptor_class.ADAPTOR_OPTIONS:
+                if option in kwargs:
+                    adaptor_options[option] = kwargs[option]
+
+            self.mesh_adaptor = adaptor_class(**adaptor_options)
         else:
             raise ValueError('Must provide a mesh adaptor class')
 
         self.color_pattern = kwargs.get('color_pattern') or None
 
         self.tiles = None
         self.face_types = {}
```

### Comparing `tessagon-0.8/tessagon/core/tessagon_discovery.py` & `tessagon-0.8.1/tessagon/core/tessagon_discovery.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/core/tessagon_metadata.py` & `tessagon-0.8.1/tessagon/core/tessagon_metadata.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/core/tile.py` & `tessagon-0.8.1/tessagon/core/tile.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/core/tile_generator.py` & `tessagon-0.8.1/tessagon/core/tile_generator.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/core/tile_utils.py` & `tessagon-0.8.1/tessagon/core/tile_utils.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/core/value_blend.py` & `tessagon-0.8.1/tessagon/core/value_blend.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/misc/shapes.py` & `tessagon-0.8.1/tessagon/misc/shapes.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/big_hex_tri_tessagon.py` & `tessagon-0.8.1/tessagon/types/big_hex_tri_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/brick_tessagon.py` & `tessagon-0.8.1/tessagon/types/brick_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/cloverdale_tessagon.py` & `tessagon-0.8.1/tessagon/types/cloverdale_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/dissected_hex_quad_tessagon.py` & `tessagon-0.8.1/tessagon/types/dissected_hex_quad_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/dissected_hex_tri_tessagon.py` & `tessagon-0.8.1/tessagon/types/dissected_hex_tri_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/dissected_square_tessagon.py` & `tessagon-0.8.1/tessagon/types/dissected_square_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/dissected_triangle_tessagon.py` & `tessagon-0.8.1/tessagon/types/dissected_triangle_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/dodeca_tessagon.py` & `tessagon-0.8.1/tessagon/types/dodeca_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/dodeca_tri_tessagon.py` & `tessagon-0.8.1/tessagon/types/dodeca_tri_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/floret_tessagon.py` & `tessagon-0.8.1/tessagon/types/floret_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/hex_big_tri_tessagon.py` & `tessagon-0.8.1/tessagon/types/hex_big_tri_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/hex_square_tri_tessagon.py` & `tessagon-0.8.1/tessagon/types/hex_square_tri_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/hex_tessagon.py` & `tessagon-0.8.1/tessagon/types/hex_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/hex_tri_tessagon.py` & `tessagon-0.8.1/tessagon/types/hex_tri_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/islamic_hex_stars_tessagon.py` & `tessagon-0.8.1/tessagon/types/islamic_hex_stars_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/islamic_stars_crosses_tessagon.py` & `tessagon-0.8.1/tessagon/types/islamic_stars_crosses_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/octo_tessagon.py` & `tessagon-0.8.1/tessagon/types/octo_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/penta2_tessagon.py` & `tessagon-0.8.1/tessagon/types/penta2_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/penta_tessagon.py` & `tessagon-0.8.1/tessagon/types/penta_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/pythagorean_tessagon.py` & `tessagon-0.8.1/tessagon/types/pythagorean_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/rhombus_tessagon.py` & `tessagon-0.8.1/tessagon/types/rhombus_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/square_tessagon.py` & `tessagon-0.8.1/tessagon/types/square_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/square_tri2_tessagon.py` & `tessagon-0.8.1/tessagon/types/square_tri2_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/square_tri_tessagon.py` & `tessagon-0.8.1/tessagon/types/square_tri_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/stanley_park_tessagon.py` & `tessagon-0.8.1/tessagon/types/stanley_park_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/tri_tessagon.py` & `tessagon-0.8.1/tessagon/types/tri_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/valemount_tessagon.py` & `tessagon-0.8.1/tessagon/types/valemount_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/weave_tessagon.py` & `tessagon-0.8.1/tessagon/types/weave_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon/types/zig_zag_tessagon.py` & `tessagon-0.8.1/tessagon/types/zig_zag_tessagon.py`

 * *Files identical despite different names*

### Comparing `tessagon-0.8/tessagon.egg-info/PKG-INFO` & `tessagon-0.8.1/tessagon.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tessagon
-Version: 0.8
+Version: 0.8.1
 Summary: Tessellate your favorite 2D manifolds with triangles, hexagons, and other interesting patterns.
 Home-page: https://github.com/cwant/tessagon
 Author: Chris Want
 License: UNKNOWN
 Keywords: tesselation tiling modeling blender vtk
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tessagon-0.8/tessagon.egg-info/SOURCES.txt` & `tessagon-0.8.1/tessagon.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 tessagon/__init__.py
 tessagon/version.py
 tessagon.egg-info/PKG-INFO
 tessagon.egg-info/SOURCES.txt
 tessagon.egg-info/dependency_links.txt
 tessagon.egg-info/top_level.txt
 tessagon/adaptors/__init__.py
+tessagon/adaptors/base_adaptor.py
 tessagon/adaptors/blender_adaptor.py
 tessagon/adaptors/list_adaptor.py
+tessagon/adaptors/svg_adaptor.py
 tessagon/adaptors/vtk_adaptor.py
 tessagon/core/__init__.py
 tessagon/core/abstract_tile.py
 tessagon/core/alternating_tile.py
 tessagon/core/grid_tile_generator.py
 tessagon/core/parallelogram_tile_generator.py
 tessagon/core/tessagon.py
```

