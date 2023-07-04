# Comparing `tmp/extrap-4.1.0.tar.gz` & `tmp/extrap-4.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrap-4.1.0.tar", last modified: Tue Jul  4 10:49:40 2023, max compression
+gzip compressed data, was "extrap-4.1.0a2.tar", last modified: Fri Jun 16 08:36:22 2023, max compression
```

## Comparing `extrap-4.1.0.tar` & `extrap-4.1.0a2.tar`

### file list

```diff
@@ -1,120 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:40.571534 extrap-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-04 10:49:30.000000 extrap-4.1.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-04 10:49:30.000000 extrap-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-07-04 10:49:40.567534 extrap-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-07-04 10:49:30.000000 extrap-4.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:40.559533 extrap-4.1.0/extrap/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:40.563533 extrap-4.1.0/extrap/entities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/entities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:40.563533 extrap-4.1.0/extrap/entities/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/entities/annotations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:40.563533 extrap-4.1.0/extrap/entities/annotations/comment_annotation/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/entities/annotations/comment_annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/entities/callpath.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/entities/calltree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/entities/coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/entities/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/entities/fraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/entities/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16659 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/entities/hypotheses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/entities/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/entities/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/entities/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/entities/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/entities/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/entities/terms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:40.563533 extrap-4.1.0/extrap/extrap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/extrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/extrap/extrapcmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/extrap/extrapgui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:40.563533 extrap-4.1.0/extrap/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/fileio/experiment_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:40.563533 extrap-4.1.0/extrap/fileio/file_reader/
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/fileio/file_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/fileio/file_reader/abstract_directory_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/fileio/file_reader/cube_file_reader2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21080 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/fileio/file_reader/extrap3_experiment_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/fileio/file_reader/json_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/fileio/file_reader/jsonlines_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/fileio/file_reader/talpas_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/fileio/file_reader/text_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/fileio/io_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/fileio/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:40.567534 extrap-4.1.0/extrap/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/AdvancedPlotWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/ColorWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9493 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/CubeFileReader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16933 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/DataDisplay.py
--rw-r--r--   0 runner    (1001) docker     (123)    37399 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/GraphWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/LogWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)    24689 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/MainWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/ModelerOptionsWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/ModelerWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/PlotTypeSelector.py
--rw-r--r--   0 runner    (1001) docker     (123)    14272 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/SelectorWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)    18609 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/TreeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/TreeView.py
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:40.567534 extrap-4.1.0/extrap/gui/components/
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/components/ExpanderWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/components/ParameterValueSlider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/components/ProgressWindow.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/components/annotation_delegate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/components/file_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/components/model_color_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/components/plot_formatting_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/components/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:40.567534 extrap-4.1.0/extrap/gui/plots/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/plots/AbstractPlotWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/plots/AllFunctionsAsDifferentSurfacePlotWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/plots/AllFunctionsAsOneSurfacePlotWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/plots/BaseGraphWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/plots/DominatingFunctionsAsHeatMapWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/plots/DominatingFunctionsAsSingleScatterPlotWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/plots/HeatMapGraphWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/plots/InterpolatedContourDisplayWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/plots/IsolinesDisplayWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/plots/MaxZAsSingleSurfacePlotWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/plots/MeasurementPointsPlotWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:40.567534 extrap-4.1.0/extrap/gui/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/gui/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:40.567534 extrap-4.1.0/extrap/modelers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/modelers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/modelers/abstract_modeler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/modelers/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/modelers/model_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/modelers/modeler_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:40.567534 extrap-4.1.0/extrap/modelers/multi_parameter/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/modelers/multi_parameter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/modelers/multi_parameter/multi_parameter_modeler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:40.567534 extrap-4.1.0/extrap/modelers/single_parameter/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/modelers/single_parameter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/modelers/single_parameter/abstract_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13494 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/modelers/single_parameter/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/modelers/single_parameter/refining.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:40.567534 extrap-4.1.0/extrap/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/util/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/util/classproperty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/util/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/util/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/util/extension_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/util/options_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/util/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/util/serialization_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-04 10:49:30.000000 extrap-4.1.0/extrap/util/unique_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:49:40.559533 extrap-4.1.0/extrap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-07-04 10:49:40.000000 extrap-4.1.0/extrap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-04 10:49:40.000000 extrap-4.1.0/extrap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:49:40.000000 extrap-4.1.0/extrap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-04 10:49:40.000000 extrap-4.1.0/extrap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-04 10:49:40.000000 extrap-4.1.0/extrap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 10:49:40.000000 extrap-4.1.0/extrap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 10:49:40.571534 extrap-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-04 10:49:30.000000 extrap-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.468173 extrap-4.1.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-16 08:36:08.000000 extrap-4.1.0a2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-16 08:36:08.000000 extrap-4.1.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-06-16 08:36:22.468173 extrap-4.1.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-06-16 08:36:08.000000 extrap-4.1.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.452173 extrap-4.1.0a2/extrap/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.460173 extrap-4.1.0a2/extrap/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.460173 extrap-4.1.0a2/extrap/entities/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/annotations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.460173 extrap-4.1.0a2/extrap/entities/annotations/comment_annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/annotations/comment_annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/callpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/calltree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/fraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16659 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/hypotheses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/terms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.460173 extrap-4.1.0a2/extrap/extrap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/extrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/extrap/extrapcmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/extrap/extrapgui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.460173 extrap-4.1.0a2/extrap/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/experiment_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.460173 extrap-4.1.0a2/extrap/fileio/file_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/file_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/file_reader/abstract_directory_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/file_reader/cube_file_reader2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21080 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/file_reader/extrap3_experiment_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/file_reader/json_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/file_reader/jsonlines_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/file_reader/talpas_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/file_reader/text_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/io_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.464173 extrap-4.1.0a2/extrap/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/AdvancedPlotWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/ColorWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9493 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/CubeFileReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17186 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/DataDisplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33974 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/GraphWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/LogWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/MainWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/ModelerOptionsWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/ModelerWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/PlotTypeSelector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14272 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/SelectorWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18096 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/TreeModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/TreeView.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.464173 extrap-4.1.0a2/extrap/gui/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/components/ExpanderWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/components/ParameterValueSlider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/components/ProgressWindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/components/annotation_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/components/file_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/components/model_color_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/components/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.464173 extrap-4.1.0a2/extrap/gui/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/plots/AllFunctionsAsDifferentSurfacePlotWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/plots/AllFunctionsAsOneSurfacePlotWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/plots/BaseGraphWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/plots/DominatingFunctionsAsHeatMapWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/plots/DominatingFunctionsAsSingleScatterPlotWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/plots/HeatMapGraphWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/plots/InterpolatedContourDisplayWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/plots/IsolinesDisplayWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/plots/MaxZAsSingleSurfacePlotWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/plots/MeasurementPointsPlotWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.464173 extrap-4.1.0a2/extrap/modelers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/modelers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/modelers/abstract_modeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/modelers/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/modelers/model_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/modelers/modeler_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.464173 extrap-4.1.0a2/extrap/modelers/multi_parameter/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/modelers/multi_parameter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/modelers/multi_parameter/multi_parameter_modeler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.464173 extrap-4.1.0a2/extrap/modelers/single_parameter/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/modelers/single_parameter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/modelers/single_parameter/abstract_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13494 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/modelers/single_parameter/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/modelers/single_parameter/refining.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.468173 extrap-4.1.0a2/extrap/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/util/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/util/classproperty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/util/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/util/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/util/extension_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/util/options_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/util/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/util/serialization_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/util/unique_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.456173 extrap-4.1.0a2/extrap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-06-16 08:36:22.000000 extrap-4.1.0a2/extrap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-16 08:36:22.000000 extrap-4.1.0a2/extrap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:36:22.000000 extrap-4.1.0a2/extrap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-16 08:36:22.000000 extrap-4.1.0a2/extrap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-16 08:36:22.000000 extrap-4.1.0a2/extrap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 08:36:22.000000 extrap-4.1.0a2/extrap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 08:36:22.468173 extrap-4.1.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-16 08:36:08.000000 extrap-4.1.0a2/setup.py
```

### Comparing `extrap-4.1.0/AUTHORS.md` & `extrap-4.1.0a2/AUTHORS.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # Extra-P Authors
 
 The following cumulative list contains the names (in alphabetical order) of all
 individuals who have contributed code to this repository:
 
 * Alexandru Calotoiu (calotoiu@cs.tu-darmstadt.de)
-* Alexander Geiß (alexander.geiss1@tu-darmstadt.de)
+* Alexander Geiß (geiss@cs.tu-darmstadt.de)
 * David Giessing (david.giessing93@gmail.com)
 * Marc-Andre Hermanns (m.a.hermanns@fz-juelich.de)
 * Jonas Klesy (jonas.klesy@googlemail.com)
 * Christof Jugel (christof.jugel@stud.tu-darmstadt.de)
 * Samuel Lokadjaja (samuel.lokadjaja@stud.tu-darmstadt.de)
 * Daniel Lorenz (lorenz@cs.tu-darmstadt.de
 * Benedikt Naumann (benedikt.naumann@gmx.de)
-* Jannis Neus (jannis.neus@stud.tu-darmstadt.de)
 * Nicolas Ollagnier (ncls_olg@yahoo.fr)
 * Marius Poke (m.poke@grs-sim.de)
 * Patrick Reisert (kpreisert@gmail.com)
 * Marcus Ritter (marcus.ritter@tu-darmstadt.de)
 * Niharika Sharma (niharika.sharma1908@gmail.com)
 * Moritz Vanderheyden (moritz.vanderheyden@stud.tu-darmstadt.de)
 * Johannes Wehrstein (johannes.wehrstein@gmx.de)
```

### Comparing `extrap-4.1.0/LICENSE` & `extrap-4.1.0a2/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2020-2023 Technical University of Darmstadt, Darmstadt, Germany
+Copyright (c) 2020-2021 Technical University of Darmstadt, Darmstadt, Germany
 
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
```

### Comparing `extrap-4.1.0/PKG-INFO` & `extrap-4.1.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrap
-Version: 4.1.0
+Version: 4.1.0a2
 Summary: Extra-P, automated performance modeling for HPC applications
 Home-page: https://github.com/extra-p/extrap
 Author: Extra-P project
 Author-email: extra-p@lists.parallel.informatik.tu-darmstadt.de
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `extrap-4.1.0/README.md` & `extrap-4.1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/entities/annotations/__init__.py` & `extrap-4.1.0a2/extrap/entities/annotations/__init__.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/entities/annotations/comment_annotation/__init__.py` & `extrap-4.1.0a2/extrap/entities/annotations/comment_annotation/__init__.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/entities/callpath.py` & `extrap-4.1.0a2/extrap/entities/callpath.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/entities/calltree.py` & `extrap-4.1.0a2/extrap/entities/calltree.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/entities/coordinate.py` & `extrap-4.1.0a2/extrap/entities/coordinate.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/entities/experiment.py` & `extrap-4.1.0a2/extrap/entities/experiment.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/entities/fraction.py` & `extrap-4.1.0a2/extrap/entities/fraction.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/entities/functions.py` & `extrap-4.1.0a2/extrap/entities/functions.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/entities/hypotheses.py` & `extrap-4.1.0a2/extrap/entities/hypotheses.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/entities/measurement.py` & `extrap-4.1.0a2/extrap/entities/measurement.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/entities/metric.py` & `extrap-4.1.0a2/extrap/entities/metric.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/entities/model.py` & `extrap-4.1.0a2/extrap/entities/model.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/entities/named_entity.py` & `extrap-4.1.0a2/extrap/entities/named_entity.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/entities/parameter.py` & `extrap-4.1.0a2/extrap/entities/parameter.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/entities/terms.py` & `extrap-4.1.0a2/extrap/entities/terms.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/extrap/extrapcmd.py` & `extrap-4.1.0a2/extrap/extrap/extrapcmd.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/extrap/extrapgui.py` & `extrap-4.1.0a2/extrap/extrap/extrapgui.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import argparse
 import logging
 import sys
 import threading
 import traceback
 import warnings
 
-from PySide6.QtCore import Qt, QCoreApplication
+from PySide6.QtCore import Qt
 from PySide6.QtGui import QPalette, QColor
 from PySide6.QtWidgets import QApplication, QMessageBox, QToolTip
 from matplotlib import font_manager
 
 import extrap
 from extrap.fileio.experiment_io import read_experiment
 from extrap.fileio.file_reader import all_readers
@@ -39,16 +39,14 @@
     if arguments.log_file:
         logging.basicConfig(format="%(levelname)s: %(asctime)s: %(message)s", level=log_level,
                             filename=arguments.log_file)
     else:
         logging.basicConfig(format="%(levelname)s: %(asctime)s: %(message)s", level=log_level)
     logging.getLogger().handlers[0].setLevel(logging.getLevelName(arguments.log_level.upper()))
 
-    QCoreApplication.setApplicationName(extrap.__title__)
-    QCoreApplication.setApplicationVersion(extrap.__version__)
     app = QApplication(sys.argv) if not test else QApplication.instance()
     apply_style(app)
 
     window = MainWidget()
 
     _init_warning_system(window, test)
 
@@ -169,41 +167,40 @@
             return _old_exception_handler(type, value, traceback_)
         _old_exception_handler(type, value, traceback_)
         if issubclass(type, RecoverableError):
             msg_box.open()
             activate_box(msg_box)
         else:
             activate_box(msg_box)
-            msg_box.exec()  # ensures waiting
+            msg_box.exec_()  # ensures waiting
             exit(1)
 
     warnings.showwarning = _warnings_handler
     sys.excepthook = _exception_handler
     warnings.simplefilter('always', UserWarning)
 
 
 def apply_style(app):
     app.setStyle('Fusion')
 
     palette = QPalette()
-    palette.setColor(QPalette.Window, QColor(200, 200, 200))
+    palette.setColor(QPalette.Window, QColor(190, 190, 190))
     palette.setColor(QPalette.WindowText, Qt.black)
     palette.setColor(QPalette.Base, QColor(220, 220, 220))
     palette.setColor(QPalette.AlternateBase, QColor(10, 10, 10))
     palette.setColor(QPalette.Text, Qt.black)
     palette.setColor(QPalette.Button, QColor(220, 220, 220))
     palette.setColor(QPalette.ButtonText, Qt.black)
     palette.setColor(QPalette.Highlight, QColor(31, 119, 180))
     palette.setColor(QPalette.HighlightedText, Qt.white)
     palette.setColor(QPalette.ToolTipBase, QColor(230, 230, 230))
     palette.setColor(QPalette.ToolTipText, Qt.black)
     palette.setColor(QPalette.Disabled, QPalette.Text, QColor(80, 80, 80))
     palette.setColor(QPalette.Disabled, QPalette.ButtonText, QColor(80, 80, 80))
     palette.setColor(QPalette.Disabled, QPalette.Button, QColor(150, 150, 150))
-    palette.setColor(QPalette.ColorRole.Link, QColor(21, 83, 123))
     app.setPalette(palette)
     QToolTip.setPalette(palette)
 
 
 def _preload_common_fonts():
     common_fonts = [
         font_manager.FontProperties('sans\\-serif:style=normal:variant=normal:weight=normal:stretch=normal:size=10.0'),
```

### Comparing `extrap-4.1.0/extrap/fileio/__init__.py` & `extrap-4.1.0a2/extrap/fileio/__init__.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/fileio/experiment_io.py` & `extrap-4.1.0a2/extrap/fileio/experiment_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2022, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import zipfile
 from pathlib import Path
 from typing import Union
```

### Comparing `extrap-4.1.0/extrap/fileio/file_reader/__init__.py` & `extrap-4.1.0a2/extrap/fileio/file_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/fileio/file_reader/abstract_directory_reader.py` & `extrap-4.1.0a2/extrap/fileio/file_reader/abstract_directory_reader.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/fileio/file_reader/cube_file_reader2.py` & `extrap-4.1.0a2/extrap/fileio/file_reader/cube_file_reader2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2022, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import logging
 import warnings
 from collections import defaultdict
```

### Comparing `extrap-4.1.0/extrap/fileio/file_reader/extrap3_experiment_reader.py` & `extrap-4.1.0a2/extrap/fileio/file_reader/extrap3_experiment_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2022, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import copy
 import logging
 import os
```

### Comparing `extrap-4.1.0/extrap/fileio/file_reader/json_file_reader.py` & `extrap-4.1.0a2/extrap/fileio/file_reader/json_file_reader.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/fileio/file_reader/jsonlines_file_reader.py` & `extrap-4.1.0a2/extrap/fileio/file_reader/jsonlines_file_reader.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/fileio/file_reader/talpas_file_reader.py` & `extrap-4.1.0a2/extrap/fileio/file_reader/talpas_file_reader.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/fileio/file_reader/text_file_reader.py` & `extrap-4.1.0a2/extrap/fileio/file_reader/text_file_reader.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/fileio/io_helper.py` & `extrap-4.1.0a2/extrap/fileio/io_helper.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/fileio/output.py` & `extrap-4.1.0a2/extrap/fileio/output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2022, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import re
 from typing import List, Tuple, Union, Sequence
```

### Comparing `extrap-4.1.0/extrap/gui/AdvancedPlotWidget.py` & `extrap-4.1.0a2/extrap/gui/AdvancedPlotWidget.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 from PySide6.QtWidgets import *  # @UnusedWildImport
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 
-from extrap.gui.plots.AbstractPlotWidget import AbstractPlotWidget
 
+#####################################################################
 
-class AdvancedPlotWidget(AbstractPlotWidget):
+
+class AdvancedPlotWidget(QWidget):
     """This class represents a Widget that is used to show the graph on
        the extrap window.
     """
 
     #####################################################################
 
     def __init__(self, main_widget, parent, graphDisplayWindowClass):
@@ -51,39 +52,55 @@
             self.max_y = maxValue
 
         else:
             print("[EXTRA-P:] Error: Set maximum for axis other than X-axis.")
 
     def getMaxX(self):
         """ 
-           This function returns the highest value of x that is being shown on x-axis.
+           This function returns the highest value of x that is being shown on x axis.
         """
         return self.max_x
 
+    def setMaxY(self, maxY):
+        """ This function sets the highest value of Y that is being shown on x axis.
+        """
+        self.max_y = maxY
+
     def getMaxY(self):
         """ 
-           This function returns the highest value of Y that is being shown on y-axis.
+           This function returns the highest value of Y that is being shown on x axis.
         """
         return self.max_y
 
+    def setFontSize(self, font_size):
+        """ This function sets the font size of the legend.
+        """
+        self.font_size = font_size
+
+    def getFontSize(self):
+        """ 
+           This function returns the font size of the legend.
+        """
+        return self.font_size
+
     def set_initial_value(self):
         """ 
           This function sets the initial value for different parameters required for graph.
         """
         # Basic geometry constants
         self.max_x = 10
         self.max_y = 10
         self.font_size = 6
 
     def drawGraph(self):
         """ 
             This function is being called by paintEvent to draw the graph 
         """
         # Get the font size as selected by the user and set it
-        self.font_size = int(self.main_widget.plot_formatting_options.font_size)
+        self.font_size = int(self.main_widget.getFontSize())
         # Call the 3D function display window
         if self.graphDisplayWindow is None:
             self.graphDisplayWindow = self.graphDisplayWindowClass(
                 self, self.main_widget, width=5, height=4, dpi=100)
             self.toolbar = MyCustomToolbar(self.graphDisplayWindow, self)
             self.grid.addWidget(self.graphDisplayWindow)
             self.grid.addWidget(self.toolbar)
```

### Comparing `extrap-4.1.0/extrap/gui/ColorWidget.py` & `extrap-4.1.0a2/extrap/gui/ColorWidget.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/gui/CubeFileReader.py` & `extrap-4.1.0a2/extrap/gui/CubeFileReader.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/gui/DataDisplay.py` & `extrap-4.1.0a2/extrap/gui/DataDisplay.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 
 from PySide6.QtCore import *  # @UnusedWildImport
 from PySide6.QtGui import *  # @UnusedWildImport
 from PySide6.QtWidgets import *  # @UnusedWildImport
 
 from extrap.entities.parameter import Parameter
 from extrap.gui.AdvancedPlotWidget import AdvancedPlotWidget
-from extrap.gui.GraphWidget import GraphWidget, GraphWrapperWidget
+from extrap.gui.GraphWidget import GraphWidget
 from extrap.gui.plots.AllFunctionsAsDifferentSurfacePlotWidget import AllFunctionsAsDifferentSurfacePlot
 from extrap.gui.plots.AllFunctionsAsOneSurfacePlotWidget import AllFunctionsAsOneSurfacePlot
 from extrap.gui.plots.DominatingFunctionsAsSingleScatterPlotWidget import DominatingFunctionsAsSingleScatterPlot
 from extrap.gui.plots.HeatMapGraphWidget import HeatMapGraph
 from extrap.gui.plots.InterpolatedContourDisplayWidget import InterpolatedContourDisplay
 from extrap.gui.plots.IsolinesDisplayWidget import IsolinesDisplay
 from extrap.gui.plots.MaxZAsSingleSurfacePlotWidget import MaxZAsSingleSurfacePlot
 from extrap.gui.plots.MeasurementPointsPlotWidget import MeasurementPointsPlot
-
 #####################################################################
 MIN_PARAM_VALUE = 0.01
 MAX_PARAM_VALUE = 2000000000
 
 
 class AxisSelection(QWidget):
     """ This class is a helper class for the class DataDisplay.
@@ -104,16 +103,19 @@
         """ This function should only be called from the connected event
             when the user has entered a new value.
             Otherwise use maxChanged() which does not update the graph drawing.
             This is to avoid multiple updates of the graph.
         """
         self.maxChanged()
         display = self.manager.display_widget.currentWidget()
-        display.drawGraph()
-        display.update()
+        if isinstance(display, GraphWidget):
+            display.update()
+        else:
+            display.drawGraph()
+            display.update()
 
     def maxChanged(self):
         """ This function updates the max value without redrawing the graph.
             Use this function from external calls to avoid multiple redraws
             of the graph.
         """
         if self.max_edit.value() == 0:
@@ -218,16 +220,19 @@
     @Slot(float)
     def _value_changed(self, value):
         if value == 0:
             self.value_edit.setValue(self.value_edit.minimum())
             return
         self.default_values[self.parameter] = value
         display = self.manager.display_widget.currentWidget()
-        display.drawGraph()
-        display.update()
+        if isinstance(display, GraphWidget):
+            display.update()
+        else:
+            display.drawGraph()
+            display.update()
 
     def setName(self, parameter):
         self.parameter = parameter.id
         self.parameter_name = parameter.name
         self.parameter_label.setText(self.parameter_name)
 
     def clearRowLayout(self):
@@ -274,15 +279,14 @@
         grid = QGridLayout(self)
 
         self.display_widget = QTabWidget(self)
         self.display_widget.setMovable(True)
         self.display_widget.setTabsClosable(True)
         self.display_widget.tabCloseRequested.connect(self.closeTab)
         grid.addWidget(self.display_widget, 0, 0)
-
         # loading this tab as default view (Line graph)
         self.reloadTabs([0])
 
         self.display_widget.tabsClosable()
         self.display_widget.currentChanged.connect(self.experimentChange)
         self.show()
 
@@ -308,15 +312,15 @@
         # 6: IsolinesDisplayWidget
         # 7: InterpolatedContourDisplayWidget
         # 8: Measurement Points
         if 0 in selectedCheckBoxesIndex:
             labelText = "Line graph"
             tabStatus = self.is_tab_already_opened(labelText)
             if tabStatus is False:
-                graph = GraphWrapperWidget(self.main_widget, self)
+                graph = GraphWidget(self.main_widget, self)
                 self.display_widget.addTab(graph, labelText)
 
         graph_widgets = {
             1: ('Single surface plot', AllFunctionsAsOneSurfacePlot),
             2: ('Surface plots', AllFunctionsAsDifferentSurfacePlot),
             3: ('Domination scatter plot', DominatingFunctionsAsSingleScatterPlot),
             4: ('Max. Z surface plot', MaxZAsSingleSurfacePlot),
@@ -386,17 +390,18 @@
                 self.updateWidget()
                 return
 
     def updateWidget(self):
         display = self.display_widget.currentWidget()
         if not display:
             return
-        display.drawGraph()
-
-
+        if isinstance(display, GraphWidget):
+            display.update()
+        else:
+            display.drawGraph()
 
 
 class GraphLimitsWidget(QWidget):
     def __init__(self, parent, data_display: DataDisplayManager):
         super().__init__(parent)
         self.data_display = data_display
         self.display_widget = data_display.display_widget
```

### Comparing `extrap-4.1.0/extrap/gui/GraphWidget.py` & `extrap-4.1.0a2/extrap/gui/GraphWidget.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,22 @@
 # Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 from __future__ import annotations
 
-import importlib.resources
 import math
 import typing
 
 import numpy
-from PySide6 import QtGui
 from PySide6.QtCore import *  # @UnusedWildImport
 from PySide6.QtGui import *  # @UnusedWildImport
 from PySide6.QtWidgets import *  # @UnusedWildImport
 
-from extrap.gui.plots.AbstractPlotWidget import AbstractPlotWidget
 from extrap.gui.Utils import formatFormula
 from extrap.gui.Utils import formatNumber
 
 if typing.TYPE_CHECKING:
     from extrap.gui.MainWidget import MainWidget
 
 
@@ -133,20 +130,25 @@
     def show_datapoints(self):
         return not self.combine_all_callpath and self.datapoints_type != ''
 
     @property
     def combine_all_callpath(self):
         return self.aggregate_callpath and len(self.main_widget.get_selected_call_tree_nodes()) > 1
 
-    def create_context_menu(self) -> typing.Optional[QMenu]:
+    @Slot(QPoint)
+    def showContextMenu(self, point):
+        """
+          This function takes care of different options and their visibility in the context menu.
+        """
+
         # selected_metric = self.main_widget.get_selected_metric()
         selected_callpaths = self.main_widget.get_selected_call_tree_nodes()
 
         if not selected_callpaths:
-            return None
+            return
 
         menu = QMenu(self)
         points_group = QActionGroup(self)
         points_group.setEnabled(not self.combine_all_callpath)
 
         data_point_selection = [
             # To show data points for mean values
@@ -193,27 +195,15 @@
         # Export
         menu.addSeparator()
         exportDataAction = menu.addAction("Export Data")
         exportDataAction.triggered.connect(self.exportData)
         screenshotAction = menu.addAction("Screenshot")
         screenshotAction.triggered.connect(self.screenshot)
 
-        return menu
-
-    @Slot(QPoint)
-    def showContextMenu(self, point):
-        """
-          This function takes care of different options and their visibility in the context menu.
-        """
-
-        menu = self.create_context_menu()
-        if not menu:
-            return
-
-        menu.exec(self.mapToGlobal(point))
+        menu.exec_(self.mapToGlobal(point))
 
     @Slot()
     def selectDataPoints(self):
         """
           This function hides all the datapoints that is being shown on graph.
         """
         self.datapoints_type = QObject.sender(self).data()
@@ -267,46 +257,34 @@
                                   formatFormula(
                                       model.hypothesis.function.to_string(*parameters))
 
             data_points_text = '\n'.join(
                 ('(' + str(x) + ', ' + str(y) + ')') for (x, y) in data_points)
             text += callpath_name + '\n' + data_points_text + '\n' + model_function_text + '\n\n'
 
-        msg = QDialog()
+        msg = QMessageBox(self)
+        msg.setIcon(QMessageBox.Information)
+        msg.setText(
+            "Exported data (text can be copied to the clipboard using the context menu):")
+        msg.setInformativeText(text)
         msg.setWindowTitle("Export Data")
-        msg.setFixedSize(600, 400)
-        layout = QGridLayout()
-        layout.addWidget(QLabel("Exported data (text can be copied to the clipboard using the context menu):"))
-
-        info_text = QTextEdit()
-        info_text.setTextInteractionFlags(
-            Qt.TextInteractionFlag.TextSelectableByMouse | Qt.TextInteractionFlag.TextSelectableByKeyboard)
-        info_text.setText(text)
-        layout.addWidget(info_text)
-
-        btn = QPushButton('OK', msg)
-        btn.setDefault(True)
-        btn.clicked.connect(msg.accept)
-        layout.addWidget(btn)
-        msg.setLayout(layout)
-        msg.exec()
+        # msg.setDetailedText("The details are as follows:")
+        msg.setStandardButtons(QMessageBox.Ok)
+        msg.exec_()
 
     def drawGraph(self, paint):
         """
             This function is being called by paintEvent to draw the graph
         """
 
         # Get data
         model_list, selected_call_nodes = self.main_widget.get_selected_models()
         if not model_list:
             return
 
-        plot_options = self.main_widget.plot_formatting_options
-        paint.setFont(QFont(plot_options.font_family, plot_options.font_size))
-
         # Calculate geometry constraints
         self.graph_width = self.frameGeometry().width() - self.left_margin - self.right_margin
         self.graph_height = self.frameGeometry().height() - self.top_margin - self.bottom_margin
         y = self.calculateMaxY(model_list) * 1.2
         self.max_y = y
 
         # Draw coordinate system
@@ -323,15 +301,14 @@
             # color = main_widget.model_color_map[selected_call_nodes[0]]
             self.drawAggregratedModel(paint, model_list)
 
         # Draw data points
         self.drawDataPoints(paint, model_list)
 
         # Draw legend
-        paint.setFont(QFont(plot_options.font_family, plot_options.legend_font_size))
         self.drawLegend(paint)
 
     def drawDataPoints(self, paint, selected_models):
         if self.show_datapoints is True:
             pen = QPen(self.DATA_POINT_COLOR)
             pen.setWidth(4)
             paint.setPen(pen)
@@ -342,85 +319,80 @@
 
                 else:
                     data_points = self.calculateDataPoints(selected_model)
                     self.plotPointsOnGraph(paint, data_points)
 
     def drawLegend(self, paint):
         # drawing the graph legend
-
+        px_between = 15
         widget = self.main_widget
         callpath_color_dict = widget.model_color_map
         dict_size = len(callpath_color_dict)
+        font_size = int(self.main_widget.getFontSize())
+        paint.setFont(QFont('Decorative', font_size))
         paint.setBrush(self.BACKGROUND_COLOR)
-        font_metrics = paint.fontMetrics()
         pen = QPen(self.TEXT_COLOR)
         pen.setWidth(1)
         paint.setPen(pen)
-
-        px_between = 2
-        font_height = font_metrics.height()
-        counter_increment = font_height + px_between
-        line_offset = font_height / 2
-        left_margin_text = self.legend_x + 45
+        counter_increment = font_size + 3
 
         if self.combine_all_callpath is False:
             text_len = 0
             for callpath, color in callpath_color_dict.items():
-                text_len = max(text_len, font_metrics.horizontalAdvance(callpath.name))
-            self.legend_width = 55 + text_len
-            self.legend_height = counter_increment * dict_size + 3 * px_between
+                text_len = max(text_len, len(callpath.name))
+            self.legend_width = 55 + text_len * (font_size - 1)
+            self.legend_height = counter_increment * dict_size + px_between
 
             paint.drawRect(self.legend_x,
                            self.legend_y,
                            self.legend_width,
                            self.legend_height)
-            counter = 2 * px_between
+            counter = 0
             for callpath, color in callpath_color_dict.items():
                 pen = QPen(QColor(color))
                 pen.setWidth(2)
                 paint.setPen(pen)
-                paint.drawLine(QPoint(self.legend_x + 5,
-                                      self.legend_y + counter + line_offset),
-                               QPoint(self.legend_x + 35,
-                                      self.legend_y + counter + line_offset))
+                paint.drawLine(self.legend_x + 5,
+                               self.legend_y + px_between + counter,
+                               self.legend_x + 35,
+                               self.legend_y + px_between + counter)
                 paint.setPen(self.TEXT_COLOR)
-                paint.drawText(QRect(left_margin_text, self.legend_y + counter,
-                                     text_len, font_height),
-                               Qt.TextFlag.TextDontClip, callpath.name)
-
+                paint.drawText(self.legend_x + 45,
+                               self.legend_y + px_between + counter,
+                               callpath.name)
                 counter = counter + counter_increment
 
         else:
+            text_len = 0
+            callpath_list = list()
 
-            aggregated_callpath_name = ' + '.join(callpath.name for callpath, color in callpath_color_dict.items())
-
-            bounding_rect_text = font_metrics.boundingRect(
-                QRect(left_margin_text, self.legend_y + 2 * px_between, self.graph_width - left_margin_text,
-                      self.graph_height - self.legend_y + 2 * px_between),
-                Qt.TextFlag.TextWordWrap | Qt.TextFlag.TextDontClip, aggregated_callpath_name)
-
-            text_len = bounding_rect_text.width()
-            self.legend_width = 55 + text_len
-
-            self.legend_height = bounding_rect_text.height() + 4 * px_between
+            for callpath, color in callpath_color_dict.items():
+                callpath_list.append(callpath.name)
+                text_len = max(text_len, text_len +
+                               len(callpath.name))
+
+            aggregated_callpath_name = str.join('+', callpath_list)
+            self.legend_width = 55 + text_len * (font_size - 1)
+            self.legend_height = counter_increment * 1 + px_between
 
             paint.drawRect(self.legend_x,
                            self.legend_y,
                            self.legend_width,
                            self.legend_height)
             pen = QPen(self.AGGREGATE_MODEL_COLOR)
             pen.setWidth(2)
             paint.setPen(pen)
             paint.drawLine(self.legend_x + 5,
-                           self.legend_y + 2 * px_between + line_offset,
+                           self.legend_y + px_between,
                            self.legend_x + 35,
-                           self.legend_y + 2 * px_between + line_offset)
+                           self.legend_y + px_between)
             paint.setPen(self.TEXT_COLOR)
-            paint.drawText(bounding_rect_text,
-                           Qt.TextFlag.TextWordWrap | Qt.TextFlag.TextDontClip, aggregated_callpath_name)
+            paint.drawText(self.legend_x + 45,
+                           self.legend_y + px_between,
+                           aggregated_callpath_name)
 
     def drawModel(self, paint, model, color):
         function = model.hypothesis.function
 
         cord_list = self.calculate_function(function, self.graph_width)
 
         pen = QPen(QColor(color))
@@ -870,64 +842,7 @@
     def mouseReleaseEvent(self, event):
         self.clicked_x_pos = None
         self.clicked_y_pos = None
 
     @staticmethod
     def getNumAxis():
         return 1
-
-
-class GraphWrapperWidget(AbstractPlotWidget):
-    _menu_icon_path = importlib.resources.path("extrap.gui.resources", "menu.svg").__enter__()
-
-    def setMax(self, axis, maxValue):
-        raise NotImplementedError("The assignment should happen in __init__")
-
-    def set_initial_value(self):
-        raise NotImplementedError("The assignment should happen in __init__")
-
-    @staticmethod
-    def getNumAxis():
-        return GraphWidget.getNumAxis()
-
-    def __init__(self, main_widget: MainWidget, parent):
-        super().__init__(parent)
-        grid = QGridLayout(self)
-        grid.setContentsMargins(0, 0, 0, 0)
-        grid.setSpacing(0)
-
-        self._main_widget = main_widget
-        self._graph_widget = GraphWidget(main_widget, self)
-        grid.addWidget(self._graph_widget, 0, 0)
-
-        self.setMax = self._graph_widget.setMax
-        self.set_initial_value = self._graph_widget.set_initial_value
-
-        self.context_menu_button = QToolButton(self)
-
-        self.context_menu_button.setIcon(QIcon(str(GraphWrapperWidget._menu_icon_path)))
-        self.context_menu_button.setText("Graph options")
-        self.context_menu_button.setEnabled(False)
-        self.context_menu_button.clicked.connect(self._context_menu_button_clicked)
-        button_layout = QVBoxLayout()
-        button_layout.setContentsMargins(15, 15, 15, 15)
-        button_layout.addWidget(self.context_menu_button)
-
-        grid.addLayout(button_layout, 0, 0, alignment=Qt.AlignLeft | Qt.AlignBottom)
-
-    def _context_menu_button_clicked(self):
-        if self._graph_widget:
-            menu = self._graph_widget.create_context_menu()
-            self.context_menu_button.setMenu(menu)
-            self.context_menu_button.showMenu()
-            self.context_menu_button.setMenu(None)
-            # button_pos = self.context_menu_button.pos()
-            # button_pos -= QPoint(0, self.context_menu_button.height())
-            # graph_widget.showContextMenu(button_pos)
-
-    def drawGraph(self):
-        model_list, selected_call_nodes = self._main_widget.get_selected_models()
-        if model_list:
-            self.context_menu_button.setEnabled(True)
-        else:
-            self.context_menu_button.setEnabled(False)
-        self._graph_widget.update()
```

### Comparing `extrap-4.1.0/extrap/gui/LogWidget.py` & `extrap-4.1.0a2/extrap/gui/LogWidget.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/gui/MainWidget.py` & `extrap-4.1.0a2/extrap/gui/MainWidget.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
 # Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
-import itertools
-import logging
 import signal
 import sys
-from urllib.error import URLError, HTTPError
 from enum import Enum
 from functools import partial
 from pathlib import Path
 from typing import Optional, Sequence, Tuple
 
-from PySide6 import QtGui
 from PySide6.QtCore import *  # @UnusedWildImport
 from PySide6.QtGui import *  # @UnusedWildImport
 from PySide6.QtWidgets import *  # @UnusedWildImport
 
 import extrap
 from extrap.entities.calltree import Node
 from extrap.entities.experiment import Experiment
@@ -33,19 +29,15 @@
 from extrap.gui.LogWidget import LogWidget
 from extrap.gui.ModelerWidget import ModelerWidget
 from extrap.gui.PlotTypeSelector import PlotTypeSelector
 from extrap.gui.components.ProgressWindow import ProgressWindow
 from extrap.gui.SelectorWidget import SelectorWidget
 from extrap.gui.components import file_dialog
 from extrap.gui.components.model_color_map import ModelColorMap
-from extrap.gui.components.plot_formatting_options import PlotFormattingOptions, PlotFormattingDialog
 from extrap.modelers.model_generator import ModelGenerator
-from extrap.util.deprecation import deprecated
-
-_SETTING_CHECK_FOR_UPDATES_ON_STARTUP = 'check_for_updates_on_startup'
 
 DEFAULT_MODEL_NAME = "Default Model"
 
 
 class CallPathEnum(Enum):
     constant = "constant"
     logarithmic = "logarithmic"
@@ -56,25 +48,20 @@
 class MainWidget(QMainWindow):
 
     def __init__(self, *args, **kwargs):
         """
         Initializes the extrap application widget.
         """
         super(MainWidget, self).__init__(*args, **kwargs)
-
-        self.settings = QSettings(QSettings.Scope.UserScope, "Extra-P", "Extra-P GUI")
-
-        status = self.settings.status()
-
         self.max_value = 0
         self.min_value = 0
         self.old_x_pos = 0
         self._experiment = None
         self.model_color_map = ModelColorMap()
-        self.plot_formatting_options = PlotFormattingOptions()
+        self.font_size = 6
         self.experiment_change = True
         self.initUI()
         signal.signal(signal.SIGINT, signal.SIG_DFL)
 
         # switch for using mean or median measurement values for modeling
         # is used when loading the data from a file and then modeling directly
         self.median = False
@@ -163,17 +150,17 @@
         save_experiment_action.setStatusTip('Saves experiment file')
         save_experiment_action.setShortcut(QKeySequence.Save)
         save_experiment_action.triggered.connect(self.save_experiment)
         save_experiment_action.setEnabled(False)
         self.save_experiment_action = save_experiment_action
 
         # View menu
-        change_font_action = QAction('Plot &formatting options', self)
-        change_font_action.setStatusTip('Change the formatting of the plots')
-        change_font_action.triggered.connect(self.open_plot_format_dialog_box)
+        change_font_action = QAction('Legend &font size', self)
+        change_font_action.setStatusTip('Change the legend font size')
+        change_font_action.triggered.connect(self.open_font_dialog_box)
 
         select_view_action = QAction('Select plot &type', self)
         select_view_action.setStatusTip('Select the plots you want to view')
         select_view_action.triggered.connect(self.open_select_plots_dialog_box)
 
         # Plots menu
         graphs = ['&Line graph', 'Selected models in same &surface plot', 'Selected models in &different surface plots',
@@ -257,41 +244,14 @@
         doc_action.triggered.connect(lambda: QDesktopServices.openUrl(QUrl(extrap.__documentation_link__)))
         help_menu.addAction(doc_action)
 
         about_action = QAction('&About', self)
         about_action.triggered.connect(self.show_about_dialog)
         help_menu.addAction(about_action)
 
-        if self.settings.value(_SETTING_CHECK_FOR_UPDATES_ON_STARTUP, True, bool):
-            update_available = None
-            try:
-                update_available = self.update_available()
-            except Exception as e:
-                logging.error("Check for updates: " + str(e))
-
-            if update_available:
-                update_menu = menubar.addMenu("UPDATE AVAILABLE")
-                update_action = QAction(
-                    f'Version {update_available[0]} is available here: {update_available[1]}',
-                    self)
-                update_action.triggered.connect(lambda: QDesktopServices.openUrl(QUrl(update_available[1])))
-                update_menu.addAction(update_action)
-
-                ignore_action = QAction("Ignore", self)
-                ignore_action.triggered.connect(lambda: update_menu.menuAction().setVisible(False))
-                update_menu.addAction(ignore_action)
-                update_menu.addSeparator()
-                auto_update_toggle = QAction(f'Check for updates on startup', self)
-                auto_update_toggle.setChecked(True)
-                auto_update_toggle.setCheckable(True)
-                update_menu.addAction(auto_update_toggle)
-                auto_update_toggle.toggled.connect(
-                    lambda toggled: self.settings.setValue(_SETTING_CHECK_FOR_UPDATES_ON_STARTUP,
-                                                           toggled))
-
         # Main window
         self.resize(1200, 800)
         self.setCentralWidget(central_widget)
         self.experiment_change = False
         self.show()
 
     def set_experiment(self, experiment, file_name="", *, compared=False):
@@ -322,15 +282,15 @@
         if not self.windowFilePath():
             event.accept()
             return
         msg_box = QMessageBox(QMessageBox.Question, 'Quit', "Are you sure to quit?",
                               QMessageBox.No | QMessageBox.Yes, self, Qt.Sheet)
         msg_box.setDefaultButton(QMessageBox.No)
 
-        if msg_box.exec() == QMessageBox.Yes:
+        if msg_box.exec_() == QMessageBox.Yes:
             event.accept()
         else:
             event.ignore()
 
     def getExperiment(self) -> Experiment:
         return self._experiment
 
@@ -342,17 +302,23 @@
 
     def get_current_model_gen(self) -> Optional[ModelGenerator]:
         return self.selector_widget.getCurrentModel()
 
     def get_selected_models(self) -> Tuple[Optional[Sequence[Model]], Optional[Sequence[Node]]]:
         return self.selector_widget.get_selected_models()
 
-    def open_plot_format_dialog_box(self):
-        dialog = PlotFormattingDialog(self.plot_formatting_options, self, Qt.Sheet)
-        if dialog.exec() == QDialog.DialogCode.Accepted:
+    def open_font_dialog_box(self):
+        fontSizeItems = list()
+        for i in range(4, 9, +1):
+            fontSizeItems.append(str(i))
+
+        fontSize, ok = QInputDialog.getItem(
+            self, "Font Size", "Select the font size:", fontSizeItems, 0, False, Qt.Sheet)
+        if ok:
+            self.font_size = fontSize
             self.data_display.updateWidget()
             self.update()
 
     def open_select_plots_dialog_box(self):
         dialog = PlotTypeSelector(self, self.data_display)
         dialog.setModal(True)
         dialog.open()
@@ -360,17 +326,16 @@
     # def hide_callpath_dialog_box(self):
     #     callpathList = list()
     #     for callpath in CallPathEnum:
     #         callpathList.append(callpath.value)
     #     answer,ok = QInputDialog.getItem(
     #         self, "Callpath Filter", "Select the call path to hide:", callpathList, 0, True)
 
-    @deprecated
     def getFontSize(self):
-        return self.plot_formatting_options.font_size
+        return self.font_size
 
     def screenshot(self, _checked=False, target=None, name_addition=""):
         """
         This function creates a screenshot of this or the target widget
         and stores it into a file. It opens a file dialog to
         specify the file name and type.
         """
@@ -441,104 +406,31 @@
         file_dialog.showSave(self, _save, 'Save Experiment', filter='Experiments (*.extra-p)')
 
     def open_cube_file(self):
         def _process_cube(dir_name):
             dialog = CubeFileReader(self, dir_name)
             dialog.setWindowFlag(Qt.Sheet, True)
             dialog.setModal(True)
-            dialog.exec()  # do not use open, wait for loading to finish
+            dialog.exec_()  # do not use open, wait for loading to finish
             if dialog.valid:
                 self.model_experiment(dialog.experiment, dir_name)
 
         file_dialog.showOpenDirectory(self, _process_cube, 'Select a Directory with a Set of CUBE Files')
 
     def updateMinMaxValue(self):
         if not self.experiment_change:
             self.color_widget.update_min_max(*self.selector_widget.update_min_max_value())
 
     def show_about_dialog(self):
-        about_dialog = QDialog(self)
-        about_dialog.setWindowTitle("About " + extrap.__title__)
-        layout = QGridLayout()
-        layout.setSpacing(4)
-        layout.setColumnStretch(0, 0)
-        layout.setColumnStretch(1, 0)
-        layout.setColumnStretch(2, 0)
-        layout.setColumnStretch(3, 1)
-
-        row = itertools.count(0)
-
-        columnSpan = 4
-        layout.addWidget(QLabel(f"<h1>{extrap.__title__}</h1>"), next(row), 0, 1, columnSpan)
-        layout.addWidget(QLabel(f"<b>{extrap.__description__}</b>"), next(row), 0, 1, columnSpan)
-        layout.addItem(QSpacerItem(0, 2), next(row), 0, 1, columnSpan)
-
-        icon_label = QLabel()
-        text_label = QLabel()
-        text_label.setOpenExternalLinks(True)
-        same_row = next(row)
-        layout.addWidget(icon_label, same_row, 0, 1, 1)
-        layout.addWidget(text_label, same_row, 1, 1, columnSpan - 1)
-        try:
-            update_available = self.update_available()
-            if not update_available:
-                icon_label.setPixmap(self.style().standardIcon(QStyle.StandardPixmap.SP_DialogApplyButton).pixmap(16))
-                text_label.setText(f"{extrap.__title__} is up to date")
-            else:
-                icon_label.setPixmap(
-                    self.style().standardIcon(QStyle.StandardPixmap.SP_MessageBoxInformation).pixmap(16))
-                text_label.setText(f'Version {update_available[0]} is available. '
-                                   f'Get it here: <a href="{update_available[1]}">{update_available[1]}</a>')
-        except HTTPError as e:
-            icon_label.setPixmap(self.style().standardIcon(QStyle.StandardPixmap.SP_MessageBoxWarning).pixmap(16))
-            text_label.setText(f"Could not check for updates: " + str(e))
-        except URLError as e:
-            icon_label.setPixmap(self.style().standardIcon(QStyle.StandardPixmap.SP_MessageBoxWarning).pixmap(16))
-            text_label.setText(f"Could not check for updates: " + str(e.reason))
-        except Exception as e:
-            icon_label.setPixmap(self.style().standardIcon(QStyle.StandardPixmap.SP_MessageBoxWarning).pixmap(16))
-            text_label.setText(f"Could not check for updates: " + str(e))
-
-        same_row = next(row)
-        layout.addWidget(QLabel(f"Version {extrap.__version__}"), same_row, 1, 1, 1)
-        layout.addWidget(QLabel(' — '), same_row, 2, 1, 1)
-
-        check_for_updates = QCheckBox(self)
-        check_for_updates.setChecked(self.settings.value(_SETTING_CHECK_FOR_UPDATES_ON_STARTUP, True, bool))
-        check_for_updates.setText("Check for updates on start up")
-        check_for_updates.toggled.connect(
-            lambda status: self.settings.setValue(_SETTING_CHECK_FOR_UPDATES_ON_STARTUP, status))
-        layout.addWidget(check_for_updates, same_row, 3, 1, 1)
-
-        layout.addItem(QSpacerItem(0, 2), next(row), 0, 1, columnSpan)
-
-        creators = QLabel(extrap.__developed_by_html__)
-        creators.setOpenExternalLinks(True)
-        layout.addWidget(creators, next(row), 0, 1, columnSpan)
-        layout.addItem(QSpacerItem(0, 2), next(row), 0, 1, columnSpan)
-        support = QLabel(f'Do you have questions or suggestions?<br>'
-                         f'Write us: <a href="mailto:{extrap.__support_email__}">{extrap.__support_email__}</a>')
-        support.setOpenExternalLinks(True)
-        layout.addWidget(support, next(row), 0, 1, columnSpan)
-
-        layout.addItem(QSpacerItem(0, 10), next(row), 0, 1, columnSpan)
-
-        layout.addWidget(QLabel(extrap.__copyright__), next(row), 0, 1, columnSpan)
-
-        layout.addItem(QSpacerItem(0, 10), next(row), 0, 1, columnSpan)
-
-        button_box = QDialogButtonBox(QDialogButtonBox.StandardButton.Ok)
-        button_box.accepted.connect(about_dialog.accept)
-
-        # button_box.addButton(check_for_updates, QDialogButtonBox.ButtonRole.ResetRole)
-        # ResetRole is a hack to achieve left alignment
-        layout.addWidget(button_box, next(row), 0, 1, columnSpan)
-        about_dialog.setLayout(layout)
-
-        about_dialog.open()
+        QMessageBox.about(self, "About " + extrap.__title__,
+                          f"""<h1>{extrap.__title__}</h1>
+<p>Version {extrap.__version__}</p>
+<p>{extrap.__description__}</p>
+<p>{extrap.__copyright__}</p>
+""")
 
     activate_event_handlers = []
 
     def event(self, e: QEvent) -> bool:
         if e.type() == QEvent.Type.WindowActivate:
             for h in self.activate_event_handlers:
                 h(e)
@@ -556,22 +448,7 @@
             ns_window.setTitlebarAppearsTransparent_(True)
             ns_window.setColorSpace_(NSColorSpace.sRGBColorSpace())
             c = self.palette().window().color()
             ns_window_color = NSColor.colorWithDeviceRed_green_blue_alpha_(c.redF(), c.greenF(), c.blueF(), c.alphaF())
             ns_window.setBackgroundColor_(ns_window_color)
         except ImportError:
             pass
-
-    @staticmethod
-    def update_available():
-        import json
-        import urllib.request
-        from packaging.version import Version
-
-        with urllib.request.urlopen(extrap.__current_version_api__) as response:
-            data = json.loads(response.read().decode('utf-8'))
-            info = data['info']
-
-            if Version(info['version']) > Version(extrap.__version__):
-                return info['version'], info['release_url']
-            else:
-                return False
```

### Comparing `extrap-4.1.0/extrap/gui/ModelerOptionsWidget.py` & `extrap-4.1.0a2/extrap/gui/ModelerOptionsWidget.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/gui/ModelerWidget.py` & `extrap-4.1.0a2/extrap/gui/ModelerWidget.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/gui/PlotTypeSelector.py` & `extrap-4.1.0a2/extrap/gui/PlotTypeSelector.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,44 +8,52 @@
 from PySide6.QtWidgets import *  # @UnusedWildImport
 
 
 class PlotTypeSelector(QDialog):
 
     def __init__(self, parent, dataDisplay):
         super(PlotTypeSelector, self).__init__(parent)
+        self.valid = False
         self.dataDisplay = dataDisplay
         self.init_UI()
 
     def init_UI(self):
         self.setWindowTitle("Select the Plots")
         self.setFixedWidth(350)
 
         plotTypes = ['Line graph', 'Selected models in same surface plot', 'Selected models in different surface plots',
                      'Dominating models in a 3D Scatter plot', 'Max z as a single surface plot',
-                     'Dominating models and max z as heat map', 'Selected models in contour plot',
+                     'Dominating models and max z as heat map', ' Selected models in contour plot',
                      'Selected models in interpolated contour plots', 'Measurement points']
 
-        layout = QVBoxLayout()
+        self.checkBoxes = [QCheckBox(plotType, self) for plotType in plotTypes]
 
-        self.checkBoxes = []
-        for plotType in plotTypes:
-            check_box = QCheckBox(plotType, self)
-            self.checkBoxes.append(check_box)
-            layout.addWidget(check_box)
-
-        dialog_buttons = QDialogButtonBox(QDialogButtonBox.Ok | QDialogButtonBox.Cancel, self)
-        dialog_buttons.accepted.connect(self.accept)
-        dialog_buttons.rejected.connect(self.reject)
-        layout.addWidget(dialog_buttons)
+        y_cord = 10
+        for checkBox in self.checkBoxes:
+            checkBox.move(10, y_cord)
+            y_cord = y_cord + 30
+
+        self.setFixedHeight(y_cord + 70)
+
+        ok_button = QPushButton(self)
+        ok_button.setText("OK")
+        ok_button.move(165, y_cord + 30)
+        ok_button.setFixedWidth(110)
+        ok_button.pressed.connect(self.ok_pressed)
+
+        cancel_button = QPushButton(self)
+        cancel_button.setText("Cancel")
+        cancel_button.move(40, y_cord + 30)
+        cancel_button.setFixedWidth(100)
+        cancel_button.pressed.connect(self.close)
 
-        self.setLayout(layout)
-
-    def accept(self):
+    def ok_pressed(self):
         numberOfCheckBox = len(self.checkBoxes)
         selectedCheckBoxesIndex = list()
 
         for count in range(0, numberOfCheckBox):
             if self.checkBoxes[count].isChecked():
                 selectedCheckBoxesIndex.append(count)
 
+        self.valid = True
+        self.close()
         self.dataDisplay.reloadTabs(selectedCheckBoxesIndex)
-        super().accept()
```

### Comparing `extrap-4.1.0/extrap/gui/SelectorWidget.py` & `extrap-4.1.0a2/extrap/gui/SelectorWidget.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/gui/TreeModel.py` & `extrap-4.1.0a2/extrap/gui/TreeModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,37 +40,27 @@
     def removeRows(self, position=0, count=1, parent=QModelIndex()):
         node = self._node_from_index(parent)
         self.beginRemoveRows(parent, position, position + count - 1)
         node.childItems.pop(position)
         self.endRemoveRows()
 
     def _node_from_index(self, index):
-        if not self.checkIndex(index):
-            raise IndexError()
-
         if index.isValid():
             return index.internalPointer()
         else:
             return self.root_item
 
     # noinspection PyMethodMayBeStatic
     def getValue(self, index) -> Optional[calltree.Node]:
-        if not self.checkIndex(index):
-            raise IndexError()
-
         item = index.internalPointer()
         if item is None:
             return None
         return item.data()
 
     def data(self, index, role=None):
-
-        if not self.checkIndex(index, QAbstractItemModel.CheckIndexOption.IndexIsValid):
-            raise IndexError()
-
         if not index.isValid():
             return None
 
         getDecorationBoxes = (role == Qt.DecorationRole and index.column() == 1)
         get_tooltip_annotations = (role == Qt.ToolTipRole and index.column() == 2)
 
         if role != Qt.DisplayRole and not (getDecorationBoxes or get_tooltip_annotations):
@@ -216,16 +206,14 @@
         #     if self.root_item.does_selection_change(selection_function):
         #         self.beginResetModel()
         #         self.root_item.calculate_selection(selection_function)
         #         self.endResetModel()
         #     self.valuesChanged()
 
     def flags(self, index):
-        if not self.checkIndex(index):
-            raise IndexError()
         if not index.isValid():
             return Qt.NoItemFlags
 
         return Qt.ItemIsEnabled | Qt.ItemIsSelectable
 
     def columnCount(self, _=None):
         return 8  # This needs to be updated when a new column is added!
@@ -249,71 +237,64 @@
             elif section == 6:
                 return "SMAPE"
             elif section == 7:
                 return "RE"
 
         return None
 
-    def index(self, row, column, parent=QModelIndex()):
-        if not self.checkIndex(parent):
-            raise IndexError()
-        if not parent.isValid():
-            parentItem = self.root_item
-        else:
-            parentItem = parent.internalPointer()
+    def index(self, row, column, parent=None):
 
         # print("In tree model # of rows",self.rowCount(parent))
         if row < 0 or column < 0 or row >= self.rowCount(parent) or column >= self.columnCount(parent):
             return QModelIndex()
 
+        if not parent.isValid():
+            parentItem = self.root_item
+        else:
+            parentItem = parent.internalPointer()
+
         childItem = parentItem.child(row)
         if childItem:
             return self.createIndex(row, column, childItem)
         else:
             return QModelIndex()
 
     def parent(self, index=...):
-        self.checkIndex(index, QAbstractItemModel.CheckIndexOption.DoNotUseParent)
-
         if not index.isValid():
             return QModelIndex()
 
         childItem: TreeItem = index.internalPointer()
-        if childItem == self.root_item:
+        if childItem is None:
             return QModelIndex()
-
         parentItem = childItem.parent()
+
         if parentItem == self.root_item:
             return QModelIndex()
         try:
             return self.createIndex(parentItem.row(), 0, parentItem)
         except ValueError:
             return QModelIndex()
 
     def rowCount(self, parent=None):
-        if parent is None:
-            parent = QModelIndex()
-
-        # if parent.column() > 0:
-        #     return 0
-        if not self.checkIndex(parent):
-            raise IndexError()
+        if parent.column() > 0:
+            return 0
 
         if not parent.isValid():
             parentItem = self.root_item
         else:
             parentItem = parent.internalPointer()
 
         return len(parentItem.child_items)
 
     def valuesChanged(self):
         if not self.main_widget.getExperiment():
             return
-
-        self.dataChanged.emit(QModelIndex(), QModelIndex())  # The whole tree changed its values
+        self.dataChanged.emit(self.createIndex(0, 0),
+                              self.createIndex(len(self.main_widget.getExperiment().callpaths) - 1,
+                                               self.columnCount(None) - 1))
 
 
 class TreeItem(object):
     def __init__(self, call_tree_node, parent=None):
         self.parent_item = parent
         self.call_tree_node: calltree.Node = call_tree_node
         self.child_items: List[TreeItem] = []
```

### Comparing `extrap-4.1.0/extrap/gui/TreeView.py` & `extrap-4.1.0a2/extrap/gui/TreeView.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
                 showDataPointsAction.triggered.connect(
                     lambda: self.showDataPoints(selectedModel))
                 copyModel = menu.addAction("Copy model")
                 copyModel.setDisabled(selectedModel is None)
                 copyModel.triggered.connect(
                     lambda: self.copy_model_to_clipboard(selectedModel)
                 )
-                menu.exec(self.mapToGlobal(event.pos()))
+                menu.exec_(self.mapToGlobal(event.pos()))
 
     def _create_expand_collapse_menu(self, model):
         expand_collapse_submenu = QMenu("Expand / Collapse")
         expandAction2 = expand_collapse_submenu.addAction("Expand all")
         expandAction2.triggered.connect(self.expandAll)
         expandSubtree = expand_collapse_submenu.addAction("Expand subtree")
         expandSubtree.triggered.connect(
@@ -140,15 +140,15 @@
             "Model has the following comments attached (text can be copied to the clipboard using the context menu):")
         allComments = '\n'.join(("– " + c.getMessage())
                                 for c in model.getComments())
         msg.setInformativeText(allComments)
         msg.setWindowTitle("Model Comments")
         # msg.setDetailedText("The details are as follows:")
         msg.setStandardButtons(QMessageBox.Ok)
-        msg.exec()
+        msg.exec_()
 
     # print the data points used in compute cost
     @staticmethod
     def showDataPoints(model):
         msgBox = QDialog()
         msgBox.setWindowTitle("Data Points")
         msgBox.setFixedSize(600, 400)
@@ -174,15 +174,15 @@
                 # print(str(ps[i])+","+str(actual_points[i]))
         else:
             msg_txt += "No data available."
 
         print(msg_txt)
         print("")
         msg.setText(msg_txt)
-        msgBox.exec()
+        msgBox.exec_()
 
     def dragEnterEvent(self, event: QDragEnterEvent) -> None:
         self._handle_drop_event(event)
 
     def dragMoveEvent(self, event: QDragMoveEvent) -> None:
         self._handle_drop_event(event)
```

### Comparing `extrap-4.1.0/extrap/gui/Utils.py` & `extrap-4.1.0a2/extrap/gui/Utils.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/gui/components/ExpanderWidget.py` & `extrap-4.1.0a2/extrap/gui/components/ExpanderWidget.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/gui/components/ParameterValueSlider.py` & `extrap-4.1.0a2/extrap/gui/components/ParameterValueSlider.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/gui/components/ProgressWindow.py` & `extrap-4.1.0a2/extrap/gui/components/ProgressWindow.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/gui/components/annotation_delegate.py` & `extrap-4.1.0a2/extrap/gui/components/annotation_delegate.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/gui/components/file_dialog.py` & `extrap-4.1.0a2/extrap/gui/components/file_dialog.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/gui/components/model_color_map.py` & `extrap-4.1.0a2/extrap/gui/components/model_color_map.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/gui/components/worker.py` & `extrap-4.1.0a2/extrap/gui/components/worker.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/gui/plots/AllFunctionsAsDifferentSurfacePlotWidget.py` & `extrap-4.1.0a2/extrap/gui/plots/AllFunctionsAsDifferentSurfacePlotWidget.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/gui/plots/AllFunctionsAsOneSurfacePlotWidget.py` & `extrap-4.1.0a2/extrap/gui/plots/AllFunctionsAsOneSurfacePlotWidget.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/gui/plots/BaseGraphWidget.py` & `extrap-4.1.0a2/extrap/gui/plots/BaseGraphWidget.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,18 +5,16 @@
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 from __future__ import annotations
 
 import warnings
 from abc import abstractmethod
-from itertools import chain
 from typing import TYPE_CHECKING
 
-import matplotlib
 import numpy as np
 from PySide6.QtWidgets import QSizePolicy
 from matplotlib import patches as mpatches
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from matplotlib.figure import Figure
 from mpl_toolkits.mplot3d import Axes3D
 
@@ -24,31 +22,33 @@
     from extrap.gui.MainWidget import MainWidget
 
 
 class GraphDisplayWindow(FigureCanvas):
     def __init__(self, graphWidget, main_widget: MainWidget, width=5, height=4, dpi=100):
         self.graphWidget = graphWidget
         self.main_widget = main_widget
-        with matplotlib.rc_context({'font.family': self.main_widget.plot_formatting_options.font_family,
-                                    'font.size': self.main_widget.plot_formatting_options.font_size}):
-            self.fig = Figure(figsize=(width, height), dpi=dpi, layout='tight')
-            super().__init__(self.fig)
-            super().setSizePolicy(QSizePolicy.Expanding,
-                                  QSizePolicy.Expanding)
-            super().updateGeometry()
-            self.draw_figure()
+        self.fig = Figure(figsize=(width, height), dpi=dpi)
+        super().__init__(self.fig)
+        super().setSizePolicy(QSizePolicy.Expanding,
+                              QSizePolicy.Expanding)
+        super().updateGeometry()
+        self.draw_figure()
+        with warnings.catch_warnings():
+            warnings.simplefilter('ignore')
+            self.fig.tight_layout()
 
     def redraw(self):
-        with matplotlib.rc_context({'font.family': self.main_widget.plot_formatting_options.font_family,
-                                    'font.size': self.main_widget.plot_formatting_options.font_size}):
-            rotation = self._save_rotation()
-            self.fig.clear()
-            self.draw_figure()
-            self._restore_rotation(rotation)
-            self.fig.canvas.draw_idle()
+        rotation = self._save_rotation()
+        self.fig.clear()
+        self.draw_figure()
+        with warnings.catch_warnings():
+            warnings.simplefilter('ignore')
+            self.fig.tight_layout()
+        self._restore_rotation(rotation)
+        self.fig.canvas.draw_idle()
 
     def _save_rotation(self):
         return [(ax.elev, ax.azim) if isinstance(ax, Axes3D) else (None, None) for ax in self.fig.axes]
 
     def _restore_rotation(self, rotations):
         for ax, (elev, azim) in zip(self.fig.axes, rotations):
             if isinstance(ax, Axes3D):
@@ -116,23 +116,24 @@
         np.seterr(**previous)
         for z, Z in zip(z_List, Z_List):
             z[np.isinf(z)] = max_z
             Z[np.isinf(Z)] = max_z
         return X, Y, Z_List, z_List
 
     def draw_legend(self, ax_all, dict_callpath_color):
+        fontSize = self.graphWidget.getFontSize()
         # draw legend
         patches = list()
         for key, value in dict_callpath_color.items():
             labelName = str(key.name)
             if labelName.startswith("_"):
                 labelName = labelName[1:]
             patch = mpatches.Patch(color=value, label=labelName)
             patches.append(patch)
-        leg = ax_all.legend(handles=patches, fontsize=self.main_widget.plot_formatting_options.legend_font_size,
+        leg = ax_all.legend(handles=patches, fontsize=fontSize,
                             loc="upper right", bbox_to_anchor=(1, 1))
         if leg:
             leg.set_draggable(True)
 
     def get_max(self, lower_max=2.0):
         # since we are drawing the plots with minimum axis value of 1 to avoid nan values,
         # so the first max-value of parameter could be 2 to calculate number of subdivisions
```

### Comparing `extrap-4.1.0/extrap/gui/plots/DominatingFunctionsAsHeatMapWidget.py` & `extrap-4.1.0a2/extrap/gui/plots/DominatingFunctionsAsHeatMapWidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         for (x, y, colour) in zip(X, Y, max_Color_List):
             ax1.scatter(x, y, c=colour)
 
         numOfCurves = 12
         maxZ = max([max(row) for row in max_Z_List])
         levels = np.arange(0, maxZ, (1 / float(numOfCurves)) * maxZ)
         CS = ax1.contour(X, Y, max_Z_List, levels=levels)
-        ax1.clabel(CS, CS.levels[::1], inline=True, fontsize=self.main_widget.plot_formatting_options.font_size * 0.8)
+        ax1.clabel(CS, CS.levels[::1], inline=True, fontsize=8)
 
         # legend
 
         patches = list()
         for key, value in dict_callpath_color.items():
             patch = mpatches.Patch(color=value, label=key)
             patches.append(patch)
```

### Comparing `extrap-4.1.0/extrap/gui/plots/DominatingFunctionsAsSingleScatterPlotWidget.py` & `extrap-4.1.0a2/extrap/gui/plots/DominatingFunctionsAsSingleScatterPlotWidget.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/gui/plots/HeatMapGraphWidget.py` & `extrap-4.1.0a2/extrap/gui/plots/HeatMapGraphWidget.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/gui/plots/InterpolatedContourDisplayWidget.py` & `extrap-4.1.0a2/extrap/gui/plots/InterpolatedContourDisplayWidget.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import warnings
 
 import matplotlib.ticker as ticker
@@ -32,15 +32,15 @@
 
         # Get data
         model_list, selected_callpaths = self.main_widget.get_selected_models()
         if model_list is None:
             return
 
         # Get font size for legend
-        font_size_legend = self.main_widget.plot_formatting_options.legend_font_size
+        fontSize = self.graphWidget.getFontSize()
 
         # Get max x and max y value as a initial default value or a value provided by user
         maxX, maxY = self.get_max()
 
         X, Y, Z_List, z_List = self.calculate_z_models(maxX, maxY, model_list)
 
         # Get the callpath color map
@@ -85,27 +85,28 @@
             CM = ax.pcolormesh(X, Y, Z_List[i], cmap=self.colormap)
             self.fig.colorbar(CM, ax=ax, orientation="horizontal",
                               pad=0.2, format=ticker.ScalarFormatter(useMathText=True))
             try:
                 with warnings.catch_warnings():
                     warnings.filterwarnings('ignore', 'No contour levels were found within the data range.')
                     CS = ax.contour(X, Y, Z_List[i], colors="white", levels=levels)
-                    ax.clabel(CS, CS.levels[::1], inline=True,
-                              fontsize=self.main_widget.plot_formatting_options.font_size * 0.8)
+                    ax.clabel(CS, CS.levels[::1], inline=True, fontsize=8)
             except ValueError:  # raised if function selected is constant
                 pass
             ax.set_xlabel('\n' + x_label)
             ax.set_ylabel('\n' + y_label)
 
             titleName = selected_callpaths[i].name
             if titleName.startswith("_"):
                 titleName = titleName[1:]
             ax.set_title(titleName)
+            for item in ([ax.xaxis.label, ax.yaxis.label]):
+                item.set_fontsize(10)
             for item in ([ax.title]):
-                item.set_fontsize(font_size_legend)
+                item.set_fontsize(fontSize)
 
     @staticmethod
     def getColorMap():
         colors = [(0, 0, 1), (0, 1, 0), (1, 0, 0)]
         n_bin = 100
         cmap_name = 'my_list'
         colorMap = LinearSegmentedColormap.from_list(
```

### Comparing `extrap-4.1.0/extrap/gui/plots/IsolinesDisplayWidget.py` & `extrap-4.1.0a2/extrap/gui/plots/IsolinesDisplayWidget.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import warnings
 
 from extrap.gui.plots.BaseGraphWidget import BaseContourGraph
@@ -28,82 +28,82 @@
             return
 
         # Get max x and max y value as a initial default value or a value provided by user
         maxX, maxY = self.get_max()
 
         X, Y, Z_List, z_List = self.calculate_z_models(maxX, maxY, model_list)
 
+        # Get the callpath color map
+        widget = self.main_widget
+        dict_callpath_color = widget.model_color_map
+        number_of_subplots = 1
+        if len(Z_List) > 1:
+            number_of_subplots = len(Z_List) + 1
+
+        # Adjusting subplots in order to avoid overlapping of labels
+        # Reference : https://stackoverflow.com/questions/2418125/matplotlib-subplots-adjust-hspace-so-titles-and-xlabels-dont-overlap
+        left = 0.1
+        right = 0.9
+        bottom = 0.2
+        top = 0.9
+        wspace = 0.5
+        hspace = 0.2
+        self.fig.subplots_adjust(
+            left=left, bottom=bottom, right=right, top=top, wspace=wspace, hspace=hspace)
+
         # Set the x_label and y_label based on parameter selected.
         x_label = self.main_widget.data_display.getAxisParameter(0).name
         if x_label.startswith("_"):
             x_label = x_label[1:]
         y_label = self.main_widget.data_display.getAxisParameter(1).name
         if y_label.startswith("_"):
             y_label = y_label[1:]
 
-        # Get the callpath color map
-        widget = self.main_widget
-        dict_callpath_color = widget.model_color_map
-        number_of_subplots = 1
-        if len(Z_List) > 1:
-            number_of_subplots = len(Z_List) + 1
-
-            # Adjusting subplots in order to avoid overlapping of labels
-            # Reference : https://stackoverflow.com/questions/2418125/matplotlib-subplots-adjust-hspace-so-titles-and-xlabels-dont-overlap
-            # left = 0.1
-            # right = 0.9
-            # bottom = 0.2
-            # top = 0.9
-            # wspace = 0.5
-            # hspace = 0.2
-            # self.fig.subplots_adjust(
-            #     left=left, bottom=bottom, right=right, top=top, wspace=wspace, hspace=hspace)
-
-            # Set the axis details for the subplot where we will draw all isolines
-            ax_all = self.fig.add_subplot(
-                1, number_of_subplots, number_of_subplots)
-            ax_all.xaxis.major.formatter._useMathText = True
-            ax_all.yaxis.major.formatter._useMathText = True
-            ax_all.set_xlabel('\n' + x_label)
-            ax_all.set_ylabel('\n' + y_label)
-            ax_all.set_title(r'All')
+        # Set the axis details for the subplot where we will draw all isolines
+        ax_all = self.fig.add_subplot(
+            1, number_of_subplots, number_of_subplots)
+        ax_all.xaxis.major.formatter._useMathText = True
+        ax_all.yaxis.major.formatter._useMathText = True
+        ax_all.set_xlabel('\n' + x_label)
+        ax_all.set_ylabel('\n' + y_label)
+        ax_all.set_title(r'All')
+        for item in ([ax_all.title, ax_all.xaxis.label, ax_all.yaxis.label]):
+            item.set_fontsize(10)
 
         # Draw isolines
         for i in range(len(Z_List)):
-            ax = self.fig.add_subplot(1, number_of_subplots, i + 1)
+            if i == 0:
+                ax = ax_all
+            else:
+                ax = self.fig.add_subplot(1, number_of_subplots, i + 1)
             ax.xaxis.major.formatter._useMathText = True
             ax.yaxis.major.formatter._useMathText = True
             try:
                 with warnings.catch_warnings():
                     warnings.filterwarnings('ignore', 'No contour levels were found within the data range.')
                     cs = ax.contour(X, Y, Z_List[i], colors=dict_callpath_color[selected_callpaths[i]])
-                    ax.clabel(cs, cs.levels[::2], inline=True,
-                              fontsize=self.main_widget.plot_formatting_options.font_size * 0.8)
+                    ax.clabel(cs, cs.levels[::2], inline=True, fontsize=7)
             except ValueError:  # raised if function selected is constant
                 pass
             ax.set_xlabel('\n' + x_label)
             ax.set_ylabel('\n' + y_label)
 
             # ax.set_title ('function'+ str(i+1))
-            ax.set_title(selected_callpaths[i].name,
-                         fontdict={'fontsize': self.main_widget.plot_formatting_options.legend_font_size})
-
+            # ax.set_title(functions[i])
             if len(Z_List) > 1:
                 try:
                     cs_all = ax_all.contour(
                         X, Y, Z_List[i], colors=dict_callpath_color[selected_callpaths[i]])
                     ax_all.clabel(
-                        cs_all, cs_all.levels[::2], inline=True,
-                        fontsize=self.main_widget.plot_formatting_options.font_size * 0.8)
+                        cs_all, cs_all.levels[::2], inline=True, fontsize=7)
                 except ValueError:  # raised if function selected is constant
                     pass
-            # self.fig.subplots_adjust(
-            #     left=left, bottom=bottom, right=right, top=top, wspace=wspace, hspace=hspace)
-            # for item in ([ax.title, ax.xaxis.label, ax.yaxis.label]):
-            #     item.set_fontsize(10)
+            self.fig.subplots_adjust(
+                left=left, bottom=bottom, right=right, top=top, wspace=wspace, hspace=hspace)
+            for item in ([ax.title, ax.xaxis.label, ax.yaxis.label]):
+                item.set_fontsize(10)
             # self.fig.colorbar(CS, ax=ax)
             # cax = ax.imshow(Z_List[i], interpolation='nearest', cmap=cm.coolwarm)
             # self.fig.colorbar(cax)
 
-        if len(Z_List) > 1:
-            # draw legend
-            self.draw_legend(ax_all, dict_callpath_color)
+        # draw legend
+        self.draw_legend(ax_all, dict_callpath_color)
```

### Comparing `extrap-4.1.0/extrap/gui/plots/MaxZAsSingleSurfacePlotWidget.py` & `extrap-4.1.0a2/extrap/gui/plots/MaxZAsSingleSurfacePlotWidget.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/gui/plots/MeasurementPointsPlotWidget.py` & `extrap-4.1.0a2/extrap/gui/plots/MeasurementPointsPlotWidget.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/modelers/abstract_modeler.py` & `extrap-4.1.0a2/extrap/modelers/abstract_modeler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2022, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import copy
 import logging
 import warnings
```

### Comparing `extrap-4.1.0/extrap/modelers/loader.py` & `extrap-4.1.0a2/extrap/modelers/loader.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/modelers/model_generator.py` & `extrap-4.1.0a2/extrap/modelers/model_generator.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/modelers/modeler_options.py` & `extrap-4.1.0a2/extrap/modelers/modeler_options.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/modelers/multi_parameter/__init__.py` & `extrap-4.1.0a2/extrap/modelers/multi_parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/modelers/multi_parameter/multi_parameter_modeler.py` & `extrap-4.1.0a2/extrap/modelers/multi_parameter/multi_parameter_modeler.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/modelers/single_parameter/__init__.py` & `extrap-4.1.0a2/extrap/modelers/single_parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/modelers/single_parameter/abstract_base.py` & `extrap-4.1.0a2/extrap/modelers/single_parameter/abstract_base.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/modelers/single_parameter/basic.py` & `extrap-4.1.0a2/extrap/modelers/single_parameter/basic.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/modelers/single_parameter/refining.py` & `extrap-4.1.0a2/extrap/modelers/single_parameter/refining.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/util/caching.py` & `extrap-4.1.0a2/extrap/util/caching.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/util/classproperty.py` & `extrap-4.1.0a2/extrap/util/classproperty.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/util/deprecation.py` & `extrap-4.1.0a2/extrap/util/deprecation.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/util/exceptions.py` & `extrap-4.1.0a2/extrap/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/util/extension_loader.py` & `extrap-4.1.0a2/extrap/util/extension_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import importlib
 import inspect
 import pkgutil
```

### Comparing `extrap-4.1.0/extrap/util/options_parser.py` & `extrap-4.1.0a2/extrap/util/options_parser.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/util/progress_bar.py` & `extrap-4.1.0a2/extrap/util/progress_bar.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/util/serialization_schema.py` & `extrap-4.1.0a2/extrap/util/serialization_schema.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap/util/unique_list.py` & `extrap-4.1.0a2/extrap/util/unique_list.py`

 * *Files identical despite different names*

### Comparing `extrap-4.1.0/extrap.egg-info/PKG-INFO` & `extrap-4.1.0a2/extrap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrap
-Version: 4.1.0
+Version: 4.1.0a2
 Summary: Extra-P, automated performance modeling for HPC applications
 Home-page: https://github.com/extra-p/extrap
 Author: Extra-P project
 Author-email: extra-p@lists.parallel.informatik.tu-darmstadt.de
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `extrap-4.1.0/extrap.egg-info/SOURCES.txt` & `extrap-4.1.0a2/extrap.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -59,29 +59,26 @@
 extrap/gui/components/ExpanderWidget.py
 extrap/gui/components/ParameterValueSlider.py
 extrap/gui/components/ProgressWindow.py
 extrap/gui/components/__init__.py
 extrap/gui/components/annotation_delegate.py
 extrap/gui/components/file_dialog.py
 extrap/gui/components/model_color_map.py
-extrap/gui/components/plot_formatting_options.py
 extrap/gui/components/worker.py
-extrap/gui/plots/AbstractPlotWidget.py
 extrap/gui/plots/AllFunctionsAsDifferentSurfacePlotWidget.py
 extrap/gui/plots/AllFunctionsAsOneSurfacePlotWidget.py
 extrap/gui/plots/BaseGraphWidget.py
 extrap/gui/plots/DominatingFunctionsAsHeatMapWidget.py
 extrap/gui/plots/DominatingFunctionsAsSingleScatterPlotWidget.py
 extrap/gui/plots/HeatMapGraphWidget.py
 extrap/gui/plots/InterpolatedContourDisplayWidget.py
 extrap/gui/plots/IsolinesDisplayWidget.py
 extrap/gui/plots/MaxZAsSingleSurfacePlotWidget.py
 extrap/gui/plots/MeasurementPointsPlotWidget.py
 extrap/gui/plots/__init__.py
-extrap/gui/resources/__init__.py
 extrap/modelers/__init__.py
 extrap/modelers/abstract_modeler.py
 extrap/modelers/loader.py
 extrap/modelers/model_generator.py
 extrap/modelers/modeler_options.py
 extrap/modelers/multi_parameter/__init__.py
 extrap/modelers/multi_parameter/multi_parameter_modeler.py
```

### Comparing `extrap-4.1.0/setup.py` & `extrap-4.1.0a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     python_requires='>=3.8',
     install_requires=[
         "pyside6~=6.4",
         "numpy~=1.18",
-        "matplotlib~=3.5",
+        "matplotlib~=3.4",
         "tqdm~=4.47",
         "pycubexr>=1.1,<3",
         "marshmallow~=3.7",
         "packaging~=20.0",
         "pyobjc-framework-Cocoa~=9.0; sys_platform == 'darwin'"
     ]
 )
```

