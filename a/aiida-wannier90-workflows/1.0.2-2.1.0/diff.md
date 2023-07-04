# Comparing `tmp/aiida-wannier90-workflows-1.0.2.tar.gz` & `tmp/aiida_wannier90_workflows-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-wannier90-workflows-1.0.2.tar", last modified: Wed Jul 13 20:14:36 2022, max compression
+gzip compressed data, was "aiida_wannier90_workflows-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida-wannier90-workflows-1.0.2.tar` & `aiida_wannier90_workflows-2.1.0.tar`

### file list

```diff
@@ -1,32 +1,80 @@
-drwxr-xr-x   0 junfeng   (1000) junfeng   (1000)        0 2022-07-13 20:14:36.656970 aiida-wannier90-workflows-1.0.2/
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)      558 2022-07-13 20:13:56.000000 aiida-wannier90-workflows-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)       86 2022-07-13 20:13:56.000000 aiida-wannier90-workflows-1.0.2/.style.yapf
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)     1072 2022-05-12 21:21:56.000000 aiida-wannier90-workflows-1.0.2/LICENSE
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)      219 2022-07-13 20:13:56.000000 aiida-wannier90-workflows-1.0.2/MANIFEST.in
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)      839 2022-07-13 20:14:36.656970 aiida-wannier90-workflows-1.0.2/PKG-INFO
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)     2382 2022-07-13 20:13:56.000000 aiida-wannier90-workflows-1.0.2/README.md
-drwxr-xr-x   0 junfeng   (1000) junfeng   (1000)        0 2022-07-13 20:14:36.653637 aiida-wannier90-workflows-1.0.2/aiida_wannier90_workflows/
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)      235 2022-07-13 20:13:56.000000 aiida-wannier90-workflows-1.0.2/aiida_wannier90_workflows/__init__.py
-drwxr-xr-x   0 junfeng   (1000) junfeng   (1000)        0 2022-07-13 20:14:36.656970 aiida-wannier90-workflows-1.0.2/aiida_wannier90_workflows/tools/
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)     2389 2022-07-13 20:13:56.000000 aiida-wannier90-workflows-1.0.2/aiida_wannier90_workflows/tools/get_w90model_from_aiida.py
-drwxr-xr-x   0 junfeng   (1000) junfeng   (1000)        0 2022-07-13 20:14:36.656970 aiida-wannier90-workflows-1.0.2/aiida_wannier90_workflows/workflows/
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)      315 2022-07-13 20:13:56.000000 aiida-wannier90-workflows-1.0.2/aiida_wannier90_workflows/workflows/__init__.py
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)     8092 2022-07-13 20:13:56.000000 aiida-wannier90-workflows-1.0.2/aiida_wannier90_workflows/workflows/band_structure.py
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)    30078 2022-07-13 20:13:56.000000 aiida-wannier90-workflows-1.0.2/aiida_wannier90_workflows/workflows/bands.py
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)    40410 2022-07-13 20:13:56.000000 aiida-wannier90-workflows-1.0.2/aiida_wannier90_workflows/workflows/wannier.py
-drwxr-xr-x   0 junfeng   (1000) junfeng   (1000)        0 2022-07-13 20:14:36.656970 aiida-wannier90-workflows-1.0.2/aiida_wannier90_workflows.egg-info/
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)      839 2022-07-13 20:14:36.000000 aiida-wannier90-workflows-1.0.2/aiida_wannier90_workflows.egg-info/PKG-INFO
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)      803 2022-07-13 20:14:36.000000 aiida-wannier90-workflows-1.0.2/aiida_wannier90_workflows.egg-info/SOURCES.txt
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)        1 2022-07-13 20:14:36.000000 aiida-wannier90-workflows-1.0.2/aiida_wannier90_workflows.egg-info/dependency_links.txt
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)      207 2022-07-13 20:14:36.000000 aiida-wannier90-workflows-1.0.2/aiida_wannier90_workflows.egg-info/entry_points.txt
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)       75 2022-07-13 20:14:36.000000 aiida-wannier90-workflows-1.0.2/aiida_wannier90_workflows.egg-info/requires.txt
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)       26 2022-07-13 20:14:36.000000 aiida-wannier90-workflows-1.0.2/aiida_wannier90_workflows.egg-info/top_level.txt
-drwxr-xr-x   0 junfeng   (1000) junfeng   (1000)        0 2022-07-13 20:14:36.656970 aiida-wannier90-workflows-1.0.2/examples/
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)      519 2022-07-13 20:13:56.000000 aiida-wannier90-workflows-1.0.2/examples/plot_wannier_centres.py
--rwxr-xr-x   0 junfeng   (1000) junfeng   (1000)     1358 2021-11-01 22:57:14.000000 aiida-wannier90-workflows-1.0.2/examples/run_workflow1.py
-drwxr-xr-x   0 junfeng   (1000) junfeng   (1000)        0 2022-07-13 20:14:36.656970 aiida-wannier90-workflows-1.0.2/examples/workflows/
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)      326 2022-07-13 20:13:56.000000 aiida-wannier90-workflows-1.0.2/examples/workflows/GaAs.xsf
--rwxr-xr-x   0 junfeng   (1000) junfeng   (1000)     5707 2022-07-13 20:13:56.000000 aiida-wannier90-workflows-1.0.2/examples/workflows/run_automated_wannier.py
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)       38 2022-07-13 20:14:36.656970 aiida-wannier90-workflows-1.0.2/setup.cfg
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)     1237 2022-07-13 20:13:56.000000 aiida-wannier90-workflows-1.0.2/setup.json
--rw-r--r--   0 junfeng   (1000) junfeng   (1000)      382 2022-07-13 20:13:56.000000 aiida-wannier90-workflows-1.0.2/setup.py
+-rw-r--r--   0        0        0     1072 2023-07-04 14:58:24.405382 aiida_wannier90_workflows-2.1.0/LICENSE
+-rw-r--r--   0        0        0     2440 2023-07-04 16:55:03.479390 aiida_wannier90_workflows-2.1.0/README.md
+-rw-r--r--   0        0        0     6218 2023-07-04 16:55:03.479390 aiida_wannier90_workflows-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/__init__.py
+-rw-r--r--   0        0        0     5395 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/calculations/split.py
+-rw-r--r--   0        0        0      278 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/cli/__init__.py
+-rw-r--r--   0        0        0     2665 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/cli/group.py
+-rw-r--r--   0        0        0     8439 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/cli/list.py
+-rw-r--r--   0        0        0    18836 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/cli/node.py
+-rw-r--r--   0        0        0     2787 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/cli/params.py
+-rw-r--r--   0        0        0    11254 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/cli/plot.py
+-rw-r--r--   0        0        0      492 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/cli/root.py
+-rw-r--r--   0        0        0     3160 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/cli/statistics.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/common/__init__.py
+-rw-r--r--   0        0        0     2216 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/common/types.py
+-rw-r--r--   0        0        0     3699 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/parsers/split.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/__init__.py
+-rw-r--r--   0        0        0     1727 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/bands/__init__.py
+-rw-r--r--   0        0        0     7987 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/bands/distance.py
+-rw-r--r--   0        0        0     1906 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/code.py
+-rw-r--r--   0        0        0     7777 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/kpoints.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/parser/__init__.py
+-rw-r--r--   0        0        0     1715 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/parser/bands.py
+-rw-r--r--   0        0        0    16349 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/parser/center.py
+-rw-r--r--   0        0        0     2069 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/parser/get_w90model_from_aiida.py
+-rw-r--r--   0        0        0     2393 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/parser/spread.py
+-rw-r--r--   0        0        0    12486 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/pseudo/__init__.py
+-rw-r--r--   0        0        0     7625 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/pseudo/data/__init__.py
+-rw-r--r--   0        0        0    10828 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/pseudo/data/dojo_nc_fr.json
+-rw-r--r--   0        0        0    18445 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/pseudo/data/pslibrary_paw_relpbe_1.0.0.json
+-rw-r--r--   0        0        0    16663 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/pseudo/data/semicore/PseudoDojo_0.4_LDA_SR_standard_upf.json
+-rw-r--r--   0        0        0    17221 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/pseudo/data/semicore/PseudoDojo_0.4_PBE_SR_standard_upf.json
+-rw-r--r--   0        0        0    23472 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/pseudo/data/semicore/SSSP_1.1_PBE_efficiency.json
+-rw-r--r--   0        0        0    23528 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/pseudo/data/semicore/SSSP_1.1_PBEsol_efficiency.json
+-rw-r--r--   0        0        0    15742 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/pseudo/upf.py
+-rw-r--r--   0        0        0     5886 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/scdm.py
+-rw-r--r--   0        0        0      700 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/str.py
+-rw-r--r--   0        0        0      503 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/structure.py
+-rw-r--r--   0        0        0      565 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/workflows/__init__.py
+-rw-r--r--   0        0        0     5100 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/workflows/bands.py
+-rw-r--r--   0        0        0     5714 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/workflows/builder/generator/__init__.py
+-rw-r--r--   0        0        0     4987 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/workflows/builder/generator/post.py
+-rw-r--r--   0        0        0     4238 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/workflows/builder/projections.py
+-rw-r--r--   0        0        0     5681 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/workflows/builder/serializer.py
+-rw-r--r--   0        0        0    18638 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/workflows/builder/setter.py
+-rw-r--r--   0        0        0     6262 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/workflows/builder/submit.py
+-rw-r--r--   0        0        0     2708 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/workflows/group.py
+-rwxr-xr-x   0        0        0    24517 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/workflows/plot/bands.py
+-rw-r--r--   0        0        0     7021 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/workflows/plot/checkerboard.py
+-rw-r--r--   0        0        0     8854 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/workflows/plot/distance.py
+-rw-r--r--   0        0        0     2283 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/workflows/pw.py
+-rw-r--r--   0        0        0      761 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/__init__.py
+-rw-r--r--   0        0        0    17791 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/bands.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/base/__init__.py
+-rw-r--r--   0        0        0     3244 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/base/open_grid.py
+-rw-r--r--   0        0        0     3683 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/base/projwfc.py
+-rw-r--r--   0        0        0    11458 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/base/pw2wannier90.py
+-rw-r--r--   0        0        0     7343 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/base/qebaserestart.py
+-rw-r--r--   0        0        0    33195 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/base/wannier90.py
+-rw-r--r--   0        0        0     9251 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/open_grid.py
+-rw-r--r--   0        0        0    31224 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/optimize.py
+-rw-r--r--   0        0        0     6638 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/projwfcbands.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/protocols/__init__.py
+-rw-r--r--   0        0        0      553 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/protocols/bands.yaml
+-rw-r--r--   0        0        0        0 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/protocols/base/__init__.py
+-rw-r--r--   0        0        0      670 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/protocols/base/open_grid.yaml
+-rw-r--r--   0        0        0      737 2023-07-04 14:58:24.429382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/protocols/base/projwfc.yaml
+-rw-r--r--   0        0        0      717 2023-07-04 14:58:24.433382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/protocols/base/pw2wannier90.yaml
+-rw-r--r--   0        0        0     1817 2023-07-04 14:58:24.433382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/protocols/base/wannier90.yaml
+-rw-r--r--   0        0        0      462 2023-07-04 14:58:24.433382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/protocols/open_grid.yaml
+-rw-r--r--   0        0        0      462 2023-07-04 14:58:24.433382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/protocols/optimize.yaml
+-rw-r--r--   0        0        0        0 2023-07-04 14:58:24.433382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/protocols/overrides/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:58:24.433382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/protocols/overrides/base/__init__.py
+-rw-r--r--   0        0        0      881 2023-07-04 14:58:24.433382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/protocols/overrides/wannier90.yaml
+-rw-r--r--   0        0        0      462 2023-07-04 14:58:24.433382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/protocols/projwfcbands.yaml
+-rw-r--r--   0        0        0      462 2023-07-04 14:58:24.433382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/protocols/split.yaml
+-rw-r--r--   0        0        0      462 2023-07-04 14:58:24.433382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/protocols/wannier90.yaml
+-rw-r--r--   0        0        0    35754 2023-07-04 14:58:24.433382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/split.py
+-rw-r--r--   0        0        0    41966 2023-07-04 14:58:24.433382 aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/wannier90.py
+-rw-r--r--   0        0        0     4659 1970-01-01 00:00:00.000000 aiida_wannier90_workflows-2.1.0/PKG-INFO
```

### Comparing `aiida-wannier90-workflows-1.0.2/LICENSE` & `aiida_wannier90_workflows-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida-wannier90-workflows-1.0.2/aiida_wannier90_workflows/tools/get_w90model_from_aiida.py` & `aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/utils/parser/get_w90model_from_aiida.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,54 @@
-import pythtb
-import tempfile
 import os
 import shutil
+import tempfile
+
+import pythtb
+
 from aiida_wannier90.parsers import raw_wout_parser
 
 
 def get_pythtb(wan_calculation, xyz_workaround=False):
     tmpdir = tempfile.mkdtemp()
 
     seedname = os.path.splitext(wan_calculation._INPUT_FILE)[0]
-    out_dir = os.path.join(
-        wan_calculation.out.retrieved.folder.abspath, "path"
-    )
+    out_dir = os.path.join(wan_calculation.out.retrieved.folder.abspath, "path")
     for filepath in [
-        os.path.join(
-            wan_calculation.folder.abspath, "raw_input",
-            "{}.win".format(seedname)
-        ),
-        os.path.join(out_dir, "{}.wout".format(seedname)),
-        os.path.join(out_dir, "{}_hr.dat".format(seedname)),
-        os.path.join(out_dir, "{}_wsvec.dat".format(seedname)),
-        os.path.join(out_dir, "{}_centres.xyz".format(seedname)),
-        os.path.join(out_dir, "{}_band.kpt".format(seedname)),
-        os.path.join(out_dir, "{}_band.dat".format(seedname)),
+        os.path.join(wan_calculation.folder.abspath, "raw_input", f"{seedname}.win"),
+        os.path.join(out_dir, f"{seedname}.wout"),
+        os.path.join(out_dir, f"{seedname}_hr.dat"),
+        os.path.join(out_dir, f"{seedname}_wsvec.dat"),
+        os.path.join(out_dir, f"{seedname}_centres.xyz"),
+        os.path.join(out_dir, f"{seedname}_band.kpt"),
+        os.path.join(out_dir, f"{seedname}_band.dat"),
     ]:
         if os.path.exists(filepath):
-            shutil.copy(
-                filepath, os.path.join(tmpdir, os.path.basename(filepath))
-            )
+            shutil.copy(filepath, os.path.join(tmpdir, os.path.basename(filepath)))
         else:
-            print("Skipping {}".format(os.path.basename(filepath)))
+            print(f"Skipping {os.path.basename(filepath)}")
 
     if xyz_workaround:
         parsed = raw_wout_parser(
-            open(os.path.join(out_dir, "{}.wout".format(seedname))).readlines()
+            open(os.path.join(out_dir, f"{seedname}.wout")).readlines()
         )
         num_atoms = len(wan_calculation.inp.structure.sites)
-        num_wf = len(parsed['wannier_functions_output'])
+        num_wf = len(parsed["wannier_functions_output"])
 
         xyz = []
         xyz.append(str(num_atoms + num_wf))
         xyz.append(str(num_atoms + num_wf))
-        for wf in parsed['wannier_functions_output']:
+        for wf in parsed["wannier_functions_output"]:
             xyz.append(
-                "X {} {} {}".format(
-                    wf['coordinates'][0], wf['coordinates'][1],
-                    wf['coordinates'][2]
-                )
+                f"X {wf['coordinates'][0]} {wf['coordinates'][1]} {wf['coordinates'][2]}"
             )
         for site in wan_calculation.inp.structure.sites:
             xyz.append(
-                "{} {} {} {}".format(
-                    site.kind_name, site.position[0], site.position[1],
-                    site.position[2]
-                )
+                f"{site.kind_name} {site.position[0]} {site.position[1]} {site.position[2]}"
             )
-        with open(
-            os.path.join(tmpdir, "{}_centres.xyz".format(seedname)), 'w'
-        ) as f:
+        with open(os.path.join(tmpdir, f"{seedname}_centres.xyz"), "w") as f:
             f.write("\n".join(xyz))
 
     tb_w90 = pythtb.w90(tmpdir, seedname)
     # Remove the folder
     shutil.rmtree(tmpdir)
 
     return tb_w90
```

### Comparing `aiida-wannier90-workflows-1.0.2/aiida_wannier90_workflows/workflows/bands.py` & `aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/base/wannier90.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,785 +1,771 @@
+"""Wrapper workchain for `Wannier90Calculation` to automatically handle several errors."""
+import pathlib
+import typing as ty
+
 from aiida import orm
 from aiida.common import AttributeDict
-from aiida.engine import WorkChain, ToContext
-from aiida.plugins import WorkflowFactory
+from aiida.common.lang import type_check
+from aiida.engine import (
+    BaseRestartWorkChain,
+    ProcessHandlerReport,
+    process_handler,
+    while_,
+)
+from aiida.engine.processes.builder import ProcessBuilder
+from aiida.orm.nodes.data.base import to_aiida_type
+
+from aiida_quantumespresso.common.types import ElectronicType, SpinType
+from aiida_quantumespresso.workflows.protocols.utils import ProtocolMixin
+
+from aiida_wannier90.calculations import Wannier90Calculation
+
+from aiida_wannier90_workflows.common.types import (
+    WannierDisentanglementType,
+    WannierFrozenType,
+    WannierProjectionType,
+)
+
+__all__ = ["validate_inputs_base", "validate_inputs", "Wannier90BaseWorkChain"]
+
+# pylint: disable=inconsistent-return-statements
+
+
+def validate_inputs_base(inputs: AttributeDict, ctx=None) -> None:
+    """Validate the inputs of the entire input namespace."""
+    # pylint: disable=inconsistent-return-statements,unused-argument
+
+    # Check `settings`
+    if "settings" in inputs:
+        settings = inputs["settings"].get_dict()
+        valid_keys = ("remote_symlink_files",)
+        for key in settings:
+            if key not in valid_keys:
+                return f"Invalid settings: `{key}`, valid keys are: {valid_keys}"
+
+
+def validate_inputs(inputs: AttributeDict, ctx=None) -> None:
+    """Validate the inputs of the entire input namespace."""
+    # pylint: disable=too-many-return-statements,unused-argument
+
+    result = validate_inputs_base(inputs, ctx)
+    if result:
+        return result
+
+    # pylint: disable=protected-access
+    calc_inputs = AttributeDict(inputs[Wannier90BaseWorkChain._inputs_namespace])
+    calc_parameters = calc_inputs.parameters.get_dict()
+
+    # Check existence of `fermi_energy`
+    if inputs["shift_energy_windows"]:
+        if "fermi_energy" not in calc_parameters:
+            return "`shift_energy_windows` is requested but no `fermi_energy` in input parameters"
+        if "bands" not in inputs:
+            return "`shift_energy_windows` is requested but no `bands` in inputs"
+
+    # Check `bands`
+    if any(_ in inputs for _ in ("bands", "bands_projections")) and all(
+        _ not in inputs for _ in ("shift_energy_windows", "auto_energy_windows")
+    ):
+        return (
+            "`bands` and/or `bands_projections` are provided but both `shift_energy_windows` "
+            "and `auto_energy_windows` are False?"
+        )
+
+    # Check `auto_energy_windows`
+    if inputs["auto_energy_windows"]:
+        if inputs["shift_energy_windows"]:
+            return "No need to shift energy windows when auto set energy windows"
+
+        if any(_ not in inputs for _ in ("bands_projections", "bands")):
+            return "`auto_energy_windows` is requested but `bands_projections` or `bands` is empty"
+
+        # Check bands and bands_projections are consistent
+        bands_num_kpoints, bands_num_bands = inputs["bands"].attributes["array|bands"]
+        projections_num_kpoints, projections_num_bands = inputs[
+            "bands_projections"
+        ].attributes["array|proj_array_0"]
+        if bands_num_kpoints != projections_num_kpoints:
+            return (
+                "`bands` and `bands_projections` have different number of kpoints: "
+                f"{bands_num_kpoints} != {projections_num_kpoints}"
+            )
+        if bands_num_bands != projections_num_bands:
+            return (
+                "`bands` and `bands_projections` have different number of bands: "
+                f"{bands_num_bands} != {projections_num_bands}"
+            )
+
 
-from aiida_quantumespresso.workflows.functions.seekpath_structure_analysis import seekpath_structure_analysis
-from aiida_quantumespresso.utils.protocols.pw import ProtocolManager
-from aiida_quantumespresso.utils.pseudopotential import get_pseudos_from_dict
-from .wannier import Wannier90WorkChain
+class Wannier90BaseWorkChain(ProtocolMixin, BaseRestartWorkChain):
+    """Workchain to run a `Wannier90Calculation` with automated error handling and restarts."""
 
+    _process_class = Wannier90Calculation
+    _inputs_namespace = "wannier90"
+
+    _WANNIER90_DEFAULT_KMESH_TOL = 1e-6
+    _WANNIER90_DEFAULT_DIS_PROJ_MIN = 0.1
+    _WANNIER90_DEFAULT_DIS_PROJ_MAX = 0.9
+    _WANNIER90_DEFAULT_WANNIER_PLOT_SUPERCELL = 2
 
-class Wannier90BandsWorkChain(WorkChain):
-    """
-    A high level workchain which can automatically compute a Wannier band structure for a given structure. Can also output Wannier Hamiltonian.
-    """
     @classmethod
-    def define(cls, spec):
-        """Define the process specification."""
-        super().define(spec)
-        # spec.input('vdw_table', valid_type=orm.SinglefileData, required=False)
-        spec.input(
-            'code.pw',
-            valid_type=orm.Code,
-            help='The `pw.x` code to use for the `PwCalculations`.'
-        )
-        spec.input(
-            'code.pw2wannier90',
-            valid_type=orm.Code,
-            help=
-            'The `pw2wannier90.x` code to use for the `Pw2WannierCalculations`.'
-        )
-        spec.input(
-            'code.wannier90',
-            valid_type=orm.Code,
-            help='The `wannier90.x` code to use for the `PwCalculations`.'
-        )
-        spec.input(
-            'code.projwfc',
-            valid_type=orm.Code,
-            required=False,
-            help='The `projwfc.x` code to use for the `PwCalculations`.'
-        )
-        spec.input(
-            'structure',
-            valid_type=orm.StructureData,
-            help='The input structure.'
-        )
-        spec.input(
-            'protocol',
-            valid_type=orm.Dict,
-            default=lambda: orm.Dict(dict={'name': 'theos-ht-1.0'}),
-            help='The protocol to use for the workchain.',
-            validator=validate_protocol
-        )
-        spec.input(
-            'controls.auto_projections',
-            valid_type=orm.Bool,
-            default=lambda: orm.Bool(True),
-            help=
-            'Whether using SCDM to automatically construct Wannier functions or not.'
-        )
-        spec.input(
-            'controls.only_valence',
-            valid_type=orm.Bool,
-            default=lambda: orm.Bool(False),
-            help='Group name that the calculations will be added to.'
-        )
-        spec.input(
-            'controls.retrieve_hamiltonian',
-            valid_type=orm.Bool,
-            default=lambda: orm.Bool(False),
-            help='Group name that the calculations will be added to.'
+    def define(cls, spec) -> None:
+        """Define the process spec."""
+        from aiida_wannier90.calculations.wannier90 import (
+            validate_inputs_base as validate_inputs_base_wannier90,
         )
+
+        super().define(spec)
+
+        spec.expose_inputs(Wannier90Calculation, namespace=cls._inputs_namespace)
+        spec.inputs[cls._inputs_namespace]["metadata"]["options"][
+            "resources"
+        ].default = {
+            "num_machines": 1,
+            # 'num_mpiprocs_per_machine': 1,
+        }
+
+        spec.inputs["wannier90"].validator = validate_inputs_base_wannier90
+
         spec.input(
-            'controls.plot_wannier_functions',
+            "shift_energy_windows",
             valid_type=orm.Bool,
             default=lambda: orm.Bool(False),
-            help='Group name that the calculations will be added to.'
+            serializer=to_aiida_type,
+            help=(
+                "If True the `dis_froz_min`, `dis_froz_max`, `dis_win_min`, `dis_win_max` will be shifted by "
+                "Fermi enerngy. False is the default behaviour of wannier90."
+            ),
         )
         spec.input(
-            'controls.do_disentanglement',
+            "auto_energy_windows",
             valid_type=orm.Bool,
             default=lambda: orm.Bool(False),
-            help=
-            'Used only if only_valence == False. Usually disentanglement worsens SCDM bands, keep it default to False.'
+            serializer=to_aiida_type,
+            help=(
+                "If True use the energy corresponding to projectability = auto_energy_windows_threshold "
+                "as `dis_froz_max` for wannier90."
+            ),
         )
         spec.input(
-            'controls.do_mlwf',
-            valid_type=orm.Bool,
-            default=lambda: orm.Bool(True),
-            help='Group name that the calculations will be added to.'
-        )
-        spec.input(
-            'controls.kpoints_distance_for_bands',
+            "auto_energy_windows_threshold",
             valid_type=orm.Float,
-            default=lambda: orm.Float(0.01),
-            help='Kpoint mesh density of the resulting band structure.'
-        )
-        # spec.input('controls.nbands_factor', valid_type=orm.Float, default=orm.Float(1.5),
-        # help='The number of bands for the NSCF calculation is that used for the SCF multiplied by this factor.')
-
-        spec.output(
-            'primitive_structure',
-            valid_type=orm.StructureData,
-            help=
-            'The normalized and primitivized structure for which the calculations are computed.'
-        )
-        spec.output(
-            'seekpath_parameters',
-            valid_type=orm.Dict,
-            help=
-            'The parameters used in the SeeKpath call to normalize the input or relaxed structure.'
-        )
-        spec.output(
-            'scf_parameters',
-            valid_type=orm.Dict,
-            help='The output parameters of the SCF `PwBaseWorkChain`.'
+            default=lambda: orm.Float(0.9),
+            serializer=to_aiida_type,
+            help="Threshold for auto_energy_windows.",
         )
-        spec.output(
-            'nscf_parameters',
-            valid_type=orm.Dict,
-            help='The output parameters of the NSCF `PwBaseWorkChain`.'
-        )
-        spec.output(
-            'projwfc_bands',
+        spec.input(
+            "bands",
             valid_type=orm.BandsData,
             required=False,
-            help='The output bands of projwfc run.'
+            help=(
+                "For shift_energy_windows, if provided the energy windows will be shifted by Fermi energy "
+                "for metals or minimum of lowest-unoccupied bands for insulators. "
+                "The bands should be along a kpath to better estimate the band gap. "
+                "For auto_energy_windows, the bands is used to find out the energy corresponds to "
+                "projectability = auto_energy_windows_threshold, the energy is used as `dis_froz_max`. "
+                "In this case the bands should be on a nscf kmesh."
+            ),
         )
-        spec.output(
-            'projwfc_projections',
+        spec.input(
+            "bands_projections",
             valid_type=orm.ProjectionData,
             required=False,
-            help='The output projections of projwfc run.'
+            help="Projectability of bands to auto set `dis_froz_max`.",
         )
-        spec.output(
-            'pw2wannier90_remote_folder',
-            valid_type=orm.RemoteData,
-            required=False
-        )
-        spec.output('wannier90_parameters', valid_type=orm.Dict)
-        spec.output('wannier90_retrieved', valid_type=orm.FolderData)
-        spec.output(
-            'wannier90_remote_folder',
-            valid_type=orm.RemoteData,
-            required=False
-        )
-        spec.output(
-            'wannier90_interpolated_bands',
-            valid_type=orm.BandsData,
+        spec.input(
+            "settings",
+            valid_type=orm.Dict,
             required=False,
-            help='The computed band structure.'
+            serializer=to_aiida_type,
+            help="Additional settings.",
         )
+        spec.inputs.validator = validate_inputs
 
         spec.outline(
-            cls.setup, cls.run_seekpath, cls.setup_parameters,
-            cls.run_wannier_workchain, cls.results
+            cls.setup,
+            while_(cls.should_run_process)(
+                cls.run_process,
+                cls.inspect_process,
+            ),
+            cls.results,
         )
 
+        spec.expose_outputs(Wannier90Calculation)
+
+        spec.exit_code(401, "ERROR_BVECTORS", message="Unrecoverable bvectors error.")
         spec.exit_code(
-            201,
-            'ERROR_INVALID_INPUT_UNRECOGNIZED_KIND',
-            message='Input `StructureData` contains an unsupported kind.'
+            402,
+            "ERROR_DISENTANGLEMENT_NOT_ENOUGH_STATES",
+            message="Unrecoverable disentanglement error.",
         )
         spec.exit_code(
-            401,
-            'ERROR_SUB_PROCESS_FAILED_BANDS',
-            message='The `PwBandsWorkChain` sub process failed.'
+            403, "ERROR_PLOT_WF_CUBE", message="Unrecoverable cube format error."
+        )
+        spec.exit_code(
+            404,
+            "ERROR_OUTPUT_STDOUT_INCOMPLETE",
+            message="The stdout output file was incomplete probably because the calculation got interrupted.",
         )
 
-    def _get_protocol(self):
-        """Return a `ProtocolManager` instance and a dictionary of modifiers."""
-        protocol_data = self.inputs.protocol.get_dict()
-        protocol_name = protocol_data['name']
-        protocol = ProtocolManager(protocol_name)
-
-        protocol_modifiers = protocol_data.get('modifiers', {})
+    @classmethod
+    def get_protocol_filepath(cls) -> pathlib.Path:
+        """Return the ``pathlib.Path`` to the ``.yaml`` file that defines the protocols."""
+        from importlib_resources import files
 
-        return protocol, protocol_modifiers
+        from .. import protocols
 
-    def setup_protocol(self):
-        """Set up context variables and inputs for the `PwBandsWorkChain`.
+        return files(protocols) / "base" / "wannier90.yaml"
 
-        Based on the specified protocol, we define values for variables that affect the execution of the calculations.
+    @classmethod
+    def get_builder_from_protocol(
+        cls,
+        code: ty.Union[orm.Code, str, int],
+        *,
+        structure: orm.StructureData,
+        protocol: str = None,
+        overrides: dict = None,
+        pseudo_family: str = None,
+        electronic_type: ElectronicType = ElectronicType.METAL,
+        spin_type: SpinType = SpinType.NONE,
+        projection_type: WannierProjectionType = WannierProjectionType.ATOMIC_PROJECTORS_QE,
+        disentanglement_type: WannierDisentanglementType = WannierDisentanglementType.SMV,
+        frozen_type: WannierFrozenType = WannierFrozenType.FIXED_PLUS_PROJECTABILITY,
+    ) -> ProcessBuilder:
+        """Return a builder prepopulated with inputs selected according to the chosen protocol.
+
+        :param code: [description]
+        :type code: ty.Union[orm.Code, str, int]
+        :param structure: [description]
+        :type structure: orm.StructureData
+        :param protocol: [description], defaults to None
+        :type protocol: str, optional
+        :param overrides: [description], defaults to None
+        :type overrides: dict, optional
+        :return: [description]
+        :rtype: ProcessBuilder
         """
-        protocol, protocol_modifiers = self._get_protocol()
-        self.report(
-            'running the workchain with the "{}" protocol'.format(
-                protocol.name
+        # pylint: disable=too-many-statements,too-many-locals,too-many-branches
+        from aiida_quantumespresso.workflows.protocols.utils import recursive_merge
+
+        from aiida_wannier90_workflows.utils.kpoints import (
+            create_kpoints_from_distance,
+            get_explicit_kpoints,
+        )
+        from aiida_wannier90_workflows.utils.pseudo import (
+            get_number_of_projections,
+            get_pseudo_and_cutoff,
+            get_pseudo_orbitals,
+            get_semicore_list,
+            get_wannier_number_of_bands,
+        )
+
+        if isinstance(code, (int, str)):
+            code = orm.load_code(code)
+
+        type_check(code, orm.Code)
+        type_check(structure, orm.StructureData)
+        type_check(electronic_type, ElectronicType)
+        type_check(spin_type, SpinType)
+        type_check(projection_type, WannierProjectionType)
+        type_check(disentanglement_type, WannierDisentanglementType)
+        type_check(frozen_type, WannierFrozenType)
+
+        if electronic_type in [ElectronicType.AUTOMATIC]:
+            raise NotImplementedError("`ElectronicType.AUTOMATIC` not implemented")
+
+        if spin_type == SpinType.COLLINEAR:
+            raise NotImplementedError("`SpinType.COLLINEAR` not implemented")
+        if spin_type == SpinType.SPIN_ORBIT and pseudo_family is None:
+            raise ValueError(
+                "Need to explicitly specify `pseudo_family` for SOC calculation"
             )
-        )
-        self.ctx.protocol = protocol.get_protocol_data(
-            modifiers=protocol_modifiers
-        )
-        # self.report('protocol: ' + str(self.ctx.protocol))
 
-    def setup(self):
+        inputs = cls.get_protocol_inputs(protocol, overrides)
 
-        self.setup_protocol()
-        try:
-            controls = self.inputs.controls
-            if controls.only_valence:
-                valence_info = "valence bands only"
-            else:
-                valence_info = "valence + conduction bands"
-            self.report('workchain controls found in inputs: ' + valence_info)
-        except AttributeError:
-            controls = {}
-        controls = AttributeDict(controls)
-        # try:
-        #     controls.group_name
-        # except AttributeError:
-        #     self.ctx.group_name = self._DEFAULT_CONTROLS_GROUP_NAME
-        # else:
-        #     self.ctx.group_name = controls.group_name
+        # Update the parameters based on the protocol inputs
+        parameters = inputs[cls._inputs_namespace]["parameters"]
+        metadata = inputs[cls._inputs_namespace]["metadata"]
+
+        meta_parameters = inputs.pop("meta_parameters")
+        num_atoms = len(structure.sites)
+        parameters["conv_tol"] = num_atoms * meta_parameters["conv_tol_per_atom"]
+        parameters["dis_conv_tol"] = (
+            num_atoms * meta_parameters["dis_conv_tol_per_atom"]
+        )
+
+        # Set `num_bands`, `num_wann`, also take care of semicore states
+        only_valence = electronic_type == ElectronicType.INSULATOR
+        spin_polarized = spin_type == SpinType.COLLINEAR
+        spin_orbit_coupling = spin_type == SpinType.SPIN_ORBIT
+
+        if pseudo_family is None:
+            pseudo_family = meta_parameters["pseudo_family"]
+        pseudos, _, _ = get_pseudo_and_cutoff(pseudo_family, structure)
+
+        num_bands = get_wannier_number_of_bands(
+            structure=structure,
+            pseudos=pseudos,
+            factor=meta_parameters["num_bands_factor"],
+            only_valence=only_valence,
+            spin_polarized=spin_polarized,
+            spin_orbit_coupling=spin_orbit_coupling,
+        )
+        num_projs = get_number_of_projections(
+            structure=structure,
+            pseudos=pseudos,
+            spin_orbit_coupling=spin_orbit_coupling,
+        )
 
-    def run_seekpath(self):
-        """Run the structure through SeeKpath to get the primitive and normalized structure.
-        """
-        kpoints_distance_for_bands = self.inputs.controls.get(
-            'kpoints_distance_for_bands',
-            self.ctx.protocol['kpoints_distance_for_bands']
-        )
-        seekpath_parameters = orm.Dict(
-            dict={'reference_distance': kpoints_distance_for_bands}
-        )
-        structure_formula = self.inputs.structure.get_formula()
-        self.report(
-            'running seekpath to get primitive structure for: {}'.
-            format(structure_formula)
-        )
-        result = seekpath_structure_analysis(
-            self.inputs.structure, seekpath_parameters
-        )
-        self.ctx.current_structure = result['primitive_structure']
-        self.ctx.explicit_kpoints_path = result['explicit_kpoints']
-        # save kpoint_path for bands_plot
-        self.ctx.kpoints_path = {
-            'path': result['parameters']['path'],
-            'point_coords': result['parameters']['point_coords']
-        }
+        if electronic_type == ElectronicType.INSULATOR:
+            num_wann = num_bands
+        else:
+            num_wann = num_projs
 
-        self.out('primitive_structure', result['primitive_structure'])
-        self.out('seekpath_parameters', result['parameters'])
+        if meta_parameters["exclude_semicore"]:
+            pseudo_orbitals = get_pseudo_orbitals(pseudos)
+            semicore_list = get_semicore_list(structure, pseudo_orbitals)
+            num_excludes = len(semicore_list)
+            # TODO I assume all the semicore bands are the lowest  # pylint: disable=fixme
+            exclude_pswfcs = range(1, num_excludes + 1)
+            if num_excludes != 0:
+                parameters["exclude_bands"] = exclude_pswfcs
+                num_wann -= num_excludes
+                num_bands -= num_excludes
+
+        if num_wann <= 0:
+            raise ValueError(f"Wrong num_wann {num_wann}")
+        parameters["num_wann"] = num_wann
+        parameters["num_bands"] = num_bands
+
+        # Spinor
+        if spin_type in [SpinType.NON_COLLINEAR, SpinType.SPIN_ORBIT]:
+            parameters["spinors"] = True
+
+        # Set initial projections
+        if projection_type in [
+            WannierProjectionType.SCDM,
+            WannierProjectionType.ATOMIC_PROJECTORS_QE,
+            WannierProjectionType.ATOMIC_PROJECTORS_OPENMX,
+        ]:
+            parameters["auto_projections"] = True
+        elif projection_type == WannierProjectionType.ANALYTIC:
+            pseudo_orbitals = get_pseudo_orbitals(pseudos)
+            projections = []
+            for kind in structure.kinds:
+                for orb in pseudo_orbitals[kind.name]["pswfcs"]:
+                    if meta_parameters["exclude_semicore"]:
+                        if orb in pseudo_orbitals[kind.name]["semicores"]:
+                            continue
+                    projections.append(f"{kind.name}:{orb[-1].lower()}")
+            inputs[cls._inputs_namespace]["projections"] = orm.List(list=projections)
+        elif projection_type == WannierProjectionType.RANDOM:
+            settings = inputs[cls._inputs_namespace].get("settings", {})
+            settings.update({"random_projections": True})
+            inputs[cls._inputs_namespace]["settings"] = settings
+        else:
+            raise ValueError(f"Unrecognized projection type {projection_type}")
 
-    def setup_parameters(self):
-        """setup input parameters of each calculations, 
-        since there are some dependencies between input parameters, 
-        we store them in context variables.
-        """
-        self.setup_scf_parameters()
-        # self.setup_nscf_parameters()
-        self.setup_projwfc_parameters()
-        self.setup_pw2wannier90_parameters()
-        self.setup_wannier90_parameters()
-        # self.report("scf:" + str(self.ctx.scf_parameters.get_dict()))
-        # self.report("nscf:" + str(self.ctx.nscf_parameters.get_dict()))
-        # self.report("projwfc:" + str(self.ctx.projwfc_parameters.get_dict()))
-        # self.report("pw2wannier90:" + str(self.ctx.pw2wannier90_parameters.get_dict()))
-        # self.report("wannier90:" + str(self.ctx.wannier90_parameters.get_dict()))
-        self.report(
-            'number of machines {} auto-set according to number of atoms'.
-            format(estimate_num_machines(self.ctx.current_structure))
-        )
-
-    def setup_scf_parameters(self):
-        """Set up the default input parameters required for the `PwBandsWorkChain`, and store it in self.ctx"""
-        ecutwfc = []
-        ecutrho = []
-
-        for kind in self.ctx.current_structure.get_kind_names():
-            try:
-                dual = self.ctx.protocol['pseudo_data'][kind]['dual']
-                cutoff = self.ctx.protocol['pseudo_data'][kind]['cutoff']
-                cutrho = dual * cutoff
-                ecutwfc.append(cutoff)
-                ecutrho.append(cutrho)
-            except KeyError:
-                self.report(
-                    'failed to retrieve the cutoff or dual factor for {}'.
-                    format(kind)
+        # Set disentanglement
+        if disentanglement_type == WannierDisentanglementType.NONE:
+            parameters["dis_num_iter"] = 0
+            parameters.pop("dis_froz_min", None)
+            parameters.pop("dis_froz_max", None)
+            parameters.pop("dis_win_min", None)
+            parameters.pop("dis_win_max", None)
+        elif disentanglement_type == WannierDisentanglementType.SMV:
+            if frozen_type == WannierFrozenType.ENERGY_FIXED:
+                inputs["shift_energy_windows"] = True
+                parameters.update(
+                    {
+                        # Here +2 means fermi_energy + 2 eV, however Fermi energy is calculated at runtime
+                        # inside Wannier90WorkChain, so it will add Fermi energy with this
+                        # dis_froz_max dynamically.
+                        "dis_froz_max": +2.0,
+                    }
+                )
+            elif frozen_type == WannierFrozenType.ENERGY_AUTO:
+                # ENERGY_AUTO needs projectability, will be set dynamically when workchain is running
+                inputs["auto_energy_windows"] = True
+            elif frozen_type == WannierFrozenType.PROJECTABILITY:
+                parameters.update(
+                    {
+                        "dis_proj_min": 0.01,
+                        "dis_proj_max": 0.95,
+                    }
                 )
-                return self.exit_codes.ERROR_INVALID_INPUT_UNRECOGNIZED_KIND
+            elif frozen_type == WannierFrozenType.FIXED_PLUS_PROJECTABILITY:
+                inputs["shift_energy_windows"] = True
+                parameters.update(
+                    {
+                        "dis_proj_min": 0.01,
+                        "dis_proj_max": 0.95,
+                        "dis_froz_max": +2.0,  # relative to fermi_energy
+                    }
+                )
+            elif frozen_type == WannierFrozenType.NONE:
+                parameters.pop("dis_froz_min", None)
+                parameters.pop("dis_froz_max", None)
+                parameters.pop("dis_win_min", None)
+                parameters.pop("dis_win_max", None)
+            else:
+                raise ValueError(f"Not supported frozen type: {frozen_type}")
+        else:
+            raise ValueError(
+                f"Not supported disentanglement type: {disentanglement_type}"
+            )
 
-        number_of_atoms = len(self.ctx.current_structure.sites)
-        pw_parameters = {
-            'CONTROL': {
-                'restart_mode': 'from_scratch',
-                'tstress': self.ctx.protocol['tstress'],
-                'tprnfor': self.ctx.protocol['tprnfor'],
-            },
-            'SYSTEM': {
-                'ecutwfc': max(ecutwfc),
-                'ecutrho': max(ecutrho),
-                'smearing': self.ctx.protocol['smearing'],
-                'degauss': self.ctx.protocol['degauss'],
-                'occupations': self.ctx.protocol['occupations'],
-            },
-            'ELECTRONS': {
-                'conv_thr':
-                self.ctx.protocol['convergence_threshold_per_atom'] *
-                number_of_atoms,
-            }
-        }
+        # Set kpoints
+        # If inputs.kpoints is a kmesh, mp_grid will be auto-set by `Wannier90Calculation`,
+        # otherwise we need to set it manually. If use open_grid, kpoints will be set dynamically
+        # after open_grid calculation.
+        kpoints = create_kpoints_from_distance(
+            structure,
+            distance=meta_parameters["kpoints_distance"],
+            force_parity=meta_parameters["kpoints_force_parity"],
+        )
+        inputs["kpoints"] = get_explicit_kpoints(kpoints)
+        parameters["mp_grid"] = kpoints.get_kpoints_mesh()[0]
+
+        # If overrides are provided, they take precedence over default values
+        if overrides:
+            parameter_overrides = overrides.get(cls._inputs_namespace, {}).get(
+                "parameters", {}
+            )
+            parameters = recursive_merge(parameters, parameter_overrides)
+            metadata_overrides = overrides.get(cls._inputs_namespace, {}).get(
+                "metadata", {}
+            )
+            metadata = recursive_merge(metadata, metadata_overrides)
 
-        self.ctx.scf_parameters = orm.Dict(dict=pw_parameters)
+        # pylint: disable=no-member
+        builder = cls.get_builder()
+        builder[cls._inputs_namespace]["code"] = code
+        builder[cls._inputs_namespace]["structure"] = structure
+        builder[cls._inputs_namespace]["kpoints"] = inputs["kpoints"]
+        builder[cls._inputs_namespace]["parameters"] = orm.Dict(parameters)
+        builder[cls._inputs_namespace]["metadata"] = metadata
+        if "projections" in inputs[cls._inputs_namespace]:
+            builder[cls._inputs_namespace]["projections"] = inputs[
+                cls._inputs_namespace
+            ]["projections"]
+        if "settings" in inputs[cls._inputs_namespace]:
+            builder[cls._inputs_namespace]["settings"] = orm.Dict(
+                dict=inputs[cls._inputs_namespace]["settings"]
+            )
+        if "settings" in inputs:
+            builder["settings"] = orm.Dict(inputs["settings"])
+        builder["clean_workdir"] = orm.Bool(inputs["clean_workdir"])
+        builder["shift_energy_windows"] = orm.Bool(inputs["shift_energy_windows"])
+        builder["auto_energy_windows"] = orm.Bool(inputs["auto_energy_windows"])
+        builder["auto_energy_windows_threshold"] = orm.Float(
+            inputs["auto_energy_windows_threshold"]
+        )
+        # pylint: enable=no-member
 
-    # we do not need this anymore, since now Wannier90WorkChain accepts input only_valence,
-    # it will set nbnd & occupations in itself.
-    # def setup_nscf_parameters(self):
-    #     """almost identical to scf_parameters, but need set nbnd
-
-    #     :return: [description]
-    #     :rtype: [type]
-    #     """
-    #     def get_z_valence_from_upf(upf_content):
-    #         """a fragile parser for upf file, to get z_valence
-
-    #         :param upf_content: the content of a upf file stored in a string
-    #         :type upf_content: str
-    #         :return: z_valence of this upf file
-    #         :rtype: float
-    #         """
-    #         for l in upf_content.split('\n'):
-    #             if 'Z valence' in l:
-    #                 #e.g. 11.00000000000      Z valence
-    #                 z = float(l.strip().split()[0])
-    #                 break
-    #             elif 'z_valence' in l:
-    #                 #e.g. z_valence="3.000000000000000E+000"
-    #                 z = float(l.strip().split("=")[1][1:-1])
-    #                 break
-    #         try:
-    #             z
-    #         except NameError:
-    #             raise KeyError('z_valence not found!')
-    #         return z
-
-    #     protocol, protocol_modifiers = self._get_protocol()
-    #     checked_pseudos = protocol.check_pseudos(
-    #         modifier_name=protocol_modifiers.get('pseudo', None),
-    #         pseudo_data=protocol_modifiers.get('pseudo_data', None))
-    #     known_pseudos = checked_pseudos['found']
-    #     pseudos = get_pseudos_from_dict(self.ctx.current_structure, known_pseudos)
-
-    #     # we try to parse the upf file to generate z_valence
-    #     # maybe use nbands_factor (aiida_qe/workflows/pw/bands.py) in the future
-    #     number_of_electrons = 0
-    #     composition = self.ctx.current_structure.get_composition()
-    #     for kind in self.ctx.current_structure.get_kind_names():
-    #         try:
-    #             upf_name = pseudos[kind].list_object_names()[0]
-    #             upf_content = pseudos[kind].get_object_content(upf_name)
-    #             z_valence = get_z_valence_from_upf(upf_content)
-    #             # self.report("found z_valence of " + kind +": " + str(z))
-    #             number_of_electrons += z_valence*composition[kind]
-    #         except KeyError:
-    #             self.report('failed to retrieve the z_valence for {}'.format(kind))
-    #             return self.exit_codes.ERROR_INVALID_INPUT_UNRECOGNIZED_KIND
-    #     if self.inputs.controls.only_valence:
-    #         nbnd = int(number_of_electrons / 2)
-    #     else:
-    #         #Three times the number of occupied bands
-    #         nbnd = int(number_of_electrons * 1.5)
-    #     self.report('nscf nbnd calculated from pseudos: ' + str(nbnd))
-
-    #     # we need deepcopy for 'nbnd', otherwise scf_parameters will change as well
-    #     from copy import deepcopy
-    #     nscf_parameters = deepcopy(self.ctx.scf_parameters.get_dict())
-    #     nscf_parameters['SYSTEM']['nbnd'] = nbnd
-
-    #     if self.inputs.controls.only_valence:
-    #         nscf_parameters['SYSTEM']['occupations'] = 'fixed'
-    #         nscf_parameters['SYSTEM'].pop('smearing')
-    #         nscf_parameters['SYSTEM'].pop('degauss')
-
-    #     nscf_parameters = orm.Dict(dict=nscf_parameters)
-    #     self.ctx.nscf_parameters = nscf_parameters
-
-    def setup_projwfc_parameters(self):
-
-        projwfc_parameters = orm.Dict(dict={'PROJWFC': {'DeltaE': 0.2}})
-        self.ctx.projwfc_parameters = projwfc_parameters
-
-    def setup_pw2wannier90_parameters(self):
-
-        parameters = {}
-        #Write UNK files (to plot WFs)
-        if self.inputs.controls.plot_wannier_functions:
-            parameters['write_unk'] = True
-            self.report("UNK files will be written.")
-
-        pw2wannier90_parameters = orm.Dict(dict={'inputpp': parameters})
-        self.ctx.pw2wannier90_parameters = pw2wannier90_parameters
-
-    def setup_wannier90_parameters(self):
-        parameters = {
-            'use_ws_distance': True,
-            # no need anymore since kmesh_tol is handled by Wannier90BaseWorkChain
-            # 'kmesh_tol': 1e-8
-        }
+        return builder
+
+    def setup(self) -> None:
+        """Call the `setup` of the `BaseRestartWorkChain` and then create the inputs dictionary in `self.ctx.inputs`.
 
-        if self.inputs.controls.auto_projections:
-            parameters['auto_projections'] = True
+        This `self.ctx.inputs` dictionary will be used by the `BaseRestartWorkChain` to submit
+        the calculations in the internal loop.
+        """
+        super().setup()
 
-        parameters['bands_plot'] = True
-        # parameters['num_bands'] = self.ctx.nscf_parameters['SYSTEM']['nbnd']
+        self.ctx.inputs = self.prepare_inputs()
 
-        if self.inputs.controls.plot_wannier_functions:
-            parameters['wannier_plot'] = True
-            # 'wannier_plot_list':[1]
-
-        number_of_atoms = len(self.ctx.current_structure.sites)
-        if self.inputs.controls.do_mlwf:
-            parameters.update({
-                'num_iter': 400,
-                'conv_tol': 1e-7 * number_of_atoms,
-                'conv_window': 3,
-            })
-        else:
-            parameters.update({'num_iter': 0})
+        self.ctx.kmeshtol_new = [self._WANNIER90_DEFAULT_KMESH_TOL, 1e-8, 1e-4]
+        self.ctx.disprojmin_multipliers = [0.5, 0.25, 0.125, 0]
+        self.ctx.wannier_plot_supercell_new = [4, 6, 8, 10]
 
-        # TODO exclude_bands
-        # if exclude_bands is not None:
-        #     wannier90_params_dict['exclude_bands'] = exclude_bands
-        #'exclude_bands': range(5,13),
+    def prepare_inputs(
+        self,
+    ) -> AttributeDict:
+        """Prepare `Wannier90Calculation` inputs according to workchain input sepc.
 
-        if self.inputs.controls.only_valence:
-            parameters['dis_num_iter'] = 0
-        else:
-            if self.inputs.controls.do_disentanglement:
-                parameters.update({
-                    'dis_num_iter': 200,
-                    'dis_conv_tol': parameters['conv_tol'],
-                    'dis_froz_max': 1.0,  #TODO a better value??
-                    #'dis_mix_ratio':1.d0,
-                    #'dis_win_max':10.0,
-                })
-            else:
-                parameters.update({'dis_num_iter': 0})
+        Different from `get_builder_from_protocol', this function is executed at runtime.
+        """
+        # pylint: disable=too-many-statements,too-many-locals,too-many-branches
+        import numpy as np
 
-        if self.inputs.controls.retrieve_hamiltonian:
-            parameters['write_tb'] = True
-            parameters['write_hr'] = True
-            parameters['write_xyz'] = True
-
-        # try:
-        #     self.ctx.random_projections = control_dict['random_projections']
-        #     if self.ctx.random_projections:
-        #         self.report("projections override: set to random from input.")
-        # except KeyError:
-        #     self.ctx.random_projections = False
-
-
-#        We expect either a KpointsData with given mesh or a desired distance between k-points
-#        if all([key not in self.inputs for key in ['kpoints_mesh', 'kpoints_distance']]):
-#            self.abort_nowait('neither the kpoints_mesh nor a kpoints_distance was specified in the inputs')
-#           return
-
-# Add the van der Waals kernel table file if specified
-#        if 'vdw_table' in self.inputs:
-#            self.ctx.inputs['vdw_table'] = self.inputs.vdw_table
-#            self.inputs.relax['vdw_table'] = self.inputs.vdw_table
-
-#        # Set the correct relaxation scheme in the input parameters
-#        if 'CONTROL' not in self.ctx.inputs['parameters']:
-#            self.ctx.inputs['parameters']['CONTROL'] = {}
-        wannier90_parameters = orm.Dict(dict=parameters)
-        self.ctx.wannier90_parameters = wannier90_parameters
-
-    def get_pw_common_inputs(self):
-        """Return the dictionary of inputs to be used as the basis for each `PwBaseWorkChain`."""
-        protocol, protocol_modifiers = self._get_protocol()
-        checked_pseudos = protocol.check_pseudos(
-            modifier_name=protocol_modifiers.get('pseudo', None),
-            pseudo_data=protocol_modifiers.get('pseudo_data', None)
-        )
-        known_pseudos = checked_pseudos['found']
-
-        inputs = AttributeDict({
-            'pw': {
-                'code':
-                self.inputs.code.pw,
-                'pseudos':
-                get_pseudos_from_dict(
-                    self.ctx.current_structure, known_pseudos
-                ),
-                'parameters':
-                self.ctx.scf_parameters,
-                'metadata': {},
-            }
-        })
+        from aiida_wannier90_workflows.utils.bands import (
+            get_homo_lumo,
+            remove_exclude_bands,
+        )
+        from aiida_wannier90_workflows.utils.scdm import get_energy_of_projectability
+
+        inputs = AttributeDict(
+            self.exposed_inputs(Wannier90Calculation, self._inputs_namespace)
+        )
+        parameters = inputs.parameters.get_dict()
+
+        if self.inputs.shift_energy_windows:
+            fermi_energy = parameters["fermi_energy"]
+            # For metal, we shift the four parameters by Fermi energy.
+            shift_energy = fermi_energy
+            if "bands" in self.inputs:
+                # Check the system is metal or insulator.
+                # For insulator, we shift them by the minimum of LUMO.
+                bands = self.inputs.bands.get_bands()
+                homo, lumo = get_homo_lumo(bands, fermi_energy)
+                bandgap = lumo - homo
+                if bandgap > 1e-3:
+                    shift_energy = lumo
+
+            keys = ("dis_froz_min", "dis_froz_max", "dis_win_min", "dis_win_max")
+            for key in keys:
+                if key in parameters:
+                    parameters[key] += shift_energy
+
+        # Auto set `dis_froz_max`
+        if self.inputs.auto_energy_windows:
+            dis_froz_max = get_energy_of_projectability(
+                bands=self.inputs.bands,
+                projections=self.inputs.bands_projections,
+                thresholds=self.inputs.auto_energy_windows_threshold.value,
+            )
+            parameters["dis_froz_max"] = dis_froz_max
 
-        if 'options' in self.inputs:
-            inputs.pw.metadata.options = self.inputs.options.get_dict()
-        else:
-            inputs.pw.metadata.options = self.get_default_options(
-                with_mpi=True
+        # Prevent error:
+        #   dis_windows: More states in the frozen window than target WFs
+        if "dis_froz_max" in parameters and "bands" in self.inputs:
+            bands = self.inputs.bands.get_bands()
+            if parameters.get("exclude_bands", None):
+                # Index of parameters['exclude_bands'] starts from 1,
+                # I need to change it to 0-based
+                exclude_bands = [_ - 1 for _ in parameters["exclude_bands"]]
+                bands = remove_exclude_bands(bands=bands, exclude_bands=exclude_bands)
+            highest_band = bands[:, min(parameters["num_wann"], bands.shape[1]) - 1]
+            # This is the energy to freeze all the num_wann bands
+            max_froz_energy = np.max(highest_band)
+            # Cannot freeze more bands than num_wann,
+            # this sets the upper limit of `dis_froz_max`.
+            if bands.shape[1] > parameters["num_wann"]:
+                min_next_band = np.min(bands[:, parameters["num_wann"]])
+                # I subtract a small value for safety
+                min_next_band -= 1e-4
+                max_froz_energy = min(max_froz_energy, min_next_band)
+            # `dis_froz_max` should be smaller than this max_froz_energy
+            # to allow doing disentanglement
+            dis_froz_max = min(max_froz_energy, parameters["dis_froz_max"])
+            parameters["dis_froz_max"] = dis_froz_max
+
+        inputs.parameters = orm.Dict(parameters)
+
+        if "remote_input_folder" in inputs and "settings" in self.inputs:
+            # Note there is an `additional_remote_symlink_list` in Wannier90Calculation.inputs.settings,
+            # however it requires user providing a list of
+            #   (computer_uuid, remote_input_folder_abs_path, dest_path)
+            # This is impossible if we launch a Wannier90Calculation inside a workflow since we don't
+            # know the remote_input_folder when setting the inputs of the workflow.
+            # Thus I add an `inputs.settings['remote_symlink_files']` to Wannier90BaseWorkChain,
+            # which only accepts a list of filenames and generate the full
+            # `additional_remote_symlink_list` here.
+            remote_input_folder = inputs["remote_input_folder"]
+            remote_input_folder_path = pathlib.Path(
+                remote_input_folder.get_remote_path()
             )
+            workflow_settings = self.inputs.settings.get_dict()
+            if "settings" in inputs:
+                calc_settings = inputs.settings.get_dict()
+            else:
+                calc_settings = {}
+            remote_symlink_list = calc_settings.get(
+                "additional_remote_symlink_list", []
+            )
+            existed_symlinks = [_[-1] for _ in remote_symlink_list]
+            for filename in workflow_settings.get("remote_symlink_files", []):
+                if filename in existed_symlinks:
+                    continue
+                remote_symlink_list.append(
+                    (
+                        remote_input_folder.computer.uuid,
+                        str(remote_input_folder_path / filename),
+                        filename,
+                    )
+                )
+            calc_settings["additional_remote_symlink_list"] = remote_symlink_list
+            inputs.settings = orm.Dict(calc_settings)
 
         return inputs
 
-    def get_scf_inputs(self):
-        """
-        For the scf calculation, we use m-v cold smearing, thus the default nbnd 
-        of QE is a bit higher than num_electrons/2, so we can get Fermi energy 
-        from scf calculation.
+    def report_error_handled(self, calculation, action) -> None:
+        """Report an action taken for a calculation that has failed.
+
+        This should be called in a registered error handler if its condition is met and an action was taken.
+
+        :param calculation: the failed calculation node
+        :param action: a string message with the action taken
         """
-        return self.get_pw_common_inputs()
+        message = f"{calculation.process_label}<{calculation.pk}> failed"
+        message += (
+            f" with exit status {calculation.exit_status}: {calculation.exit_message}"
+        )
+        self.report(message)
+        self.report(f"Action taken: {action}")
+
+    @process_handler(exit_codes=[Wannier90Calculation.exit_codes.ERROR_BVECTORS])
+    def handle_bvectors(self, calculation) -> ProcessHandlerReport:
+        """Try to fix Wannier90 bvectors errors by tunning `kmesh_tol`.
 
-    def get_nscf_inputs(self):
+        The handler will try to use kmesh_tol = 1e-6, 1e-8, 1e-4.
         """
-        The nscf nbnd will be set in Wannier90WorkChain, if only_valence then 
-        nbnd = num_electrons/2 and occupations = fixed (no smearing), 
-        otherwise nbnd = num_electrons * 1.5 and m-v cold smearing.
-        Here the num_electrons is obtained from scf output_parameters, 
-        so we do not need to calculate num_electrons from pseudos.
+        parameters = self.ctx.inputs.parameters.get_dict()
+
+        # If the user has specified `kmesh_tol` in the input parameters and it is different
+        # from the default, we will first try to use the default `kmesh_tol`.
+        current_kmeshtol = parameters.get(
+            "kmesh_tol", self._WANNIER90_DEFAULT_KMESH_TOL
+        )
+        if current_kmeshtol in self.ctx.kmeshtol_new:
+            self.ctx.kmeshtol_new.remove(current_kmeshtol)
+
+        if len(self.ctx.kmeshtol_new) == 0:
+            action = "Unrecoverable bvectors error after several trials of kmesh_tol"
+            self.report_error_handled(calculation, action)
+            return ProcessHandlerReport(True, self.exit_codes.ERROR_BVECTORS)
+
+        new_kmeshtol = self.ctx.kmeshtol_new.pop(0)
+        parameters["kmesh_tol"] = new_kmeshtol
+        action = f"Bvectors error, current kmesh_tol = {current_kmeshtol}, new kmesh_tol = {new_kmeshtol}"
+        self.report_error_handled(calculation, action)
+        self.ctx.inputs.parameters = orm.Dict(parameters)
+
+        return ProcessHandlerReport(True)
+
+    @process_handler(
+        exit_codes=[
+            Wannier90Calculation.exit_codes.ERROR_DISENTANGLEMENT_NOT_ENOUGH_STATES
+        ]
+    )
+    def handle_disentanglement_not_enough_states(
+        self, calculation
+    ) -> ProcessHandlerReport:
+        """Try to fix Wannier90 wout error message related to projectability disentanglement.
+
+        The error message is: 'Energy window contains fewer states than number of target WFs,
+        consider reducing dis_proj_min/increasing dis_win_max?'.
+
+        The handler will try to use decrease 'dis_proj_min' to allow for more states for disentanglement.
         """
-        inputs = self.get_pw_common_inputs()
-        # inputs['pw']['parameters'] = self.ctx.nscf_parameters
-        return inputs
+        parameters = self.ctx.inputs.parameters.get_dict()
+        if "dis_proj_min" not in parameters and "dis_proj_max" not in parameters:
+            # If neither is present, I should never encounter this exit_code
+            action = "Unrecoverable bvectors error: the error handler is only for projectability disentanglement"
+            self.report_error_handled(calculation, action)
+            return ProcessHandlerReport(
+                True, self.exit_codes.ERROR_DISENTANGLEMENT_NOT_ENOUGH_STATES
+            )
 
-    def get_projwfc_inputs(self):
-        inputs = AttributeDict({
-            'code': self.inputs.code.projwfc,
-            'parameters': self.ctx.projwfc_parameters,
-            'metadata': {},
-        })
+        if len(self.ctx.disprojmin_multipliers) == 0:
+            action = "Unrecoverable error after several trials of dis_proj_min"
+            self.report_error_handled(calculation, action)
+            return ProcessHandlerReport(
+                True, self.exit_codes.ERROR_DISENTANGLEMENT_NOT_ENOUGH_STATES
+            )
 
-        if 'options' in self.inputs:
-            inputs.metadata.options = self.inputs.options.get_dict()
-        else:
-            inputs.metadata.options = self.get_default_options(with_mpi=True)
-            # inputs.metadata.options = get_manual_options()
+        current_disprojmin = parameters.get(
+            "dis_proj_min", self._WANNIER90_DEFAULT_KMESH_TOL
+        )
+        multiplier = self.ctx.disprojmin_multipliers.pop(0)
+        new_disprojmin = current_disprojmin * multiplier
+        parameters["dis_proj_min"] = new_disprojmin
 
-        return inputs
+        action = "Not enough states for disentanglement, "
+        action += f"current dis_proj_min = {current_disprojmin}, new dis_proj_min = {new_disprojmin}"
+        self.report_error_handled(calculation, action)
+        self.ctx.inputs.parameters = orm.Dict(parameters)
 
-    def get_pw2wannier90_inputs(self):
-        inputs = AttributeDict({
-            'code': self.inputs.code.pw2wannier90,
-            'parameters': self.ctx.pw2wannier90_parameters,
-            'metadata': {},
-        })
-
-        # TODO max_projectability, sigma_factor_shift
-        # try:
-        #     self.ctx.max_projectability = control_dict['max_projectability']
-        #     self.report("Max projectability set to {}.".format(
-        #         self.ctx.max_projectability))
-        # except KeyError:
-        #     self.ctx.max_projectability = 0.95
-        #     self.report("Max projectability set to {} (DEFAULT).".format(
-        #         self.ctx.max_projectability))
-
-        # try:
-        #     self.ctx.sigma_factor_shift = control_dict['sigma_factor_shift']
-        #     self.report("Sigma factor shift set to {}.".format(
-        #         self.ctx.sigma_factor_shift))
-        # except KeyError:
-        #     self.ctx.sigma_factor_shift = 3.
-        #     self.report("Sigma factor shift set to {} (DEFAULT).".format(
-        #         self.ctx.sigma_factor_shift))
-
-        # dict={
-        #     #'max_projectability': self.ctx.max_projectability,
-        #     'sigma_factor_shift': self.ctx.sigma_factor_shift,
-        # }
+        return ProcessHandlerReport(True)
 
-        if 'options' in self.inputs:
-            inputs.metadata.options = self.inputs.options.get_dict()
-        else:
-            inputs.metadata.options = self.get_default_options(with_mpi=True)
+    @process_handler(exit_codes=[Wannier90Calculation.exit_codes.ERROR_PLOT_WF_CUBE])
+    def handle_plot_wf_cube(self, calculation) -> ProcessHandlerReport:
+        """Try to fix Wannier90 wout error message related to cube format.
 
-        return inputs
+        The error message is: 'Error plotting WF cube. Try one of the following:'.
 
-    def get_wannier90_inputs(self):
-        inputs = AttributeDict({
-            'code':
-            self.inputs.code.wannier90,
-            'parameters':
-            self.ctx.wannier90_parameters,
-            'metadata': {},
-            'kpoint_path':
-            orm.Dict(dict=self.ctx.kpoints_path)
-        })
-
-        #TODO ramdom_projections
-        # if self.ctx.random_projections:
-        #     if settings is not None:
-        #         settings['random_projections'] = True
-        #     else:
-        #         settings = {'random_projections': True}
-
-        if self.inputs.controls.retrieve_hamiltonian:
-            settings = {}
-            # settings['retrieve_hoppings'] = True
-            # tbmodels needs aiida.win file
-            from aiida.plugins import CalculationFactory
-            Wannier90Calculation = CalculationFactory('wannier90.wannier90')
-            settings['additional_retrieve_list'] = [
-                Wannier90Calculation._DEFAULT_INPUT_FILE
-            ]
-            # also retrieve .chk file in case we need it later
-            # seedname = Wannier90Calculation._DEFAULT_INPUT_FILE.split('.')[0]
-            # settings['additional_retrieve_list'] += [
-            #     '{}.{}'.format(seedname, ext)
-            #     for ext in ['chk', 'eig', 'amn', 'mmn', 'spn']
-            # ]
-            inputs['settings'] = orm.Dict(dict=settings)
-
-        # try:
-        #     self.ctx.options.energies_relative_to_fermi
-        # except KeyError:
-        #     self.report("W90 windows defined with the Fermi level as zero.")
+        The handler will try to increase 'wannier_plot_supercell'.
+        """
+        parameters = self.ctx.inputs.parameters.get_dict()
 
-        if 'options' in self.inputs:
-            inputs.metadata.options = self.inputs.options.get_dict()
-        else:
-            inputs.metadata.options = self.get_default_options(with_mpi=True)
+        current_supercell = parameters.get(
+            "wannier_plot_supercell", self._WANNIER90_DEFAULT_WANNIER_PLOT_SUPERCELL
+        )
+        # Remove sizes which are smaller equal than current supercell size
+        self.ctx.wannier_plot_supercell_new = [
+            _ for _ in self.ctx.wannier_plot_supercell_new if _ > current_supercell
+        ]
+
+        if len(self.ctx.wannier_plot_supercell_new) == 0:
+            action = (
+                "Unrecoverable error after several trials of wannier_plot_supercell"
+            )
+            self.report_error_handled(calculation, action)
+            return ProcessHandlerReport(True, self.exit_codes.ERROR_PLOT_WF_CUBE)
 
-        return inputs
+        new_supercell = self.ctx.wannier_plot_supercell_new.pop(0)
+        parameters["wannier_plot_supercell"] = new_supercell
 
-    def run_wannier_workchain(self):
-        """Run the `PwBandsWorkChain` to compute the band structure."""
+        action = "Error plotting WFs in cube format, "
+        action += f"current wannier_plot_supercell = {current_supercell}, new wannier_plot_supercell = {new_supercell}"
+        self.report_error_handled(calculation, action)
+        self.ctx.inputs.parameters = orm.Dict(parameters)
+
+        return ProcessHandlerReport(True)
+
+    @process_handler(
+        exit_codes=[Wannier90Calculation.exit_codes.ERROR_OUTPUT_STDOUT_INCOMPLETE]
+    )
+    def handle_output_stdout_incomplete(self, calculation) -> ProcessHandlerReport:
+        """Try to fix incomplete stdout error by reducing the number of cores.
 
-        inputs = AttributeDict({
-            'structure': self.ctx.current_structure,
-            'only_valence': self.inputs.controls.only_valence,
-            # 'relax': {
-            #     'base': get_pw_common_inputs(),
-            #     'relaxation_scheme': orm.Str('vc-relax'),
-            #     'meta_convergence': orm.Bool(self.ctx.protocol['meta_convergence']),
-            #     'volume_convergence': orm.Float(self.ctx.protocol['volume_convergence']),
-            # },
-            'scf': self.get_scf_inputs(),
-            # 'bands': get_pw_common_inputs(),
-            'nscf': self.get_nscf_inputs(),
-            'projwfc': self.get_projwfc_inputs(),
-            'pw2wannier90': self.get_pw2wannier90_inputs(),
-            'wannier90': self.get_wannier90_inputs(),
-        })
-
-        # inputs.relax.base.kpoints_distance = orm.Float(self.ctx.protocol['kpoints_mesh_density'])
-        inputs.scf.kpoints_distance = orm.Float(
-            self.ctx.protocol['kpoints_mesh_density']
-        )
-        # inputs.bands.kpoints_distance = orm.Float(self.ctx.protocol['kpoints_distance_for_bands'])
-        inputs.nscf.kpoints_distance = orm.Float(
-            self.ctx.protocol['kpoints_mesh_density']
-        )
-
-        # num_bands_factor = self.ctx.protocol.get('num_bands_factor', None)
-        # if num_bands_factor is not None:
-        #     inputs.nbands_factor = orm.Float(num_bands_factor)
-
-        running = self.submit(Wannier90WorkChain, **inputs)
-
-        self.report('launching Wannier90WorkChain<{}>'.format(running.pk))
-
-        return ToContext(workchain_bands=running)
-
-    def results(self):
-        """Attach the relevant output nodes from the band calculation to the workchain outputs for convenience."""
-
-        workchain = self.ctx.workchain_bands
-
-        if not workchain.is_finished_ok:
-            self.report(
-                'sub process Wannier90WorkChain<{}> failed'.format(
-                    workchain.pk
-                )
+        Often the ERROR_OUTPUT_STDOUT_INCOMPLETE is due to out-of-memory.
+        The handler will try to set `num_mpiprocs_per_machine` to 1.
+        """
+        import re
+
+        regex_oom = re.compile(r"Detected \d+ oom-kill event\(s\) in step")
+        regex_bus = re.compile(
+            r"Program received signal SIGBUS: Access to an undefined portion of a memory object"
+        )
+        # srun: error: nid002144: tasks 0-63: Killed
+        regex_killed = re.compile(r"srun: error: \w+: tasks? [\w\-,]+: Killed")
+        scheduler_stderr = calculation.get_scheduler_stderr()
+        for line in scheduler_stderr.split("\n"):
+            if (
+                regex_oom.search(line)
+                or regex_bus.search(line)
+                or regex_killed.search(line)
+                or "Out Of Memory" in line
+            ):
+                break
+        else:
+            action = "Unrecoverable incomplete stdout error"
+            self.report_error_handled(calculation, action)
+            return ProcessHandlerReport(
+                True, self.exit_codes.ERROR_OUTPUT_STDOUT_INCOMPLETE
             )
-            return self.exit_codes.ERROR_SUB_PROCESS_FAILED_BANDS
 
-        self.out('scf_parameters', workchain.outputs.scf__output_parameters)
-        self.out('nscf_parameters', workchain.outputs.nscf__output_parameters)
-        if 'projwfc__bands' in workchain.outputs:
-            self.out('projwfc_bands', workchain.outputs.projwfc__bands)
-            self.out(
-                'projwfc_projections', workchain.outputs.projwfc__projections
-            )
-        self.out(
-            'pw2wannier90_remote_folder',
-            workchain.outputs.pw2wannier90__remote_folder
-        )
-        self.out(
-            'wannier90_parameters',
-            workchain.outputs.wannier90__output_parameters
-        )
-        self.out('wannier90_retrieved', workchain.outputs.wannier90__retrieved)
-        self.out(
-            'wannier90_remote_folder',
-            workchain.outputs.wannier90__remote_folder
-        )
-        if 'wannier90__interpolated_bands' in workchain.outputs:
-            self.out(
-                'wannier90_interpolated_bands',
-                workchain.outputs.wannier90__interpolated_bands
-            )
-            self.report(
-                'wannier90 interpolated bands pk: {}'.format(
-                    workchain.outputs.wannier90__interpolated_bands.pk
-                )
+        metadata = self.ctx.inputs["metadata"]
+        current_num_mpiprocs_per_machine = metadata["options"]["resources"].get(
+            "num_mpiprocs_per_machine", 1
+        )
+        # num_mpiprocs_per_machine = calculation.attributes['resources'].get('num_mpiprocs_per_machine', 1)
+
+        if current_num_mpiprocs_per_machine == 1:
+            action = "Unrecoverable out-of-memory error after setting num_mpiprocs_per_machine to 1"
+            self.report_error_handled(calculation, action)
+            return ProcessHandlerReport(
+                True, self.exit_codes.ERROR_OUTPUT_STDOUT_INCOMPLETE
             )
 
-        self.report('Wannier90BandsWorkChain successfully completed')
+        new_num_mpiprocs_per_machine = current_num_mpiprocs_per_machine // 2
+        metadata["options"]["resources"][
+            "num_mpiprocs_per_machine"
+        ] = new_num_mpiprocs_per_machine
+        action = f"Out-of-memory error, current num_mpiprocs_per_machine = {current_num_mpiprocs_per_machine}"
+        action += f", new num_mpiprocs_per_machine = {new_num_mpiprocs_per_machine}"
+        self.report_error_handled(calculation, action)
+        self.ctx.inputs["metadata"] = metadata
 
-    def get_default_options(self, with_mpi=False):
-        """Increase wallclock to 5 hour, use mpi, set number of machines according to 
-        number of atoms.
-        
-        :param with_mpi: [description], defaults to False
-        :type with_mpi: bool, optional
-        :return: [description]
-        :rtype: [type]
-        """
-        from aiida_quantumespresso.utils.resources import get_default_options as get_opt
-        num_machines = estimate_num_machines(self.ctx.current_structure)
-        opt = get_opt(
-            max_num_machines=num_machines,
-            max_wallclock_seconds=3600 * 5,
-            with_mpi=with_mpi
-        )
-        return opt
-
-
-def estimate_num_machines(structure):
-    """
-     1 <= num_atoms <= 10 -> 1 machine
-    11 <= num_atoms <= 20 -> 2 machine
-    
-    :param structure: [description]
-    :type structure: [type]
-    :return: [description]
-    :rtype: [type]
-    """
-    from math import ceil
-    number_of_atoms = len(structure.sites)
-    return ceil(number_of_atoms / 10)
-
-
-def validate_protocol(protocol_dict, ctx):
-    """Check that the protocol is one for which we have a definition."""
-    try:
-        protocol_name = protocol_dict['name']
-    except KeyError as exception:
-        return 'Missing key `name` in protocol dictionary'
-    try:
-        ProtocolManager(protocol_name)
-    except ValueError as exception:
-        return str(exception)
-
-
-def get_manual_options():
-    # QE projwfc.x complains
-    #         Calling projwave ....
-    #     linear algebra parallelized on  16 procs
-
-    # Problem Sizes
-    # natomwfc =           14
-    # nx       =            4
-    # nbnd     =           24
-    # nkstot   =          216
-    # npwx     =           83
-    # nkb      =           20
-
-    # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
-    #     Error in routine  blk2cyc_zredist (1):
-
-    # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
-    #     Error in routine  blk2cyc_zredist (1):
-    #     nb less than the number of proc
-
-    # https://aiida-core.readthedocs.io/en/v1.1.1/scheduler/index.html#nodenumberjobresource
-    return {
-        'resources': {
-            'num_machines': 1,
-            'num_mpiprocs_per_machine': 8,
-            # 'tot_num_mpiprocs': ,
-            # 'num_cores_per_machine': ,
-            # 'num_cores_per_mpiproc': ,
-        },
-        'max_wallclock_seconds': 3600 * 5,
-        'withmpi': True,
-    }
+        return ProcessHandlerReport(True)
```

### Comparing `aiida-wannier90-workflows-1.0.2/aiida_wannier90_workflows/workflows/wannier.py` & `aiida_wannier90_workflows-2.1.0/src/aiida_wannier90_workflows/workflows/wannier90.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1105 +1,1026 @@
+"""Base class for Wannierisation workflow."""
+import pathlib
+import typing as ty
+
 from aiida import orm
 from aiida.common import AttributeDict
-from aiida.engine.processes import WorkChain, ToContext, if_
-from aiida.engine.processes import calcfunction
-from aiida.plugins import WorkflowFactory, CalculationFactory
+from aiida.common.lang import type_check
+from aiida.engine.processes import ProcessBuilder, ToContext, WorkChain, if_
+from aiida.orm.nodes.data.base import to_aiida_type
+
+from aiida_quantumespresso.calculations.pw import PwCalculation
+from aiida_quantumespresso.common.types import ElectronicType, SpinType
 from aiida_quantumespresso.utils.mapping import prepare_process_inputs
+from aiida_quantumespresso.workflows.protocols.utils import ProtocolMixin
 from aiida_quantumespresso.workflows.pw.base import PwBaseWorkChain
-from aiida_quantumespresso.workflows.pw.relax import PwRelaxWorkChain
-from aiida_quantumespresso.calculations.projwfc import ProjwfcCalculation
-from aiida_quantumespresso.calculations.pw2wannier90 import Pw2wannier90Calculation
-from aiida_wannier90.calculations import Wannier90Calculation
 
+from aiida_wannier90_workflows.common.types import (
+    WannierDisentanglementType,
+    WannierFrozenType,
+    WannierProjectionType,
+)
 
-class Wannier90WorkChain(WorkChain):
-    """
-    Workchain to obtain maximally localised Wannier functions (MLWF)
-    Authors: Antimo Marrazzo (antimo.marrazzo@epfl.ch), Giovanni Pizzi (giovanni.pizzi@epfl.ch), Junfeng Qiao(junfeng.qiao@epfl.ch)
-    
-    MIT License - Copyright (c), 2018, ECOLE POLYTECHNIQUE FEDERALE DE LAUSANNE
-    (Theory and Simulation of Materials (THEOS) and National Centre for 
-    Computational Design and Discovery of Novel Materials (NCCR MARVEL)).
-    All rights reserved.
-
-    Scheme: setup --> relax(optional) --> scf --> nscf --> projwfc 
-            -> wannier90_postproc --> pw2wannier90 --> wannier90 --> results
-    
-    This is a very basic workchain, in that user needs to specify 
-    inputs of every step. Please consider using Wannier90BandsWorkChain, 
-    which automatically generates inputs.
+from .base.projwfc import ProjwfcBaseWorkChain
+from .base.pw2wannier90 import Pw2wannier90BaseWorkChain
+from .base.wannier90 import Wannier90BaseWorkChain
+
+__all__ = ["validate_inputs", "Wannier90WorkChain"]
+
+
+def validate_inputs(  # pylint: disable=unused-argument,inconsistent-return-statements
+    inputs, ctx=None
+):
+    """Validate the inputs of the entire input namespace of `Wannier90WorkChain`."""
+    # If no scf inputs, the nscf must have a `parent_folder`
+    if "scf" not in inputs:
+        if "parent_folder" not in inputs["nscf"]["pw"]:
+            return "If skipping scf step, nscf inputs must have a `parent_folder`"
+
+    # Cannot specify both `auto_energy_windows` and `scdm_proj`
+    pw2wannier_parameters = inputs["pw2wannier90"]["pw2wannier90"][
+        "parameters"
+    ].get_dict()
+    auto_energy_windows = inputs["wannier90"].get("auto_energy_windows", False)
+    scdm_proj = pw2wannier_parameters["inputpp"].get("scdm_proj", False)
+    if auto_energy_windows and scdm_proj:
+        return "`auto_energy_windows` is incompatible with SCDM"
+
+    # Cannot specify both `auto_energy_windows` and `shift_energy_windows`
+    shift_energy_windows = inputs["wannier90"].get("shift_energy_windows", False)
+    if auto_energy_windows and shift_energy_windows:
+        return "`auto_energy_windows` and `shift_energy_windows` are incompatible"
+
+
+# pylint: disable=fixme,too-many-lines
+class Wannier90WorkChain(
+    ProtocolMixin, WorkChain
+):  # pylint: disable=too-many-public-methods
+    """Workchain to obtain maximally localised Wannier functions (MLWF).
+
+    Run the following steps:
+        scf -> nscf -> projwfc -> wannier90 postproc -> pw2wannier90 -> wannier90
     """
+
     @classmethod
     def define(cls, spec):
-        super().define(spec)
-        spec.input(
-            'structure',
-            valid_type=orm.StructureData,
-            help='The inputs structure.'
+        """Define the process spec."""
+        from .base.pw2wannier90 import (
+            validate_inputs_base as validate_inputs_base_pw2wannier90,
         )
-        spec.input(
-            'clean_workdir',
-            valid_type=orm.Bool,
-            default=orm.Bool(False),
-            help=
-            'If `True`, work directories of all called calculation will be cleaned at the end of execution.'
+        from .base.wannier90 import (
+            validate_inputs_base as validate_inputs_base_wannier90,
         )
+
+        super().define(spec)
+
         spec.input(
-            'only_valence',
-            valid_type=orm.Bool,
-            default=orm.Bool(False),
-            help='Whether only wannierise valence band or not'
+            "structure", valid_type=orm.StructureData, help="The input structure."
         )
         spec.input(
-            'wannier_energies_relative_to_fermi',
+            "clean_workdir",
             valid_type=orm.Bool,
-            default=orm.Bool(False),
-            help=
-            'determines if the energies(dis_froz_min/max, dis_win_min/max) defined in the input parameters '
-            + 'are relative to scf Fermi energy or not.'
-        )
-        spec.input(
-            'scdm_thresholds',
-            valid_type=orm.Dict,
-            default=orm.Dict(
-                dict={
-                    'max_projectability': 0.95,
-                    'sigma_factor': 3
-                }
+            serializer=to_aiida_type,
+            default=lambda: orm.Bool(False),
+            help=(
+                "If True, work directories of all called calculation will be cleaned "
+                "at the end of execution."
             ),
-            help='can contain two keyword: max_projectability, sigma_factor'
-        )
-        spec.expose_inputs(
-            PwRelaxWorkChain,
-            namespace='relax',
-            exclude=('clean_workdir', 'structure'),
-            namespace_options={
-                'required':
-                False,
-                'populate_defaults':
-                False,
-                'help':
-                'Inputs for the `PwRelaxWorkChain`, if not specified at all, the relaxation step is skipped.'
-            }
         )
         spec.expose_inputs(
             PwBaseWorkChain,
-            namespace='scf',
-            exclude=('clean_workdir', 'pw.structure'),
+            namespace="scf",
+            exclude=("clean_workdir", "pw.structure"),
             namespace_options={
-                'help':
-                'Inputs for the `PwBaseWorkChain` for the SCF calculation.'
-            }
+                "required": False,
+                "populate_defaults": False,
+                "help": "Inputs for the `PwBaseWorkChain` for the SCF calculation.",
+            },
         )
         spec.expose_inputs(
             PwBaseWorkChain,
-            namespace='nscf',
-            exclude=('clean_workdir', 'pw.structure'),
+            namespace="nscf",
+            exclude=("clean_workdir", "pw.structure"),
             namespace_options={
-                'help':
-                'Inputs for the `PwBaseWorkChain` for the NSCF calculation.'
-            }
+                "required": False,
+                "populate_defaults": False,
+                "help": "Inputs for the `PwBaseWorkChain` for the NSCF calculation.",
+            },
         )
+        spec.inputs["nscf"]["pw"].validator = PwCalculation.validate_inputs_base
         spec.expose_inputs(
-            ProjwfcCalculation,
-            namespace='projwfc',
-            exclude=('parent_folder', ),
+            ProjwfcBaseWorkChain,
+            namespace="projwfc",
+            exclude=("clean_workdir", "projwfc.parent_folder"),
             namespace_options={
-                'required':
-                False,
-                'help':
-                'Inputs for the `ProjwfcCalculation` for the Projwfc calculation.'
-            }
+                "required": False,
+                "populate_defaults": False,
+                "help": "Inputs for the `ProjwfcBaseWorkChain`.",
+            },
         )
         spec.expose_inputs(
-            Pw2wannier90Calculation,
-            namespace='pw2wannier90',
-            exclude=('parent_folder', 'nnkp_file'),
-            namespace_options={
-                'help':
-                'Inputs for the `Pw2wannier90Calculation` for the pw2wannier90 calculation.'
-            }
+            Pw2wannier90BaseWorkChain,
+            namespace="pw2wannier90",
+            exclude=(
+                "clean_workdir",
+                "pw2wannier90.parent_folder",
+                "pw2wannier90.nnkp_file",
+            ),
+            namespace_options={"help": "Inputs for the `Pw2wannier90BaseWorkChain`."},
         )
+        spec.inputs["pw2wannier90"].validator = validate_inputs_base_pw2wannier90
         spec.expose_inputs(
-            Wannier90Calculation,
-            namespace='wannier90',
-            exclude=('structure', 'kpoints'),
-            namespace_options={
-                'help':
-                'Inputs for the `Wannier90Calculation` for the Wannier90 calculation.'
-            }
+            Wannier90BaseWorkChain,
+            namespace="wannier90",
+            exclude=("clean_workdir", "wannier90.structure"),
+            namespace_options={"help": "Inputs for the `Wannier90BaseWorkChain`."},
         )
+        spec.inputs["wannier90"].validator = validate_inputs_base_wannier90
+
+        spec.inputs.validator = validate_inputs
+
         spec.outline(
             cls.setup,
-            if_(cls.should_do_relax)(
-                cls.run_relax,
-                cls.inspect_relax,
+            if_(cls.should_run_scf)(
+                cls.run_scf,
+                cls.inspect_scf,
+            ),
+            if_(cls.should_run_nscf)(
+                cls.run_nscf,
+                cls.inspect_nscf,
             ),
-            cls.run_scf,
-            cls.inspect_scf,
-            cls.run_nscf,
-            cls.inspect_nscf,
-            if_(cls.should_do_projwfc)(
+            if_(cls.should_run_projwfc)(
                 cls.run_projwfc,
                 cls.inspect_projwfc,
             ),
             cls.run_wannier90_pp,
             cls.inspect_wannier90_pp,
             cls.run_pw2wannier90,
             cls.inspect_pw2wannier90,
             cls.run_wannier90,
             cls.inspect_wannier90,
             cls.results,
         )
 
         spec.expose_outputs(
-            PwRelaxWorkChain,
-            namespace='relax',
-            namespace_options={'required': False}
+            PwBaseWorkChain, namespace="scf", namespace_options={"required": False}
         )
-        spec.expose_outputs(PwBaseWorkChain, namespace='scf')
-        spec.expose_outputs(PwBaseWorkChain, namespace='nscf')
         spec.expose_outputs(
-            ProjwfcCalculation,
-            namespace='projwfc',
-            namespace_options={'required': False}
-        )
-        spec.expose_outputs(Pw2wannier90Calculation, namespace='pw2wannier90')
-        spec.expose_outputs(Wannier90Calculation, namespace='wannier90_pp')
-        spec.expose_outputs(Wannier90Calculation, namespace='wannier90')
-
-        spec.exit_code(
-            401,
-            'ERROR_SUB_PROCESSS_FAILED_SETUP',
-            message='setup failed, check your input'
+            PwBaseWorkChain, namespace="nscf", namespace_options={"required": False}
         )
+        spec.expose_outputs(
+            ProjwfcBaseWorkChain,
+            namespace="projwfc",
+            namespace_options={"required": False},
+        )
+        spec.expose_outputs(Pw2wannier90BaseWorkChain, namespace="pw2wannier90")
+        spec.expose_outputs(Wannier90BaseWorkChain, namespace="wannier90_pp")
+        spec.expose_outputs(Wannier90BaseWorkChain, namespace="wannier90")
+
         spec.exit_code(
-            402,
-            'ERROR_SUB_PROCESS_FAILED_RELAX',
-            message='the PwRelaxWorkChain sub process failed'
+            420,
+            "ERROR_SUB_PROCESS_FAILED_SCF",
+            message="the scf PwBaseWorkChain sub process failed",
         )
         spec.exit_code(
-            403,
-            'ERROR_SUB_PROCESS_FAILED_SCF',
-            message='the scf PwBasexWorkChain sub process failed'
+            430,
+            "ERROR_SUB_PROCESS_FAILED_NSCF",
+            message="the nscf PwBaseWorkChain sub process failed",
         )
         spec.exit_code(
-            404,
-            'ERROR_SUB_PROCESS_FAILED_NSCF',
-            message='the nscf PwBasexWorkChain sub process failed'
+            440,
+            "ERROR_SUB_PROCESS_FAILED_PROJWFC",
+            message="the ProjwfcBaseWorkChain sub process failed",
         )
         spec.exit_code(
-            405,
-            'ERROR_SUB_PROCESS_FAILED_PROJWFC',
-            message='the ProjwfcCalculation sub process failed'
+            450,
+            "ERROR_SUB_PROCESS_FAILED_WANNIER90PP",
+            message="the postproc Wannier90BaseWorkChain sub process failed",
         )
         spec.exit_code(
-            406,
-            'ERROR_SUB_PROCESS_FAILED_WANNIER90PP',
-            message='the postproc Wannier90Calculation sub process failed'
+            460,
+            "ERROR_SUB_PROCESS_FAILED_PW2WANNIER90",
+            message="the Pw2wannier90BaseWorkChain sub process failed",
         )
         spec.exit_code(
-            407,
-            'ERROR_SUB_PROCESS_FAILED_PW2WANNIER90',
-            message='the Pw2wannier90Calculation sub process failed'
+            470,
+            "ERROR_SUB_PROCESS_FAILED_WANNIER90",
+            message="the Wannier90BaseWorkChain sub process failed",
         )
         spec.exit_code(
-            408,
-            'ERROR_SUB_PROCESS_FAILED_WANNIER90',
-            message='the Wannier90Calculation sub process failed'
+            480, "ERROR_SANITY_CHECK_FAILED", message="outputs sanity check failed"
         )
 
-    def setup(self):
-        """
-        Define the current structure in the context to be the input structure.
-        """
-        self.ctx.current_structure = self.inputs.structure
+    @classmethod
+    def get_protocol_filepath(cls) -> pathlib.Path:
+        """Return ``pathlib.Path`` to the ``.yaml`` file that defines the protocols."""
+        from importlib_resources import files
 
-        inputs = AttributeDict(
-            self.exposed_inputs(Wannier90Calculation, namespace='wannier90')
-        )
-        parameters = inputs.parameters.get_dict()
+        from . import protocols
 
-        self.ctx.bands_plot = parameters.get('bands_plot', False)
-        self.ctx.auto_projections = parameters.get('auto_projections', False)
+        return files(protocols) / "wannier90.yaml"
 
-        # check bands_plot kpoint_path
-        if self.ctx.bands_plot:
-            kpoint_path = inputs.get('kpoint_path', None)
-            if kpoint_path is None:
-                self.report(
-                    'bands_plot is required but no kpoint_path provided'
+    @classmethod
+    def get_protocol_overrides(cls) -> dict:
+        """Return the ``pathlib.Path`` to the ``.yaml`` file that defines the protocols."""
+        from importlib_resources import files
+        import yaml
+
+        from . import protocols
+
+        path = files(protocols) / "overrides" / "wannier90.yaml"
+        with path.open() as file:
+            return yaml.safe_load(file)
+
+    @classmethod
+    def get_builder_from_protocol(  # pylint: disable=unused-argument
+        cls,
+        codes: ty.Mapping[str, ty.Union[str, int, orm.Code]],
+        structure: orm.StructureData,
+        *,
+        protocol: str = None,
+        overrides: dict = None,
+        pseudo_family: str = None,
+        electronic_type: ElectronicType = ElectronicType.METAL,
+        spin_type: SpinType = SpinType.NONE,
+        initial_magnetic_moments: dict = None,
+        projection_type: WannierProjectionType = WannierProjectionType.SCDM,
+        disentanglement_type: WannierDisentanglementType = None,
+        frozen_type: WannierFrozenType = None,
+        exclude_semicore: bool = True,
+        external_projectors_path: str = None,
+        plot_wannier_functions: bool = False,
+        retrieve_hamiltonian: bool = False,
+        retrieve_matrices: bool = False,
+        print_summary: bool = True,
+        summary: dict = None,
+    ) -> ProcessBuilder:
+        """Return a builder prepopulated with inputs selected according to the chosen protocol.
+
+        The builder can be submitted directly by `aiida.engine.submit(builder)`.
+
+        :param codes: a dictionary of ``Code`` instance for pw.x, pw2wannier90.x, wannier90.x, (optionally) projwfc.x.
+        :type codes: dict
+        :param structure: the ``StructureData`` instance to use.
+        :type structure: orm.StructureData
+        :param protocol: protocol to use, if not specified, the default will be used.
+        :type protocol: str
+        :param overrides: optional dictionary of inputs to override the defaults of the protocol.
+        :param electronic_type: indicate the electronic character of the system through ``ElectronicType`` instance.
+        :param spin_type: indicate the spin polarization type to use through a ``SpinType`` instance.
+        :param initial_magnetic_moments: optional dictionary that maps the initial magnetic moment of
+        each kind to a desired value for a spin polarized calculation.
+        Note that for ``spin_type == SpinType.COLLINEAR`` an initial guess for the magnetic moment
+        is automatically set in case this argument is not provided.
+        :param projection_type: indicate the Wannier initial projection type of the system
+        through ``WannierProjectionType`` instance.
+        Default to SCDM.
+        :param disentanglement_type: indicate the Wannier disentanglement type of the system through
+        ``WannierDisentanglementType`` instance. Default to None, which will choose the best type
+        based on `projection_type`:
+            For WannierProjectionType.SCDM, use WannierDisentanglementType.NONE
+            For other WannierProjectionType, use WannierDisentanglementType.SMV
+        :param frozen_type: indicate the Wannier disentanglement type of the system
+        through ``WannierFrozenType`` instance. Default to None, which will choose
+        the best frozen type based on `electronic_type` and `projection_type`.
+            for ElectronicType.INSULATOR, use WannierFrozenType.NONE
+            for metals or insulators with conduction bands:
+                for WannierProjectionType.ANALYTIC/RANDOM, use WannierFrozenType.ENERGY_FIXED
+                for WannierProjectionType.ATOMIC_PROJECTORS_QE/OPENMX, use WannierFrozenType.FIXED_PLUS_PROJECTABILITY
+                for WannierProjectionType.SCDM, use WannierFrozenType.NONE
+        :param maximal_localisation: if true do maximal localisation of Wannier functions.
+        :param exclude_semicores: if True do not Wannierise semicore states.
+        :param plot_wannier_functions: if True plot Wannier functions as xsf files.
+        :param retrieve_hamiltonian: if True retrieve Wannier Hamiltonian.
+        :param retrieve_matrices: if True retrieve amn/mmn/eig/chk/spin files.
+        :param print_summary: if True print a summary of key input parameters
+        :param summary: A dict containing key input parameters and can be printed out
+        when the `get_builder_from_protocol` returns, to let user have a quick check of the
+        generated inputs. Since in python dict is pass-by-reference, the input dict can be
+        modified in the method and used by the invoking function. This allows printing the
+        summary only by the last overriding method.
+        :return: a process builder instance with all inputs defined and ready for launch.
+        :rtype: ProcessBuilder
+        """
+        from aiida_wannier90_workflows.utils.pseudo import (
+            get_pseudo_orbitals,
+            get_semicore_list,
+        )
+        from aiida_wannier90_workflows.utils.workflows.builder.generator import (
+            get_nscf_builder,
+            get_scf_builder,
+        )
+        from aiida_wannier90_workflows.utils.workflows.builder.projections import (
+            guess_wannier_projection_types,
+        )
+        from aiida_wannier90_workflows.utils.workflows.builder.submit import (
+            check_codes,
+            recursive_merge_builder,
+        )
+
+        # Check function arguments
+        codes = check_codes(codes)
+        type_check(electronic_type, ElectronicType)
+        type_check(spin_type, SpinType)
+        type_check(projection_type, WannierProjectionType)
+        if disentanglement_type:
+            type_check(disentanglement_type, WannierDisentanglementType)
+        if frozen_type:
+            type_check(frozen_type, WannierFrozenType)
+
+        if electronic_type not in [ElectronicType.METAL, ElectronicType.INSULATOR]:
+            raise NotImplementedError(
+                f"electronic type `{electronic_type}` is not supported."
+            )
+
+        if spin_type not in [SpinType.NONE, SpinType.SPIN_ORBIT]:
+            raise NotImplementedError(f"spin type `{spin_type}` is not supported.")
+
+        if initial_magnetic_moments and spin_type != SpinType.COLLINEAR:
+            raise ValueError(
+                f"`initial_magnetic_moments` is specified but spin type `{spin_type}` is incompatible."
+            )
+
+        (
+            projection_type,
+            disentanglement_type,
+            frozen_type,
+        ) = guess_wannier_projection_types(
+            electronic_type=electronic_type,
+            projection_type=projection_type,
+            disentanglement_type=disentanglement_type,
+            frozen_type=frozen_type,
+        )
+
+        if projection_type == WannierProjectionType.ATOMIC_PROJECTORS_OPENMX:
+            if external_projectors_path is None:
+                raise ValueError(
+                    f"Must specify `external_projectors_path` when using {projection_type}"
                 )
-                return self.exit_codes.ERROR_SUB_PROCESSS_FAILED_SETUP
+            type_check(external_projectors_path, str)
 
-        # debug
-        # self.ctx.workchain_scf = orm.load_node(13623) # CsH
-        # self.ctx.workchain_nscf = orm.load_node(13643)
-        # self.ctx.calc_projwfc = orm.load_node(13652)
-        # self.ctx.nscf_kmesh = orm.KpointsData()
-        # self.ctx.nscf_kmesh.set_kpoints_mesh([9, 9, 9])
-        # self.ctx.workchain_wannier90_pp = orm.load_node(13712)
-        # self.ctx.calc_pw2wannier90 = orm.load_node(13726)
-        # self.ctx.calc_wannier90 = orm.load_node(13798)
+        if pseudo_family is None:
+            if spin_type == SpinType.SPIN_ORBIT:
+                # I use pseudo-dojo for SOC
+                pseudo_family = "PseudoDojo/0.4/PBE/FR/standard/upf"
+            else:
+                pseudo_family = Wannier90BaseWorkChain.get_protocol_inputs(
+                    protocol=protocol
+                )["meta_parameters"]["pseudo_family"]
+
+        # Prepare workchain builder
+        # I need to use explicitly `Wannier90WorkChain.get_protocol_inputs()` instead of
+        # `cls.get_protocol_inputs()`, because for a subclass of Wannier90WorkChain,
+        # `cls.get_protocol_inputs()` will call the `get_protocol_inputs` of that subclass,
+        # which might be different from this base class.
+        builder = Wannier90WorkChain.get_builder()
+        inputs = Wannier90WorkChain.get_protocol_inputs(protocol, overrides)
+        builder = recursive_merge_builder(builder, inputs)
+
+        builder["structure"] = structure
+
+        if not overrides:
+            overrides = {}
+
+        # Prepare wannier90
+        wannier_overrides = overrides.get("wannier90", {})
+        wannier_overrides.setdefault("meta_parameters", {})
+        wannier_overrides["meta_parameters"].setdefault("pseudo_family", pseudo_family)
+        wannier_overrides["meta_parameters"].setdefault(
+            "exclude_semicore", exclude_semicore
+        )
+        wannier_builder = Wannier90BaseWorkChain.get_builder_from_protocol(
+            code=codes["wannier90"],
+            structure=structure,
+            protocol=protocol,
+            overrides=wannier_overrides,
+            electronic_type=electronic_type,
+            spin_type=spin_type,
+            projection_type=projection_type,
+            disentanglement_type=disentanglement_type,
+            frozen_type=frozen_type,
+        )
+        # Remove workchain excluded inputs
+        wannier_builder["wannier90"].pop("structure", None)
+        wannier_builder.pop("clean_workdir", None)
+        builder[
+            "wannier90"
+        ] = wannier_builder._inputs(  # pylint: disable=protected-access
+            prune=True
+        )
+
+        kpoints_distance = Wannier90BaseWorkChain.get_protocol_inputs(
+            protocol=protocol, overrides=wannier_overrides
+        )["meta_parameters"]["kpoints_distance"]
+
+        # Prepare scf
+        scf_overrides = overrides.get("scf", {})
+        scf_builder = get_scf_builder(
+            code=codes["pw"],
+            structure=structure,
+            kpoints_distance=kpoints_distance,
+            pseudo_family=pseudo_family,
+            electronic_type=electronic_type,
+            spin_type=spin_type,
+            overrides=scf_overrides,
+        )
+        # Remove workchain excluded inputs
+        scf_builder["pw"].pop("structure", None)
+        scf_builder.pop("clean_workdir", None)
+        builder["scf"] = scf_builder._inputs(  # pylint: disable=protected-access
+            prune=True
+        )
+
+        # Prepare nscf
+        num_bands = wannier_builder["wannier90"]["parameters"]["num_bands"]
+        exclude_bands = (
+            wannier_builder["wannier90"]["parameters"]
+            .get_dict()
+            .get("exclude_bands", [])
+        )
+        nbnd = num_bands + len(exclude_bands)
+        # Use explicit list of kpoints generated by wannier builder.
+        # Since the QE auto generated kpoints might be different from wannier90, here we explicitly
+        # generate a list of kpoint coordinates to avoid discrepencies.
+        kpoints = wannier_builder["wannier90"]["kpoints"]
+        nscf_overrides = overrides.get("nscf", {})
+        nscf_builder = get_nscf_builder(
+            code=codes["pw"],
+            structure=structure,
+            nbnd=nbnd,
+            kpoints=kpoints,
+            pseudo_family=pseudo_family,
+            electronic_type=electronic_type,
+            spin_type=spin_type,
+            overrides=nscf_overrides,
+        )
+        # Remove workchain excluded inputs
+        nscf_builder["pw"].pop("structure", None)
+        nscf_builder.pop("clean_workdir", None)
+        builder["nscf"] = nscf_builder._inputs(  # pylint: disable=protected-access
+            prune=True
+        )
+
+        # Prepare projwfc
+        if projection_type == WannierProjectionType.SCDM:
+            run_projwfc = True
+        else:
+            if (  # pylint: disable=simplifiable-if-statement
+                frozen_type == WannierFrozenType.ENERGY_AUTO
+            ):
+                run_projwfc = True
+            else:
+                run_projwfc = False
+        if run_projwfc:
+            projwfc_overrides = overrides.get("projwfc", {})
+            projwfc_builder = ProjwfcBaseWorkChain.get_builder_from_protocol(
+                code=codes["projwfc"], protocol=protocol, overrides=projwfc_overrides
+            )
+            # Remove workchain excluded inputs
+            projwfc_builder.pop("clean_workdir", None)
+            builder[
+                "projwfc"
+            ] = projwfc_builder._inputs(  # pylint: disable=protected-access
+                prune=True
+            )
+
+        # Prepare pw2wannier90
+        exclude_projectors = None
+        if exclude_semicore:
+            pseudo_orbitals = get_pseudo_orbitals(builder["scf"]["pw"]["pseudos"])
+            exclude_projectors = get_semicore_list(structure, pseudo_orbitals)
+        pw2wannier90_overrides = overrides.get("projwfc", {})
+        pw2wannier90_builder = Pw2wannier90BaseWorkChain.get_builder_from_protocol(
+            code=codes["pw2wannier90"],
+            protocol=protocol,
+            overrides=pw2wannier90_overrides,
+            electronic_type=electronic_type,
+            projection_type=projection_type,
+            exclude_projectors=exclude_projectors,
+            external_projectors_path=external_projectors_path,
+        )
+        # Remove workchain excluded inputs
+        pw2wannier90_builder.pop("clean_workdir", None)
+        builder[
+            "pw2wannier90"
+        ] = pw2wannier90_builder._inputs(  # pylint: disable=protected-access
+            prune=True
+        )
+
+        # Apply several overrides
+        protocol_overrides = Wannier90WorkChain.get_protocol_overrides()
+        if plot_wannier_functions:
+            builder = recursive_merge_builder(
+                builder, protocol_overrides["plot_wannier_functions"]
+            )
+        if retrieve_hamiltonian:
+            builder = recursive_merge_builder(
+                builder, protocol_overrides["retrieve_hamiltonian"]
+            )
+        if retrieve_matrices:
+            builder = recursive_merge_builder(
+                builder, protocol_overrides["retrieve_matrices"]
+            )
+
+        # A dictionary containing key info of Wannierisation and will be printed when the function returns.
+        if summary is None:
+            summary = {}
+        summary["Formula"] = structure.get_formula()
+        summary["PseudoFamily"] = pseudo_family
+        summary["ElectronicType"] = electronic_type.name
+        summary["SpinType"] = spin_type.name
+        summary["WannierProjectionType"] = projection_type.name
+        summary["WannierDisentanglementType"] = disentanglement_type.name
+        summary["WannierFrozenType"] = frozen_type.name
+
+        params = builder["wannier90"]["wannier90"]["parameters"].get_dict()
+        summary["num_bands"] = params["num_bands"]
+        summary["num_wann"] = params["num_wann"]
+        if "exclude_bands" in params:
+            summary["exclude_bands"] = params["exclude_bands"]
+        summary["mp_grid"] = params["mp_grid"]
 
-    def should_do_relax(self):
-        """
-        If the 'relax' input namespace was specified, we relax the input structure.
-        """
-        return 'relax' in self.inputs
+        notes = summary.get("notes", [])
+        summary["notes"] = notes
 
-    def run_relax(self):
-        """
-        Run the PwRelaxWorkChain to run a relax calculation
-        """
-        inputs = AttributeDict(
-            self.exposed_inputs(PwRelaxWorkChain, namespace='relax')
-        )
-        inputs.structure = self.ctx.current_structure
-
-        running = self.submit(PwRelaxWorkChain, **inputs)
+        if print_summary:
+            cls.print_summary(summary)
 
-        self.report('launching PwRelaxWorkChain<{}>'.format(running.pk))
+        return builder
 
-        return ToContext(workchain_relax=running)
+    @classmethod
+    def print_summary(cls, summary: ty.Dict) -> None:
+        """Try to pretty print the summary when the `get_builder_from_protocol` returns."""
+        notes = summary.pop("notes", [])
+
+        print("Summary of key input parameters:")
+        for key, val in summary.items():
+            print(f"  {key}: {val}")
+        print("")
+
+        if len(notes) == 0:
+            return
+
+        print("Notes:")
+        for note in notes:
+            print(f"  * {note}")
 
-    def inspect_relax(self):
-        """
-        verify that the PwRelaxWorkChain successfully finished.
-        """
-        workchain = self.ctx.workchain_relax
+    def setup(self) -> None:
+        """Define the current structure in the context to be the input structure."""
+        self.ctx.current_structure = self.inputs.structure
 
-        if not workchain.is_finished_ok:
-            self.report(
-                'PwRelaxWorkChain failed with exit status {}'.format(
-                    workchain.exit_status
-                )
-            )
-            return self.exit_codes.ERROR_SUB_PROCESS_FAILED_RELAX
+        if not self.should_run_scf():
+            self.ctx.current_folder = self.inputs["nscf"]["pw"]["parent_folder"]
 
-        self.ctx.current_structure = workchain.outputs.output_structure
+    def should_run_scf(self) -> bool:
+        """If the 'scf' input namespace was specified, run the scf workchain."""
+        return "scf" in self.inputs
 
     def run_scf(self):
-        """
-        Run the PwBaseWorkChain in scf mode on the primitive cell of (optionally relaxed) input structure.
-        """
-        inputs = AttributeDict(
-            self.exposed_inputs(PwBaseWorkChain, namespace='scf')
-        )
+        """Run the `PwBaseWorkChain` in scf mode on the current structure."""
+        inputs = AttributeDict(self.exposed_inputs(PwBaseWorkChain, namespace="scf"))
         inputs.pw.structure = self.ctx.current_structure
-        inputs.pw.parameters = inputs.pw.parameters.get_dict()
-        inputs.pw.parameters.setdefault('CONTROL', {})
-        inputs.pw.parameters['CONTROL']['calculation'] = 'scf'
+        inputs.metadata.call_link_label = "scf"
 
         inputs = prepare_process_inputs(PwBaseWorkChain, inputs)
         running = self.submit(PwBaseWorkChain, **inputs)
-
-        self.report(
-            'scf step - launching PwBaseWorkChain<{}> in {} mode'.format(
-                running.pk, 'scf'
-            )
-        )
+        self.report(f"launching {running.process_label}<{running.pk}> in scf mode")
 
         return ToContext(workchain_scf=running)
 
-    def inspect_scf(self):
-        """Verify that the PwBaseWorkChain for the scf run successfully finished."""
+    def inspect_scf(self):  # pylint: disable=inconsistent-return-statements
+        """Verify that the `PwBaseWorkChain` for the scf run successfully finished."""
         workchain = self.ctx.workchain_scf
 
         if not workchain.is_finished_ok:
             self.report(
-                'scf PwBaseWorkChain failed with exit status {}'.format(
-                    workchain.exit_status
-                )
+                f"scf {workchain.process_label} failed with exit status {workchain.exit_status}"
             )
             return self.exit_codes.ERROR_SUB_PROCESS_FAILED_SCF
 
         self.ctx.current_folder = workchain.outputs.remote_folder
-        self.report("scf PwBaseWorkChain successfully finished")
+
+    def should_run_nscf(self) -> bool:
+        """If the `nscf` input namespace was specified, run the nscf workchain."""
+        return "nscf" in self.inputs
 
     def run_nscf(self):
-        """
-        Run the PwBaseWorkChain in nscf mode
-        """
-        inputs = AttributeDict(
-            self.exposed_inputs(PwBaseWorkChain, namespace='nscf')
-        )
+        """Run the PwBaseWorkChain in nscf mode."""
+        inputs = AttributeDict(self.exposed_inputs(PwBaseWorkChain, namespace="nscf"))
         inputs.pw.structure = self.ctx.current_structure
         inputs.pw.parent_folder = self.ctx.current_folder
-        inputs.pw.parameters = inputs.pw.parameters.get_dict()
-        inputs.pw.parameters.setdefault('CONTROL', {})
-        inputs.pw.parameters.setdefault('SYSTEM', {})
-        inputs.pw.parameters.setdefault('ELECTRONS', {})
-        inputs.pw.parameters['CONTROL']['restart_mode'] = 'from_scratch'
-        inputs.pw.parameters['CONTROL']['calculation'] = 'nscf'
-        inputs.pw.parameters['SYSTEM']['nosym'] = True
-        inputs.pw.parameters['SYSTEM']['noinv'] = True
-        inputs.pw.parameters['ELECTRONS']['diagonalization'] = 'cg'
-        inputs.pw.parameters['ELECTRONS']['diago_full_acc'] = True
-
-        if self.inputs.only_valence:
-            inputs.pw.parameters['SYSTEM']['occupations'] = 'fixed'
-            inputs.pw.parameters['SYSTEM'].pop(
-                'smearing', None
-            )  # pop None to avoid KeyError
-            inputs.pw.parameters['SYSTEM'].pop(
-                'degauss', None
-            )  # pop None to avoid KeyError
-
-        # inputs.pw.pseudos is an AttributeDict, but calcfunction only accepts
-        # orm.Data, so we unpack it to pass in orm.UpfData
-        inputs.pw.parameters = update_nscf_num_bands(
-            orm.Dict(dict=inputs.pw.parameters),
-            self.ctx.workchain_scf.outputs.output_parameters,
-            self.ctx.current_structure, self.inputs.only_valence,
-            **inputs.pw.pseudos
-        )
-        self.report(
-            'nscf number of bands set as ' +
-            str(inputs.pw.parameters['SYSTEM']['nbnd'])
-        )
-
-        # check kmesh
-        try:
-            inputs.kpoints
-        except AttributeError:
-            # then kpoints_distance must exists, since this is ensured by inputs check of this workchain
-            from aiida_quantumespresso.workflows.functions.create_kpoints_from_distance import create_kpoints_from_distance
-            force_parity = inputs.get('kpoints_force_parity', orm.Bool(False))
-            kmesh = create_kpoints_from_distance(
-                self.ctx.current_structure, inputs.kpoints_distance,
-                force_parity
-            )
-            #kpoints_data = orm.KpointsData()
-            # kpoints_data.set_cell_from_structure(self.ctx.current_structure)
-            # kmesh = kpoints_data.set_kpoints_mesh_from_density(inputs.kpoints_distance.value)
-        else:
-            try:
-                inputs.kpoints.get_kpoints_mesh()
-            except AttributeError:
-                self.report("nscf only support `mesh' type KpointsData")
-                return self.exit_codes.ERROR_SUB_PROCESS_FAILED_NSCF
-            else:
-                kmesh = inputs.kpoints
-        # convert kmesh to explicit list, since auto generated kpoints
-        # maybe different between QE & Wannier90. Here we explicitly
-        # generate a list of kpoint to avoid discrepencies between
-        # QE's & Wannier90's automatically generated kpoints.
-        self.ctx.nscf_kmesh = kmesh  # store it since it will be used by w90
-        inputs.kpoints = convert_kpoints_mesh_to_list(kmesh)
+        inputs.metadata.call_link_label = "nscf"
 
         inputs = prepare_process_inputs(PwBaseWorkChain, inputs)
         running = self.submit(PwBaseWorkChain, **inputs)
-
-        self.report(
-            'nscf step - launching PwBaseWorkChain<{}> in {} mode'.format(
-                running.pk, 'nscf'
-            )
-        )
+        self.report(f"launching {running.process_label}<{running.pk}> in nscf mode")
 
         return ToContext(workchain_nscf=running)
 
-    def inspect_nscf(self):
-        """Verify that the PwBaseWorkChain for the nscf run successfully finished."""
+    def inspect_nscf(self):  # pylint: disable=inconsistent-return-statements
+        """Verify that the `PwBaseWorkChain` for the nscf run successfully finished."""
         workchain = self.ctx.workchain_nscf
 
         if not workchain.is_finished_ok:
             self.report(
-                'nscf PwBaseWorkChain failed with exit status {}'.format(
-                    workchain.exit_status
-                )
+                f"nscf {workchain.process_label} failed with exit status {workchain.exit_status}"
             )
             return self.exit_codes.ERROR_SUB_PROCESS_FAILED_NSCF
 
         self.ctx.current_folder = workchain.outputs.remote_folder
-        self.report("nscf PwBaseWorkChain successfully finished")
 
-    def should_do_projwfc(self):
-        """
-        If the 'auto_projections = true' && only_valence, we 
-        run projwfc calculation to extract SCDM mu & sigma.
-        """
-        self.report("SCDM mu & sigma are auto-set using projectability")
-        return self.ctx.auto_projections and not self.inputs.only_valence.value
+    def should_run_projwfc(self) -> bool:
+        """If the 'projwfc' input namespace was specified, run the projwfc calculation."""
+        return "projwfc" in self.inputs
 
     def run_projwfc(self):
-        """
-        Projwfc step
-        :return:
-        """
+        """Projwfc step."""
         inputs = AttributeDict(
-            self.exposed_inputs(ProjwfcCalculation, namespace='projwfc')
+            self.exposed_inputs(ProjwfcBaseWorkChain, namespace="projwfc")
         )
-        inputs.parent_folder = self.ctx.current_folder
+        inputs.projwfc.parent_folder = self.ctx.current_folder
+        inputs.metadata.call_link_label = "projwfc"
 
-        inputs = prepare_process_inputs(ProjwfcCalculation, inputs)
-        running = self.submit(ProjwfcCalculation, **inputs)
+        inputs = prepare_process_inputs(ProjwfcBaseWorkChain, inputs)
+        running = self.submit(ProjwfcBaseWorkChain, **inputs)
+        self.report(f"launching {running.process_label}<{running.pk}>")
 
-        self.report(
-            'projwfc step - launching ProjwfcCalculation<{}>'.format(
-                running.pk
-            )
-        )
-
-        return ToContext(calc_projwfc=running)
+        return ToContext(workchain_projwfc=running)
 
-    def inspect_projwfc(self):
-        """Verify that the ProjwfcCalculation for the projwfc run successfully finished."""
-        calculation = self.ctx.calc_projwfc
+    def inspect_projwfc(self):  # pylint: disable=inconsistent-return-statements
+        """Verify that the `ProjwfcCalculation` for the projwfc run successfully finished."""
+        workchain = self.ctx.workchain_projwfc
 
-        if not calculation.is_finished_ok:
+        if not workchain.is_finished_ok:
             self.report(
-                'ProjwfcCalculation failed with exit status {}'.format(
-                    calculation.exit_status
-                )
+                f"{workchain.process_label} failed with exit status {workchain.exit_status}"
             )
             return self.exit_codes.ERROR_SUB_PROCESS_FAILED_PROJWFC
 
-        self.ctx.current_folder = calculation.outputs.remote_folder
-        self.report("projwfc ProjwfcCalculation successfully finished")
+    def prepare_wannier90_pp_inputs(self):  # pylint: disable=too-many-statements
+        """Prepare the inputs of wannier90 calculation before submission.
 
-    def run_wannier90_pp(self):
-        """The input of wannier90 calculation is build here.
-        
-        :return: [description]
-        :rtype: [type]
+        This method will be called by the workchain at runtime, to fill some parameters such as
+        Fermi energy which can only be retrieved after scf step.
+        Moreover, this allows overriding the method in derived classes to further modify the inputs.
         """
-        inputs = AttributeDict(
-            self.exposed_inputs(Wannier90Calculation, namespace='wannier90')
+        from aiida_wannier90_workflows.utils.workflows.pw import (
+            get_fermi_energy,
+            get_fermi_energy_from_nscf,
+        )
+
+        base_inputs = AttributeDict(
+            self.exposed_inputs(Wannier90BaseWorkChain, namespace="wannier90")
         )
+        inputs = base_inputs["wannier90"]
         inputs.structure = self.ctx.current_structure
         parameters = inputs.parameters.get_dict()
 
-        # get nscf kmesh
-        inputs.kpoints = self.ctx.workchain_nscf.inputs.kpoints
-        # the input kpoints of nscf is an explicitly generated list of kpoints,
-        # we mush retrieve the original kmesh, and explicitly set w90 mp_grid keyword
-        parameters['mp_grid'] = self.ctx.nscf_kmesh.get_kpoints_mesh()[0]
-
-        # check num_bands, exclude_bands, nscf nbnd
-        nbnd = self.ctx.workchain_nscf.outputs.output_parameters.get_dict(
-        )['number_of_bands']
-        num_ex_bands = len(get_exclude_bands(inputs.parameters.get_dict()))
-        parameters['num_bands'] = nbnd - num_ex_bands
-
-        # set num_wann for auto_projections
-        if self.ctx.auto_projections:
-            if self.inputs.only_valence:
-                parameters['num_wann'] = parameters['num_bands']
-                inputs.parameters = orm.Dict(dict=parameters)
-            else:
-                inputs.parameters = orm.Dict(dict=parameters)
-                inputs.parameters = update_w90_params_numwann(
-                    inputs.parameters,
-                    self.ctx.calc_projwfc.outputs.projections
-                )
-                self.report(
-                    'number of Wannier functions extracted from projections: '
-                    + str(inputs.parameters['num_wann'])
-                )
+        # Add Fermi energy
+        if "workchain_scf" in self.ctx:
+            scf_output_parameters = self.ctx.workchain_scf.outputs.output_parameters
+            fermi_energy = get_fermi_energy(scf_output_parameters)
+        elif "workchain_nscf" in self.ctx:
+            fermi_energy = get_fermi_energy_from_nscf(self.ctx.workchain_nscf)
+        else:
+            raise ValueError("Cannot retrieve Fermi energy from scf or nscf output")
+        parameters["fermi_energy"] = fermi_energy
 
-        # get scf Fermi energy
-        try:
-            energies_relative_to_fermi = self.inputs.get(
-                'wannier_energies_relative_to_fermi'
-            )
-            inputs.parameters = update_w90_params_fermi(
-                inputs.parameters,
-                self.ctx.workchain_scf.outputs.output_parameters,
-                energies_relative_to_fermi
-            )
-        except TypeError:
-            self.report(
-                "Error in retriving the SCF Fermi energy "
-                "from pk: {}".format(self.ctx.workchain_scf)
-            )
-            return self.exit_codes.ERROR_SUB_PROCESS_FAILED_WANNIER90PP
+        inputs.parameters = orm.Dict(parameters)
 
-        #Check if settings is given in input
-        try:
-            settings = inputs['settings'].get_dict()
-        except KeyError:
+        # Add `postproc_setup`
+        if "settings" in inputs:
+            settings = inputs["settings"].get_dict()
+        else:
             settings = {}
-        settings['postproc_setup'] = True
-        inputs['settings'] = settings
+        settings["postproc_setup"] = True
+        inputs["settings"] = settings
 
-        inputs = prepare_process_inputs(Wannier90Calculation, inputs)
-        running = self.submit(Wannier90Calculation, **inputs)
+        # I should not stash files in postproc, otherwise there is a RemoteStashFolderData in outputs
+        inputs["metadata"]["options"].pop("stash", None)
 
-        self.report(
-            'wannier90 postproc step - launching Wannier90Calculation<{}> in postproc mode'
-            .format(running.pk)
-        )
+        base_inputs["wannier90"] = inputs
+
+        if base_inputs["shift_energy_windows"] and "bands" not in base_inputs:
+            if "workchain_scf" in self.ctx:
+                output_band = self.ctx.workchain_scf.outputs.output_band
+            elif "workchain_nscf" in self.ctx:
+                output_band = self.ctx.workchain_nscf.outputs.output_band
+            else:
+                raise ValueError("No output scf or nscf bands")
+            base_inputs.bands = output_band
 
-        return ToContext(calc_wannier90_pp=running)
+        if base_inputs["auto_energy_windows"]:
+            if "bands" not in base_inputs:
+                base_inputs.bands = self.ctx.workchain_projwfc.outputs.bands
+            if "bands_projections" not in base_inputs:
+                base_inputs.bands_projections = (
+                    self.ctx.workchain_projwfc.outputs.projections
+                )
+
+        base_inputs["clean_workdir"] = orm.Bool(False)
 
-    def inspect_wannier90_pp(self):
-        """Verify that the Wannier90Calculation for the wannier90 run successfully finished."""
-        workchain = self.ctx.calc_wannier90_pp
+        return base_inputs
+
+    def run_wannier90_pp(self):
+        """Wannier90 post processing step."""
+        inputs = self.prepare_wannier90_pp_inputs()
+        inputs["metadata"] = {"call_link_label": "wannier90_pp"}
+
+        inputs = prepare_process_inputs(Wannier90BaseWorkChain, inputs)
+        running = self.submit(Wannier90BaseWorkChain, **inputs)
+        self.report(f"launching {running.process_label}<{running.pk}> in postproc mode")
+
+        return ToContext(workchain_wannier90_pp=running)
+
+    def inspect_wannier90_pp(self):  # pylint: disable=inconsistent-return-statements
+        """Verify that the `Wannier90Calculation` for the wannier90 run successfully finished."""
+        workchain = self.ctx.workchain_wannier90_pp
 
         if not workchain.is_finished_ok:
             self.report(
-                'wannier90 postproc Wannier90Calculation failed with exit status {}'
-                .format(workchain.exit_status)
+                f"wannier90 postproc {workchain.process_label} failed with exit status {workchain.exit_status}"
             )
             return self.exit_codes.ERROR_SUB_PROCESS_FAILED_WANNIER90PP
 
-        self.ctx.current_folder = workchain.outputs.remote_folder
-        self.report(
-            "wannier90 postproc Wannier90Calculation successfully finished"
+    def prepare_pw2wannier90_inputs(self):
+        """Prepare the inputs of `Pw2wannier90BaseWorkChain` before submission.
+
+        This method will be called by the workchain at runtime, so it can dynamically add/modify inputs
+        based on outputs of previous calculations, e.g. add bands and projections for calculating
+        scdm_mu/sigma from projectability, etc.
+        Moreover, it can be overridden in derived classes.
+        """
+        base_inputs = AttributeDict(
+            self.exposed_inputs(Pw2wannier90BaseWorkChain, namespace="pw2wannier90")
         )
+        inputs = base_inputs["pw2wannier90"]
+        parameters = inputs.parameters.get_dict().get("inputpp", {})
 
-    def run_pw2wannier90(self):
-        inputs = AttributeDict(
-            self.exposed_inputs(
-                Pw2wannier90Calculation, namespace='pw2wannier90'
-            )
+        scdm_proj = parameters.get("scdm_proj", False)
+        scdm_entanglement = parameters.get("scdm_entanglement", None)
+        scdm_mu = parameters.get("scdm_mu", None)
+        scdm_sigma = parameters.get("scdm_sigma", None)
+
+        fit_scdm = (
+            scdm_proj
+            and scdm_entanglement == "erfc"
+            and (scdm_mu is None or scdm_sigma is None)
         )
 
-        try:
-            remote_folder = self.ctx.workchain_nscf.outputs.remote_folder
-        except AttributeError:
-            return self.exit_codes.ERROR_SUB_PROCESS_FAILED_PW2WANNIER90(
-                'the nscf WorkChain did not output a remote_folder node'
-            )
+        if fit_scdm:
+            if "workchain_projwfc" not in self.ctx:
+                raise ValueError("Needs to run projwfc for SCDM projection")
+            base_inputs["bands"] = self.ctx.workchain_projwfc.outputs.bands
+            base_inputs[
+                "bands_projections"
+            ] = self.ctx.workchain_projwfc.outputs.projections
 
-        inputs['parent_folder'] = remote_folder
-        inputs['nnkp_file'] = self.ctx.calc_wannier90_pp.outputs.nnkp_file
-        inputs.parameters = inputs.parameters.get_dict()
-        inputs.parameters['inputpp'].update({
-            'write_mmn': True,
-            'write_amn': True,
-        })
+        inputs["parent_folder"] = self.ctx.current_folder
+        inputs["nnkp_file"] = self.ctx.workchain_wannier90_pp.outputs.nnkp_file
 
-        if self.ctx.auto_projections:
-            inputs.parameters['inputpp']['scdm_proj'] = True
+        base_inputs["pw2wannier90"] = inputs
 
-            # TODO: if exclude_band: gaussian
-            # TODO: auto check if is insulator?
-            if self.inputs.only_valence:
-                inputs.parameters['inputpp']['scdm_entanglement'] = 'isolated'
-            else:
-                inputs.parameters['inputpp']['scdm_entanglement'] = 'erfc'
-                try:
-                    inputs.parameters = update_pw2wan_params_mu_sigma(
-                        parameters=orm.Dict(dict=inputs.parameters),
-                        wannier_parameters=self.ctx.calc_wannier90_pp.inputs.parameters,
-                        bands=self.ctx.calc_projwfc.outputs.bands,
-                        projections=self.ctx.calc_projwfc.outputs.projections,
-                        thresholds=self.inputs.get('scdm_thresholds')
-                    )
-                except ValueError:
-                    self.report(
-                        'WARNING: update_pw2wan_params_mu_sigma failed!'
-                    )
-                    return self.exit_codes.ERROR_SUB_PROCESS_FAILED_PW2WANNIER90
-
-        inputs = prepare_process_inputs(Pw2wannier90Calculation, inputs)
-        running = self.submit(Pw2wannier90Calculation, **inputs)
-
-        self.report(
-            'pw2wannier90 step - launching Pw2Wannier90Calculation<{}>'.format(
-                running.pk
-            )
-        )
-        return ToContext(calc_pw2wannier90=running)
-
-    def inspect_pw2wannier90(self):
-        """Verify that the PwBaseWorkChain for the wannier90 run successfully finished."""
-        workchain = self.ctx.calc_pw2wannier90
+        return base_inputs
+
+    def run_pw2wannier90(self):
+        """Run the pw2wannier90 step."""
+        inputs = self.prepare_pw2wannier90_inputs()
+        inputs.metadata.call_link_label = "pw2wannier90"
+
+        inputs = prepare_process_inputs(Pw2wannier90BaseWorkChain, inputs)
+        running = self.submit(Pw2wannier90BaseWorkChain, **inputs)
+        self.report(f"launching {running.process_label}<{running.pk}>")
+
+        return ToContext(workchain_pw2wannier90=running)
+
+    def inspect_pw2wannier90(self):  # pylint: disable=inconsistent-return-statements
+        """Verify that the Pw2wannier90BaseWorkChain for the pw2wannier90 run successfully finished."""
+        workchain = self.ctx.workchain_pw2wannier90
 
         if not workchain.is_finished_ok:
             self.report(
-                'Pw2wannier90Calculation failed with exit status {}'.format(
-                    workchain.exit_status
-                )
+                f"{workchain.process_label} failed with exit status {workchain.exit_status}"
             )
             return self.exit_codes.ERROR_SUB_PROCESS_FAILED_PW2WANNIER90
 
         self.ctx.current_folder = workchain.outputs.remote_folder
-        self.report("Pw2wannier90Calculation successfully finished")
 
-    def run_wannier90(self):
-        try:
-            remote_folder = self.ctx.calc_pw2wannier90.outputs.remote_folder
-        except AttributeError:
-            self.report(
-                'the Pw2wannier90Calculation did not output a remote_folder node'
-            )
-            return self.exit_codes.ERROR_SUB_PROCESS_FAILED_WANNIER90
+    def prepare_wannier90_inputs(self):  # pylint: disable=too-many-statements
+        """Prepare the inputs of wannier90 calculation before submission.
 
-        # we need metadata in exposed_inputs
-        inputs = AttributeDict(
-            self.exposed_inputs(Wannier90Calculation, namespace='wannier90')
+        This method will be called by the workchain at runtime, to fill some parameters such as
+        Fermi energy which can only be retrieved after scf step.
+        Moreover, this allows overriding the method in derived classes to further modify the inputs.
+        """
+        from copy import deepcopy
+
+        from aiida_wannier90_workflows.utils.workflows import get_last_calcjob
+
+        base_inputs = AttributeDict(
+            self.exposed_inputs(Wannier90BaseWorkChain, namespace="wannier90")
         )
-        pp_inputs = self.ctx.calc_wannier90_pp.inputs
-        pp_keys = [
-            'code', 'parameters', 'kpoint_path', 'structure', 'kpoints',
-            'settings'
-        ]
-        for key in pp_keys:
-            inputs[key] = pp_inputs[key]
 
-        inputs['remote_input_folder'] = remote_folder
+        # I need to disable Fermi energy shifting since this is done in postproc step,
+        # otherwise it will be shifted twice!
+        base_inputs.pop("shift_energy_windows", None)
+        base_inputs.pop("auto_energy_windows", None)
+        base_inputs.pop("auto_energy_windows_threshold", None)
+        base_inputs.pop("bands", None)
+        base_inputs.pop("bands_projections", None)
+
+        inputs = base_inputs["wannier90"]
+
+        # I should stash files, which was removed from metadata in the postproc step
+        stash = None
+        if "stash" in inputs["metadata"]["options"]:
+            stash = deepcopy(inputs["metadata"]["options"]["stash"])
+
+        # Use the Wannier90BaseWorkChain-corrected parameters
+        last_calc = get_last_calcjob(self.ctx.workchain_wannier90_pp)
+        # copy postproc inputs, especially the `kmesh_tol` might have been corrected
+        for key in last_calc.inputs:
+            inputs[key] = last_calc.inputs[key]
+
+        inputs["remote_input_folder"] = self.ctx.current_folder
+
+        if "settings" in inputs:
+            settings = inputs.settings.get_dict()
+        else:
+            settings = {}
+        settings["postproc_setup"] = False
 
-        settings = inputs.settings.get_dict()
-        settings['postproc_setup'] = False
         inputs.settings = settings
 
-        inputs = prepare_process_inputs(Wannier90Calculation, inputs)
-        running = self.submit(Wannier90Calculation, **inputs)
+        # Restore stash files
+        if stash:
+            options = deepcopy(inputs["metadata"]["options"])
+            options["stash"] = stash
+            inputs["metadata"]["options"] = options
 
-        self.report(
-            'wannier90 step - launching Wannier90Calculation<{}>'.format(
-                running.pk
-            )
-        )
+        base_inputs["wannier90"] = inputs
+        base_inputs["clean_workdir"] = orm.Bool(False)
 
-        return ToContext(calc_wannier90=running)
+        return base_inputs
 
-    def inspect_wannier90(self):
-        """Verify that the PwBaseWorkChain for the wannier90 run successfully finished."""
-        workchain = self.ctx.calc_wannier90
+    def run_wannier90(self):
+        """Wannier90 step for MLWF."""
+        inputs = self.prepare_wannier90_inputs()
+        inputs["metadata"] = {"call_link_label": "wannier90"}
+
+        inputs = prepare_process_inputs(Wannier90BaseWorkChain, inputs)
+        running = self.submit(Wannier90BaseWorkChain, **inputs)
+        self.report(f"launching {running.process_label}<{running.pk}>")
+
+        return ToContext(workchain_wannier90=running)
+
+    def inspect_wannier90(self):  # pylint: disable=inconsistent-return-statements
+        """Verify that the `Wannier90BaseWorkChain` for the wannier90 run successfully finished."""
+        workchain = self.ctx.workchain_wannier90
 
         if not workchain.is_finished_ok:
             self.report(
-                'Wannier90Calculation failed with exit status {}'.format(
-                    workchain.exit_status
-                )
+                f"{workchain.process_label} failed with exit status {workchain.exit_status}"
             )
             return self.exit_codes.ERROR_SUB_PROCESS_FAILED_WANNIER90
 
-        self.report("Wannier90Calculation successfully finished")
         self.ctx.current_folder = workchain.outputs.remote_folder
 
-    # def run_bands(self):  # pylint: disable=inconsistent-return-statements
-    #     """
-    #     Run the PwBaseWorkChain to run a bands PwCalculation
-    #     """
-    #     try:
-    #         remote_folder = self.ctx.workchain_scf.out.remote_folder
-    #     except AttributeError:
-    #         self.abort_nowait(
-    #             'the scf workchain did not output a remote_folder node')
-    #         return
-
-    #     inputs = dict(self.ctx.inputs)
-    #     structure = self.ctx.structure_relaxed_primitive
-    #     restart_mode = 'restart'
-    #     calculation_mode = 'bands'
-
-    #     # Set the correct pw.x input parameters
-    #     inputs['parameters']['CONTROL']['restart_mode'] = restart_mode
-    #     inputs['parameters']['CONTROL']['calculation'] = calculation_mode
-
-    #     # Tell the plugin to retrieve the bands
-    #     settings = inputs['settings'].get_dict()
-    #     settings['also_bands'] = True
-
-    #     # Final input preparation, wrapping dictionaries in Dict nodes
-    #     inputs['kpoints'] = self.ctx.kpoints_path
-    #     inputs['structure'] = structure
-    #     inputs['parent_folder'] = remote_folder
-    #     inputs['parameters'] = Dict(dict=inputs['parameters'])
-    #     inputs['settings'] = Dict(dict=settings)
-    #     inputs['pseudo_family'] = self.inputs.pseudo_family
-
-    #     running = submit(PwBaseWorkChain, **inputs)
-
-    #     self.report('launching PwBaseWorkChain<{}> in {} mode'.format(
-    #         running.pk, calculation_mode))
-
-    #     return ToContext(workchain_bands=running)
+    def results(self):  # pylint: disable=inconsistent-return-statements
+        """Attach the desired output nodes directly as outputs of the workchain."""
 
-    def results(self):
-        """
-        Attach the desired output nodes directly as outputs of the workchain
-        """
-        self.report('final step - preparing outputs')
-        try:
-            self.ctx.workchain_relax
-        except AttributeError:
-            pass
-        else:
+        if "workchain_scf" in self.ctx:
             self.out_many(
                 self.exposed_outputs(
-                    self.ctx.workchain_relax,
-                    PwRelaxWorkChain,
-                    namespace='relax'
+                    self.ctx.workchain_scf, PwBaseWorkChain, namespace="scf"
                 )
             )
-        self.out_many(
-            self.exposed_outputs(
-                self.ctx.workchain_scf, PwBaseWorkChain, namespace='scf'
-            )
-        )
-        self.out_many(
-            self.exposed_outputs(
-                self.ctx.workchain_nscf, PwBaseWorkChain, namespace='nscf'
+
+        if "workchain_nscf" in self.ctx:
+            self.out_many(
+                self.exposed_outputs(
+                    self.ctx.workchain_nscf, PwBaseWorkChain, namespace="nscf"
+                )
             )
-        )
-        try:
-            self.ctx.calc_projwfc
-        except AttributeError:
-            pass
-        else:
+
+        if "workchain_projwfc" in self.ctx:
             self.out_many(
                 self.exposed_outputs(
-                    self.ctx.calc_projwfc,
-                    ProjwfcCalculation,
-                    namespace='projwfc'
+                    self.ctx.workchain_projwfc,
+                    ProjwfcBaseWorkChain,
+                    namespace="projwfc",
                 )
             )
+
         self.out_many(
             self.exposed_outputs(
-                self.ctx.calc_pw2wannier90,
-                Pw2wannier90Calculation,
-                namespace='pw2wannier90'
+                self.ctx.workchain_pw2wannier90,
+                Pw2wannier90BaseWorkChain,
+                namespace="pw2wannier90",
             )
         )
         self.out_many(
             self.exposed_outputs(
-                self.ctx.calc_wannier90_pp,
-                Wannier90Calculation,
-                namespace='wannier90_pp'
+                self.ctx.workchain_wannier90_pp,
+                Wannier90BaseWorkChain,
+                namespace="wannier90_pp",
             )
         )
         self.out_many(
             self.exposed_outputs(
-                self.ctx.calc_wannier90,
-                Wannier90Calculation,
-                namespace='wannier90'
-            )
-        )
-        self.report('Wannier90WorkChain successfully completed')
-
-
-@calcfunction
-def convert_kpoints_mesh_to_list(kmesh):
-    """works just like kmesh.pl in Wannier90
-    
-    :param kmesh: [description]
-    :type kmesh: KpointsData
-    :raises ValueError: [description]
-    :return: [description]
-    :rtype: [type]
-    """
-    import numpy as np
-    try:  # test if it is a mesh
-        results = kmesh.get_kpoints_mesh()
-    except AttributeError:
-        try:
-            kmesh.get_kpoints()
-        except AttributeError as e:  # an empty input
-            e.args = ('input kmesh is empty!', )
-            raise e
-        else:
-            return kmesh
-    else:
-        # currently we ignore offset
-        mesh = results[0]
-
-        # following is similar to wannier90/kmesh.pl
-        totpts = np.prod(mesh)
-        weights = np.ones([totpts]) / totpts
-
-        kpoints = np.zeros([totpts, 3])
-        ind = 0
-        for x in range(mesh[0]):
-            for y in range(mesh[1]):
-                for z in range(mesh[2]):
-                    kpoints[ind, :] = [x / mesh[0], y / mesh[1], z / mesh[2]]
-                    ind += 1
-        klist = orm.KpointsData()
-        klist.set_kpoints(kpoints=kpoints, cartesian=False, weights=weights)
-        return klist
-
-
-@calcfunction
-def update_nscf_num_bands(
-    nscf_input_parameters, scf_output_parameters, structure, only_valence,
-    **pseudos
-):
-    '''
-    this calcfunction does 2 works:
-        1. calculate nbnd based on scf output_parameters
-        2. calculate number of projections based on pseudos
-    The resulting nbnd is the max of the two.
-    '''
-    def get_num_projections_from_pseudos(structure, **pseudos):
-        def get_nprojs_from_upf(upf):
-            upf_name = upf.list_object_names()[0]
-            upf_content = upf.get_object_content(upf_name)
-            upf_content = upf_content.split('\n')
-            # get PP_PSWFC block
-            pswfc_block = ''
-            found_begin = False
-            found_end = False
-            for line in upf_content:
-                if 'PP_PSWFC' in line:
-                    pswfc_block += line + '\n'
-                    if not found_begin:
-                        found_begin = True
-                        continue
-                    else:
-                        if not found_end:
-                            found_end = True
-                            break
-                if found_begin:
-                    pswfc_block += line + '\n'
-
-            num_projections = 0
-            # parse XML
-            import xml.etree.ElementTree as ET
-            PP_PSWFC = ET.XML(pswfc_block)
-            if len(PP_PSWFC.getchildren()) == 0:
-                # old upf format
-                import re
-                r = re.compile(r'[\d]([SPDF])')
-                spdf = r.findall(PP_PSWFC.text)
-                for orbit in spdf:
-                    orbit = orbit.lower()
-                    if orbit == 's':
-                        l = 0
-                    elif orbit == 'p':
-                        l = 1
-                    elif orbit == 'd':
-                        l = 2
-                    elif orbit == 'f':
-                        l = 3
-                    num_projections += 2 * l + 1
-            else:
-                # upf format 2.0.1
-                for child in PP_PSWFC:
-                    l = int(child.get('l'))
-                    num_projections += 2 * l + 1
-            return num_projections
-
-        tot_nprojs = 0
-        composition = structure.get_composition()
-        for kind in pseudos:
-            upf = pseudos[kind]
-            nprojs = get_nprojs_from_upf(upf)
-            tot_nprojs += nprojs * composition[kind]
-        return tot_nprojs
-
-    # Get info from SCF on number of electrons and number of spin components
-    scf_out_dict = scf_output_parameters.get_dict()
-    nelectron = int(scf_out_dict['number_of_electrons'])
-    nspin = int(scf_out_dict['number_of_spin_components'])
-    if only_valence:
-        nbands = int(nelectron / 2)
-    else:
-        nbands = int(0.5 * nelectron * nspin + 4 * nspin)
-        # nbands must > num_projections = num_wann
-        nprojs = get_num_projections_from_pseudos(structure, **pseudos)
-        nbands = max(nbands, nprojs + 10)
-    nscf_in_dict = nscf_input_parameters.get_dict()
-    nscf_in_dict['SYSTEM']['nbnd'] = nbands
-    return orm.Dict(dict=nscf_in_dict)
-
-
-def get_exclude_bands(parameters):
-    """get exclude_bands from Wannier90 parameters
-    
-    :param parameters: Wannier90Calculation input parameters
-    :type parameters: dict, NOT Dict, this is not a calcfunction
-    :return: the indices of the bands to be excluded
-    :rtype: list
-    """
-    exclude_bands = parameters.get('exclude_bands', [])
-    return exclude_bands
+                self.ctx.workchain_wannier90,
+                Wannier90BaseWorkChain,
+                namespace="wannier90",
+            )
+        )
 
+        result = self.sanity_check()
+        if result:
+            return result
 
-def get_keep_bands(parameters):
-    """get keep_bands from Wannier90 parameters
-    
-    :param parameters: Wannier90Calculation input parameters
-    :type parameters: dict, NOT Dict, this is not a calcfunction
-    :return: the indices of the bands to be kept
-    :rtype: list
-    """
-    import numpy as np
-    exclude_bands = get_exclude_bands(parameters)
-    xb_startzero_set = set([idx - 1 for idx in exclude_bands]
-                           )  # in Fortran/W90: 1-based; in py: 0-based
-    keep_bands = np.array([
-        idx for idx in range(parameters['num_bands'] + len(exclude_bands))
-        if idx not in xb_startzero_set
-    ])
-    return keep_bands
+        self.report(f"{self.get_name()} successfully completed")
 
+    def sanity_check(self):  # pylint: disable=inconsistent-return-statements
+        """Sanity checks for final outputs.
 
-@calcfunction
-def update_w90_params_fermi(
-    parameters, scf_output_parameters, relative_to_fermi
-):
-    """
-    Updated W90 windows with the specified Fermi energy.
-    
-    :param parameters: Wannier90Calculation input parameters
-    :type parameters: Dict
-    :param fermi_energy: [description]
-    :type fermi_energy: Float
-    :param relative_to_fermi: if energies in input parameters are defined relative 
-    scf Fermi energy.
-    :type relative_to_fermi: Bool
-    :return: updated parameters
-    :rtype: Dict
-    """
-    def get_fermi_energy():
-        """get Fermi energy from scf output parameters, unit is eV
+        Not necessary but it is good to check it.
         """
-        try:
-            scf_out_dict = scf_output_parameters.get_dict()
-            efermi = scf_out_dict['fermi_energy']
-            efermi_units = scf_out_dict['fermi_energy_units']
-            if efermi_units != 'eV':
-                raise TypeError(
-                    "Error: Fermi energy is not in eV!"
-                    "it is {}".format(efermi_units)
-                )
-        except AttributeError:
-            raise TypeError(
-                "Error in retriving the SCF Fermi energy from pk: {}".format(
-                    scf_output_parameters.pk
+        from aiida_wannier90_workflows.utils.pseudo import (
+            get_number_of_electrons,
+            get_number_of_projections,
+        )
+
+        # If using external atomic projectors, disable sanity check
+        p2w_params = self.ctx.workchain_pw2wannier90.inputs["pw2wannier90"][
+            "parameters"
+        ].get_dict()["inputpp"]
+        atom_proj = p2w_params.get("atom_proj", False)
+        atom_proj_ext = p2w_params.get("atom_proj_ext", False)
+        if atom_proj and atom_proj_ext:
+            return
+
+        # 1. the calculated number of projections is consistent with QE projwfc.x
+        if "scf" in self.inputs:
+            pseudos = self.inputs["scf"]["pw"]["pseudos"]
+        else:
+            pseudos = self.inputs["nscf"]["pw"]["pseudos"]
+        args = {
+            "structure": self.ctx.current_structure,
+            # The type of `self.inputs['scf']['pw']['pseudos']` is AttributesFrozendict,
+            # we need to convert it to dict, otherwise get_number_of_projections will fail.
+            "pseudos": dict(pseudos),
+        }
+        if "workchain_projwfc" in self.ctx:
+            num_proj = len(
+                self.ctx.workchain_projwfc.outputs["projections"].get_orbitals()
+            )
+            params = self.ctx.workchain_wannier90.inputs["wannier90"][
+                "parameters"
+            ].get_dict()
+            spin_orbit_coupling = params.get("spinors", False)
+            number_of_projections = get_number_of_projections(
+                **args, spin_orbit_coupling=spin_orbit_coupling
+            )
+            if number_of_projections != num_proj:
+                self.report(
+                    f"number of projections {number_of_projections} != projwfc.x output {num_proj}"
                 )
+                return self.exit_codes.ERROR_SANITY_CHECK_FAILED
+
+        # 2. the number of electrons is consistent with QE output
+        if "workchain_scf" in self.ctx:
+            num_elec = self.ctx.workchain_scf.outputs["output_parameters"][
+                "number_of_electrons"
+            ]
+        else:
+            num_elec = self.ctx.workchain_nscf.outputs["output_parameters"][
+                "number_of_electrons"
+            ]
+        number_of_electrons = get_number_of_electrons(**args)
+        if number_of_electrons != num_elec:
+            self.report(
+                f"number of electrons {number_of_electrons} != QE output {num_elec}"
             )
-        return efermi
+            return self.exit_codes.ERROR_SANITY_CHECK_FAILED
 
-    params = parameters.get_dict()
-    fermi = get_fermi_energy()
-    params['fermi_energy'] = fermi
-
-    if relative_to_fermi:
-        try:
-            dwmax = params['dis_win_max']
-            dwmax += fermi
-            params['dis_win_max'] = dwmax
-        except KeyError:
-            pass
-        try:
-            dfmax = params['dis_froz_max']
-            dfmax += fermi
-            params['dis_froz_max'] = dfmax
-        except KeyError:
-            pass
-        try:
-            dwmin = params['dis_win_min']
-            dwmin += fermi
-            params['dis_win_min'] = dwmin
-        except KeyError:
-            pass
-        try:
-            dfmin = params['dis_froz_min']
-            dfmin += fermi
-            params['dis_froz_min'] = dfmin
-        except KeyError:
-            pass
-    return orm.Dict(dict=params)
-
-
-@calcfunction
-def update_w90_params_numwann(parameters, projections):
-    def get_numwann_from_projections():
-        """
-        Calculate num_wann from projections, also consider exclude_bands
-        :param
-        :return:
-        """
-        num_wann = len(projections.get_orbitals())
-        num_wann -= len(get_exclude_bands(parameters.get_dict()))
-        return num_wann
-
-    parameters_dict = parameters.get_dict()
-    parameters_dict['num_wann'] = get_numwann_from_projections()
-    return orm.Dict(dict=parameters_dict)
+    def on_terminated(self):
+        """Clean the working directories of all child calculations if `clean_workdir=True` in the inputs."""
+        super().on_terminated()
 
+        if not self.inputs.clean_workdir:
+            self.report("remote folders will not be cleaned")
+            return
 
-@calcfunction
-def update_pw2wan_params_mu_sigma(
-    parameters, wannier_parameters, bands, projections, thresholds
-):
-    """[summary]
-    
-    :param pw2wan_parameters: [description]
-    :type pw2wan_parameters: Dict
-    :param mu_sigma: [description]
-    :type mu_sigma: Dict
-    :return: [description]
-    :rtype: Dict
-    """
-    def get_mu_and_sigma_from_projections(
-        wannier_parameters,
-        bands,
-        projections,  # pylint: disable=too-many-locals
-        thresholds
-    ):
-        '''
-        Setting mu parameter for the SCDM-k method:
-        The projectability of all orbitals is fitted using an erfc(x)
-        function. Mu and sigma are extracted from the fitted distribution,
-        with mu = mu_fit - k * sigma, sigma = sigma_fit and
-        k a parameter with default k = 3.
-
-        :param bands: output of projwfc, it was computed in the nscf calc
-        :param parameters: wannier90 input params (the one to update with this calcfunction)
-        :param projections: output of projwfc
-        :param thresholds: must contain 'sigma_factor'; scdm_mu will be set to::
-            scdm_mu = E(projectability==max_projectability) - sigma_factor * scdm_sigma
-            Pass sigma_factor = 0 if you do not want to shift
-        :return: a modified Dict in output_parameters, with the proper value for scdm_mu set,
-                and a Bool called 'success' that tells if the algorithm could find the energy at which
-                the required projectability is achieved.
-        '''
-        def erfc_scdm(x, mu, sigma):
-            from scipy.special import erfc  # pylint: disable=E0611
-            return 0.5 * erfc((x - mu) / sigma)
-
-        def fit_erfc(f, xdata, ydata):
-            from scipy.optimize import curve_fit
-            return curve_fit(f, xdata, ydata, bounds=([-50, 0], [50, 50]))
-
-        # List of specifications of atomic orbitals in dictionary form
-        dict_list = [i.get_orbital_dict() for i in projections.get_orbitals()]
-
-        keep_bands = get_keep_bands(wannier_parameters.get_dict())
-        # Sum of the projections on all atomic orbitals (shape kpoints x nbands)
-        # WITHOUT EXCLUDE BANDS out_array = sum([sum([x[1] for x in projections.get_projections(
-        #    **get_dict)]) for get_dict in dict_list])
-        out_array = sum([
-            sum([
-                x[1][:, keep_bands]
-                for x in projections.get_projections(**get_dict)
-            ]) for get_dict in dict_list
-        ])
-
-        # Flattening (projection modulus squared according to QE, energies)
-        projwfc_flat, bands_flat = out_array.flatten(), bands.get_bands(
-        )[:, keep_bands].flatten()
-        # Sorted by energy
-        sorted_bands, sorted_projwfc = zip(
-            *sorted(zip(bands_flat, projwfc_flat))
-        )
-        popt, pcov = fit_erfc(erfc_scdm, sorted_bands, sorted_projwfc)
-        mu = popt[0]
-        sigma = popt[1]
-        # Temporary, TODO add check on interpolation
-        success = True
-        params = {}
-        params['scdm_sigma'] = sigma
-        sigma_factor = thresholds.get_dict().get('sigma_factor', 3)
-        params['scdm_mu'] = mu - sigma * sigma_factor
-        result = {
-            'success': orm.Bool(success),
-            'scdm_parameters': orm.Dict(dict=params)
-        }
-        return result
+        cleaned_calcs = []
+
+        for called_descendant in self.node.called_descendants:
+            if isinstance(called_descendant, orm.CalcJobNode):
+                try:
+                    called_descendant.outputs.remote_folder._clean()  # pylint: disable=protected-access
+                    cleaned_calcs.append(called_descendant.pk)
+                except (OSError, KeyError):
+                    pass
 
-    results = get_mu_and_sigma_from_projections(
-        wannier_parameters, bands, projections, thresholds
-    )
-    if not results['success']:
-        raise ValueError('mu and sigma failed')
-    parameters_dict = parameters.get_dict()
-    parameters_dict['inputpp'].update(results['scdm_parameters'].get_dict())
-    return orm.Dict(dict=parameters_dict)
+        if cleaned_calcs:
+            self.report(
+                f"cleaned remote folders of calculations: {' '.join(map(str, cleaned_calcs))}"
+            )
```

