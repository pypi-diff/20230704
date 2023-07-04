# Comparing `tmp/mapchete-2023.6.5.tar.gz` & `tmp/mapchete-2023.7.0.tar.gz`

## Comparing `mapchete-2023.6.5.tar` & `mapchete-2023.7.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/__init__.py
--rw-r--r--   0        0        0    29123 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/_core.py
--rw-r--r--   0        0        0    26311 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/_executor.py
--rw-r--r--   0        0        0    32289 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/_processing.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/_registered.py
--rw-r--r--   0        0        0    16702 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/_tasks.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/_timer.py
--rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/_user_process.py
--rw-r--r--   0        0        0    49580 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/config.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/errors.py
--rw-r--r--   0        0        0    17833 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/index.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/log.py
--rw-r--r--   0        0        0    25018 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/path.py
--rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/stac.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/testing.py
--rw-r--r--   0        0        0    17045 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/tile.py
--rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/types.py
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/validate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/cli/__init__.py
--rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/cli/main.py
--rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/cli/options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/cli/default/__init__.py
--rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/cli/default/convert.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/cli/default/cp.py
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/cli/default/create.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/cli/default/execute.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/cli/default/formats.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/cli/default/index.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/cli/default/processes.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/cli/default/rm.py
--rwxr-xr-x   0        0        0     5035 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/cli/default/serve.py
--rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/cli/default/stac.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/commands/__init__.py
--rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/commands/_convert.py
--rw-r--r--   0        0        0     8546 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/commands/_cp.py
--rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/commands/_execute.py
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/commands/_index.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/commands/_rm.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/commons/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/commons/clip.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/commons/contours.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/commons/hillshade.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/formats/__init__.py
--rw-r--r--   0        0        0    20760 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/formats/base.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/formats/drivers.py
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/formats/loaders.py
--rw-r--r--   0        0        0    12732 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/formats/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/formats/default/__init__.py
--rw-r--r--   0        0        0     6783 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/formats/default/_fiona_base.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/formats/default/flatgeobuf.py
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/formats/default/geobuf.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/formats/default/geojson.py
--rw-r--r--   0        0        0    22184 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/formats/default/gtiff.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/formats/default/mapchete_input.py
--rw-r--r--   0        0        0     6935 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/formats/default/png.py
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/formats/default/png_hillshade.py
--rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/formats/default/raster_file.py
--rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/formats/default/tile_directory.py
--rw-r--r--   0        0        0     9450 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/formats/default/vector_file.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/io/__init__.py
--rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/io/_geometry_operations.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/io/_json.py
--rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/io/_misc.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/io/_path.py
--rw-r--r--   0        0        0    44448 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/io/raster.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/io/settings.py
--rw-r--r--   0        0        0    22010 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/io/vector.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/processes/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/processes/contours.py
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/processes/convert.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/processes/hillshade.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/processes/examples/__init__.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/processes/examples/example_process.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/static/__init__.py
--rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/static/index.html
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/static/mapchete_template.mapchete
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 mapchete-2023.6.5/mapchete/static/process_template.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mapchete-2023.6.5/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapchete-2023.6.5/LICENSE
--rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2023.6.5/README.rst
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 mapchete-2023.6.5/pyproject.toml
--rw-r--r--   0        0        0     9061 2020-02-02 00:00:00.000000 mapchete-2023.6.5/PKG-INFO
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/__init__.py
+-rw-r--r--   0        0        0    29123 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/_core.py
+-rw-r--r--   0        0        0    25534 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/_executor.py
+-rw-r--r--   0        0        0    32289 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/_processing.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/_registered.py
+-rw-r--r--   0        0        0    16702 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/_tasks.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/_timer.py
+-rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/_user_process.py
+-rw-r--r--   0        0        0    49580 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/config.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/errors.py
+-rw-r--r--   0        0        0    17833 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/index.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/log.py
+-rw-r--r--   0        0        0    25327 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/path.py
+-rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/stac.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/testing.py
+-rw-r--r--   0        0        0    17045 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/tile.py
+-rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/types.py
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/validate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/__init__.py
+-rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/main.py
+-rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/default/__init__.py
+-rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/default/convert.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/default/cp.py
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/default/create.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/default/execute.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/default/formats.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/default/index.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/default/processes.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/default/rm.py
+-rwxr-xr-x   0        0        0     5035 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/default/serve.py
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/default/stac.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/commands/__init__.py
+-rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/commands/_convert.py
+-rw-r--r--   0        0        0     8546 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/commands/_cp.py
+-rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/commands/_execute.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/commands/_index.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/commands/_rm.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/commons/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/commons/clip.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/commons/contours.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/commons/hillshade.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/__init__.py
+-rw-r--r--   0        0        0    20760 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/base.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/drivers.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/loaders.py
+-rw-r--r--   0        0        0    12732 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/__init__.py
+-rw-r--r--   0        0        0     6783 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/_fiona_base.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/flatgeobuf.py
+-rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/geobuf.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/geojson.py
+-rw-r--r--   0        0        0    22184 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/gtiff.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/mapchete_input.py
+-rw-r--r--   0        0        0     6935 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/png.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/png_hillshade.py
+-rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/raster_file.py
+-rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/tile_directory.py
+-rw-r--r--   0        0        0     9450 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/vector_file.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/io/__init__.py
+-rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/io/_geometry_operations.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/io/_json.py
+-rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/io/_misc.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/io/_path.py
+-rw-r--r--   0        0        0    44448 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/io/raster.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/io/settings.py
+-rw-r--r--   0        0        0    22010 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/io/vector.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/processes/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/processes/contours.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/processes/convert.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/processes/hillshade.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/processes/examples/__init__.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/processes/examples/example_process.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/static/__init__.py
+-rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/static/index.html
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/static/mapchete_template.mapchete
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/static/process_template.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mapchete-2023.7.0/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapchete-2023.7.0/LICENSE
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2023.7.0/README.rst
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 mapchete-2023.7.0/pyproject.toml
+-rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 mapchete-2023.7.0/PKG-INFO
```

### Comparing `mapchete-2023.6.5/mapchete/__init__.py` & `mapchete-2023.7.0/mapchete/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,11 +15,11 @@
     "ProcessInfo",
     "Timer",
     "Executor",
     "FakeFuture",
     "SkippedFuture",
     "Job",
 ]
-__version__ = "2023.6.5"
+__version__ = "2023.7.0"
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
```

### Comparing `mapchete-2023.6.5/mapchete/_core.py` & `mapchete-2023.7.0/mapchete/_core.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/_executor.py` & `mapchete-2023.7.0/mapchete/_executor.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,22 +72,26 @@
         fargs=None,
         fkwargs=None,
         max_submitted_tasks=500,
         item_skip_bool=False,
         **kwargs,
     ):
         """Submit tasks to executor and start yielding finished futures."""
+
+        # before running, make sure cancel signal is False
+        self.cancel_signal = False
+
         try:
             fargs = fargs or ()
             fkwargs = fkwargs or {}
             logger.debug("submitting tasks to executor")
             i = 0
             with Timer() as timer:
                 for i, item in enumerate(iterable, 1):
-                    if self.cancelled:  # pragma: no cover
+                    if self.cancel_signal:  # pragma: no cover
                         logger.debug("executor cancelled")
                         return
 
                     # skip task submission if option is activated
                     if item_skip_bool:
                         item, skip, skip_info = item
                         if skip:
@@ -123,14 +127,15 @@
                 yield self._finished_future(future)
 
         except CancelledError:  # pragma: no cover
             return
         finally:
             # reset so futures won't linger here for next call
             self.running_futures = set()
+            self.finished_futures = set()
 
     def _submit(self, func, *fargs, **fkwargs):
         future = self._executor.submit(func, *fargs, **fkwargs)
         self.running_futures.add(future)
         future.add_done_callback(self._add_to_finished)
 
     def _ready(self):
@@ -139,15 +144,15 @@
     def _add_to_finished(self, future):
         self.finished_futures.add(future)
 
     def map(self, func, iterable, fargs=None, fkwargs=None):
         return self._map(func, iterable, fargs=fargs, fkwargs=fkwargs)
 
     def cancel(self):
-        self.cancelled = True
+        self.cancel_signal = True
         logger.debug("cancel %s futures...", len(self.running_futures))
         for future in self.running_futures:
             future.cancel()
         logger.debug("%s futures cancelled", len(self.running_futures))
         self.wait()
         # reset so futures won't linger here for next call
         self.running_futures = set()
@@ -185,19 +190,14 @@
 
         # raise exception if future errored or was cancelled
         future = future_raise_exception(future)
 
         # create minimal Future-like object with no references to the cluster
         finished_future = FinishedFuture(future, result=result)
 
-        # explicitly release future
-        try:
-            future.release()
-        except AttributeError:
-            pass
         return finished_future
 
     @cached_property
     def _executor(self):
         return self._executor_cls(*self._executor_args, **self._executor_kwargs)
 
     def __enter__(self):
@@ -301,26 +301,27 @@
             Submit tasks in chunks to scheduler.
 
         Yields
         ------
         finished futures
 
         """
-        from dask.distributed import TimeoutError
-
         max_submitted_tasks = max_submitted_tasks or 500
         chunksize = chunksize or 100
 
+        # before running, make sure cancel signal is False
+        self.cancel_signal = False
+
         try:
             fargs = fargs or ()
             fkwargs = fkwargs or {}
             chunk = []
             for item in iterable:
                 # abort if execution is cancelled
-                if self.cancelled:  # pragma: no cover
+                if self.cancel_signal:  # pragma: no cover
                     logger.debug("executor cancelled")
                     return
 
                 # skip task submission if option is activated
                 if item_skip_bool:
                     item, skip, skip_info = item
                     if skip:
@@ -368,15 +369,14 @@
             # submit last chunk of items
             self._submit_chunk(
                 chunk=chunk,
                 func=func,
                 fargs=fargs,
                 fkwargs=fkwargs,
             )
-            chunk = []
             # yield remaining futures as they finish
             if self._ac_iterator is not None:
                 logger.debug("yield %s remaining futures", self._submitted)
                 for batch in self._ac_iterator.batches():
                     try:
                         yield from self._yield_from_batch(batch)
                     except JobCancelledError:  # pragma: no cover
@@ -385,72 +385,27 @@
         finally:
             # reset so futures won't linger here for next call
             self.running_futures = set()
             self._ac_iterator.clear()
             self._submitted = 0
 
     def _submit_chunk(self, chunk=None, func=None, fargs=None, fkwargs=None):
-        logger.debug("submit chunk of %s items to cluster", len(chunk))
-        futures = self._executor.map(partial(func, *fargs, **fkwargs), chunk)
-        self._ac_iterator.update(futures)
-        self._submitted += len(futures)
+        if chunk:
+            logger.debug("submit chunk of %s items to cluster", len(chunk))
+            futures = self._executor.map(partial(func, *fargs, **fkwargs), chunk)
+            self._ac_iterator.update(futures)
+            self._submitted += len(futures)
 
     def _yield_from_batch(self, batch):
-        from dask.distributed import TimeoutError
-        from distributed.comm.core import CommClosedError
-
-        cancelled_futures = []
-
         for future, result in batch:
             self._submitted -= 1
-            if self.cancelled:  # pragma: no cover
+            if self.cancel_signal:  # pragma: no cover
                 logger.debug("executor cancelled")
                 raise JobCancelledError()
-            try:
-                yield self._finished_future(future, result, _dask=True)
-            except TimeoutError:  # pragma: no cover
-                logger.error(
-                    "%s: couldn't fetch future result() or exception() in %ss",
-                    future,
-                    FUTURE_TIMEOUT,
-                )
-                self._retry(future)
-            except CancelledError as exc:  # pragma: no cover
-                logger.error("%s got cancelled: %s", future, exc)
-                cancelled_futures.append(future)
-
-        if cancelled_futures:  # pragma: no cover
-            logger.error("caught %s cancelled_futures", len(cancelled_futures))
-            try:
-                logger.debug("try to get scheduler logs...")
-                logger.debug(
-                    "scheduler logs: %s", self._executor.get_scheduler_logs(n=1000)
-                )
-            except Exception as e:
-                logger.exception(e)
-            status = self._executor.status
-            if status in ("running", "connecting"):
-                try:
-                    logger.debug("retry %s futures...", len(cancelled_futures))
-                    for future in cancelled_futures:
-                        self._retry(future)
-                except KeyError:
-                    raise RuntimeError(
-                        f"unable to retry {len(cancelled_futures)} cancelled futures {self._executor} ({status})"
-                    )
-            else:
-                raise RuntimeError(
-                    f"client lost connection to scheduler {self._executor} ({status})"
-                )
-
-    def _retry(self, future):  # pragma: no cover
-        logger.debug("retry future %s", future)
-        future.retry()
-        self._ac_iterator.add(future)
-        self._submitted += 1
+            yield self._finished_future(future, result, _dask=True)
 
     @cached_property
     def _executor(self):
         return self._executor_client or self._executor_cls(
             *self._executor_args, **self._executor_kwargs
         )
 
@@ -550,16 +505,19 @@
     def as_completed(
         self, func, iterable, fargs=None, fkwargs=None, item_skip_bool=False, **kwargs
     ):
         """Yield finished tasks."""
         fargs = fargs or []
         fkwargs = fkwargs or {}
 
+        # before running, make sure cancel signal is False
+        self.cancel_signal = False
+
         for item in iterable:
-            if self.cancelled:
+            if self.cancel_signal:
                 logger.debug("executor cancelled")
                 return
             # skip task submission if option is activated
             if item_skip_bool:
                 item, skip, skip_info = item
                 if skip:
                     yield SkippedFuture(item, skip_info=skip_info)
@@ -570,15 +528,15 @@
 
     def _map(self, func, iterable, fargs=None, fkwargs=None):
         fargs = fargs or []
         fkwargs = fkwargs or {}
         return list(map(partial(func, *fargs, **fkwargs), iterable))
 
     def cancel(self):
-        self.cancelled = True
+        self.cancel_signal = True
 
     def _wait(self):  # pragma: no cover
         return
 
     def __exit__(self, *args):
         """Exit context manager."""
         logger.debug("SequentialExecutor closed")
@@ -698,14 +656,15 @@
 
     This is a workaround between the slightly different APIs of dask and concurrent.futures.
     It also tries to avoid potentially expensive calls to the dask scheduler.
     """
     # dask futures
     if hasattr(future, "status"):
         if future.status == "cancelled":  # pragma: no cover
+            # dask CancelledErrors hide inside future.result(), so get it from here
             exception = future.result(timeout=FUTURE_TIMEOUT)
         elif future.status == "error":
             exception = future.exception(timeout=FUTURE_TIMEOUT)
         else:  # pragma: no cover
             exception = None
 
     # concurrent.futures futures
@@ -716,28 +675,50 @@
         raise TypeError("future %s does not have an exception to raise", future)
 
     return exception
 
 
 def future_raise_exception(future, raise_errors=True):
     """
-    Checks whether future contains an exception and raises it.
+    Checks whether future contains an exception and raises it as MapcheteTaskFailed.
     """
+
+    # Some exception types such as dask exceptions or generic CancelledErrors indicate that
+    # there was an error around the Executor rather than from the future/task itself.
+    # Let's directly re-raise these to be more transparent.
+    try:
+        # when using dask, also directly raise specific dask errors
+        from distributed import CancelledError
+        from dask.distributed import TimeoutError
+        from distributed.comm.core import CommClosedError
+
+        keep_exceptions = (CancelledError, TimeoutError, CommClosedError)
+    except ImportError:  # pragma: no cover
+        keep_exceptions = (CancelledError,)
+
     if raise_errors and future_is_failed_or_cancelled(future):
         future_name = (
             future.key.rstrip("_finished") if hasattr(future, "key") else str(future)
         )
+
         try:
             exception = future_exception(future)
+
+        # in case the exception cannot be retrieved
         except Exception as exc:  # pragma: no cover
             # dask futures
             if hasattr(future, "status"):
                 msg = f"{future_name} has status '{future.status}' but its exception could not be recovered due to a {exc}"
             # concurrent.futures futures
             else:
                 msg = f"{future_name} failed but its exception could not be recovered due to a {exc}"
             raise MapcheteTaskFailed(msg)
 
+        # keep some exceptions as they are
+        if isinstance(exception, keep_exceptions):
+            raise exception
+
         raise MapcheteTaskFailed(
             f"{future_name} raised a {repr(exception)}"
         ).with_traceback(exception.__traceback__)
+
     return future
```

### Comparing `mapchete-2023.6.5/mapchete/_processing.py` & `mapchete-2023.7.0/mapchete/_processing.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/_registered.py` & `mapchete-2023.7.0/mapchete/_registered.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/_tasks.py` & `mapchete-2023.7.0/mapchete/_tasks.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/_timer.py` & `mapchete-2023.7.0/mapchete/_timer.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/_user_process.py` & `mapchete-2023.7.0/mapchete/_user_process.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/config.py` & `mapchete-2023.7.0/mapchete/config.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/errors.py` & `mapchete-2023.7.0/mapchete/errors.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/index.py` & `mapchete-2023.7.0/mapchete/index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/log.py` & `mapchete-2023.7.0/mapchete/log.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/path.py` & `mapchete-2023.7.0/mapchete/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from rasterio.session import Session as RioSession
 
 from mapchete._executor import Executor
 from mapchete.io.settings import GDAL_HTTP_OPTS
 
 logger = logging.getLogger(__name__)
 
-DEFAULT_STORAGE_OPTIONS = {"asynchronous": False, "timeout": 5}
+DEFAULT_STORAGE_OPTIONS = {"asynchronous": False, "timeout": None}
 UNALLOWED_S3_KWARGS = ["timeout"]
 UNALLOWED_HTTP_KWARGS = ["username", "password"]
 
 
 class MPath(os.PathLike):
     """
     Partially replicates pathlib.Path but with remote file support.
@@ -85,15 +85,14 @@
         elif isinstance(inp, MPath):
             if kwargs:
                 return MPath(inp, **kwargs)
             return inp
         elif hasattr(inp, "__fspath__"):  # pragma: no cover
             return MPath(inp.__fspath__(), **kwargs)
         else:  # pragma: no cover
-            breakpoint()
             raise TypeError(f"cannot construct MPath object from {inp}")
 
     def to_dict(self) -> dict:
         return dict(
             path=self._path_str,
             storage_options=self._storage_options,
             fs=self.fs,
@@ -330,23 +329,28 @@
             Indicate whether Env is for a remote file.
 
         Returns
         -------
         dictionary
         """
         user_opts = {} if opts is None else dict(**opts)
+
+        # for remote paths, we need some special settings
         if self.is_remote():
             gdal_opts = GDAL_HTTP_OPTS.copy()
-            if self.suffix == ".vrt":
-                # we cannot know at this point which file types the VRT is pointing to,
-                # so in order to play safe, we remove the extensions constraint here
+
+            # we cannot know at this point which file types the VRT or STACTA JSON
+            # is pointing to, so in order to play safe, we remove the extensions constraint here
+            if self.suffix in (".vrt", ".json"):
                 try:
                     gdal_opts.pop("CPL_VSIL_CURL_ALLOWED_EXTENSIONS")
                 except KeyError:  # pragma: no cover
                     pass
+
+            # limit requests only to allowed extensions
             else:
                 default_remote_extensions = gdal_opts.get(
                     "CPL_VSIL_CURL_ALLOWED_EXTENSIONS", ""
                 ).split(", ")
                 if allowed_remote_extensions:
                     extensions = allowed_remote_extensions.split(",") + (
                         default_remote_extensions
@@ -354,21 +358,32 @@
                 extensions = default_remote_extensions + [self.suffix]
                 # make sure current path extension is added to allowed_remote_extensions
                 gdal_opts.update(
                     CPL_VSIL_CURL_ALLOWED_EXTENSIONS=", ".join(
                         set([ext for ext in extensions if ext != ""])
                     )
                 )
+
+            # secure HTTP credentials
             if self.fs.kwargs.get("auth"):
                 gdal_opts.update(
                     GDAL_HTTP_USERPWD=f"{self.fs.kwargs['auth'].login}:{self.fs.kwargs['auth'].password}"
                 )
+
+            # if a custom S3 endpoint is used, we need to deactivate these AWS options
+            if self._endpoint_url:
+                gdal_opts.update(AWS_VIRTUAL_HOSTING=False, AWS_HTTPS=False)
+
+            # merge everything with user options
             gdal_opts.update(user_opts)
+
+        # reading only locally, go with user options
         else:
             gdal_opts = user_opts
+
         logger.debug("using GDAL options: %s", gdal_opts)
         return gdal_opts
 
     @cached_property
     def _endpoint_url(self):
         # GDAL parses the paths in a weird way, so we have to be careful with a custom
         # endpoint
@@ -394,17 +409,15 @@
     def rio_env_config(self, opts=None, allowed_remote_extensions=None) -> dict:
         """Return configuration parameters for rasterio.Env()."""
         out = self.gdal_env_params(
             opts=opts,
             allowed_remote_extensions=allowed_remote_extensions,
         )
         if self.is_remote():
-            out.update(
-                session=self.rio_session(), AWS_VIRTUAL_HOSTING=False, AWS_HTTPS=False
-            )
+            out.update(session=self.rio_session())
         return out
 
     def rio_env(self, opts=None, allowed_remote_extensions=None) -> rasterio.Env:
         """Return preconfigured rasterio.Env context manager for path."""
         return rasterio.Env(
             **self.rio_env_config(
                 opts=opts, allowed_remote_extensions=allowed_remote_extensions
@@ -428,17 +441,15 @@
     def fio_env_config(self, opts=None, allowed_remote_extensions=None) -> dict:
         """Return configuration parameters for fiona.Env()."""
         out = self.gdal_env_params(
             opts=opts,
             allowed_remote_extensions=allowed_remote_extensions,
         )
         if self.is_remote():
-            out.update(
-                session=self.fio_session(), AWS_VIRTUAL_HOSTING=False, AWS_HTTPS=False
-            )
+            out.update(session=self.fio_session())
         return out
 
     def fio_env(self, opts=None, allowed_remote_extensions=None) -> fiona.Env:
         """Return preconfigured fiona.Env context manager for path."""
         return fiona.Env(
             **self.fio_env_config(
                 opts=opts, allowed_remote_extensions=allowed_remote_extensions
```

### Comparing `mapchete-2023.6.5/mapchete/stac.py` & `mapchete-2023.7.0/mapchete/stac.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/testing.py` & `mapchete-2023.7.0/mapchete/testing.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/tile.py` & `mapchete-2023.7.0/mapchete/tile.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/types.py` & `mapchete-2023.7.0/mapchete/types.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/validate.py` & `mapchete-2023.7.0/mapchete/validate.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/cli/options.py` & `mapchete-2023.7.0/mapchete/cli/options.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/cli/default/convert.py` & `mapchete-2023.7.0/mapchete/cli/default/convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/cli/default/cp.py` & `mapchete-2023.7.0/mapchete/cli/default/cp.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/cli/default/create.py` & `mapchete-2023.7.0/mapchete/cli/default/create.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/cli/default/execute.py` & `mapchete-2023.7.0/mapchete/cli/default/execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/cli/default/formats.py` & `mapchete-2023.7.0/mapchete/cli/default/formats.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/cli/default/index.py` & `mapchete-2023.7.0/mapchete/cli/default/index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/cli/default/processes.py` & `mapchete-2023.7.0/mapchete/cli/default/processes.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/cli/default/rm.py` & `mapchete-2023.7.0/mapchete/cli/default/rm.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/cli/default/serve.py` & `mapchete-2023.7.0/mapchete/cli/default/serve.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/cli/default/stac.py` & `mapchete-2023.7.0/mapchete/cli/default/stac.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/commands/_convert.py` & `mapchete-2023.7.0/mapchete/commands/_convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/commands/_cp.py` & `mapchete-2023.7.0/mapchete/commands/_cp.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/commands/_execute.py` & `mapchete-2023.7.0/mapchete/commands/_execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/commands/_index.py` & `mapchete-2023.7.0/mapchete/commands/_index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/commands/_rm.py` & `mapchete-2023.7.0/mapchete/commands/_rm.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/commons/clip.py` & `mapchete-2023.7.0/mapchete/commons/clip.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/commons/contours.py` & `mapchete-2023.7.0/mapchete/commons/contours.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/commons/hillshade.py` & `mapchete-2023.7.0/mapchete/commons/hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/formats/__init__.py` & `mapchete-2023.7.0/mapchete/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/formats/base.py` & `mapchete-2023.7.0/mapchete/formats/base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/formats/loaders.py` & `mapchete-2023.7.0/mapchete/formats/loaders.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/formats/tools.py` & `mapchete-2023.7.0/mapchete/formats/tools.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/formats/default/_fiona_base.py` & `mapchete-2023.7.0/mapchete/formats/default/_fiona_base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/formats/default/flatgeobuf.py` & `mapchete-2023.7.0/mapchete/formats/default/flatgeobuf.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/formats/default/geobuf.py` & `mapchete-2023.7.0/mapchete/formats/default/geobuf.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/formats/default/geojson.py` & `mapchete-2023.7.0/mapchete/formats/default/geojson.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/formats/default/gtiff.py` & `mapchete-2023.7.0/mapchete/formats/default/gtiff.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/formats/default/mapchete_input.py` & `mapchete-2023.7.0/mapchete/formats/default/mapchete_input.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/formats/default/png.py` & `mapchete-2023.7.0/mapchete/formats/default/png.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/formats/default/png_hillshade.py` & `mapchete-2023.7.0/mapchete/formats/default/png_hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/formats/default/raster_file.py` & `mapchete-2023.7.0/mapchete/formats/default/raster_file.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/formats/default/tile_directory.py` & `mapchete-2023.7.0/mapchete/formats/default/tile_directory.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/formats/default/vector_file.py` & `mapchete-2023.7.0/mapchete/formats/default/vector_file.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/io/__init__.py` & `mapchete-2023.7.0/mapchete/io/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/io/_geometry_operations.py` & `mapchete-2023.7.0/mapchete/io/_geometry_operations.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/io/_json.py` & `mapchete-2023.7.0/mapchete/io/_json.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/io/_misc.py` & `mapchete-2023.7.0/mapchete/io/_misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,10 +185,14 @@
     # create parent directories on local filesystems
     dst_path.parent.makedirs()
 
     # copy either within a filesystem or between filesystems
     if src_path.fs == dst_path.fs:
         src_path.fs.copy(str(src_path), str(dst_path))
     else:
+        # read source data first
         with src_path.open("rb") as src:
-            with dst_path.open("wb") as dst:
-                dst.write(src.read())
+            content = src.read()
+        # only write to destination if reading source data didn't raise errors,
+        # otherwise we can end up with empty objects on an object store
+        with dst_path.open("wb") as dst:
+            dst.write(content)
```

### Comparing `mapchete-2023.6.5/mapchete/io/raster.py` & `mapchete-2023.7.0/mapchete/io/raster.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/io/settings.py` & `mapchete-2023.7.0/mapchete/io/settings.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/io/vector.py` & `mapchete-2023.7.0/mapchete/io/vector.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/processes/__init__.py` & `mapchete-2023.7.0/mapchete/processes/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/processes/contours.py` & `mapchete-2023.7.0/mapchete/processes/contours.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/processes/convert.py` & `mapchete-2023.7.0/mapchete/processes/convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/processes/hillshade.py` & `mapchete-2023.7.0/mapchete/processes/hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/processes/examples/example_process.py` & `mapchete-2023.7.0/mapchete/processes/examples/example_process.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/static/index.html` & `mapchete-2023.7.0/mapchete/static/index.html`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/mapchete/static/process_template.py` & `mapchete-2023.7.0/mapchete/static/process_template.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/LICENSE` & `mapchete-2023.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/README.rst` & `mapchete-2023.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.5/pyproject.toml` & `mapchete-2023.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     "Flask-RangeRequest",
     "fsspec[http]",
     "fsspec[s3]",
     "geobuf",
     "lxml",
     "matplotlib",
     "protobuf<=3.20.1",
-    "pystac",
+    "pystac[urllib3]<=1.7.3",
     "requests",
     "rtree",
     "werkzeug>=0.15",
 ]
 contours = [
     "matplotlib",
 ]
@@ -87,15 +87,15 @@
     "Flask-RangeRequest",
     "werkzeug>=0.15",
 ]
 spatial-index = [
     "rtree",
 ]
 stac = [
-    "pystac",
+    "pystac[urllib3]<=1.7.3",
 ]
 vrt = [
     "lxml",
 ]
 
 [project.scripts]
 mapchete = "mapchete.cli.main:main"
```

### Comparing `mapchete-2023.6.5/PKG-INFO` & `mapchete-2023.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapchete
-Version: 2023.6.5
+Version: 2023.7.0
 Summary: Tile-based geodata processing using rasterio & Fiona
 Project-URL: Homepage, https://github.com/ungarj/mapchete
 Author-email: Joachim Ungar <joachim.ungar@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -41,15 +41,15 @@
 Requires-Dist: flask-rangerequest; extra == 'complete'
 Requires-Dist: fsspec[http]; extra == 'complete'
 Requires-Dist: fsspec[s3]; extra == 'complete'
 Requires-Dist: geobuf; extra == 'complete'
 Requires-Dist: lxml; extra == 'complete'
 Requires-Dist: matplotlib; extra == 'complete'
 Requires-Dist: protobuf<=3.20.1; extra == 'complete'
-Requires-Dist: pystac; extra == 'complete'
+Requires-Dist: pystac[urllib3]<=1.7.3; extra == 'complete'
 Requires-Dist: requests; extra == 'complete'
 Requires-Dist: rtree; extra == 'complete'
 Requires-Dist: werkzeug>=0.15; extra == 'complete'
 Provides-Extra: contours
 Requires-Dist: matplotlib; extra == 'contours'
 Provides-Extra: dask
 Requires-Dist: dask; extra == 'dask'
@@ -68,15 +68,15 @@
 Provides-Extra: serve
 Requires-Dist: flask; extra == 'serve'
 Requires-Dist: flask-rangerequest; extra == 'serve'
 Requires-Dist: werkzeug>=0.15; extra == 'serve'
 Provides-Extra: spatial-index
 Requires-Dist: rtree; extra == 'spatial-index'
 Provides-Extra: stac
-Requires-Dist: pystac; extra == 'stac'
+Requires-Dist: pystac[urllib3]<=1.7.3; extra == 'stac'
 Provides-Extra: vrt
 Requires-Dist: lxml; extra == 'vrt'
 Description-Content-Type: text/x-rst
 
 .. image:: logo/mapchete.svg
 
 Tile-based geodata processing.
```

